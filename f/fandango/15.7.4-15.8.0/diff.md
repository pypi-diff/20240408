# Comparing `tmp/fandango-15.7.4.tar.gz` & `tmp/fandango-15.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fandango-15.7.4.tar", last modified: Fri Dec  1 15:31:01 2023, max compression
+gzip compressed data, was "fandango-15.8.0.tar", last modified: Mon Apr  8 14:25:09 2024, max compression
```

## Comparing `fandango-15.7.4.tar` & `fandango-15.8.0.tar`

### file list

```diff
@@ -1,100 +1,102 @@
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-01 15:31:01.240981 fandango-15.7.4/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      556 2022-05-25 08:42:07.000000 fandango-15.7.4/AUTHORS
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     3691 2022-05-25 08:42:07.000000 fandango-15.7.4/LICENSE
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      106 2022-05-25 08:42:07.000000 fandango-15.7.4/MANIFEST.in
--rw-r--r--   0 srubio    (1206) Control   (1200)     1272 2023-12-01 15:31:01.241997 fandango-15.7.4/PKG-INFO
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    12517 2023-07-06 07:51:28.000000 fandango-15.7.4/README.md
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-01 15:31:00.494958 fandango-15.7.4/fandango/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    52702 2022-05-25 08:42:07.000000 fandango-15.7.4/fandango/CHANGELOG
--rwxr-xr-x   0 srubio    (1206) Control   (1200)        7 2023-12-01 15:29:13.000000 fandango-15.7.4/fandango/VERSION
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     9281 2023-10-23 11:33:21.000000 fandango-15.7.4/fandango/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    58353 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/arrays.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    79455 2023-11-08 21:04:30.000000 fandango-15.7.4/fandango/callbacks.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    19336 2023-10-23 11:33:21.000000 fandango-15.7.4/fandango/db.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2702 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/debug.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-01 15:31:00.536962 fandango-15.7.4/fandango/device/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     3760 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/device/DDebug.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    27004 2023-10-23 11:33:21.000000 fandango-15.7.4/fandango/device/Dev4Tango.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      238 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/device/DynamicDS.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    16925 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/device/FolderDS.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     3630 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/device/FolderGUI.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    19656 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/device/WorkerDS.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      503 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/device/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    11697 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/devslist.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    33197 2023-11-08 21:04:30.000000 fandango-15.7.4/fandango/dicts.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     4952 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/doc.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)   144440 2023-12-01 15:13:45.000000 fandango-15.7.4/fandango/dynamic.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    15200 2023-12-01 11:44:32.000000 fandango-15.7.4/fandango/excepts.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    58222 2023-11-24 16:33:50.000000 fandango-15.7.4/fandango/functional.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-01 15:31:00.545957 fandango-15.7.4/fandango/interface/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    11571 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/interface/CopyCatDS.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      297 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/interface/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     9345 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/interface/inheritance.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    22723 2023-11-14 13:16:54.000000 fandango-15.7.4/fandango/linos.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    19227 2023-11-08 21:04:30.000000 fandango-15.7.4/fandango/log.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    43538 2023-11-27 10:15:29.000000 fandango-15.7.4/fandango/objects.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     3747 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/pipes.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    86406 2023-10-23 11:33:21.000000 fandango-15.7.4/fandango/qt.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-01 15:31:00.563962 fandango-15.7.4/fandango/scripts/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2062 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/CopyCatDS
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     3171 2023-10-23 11:33:21.000000 fandango-15.7.4/fandango/scripts/DynamicDS
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2059 2022-08-29 16:35:46.000000 fandango-15.7.4/fandango/scripts/FolderDS
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2059 2022-08-29 16:35:46.000000 fandango-15.7.4/fandango/scripts/WorkerDS
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      118 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    12037 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/csv2tango
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     8201 2023-11-08 21:04:30.000000 fandango-15.7.4/fandango/scripts/fandango
--rwxr-xr-x   0 srubio    (1206) Control   (1200)       93 2022-08-29 16:35:46.000000 fandango-15.7.4/fandango/scripts/folder-gui
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     4788 2023-10-23 11:33:21.000000 fandango-15.7.4/fandango/scripts/my2to3.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     1107 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/sardanact
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    44592 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/servers_lite.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     1944 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/setup.ds.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     7704 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/tango2csv
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     1764 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/tango2json
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      106 2022-08-29 16:35:46.000000 fandango-15.7.4/fandango/scripts/tango_cleanup
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2177 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/tango_create_device.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     4053 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/tango_create_starter.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      321 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/tango_host
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     5291 2023-11-27 13:24:11.000000 fandango-15.7.4/fandango/scripts/tango_monitor
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2800 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/scripts/tango_property
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     5238 2023-11-08 21:04:30.000000 fandango-15.7.4/fandango/scripts/tango_servers
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    48266 2023-11-14 08:14:13.000000 fandango-15.7.4/fandango/servers.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-01 15:31:00.590961 fandango-15.7.4/fandango/tango/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      462 2023-10-23 11:33:21.000000 fandango-15.7.4/fandango/tango/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     9766 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/tango/command.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    24720 2023-11-08 21:05:50.000000 fandango-15.7.4/fandango/tango/defaults.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    26945 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/tango/dynattr.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    13208 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/tango/export.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    57595 2023-11-08 21:04:30.000000 fandango-15.7.4/fandango/tango/methods.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    17047 2023-11-08 21:04:30.000000 fandango-15.7.4/fandango/tango/search.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    28413 2023-11-14 13:16:54.000000 fandango-15.7.4/fandango/tango/tangoeval.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-01 15:31:00.607956 fandango-15.7.4/fandango/testing/
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/testing/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     1254 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/testing/check_callbacks.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2164 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/testing/check_fandango.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     7260 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/testing/checkmodule.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     3598 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/testing/gen_test_file.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     4305 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/testing/simulation.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    70052 2023-12-01 15:07:52.000000 fandango-15.7.4/fandango/threads.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    13096 2023-07-06 07:51:28.000000 fandango-15.7.4/fandango/web.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-01 15:31:00.610958 fandango-15.7.4/fandango/widget/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2022-05-25 08:42:08.000000 fandango-15.7.4/fandango/widget/__init__.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-01 15:31:00.515957 fandango-15.7.4/fandango.egg-info/
--rw-r--r--   0 srubio    (1206) Control   (1200)     1272 2023-12-01 15:30:59.000000 fandango-15.7.4/fandango.egg-info/PKG-INFO
--rw-r--r--   0 srubio    (1206) Control   (1200)     2269 2023-12-01 15:30:59.000000 fandango-15.7.4/fandango.egg-info/SOURCES.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)        1 2023-12-01 15:30:59.000000 fandango-15.7.4/fandango.egg-info/dependency_links.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       20 2023-12-01 15:30:59.000000 fandango-15.7.4/fandango.egg-info/entry_points.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)        1 2022-08-29 16:49:35.000000 fandango-15.7.4/fandango.egg-info/not-zip-safe
--rw-r--r--   0 srubio    (1206) Control   (1200)       62 2023-12-01 15:30:59.000000 fandango-15.7.4/fandango.egg-info/requires.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       15 2023-12-01 15:30:59.000000 fandango-15.7.4/fandango.egg-info/top_level.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       67 2023-12-01 15:31:01.245962 fandango-15.7.4/setup.cfg
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     8046 2023-10-23 11:33:21.000000 fandango-15.7.4/setup.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-01 15:31:01.197956 fandango-15.7.4/tests/
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-07-06 07:51:28.000000 fandango-15.7.4/tests/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    34621 2023-07-06 07:51:28.000000 fandango-15.7.4/tests/definitions.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-01 15:31:01.225967 fandango-15.7.4/tests/dependencies/
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-07-06 07:51:28.000000 fandango-15.7.4/tests/dependencies/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)      175 2023-07-06 07:51:28.000000 fandango-15.7.4/tests/dependencies/dummy_module.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    42849 2023-07-06 07:51:28.000000 fandango-15.7.4/tests/test_functional.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    21320 2023-07-06 07:51:28.000000 fandango-15.7.4/tests/test_functional_auto_gen.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    14830 2023-07-06 07:51:28.000000 fandango-15.7.4/tests/test_functional_skip.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    14133 2023-07-06 07:51:28.000000 fandango-15.7.4/tests/test_objects.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:25:09.431813 fandango-15.8.0/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      556 2023-12-04 12:00:15.000000 fandango-15.8.0/AUTHORS
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     3691 2023-12-04 12:00:15.000000 fandango-15.8.0/LICENSE
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      106 2023-12-04 12:00:15.000000 fandango-15.8.0/MANIFEST.in
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1272 2024-04-08 14:25:09.432805 fandango-15.8.0/PKG-INFO
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    12517 2023-12-04 12:00:15.000000 fandango-15.8.0/README.md
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:25:09.278781 fandango-15.8.0/fandango/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    52702 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/CHANGELOG
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)        7 2024-04-08 14:25:03.000000 fandango-15.8.0/fandango/VERSION
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     9304 2024-02-28 16:07:39.000000 fandango-15.8.0/fandango/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    58349 2024-02-28 16:07:39.000000 fandango-15.8.0/fandango/arrays.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    79430 2024-04-08 14:25:03.000000 fandango-15.8.0/fandango/callbacks.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    19336 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/db.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2702 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/debug.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:25:09.324779 fandango-15.8.0/fandango/device/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     3760 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/device/DDebug.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    27004 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/device/Dev4Tango.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      238 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/device/DynamicDS.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    16925 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/device/FolderDS.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     3630 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/device/FolderGUI.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     5450 2024-02-28 16:07:39.000000 fandango-15.8.0/fandango/device/ScriptDS.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    19656 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/device/WorkerDS.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      503 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/device/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    11697 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/devslist.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    33197 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/dicts.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     4952 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/doc.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)   145112 2024-04-03 15:52:26.000000 fandango-15.8.0/fandango/dynamic.last.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)   145054 2024-04-08 14:25:03.000000 fandango-15.8.0/fandango/dynamic.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    15200 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/excepts.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    58176 2024-04-08 14:25:03.000000 fandango-15.8.0/fandango/functional.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:25:09.334776 fandango-15.8.0/fandango/interface/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    11571 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/interface/CopyCatDS.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      297 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/interface/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     9345 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/interface/inheritance.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    22723 2024-04-08 14:25:03.000000 fandango-15.8.0/fandango/linos.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    19440 2024-02-28 16:07:39.000000 fandango-15.8.0/fandango/log.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    43784 2024-03-04 11:28:57.000000 fandango-15.8.0/fandango/objects.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     3747 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/pipes.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    86406 2024-04-08 14:25:03.000000 fandango-15.8.0/fandango/qt.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:25:09.352788 fandango-15.8.0/fandango/scripts/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2062 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/scripts/CopyCatDS
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     3171 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/scripts/DynamicDS
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2059 2022-08-29 16:35:46.000000 fandango-15.8.0/fandango/scripts/FolderDS
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2059 2022-08-29 16:35:46.000000 fandango-15.8.0/fandango/scripts/WorkerDS
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      118 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/scripts/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    12037 2023-12-04 12:13:52.000000 fandango-15.8.0/fandango/scripts/csv2tango
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     8201 2023-12-04 12:13:52.000000 fandango-15.8.0/fandango/scripts/fandango
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)       93 2023-12-04 12:13:52.000000 fandango-15.8.0/fandango/scripts/folder-gui
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     4788 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/scripts/my2to3.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1107 2023-12-04 12:13:52.000000 fandango-15.8.0/fandango/scripts/sardanact
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    44592 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/scripts/servers_lite.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1944 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/scripts/setup.ds.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     7704 2023-12-04 12:13:52.000000 fandango-15.8.0/fandango/scripts/tango2csv
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1764 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/scripts/tango2json
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      106 2022-08-29 16:35:46.000000 fandango-15.8.0/fandango/scripts/tango_cleanup
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2177 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/scripts/tango_create_device.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     4053 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/scripts/tango_create_starter.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      321 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/scripts/tango_host
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     5291 2023-12-04 12:13:52.000000 fandango-15.8.0/fandango/scripts/tango_monitor
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2800 2023-12-04 12:13:52.000000 fandango-15.8.0/fandango/scripts/tango_property
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     5238 2024-04-08 14:25:03.000000 fandango-15.8.0/fandango/scripts/tango_servers
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    48266 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/servers.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:25:09.380793 fandango-15.8.0/fandango/tango/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      463 2024-02-28 16:07:39.000000 fandango-15.8.0/fandango/tango/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     9766 2024-02-28 16:07:39.000000 fandango-15.8.0/fandango/tango/commands.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    24518 2024-02-28 16:07:39.000000 fandango-15.8.0/fandango/tango/defaults.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    27065 2024-02-28 16:07:39.000000 fandango-15.8.0/fandango/tango/dynattr.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    13208 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/tango/export.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    57751 2024-04-08 14:25:03.000000 fandango-15.8.0/fandango/tango/methods.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    17214 2024-02-28 16:07:39.000000 fandango-15.8.0/fandango/tango/search.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    28413 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/tango/tangoeval.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:25:09.400780 fandango-15.8.0/fandango/testing/
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/testing/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1254 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/testing/check_callbacks.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2164 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/testing/check_fandango.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     7260 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/testing/checkmodule.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     3598 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/testing/gen_test_file.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     4305 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/testing/simulation.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    70434 2024-02-28 16:07:39.000000 fandango-15.8.0/fandango/threads.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    13096 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/web.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:25:09.403805 fandango-15.8.0/fandango/widget/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-12-04 12:00:15.000000 fandango-15.8.0/fandango/widget/__init__.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:25:09.299790 fandango-15.8.0/fandango.egg-info/
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1272 2024-04-08 14:25:09.000000 fandango-15.8.0/fandango.egg-info/PKG-INFO
+-rw-r--r--   0 srubio    (1206) Control   (1200)     2323 2024-04-08 14:25:09.000000 fandango-15.8.0/fandango.egg-info/SOURCES.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)        1 2024-04-08 14:25:09.000000 fandango-15.8.0/fandango.egg-info/dependency_links.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       20 2024-04-08 14:25:09.000000 fandango-15.8.0/fandango.egg-info/entry_points.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)        1 2022-08-29 16:49:35.000000 fandango-15.8.0/fandango.egg-info/not-zip-safe
+-rw-r--r--   0 srubio    (1206) Control   (1200)       62 2024-04-08 14:25:09.000000 fandango-15.8.0/fandango.egg-info/requires.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       15 2024-04-08 14:25:09.000000 fandango-15.8.0/fandango.egg-info/top_level.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       67 2024-04-08 14:25:09.435822 fandango-15.8.0/setup.cfg
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     8046 2023-12-04 12:13:52.000000 fandango-15.8.0/setup.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:25:09.423806 fandango-15.8.0/tests/
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-12-04 12:00:15.000000 fandango-15.8.0/tests/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    34621 2023-12-04 12:00:15.000000 fandango-15.8.0/tests/definitions.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:25:09.429801 fandango-15.8.0/tests/dependencies/
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-12-04 12:00:15.000000 fandango-15.8.0/tests/dependencies/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)      175 2023-12-04 12:00:15.000000 fandango-15.8.0/tests/dependencies/dummy_module.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    42849 2023-12-04 12:00:15.000000 fandango-15.8.0/tests/test_functional.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    21320 2023-12-04 12:00:15.000000 fandango-15.8.0/tests/test_functional_auto_gen.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    14830 2023-12-04 12:00:15.000000 fandango-15.8.0/tests/test_functional_skip.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    14133 2023-12-04 12:00:15.000000 fandango-15.8.0/tests/test_objects.py
```

### Comparing `fandango-15.7.4/AUTHORS` & `fandango-15.8.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/LICENSE` & `fandango-15.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/PKG-INFO` & `fandango-15.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fandango
-Version: 15.7.4
+Version: 15.8.0
 Summary: Simplify the configuration of big Tango control systems
 Home-page: UNKNOWN
 Author: Sergi Rubio
 Author-email: srubio@cells.es
 License: UNKNOWN
 Description: Fandango is a Python module created to simplify the configuration of big control systems; implementing the behavior of Jive (configuration) and/or Astor (deployment) tools in methods that could be called from scripts using regexp and wildcards. Fandango provides functional methods, classes and utilities to develop high-level device servers and APIs for Tango control system.
 Platform: Linux,Windows XP/Vista/7/8
```

### Comparing `fandango-15.7.4/README.md` & `fandango-15.8.0/README.md`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/CHANGELOG` & `fandango-15.8.0/fandango/CHANGELOG`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/__init__.py` & `fandango-15.8.0/fandango/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,16 +120,16 @@
 except Exception as e:
     print(traceback.format_exc())
     print("Unable to load RELEASE number: %s" % e)
     
 if '--mem' in __options__: print('objects',get_mbs())
 
 try:
-    from .log import (printf, Logger, LogFilter, shortstr, except2str, 
-            FakeLogger, pprint, Debugged, InOutLogged, Logged)
+    from .log import (printf, Logger, LogFilter, shortstr, except2str, trace, 
+            FakeLogger, pprint, Debugged, InOutLogged, Logged, tprint, lprint)
 except Exception as e:
     print("Unable to import log module: %s" % e)
 
 if '--mem' in __options__: print('log',get_mbs())
 
 try:
     from .excepts import (
```

### Comparing `fandango-15.7.4/fandango/arrays.py` & `fandango-15.8.0/fandango/arrays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1367,15 +1367,15 @@
                 pass
 
         if readed:
             i, check = 0, True
             for row in readed:
                 # Empty rows are avoided, Row is added only if not commented
                 if (not prune_empty_lines) or (
-                    max([len(el) for el in row] or [0]) is not 0
+                    max([len(el) for el in row] or [0]) != 0
                     and (not comment or not str(row[0]).startswith(comment))
                 ):
                     row2 = [str(r).strip() for r in row]
                     if i == header:
                         headers = [s.lower() for s in row2]
 
                     elif i > header and filters:
```

### Comparing `fandango-15.7.4/fandango/callbacks.py` & `fandango-15.8.0/fandango/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -525,20 +525,18 @@
                     e = events.pop(0)
                     source, args = e
                     if filtered:  # write last read time to all sources
                         sources = self.get_sources(s)  # self.get_source_name(s))
                     else:
                         sources = [source]  # each source should push its own events
                     for source in sources:
-                        if True:
-                            # Update timestamp also for errors
-                            # not filtered in push_event
-                            # redundance needed to avoid overpolling
-                            source.last_read_time = now()
-
+                        # Update timestamp also for errors
+                        # not filtered in push_event
+                        # redundance needed to avoid overpolling
+                        source.last_read_time = now()
                         self.fireEvent(source, *args)
                         self.wait(self.MinWait / 10.0)  # breathing
                 except:
                     self.error("%s:%s\n%s" % (s, e, traceback.format_exc()))
 
         self.wait(1e-6)  # breathing
 
@@ -569,15 +567,15 @@
                         s.polling_period if polled else s.KeepAlive
                     )
                     pollings.append((nxt, s))
 
         for nxt, s in reversed(ksorted(pollings)):
             if t0 > nxt and (s.isPollingActive() or WAS_EMPTY):
                 try:
-                    self.info(
+                    self.debug(
                         "%s.process => checkEvents(%s,%s)"
                         % (self.full_name, s, s.getState())
                     )
                     # Tries to subscribe/updates polling
                     s.checkEvents(tdiff=2e-3 * s.polling_period)
 
                     self.debug(
@@ -1402,15 +1400,15 @@
             vtime = ctime2time(getattr(self.attr_value, "time", None))
             if vtime > t0:
                 vtime = t0  # correct "future" data
             self.debug(str([t0, vtime, self.keep_time * 1e-3]))
             if self.fake or (t0 < (vtime + self.keep_time * 1e-3)):
                 cache = True
             # If not polled, force HW reading
-            elif not self.getMode():
+            elif not self.getMode(): #Not polled, not events
                 cache = False
             else:
                 cache = True
 
         self.debug(
             "read(cache=%s,asynch=%s,threaded=%s)"
             % (cache, asynch, self.get_thread().is_alive())
```

### Comparing `fandango-15.7.4/fandango/db.py` & `fandango-15.8.0/fandango/db.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/debug.py` & `fandango-15.8.0/fandango/debug.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/device/DDebug.py` & `fandango-15.8.0/fandango/device/DDebug.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/device/Dev4Tango.py` & `fandango-15.8.0/fandango/device/Dev4Tango.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/device/FolderDS.py` & `fandango-15.8.0/fandango/device/FolderDS.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/device/FolderGUI.py` & `fandango-15.8.0/fandango/device/FolderGUI.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/device/WorkerDS.py` & `fandango-15.8.0/fandango/device/WorkerDS.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/devslist.py` & `fandango-15.8.0/fandango/devslist.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/dicts.py` & `fandango-15.8.0/fandango/dicts.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/doc.py` & `fandango-15.8.0/fandango/doc.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/dynamic.py` & `fandango-15.8.0/fandango/dynamic.last.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,14 +552,18 @@
                     + str(p)
                     + "="
                     + str(getattr(self, p, None))
                 )
                 for p in config
             ]
 
+        if not self.ReadLocked:
+            # If True, .lock is managed by self_locked decorator
+            self.lock = None
+            
         if self.UseTaurus:
             self.UseTaurus = (ft.TAU or ft.loadTaurus()) and self.UseTaurus
 
         if self.LoadFromFile:
             DynamicDS.load_from_file(device=self)
 
         # Adding Static Attributes if defined in the SubClass
@@ -664,15 +668,15 @@
                     "Removing Attribute %s from %s.polled_attr Property"
                     % (att, my_name)
                 )
                 if use_admin:
                     try:
                         admin.rem_obj_polling([my_name, "attribute", att])
                     except:
-                        print(traceback.format_exc())
+                        self.error(traceback.format_exc())
         # Second: add new attributes to the list of attributes to configure; attributes where value is None will not be polled
         for n, v in new_attr.items():
             if n.lower() not in npattrs and v:
                 (npattrs.append(n.lower()), npattrs.append(v))
                 self.info(
                     "Attribute %s added to %s.polled_attr Property" % (n, my_name)
                 )
@@ -686,16 +690,16 @@
                             [[int(period)], [my_name, "attribute", att]]
                         )
                     else:
                         admin.upd_obj_polling_period(
                             [[int(period)], [my_name, "attribute", att]]
                         )
                 except:
-                    print("Unable to set %s polling" % (npattrs[i]))
-                    print(traceback.format_exc())
+                    self.warning("Unable to set %s polling" % (npattrs[i]))
+                    self.warning(traceback.format_exc())
         else:
             self.info("Updating polled_attr: %s" % (npattrs,))
             self._db.put_device_property(my_name, {"polled_attr": npattrs})
         self.info("Out of check_polled_attributes ...")
 
     def updateDynamicAttributes(self):
         """Forces dynamic attributes update from properties.
@@ -726,15 +730,15 @@
                     self.error("Unable to remove attribute %s: %s" % (a, str(e)))
         DynamicDS.dyn_attr(self)
 
         # Updating DynamicCommands (just update of formulas)
         try:
             CreateDynamicCommands(type(self), type(self.get_device_class()))
         except:
-            print("CreateDynamicCommands failed: %s" % traceback.format_exc())
+            self.error"CreateDynamicCommands failed: %s" % traceback.format_exc())
 
 
 ###############################################################################
 
 
 class DynamicDSAttrs(DynamicDSImpl):
 
@@ -853,17 +857,19 @@
                 if not any(k.lower() == aname.lower() for k in self.dyn_values):
                     create = True
                     self.dyn_values[aname] = DynamicAttribute(name=aname)
                 else:
                     self.info("\tAttribute %s already exists" % (aname,))
                     create = False
 
-                def _is_allowed(*args, attr_name=aname, s=self):
+                #def _is_allowed(*args, attr_name=aname, s=self):
                     #s.debug('>'*80+'\n\n_is_allowed(%s)' % str(args))
-                    req_type = args[-1]
+                    #req_type = args[-1]
+                def _is_allowed(rt1=None, rt2=None, rt3=None, attr_name=aname, s=self):
+                    req_type = rt3 if rt3 is not None else (rt2 if rt2 is not None else rt1)
                     return s.is_dyn_allowed(req_type, attr_name)
 
                 _is_allowed.__name__ = "is_%s_allowed" % aname.lower()
                 setattr(self, _is_allowed.__name__, _is_allowed)
 
                 max_size = (
                     hasattr(self, "DynamicSpectrumSize") and self.DynamicSpectrumSize
@@ -1067,15 +1073,15 @@
 
                             self.dyn_qualities[aname.lower()] = value
                     except Exception as e:
                         self.warning(
                             "In dyn_attr(qualities), re.match(%s(%s),"
                             "%s(%s)) failed" % (type(exp), exp, type(aname), aname)
                         )
-                        print(traceback.format_exc())
+                        self.warning(traceback.format_exc())
 
         if self.CheckDependencies:
             [self.check_dependencies(aname) for aname in self.dyn_values]
 
         ##Setting up state events:
         # THESE SETTINGS ARE STILL NEEDED IN TANGO >= 7
         for x in (
@@ -1093,20 +1099,20 @@
             if x != "state":
                 self.set_change_event(x, True, False)
                 if "archive" in events:
                     self.set_archive_event(x, True, False)
         try:
             self.check_polled_attributes(new_attr=new_polled_attrs)
         except:
-            print(
+            self.warning(
                 "DynamicDS.dyn_attr( ... ), unable to set polling for (%s):"
                 " \n%s" % (new_polled_attrs, traceback.format_exc())
             )
 
-        print("DynamicDS.dyn_attr( ... ), finished. "
+        self.warning("DynamicDS.dyn_attr( ... ), finished. "
             "Attributes ready to accept request ..."
             "\n"+("="*80))
 
     # dyn_attr MUST be an static method, to avoid attribute mismatching (self will be always passed as argument)
     dyn_attr = staticmethod(dyn_attr)
 
     # ------------------------------------------------------------------------------------------------------
@@ -1300,15 +1306,15 @@
                     self.debug(
                         "In check_changed_event(%s,%s): nothing changed"
                         % (aname, shortstr(new_value))
                     )
                     return False
 
         except:  # Needed to prevent fails if attribute_config_3 is not available
-            print(traceback.format_exc())
+            self.warning(traceback.format_exc())
 
         return False
 
     @Cached
     def check_dependencies(self, aname):
         # Checking attribute dependencies
         aname = self.get_attr_name(aname)
@@ -1350,41 +1356,41 @@
         ##Checking attribute dependencies
         # dependencies assigned at dyn_attr by self.check_dependencies()
         # Updating Last Attribute Values
         now = time.time()
         changed = False
         aname = self.get_attr_name(aname)
         for k in self.dyn_values[aname].dependencies or []:
-            self.info(
+            self.debug(
                 "In update_dependencies(%s): "
                 " (%s,last update at %s, KeepTime is %s)"
                 % (aname, k, self.dyn_values[k].updated, self.KeepTime)
             )
 
             old = self._locals.get(k)
             updated = self.dyn_values[k].updated
             if self.KeepTime and (
                 not updated or now > (updated + (old_div(self.KeepTime, 1e3)))
             ):
-                #self.debug("In update_dependencies(%s): read value" % (k,))
-                if USE_STATIC_METHODS:
-                    self.read_dyn_attr(self, ft.fakeAttributeValue(k))
-                else:
-                    self.read_dyn_attr(ft.fakeAttributeValue(k))
+                self.debug("In update_dependencies(%s): read value" % str(k))
+                self.evalAttr(k)
+                #if USE_STATIC_METHODS:
+                    #self.read_dyn_attr(self, ft.fakeAttributeValue(k))
+                #else:
+                    #self.read_dyn_attr(ft.fakeAttributeValue(k))
 
             v = self.dyn_values[k]
 
             if k.lower().strip() != aname.lower().strip() and isinstance(
                 v.value, Exception
             ):
                 self.warning(
                     "evalAttr(%s): An exception is rethrowed "
-                    "from attribute %s" % (aname, k)
+                    "from attribute %s (%s)" % (aname, k, v.value)
                 )
-                print((k, aname, v.value))
                 # Exceptions are passed to dependent attributes
                 raise RethrownException(v.value)
             else:
                 self._locals[k] = v.value  # .value
 
             try:
                 if self._locals[k] != old:
@@ -1419,26 +1425,29 @@
             )
             return attr.set_value_date_quality(v.value, v.time, v.quality)
 
         try:
             #self.debug("DynamicDS(%s)::read_dyn_atr(%s) => evalAttr()"
                 #% (self.get_name(), aname))
 
+            ##################################################
             result = self.evalAttr(aname)  # push is done here
+            ##################################################
 
             quality = self.get_attr_quality(aname, result)
             date = self.get_attr_date(aname, result)
             value = self.get_attr_value(aname, result)
             attr.set_value_date_quality(value, date, quality)
 
             text_result = (
                 type(value) is list
                 and value
                 and "%s[%s]" % (type(value[0]), len(value))
             ) or str(value)
+            
             now = time.time()
             self._last_period[aname] = now - self._last_read.get(aname, 0)
             self._last_read[aname] = now
             self._read_times[aname] = now - self._hook_epoch
             self._total_usage += now - self._hook_epoch
             self.debug(
                 "DynamicDS("
@@ -1467,20 +1476,20 @@
             self._last_period[aname] = now - self._last_read.get(aname, 0)
             self._last_read[aname] = now
             self._read_times[aname] = now - self._hook_epoch  # Internal debugging
             self._eval_times[aname] = now - tstart  # Internal debugging
             if aname == list(self.dyn_values.keys())[-1]:
                 self._cycle_start = now
             last_exc = str(e)
-            print(
+            self.warning(
                 "DynamicDS_read_%s_Exception: %s\n\tresult=%s"
                 % (aname, last_exc, result)
             )
             if not isinstance(e, RethrownException):
-                print(traceback.format_exc())
+                self.warning(traceback.format_exc())
             raise Exception("DynamicDS_read_%s_Exception: %s" % (aname, last_exc))
 
     ##This hook has been used to force self to be passed always as argument and avoid dynattr missmatching
     if USE_STATIC_METHODS:
         read_dyn_attr = staticmethod(read_dyn_attr)
 
     # @Catched
@@ -1493,30 +1502,28 @@
             + ")::write_dyn_atr("
             + aname
             + "), entering at "
             + time.ctime()
             + "..."
         )
 
-        # THIS CHANGE MUST BE TESTED AGAINST PYTANGO7!!!! For Scalar/Spectrum/Image R/W Attrs!!
+        #For Scalar/Spectrum/Image R/W Attrs!!
         try:  # PyTango8
             data = attr.get_write_value()
         except:
             data = []
             attr.get_write_value(data)
 
         if fun.isSequence(data) and self.dyn_values[aname].type.dimx == 1:
             data = data[0]
         elif self.dyn_values[aname].type.dimy != 1:
             x = attr.get_max_dim_x()
             data = [data[i : i + x] for i in range(len(data))[::x]]
 
-        self.setAttr(aname, data)
-        # self.dyn_values[aname].update(result,time.time(),PyTango.AttrQuality.ATTR_VALID)
-        ##if fire_event: self.fireAttrEvent(aname,data)
+        self.setAttr(aname, data) # Executes, caches result and pushes event
 
     ##This hook has been used to force self to be passed always as argument and avoid dynattr missmatching
     if USE_STATIC_METHODS:
         write_dyn_attr = staticmethod(write_dyn_attr)
 
     def push_dyn_attr(
         self,
@@ -1598,29 +1605,31 @@
 
     # --------------------------------------------------------------------------
     #   Attributes and State Evaluation Methods
     # --------------------------------------------------------------------------
 
     ## DYNAMIC ATTRIBUTE EVALUATION ...
     # Copy it to your device and add any method you will need
-    def evalAttr(self, aname, WRITE=False, VALUE=None, _locals=None, push=False):
+    def evalAttr(self, aname, WRITE=False, VALUE=None, 
+                 _locals=None, push=False):
         """
         SPECIFIC METHODS DEFINITION DONE IN self._locals!!!
         @remark Generators don't work  inside eval!, use lists instead
         If push=True, any result is considered as change
         """
         aname, formula = self.get_attr_name(aname), ""
         self.info(
             "DynamicDS(%s)::evalAttr(%s,write=%s,push=%s): ... last value was %s"
             % (
                 self.get_name(),
                 aname,
                 WRITE,
                 push,
-                shortstr(getattr(self.dyn_values.get(aname, None), "value", None)),
+                shortstr(getattr(self.dyn_values.get(aname, None), 
+                                 "value", None)),
             )
         )
         tstart = time.time()
 
         try:
             aname, formula, compiled = self.get_attr_formula(aname, full=True)
 
@@ -1685,21 +1694,24 @@
 
                 # Redundant but needed to avoid attributes overwriting them
                 self._locals.update(list(AttrQuality.names.items()))
                 self._locals.update(list(DynamicDSTypes.items()))
 
                 # Adding states for convenience evaluation
                 self.TangoStates = dict(
-                    (str(v), v) for k, v in list(PyTango.DevState.values.items())
+                    (str(v), v) for k, v in 
+                    list(PyTango.DevState.values.items())
                 )
                 self._locals.update(self.TangoStates)
 
                 # IT IS IMPORTANT TO DO THIS AT THE END!
                 if _locals is not None:
                     # High Priority: variables passed as argument
+                    #print('evalAttr(_locals={})'.format([
+                        #l for l in _locals if l not in self._locals]))
                     self._locals.update(_locals)
 
             except Exception as e:
                 self.error("<" * 80)
                 self.error(traceback.format_exc())
                 da = self.dyn_values.get(aname, None)
                 for t in (
@@ -1783,15 +1795,15 @@
                 )
             )
 
             et = 1e3 * (fn.now() - tstart)
             cached = events or self.dyn_values[aname].keep
             (self.debug if et < 5.0 else self.warning)(
                 "evalAttr(%s): events = %s, check = %s, cached = %s, "
-                "eval_ms = %d" % (aname, events, check, cached, et)
+                "eval_ms = %d" % (aname, events, check, cached, et) 
             )
             if events and check:
                 self.push_dyn_attr(
                     aname,
                     value=value,
                     quality=quality,
                     date=date,
@@ -1814,49 +1826,44 @@
                     self.warning("Unable to check state!")
                     self.warning(traceback.format_exc())
 
             return result
 
         except PyTango.DevFailed as e:
             if self.trace:
-                print("-" * 80)
-                print(
-                    "\n".join(
+                self.warning("-" * 80 + '\n'
+                    +  "\n".join(
                         [
                             "DynamicDS_evalAttr(%s)_WrongFormulaException:" % aname,
                             '\t"%s"' % (formula,),
                             str(traceback.format_exc()),
                         ]
-                    )
-                )
-                print("\n".join([str(e.args[0])]) + "\n" + "*" * 80)
-                print("-" * 80)
+                        ) + '\n' +
+                    + "\n".join([str(e.args[0])]) + "\n" + "*" * 80 + '\n' 
+                    + "-" * 80)
             err = e.args[0]
             self.error(e)
             raise e  # Exception,';'.join([err.origin,err.reason,err.desc])
 
         except Exception as e:
             if self.last_attr_exception and self.last_attr_exception[0] > tstart:
                 e = self.last_attr_exception[-1]
-            if 1:
-                print(
-                    "\n".join(
-                        [
-                            "DynamicDS_evalAttr(%s)_WrongFormulaException"
-                            "%s is not a valid expression!" % (aname,formula,),
-                        ]
-                    )
-                )
-            #s = traceback.format_exc()
-            # self.error(s)
-            #print(s)
+
+            self.warning(
+                "\n".join(
+                    [
+                        "DynamicDS_evalAttr(%s)_WrongFormulaException"
+                        "%s is not a valid expression!" % (aname,formula,),
+                    ]
+                ))
+
             s = traceback.format_exc()
             self.error(s)
             if "not defined" in str(s):
-                print('locals: %s' % str(sorted(self._locals.keys())))
+                self.warning('locals: %s' % str(sorted(self._locals.keys())))
             raise e  # Exception(s)
 
         finally:
             self._eval_times[aname] = fun.now() - tstart
             self._locals["ATTRIBUTE"] = ""
 
     def evalCommand(self, cmd, argin=None):
@@ -1973,15 +1980,15 @@
                                 "DynamicDS(%s.check_state(): New State is %s := %s"
                                 % (self.get_name(), nstate, formula)
                             )
                             if set_state:
                                 self.set_state(new_state, push=True)
                         break
         except Exception as e:
-            print(traceback.format_exc())
+            self.warning(traceback.format_exc())
             raise e
         finally:
             if self.state_lock.locked():
                 self.state_lock.release()
         return new_state
 
     def check_status(self, set=True, previous=''):
@@ -2656,15 +2663,15 @@
             for c, f in list(self.dyn_comms.items()):
                 k = c.split("/")[-1]
                 if self.get_name().lower() in c.lower() and k not in self._locals:
                     self._locals.update(
                         {k: (lambda argin, cmd=k: self.evalCommand(cmd, argin))}
                     )
         except:
-            print(traceback.format_exc())  # self.warning(traceback.format_exc())
+            self.warning(traceback.format_exc())  # self.warning(traceback.format_exc())
 
         self.reset_memleak()
         self._init_count += 1
 
     def delete_device(self):
         self.warning("DynamicDS.delete_device(): ... ")
         PyTango.LatestDeviceImpl.delete_device(self)
@@ -2803,17 +2810,16 @@
     #    Description: Return current dynamic attributes
     #
     #    argin:  DevVoid
     #    argout: DevVarStringArray      Return current dynamic attributes
     # ------------------------------------------------------------------
     # Methods started with underscore could be inherited by child device servers for debugging purposes
     def getDynamicAttributes(self):
-        return sorted(
-            "%s=%s" % (k, v.formula) for k, v in list(self.dyn_values.items())
-        )
+        return sorted(self.dyn_values.keys())
+            #"%s=%s" % (k, v.formula) for k, v in self.dyn_values.items())
 
     # ------------------------------------------------------------------
     #    GetMemUsage command:
     #
     #    Description: Returns own process RSS memory usage (Kb).
     #
     #    argin:  DevVoid
@@ -2986,33 +2992,33 @@
                     old_div(
                         sum(self._eval_times.values()),
                         (sum(self._read_times.values()) or 1),
                     )
                 )
             )
 
-            if False:  # GARBAGE_COLLECTION:
-                if not gc.isenabled():
-                    gc.enable()
-                gc.collect()
-                grb = gc.get_objects()
-                self.info(
-                    "%d objects in garbage collector, %d objects are uncollectable."
-                    % (len(grb), len(gc.garbage))
-                )
-                try:
-                    if self.GARBAGE:
-                        NEW_GARBAGE = [o for o in grb if o not in self.GARBAGE]
-                        self.info(
-                            "New objects added to garbage are: %s"
-                            % ([str(o) for o in NEW_GARBAGE],)
-                        )
-                except:
-                    print(traceback.format_exc())
-                self.GARBAGE = grb
+            #if False:  # GARBAGE_COLLECTION:
+                #if not gc.isenabled():
+                    #gc.enable()
+                #gc.collect()
+                #grb = gc.get_objects()
+                #self.info(
+                    #"%d objects in garbage collector, %d objects are uncollectable."
+                    #% (len(grb), len(gc.garbage))
+                #)
+                #try:
+                    #if self.GARBAGE:
+                        #NEW_GARBAGE = [o for o in grb if o not in self.GARBAGE]
+                        #self.info(
+                            #"New objects added to garbage are: %s"
+                            #% ([str(o) for o in NEW_GARBAGE],)
+                        #)
+                #except:
+                    #print(traceback.format_exc())
+                #self.GARBAGE = grb
 
             # if MEM_CHECK:
             # self._locals['heap'] = h = HEAPY.heap()
             # self.info(str(h))
 
             for a in self._read_count:
                 self._read_count[a] = 0
@@ -3124,14 +3130,19 @@
         ],
         "ReadOnWrite": [
             PyTango.DevBoolean,
             "When True, this will trigger a read attribute just after writing"
             " (e.g. for pushing events on write).",
             [False],
         ],
+        "ReadLocked": [
+            PyTango.DevBoolean,
+            "When True, use a threading lock to avoid simultaneous read_dyn_attr calls",
+            [True],
+        ],        
         "UseEvents": [
             PyTango.DevVarStringArray,
             "Value of this property will be yes/true,no/false or a list of "
             "attributes that will trigger push_event (if configured from jive). "
             "If UseEvents=always, it will be always pushed, "
             "if UseEvents=push, will always push on any change, ignoring config, "
             "if UseEvents=True, then Tango DB config prevails, and is checked",
```

### Comparing `fandango-15.7.4/fandango/excepts.py` & `fandango-15.8.0/fandango/excepts.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/functional.py` & `fandango-15.8.0/fandango/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -2014,19 +2014,18 @@
 
         if _trace:
             print("Out of evalX(%s): %s" % (target, value))
     return value
 
 ###############################################################################
 # Python 2to3 wrappers/helpers
-
-def raw_input(*args, **kwargs):
-    if sys.version_info.major <= 2:
-        return raw_input(*args, **kwargs)
-    else:
+try:
+    raw_input = raw_input
+except:
+    def raw_input(*args, **kwargs):
         return input(*args, **kwargs)
 
 ###############################################################################
 
 try:
     from . import doc
```

### Comparing `fandango-15.7.4/fandango/interface/CopyCatDS.py` & `fandango-15.8.0/fandango/interface/CopyCatDS.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/interface/inheritance.py` & `fandango-15.8.0/fandango/interface/inheritance.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/linos.py` & `fandango-15.8.0/fandango/linos.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/log.py` & `fandango-15.8.0/fandango/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,16 +111,24 @@
 
 def printf(*args):
     # This is a 'lambdable' version of print
     print("".join(map(str, args)))
 
 
 def tprint(*args):
-    print("%s: %s" % (time2str(), " - ".join(map(str, args))))
-
+    print("%s: %s" % (time2str(), "".join(map(str, args))))
+    
+def lprint(sequence):
+    for i,l in enumerate(sequence):
+        print('%05d: %s' % (i,str(l)))
+
+def trace(msg, level):
+    if level > TRACE_LEVEL:
+        return
+    tprint(TRACE_LEVELS.get(level, level), msg)
 
 def printerr(*args):
     sys.stderr.write(*args)
 
 
 def except2str(e=None, max_len=int(7.5 * 80)):
     if e is None:
```

### Comparing `fandango-15.7.4/fandango/objects.py` & `fandango-15.8.0/fandango/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,26 +599,34 @@
             functions; it will cause Deadlock!
         With RLock this problem is avoided ... but you should rely more
             on python threading.
     """
 
     @functools.wraps(func)
     def lock_fun(self, *args, **kwargs):
-        # self,args = args[0],args[1:]
+        # self,args = args[0],args[1:]       
         if not hasattr(self, "lock"):
             setattr(self, "lock", threading.RLock() if reentrant else threading.Lock())
-        if not hasattr(self, "trace"):
-            setattr(self, "trace", False)
-        self.lock.acquire()
+        if not hasattr(self, "lock_trace"):
+            setattr(self, "lock_trace", False)
+
         try:
-            # if self.trace: print "locked: %s"%self.lock
+            if self.lock is not None:
+                self.lock.acquire()            
+                if self.lock_trace:
+                    print("locked: %s" % self.lock)
+                    
             result = func(self, *args, **kwargs)
+            
         finally:
-            self.lock.release()
-            # if self.trace: print "released: %s"%self.lock
+            if self.lock is not None:
+                if self.lock_trace: 
+                    print("released: %s" % self.lock)                
+                self.lock.release()
+                
         return result
 
     # lock_fun.__name__ = func.__name__
     # lock_fun.__doc__ = func.__doc__
     return lock_fun
```

### Comparing `fandango-15.7.4/fandango/pipes.py` & `fandango-15.8.0/fandango/pipes.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/qt.py` & `fandango-15.8.0/fandango/qt.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/CopyCatDS` & `fandango-15.8.0/fandango/scripts/CopyCatDS`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/DynamicDS` & `fandango-15.8.0/fandango/scripts/DynamicDS`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/FolderDS` & `fandango-15.8.0/fandango/scripts/FolderDS`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/WorkerDS` & `fandango-15.8.0/fandango/scripts/WorkerDS`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/csv2tango` & `fandango-15.8.0/fandango/scripts/csv2tango`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/fandango` & `fandango-15.8.0/fandango/scripts/fandango`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/my2to3.py` & `fandango-15.8.0/fandango/scripts/my2to3.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/sardanact` & `fandango-15.8.0/fandango/scripts/sardanact`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/servers_lite.py` & `fandango-15.8.0/fandango/scripts/servers_lite.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/setup.ds.py` & `fandango-15.8.0/fandango/scripts/setup.ds.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/tango2csv` & `fandango-15.8.0/fandango/scripts/tango2csv`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/tango2json` & `fandango-15.8.0/fandango/scripts/tango2json`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/tango_create_device.py` & `fandango-15.8.0/fandango/scripts/tango_create_device.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/tango_create_starter.py` & `fandango-15.8.0/fandango/scripts/tango_create_starter.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/tango_monitor` & `fandango-15.8.0/fandango/scripts/tango_monitor`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/tango_property` & `fandango-15.8.0/fandango/scripts/tango_property`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/scripts/tango_servers` & `fandango-15.8.0/fandango/scripts/tango_servers`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/servers.py` & `fandango-15.8.0/fandango/servers.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/tango/command.py` & `fandango-15.8.0/fandango/tango/commands.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/tango/defaults.py` & `fandango-15.8.0/fandango/tango/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -362,17 +362,18 @@
     
         
 
 @Cached(depth=100, expire=60)
 def get_tango_host(dev_name="", use_db=False, fqdn=None):
     """
     If device is a tango model, it will extract the host from the model URL
-    If devicesis none, then environment variable or PyTango.Database are used
+    If devices is none, then environment variable or PyTango.Database are used
     to extract the host
-    If TANGO_HOST is not defined it will always fallback to PyTango.Database()
+    If use_db is True, then it will get the host from Db before environment
+    If false, it tries TANGO_HOST environment first and then the Db.
     """
     if fqdn is None:
         global USE_FQDN
         fqdn = USE_FQDN
 
     try:
         if dev_name:
@@ -384,25 +385,22 @@
                 m, use_db = None, dev_name
 
             if not m:
                 return get_tango_host(use_db=use_db, fqdn=fqdn)
             else:
                 host, port = m.groups()[0].split(":")
 
-        elif use_db:
-            use_db = use_db if hasattr(use_db, "get_db_host") else get_database()
-
-            host, port = use_db.get_db_host(), int(use_db.get_db_port())
-
         else:
-            host = os.getenv("TANGO_HOST")
-            if not host:
-                return get_tango_host(use_db=True, fqdn=fqdn)
+            tango_host = os.getenv("TANGO_HOST")
+            if use_db or not tango_host:
+                use_db = (use_db if hasattr(use_db, "get_db_host") 
+                    else get_database(use_env=bool(tango_host)))
+                host, port = use_db.get_db_host(), int(use_db.get_db_port())
             else:
-                host, port = host.split(":", 1)
+                host, port = tango_host.split(":", 1)
 
         if fqdn:
             try:
                 if host.count(".") < 2:
                     host = get_fqdn(host)
             except:
                 traceback.print_exc()
@@ -437,48 +435,42 @@
                 f.cache.clear()
             except:
                 pass
     os.environ["TANGO_HOST"] = tango_host
     return tango_host
 
 
-def get_database(host="", port=""):
+@Cached(depth=10, expire=60)
+def get_database(host="", port="", use_env=True):
     """
     Method to get a singleton instance of the Tango Database
     host/port can be a host,port tuple; a 'host:port' string or a taurus model.
     @TODO: host/port is checked only at first creation, once initialized
     you can't change HOST
     """
     global TangoDatabase
     if host in (True, False):
         # For backwards compatibility
         host, port = host, "", ""
 
-    else:
+    elif host:
         if "/" in host:
             # Parsing a taurus model
             host = get_tango_host(host)
         if ":" in host:
             # Parsing a host:port string
             host, port = host.split(":")
-    args = [host, int(port)] if host and port else []
 
-    ### DISABLED, CRUSHED WITH BAD_INV_ORDER CORBA in Tango8
-    if False and not args and TangoDatabase:
-        try:
-            t = time.time()
-            # TangoDatabase.get_info() #TOO SLOW TO BE A CHECK!
-            # TangoDatabase.check_tango_host(TangoDatabase.get_db_host()\
-            # +':'+TangoDatabase.get_db_port())
-            # TangoDatabase.get_timeout_millis()
-            print(time.time() - t)
-            return TangoDatabase
-        except:
-            # traceback.print_exc()
-            pass  # defaulting to Taurus/PyTango
+    elif use_env: 
+        # Don't call get_tango_host here to avoid recursive calls
+        # TANGO_HOST env will take precedence over /etc/tangorc
+        host = os.getenv("TANGO_HOST") or ":"
+        host, port = host.split(":", 1)
+
+    args = [host, int(port)] if host and port else []
     try:
         db = Database(*args)
         if not args:
             TangoDatabase = db
         return db
     except:
         print(traceback.format_exc())
```

### Comparing `fandango-15.7.4/fandango/tango/dynattr.py` & `fandango-15.8.0/fandango/tango/dynattr.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,24 +451,26 @@
         if len(r) > 80 * 2:
             r = r.replace(";", ",\n\t")
         else:
             r = r.replace(";", ",")
         return r
 
     def operator(self, op_name, other=None, unary=False, multipleargs=False):
-        # print('operator() called for %s(%s).%s(%s)'%(self.__class__,str(type(self.value)),op_name,other and other.__class__ or ''))
+        #print('operator() called for %s(%s).%s(%s)'
+              #% (self.__class__,str(type(self.value)),op_name,other and other.__class__ or ''))
         value = self.value
 
         if value is None:
             if op_name in [
                 "__nonzero__",
                 "__int__",
                 "__float__",
                 "__long__",
                 "__complex__",
+                "__bool__",
             ]:
                 value = 0
             elif op_name in ["__str__", "__repr__"]:
                 return ""
             else:
                 return None
         elif float in (type(value), type(other)):
@@ -508,15 +510,16 @@
                 method = lambda s, x: (s.__cmp__(x) > 0)
             if op_name == "__ge__":
                 method = lambda s, x: (s.__cmp__(x) >= 0)
 
         elif hasattr(type(value), op_name) and hasattr(value, op_name):
             # Be Careful, method from the class and from the instance don't get the same args
             method = getattr(type(value), op_name)
-            # print('Got %s from %s: %s'%(op_name,type(value),method))
+            #print('Got %s from %s: %s'%(op_name,type(value),method))
+            
         # elif op_name in value.__class__.__base__.__dict__:
         #    method = value.__class__.__base__.__dict__[op_name]
 
         else:
             raise_(
                 Exception,
                 "DynamicAttribute_WrongMethod%sFor%sType==(%s)"
@@ -526,14 +529,15 @@
         if unary:
             if value is None and op_name in [
                 "__nonzero__",
                 "__int__",
                 "__float__",
                 "__long__",
                 "__complex__",
+                "__bool__",
             ]:
                 result.value = method(0)
             else:
                 result.value = method(value)
         elif multipleargs:
             args = [value] + list(other)
             result.value = method(*args)
@@ -553,14 +557,15 @@
             result.value = method(value, other.value)
         else:
             #### THIS IS THE DEFAULT FOR MOST OPERATIONS
             # print('%s,%s(%s),%s(%s)' % (method,type(value),value,type(other),other))
             result.value = method(value, other)
         if op_name in [
             "__nonzero__",
+            "__bool__",            
             "__int__",
             "__float__",
             "__long__",
             "__complex__",
             "__index__",
             "__len__",
             "__str__",
```

### Comparing `fandango-15.7.4/fandango/tango/export.py` & `fandango-15.8.0/fandango/tango/export.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/tango/methods.py` & `fandango-15.8.0/fandango/tango/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1489,19 +1489,25 @@
     
     model can be attribute, device or proxy
     """
     return check_attribute(model, attr, timeout=timeout, 
             readable=True, brief=not full)
 
 def read_attributes(models, timeout=0, full=False):
+    """ expands regexp in models and returns attr:value dictionary """
+    from fandango.tango.search import find_attributes
     if isString(models):
         models = toList(models)
-    from fandango.tango.search import find_attributes
-    models = [t for m in models for t in find_attributes(m)]
-    return {m:read_attribute(m,timeout=timeout,full=full) for m in models}
+    attrs = []
+    for m in models:
+        if isRegexp(m):
+            attrs.extend(find_attributes(m))
+        else:
+            attrs.append(m)
+    return {m:read_attribute(m,timeout=timeout,full=full) for m in attrs}
 
 
 def write_attribute(attr, value, timeout=0, full=False):
     """Write attribute value to device"""
     model = parse_tango_model(attr)
     dp = get_device(model.device)
     dp.set_timeout_millis(timeout * 1000)
```

### Comparing `fandango-15.7.4/fandango/tango/search.py` & `fandango-15.8.0/fandango/tango/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,29 +152,32 @@
     # Dont count slashes, as regexps may be complex
     fullname = fullname or any(h not in (defhost, None) for h in hosts)
 
     all_devs = []
     if trace:
         print((hosts, fullname))
 
-    condition = (clsearch,clmatch)[any(isRegexp(e) for e in patterns)]
+    condition = clsearch if any(isRegexp(e) for e in patterns) else None
         
     for host in hosts:
         if host in (None, defhost):
             odb = get_database()
             db_devs = get_all_devices(exported)
         else:
             # print('get_matching_devices(*%s)'%host)
             odb = get_database(host)
             db_devs = list(odb.get_device_exported("*") if exported
                 else odb.get_device_name("*", "*")
                 )
         
-        db_devs = set(d for d in db_devs 
-                    for e in patterns if condition(e,d))
+        if condition:
+            db_devs = set(d for d in db_devs for e in patterns if condition(e,d))
+        else:
+            # Regular expression search is much slower than just this
+            db_devs = [d for d in db_devs if any(p in d for p in patterns)]
         
         if check_alias:
             alias = odb.get_device_alias_list('*')
             [db_devs.add(odb.get_device_alias(k)) 
                 for k in alias for e in patterns 
                 if condition(e,k)]
```

### Comparing `fandango-15.7.4/fandango/tango/tangoeval.py` & `fandango-15.8.0/fandango/tango/tangoeval.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/testing/check_callbacks.py` & `fandango-15.8.0/fandango/testing/check_callbacks.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/testing/check_fandango.py` & `fandango-15.8.0/fandango/testing/check_fandango.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/testing/checkmodule.py` & `fandango-15.8.0/fandango/testing/checkmodule.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/testing/gen_test_file.py` & `fandango-15.8.0/fandango/testing/gen_test_file.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/testing/simulation.py` & `fandango-15.8.0/fandango/testing/simulation.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango/threads.py` & `fandango-15.8.0/fandango/threads.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,15 +519,15 @@
         self,
         other=None,
         read_method=None,
         write_method=None,
         timewait=0.1,
         threaded=True,
         trace=False,
-        delay=0.0,
+        delay=0.0, #delay on thread start
         callback=None,
     ):
         self.read_method = read_method
         self.write_method = write_method
         self.callback = callback
         self.timewait = timewait
         self.threaded = threaded
@@ -544,45 +544,54 @@
         self.event = threading.Event()
 
         if other:
             dict.update(self, other)
 
     def tracer(self, text, level=0):
         if self.trace and level<self.trace:
-            print('ThreadDict:%s' % str(text))
+            print('%s: ThreadDict:%s' % (time2str(),str(text)))
         
 
     # @self_locked
     def start(self):
         if not self.threaded:
-            print("ThreadDict.start(): This Dict has no Thread!")
-            return
-        if hasattr(self, "_Thread") and self._Thread and self._Thread.is_alive():
-            print("ThreadDict.start(): ThreadDict.stop() must be executed first!")
+            self.tracer("ThreadDict.start(): This Dict has no Thread!")
             return
+        if self.alive():
+            self.tracer("ThreadDict.start(): ThreadDict.stop() "
+                "must be executed first!")
+            self.stop()
+            if self.alive():
+                raise Exception('ThreadDictNotStopped')
         if self.delay:
             self.event.wait(self.delay)
-        print("In ThreadDict.start()")  # , keys are: %s' % self.threadkeys()
+            
+        self.tracer("In ThreadDict.start()")
         self.event.clear()
         self._Thread = threading.Thread(target=self.run)
         self._Thread.setDaemon(True)
         self._Thread.start()
         self.tracer("ThreadDict started!")
 
     # @self_locked
-    def stop(self):
-        print("Stopping ThreadDict ...")
+    def stop(self,wait = 3.):
+        self.tracer("Stopping ThreadDict ...")
         if self.threaded and hasattr(self, "event"):
             self.tracer('event set')
             self.event.set()
-        self.event.wait(5e-3)
-        if hasattr(self, "_Thread"):
-            #print('thread({}) join'.format(self._Thread))
-            self._Thread.join(5.)
-        print("ThreadDict Stopped")
+        
+        if self.alive():
+            self.event.wait(5e-3)
+            self._Thread.join(wait)
+            if self.alive():
+                self.tracer("ThreadDict NOT Stopped!!",-1)
+                return False
+            
+        self.tracer("ThreadDict Stopped",-1)
+        return True
 
     def alive(self):
         if not hasattr(self, "_Thread") or not self._Thread:
             return None  # Thread never started
         else:
             return self._Thread.is_alive()  # True or False
 
@@ -701,15 +710,15 @@
 
     def __getitem__(self, key, hw=False):
         """ This method launches a hardware reading
             if there's no thread on charge of doing that 
             or if the hw flag is set to True.
         """
         if self.trace:
-            print("In ThreadDict.__getitem__(%s,%s)" % (key, hw))
+            self.tracer("In ThreadDict.__getitem__(%s,%s)" % (key, hw))
         if (
             hw or not self.threaded
         ):  # HW ACCESS MUST NOT BE DONE WITHOUT ASKING EXPLICITLY! (Use __setitem__(k,None) instead)
             self._updates[key] = time.time()
             if self.read_method:
                 value = self.read_method(key)
                 self.__locked_setitem__(key, value) #< cache update!
@@ -720,15 +729,15 @@
 
     def __setitem__(self, key, value, hw=True):
         """ This method writes value to hardware
             if the hw flag is not explicitly set to False,
             if hw=False, cache is updated for clients to read it.
         """
         if self.trace:
-            print("In ThreadDict.__setitem__(%s,...,%s)" % (key, hw))
+            self.tracer("In ThreadDict.__setitem__(%s,...,%s)" % (key, hw))
         if hw and self.write_method:
             # It implies that a key will not be added here to read thread!
             nvalue = self.write_method(*[key, value])
             #self.__locked_setitem__(key, nvalue)
             dict.__setitem__(self,key,nvalue)
         else:
             #self.__locked_setitem__(key, value)
@@ -1081,31 +1090,39 @@
     def start(self):
         self._thread.start()
 
     def stop(self):
         self.stopEvent.set()
         self._thread.join()
 
-    def isAlive(self):
+    def is_alive(self):
         return self._thread.is_alive()
-    
-    def isBusy(self):
-        return self.busy
 
-    is_alive = isAlive
+    isAlive = is_alive
 
-    def getQueue(self):
+    def is_busy(self):
+        return self.busy
+    
+    isBusy = is_busy
+
+    def get_queue(self):
         return self.outQueue
+    
+    getQueue = get_queue
 
-    def getSize(self):
+    def get_size(self):
         return self.inQueue.qsize()
 
-    def getDone(self):
+    getSize = get_size
+    
+    def get_done(self):
         return not self.getSize() and not self.isBusy() #outQueue.qsize()
 
+    getDone = get_done
+    
     def process(self, target):
         """
         This method can be overriden in child classes to perform actions distinct from evalX
         """
         self.modules = getattr(self, "modules", {})
         self.instances = getattr(self, "instances", {})
         self._locals = getattr(self, "_locals", {})
@@ -1142,15 +1159,17 @@
                             value = self.process(target)
                             try:
                                 pickle.dumps(value)
                             except pickle.PickleError:
                                 print(traceback.format_exc())
                                 raise WorkerException("%s:UnpickableValue(%s)" 
                                      % (model, value))
+
                             self.outQueue.put((model, value))
+                            
                         except Exception as e:
                             msg = "Exception in WorkerThread(%s).run(%s)\n%s" % (
                                 self._name,
                                 target,
                                 except2str(),
                             )
                             print(msg)
@@ -1361,16 +1380,17 @@
 
     def stop(self):
         # This method stops all threads
         self.trace("stop()")
         self._process_event.set(), self._threading_event.set()
         self._pipe1.close(), self._pipe2.close()
 
-    def isAlive(self):
+    def is_alive(self):
         return self._process.is_alive() and self._receiver.is_alive()
+    isAlive = is_alive
 
     is_alive = isAlive
 
     def keys(self):
         return list(self.data.keys())
 
     def add(self, key, target=None, args=None, period=0, expire=0, callback=None):
```

### Comparing `fandango-15.7.4/fandango/web.py` & `fandango-15.8.0/fandango/web.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/fandango.egg-info/PKG-INFO` & `fandango-15.8.0/fandango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fandango
-Version: 15.7.4
+Version: 15.8.0
 Summary: Simplify the configuration of big Tango control systems
 Home-page: UNKNOWN
 Author: Sergi Rubio
 Author-email: srubio@cells.es
 License: UNKNOWN
 Description: Fandango is a Python module created to simplify the configuration of big control systems; implementing the behavior of Jive (configuration) and/or Astor (deployment) tools in methods that could be called from scripts using regexp and wildcards. Fandango provides functional methods, classes and utilities to develop high-level device servers and APIs for Tango control system.
 Platform: Linux,Windows XP/Vista/7/8
```

### Comparing `fandango-15.7.4/fandango.egg-info/SOURCES.txt` & `fandango-15.8.0/fandango.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 fandango/arrays.py
 fandango/callbacks.py
 fandango/db.py
 fandango/debug.py
 fandango/devslist.py
 fandango/dicts.py
 fandango/doc.py
+fandango/dynamic.last.py
 fandango/dynamic.py
 fandango/excepts.py
 fandango/functional.py
 fandango/linos.py
 fandango/log.py
 fandango/objects.py
 fandango/pipes.py
@@ -48,27 +49,28 @@
 fandango.egg-info/requires.txt
 fandango.egg-info/top_level.txt
 fandango/device/DDebug.py
 fandango/device/Dev4Tango.py
 fandango/device/DynamicDS.py
 fandango/device/FolderDS.py
 fandango/device/FolderGUI.py
+fandango/device/ScriptDS.py
 fandango/device/WorkerDS.py
 fandango/device/__init__.py
 fandango/interface/CopyCatDS.py
 fandango/interface/__init__.py
 fandango/interface/inheritance.py
 fandango/scripts/__init__.py
 fandango/scripts/my2to3.py
 fandango/scripts/servers_lite.py
 fandango/scripts/setup.ds.py
 fandango/scripts/tango_create_device.py
 fandango/scripts/tango_create_starter.py
 fandango/tango/__init__.py
-fandango/tango/command.py
+fandango/tango/commands.py
 fandango/tango/defaults.py
 fandango/tango/dynattr.py
 fandango/tango/export.py
 fandango/tango/methods.py
 fandango/tango/search.py
 fandango/tango/tangoeval.py
 fandango/testing/__init__.py
```

### Comparing `fandango-15.7.4/setup.py` & `fandango-15.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/tests/definitions.py` & `fandango-15.8.0/tests/definitions.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/tests/test_functional.py` & `fandango-15.8.0/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/tests/test_functional_auto_gen.py` & `fandango-15.8.0/tests/test_functional_auto_gen.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/tests/test_functional_skip.py` & `fandango-15.8.0/tests/test_functional_skip.py`

 * *Files identical despite different names*

### Comparing `fandango-15.7.4/tests/test_objects.py` & `fandango-15.8.0/tests/test_objects.py`

 * *Files identical despite different names*

