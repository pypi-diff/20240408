# Comparing `tmp/PyTangoArchiving-8.5.2.tar.gz` & `tmp/PyTangoArchiving-9.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyTangoArchiving-8.5.2.tar", last modified: Mon Oct 22 08:59:47 2018, max compression
+gzip compressed data, was "PyTangoArchiving-9.2.5.tar", last modified: Mon Apr  8 14:12:03 2024, max compression
```

## Comparing `PyTangoArchiving-8.5.2.tar` & `PyTangoArchiving-9.2.5.tar`

### file list

```diff
@@ -1,79 +1,95 @@
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/scripts/
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     9283 2018-10-22 08:49:55.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/scripts/archiving2csv
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    12351 2018-10-19 15:34:53.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/scripts/archiving2plot
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     6775 2018-10-19 15:34:59.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/scripts/archiving_service
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     2619 2018-10-19 15:35:04.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/scripts/ctarchiving
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      311 2018-10-19 15:35:07.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/scripts/ctsnaps
--rwxr-xr-x   0 srubio    (1206) Control   (1200)      136 2018-10-19 15:35:12.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/scripts/taurusfinder
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/hdbpp/
--rw-r--r--   0 srubio    (1206) Control   (1200)       68 2018-04-05 08:42:49.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/hdbpp/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    35416 2018-10-19 16:43:04.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/hdbpp/config.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     1404 2018-01-04 12:54:44.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/hdbpp/create_partitions.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     6768 2018-10-09 15:40:50.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/hdbpp/decimate.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    16340 2018-08-24 08:38:37.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/hdbpp/multi.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     1065 2016-03-21 14:16:00.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/hdbpp/read.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/servers/
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/servers/PyExtractor/
--rw-r--r--   0 srubio    (1206) Control   (1200)    21613 2018-07-24 19:07:01.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/servers/PyExtractor/PyExtractor.py
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2017-01-04 12:08:14.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/servers/PyExtractor/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2017-01-04 12:07:57.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/servers/__init__.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/ui/
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2014-04-14 10:48:00.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/ui/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    11631 2018-10-12 14:54:21.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/ui/core.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     4496 2018-10-12 14:54:21.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/ui/diff.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     7491 2018-10-12 14:54:21.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/ui/modify.py
--rw-r--r--   0 srubio    (1206) Control   (1200)       20 2014-04-14 10:49:34.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     4739 2018-10-12 14:54:21.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/contexttoolbar.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     6946 2018-10-12 14:54:21.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/snapbutton.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    51709 2018-10-12 14:54:21.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/snapdialogs.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    42591 2018-10-12 14:54:21.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/snaps.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)     3869 2018-10-12 14:54:21.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/snaps/toolbar.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/ui/
--rw-r--r--   0 srubio    (1206) Control   (1200)     9681 2018-10-12 14:54:21.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/ui/TaurusAttributeChooser.ui
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2018-10-19 17:16:08.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/ui/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    39618 2018-10-12 16:28:46.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/ArchivingBrowser.py
--rw-r--r--   0 srubio    (1206) Control   (1200)      525 2017-03-01 16:32:28.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    28281 2018-10-12 16:24:26.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/dialogs.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    12750 2018-10-12 17:12:55.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/history.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    34213 2018-05-10 10:52:26.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/models.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    15923 2018-05-14 15:07:51.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/panel.py
--rw-r--r--   0 srubio    (1206) Control   (1200)      272 2017-11-15 15:57:13.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/progress.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    11585 2017-11-15 15:55:11.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/resources.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     7862 2017-11-15 15:56:53.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/taurusattributechooser.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    25583 2017-11-15 15:55:25.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/tdbwidget.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    10013 2017-11-15 16:00:15.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/tests.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    37814 2018-05-16 15:46:23.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/tree.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    48385 2018-10-12 16:40:18.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/widget/trend.py
--rw-r--r--   0 srubio    (1206) Control   (1200)        6 2018-10-22 08:58:59.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/VERSION
--rw-r--r--   0 srubio    (1206) Control   (1200)    10278 2018-10-19 15:17:15.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    69696 2018-09-17 10:17:01.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/archiving.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    18055 2018-10-16 08:30:55.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/check.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    21758 2018-10-12 15:08:56.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/common.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    35866 2018-10-07 06:47:36.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/dbs.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    56641 2018-05-14 15:10:42.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/files.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    83213 2018-10-22 08:38:48.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/reader.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     7552 2018-10-22 08:35:29.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/schemas.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    59917 2018-10-12 15:09:52.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/snap.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     1436 2016-04-28 11:46:05.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/tests.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    24255 2018-08-29 09:39:41.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/utils.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    12354 2017-11-15 15:54:47.000000 PyTangoArchiving-8.5.2/PyTangoArchiving/web.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/PyTangoArchiving.egg-info/
--rw-r--r--   0 srubio    (1206) Control   (1200)     1020 2018-10-22 08:59:46.000000 PyTangoArchiving-8.5.2/PyTangoArchiving.egg-info/PKG-INFO
--rw-r--r--   0 srubio    (1206) Control   (1200)     2265 2018-10-22 08:59:46.000000 PyTangoArchiving-8.5.2/PyTangoArchiving.egg-info/SOURCES.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)        1 2018-10-22 08:59:46.000000 PyTangoArchiving-8.5.2/PyTangoArchiving.egg-info/dependency_links.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       20 2018-10-22 08:59:46.000000 PyTangoArchiving-8.5.2/PyTangoArchiving.egg-info/entry_points.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)        1 2017-09-23 06:19:50.000000 PyTangoArchiving-8.5.2/PyTangoArchiving.egg-info/not-zip-safe
--rw-r--r--   0 srubio    (1206) Control   (1200)       30 2018-10-22 08:59:46.000000 PyTangoArchiving-8.5.2/PyTangoArchiving.egg-info/requires.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       17 2018-10-22 08:59:46.000000 PyTangoArchiving-8.5.2/PyTangoArchiving.egg-info/top_level.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)      427 2016-04-27 10:33:45.000000 PyTangoArchiving-8.5.2/AUTHORS
--rw-r--r--   0 srubio    (1206) Control   (1200)    28806 2018-10-10 07:43:16.000000 PyTangoArchiving-8.5.2/CHANGES
--rw-r--r--   0 srubio    (1206) Control   (1200)     3747 2016-04-27 10:33:45.000000 PyTangoArchiving-8.5.2/LICENSE
--rw-r--r--   0 srubio    (1206) Control   (1200)      160 2018-10-19 17:24:09.000000 PyTangoArchiving-8.5.2/MANIFEST.in
--rw-r--r--   0 srubio    (1206) Control   (1200)     1412 2018-08-13 15:08:48.000000 PyTangoArchiving-8.5.2/README.rst
--rw-r--r--   0 srubio    (1206) Control   (1200)     2828 2018-10-19 17:25:14.000000 PyTangoArchiving-8.5.2/setup.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     1020 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/PKG-INFO
--rw-r--r--   0 srubio    (1206) Control   (1200)       38 2018-10-22 08:59:47.000000 PyTangoArchiving-8.5.2/setup.cfg
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:12:03.535795 PyTangoArchiving-9.2.5/
+-rw-r--r--   0 srubio    (1206) Control   (1200)      427 2022-12-16 10:23:50.000000 PyTangoArchiving-9.2.5/AUTHORS
+-rw-r--r--   0 srubio    (1206) Control   (1200)     3747 2022-12-16 10:23:50.000000 PyTangoArchiving-9.2.5/LICENSE
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1129 2023-06-08 09:48:26.000000 PyTangoArchiving-9.2.5/MANIFEST.in
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1020 2024-04-08 14:12:03.534795 PyTangoArchiving-9.2.5/PKG-INFO
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:12:01.637812 PyTangoArchiving-9.2.5/PyTangoArchiving/
+-rw-r--r--   0 srubio    (1206) Control   (1200)        6 2024-04-08 14:11:07.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/VERSION
+-rw-r--r--   0 srubio    (1206) Control   (1200)    10744 2023-11-24 15:38:07.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    69861 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/archiving.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    39367 2024-04-08 13:42:31.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/check.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    21824 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/common.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    40534 2024-04-03 09:41:41.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/dbs.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    58075 2023-08-24 09:09:57.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/files.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:12:02.068825 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/
+-rw-r--r--   0 srubio    (1206) Control   (1200)      163 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    10276 2022-12-16 10:23:50.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/alter_datetime.sql
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1147 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/api.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     8086 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/check_and_recover_attributes.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    44859 2024-04-05 13:35:14.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/config.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    32521 2022-12-16 10:23:50.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/create_hdb++_mysql.sql
+-rw-r--r--   0 srubio    (1206) Control   (1200)     4171 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/create_hdbpp_devices.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     7865 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/decimate.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    71970 2024-04-08 14:10:13.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/maintenance.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    18970 2023-08-24 09:12:03.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/multi.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    12774 2024-04-03 09:41:41.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/periodic.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      543 2023-06-08 09:56:00.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/privileges.sh
+-rw-r--r--   0 srubio    (1206) Control   (1200)      342 2023-06-08 08:29:24.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/privileges.sql
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    37347 2023-08-24 09:12:35.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/query.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1598 2023-08-24 09:13:12.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/subscribe_attributes.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    93695 2024-04-03 09:41:41.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/reader.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    12176 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/schemas.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:12:02.437814 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      108 2022-12-16 10:23:50.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/PyExtractor
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/THIS_FOLDER_SHOULD_NOT_HAVE__init.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1537 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/alter_snap_db.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    12354 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/archiver_health_check.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    14680 2023-08-24 10:25:12.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/archiving2csv
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    12688 2022-12-16 10:23:50.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/archiving2plot
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1223 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/archiving_load.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    21664 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/archiving_report.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     4997 2022-12-16 10:23:50.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/archiving_service
+-rw-r--r--   0 srubio    (1206) Control   (1200)     9768 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/archiving_transfer.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1737 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/check_db_growth.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      840 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/check_partitions.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     2640 2022-12-16 10:23:50.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/ctarchiving
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     4135 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/db_repair.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     4376 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/decimate_table.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1893 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/inspect_hdbpp_hosts.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)     1005 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/start_hdbpp_archivers.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      136 2022-12-16 10:23:50.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/taurusfinder
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:12:02.441814 PyTangoArchiving-9.2.5/PyTangoArchiving/servers/
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:12:02.727807 PyTangoArchiving-9.2.5/PyTangoArchiving/servers/PyExtractor/
+-rw-r--r--   0 srubio    (1206) Control   (1200)    22473 2023-08-24 09:19:29.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/servers/PyExtractor/PyExtractor.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/servers/PyExtractor/__init__.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:12:02.785808 PyTangoArchiving-9.2.5/PyTangoArchiving/servers/SchemaManager/
+-rw-r--r--   0 srubio    (1206) Control   (1200)    21599 2023-08-24 09:20:18.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/servers/SchemaManager/SchemaManager.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/servers/SchemaManager/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/servers/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    31168 2024-04-03 09:41:41.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/utils.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    12367 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/web.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:12:03.491822 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/
+-rw-r--r--   0 srubio    (1206) Control   (1200)    42611 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/ArchivingBrowser.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)      342 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    30547 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/dialogs.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    12776 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/history.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    34213 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/models.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    21775 2023-08-24 09:24:00.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/panel.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)      272 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/progress.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:12:03.522831 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/resources/
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)      323 2022-12-16 10:23:51.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/resources/add.png
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1029 2022-12-16 10:23:51.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/resources/open.png
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1174 2022-12-16 10:23:51.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/resources/save.png
+-rw-r--r--   0 srubio    (1206) Control   (1200)    11585 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/resources.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)      229 2022-12-16 10:23:51.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/resources.qrc
+-rw-r--r--   0 srubio    (1206) Control   (1200)     7872 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/taurusattributechooser.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    25600 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/tdbwidget.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     9904 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/tests.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    12993 2023-06-16 14:19:52.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/tpgarchivingwidget.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    37816 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/tree.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    47959 2023-07-26 15:47:36.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/trend.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:12:03.531819 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/ui/
+-rw-r--r--   0 srubio    (1206) Control   (1200)     9681 2022-12-16 10:23:51.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/ui/TaurusAttributeChooser.ui
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2023-06-16 14:19:53.000000 PyTangoArchiving-9.2.5/PyTangoArchiving/widget/ui/__init__.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2024-04-08 14:12:01.659805 PyTangoArchiving-9.2.5/PyTangoArchiving.egg-info/
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1020 2024-04-08 14:11:59.000000 PyTangoArchiving-9.2.5/PyTangoArchiving.egg-info/PKG-INFO
+-rw-r--r--   0 srubio    (1206) Control   (1200)     3066 2024-04-08 14:11:59.000000 PyTangoArchiving-9.2.5/PyTangoArchiving.egg-info/SOURCES.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)        1 2024-04-08 14:11:59.000000 PyTangoArchiving-9.2.5/PyTangoArchiving.egg-info/dependency_links.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       20 2024-04-08 14:11:59.000000 PyTangoArchiving-9.2.5/PyTangoArchiving.egg-info/entry_points.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)        1 2023-11-24 15:43:23.000000 PyTangoArchiving-9.2.5/PyTangoArchiving.egg-info/not-zip-safe
+-rw-r--r--   0 srubio    (1206) Control   (1200)       25 2024-04-08 14:11:59.000000 PyTangoArchiving-9.2.5/PyTangoArchiving.egg-info/requires.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       17 2024-04-08 14:11:59.000000 PyTangoArchiving-9.2.5/PyTangoArchiving.egg-info/top_level.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1412 2022-12-16 10:23:51.000000 PyTangoArchiving-9.2.5/README.rst
+-rw-r--r--   0 srubio    (1206) Control   (1200)       38 2024-04-08 14:12:03.535817 PyTangoArchiving-9.2.5/setup.cfg
+-rw-r--r--   0 srubio    (1206) Control   (1200)     2879 2023-11-24 15:40:42.000000 PyTangoArchiving-9.2.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/scripts/archiving2plot` & `PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/archiving2plot`

 * *Files 2% similar despite different names*

```diff
@@ -146,22 +146,30 @@
   print "archiving2plot [--no-plot] file.csv/pck"
   sys.exit(1)
   
 options = [a for a in args if a.startswith('--')]
 files = [a for a in args if a.endswith('.pck') or a.endswith('.csv')]
 args = [a for a in args if a not in files and '--' not in a]
 folder = '/tmp/'
+schemas = [o for o in options if o.startswith('--schemas=')] or None
+if schemas:
+    schemas = schemas[0].split('=')[-1].split(',')
+    
+decimate = [d for d in options if d.startswith('--decimate=')] or None
+if decimate:
+    decimate = int(decimate[0].split('=')[-1])
 
 ats = args[:-2]
 if len(args)>=2:    
     t = map(fandango.str2time,(args[-2],args[-1]))
 if ats:
     print 'Getting %s values'%ats
     reader = PyTangoArchiving.Reader() #reader.getArchivingReader(ats,t[0])
-    vals.update(reader.get_attributes_values(ats,t[0],t[1]))
+    reader.log.setLogLevel('info')
+    vals.update(reader.get_attributes_values(ats,t[0],t[1],schemas=schemas,decimate=decimate))
     for k in ats:
         v = vals[k]
         if not v: 
             print('Attr %s has no values'%k)
             vals.pop(k)
         else:
             try:
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/scripts/ctarchiving` & `PyTangoArchiving-9.2.5/PyTangoArchiving/scripts/ctarchiving`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/bin/bash
 
 if [ "$(which alba_blissrc 2>/dev/null)" ] ; then
   echo "loading .rc file ..."
   . alba_blissrc
 fi
 
+export QT_API=pyqt4
+
 PTAROOT=$(python -c "import imp;print(imp.find_module('PyTangoArchiving')[1])")
 
 case $1 in
  --help|help)
   echo "Usage:"
   echo "  ctarchiving --help"
   echo "  ctarchiving --load <filename.csv> <hdb/tdb> [force] ;\
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/hdbpp/config.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/tree.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,904 +1,982 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 #############################################################################
-## This file is part of Tango Control System:  http://www.tango-controls.org/
 ##
-## $Author: Sergi Rubio Manrique, srubio@cells.es
-## copyleft :    ALBA Synchrotron Controls Section, www.cells.es
+# This file is part of Taurus
 ##
-## Tango Control System is free software; you can redistribute it and/or
-## modify it under the terms of the GNU General Public License as published
-## by the Free Software Foundation; either version 3 of the License, or
-## (at your option) any later version.
+# http://taurus-scada.org
 ##
-## Tango Control System is distributed in the hope that it will be useful,
-## but WITHOUT ANY WARRANTY; without even the implied warranty of
-## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-## GNU General Public License for more details.
+# Copyright 2011 CELLS / ALBA Synchrotron, Bellaterra, Spain
+##
+# Taurus is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Lesser General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+##
+# Taurus is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Lesser General Public License for more details.
+##
+# You should have received a copy of the GNU Lesser General Public License
+# along with Taurus.  If not, see <http://www.gnu.org/licenses/>.
 ##
-## You should have received a copy of the GNU General Public License
-## along with this program; if not, see <http://www.gnu.org/licenses/>.
 #############################################################################
 
-import PyTangoArchiving
-from PyTangoArchiving.dbs import ArchivingDB
-from PyTangoArchiving.common import CommonAPI
-from PyTangoArchiving.reader import Reader
-from PyTangoArchiving.utils import CatchedAndLogged
-from PyTangoArchiving.schemas import Schemas
-
-import fandango as fn
-from fandango.objects import SingletonMap, Cached
-from fandango.tango import *
-import MySQLdb,traceback,re
-from PyTango import AttrQuality
-
-__test__ = {}
-
-def get_search_model(model):
-    if model.count(':')<2:
-        model = '%/'+model
-    model = clsub('[:][0-9]+','%:%',model)
-    return model
+"""This module provides widgets that display the database in a tree format"""
 
-class HDBpp(ArchivingDB,SingletonMap):
-    
-    def __init__(self,db_name='',host='',user='',
-                 passwd='', manager='',
-                 other=None, port = '3306'):
-        """
-        Configuration can be loaded from PyTangoArchiving.Schemas,
-        an HdbConfigurationManager or another DB object.
-        """
-        assert db_name or manager, 'db_name/manager argument is required!'
-        self.tango = get_database()
+# todo: tango-centric!!
 
-        if not all((db_name,host,user,passwd)):
-            if other:
-                print('HDBpp(): Loading from DB object')
-                db_name,host,user,passwd = \
-                    other.db_name,other.host,other.user,other.passwd
-            elif manager:
-                print('HDBpp(): Loading from manager')
-                d,h,u,p = self.get_db_config(manager=manager,db_name=db_name)
-                db_name = db_name or d
-                host = host or h    
-                user = user or u
-                passwd = passwd or p                
-            else:
-                sch = Schemas.getSchema(db_name)
-                if sch:
-                    print('HDBpp(): Loading from Schemas')
-                    db_name = sch.get('dbname',sch.get('db_name'))
-                    host = host or sch.get('host')
-                    user = user or sch.get('user')
-                    passwd = passwd or sch.get('passwd')
-                    port = port or sch.get('port')
-                elif not manager:
-                    print('HDBpp(): Searching for manager')
-                    m = self.get_manager(db_name)
-                    t = self.get_db_config(manager=m,db_name=db_name)
-                    host,user,passwd = t[1],t[2],t[3]
-
-        self.port = port
-        self.archivers = []
-        self.attributes = fn.defaultdict(fn.Struct)
-        self.dedicated = {}
-        ArchivingDB.__init__(self,db_name,host,user,passwd,)
-        try:
-            self.get_manager()
-            self.get_attributes()
-        except:
-            traceback.print_exc()
-            print('Unable to get manager')
-            
-    def keys(self):
-        if not self.attributes:
-            self.get_attributes()
-        return self.attributes.keys()
-    
-    def has_key(self,k):
-        self.keys();
-        k = fn.tango.get_full_name(k).lower()
-        return k in self.attributes
-    
-    def __contains__(self,k):
-        return self.has_key(k)
-    
-    def __len__(self):
-        self.keys();
-        return len(self.attributes)
-    
-    def values(self):
-        self.keys();       
-        return self.attributes.values()
-    
-    def items(self):
-        self.keys();       
-        return self.attributes.items()
-    
-    def __getitem__(self,key):
-        self.keys();
-        key = fn.tango.get_full_name(key).lower()
-        return self.attributes[key]
-    
-    def __iter__(self):
-        self.keys();
-        return self.attributes.__iter__()
-            
-    def get_db_config(self,manager='', db_name=''):
-        if not manager:
-            manager = self.get_manager(db_name).name()
-            
-        prop = get_device_property(manager,'LibConfiguration')
-        if prop:
-            config = dict((map(str.strip,l.split('=',1)) for l in prop))
-            db_name,host,user,passwd = \
-                [config.get(k) for k in 'dbname host user password'.split()]
-        else:
-            db_name = get_device_property(manager,'DbName') or ''
-            host = get_device_property(manager,'DbHost') or ''
-            user = get_device_property(manager,'DbUser') or ''
-            passwd = get_device_property(manager,'DbPassword') or ''
-              
-        return db_name,host,user,passwd
-        
-    @staticmethod
-    def get_all_managers():
-        return get_class_devices('HdbConfigurationManager')
-    
-    @staticmethod
-    def get_all_archivers():
-        return get_class_devices('HdbEventSubscriber')
-      
-    def get_manager(self, db_name='', prop=''):
-        if not getattr(self,'manager',None):
-            db_name = db_name or getattr(self,'db_name','')
-            self.manager = ''
-            managers = self.get_all_managers()
-            for m in managers:
-                if db_name:
-                    prop = get_device_property(m,'DbName')
-                    if not prop:
-                        prop = str(get_device_property(m,'LibConfiguration'))
-                if not db_name or db_name in prop:
-                    self.manager = m
-                    break
-                    
-        dp = get_device(self.manager,keep=True) if self.manager else None
-        if not check_device(dp):
-            print('get_manager(%s): %s is not running!' 
-                  % (db_name,self.manager))
-
-        return dp
-      
-    @Cached(depth=10,expire=60.)
-    def get_archived_attributes(self,search=''):
-        #print('get_archived_attributes(%s)'%str(search))
-        attrs = []
-        archs = get_device_property(self.manager,'ArchiverList') 
-            #self.get_manager().ArchiverList
-        self.get_archivers_attributes(archs,full=False,from_db=False)
-        for d,dattrs in self.dedicated.items():
-            for a in dattrs:
-                self.attributes[a].archiver = d
-                if not search or fn.clsearch(search,a):
-                    attrs.append(a)
-        return attrs
-    
-        ## DB API
-        ##r = sorted(str(a).lower().replace('tango://','') 
-        ##THIS METHOD RETURNS ONLY 1000 ATTRIBUTES AS MUCH!!!
-        #r = sorted(parse_tango_model(a,fqdn=True).normalname 
-        #for a in self.get_manager().AttributeSearch(search))
-    
-    @Cached(depth=2,expire=60.)
-    def get_attributes(self,active=None):
-        """
-        Alias for Reader API
-        @TODO active argument not implemented
-        """
-        if active:
-            return self.get_archived_attributes()
-        else:
-            return self.get_attribute_names(False)
-    
-    def get_attributes_failed(self,regexp='*',timeout=3600,from_db=True):
-        if from_db:
-            timeout = fn.now()-timeout
-            attrs = self.get_attributes(True)
-            attrs = fn.filtersmart(attrs,regexp)
-            print('get_attributes_failed([%d])' % len(attrs))
-            print(attrs)
-            vals = self.load_last_values(attrs)
-            return sorted(t for t in vals if not t[1] or
-                         t[1][0] < timeout)
-        else:
-            # Should inspect the Subscribers Error Lists
-            raise Exception('NotImplemented')
-    
-    @Cached(expire=60.)
-    def get_archivers(self):
-        #return list(self.tango.get_device_property(self.manager,'ArchiverList')['ArchiverList'])
-        if self.manager and check_device(self.manager):
-          return self.get_manager().ArchiverList
-        else:
-          raise Exception('%s Manager not running'%self.manager)
-      
-    @Cached(expire=60.)
-    def get_archivers_attributes(self,archs=None,from_db=True,full=False):
-        #print('get_archivers_attributes(%s)' % str(archs))
-        archs = archs or self.get_archivers()
-        dedicated = fn.defaultdict(list)
-        if from_db:
-            for a in archs:
-                dedicated[a] = [str(l) for l in 
-                    get_device_property(a,'AttributeList')]
-                if not full:
-                    dedicated[a] = [str(l).split(';')[0] for l in 
-                        dedicated[a]]
-        else:
-            for a in archs:
-                try:
-                    dedicated[a].extend(get_device(a).AttributeList)
-                except:
-                    dedicated[a] = []
-                    
-        self.dedicated.update(dedicated)
-        return dedicated
-    
-    @Cached(depth=1000,expire=60.)
-    def get_attribute_archiver(self,attribute):
-        if not self.dedicated:
-            self.get_archivers_attributes()
-
-        #m = parse_tango_model(attribute,fqdn=True).fullname
-        m = get_full_name(attribute,fqdn=True)
-        for k,v in self.dedicated.items():
-            for l in v:
-                if m in l.split(';'):
-                    return k
-        return None
-    
-    def start_servers(self,host='',restart=True):
-        import fandango.servers
-        if not self.manager: self.get_manager()
-        astor = fandango.servers.Astor(self.manager)
-        if restart:
-            astor.stop_servers()
-            time.sleep(10.)
-        print('Starting manager ...')
-        astor.start_servers(host=(host or self.host))
-        time.sleep(1.)
-        
-        astor = fandango.servers.Astor()
-        devs = self.get_archivers()
-        astor.load_from_devs_list(devs)
-        if restart:
-            astor.stop_servers()
-            time.sleep(10.)
-        print('Starting archivers ...')
-        astor.start_servers(host=(host or self.host))
-        time.sleep(3.)
-        self.start_devices(force=True)
-        
-    def start_devices(self,regexp = '*', force = False, 
-                      do_init = False, do_restart = False):
-        #devs = fn.tango.get_class_devices('HdbEventSubscriber')
-        devs = self.get_archivers()
-        if regexp:
-            devs = fn.filtersmart(devs,regexp)
-        off = sorted(set(d for d in devs if not fn.check_device(d)))
-
-        if off and do_restart:
-            print('Restarting %s Archiving Servers ...'%self.db_name)
-            astor = fn.Astor()
-            astor.load_from_devs_list(list(off))
-            astor.stop_servers()
-            fn.wait(3.)
-            astor.start_servers()
-            fn.wait(3.)
-
-        for d in devs:
-            try:
-                dp = fn.get_device(d)
-                if do_init:
-                    dp.init()
-                if force or dp.attributenumber != dp.attributestartednumber:
-                    off.append(d)
-                    print('%s.Start()' % d)
-                    dp.start()
-            except Exception,e:
-                self.warning('start_archivers(%s) failed: %s' % (d,e))
-                
-        return off        
-    
-    def add_archiving_manager(self,srv,dev):
-        if '/' not in srv: srv = 'hdb++cm-srv/'+srv
-        add_new_device(srv,'HdbConfigurationManager',dev)
-        prev = get_device_property(dev,'ArchiverList') or []
-        put_device_property(dev,'ArchiverList',prev)
-        put_device_property(dev,'ArchiveName','MySQL')
-        put_device_property(dev,'DbHost',self.host)
-        put_device_property(dev,'DbName',self.db_name)
-        put_device_property(dev,'DbUser',self.user)
-        put_device_property(dev,'DbPassword',self.passwd)
-        put_device_property(dev,'DbPort','3306')
-        put_device_property(dev,'LibConfiguration',[
-          'user='+self.user,
-          'password='+self.passwd,
-          'port='+self.port,
-          'host='+self.host,
-          'dbname='+self.db_name,])
-        self.get_manager()
-        return dev
-
-    def add_event_subscriber(self,srv,dev,libpath=''):
-        if '/' not in srv: srv = 'hdb++es-srv/'+srv
-        add_new_device(srv,'HdbEventSubscriber',dev)
-        manager,dp = self.manager,self.get_manager()
-        props = Struct(get_matching_device_properties(manager,'*'))
-        prev = get_device_property(dev,'AttributeList') or []
-        put_device_property(dev,'AttributeList',prev)
-        #put_device_property(dev,'DbHost',self.host)
-        #put_device_property(dev,'DbName',self.db_name)
-        #put_device_property(dev,'DbUser',self.user)
-        #put_device_property(dev,'DbPassword',self.passwd)
-        #put_device_property(dev,'DbPort','3306')
-        #put_device_property(dev,'DbStartArchivingAtStartup','true')
-        
-        libpath = (libpath or \
-                '/homelocal/sicilia/src/hdbpp.git/lib/libhdb++mysql.so')
-        put_device_property(dev,'LibConfiguration',[
-          'user='+self.user,
-          'password='+self.passwd,
-          'port='+getattr(self,'port','3306'),
-          'host='+self.host,
-          'dbname='+self.db_name,
-          'libname='+libpath,
-          'ligthschema=1',
-          ])
-        if 'ArchiverList' not in props:
-            props.ArchiverList = []
-            
-        dev = parse_tango_model(dev,fqdn=True).fullname
-        #put_device_property(manager,'ArchiverList',
-                            #list(set(list(props.ArchiverList)+[dev])))
-        print(dev)
-        dp.ArchiverAdd(dev)
-        return dev
-    
-    def add_attributes(self,attributes,*args,**kwargs):
-        """
-        Call add_attribute sequentially with a 1s pause between calls
-        :param start: True by default, will force Start() in related archivers
-        See add_attribute? for more help on arguments
-        """
-        try:
-          start = kwargs.get('start',True)
-          for a in attributes:
-            kwargs['start'] = False #Avoid recursive start
-            self.add_attribute(a,*args,**kwargs)
-          time.sleep(3.)
-            
-          if start:
-            archs = set(map(self.get_attribute_archiver,attributes))
-            for h in archs:
-                self.info('%s.Start()' % h)
-                fn.get_device(h).Start()
-                
-        except Exception,e:
-            print('add_attribute(%s) failed!: %s'%(a,traceback.print_exc()))
-        return
+__all__ = ["TaurusDbTreeWidget", "TaurusBaseTreeWidget"]
 
-    def add_attribute(self,attribute,archiver,period=0,
-                      rel_event=None,per_event=300000,abs_event=None,
-                      code_event=False, ttl=None, start=False):
-        """
-        set _event arguments to -1 to ignore them and not modify the database
-        
-        
-        """
-        attribute = parse_tango_model(attribute,fqdn=True).fullname
-        self.info('add_attribute(%s)'%attribute)
-        config = get_attribute_config(attribute)
-        #if 'spectrum' in str(config.data_format).lower():
-          #raise Exception('Arrays not supported yet!')
-        data_type = str(PyTango.CmdArgType.values[config.data_type])
-        if not self.manager: 
-          return False
-      
-        try:
-          d = self.get_manager()
-          d.lock()
-          print('SetAttributeName: %s'%attribute)
-          d.write_attribute('SetAttributeName',attribute)
-          time.sleep(0.2)
-          if period>0:
-            d.write_attribute('SetPollingPeriod',period)
-          if per_event not in (None,-1):
-            d.write_attribute('SetPeriodEvent',per_event)
-
-          if not any((abs_event,rel_event,code_event)):
-            if re.search("short|long",data_type.lower()):
-              abs_event = 1
-            elif not re.search("bool|string",data_type.lower()):
-              rel_event = 1e-2
-          if abs_event not in (None,-1):
-            print('SetAbsoluteEvent: %s'%abs_event)
-            d.write_attribute('SetAbsoluteEvent',abs_event)
-          if rel_event not in (None,-1):
-            d.write_attribute('SetRelativeEvent',rel_event)
-          if ttl not in (None,-1):
-            d.write_attribute('SetTTL',ttl)
-            
-          d.write_attribute('SetCodePushedEvent',code_event)
-
-          d.write_attribute('SetArchiver',archiver)
-          time.sleep(.2)
-          d.AttributeAdd()
-          
-          if start:
-              try:
-                arch = archiver # self.get_attribute_archiver(attribute)
-                self.info('%s.Start()' % (arch))
-                fn.get_device(arch).Start()
-              except:
-                traceback.print_exc()
-              
-        except Exception,e:
-          if 'already archived' not in str(e).lower():
-            self.error('add_attribute(%s,%s,%s): %s'
-                       %(attribute,archiver,period,
-                         traceback.format_exc().replace('\n','')))
-          else:
-            self.warning('%s already archived!' % attribute)
-          return False
-        finally:
-          #self.warning('unlocking %s ..'%self.manager)
-          d.unlock()
-        print('%s added'%attribute)
-        
-    def is_attribute_archived(self,attribute,active=None,cached=True):
-        # @TODO active argument not implemented
-        model = parse_tango_model(attribute,fqdn=True)
-        d = self.get_manager()
-        if d and cached:
-            self.get_archived_attributes()
-            if any(m in self.attributes for m in (attribute,model.fullname,model.normalname)):
-                return model.fullname
-            else:
-                return False
-        elif d:
-            attributes = d.AttributeSearch(model.fullname)
-            a = [a for a in attributes if a.lower().endswith(attribute.lower())]
-            if len(attributes)>1: 
-                raise Exception('MultipleAttributesMatched!')
-            if len(attributes)==1:
-                return attributes[0]
-            else:
-                return False
+__docformat__ = 'restructuredtext'
+
+from taurus.external.qt import Qt
+from taurus.core.taurusbasetypes import TaurusElementType
+from taurus.core.taurusauthority import TaurusAuthority
+#from taurus.qt.qtcore.model import *
+from taurus.qt.qtgui.base import TaurusBaseWidget
+from taurus.qt.qtgui.icon import getElementTypeIcon, getElementTypeIconName
+
+from taurus.qt.qtgui.model import TaurusBaseModelWidget
+from taurus.qt.qtgui.tree.qtree import QBaseTreeWidget
+
+
+from taurus.external.qt import Qt
+from taurus.qt.qtgui.model import QBaseModelWidget, BaseToolBar
+from taurus.qt.qtgui.util import ActionFactory
+from taurus.qt.qtgui.tree import TaurusBaseTreeWidget
+
+from taurus.qt.qtcore.model.taurusdatabasemodel import ElemType, TaurusTreeDbBaseItem
+
+import sys
+from taurus.external.qt import Qt
+import taurus.core
+from taurus.qt.qtgui.container import TaurusWidget
+from taurus.core.util.containers import CaselessList
+from taurus.qt.qtgui.panel.taurusmodellist import TaurusModelList
+
+from PyTangoArchiving.widget.models import *
+from PyTangoArchiving.widget.models import TaurusArchivingDatabase
+from taurus.core.tango.tangodatabase import (TangoDevInfo,TangoAttrInfo)
+
+
+class TaurusModelSelectorTree(TaurusWidget):
+
+    addModels = Qt.pyqtSignal('QStringList')
+
+    def __init__(self, parent=None, selectables=None, buttonsPos=None, designMode=None):
+        TaurusWidget.__init__(self, parent)
+        if selectables is None:
+            selectables = [taurus.core.taurusbasetypes.TaurusElementType.Attribute, taurus.core.taurusbasetypes.TaurusElementType.Member,
+                           taurus.core.taurusbasetypes.TaurusElementType.Device]
+        self._selectables = selectables
+
+        # tree
+        self._deviceTree = TaurusDbTreeWidget(
+            perspective=taurus.core.taurusbasetypes.TaurusElementType.Device)
+        
+        self._deviceTree.getQModel().setSelectables(self._selectables)
+        #self._deviceTree.setUseParentModel(True)
+        self._deviceTree.modelObj = TaurusArchivingDatabase()
+
+        # toolbar
+        self._toolbar = Qt.QToolBar("TangoSelector toolbar")
+        self._toolbar.setIconSize(Qt.QSize(16, 16))
+        self._toolbar.setFloatable(False)
+        self._addSelectedAction = self._toolbar.addAction(
+            Qt.QIcon.fromTheme("list-add"), "Add selected", self.onAddSelected)
+
+        # defines the layout
+        self.setButtonsPos(buttonsPos)
+
+        self._deviceTree.recheckTaurusParent()  # NOT WORKING????
+        # @todo: This is Workaround because UseSetParentModel is giving trouble again!
+        self.modelChanged.connect(self._deviceTree.setModel)
+
+    def setButtonsPos(self, buttonsPos):
+        # we must delete the previous layout before we can set a new one
+        currlayout = self.layout()
+        if currlayout is not None:
+            currlayout.deleteLater()
+            Qt.QCoreApplication.sendPostedEvents(
+                currlayout, Qt.QEvent.DeferredDelete)
+        # add to layout
+        if buttonsPos is None:
+            self.setLayout(Qt.QVBoxLayout())
+            self.layout().addWidget(self._deviceTree)
+        elif buttonsPos == Qt.Qt.BottomToolBarArea:
+            self._toolbar.setOrientation(Qt.Qt.Horizontal)
+            self.setLayout(Qt.QVBoxLayout())
+            self.layout().addWidget(self._deviceTree)
+            self.layout().addWidget(self._toolbar)
+        elif buttonsPos == Qt.Qt.TopToolBarArea:
+            self._toolbar.setOrientation(Qt.Qt.Horizontal)
+            self.setLayout(Qt.QVBoxLayout())
+            self.layout().addWidget(self._toolbar)
+            self.layout().addWidget(self._deviceTree)
+        elif buttonsPos == Qt.Qt.LeftToolBarArea:
+            self._toolbar.setOrientation(Qt.Qt.Vertical)
+            self.setLayout(Qt.QHBoxLayout())
+            self.layout().addWidget(self._toolbar)
+            self.layout().addWidget(self._deviceTree)
+        elif buttonsPos == Qt.Qt.RightToolBarArea:
+            self._toolbar.setOrientation(Qt.Qt.Vertical)
+            self.setLayout(Qt.QHBoxLayout())
+            self.layout().addWidget(self._deviceTree)
+            self.layout().addWidget(self._toolbar)
         else:
-            return any(a.lower().endswith('/'+attribute.lower())
-                                          for a in self.get_attributes())
-          
-    def start_archiving(self,attribute,archiver,period=0,
-                      rel_event=None,per_event=300000,abs_event=None,
-                      code_event=False, ttl=None, start=False):
-        """
-        See HDBpp.add_attribute.__doc__ for a full description of arguments
-        """
+            raise ValueError("Invalid buttons position")
+
+    def getSelectedModels(self):
+        selected = []
         try:
-            if isSequence(attribute):
-                for attr in attribute:
-                    self.start_archiving(attr,*args,**kwargs)
-                    time.sleep(1.)
+            from taurus.core.tango.tangodatabase import (TangoDevInfo,
+                                                         TangoAttrInfo)
+            #from taurus.core.tango.tangodatabase import TangoAttrInfo
+            #from PyTangoArchiving.widget.model import TangoDevInfo
+        except:
+            return selected
+        # TODO: Tango-centric
+        for item in self._deviceTree.selectedItems():
+            nfo = item.itemData()
+            if isinstance(nfo, TangoDevInfo):
+                selected.append(nfo.fullName())
+            elif isinstance(nfo, TangoAttrInfo):
+                selected.append("%s/%s" %
+                                (nfo.device().fullName(), nfo.name()))
             else:
-                self.info('start_archiving(%s)'%attribute)
-                d = self.get_manager()
-                fullname = parse_tango_model(attribute,fqdn=True).fullname
-                if not self.is_attribute_archived(attribute):
-                    self.add_attribute(fullname,archiver=archiver,
-                        period=period, rel_event=rel_event, 
-                        per_event=per_event, abs_event=abs_event,
-                        code_event=code_event, ttl=ttl, 
-                        start=start)
-                    time.sleep(5.)
-                    #fullname = self.is_attribute_archived(attribute,cached=0)
-                d.AttributeStart(fullname)
-                return True
-        except Exception,e:
-            self.error('start_archiving(%s): %s'
-                        %(attribute,traceback.format_exc().replace('\n','')))
-        return False        
-
-    def get_attribute_ID(self,attr):
-        # returns only 1 ID
-        return self.get_attributes_IDs(attr,as_dict=0)[0][1]
-      
-    def get_attributes_IDs(self,name='%',as_dict=1):
-        # returns all matching IDs
-        name = name.replace('*','%')
-        ids = self.Query("select att_name,att_conf_id from att_conf "\
-            +"where att_name like '%s'"%get_search_model(name))
-        if not ids: return None
-        elif not as_dict: return ids
-        else: return dict(ids)
-      
-    def get_attribute_names(self,active=False):
-        if not active:
-            [self.attributes[a[0].lower()] for a 
-                in self.Query('select att_name from att_conf')]
-            return self.attributes.keys()
-        else:
-            return self.get_archived_attributes()
-    
-    @Cached(depth=10000,expire=60.)
-    def get_attribute_modes(self,attr,force=None):
-        """ force argument provided just for compatibility, replaced by cache
-        """
-        aid,tid,table = self.get_attr_id_type_table(attr)
-        r = {'ID':aid, 'MODE_E':fn.tango.get_attribute_events(attr)}
-        r['archiver'] = self.get_attribute_archiver(attr)
-        return r
-      
-    def get_table_name(self,attr):
-        return get_attr_id_type_table(attr)[-1]
-      
-    def get_attr_id_type_table(self,attr):
-        if fn.isNumber(attr):
-            where = 'att_conf_id = %s'%attr
-        else:
-            where = "att_name like '%s'"%get_search_model(attr)
-        q = "select att_name,att_conf_id,att_conf_data_type_id from att_conf"\
-            " where %s"%where
-        ids = self.Query(q)
-        self.debug(str((q,ids)))
-        if not ids: 
-            return None,None,''
-        
-        attr,aid,tid = ids[0]
-        table = self.Query("select data_type from att_conf_data_type "\
-            +"where att_conf_data_type_id = %s"%tid)[0][0]
-
-        self.attributes[attr].id = aid
-        self.attributes[attr].type = table
-        self.attributes[attr].table = 'att_'+table
-        self.attributes[attr].modes = {'MODE_E':True}
-        return aid,tid,'att_'+table
-      
-    def set_attr_event_config(self,attr,polling=0,abs_event=0,
-                              per_event=0,rel_event=0):
-        ac = get_attribute_config(attr)
-        raise Exception('@TODO')
-      
-    #def get_default_archiving_modes(self,attr):
-        #if isString(attr) and '/' in attr:
-          #attr = read_attribute(attr)
-          #pytype = type(attr)
-          
-    def get_attributes_by_table(self,table=''):
-        if table:
-          return self.Query("select att_name from att_conf,att_conf_data_type where data_type like '%s'"+
-                  " and att_conf.att_conf_data_type_id = att_conf_data_type.att_conf_data_type_id")
-        else:
-          types = self.Query("select data_type,att_conf_data_type_id from att_conf_data_type")
-          return dict((t,self.Query("select att_name from att_conf where att_conf_data_type_id = %s"%i))
-                      for t,i in types)
-          
-    #@staticmethod
-    #def decimate_values(values,N=540,method=None):
-        #"""
-        #values must be a sorted (time,...) array
-        #it will be decimated in N equal time intervals 
-        #if method is not provided, only the first value of each interval will be kept
-        #if method is given, it will be applied to buffer to choose the value to keep
-        #first value of buffer will always be the last value kept
-        #"""
-        #tmin,tmax = sorted((values[0][0],values[-1][0]))
-        #result,buff = [values[0]],[values[0]]
-        #interval = float(tmax-tmin)/N
-        #if not method:
-          #for v in values:
-            #if v[0]>=(interval+float(result[-1][0])):
-              #result.append(v)
-        #else:
-          #for v in values:
-            #if v[0]>=(interval+float(result[-1][0])):
-              #result.append(method(buff))
-              #buff = [result[-1]]
-            #buff.append(v)
+                self.info("Unknown item '%s' in selection" % repr(nfo))
+        return selected
 
-        #print(tmin,tmax,N,interval,len(values),len(result),method)
-        #return result
-        
-    def decimate_table(att_id,table):
-        """
-        @TODO
-        """
-        hours = [t0+i*3600 for i in range(24*30)]
-        days = [t0+i*86400 for i in range(30)]
-        dvalues = {}
-        q = ("select count(*) from %s where att_conf_id = %d "
-            "and data_time between '%s' and '%s'")
-        for d in days:
-            s = fn.time2str(d)
-            q = hdbpp.Query(q%(table,att_id,s,fn.time2str(d+86400))
-                            +" and (data_time %% 5) < 2;")
-        sorted(values.items())
-        3600/5
-        for h in hours:
-            s = fn.time2str(h)
-            q = hdbpp.Query("select count(*) from att_scalar_devdouble_ro "
-                "where att_conf_id = 1 and data_time between '%s' and '%s' "
-                "and (data_time %% 5) < 2;"%(s,fn.time2str(h+3600)))
-
-      
-    def get_last_attribute_values(self,table,n=1,
-                                  check_table=False,epoch=None):
-        vals = self.get_attribute_values(
-            table,N=n,human=True,desc=True,stop_date=epoch)
-        if len(vals) and abs(n)==1: 
-            return vals[0]
-        else: 
-            return vals
-    
-    def load_last_values(self,attributes,n=1,epoch=None):
-        return dict((a,self.get_last_attribute_values(a,n=n,epoch=None)) 
-                    for a in fn.toList(attributes))
-        
-    __test__['get_last_attribute_values'] = \
-        [(['bl01/vc/spbx-01/p1'],None,lambda r:len(r)>0)] #should return array
-            
-    @CatchedAndLogged(throw=True)
-    def get_attribute_values(self,table,start_date=None,stop_date=None,
-                             desc=False,N=0,unixtime=True,
-                             extra_columns='quality',decimate=0,human=False,
-                             as_double=True,
-                             **kwargs):
-        """
-        This method returns values between dates from a given table.
-        If stop_date is not given, then anything above start_date is returned.
-        desc controls the sorting of values
-        
-        unixtime = True enhances the speed of querying by a 60%!!!! 
-            #(due to MySQLdb implementation of datetime)
-        
-        If N is specified:
-        
-            * Query will return last N values if there's no stop_date
-            * If there is, then it will return the first N values (windowing?)
-            * IF N is negative, it will return the last N values instead
-            
-        start_date and stop_date must be in a format valid for SQL
-        """
-        t0 = time.time()
-        self.debug('HDBpp.get_attribute_values(%s,%s,%s,%s,decimate=%s,%s)'
-              %(table,start_date,stop_date,N,decimate,kwargs))
-        if fn.isSequence(table):
-            aid,tid,table = table
-        else:
-            aid,tid,table = self.get_attr_id_type_table(table)
-            
-        if not all((aid,tid,table)):
-            self.warning('%s is not archived' % table)
-            return []
-            
-        human = kwargs.get('asHistoryBuffer',human)
-            
-        what = 'UNIX_TIMESTAMP(data_time)' if unixtime else 'data_time'
-        if as_double:
-            what = 'CAST(%s as DOUBLE)' % what
-        if 'array' in table: what+=",idx"
-        what += ',value_r' if 'value_r' in self.getTableCols(table) \
-                                else ',value'
-        if extra_columns: what+=','+extra_columns
-        interval = 'where att_conf_id = %s'%aid if aid is not None \
-                                                else 'where att_conf_id >= 0 '
-
-        if start_date or stop_date:
-          start_date,start_time,stop_date,stop_time = \
-              Reader.get_time_interval(start_date,stop_date)
-          if start_date and stop_date:
-            interval += (" and data_time between '%s' and '%s'"
-                            %(start_date,stop_date))
-          elif start_date and fandango.str2epoch(start_date):
-            interval += " and data_time > '%s'"%start_date
-            
-        query = 'select %s from %s %s order by data_time' \
-                        % (what,table,interval)
-                    
-        if N == 1:
-            human = 1
-        if N<0 or desc: 
-            query+=" desc" # or (not stop_date and N>0):
-        if N: 
-            query+=' limit %s'%abs(N) # if 'array' not in table else 1024)
-        
-        ######################################################################
-        # QUERY
-        self.debug(query)
+    def onAddSelected(self):
+        self.addModels.emit(self.getSelectedModels())
+
+    def treeView(self):
+        return self._deviceTree.treeView()
+
+    @classmethod
+    def getQtDesignerPluginInfo(cls):
+        ret = TaurusWidget.getQtDesignerPluginInfo()
+        ret['module'] = 'taurus.qt.qtgui.panel'
+        ret['icon'] = "designer:listview.png"
+        ret['container'] = False
+        ret['group'] = 'Taurus Views'
+        return ret
+
+
+class TaurusModelChooser(TaurusWidget):
+    '''A widget that allows the user to select a list of models from a tree representing
+    devices and attributes from a Tango server.
+
+    The user selects models and adds them to a list. Then the user should click on the
+    update button to notify that the selection is ready.
+
+    signals::
+      - "updateModels"  emitted when the user clicks on the update button. It
+        passes a list<str> of models that have been selected.
+    '''
+
+    updateModels = Qt.pyqtSignal('QStringList')
+    UpdateAttrs = Qt.pyqtSignal(['QStringList'], ['QMimeData'])
+
+    def __init__(self, parent=None, selectables=None, host=None, designMode=None, singleModel=False):
+        '''Creator of TaurusModelChooser
+
+        :param parent: (QObject) parent for the dialog
+        :param selectables: (list<TaurusElementType>) if passed, only elements of the tree whose
+                            type is in the list will be selectable.
+        :param host: (QObject) Tango host to be explored by the chooser
+        :param designMode: (bool) needed for taurusdesigner but ignored here
+        :param singleModel: (bool) If True, the selection will be of just one
+                            model. Otherwise (default) a list of models can be selected
+        '''
+        TaurusWidget.__init__(self, parent)
+        if host is None:
+            host = taurus.Authority().getNormalName()
+
+        self._allowDuplicates = False
+
+        self.setLayout(Qt.QVBoxLayout())
+
+        self.tree = TaurusModelSelectorTree(
+            selectables=selectables, buttonsPos=Qt.Qt.BottomToolBarArea)
+        self.tree.setModel(host)
+        self.list = TaurusModelList()
+        self.list.setSelectionMode(Qt.QAbstractItemView.ExtendedSelection)
+        applyBT = Qt.QToolButton()
+        applyBT.setToolButtonStyle(Qt.Qt.ToolButtonTextBesideIcon)
+        applyBT.setText('Apply')
+        applyBT.setIcon(Qt.QIcon("status:available.svg"))
+
+        self.setSingleModelMode(singleModel)
+
+        # toolbar
+        self._toolbar = self.tree._toolbar
+        self._toolbar.addAction(self.list.removeSelectedAction)
+        self._toolbar.addAction(self.list.removeAllAction)
+        self._toolbar.addAction(self.list.moveUpAction)
+        self._toolbar.addAction(self.list.moveDownAction)
+        self._toolbar.addSeparator()
+        self._toolbar.addWidget(applyBT)
+        self.layout().addWidget(self.tree)
+        self.layout().addWidget(self.list)
+
+        # self.tree.setUseParentModel(True)  #It does not work!!!!
+        # @todo: This is Workaround because UseSetParentModel is giving trouble again!
+        self.modelChanged.connect(self.tree.setModel)
+
+        # connections:
+        self.tree.addModels.connect(self.addModels)
+        applyBT.clicked.connect(self._onUpdateModels)
+#        self.connect(self.tree._deviceTree, Qt.SIGNAL("itemDoubleClicked"), self.onTreeDoubleClick)
+
+#    def onTreeDoubleClick(self, item, colum): #@todo: Implement this function properly
+#        if item.Role in self.tree._selectables:
+#            self.addModels([str(item.text())])
+
+    def getListedModels(self, asMimeData=False):
+        '''returns the list of models that have been added
+
+        :param asMimeData: (bool) If False (default), the return value will be a
+                           list of models. If True, the return value is a
+                           `QMimeData` containing at least `TAURUS_MODEL_LIST_MIME_TYPE`
+                           and `text/plain` MIME types. If only one model was selected,
+                           the mime data also contains a TAURUS_MODEL_MIME_TYPE.
+
+        :return: (list<str> or QMimeData) the type of return depends on the value of `asMimeData`'''
+        models = self.list.getModelList()
+        if self.isSingleModelMode():
+            models = models[:1]
+        if asMimeData:
+            md = Qt.QMimeData()
+            md.setData(taurus.qt.qtcore.mimetypes.TAURUS_MODEL_LIST_MIME_TYPE, str(
+                "\r\n".join(models)))
+            md.setText(", ".join(models))
+            if len(models) == 1:
+                md.setData(
+                    taurus.qt.qtcore.mimetypes.TAURUS_MODEL_MIME_TYPE, str(models[0]))
+            return md
+        return models
+
+    def setListedModels(self, models):
+        '''adds the given list of models to the widget list
+        '''
+        self.list.model().clearAll()
+        self.list.addModels(models)
+
+    def resetListedModels(self):
+        '''equivalent to setListedModels([])'''
+        self.list.model().clearAll()
+
+    def updateList(self, attrList):
+        '''for backwards compatibility with AttributeChooser only. Use :meth:`setListedModels` instead'''
+        self.info(
+            'ModelChooser.updateList() is provided for backwards compatibility only. Use setListedModels() instead')
+        self.setListedModels(attrList)
+
+    def addModels(self, models):
+        ''' Add given models to the selected models list'''
+        if len(models) == 0:
+            models = ['']
+        if self.isSingleModelMode():
+            self.resetListedModels()
+        if self._allowDuplicates:
+            self.list.addModels(models)
+        else:
+            listedmodels = CaselessList(self.getListedModels())
+            for m in models:
+                if m not in listedmodels:
+                    listedmodels.append(m)
+                    self.list.addModels([m])
+
+    def onRemoveSelected(self):
+        '''
+        Remove the list-selected models from the list
+        '''
+        self.list.removeSelected()
+
+    def _onUpdateModels(self):
+        models = self.getListedModels()
+        self.updateModels.emit(models)
+        if taurus.core.taurusbasetypes.TaurusElementType.Attribute in self.tree._selectables:
+            # for backwards compatibility with the old AttributeChooser
+            self.UpdateAttrs.emit(models)
+
+    def setSingleModelMode(self, single):
+        '''sets whether the selection should be limited to just one model
+        (single=True) or not (single=False)'''
+        if single:
+            self.tree.treeView().setSelectionMode(Qt.QAbstractItemView.SingleSelection)
+        else:
+            self.tree.treeView().setSelectionMode(Qt.QAbstractItemView.ExtendedSelection)
+        self._singleModelMode = single
+
+    def isSingleModelMode(self):
+        '''returns True if the selection is limited to just one model. Returns False otherwise.
+
+        :return: (bool)'''
+        return self._singleModelMode
+
+    def resetSingleModelMode(self):
+        '''equivalent to setSingleModelMode(False)'''
+        self.setSingleModelMode(self, False)
+
+    @staticmethod
+    def modelChooserDlg(parent=None, selectables=None, host=None, asMimeData=False, singleModel=False, windowTitle='Model Chooser'):
+        '''Static method that launches a modal dialog containing a TaurusModelChooser
+
+        :param parent: (QObject) parent for the dialog
+        :param selectables: (list<TaurusElementType>) if passed, only elements of the tree whose
+                            type is in the list will be selectable.
+        :param host: (QObject) Tango host to be explored by the chooser
+        :param asMimeData: (bool) If False (default),  a list of models will be.
+                           returned. If True, a `QMimeData` object will be
+                           returned instead. See :meth:`getListedModels` for a
+                           detailed description of this QMimeData object.
+        :param singleModel: (bool) If True, the selection will be of just one
+                            model. Otherwise (default) a list of models can be selected
+        :param windowTitle: (str) Title of the dialog (default="Model Chooser")
+
+        :return: (list,bool or QMimeData,bool) Returns a models,ok tuple. models can be
+                 either a list of models or a QMimeData object, depending on
+                 `asMimeData`. ok is True if the dialog was accepted (by
+                 clicking on the "update" button) and False otherwise
+        '''
+        dlg = Qt.QDialog(parent)
+        dlg.setWindowTitle(windowTitle)
+        dlg.setWindowIcon(Qt.QIcon("logos:taurus.png"))
+        layout = Qt.QVBoxLayout()
+        w = TaurusModelChooser(
+            parent=parent, selectables=selectables, host=host, singleModel=singleModel)
+        layout.addWidget(w)
+        dlg.setLayout(layout)
+        w.updateModels.connect(dlg.accept)
+        dlg.exec_()
+        return w.getListedModels(asMimeData=asMimeData), (dlg.result() == dlg.Accepted)
+
+    @classmethod
+    def getQtDesignerPluginInfo(cls):
+        ret = TaurusWidget.getQtDesignerPluginInfo()
+        ret['module'] = 'taurus.qt.qtgui.panel'
+        ret['icon'] = "designer:listview.png"
+        ret['container'] = False
+        ret['group'] = 'Taurus Views'
+        return ret
+
+    singleModelMode = Qt.pyqtProperty(
+        "bool", isSingleModelMode, setSingleModelMode, resetSingleModelMode)
+
+
+## From TaurusPlot
+def showDataImportDlg(self,trend):
+    '''Launches the data import dialog. This dialog lets the user manage
+    which attributes are attached to the plot (using
+    :class:`TaurusModelChooser`) and also to generate raw data or import it
+    from files
+    '''
+    if self.DataImportDlg is None:
+        from taurus.qt.qtgui.panel import TaurusModelChooser
+        self.DataImportDlg = Qt.QDialog(self)
+        self.DataImportDlg.setWindowTitle(
+            "%s - Import Data" % (str(trend.windowTitle())))
+        self.DataImportDlg.modelChooser = TaurusModelChooser(
+            selectables=[taurus.core.taurusbasetypes.TaurusElementType.Attribute])
+        from taurus.qt.qtgui.panel import QRawDataWidget
+        self.DataImportDlg.rawDataChooser = QRawDataWidget()
+
+        tabs = Qt.QTabWidget()
+        tabs.addTab(self.DataImportDlg.modelChooser, "&Attributes")
+        tabs.addTab(self.DataImportDlg.rawDataChooser, "&Raw Data")
+        mainlayout = Qt.QVBoxLayout(self.DataImportDlg)
+        mainlayout.addWidget(tabs)
+
+        self.DataImportDlg.modelChooser.updateModels.connect(trend.setModel)
+        self.DataImportDlg.rawDataChooser.ReadFromFiles.connect(trend.readFromFiles)
+        self.DataImportDlg.rawDataChooser.AddCurve.connect(trend.attachRawData)
+
+    models_and_display = [(m, trend.getCurveTitle(
+        m.split('|')[-1])) for m in trend._modelNames]
+
+    self.DataImportDlg.modelChooser.setListedModels(models_and_display)
+    self.DataImportDlg.show()
+    
+    
+class TaurusTreeDeviceItem(TaurusTreeDbBaseItem):
+    """A node designed to represent a device"""
+
+    def child(self, row):
+        self.updateChilds()
+        return super(TaurusTreeDeviceItem, self).child(row)
+
+    def hasChildren(self):
+        return True
+        nb = super(TaurusTreeDeviceItem, self).childCount()
+        if nb > 0:
+            return True
+        data = self.itemData()
+        #if data.state() != TaurusDevState.Ready:
+            #return False
+        return True
+
+    def childCount(self):
+        nb = super(TaurusTreeDeviceItem, self).childCount()
+        if nb > 0:
+            return nb
+        data = self.itemData()
+        #if data.state() != TaurusDevState.Ready:
+            #return 0
+        self.updateChilds()
+        return super(TaurusTreeDeviceItem, self).childCount()
+
+    def updateChilds(self):
+        if len(self._childItems) > 0:
+            return
+        print(type(self._model),self._model,type(self._itemData),self._itemData)
+        print(self.itemData().name)
+        attrs = self._model.dataSource().get_device_attribute_list(self.itemData().name())
+        print(attrs)
+        for attr in attrs:
+            #for attr in self._itemData.attributes():
+            attr = TangoAttrInfo(self.itemData().container(), name = attr.lower(),
+                full_name = (self.itemData().name()+'/'+attr).lower(), device = self.itemData(),
+                info = None)
+            c = TaurusTreeAttributeItem(self._model, attr, self)
+            self.appendChild(c)
+        return
+
+    def data(self, index):
+        column, model = index.column(), index.model()
+        role = model.role(column, self.depth())
+        obj = self.itemData()
+        if role == ElemType.Device or role == ElemType.Name:
+            return obj.name()
+        elif role == ElemType.DeviceAlias:
+            return obj.alias()
+        elif role == ElemType.Server:
+            return obj.server().name()
+        elif role == ElemType.DeviceClass:
+            return obj.klass().name()
+        elif role == ElemType.Exported:
+            return obj.state()
+        elif role == ElemType.Host:
+            return obj.host()
+        elif role == ElemType.Domain:
+            return obj.domain()
+        elif role == ElemType.Family:
+            return obj.family()
+        elif role == ElemType.Member:
+            return obj.member()
+
+    def mimeData(self, index):
+        return self.itemData().fullName()
+
+    def role(self):
+        return ElemType.Device    
+    
+
+class TaurusDbDeviceProxyModel(TaurusDbBaseProxyModel):
+    """A Qt filter & sort model for model for the taurus models:
+           - TaurusDbBaseModel
+           - TaurusDbDeviceModel
+           - TaurusDbSimpleDeviceModel
+           - TaurusDbPlainDeviceModel"""
+
+    def filterAcceptsRow(self, sourceRow, sourceParent):
+        sourceModel = self.sourceModel()
+        idx = sourceModel.index(sourceRow, 0, sourceParent)
+        treeItem = idx.internalPointer()
+        regexp = self.filterRegExp()
+
+        # if domain node, check if it will potentially have any children
+        if isinstance(treeItem, TaurusTreeDeviceDomainItem):
+            domain = treeItem.display()
+            devices = sourceModel.getDomainDevices(domain)
+            for device in devices:
+                if self.deviceMatches(device, regexp):
+                    return True
+            return False
+
+        # if family node, check if it will potentially have any children
+        if isinstance(treeItem, TaurusTreeDeviceFamilyItem):
+            domain = treeItem.parent().display()
+            family = treeItem.display()
+            devices = sourceModel.getFamilyDevices(domain, family)
+            for device in devices:
+                if self.deviceMatches(device, regexp):
+                    return True
+            return False
+
+        if isinstance(treeItem, TaurusTreeDeviceItem) or \
+           isinstance(treeItem, TaurusTreeSimpleDeviceItem) or \
+           isinstance(treeItem, TaurusTreeDeviceMemberItem):
+            device = treeItem.itemData()
+            return self.deviceMatches(device, regexp)
+        return True
+
+    def deviceMatches(self, device, regexp):
+        name = device.name()
+
+        # if Qt.QString(name).contains(regexp):
+        if regexp.indexIn(name) != -1:
+            return True
+        name = device.alias()
+        if name is None:
+            return False
+        # return Qt.QString(name).contains(regexp)
+        return regexp.indexIn(name) != -1
+
+
+class TaurusDbDeviceModel(TaurusDbBaseModel):
+    """A Qt model that structures device elements in a 3 level tree organized
+       as:
+
+           - <domain>
+           - <family>
+           - <member>"""
+    ColumnRoles = (ElemType.Device, ElemType.Domain, ElemType.Family, ElemType.Member,
+                   ElemType.Attribute), ElemType.DeviceAlias, ElemType.Server, ElemType.DeviceClass, ElemType.Exported, ElemType.Host
+    
+    def __init__(self,*args,**kwargs):
+        super(TaurusDbDeviceModel, self).__init__(*args,**kwargs)
+        self.setDataSource(TaurusArchivingDatabase())
+
+    def setupModelData(self, data):
+        if data is None:
+            return
         try:
-            result = self.Query(query)
-        except MySQLdb.ProgrammingError as e:
-            if 'DOUBLE' in str(e) and "as DOUBLE" in query:
-                return self.get_attribute_values((aid,tid,table),start_date,
-                    stop_date,desc,N,unixtime,extra_columns,decimate,human,
-                    as_double=False,**kwargs)
-            
-        self.debug('read [%d] in %f s'%(len(result),time.time()-t0))
-        t0 = time.time()
-        if not result or not result[0]: return []
-        ######################################################################
-
-        if 'array' in table:
-            data = fandango.dicts.defaultdict(list)
-            for t in result:
-                data[float(t[0])].append(t[1:])
-            result = []
-            for k,v in sorted(data.items()):
-                l = [0]*(1+max(t[0] for t in v))
-                for i,t in enumerate(v):
-                    if None in t: 
-                        l = None
-                        break
-                    l[t[0]] = t[1] #Ignoring extra columns (e.g. quality)
-                result.append((k,l))
-            if N > 0: 
-                #for k,l in result:
-                    #print((k,l and len(l)))
-                result = result[-N:]
-            self.debug('array arranged [%d] in %f s'
-                         % (len(result),time.time()-t0))
-            t0 = time.time()
-          
-        # Converting the timestamp from Decimal to float
-        # Weird results may appear in filter_array comparison if not done
-        # Although it is INCREDIBLY SLOW!!!
-        #result = []
-        #nr = []
-        #if len(result[0]) == 2: 
-            #for i,t in enumerate(result):
-                #result[i] = (float(t[0]),t[1])
-        #elif len(result[0]) == 3: 
-            #for i,t in enumerate(result):
-                #result[i] = (float(t[0]),t[1],t[2])
-        #elif len(result[0]) == 4: 
-           #for i,t in enumerate(result):
-                #result[i] = ((float(t[0]),t[1],t[2],t[3]))
+            # TODO: Tango-centric
+            # TODO: is this try needed? (not done in, e.g. TaurusDbPlainDeviceModel)
+            from taurus.core.tango.tangodatabase import TangoDatabase
+        except ImportError:
+            return
+        if isinstance(data, TangoDatabase):
+            data = data.deviceTree()
+
+        rootItem = self._rootItem
+        for domain in data.keys():
+            families = data[domain]
+            domainItem = TaurusTreeDeviceDomainItem(
+                self, domain.upper(), rootItem)
+            for family in families.keys():
+                members = families[family]
+                familyItem = TaurusTreeDeviceFamilyItem(
+                    self, family.upper(), domainItem)
+                for member in members.keys():
+                    dev = members[member]
+                    memberItem = TaurusTreeDeviceItem(
+                        self, dev, parent=familyItem)
+                    familyItem.appendChild(memberItem)
+                domainItem.appendChild(familyItem)
+            rootItem.appendChild(domainItem)
+
+
+class TaurusDbTreeWidget(TaurusBaseTreeWidget):
+    """A class:`taurus.qt.qtgui.tree.TaurusBaseTreeWidget` that connects to a
+    :class:`taurus.core.taurusauthority.TaurusAuthority` model. It can show the list of database
+    elements in four different perspectives:
+
+    - device : a three level hierarchy of devices (domain/family/name)
+    - server : a server based perspective
+    - class : a class based perspective
+
+    Filters can be inserted into this widget to restrict the tree nodes that are
+    seen.
+    """
+
+    KnownPerspectives = {
+        TaurusElementType.Device: {
+            "label": "By device",
+            "icon": getElementTypeIconName(TaurusElementType.Device),
+            "tooltip": "View by device tree",
+            "model": [TaurusDbDeviceProxyModel, TaurusDbDeviceModel, ],
+        },
+        'PlainDevice': {
+            "label": "By plain device",
+            "icon": getElementTypeIconName(TaurusElementType.Device),
+            "tooltip": "View by plain device tree (it may take a long time if there are problems with the exported devices)",
+            "model": [TaurusDbDeviceProxyModel, TaurusDbPlainDeviceModel, ],
+        },
+
+        TaurusElementType.Server: {
+            "label": "By server",
+            "icon": getElementTypeIconName(TaurusElementType.Server),
+            "tooltip": "View by server tree",
+            "model": [TaurusDbServerProxyModel, TaurusDbServerModel, ],
+        },
+        TaurusElementType.DeviceClass: {
+            "label": "By class",
+            "icon": getElementTypeIconName(TaurusElementType.DeviceClass),
+            "tooltip": "View by class tree",
+            "model": [TaurusDbDeviceClassProxyModel, TaurusDbDeviceClassModel, ],
+        },
+    }
+
+    DftPerspective = TaurusElementType.Device
+
+    def getModelClass(self):
+        return TaurusAuthority
+
+    def sizeHint(self):
+        return Qt.QSize(1024, 512)
+    
+    @Qt.pyqtSlot('QString')
+    def setModel(self, model, obj=None):
+        """Sets/unsets the model name for this component
+
+        :param model: (str) the new model name"""
+        super(TaurusDbTreeWidget, self).setModel(model)
+        self.modelObj = obj
+        
+    def _attach(self):
+        """Attaches the component to the taurus model.
+        In general it should not be necessary to overwrite this method in a
+        subclass.
+
+        :return: (bool) True if success in attachment or False otherwise.
+        """
+        if self.isAttached():
+            return self._attached
+
+        self.preAttach()
+
+        #if cls is None:
+            #self._attached = False
+            ##self.trace("Failed to attach: Model class not found")
+        #elif self.modelName == '':
+            #self._attached = False
+            #self.modelObj = None
         #else:
-            #for i,t in enumerate(result):
-                #result[i] = ([float(t[0])]+t[1:])
-        
-        self.debug('timestamp arranged [%d] in %f s'
-                     % (len(result),time.time()-t0))
-        t0 = time.time()
-            
-        # Decimation to be done in Reader object
-        #if decimate:
-            ## When called from trends, decimate may be the decimation method
-            ## or the maximum sample number
             #try:
-                #N = int(decimate)
-                ##decimate = data_has_changed
-                #decimate = 
-                #result = PyTangoArchiving.reader.decimation(
-                                        #result,decimate,window=0,N=N)                
-            #except:
-                ##N = 1080
-                #result = PyTangoArchiving.reader.decimation(result,decimate) 
-        
-        if human: 
-            result = [list(t)+[fn.time2str(t[0])] for t in result]
+                #self.modelObj = taurus.Manager().getObject(cls, self.modelName)
+                #if self.modelObj is not None:
+                    #self.modelObj.addListener(self)
+                    #self._attached = True
+                    #self.changeLogName(self.log_name + "." + self.modelName)
+            #except Exception:
+                #self.modelObj = None
+                #self._attached = False
+                #self.debug(
+                    #"Exception occured while trying to attach '%s'" % self.modelName)
+                #self.traceback()
+
+        self.postAttach()
+        return self._attached           
+
+    @classmethod
+    def getQtDesignerPluginInfo(cls):
+        ret = TaurusBaseWidget.getQtDesignerPluginInfo()
+        ret['module'] = 'taurus.qt.qtgui.tree'
+        ret['group'] = 'Taurus Views'
+        ret['icon'] = "designer:listview.png"
+        return ret
+
+
+#class _TaurusTreePanel(Qt.QWidget, TaurusBaseWidget):
+    #"""A demonstration panel to show how :class:`taurus.qt.qtcore.TaurusDbBaseModel`
+    #models can interact with several model view widgets like QTreeView,
+    #QTableView, QListView and QComboBox"""
+
+    #def __init__(self, parent=None, designMode=False):
+        #"""doc please!"""
+        #name = self.__class__.__name__
+        #self.call__init__wo_kw(Qt.QWidget, parent)
+        #self.call__init__(TaurusBaseWidget, name, designMode=designMode)
+        #self.init(designMode)
+
+    #def init(self, designMode):
+        #l = Qt.QGridLayout()
+        #l.setContentsMargins(0, 0, 0, 0)
+        #self.setLayout(l)
+
+##        tb = self._toolbar = Qt.QToolBar("Taurus tree panel toolbar")
+##        tb.setFloatable(False)
+##        refreshAction = self._refreshAction = tb.addAction(Qt.QIcon.fromTheme("view-refresh"),"Refresh", self.refresh)
+
+##        l.addWidget(tb, 0, 0)
+
+        #main_panel = Qt.QTabWidget()
+        #self._device_tree_view = TaurusDbTreeWidget(
+            #perspective=TaurusElementType.Device)
+        #self._device_table_view = Qt.QTableView()
+        #self._device_table_view.setModel(TaurusDbBaseModel())
+        #self._device_list_view = Qt.QListView()
+        #self._device_list_view.setModel(TaurusDbSimpleDeviceModel())
+        #self._server_tree_view = TaurusDbTreeWidget(
+            #perspective=TaurusElementType.Server)
+        #self._class_tree_view = TaurusDbTreeWidget(
+            #perspective=TaurusElementType.DeviceClass)
+
+        #self._device_combo_view = Qt.QWidget()
+        #combo_form = Qt.QFormLayout()
+        #self._device_combo_view.setLayout(combo_form)
+
+        #self._combo_dev_tree_widget = TaurusDbTreeWidget(
+            #perspective=TaurusElementType.Device)
+        #qmodel = self._combo_dev_tree_widget.getQModel()
+        #qmodel.setSelectables([TaurusElementType.Member])
+        #device_combo = Qt.QComboBox()
+        #device_combo.setModel(qmodel)
+        #device_combo.setMaxVisibleItems(20)
+        #device_combo.setView(self._combo_dev_tree_widget.treeView())
+        #combo_form.addRow(
+            #"Device selector (by device hierarchy):", device_combo)
+
+        #self._combo_attr_tree_widget = TaurusDbTreeWidget(
+            #perspective=TaurusElementType.Device)
+        #qmodel = self._combo_attr_tree_widget.getQModel()
+        #device_combo = Qt.QComboBox()
+        #device_combo.setModel(qmodel)
+        #device_combo.setMaxVisibleItems(20)
+        #device_combo.setView(self._combo_attr_tree_widget.treeView())
+        #combo_form.addRow(
+            #"Attribute selector (by device hierarchy):", device_combo)
+
+        #self._combo_dev_table_view = Qt.QTableView()
+        #self._combo_dev_table_view.setModel(TaurusDbBaseModel())
+        #qmodel = self._combo_dev_table_view.model()
+        #qmodel.setSelectables([TaurusElementType.Device])
+        #device_combo = Qt.QComboBox()
+        #device_combo.setModel(qmodel)
+        #device_combo.setMaxVisibleItems(20)
+        #device_combo.setView(self._combo_dev_table_view)
+        #combo_form.addRow("Device selector (by plain device):", device_combo)
+
+        #main_panel.addTab(self._device_tree_view, "Device (Tree View)")
+        #main_panel.addTab(self._device_table_view, "Device (Table View)")
+        #main_panel.addTab(self._device_list_view, "Device (List View)")
+        #main_panel.addTab(self._server_tree_view, "Server (Tree View)")
+        #main_panel.addTab(self._class_tree_view, "Class (Tree View)")
+        #main_panel.addTab(self._device_combo_view, "ComboBox Views")
+
+        #l.addWidget(main_panel, 1, 0)
+
+        #self._main_panel = main_panel
+
+    #def deviceTreeWidget(self):
+        #return self._device_tree_view
+
+    #def deviceTableWidget(self):
+        #return self._device_table_view
+
+    #def deviceListWidget(self):
+        #return self._device_list_view
+
+    #def serverTreeWidget(self):
+        #return self._server_tree_view
+
+    #def classTreeWidget(self):
+        #return self._class_tree_view
+
+    #def sizeHint(self):
+        #return Qt.QSize(1024, 512)
+
+    #def _updateTreeModels(self):
+        #db_name, db = self.getModel(), self.getModelObj()
+
+        #self._device_tree_view.setModel(db_name)
+
+        #model = self._device_table_view.model()
+        #if model is not None:
+            #model.setDataSource(db)
+
+        #model = self._device_list_view.model()
+        #if model is not None:
+            #model.setDataSource(db)
+
+        #self._server_tree_view.setModel(db_name)
+        #self._class_tree_view.setModel(db_name)
+        #self._combo_dev_tree_widget.setModel(db_name)
+        #self._combo_attr_tree_widget.setModel(db_name)
+
+        #model = self._combo_dev_table_view.model()
+        #if model is not None:
+            #model.setDataSource(db)
+
+    #def refresh(self):
+        #db = self.getModelObj()
+        #if db is None:
+            #return
+        #db.refreshCache()
+        #self._device_tree_view.refresh()
+        #self._device_table_view.model().refresh()
+        #self._device_list_view.model().refresh()
+        #self._server_tree_view.refresh()
+        #self._class_tree_view.refresh()
+
+    #def goIntoTree(self):
+        #index = self._device_tree_view.currentIndex()
+        #if index is None:
+            #return
+        ##index_parent = index.parent()
+        ## if index_parent is None:
+        ##    return
+        #self._device_tree_view.setRootIndex(index)
+
+    #def goUpTree(self):
+        #index = self._device_tree_view.rootIndex()
+        #if index is None:
+            #return
+        #index_parent = index.parent()
+        #if index_parent is None:
+            #return
+        #self._device_tree_view.setRootIndex(index_parent)
+
+    ##-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
+    ## TaurusBaseWidget overwriting
+    ##-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
+
+    #def getModelClass(self):
+        #return TaurusAuthority
+
+    #@Qt.pyqtSlot('QString')
+    #def setModel(self, model, obj=None):
+        #"""Sets/unsets the model name for this component
+
+        #:param model: (str) the new model name"""
+        #super(_TaurusTreePanel, self).setModel(model)
+        #self.modelObj = obj
+        #self._updateTreeModels()
+        
+    #def _attach(self):
+        #"""Attaches the component to the taurus model.
+        #In general it should not be necessary to overwrite this method in a
+        #subclass.
 
-        if not desc and ((not stop_date and N>0) or (N<0)):
-            #THIS WILL BE APPLIED ONLY WHEN LAST N VALUES ARE ASKED
-            #self.warning('reversing ...' )
-            result = list(reversed(result))
-        else:
-            # why?
-            self.getCursor(klass=MySQLdb.cursors.SSCursor)
+        #:return: (bool) True if success in attachment or False otherwise.
+        #"""
+        #if self.isAttached():
+            #return self._attached
 
-        self.debug('result arranged [%d]'%len(result))            
-        return result
-        
-    def get_attributes_values(self,tables='',start_date=None,stop_date=None,
-                desc=False,N=0,unixtime=True,extra_columns='quality',
-                decimate=0,human=False):
-        
-        if not fn.isSequence(tables):
-            tables = self.get_archived_attributes(tables)
-            
-        return dict((t,self.get_attribute_values(t,start_date,stop_date,desc,
-                N,unixtime,extra_columns,decimate,human))
-                for t in tables)
-
-    def get_attribute_rows(self,attribute,start_date=0,stop_date=0):
-        aid,tid,table = self.get_attr_id_type_table(attribute)
-        if start_date and stop_date:
-            dates = map(time2str,(start_date,stop_date))
-            where = "and data_time between '%s' and '%s'" % dates
-        else:
-            where = ''
-        r = self.Query('select count(*) from %s where att_conf_id = %s'
-                          % ( table, aid) + where)
-        return r[0][0] if r else 0
-    
-    def get_failed_attributes(self,t=7200):
-        vals = self.load_last_values(self.get_attributes())
-        nones = [k for k,v in vals.items() 
-                    if (not v or v[1] is None)]
-        nones = [k for k in nones if fn.read_attribute(k) is not None]
-        lost = [k for k,v in vals.items() 
-                if k not in nones and v[0] < fn.now()-t]
-        lost = [k for k in lost if fn.read_attribute(k) is not None]
-        failed = nones+lost
-        return sorted(failed)
-    
-    def restart_attribute(self,attr, d=''):
-        try:
-            d = self.get_attribute_archiver(attr)
-            print('%s.restart_attribute(%s)' % (d,attr))
-            dp = fn.get_device(d,keep=True)
-
-            if not fn.check_device(dp):
-                self.start_devices('(.*/)?'+d,do_restart=True)
-                
-            dp.AttributeStop(attr)
-            fn.wait(.1)
-            dp.AttributeStart(attr)
-        except:
-            print('%s.AttributeStart(%s) failed!'%(d,attr))
-        
-    def restart_attributes(self,attributes=None):
-        if attributes is None:
-            attributes = self.get_failed_attributes()
-
-        for a in sorted(attributes):
-            self.restart_attribute(a)
-            
-        print('%d attributes restarted' % len(attributes))
-    
-    def check_attributes(self,attrs = '', load = False, t0 = 0):
-        
-        db,t0,result,vals = self,t0 or fn.now(),{},{}
-        print('Checking %s' % str(db))
+        #self.preAttach()
 
-        if fn.isDictionary(attrs):
-            attrs,vals = attrs.keys(),attrs
-            if isinstance(vals.values()[0],dict):
-                vals = dict((k,v.values()[0]) for k,v in vals.items())
-        else:
-            if fn.isString(attrs):
-                attrs = fn.filtersmart(db.get_attributes(),attrs)
-                load = True
-
-        if load:
-            [vals.update(db.load_last_values(a)) for a in attrs]
-
-        print('\t%d attributes'%len(attrs))
-        result['attrs'] = attrs
-        result['vals'] = vals
-        result['novals'] = [a for a,v in vals.items() if not v]
-        result['nones'],result['down'],result['lost'] = [],[],[]
-        for a,v in vals.items():
-            if not v or [1] is None:
-                if not fn.read_attribute(a): #USE read not check!!
-                    result['down'].append(a)
-                else:
-                    result['novals' if not v else 'nones'].append(a)
-            elif v[0] < (t0 - 7200):
-                result['lost'].append(a)
-        
-        print('\t%d attributes have no values'%len(result['novals']))
-        print('\t%d attributes are not readable'%len(result['down']))
-        print('\t%d attributes are not updated'%len(result['lost']))
-        print('\t%d attributes have None values'%len(result['nones']))
-        
-        return result
-    
-    
-    
-    
-    
+        ##if cls is None:
+            ##self._attached = False
+            ###self.trace("Failed to attach: Model class not found")
+        ##elif self.modelName == '':
+            ##self._attached = False
+            ##self.modelObj = None
+        ##else:
+            ##try:
+                ##self.modelObj = taurus.Manager().getObject(cls, self.modelName)
+                ##if self.modelObj is not None:
+                    ##self.modelObj.addListener(self)
+                    ##self._attached = True
+                    ##self.changeLogName(self.log_name + "." + self.modelName)
+            ##except Exception:
+                ##self.modelObj = None
+                ##self._attached = False
+                ##self.debug(
+                    ##"Exception occured while trying to attach '%s'" % self.modelName)
+                ##self.traceback()
+
+        #self.postAttach()
+        #return self._attached        
+
+    ##-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
+    ## QT property definition
+    ##-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
+
+    ##: This property holds the unique URI string representing the model name
+    ##: with which this widget will get its data from. The convention used for
+    ##: the string can be found :ref:`here <model-concept>`.
+    ##:
+    ##: In case the property :attr:`useParentModel` is set to True, the model
+    ##: text must start with a '/' followed by the attribute name.
+    ##:
+    ##: **Access functions:**
+    ##:
+    ##:     * :meth:`TaurusBaseWidget.getModel`
+    ##:     * :meth:`TaurusBaseWidget.setModel`
+    ##:     * :meth:`TaurusBaseWidget.resetModel`
+    ##:
+    ##: .. seealso:: :ref:`model-concept`
+    #model = Qt.pyqtProperty("QString", TaurusBaseWidget.getModel,
+                            #TaurusBaseWidget.setModel, TaurusBaseWidget.resetModel)
+
+
+#def main_TaurusTreePanel(host):
+    #w = _TaurusTreePanel()
+    #w.setWindowIcon(getElementTypeIcon(TaurusElementType.Device))
+    #w.setWindowTitle("A Taurus Tree Example")
+    #w.setModel(host)
+    #w.show()
+    #return w
+
+
+#def main_TaurusDbTreeWidget(host, perspective=TaurusElementType.Device):
+    #w = TaurusDbTreeWidget(perspective=perspective)
+    #w.setWindowIcon(getElementTypeIcon(perspective))
+    #w.setWindowTitle("A Taurus Tree Example")
+    #w.setModel(host)
+    #w.show()
+    #return w
+
+
+#def demo():
+    #"""DB panels"""
+    #import taurus
+    #db = TaurusArchivingDatabase() #taurus.Authority()
+    #host = db.getNormalName()
+    ##w = main_TaurusTreePanel(host)
+    ## w = main_TaurusDbTreeWidget(host, TaurusElementType.Device)
+
+    #w = _TaurusTreePanel()
+    #w.setWindowIcon(getElementTypeIcon(TaurusElementType.Device))
+    #w.setWindowTitle("A Taurus Tree Example")
+    #w.setModel(host,db)
+    #w.show()
+
+    #return w
+
+
+#def main1():
+    #import sys
+    #import taurus.qt.qtgui.application
+    #Application = taurus.qt.qtgui.application.TaurusApplication
+
+    #app = Application.instance()
+    #owns_app = app is None
+
+    #if owns_app:
+        #app = Application(app_name="DB model demo", app_version="1.0",
+                          #org_domain="Taurus", org_name="Tango community")
+    #w = demo()
+    #w.show()
+
+    #if owns_app:
+        #sys.exit(app.exec_())
+    #else:
+        #return w
+    
+#def main2(args = []):
+    #if len(sys.argv) > 1:
+        #host = sys.argv[1]
+    #else:
+        #host = None
+
+    #app = Qt.QApplication(args)
+    #tm = TaurusModelChooser()
+    ##.modelChooserDlg() #host=host)
+    #ta = TaurusArchivingDatabase()
+    #ta.get_archived_devices_list()
+    #print(dlg)
+    #sys.exit()
+    
+def main3():
+    asMimeData = True
+    app = Qt.QApplication([])
+    dlg = Qt.QDialog()
+    dlg.setWindowTitle('Archiving Tree')
+    dlg.setWindowIcon(Qt.QIcon("logos:taurus.png"))
+    layout = Qt.QVBoxLayout()
+    w = TaurusModelChooser(
+        parent=dlg) #, selectables=selectables, host=host, singleModel=singleModel)
+    layout.addWidget(w)
+    dlg.setLayout(layout)
+    w.updateModels.connect(dlg.accept)
+    dlg.exec_()
+    return w.getListedModels(asMimeData=asMimeData), (dlg.result() == dlg.Accepted)    
+
+if __name__ == "__main__":
+    print(main3())
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/hdbpp/decimate.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/decimate.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,63 +2,93 @@
 
 import PyTangoArchiving as pta, sys, time, re, fandango as fn
 import PyTangoArchiving.utils as ptau
 
 args = sys.argv[1:]
 tt0 = time.time()
 
+raise Exception('Deprecated, use maintenance.py instead')
+
 __doc__ = """
 Usage:
 
 This script should allow to decimate several HDB++ dbs/tables in parallel
 A db_repair call may be needed at the end of the process.
 
     PyTangoArchiving/hdbpp/decimate.py action db_name args 
 
 actions/args are:
 
     check db_name : 
         list bigger files in /var/lib/mysql/db_name (may need permissions)
         
     check db_name tstart tend table
-        print number of rows per attribute in the given table
+        print(number of rows per attribute in the given table)
 
     decimate db_name tstart tend [data_types / attributes] :
         will decimate data on the given table/attributes in the specified interval
 """
 
 def check_db(db_name):        
     data = fn.shell_command("du -sh /var/lib/mysql/%s/*"%db_name)
     lines = [l.strip().split() for l in data.split('\n')]
     print(lines[0])
     gs = sorted((eval(l[0].replace('G','')),'G',l[1]) for l in lines if l and 'G' in l[0])
     for g in gs:
         print(g)        
 
 def check_table(db_name,table,tstart,tend):
-    print('check_table(%s,%s,%s,%s)'% (db_name,table,tstart,tend))
+    print('check_table(%s,%s,%s,%s)' % (db_name,table,tstart,tend))
     api = pta.api(db_name)
-    tstart,tend = fn.time2str(tstart),fn.time2str(tend)
+    tstart,tend = fn.time2str(tstart),fn.time2str(tend-1)
     rows = dict()
     for a in api:
         api.get_attr_id_type_table(a)
         if api[a].table == table:
             r = api.Query("select count(*) from %s where att_conf_id = %s and "
                 "data_time between '%s' and '%s'" % (table,api[a].id,tstart,tend))
             #if r[0][0] > 1e3:
             #print(a,r)
             rows[a] = r[0][0]
             
     print('%d attributes found'  % len(rows))
     for n,k in sorted((s,a) for a,s in rows.items()):
         print('%s id=%s rows=%s' % (k, api[k].id, n))
+        
+def delete_tdb_table_data(table, date):
+    tdb = pta.api('tdb')
+    tdb.db.setLogLevel('debug')
+    if table in tdb:
+        table = tdb[table].table
+    try:
+        v = tdb.db.Query('select time from %s order by time limit 1' % table)
+        print('first value at %s' % str(v))
+    except:
+        tdb.db.Query('repair table '+table)
+        v = tdb.db.Query('select time from %s order by time limit 1' % table)
+        print('first value at %s' % str(v))        
+    try:
+        tdb.db.Query("delete from %s where time < '%s'" % (table, date))
+        tdb.db.Query('optimize table '+table)
+        tdb.db.Query('repair table '+table)
+        v = tdb.db.Query('select time from %s order by time limit 1' % table)        
+        print(v)
+        return True
+    except:
+        print(fn.except2str())
+        print(table,'failed')
+        return False
+        
             
 def decimate(db_name,keys,tstart,tend,period=10,dry=False):
     """
     time arguments are strings
+    BUT!, this method seems to not work anymore to free space in TDB
+    Maybe a mysqld restart is needed, I don't know; 
+    but up to now space is not freed
     """
     api = pta.api(db_name)
     
     if '/' in keys[0]:
         print('Decimating by attribute names')
         tables = fn.defaultdict(list)
         for a in keys:
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/hdbpp/multi.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/hdbpp/multi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 import sys,os,re,traceback
 
 import fandango as fn
 import fandango.db as fdb
 import fandango.tango as ft
 from fandango.functional import *
+from fandango import Cached
 
 import PyTangoArchiving
 import PyTangoArchiving as pta
 ##############################################################################    
 
    
-def get_archivers_filters(archiver='archiving/es/*'):
-    filters = fn.SortedDict(sorted((k,v['AttributeFilters']) for k,v in 
-                    fn.tango.get_matching_device_properties(
-                    archiver,'AttributeFilters').items()))
-    return filters
-
 def get_schema_attributes(schema='*'):
     rd = pta.Reader(schema)
     alls = rd.get_attributes(active=True)
     return alls
 
 def is_attribute_code_pushed(device,attribute,\
         event=ft.EventType.ARCHIVE_EVENT):
@@ -40,62 +35,89 @@
             return True
         # Pushed by Polling
         return False
     except:
         # No events available
         return None
         
-
-def get_hdbpp_databases(archivers=[],dbs={}):
+@fn.Cached(expire=300,depth=2)
+def get_hdbpp_databases(active=True): #archivers=[],dbs={}):
     """
     Method to obtain list of dbs/archivers; it allows to match any 
     archiver list against existing dbs.
     
     This method can be used in cached mode executed like:
     
         dbs = get_hdbpp_databases()
         for a in archivers:
-            db = get_hdbpp_databases(a,dbs).keys()[0]
+            db = fn.first(get_hdbpp_databases(a,dbs).keys())
       
     """
-    if not dbs:
-        dbs = {}
-        print('Loading databases from Tango')
-        cms = ft.get_class_devices('HdbConfigurationManager')
-        for c in cms:
-            props = ['LibConfiguration','ArchiverList']
-            props = ft.get_database().get_device_property(c,props)
-            db = dict(t.split('=') for t in props['LibConfiguration'])['dbname']
-            dbs[db] = {c:None}
-            for a in props['ArchiverList']:
-                dbs[db][a] =  ft.get_device_property(a,'AttributeList')
+    schemas = pta.Schemas.load()
+    hdbpp = sorted(k for k in schemas if fn.clsearch('hdbpp',str(schemas[k])))
+    dbactive = ft.get_free_property('PyTangoArchiving','DbActive')
+    if active:
+        r = []
+        for h in hdbpp:
+            try:
+                if h in dbactive or fn.check_device(pta.api(h).manager):
+                    r.append(h)
+            except:
+                pass
+        return r
     else:
-        dbs = dbs.copy()
-            
-    if archivers:
-        archivers = list(archivers) #Don't use toList here!
-        targets = []
-        for a in archivers:
-            m = fn.parse_tango_model(a,fqdn=True)
-            targets.extend((m.fullname, m.devicename, m.devicemodel))
-            
-        print(targets)
+        return hdbpp
 
-        for db,archs in dbs.items():
-            narchs = {}
-            for a in archs.keys():
-                if fn.inCl(a,targets):
-                    m = fn.parse_tango_model(a,fqdn=True).fullname
-                    narchs[m] = archs[a]
-            if not narchs:
-                dbs.pop(db)
-            else:
-                dbs[db] = narchs
-            
-    return dbs
+def get_host_last_partitions(host, user, passwd, 
+        exclude_db='information_schema|tdb*'):
+    import fandango.db as fdb
+    db = fdb.FriendlyDB(host=host,db_name='information_schema',
+                        user=user, passwd=passwd)
+    result = {}
+    for d in db.Query('show databases'):
+        if fn.clmatch(exclude_db,d[0]):
+            continue
+        q = ("select partition_name from partitions where "
+            "table_schema = '%s' and partition_name is not NULL "
+            "and data_length > %d order by partition_name DESC limit 1;" % 
+            (d[0], MIN_FILE_SIZE))
+        r = db.Query(q)
+        result[d[0]] = r
+    return result
+
+def get_host_first_partitions(host, user, passwd, 
+        exclude_db='information_schema|tdb*'):
+    import fandango.db as fdb
+    db = fdb.FriendlyDB(host=host,db_name='information_schema',
+                        user=user, passwd=passwd)
+    result = {}
+    for d in db.Query('show databases'):
+        if fn.clmatch(exclude_db,d[0]):
+            continue
+        q = ("select partition_name from partitions where "
+            "table_schema = '%s' and partition_name is not NULL "
+            "and data_length > %d order by partition_name limit 1;" % 
+            (d[0], MIN_FILE_SIZE))
+        r = db.Query(q)
+        result[d[0]] = r
+    return result
+    
+def get_hdbpp_filters():
+    dbs = get_hdbpp_databases(active=True)
+    sch = pta.Schemas.load()
+    return dict((d,sch[d].get('filters','*')) for d in dbs)
+
+def get_hdbpp_for_attributes(attrlist):
+    filters = get_hdbpp_filters()
+    r = fn.defaultdict(list)
+    for a in attrlist:
+        for d,f in filters.items():
+            if fn.clmatch(f,a,extend=True):
+                r[d].append(a)
+    return r
 
 def merge_csv_attrs(exported = True, currents = True, check_dups = True):
     """
     OJU! Correctors are not exported but should be archived anyway!
     """
     folder = fn.tango.get_free_property('PyTangoArchiving','CSVFolder')
     csvs = [f for f in fn.listdir(folder) if f.endswith('csv')]
@@ -104,15 +126,15 @@
 
     alldevs = fn.tango.get_all_devices(exported = exported)
     
     sources = dict()
     for f in csvs:
         try:
             sources[f] = pta.ParseCSV(folder+f)
-        except Exception,e:
+        except Exception as e:
             print('%s failed: %s\n'%(f,e))
     
     wrongs = []
     for f,data in sources.items():
         a,m,p = '','',''
         for a in data:
             try:
@@ -135,15 +157,15 @@
                                 print('%s duplicated: %s and %s' %(a,archattrs[a]['file'],f))
                             prev = archattrs[a][m][0]
                             
                         if not prev or p < prev:
                             archattrs[a]['file'] = f
                             archattrs[a][m] = mode
                             
-            except Exception,e:
+            except Exception as e:
                 print(f,a,m,e)
                 
     if currents:
         hdb,tdb = pta.api('hdb'),pta.api('tdb')
         for api in ('hdb','tdb'):
             api = pta.api(api)
             m = api.schema.upper()
@@ -171,55 +193,115 @@
             try:
                 v = reader.configs[s].get_attribute_values(a,start,stop)
             except:
                 v = None
             result.append((a,s,v and len(v)))
     return result
 
-def get_archivers_for_attributes(attrs=[],archs='archiving/es/*'):
+## DEPRECATED
+#def get_managers_filters(archiver=''):
+    ##filters = fn.SortedDict(sorted((k,v['AttributeFilters']) for k,v in 
+                    ##fn.tango.get_matching_device_properties(
+                    ##archiver,'AttributeFilters').items()))
+    #managers = fn.tango.get_class_devices('HdbConfigurationManager')
+    #filters = [fn.tango.get_device_property(m,'AttributeFilters')
+                   #for m in managers]
+    #filters = zip(managers,map(fn.toList,filters))
+    #return filters
+
+## DEPRECATED
+#@Cached(expire=60.)
+#def get_database_for_attributes(attrs):
+    #result = dict()
+    #filters = get_managers_filters()
+    #for a in attrs:
+        #for m,f in filters.items():
+            #pass
+
+def get_archivers_filters(archivers=''):
+    """
+    Returns the value of AttributeFilters property for each archiver in the list
+
+    :param archivers: sequence or regular expression  for matching archivers
+    :return: dictionary {archiver:regexp}
+    """
+    archs = archs if fn.isSequence(archivers) else fn.find_devices(archivers)
+    filters = fn.SortedDict(sorted((k,v['AttributeFilters']) for k,v in
+                    fn.tango.get_matching_device_properties(
+                    archiver,'AttributeFilters').items()))
+    return filters
+            
+
+def get_archivers_for_attributes(attrs=[],archs='archiving/*/es*'):
     """
     This method returns matching archivers for a list of attributes
     in simplename format (no tango host).
     
     It applies AttributeFilters as defined in Tango DB (sorted)
     """
-    if isString(attrs):
-        attrs = ft.find_attributes(attrs)
-    else:
-        attrs = attrs or get_schema_attributes('*')
-    
-    devattrs = fn.dicts.defaultdict(set)
-    [devattrs[a.rsplit('/',1)[0]].add(a) for a in attrs];    
-
-    if isSequence(archs): archs = '(%s)'%')|('.join(archs)
-    filters = get_archivers_filters(archs)
-    r = devattrs.keys()
-    archattrs = {}
-    
-    for i,k in enumerate(filters):
-        v = filters[k]
-        k = fn.tango.parse_tango_model(k, fqdn = True).fullname
-        if 'DEFAULT' in v:
-            df = k
+    archs = {}
+    hdbpp = pta.hdbpp.get_hdbpp_databases()
+    if len(hdbpp) == 1:
+        api = pta.api(hdbpp[0])
+        return dict((a,api.get_next_archiver()) for a in attrs)
+    for a in attrs:
+        d = a.lower().split('/')[-3]
+        if d == 'vc':
+            archs[a] = pta.api('hdbvc').get_next_archiver()
+        elif d == 'di':
+            archs[a] = pta.api('hdbdi').get_next_archiver()
+        elif d == 'rf':
+            archs[a] = pta.api('hdbrf').get_next_archiver()
+        elif d in ('pc','ma'):
+            archs[a] = pta.api('hdbpc').get_next_archiver()
+        elif d in ('ct','eps','pss'):
+            archs[a] = pta.api('hdbct').get_next_archiver()
         else:
-            m = fn.filtersmart(r,v)
-            currattrs = set(fn.join(*[devattrs[d] for d in m]))
-            if len(currattrs):
-                print(k,len(currattrs),sorted(set(i.split('/')[-2] for i in m)))
-                archattrs[k] = currattrs
-                print('\n')
-            r = [a for a in r if a not in m]
+            archs[a] = pta.api('hdbacc').get_next_archiver()
+            
+    return archs
+            
+        
+    
+    
+    #if isString(attrs):
+        #attrs = ft.find_attributes(attrs)
+    #else:
+        #attrs = attrs or get_schema_attributes('*')
+    
+    #devattrs = fn.dicts.defaultdict(set)
+    #[devattrs[a.rsplit('/',1)[0]].add(a) for a in attrs];    
+
+    #if isSequence(archs): archs = '(%s)'%')|('.join(archs)
+    #filters = get_archivers_filters(archs)
+    #r = devattrs.keys()
+    #archattrs = {}
+    
+    #for i,k in enumerate(filters):
+        #v = filters[k] # k is the archiver name
+        #k = fn.tango.parse_tango_model(k, fqdn = True).fullname
+        #if 'DEFAULT' in v:
+            #df = k
+        #else:
+            ##filtersmart(list,regexp): returns a clsearch on the list
+            #m = fn.filtersmart(r,v)
+            #currattrs = set(fn.join(*[devattrs[d] for d in m]))
+            #if len(currattrs):
+                #print(k,len(currattrs),sorted(set(i.split('/')[-2] for i in m)))
+                #archattrs[k] = currattrs
+                #print('\n')
+            #r = [a for a in r if a not in m]
             
-        if i == len(filters)-1:
-            k = df
-            m = r
-            currattrs = fn.join(*[devattrs[d] for d in m])
-            if len(currattrs):
-                print(k,len(currattrs),sorted(set(i.split('/')[-2] for i in m)))
-                archattrs[k] = currattrs
+        #if i == len(filters)-1:
+            #k = df
+            #m = r
+            #currattrs = fn.join(*[devattrs[d] for d in m])
+            #if len(currattrs):
+                #print(k,len(currattrs),sorted(set(i.split('/')[-2] for i in m)))
+                #archattrs[k] = currattrs
             
     return archattrs
 
 match_attributes_and_archivers = get_archivers_for_attributes
         
 ############################################################################## 
 
@@ -262,38 +344,33 @@
 
     result['polling'] = int(polling)        
     return result
 
 def start_archiving_for_attributes(attrs,*args,**kwargs):
     """
     from start_archiving(self,attribute,archiver,period=0,
-                      rel_event=None,per_event=300000,abs_event=None,
+                      rel_event=None,per_event=0,abs_event=None,
                       code_event=False, ttl=None, start=False):
 
     See HDBpp.add_attribute.__doc__ for a full description of arguments
     """    
-    archs = get_archivers_for_attributes(attrs)
-    dbs = get_hdbpp_databases(archs.keys())
+    #archs = get_archivers_for_attributes(attrs)
+    #dbs = get_hdbpp_databases(archs.keys())
     done = []
     
     if not args and not kwargs:
         kwargs['code_event'] = True
     
-    for db,devs in dbs.items():
+    dbs = get_hdbpp_for_attributes(attrs)
+    
+    for db,attrlist in dbs.items():
+        print('Launching %d attributes in %s'%(len(attrlist),db))
         api = PyTangoArchiving.Schemas.getApi(db)
-        devs = [d for d in devs if d in archs]
-        for d in devs:
-            ts = archs[d]
-            print('Launching %d attributes in %s.%s'%(len(ts),db,d))
-            for t in ts:
-                api.start_archiving(t,d,*args,**kwargs)            
-                done.append(fn.tango.get_full_name(t))
-
-            if not kwargs.get('start'):
-                fn.get_device(d).Start()
+        api.add_attributes(attrlist,*args,**kwargs)
+        done.extend(map(fn.tango.get_full_name,attrlist))
 
     if len(done)!=len(attrs):
         print('No hdbpp database match for: %s' % str(
             [a for a in attrs if fn.tango.get_full_name(a) not in done]))
 
     return done
 
@@ -366,15 +443,15 @@
         [devs[a.rsplit('/',1)[0]].append(a) for a in attrs]
         
         for d,v in devs.items():
             classes[fn.tango.get_device_class(d)][d] = v
             
         attrs = {}
         for c,devs in classes.items():
-            cfg = get_class_archiving(devs.keys()[0])
+            cfg = fn.first(get_class_archiving(devs.keys()))
             for d in devs:
                 raw = devs[d]
                 for a,v in cfg.items():
                     for aa in raw:
                         if fn.clmatch(a,aa.split('/')[-1],terminate=True):
                             if not attr_regexp or fn.clmatch(attr_regexp,aa):
                                 attrs[aa] = v
@@ -441,14 +518,7 @@
     allattrs = rd.get_archived_attributes(active=True)
     
     hdb,tdb = pta.api('hdb'),pta.api('tdb')
     
     for a in hdb,tdb:
         pass
 
-
-__all__ = [
-    'get_archivers_for_attributes',
-    'get_archivers_filters', 'get_hdbpp_databases',
-    'get_class_archiving', 
-    'is_attribute_code_pushed', 'check_attribute_in_all_dbs',
-    ]
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/servers/PyExtractor/PyExtractor.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/servers/PyExtractor/PyExtractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,16 @@
       
     @staticmethod
     def bool2float(argin):
         return float(not fn.isFalse(argin))
     
     @staticmethod
     def tag2attr(argin):
-        if any(argin.endswith(s) for s in ('_r','_t','_w','_d','_l','_ld')): 
+        if any(argin.endswith(s) for s in 
+               ('_r','_t','_w','_d','_l','_ld','_rg')): 
             argin = argin.rsplit('_',1)[0]
         if '/' not in argin: argin = argin.replace('__','/')
         return argin
     
     @staticmethod
     def attr2tag(argin):
         if '/' in argin: argin = argin.replace('/','__')
@@ -94,35 +95,35 @@
 
     def read_dyn_attr(self,attr):
         
         try:
             #attr.set_value(1.0)
             aname,values = attr.get_name(),[]
             attribute = self.tag2attr(aname)
-            print time.ctime()+'In read_dyn_attr(%s)'%aname
+            print(time.ctime()+'In read_dyn_attr(%s)'%aname)
             print(self.counter)
 
             try:
                 req,atformat,attype,data = self.AttrData[attribute]
-            except Exception,e:
+            except Exception as e:
                 print('Unable to read %s: key = %s ; cache = %s' % (attr,attribute,self.AttrData.keys()))
                 traceback.print_exc()
                 raise e
 
             conv = self.bool2float if attype is PyTango.DevBoolean \
             else (float if attype is PyTango.DevDouble
                 else str)
             
             if aname.endswith('_r'):
                 if atformat is PyTango.SpectrumAttr:
                     values = [conv(v[1] or 0.) for v in data]
                 else:
                     values = [map(conv,v[1]) for v in data]
-                if values: print time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'%(aname,type(values[0]),len(values),values[0],values[-1])
-                else: print '\tno values'
+                if values: print(time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'%(aname,type(values[0]),len(values),values[0],values[-1]))
+                else: print('\tno values')
                 attr.set_value(values,len(values))
                 
             elif aname.endswith('_l'):
                 print('%s: %s' % (aname,data))
                 if data[-1:]:
                     value = conv(data[-1][1])
                     date =  float(data[-1][0] or 0.)
@@ -137,57 +138,69 @@
                 attr.set_value_date_quality((value or 0.),date,q)
                 
             elif aname.endswith('_w'): 
                 if atformat is PyTango.SpectrumAttr:
                     values = [conv(v[2] or 0.) for v in data]
                 else:
                     values = [map(conv,v[2]) for v in data]
-                if values: print time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'%(aname,type(values[0]),len(values),values[0],values[-1])
-                else: print '\tno values'
+                if values: print(time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'%(aname,type(values[0]),len(values),values[0],values[-1]))
+                else: print('\tno values')
                 attr.set_value(values,len(values))
                 
             elif aname.endswith('_t'): 
                 values = [float(v[0] or 0.) for v in data]
-                if values: print time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'%(aname,type(values[0]),len(values),values[0],values[-1])
-                else: print '\tno values'
+                if values: print(time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'%(aname,type(values[0]),len(values),values[0],values[-1]))
+                else: print('\tno values')
                 attr.set_value(values,len(values))
                 
             elif aname.endswith('_d'): 
                 values = [fn.time2str(float(v[0] or 0.)) for v in data]
-                if values: print time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'%(aname,type(values[0]),len(values),values[0],values[-1])
-                else: print '\tno values'
+                if values: 
+                    print(time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'
+                        %(aname,type(values[0]),len(values),
+                          values[0],values[-1]))
+                else: 
+                    print('\tno values')
                 attr.set_value(values,len(values))            
                 
             elif aname.endswith('_ld'): 
                 lv = [fn.time2str(float(v[0] or 0.)) for v in data[-1:]]
                 if lv: 
                     print(time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'
                             %(aname,type(lv[0]),len(lv),lv[0],lv[-1]))
-                else: print '\tno values'
+                else: print('\tno values')
                 attr.set_value(lv[-1])
                 
+            elif aname.endswith('_rg'): 
+                lv = [fn.time2str(float(v[0] or 0.)) for v in data]
+                if lv: 
+                    print(time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'
+                            %(aname,type(lv[0]),len(lv),lv[0],lv[-1]))
+                else: print('\tno values')
+                attr.set_value('%s - %s' % (lv[0],lv[-1]))
+                
             else:
                 if atformat == PyTango.SpectrumAttr:
                     if attype == PyTango.DevString:
                         values = [(fn.time2str(d[0]),str(d[1])) for d in data]
                     else:
                         values = [(d[0],conv(d[1])) for d in data]
                 else:
                     if attype is PyTango.DevString:
                         values = [[fn.time2str(d[0])]+map(str,d[1]) for d in data]
                     else:
                         values = [[d[0]]+map(conv,d[1]) for d in data]
                 
                 if values: 
-                    print time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'%(aname,type(values[0]),len(values),values[0],values[-1])
+                    print(time.ctime()+'In read_dyn_attr(%s): %s[%d]:%s...%s'%(aname,type(values[0]),len(values),values[0],values[-1]))
                 else: 
-                    print '\tno values'
+                    print('\tno values')
                 attr.set_value(values,len(values))
                 
-            print '\treturned %d values'%len(values)
+            print('\treturned %d values'%len(values))
             
         except Exception as e:
             traceback.print_exc()
             raise e
         
     def is_dyn_attr_allowed(self,attr,req_type=None):
         return True #self.IsDataReady(attr.name)
@@ -241,14 +254,18 @@
                                self.read_dyn_attr,None,self.is_dyn_attr_allowed)   
             
             #LAST DATE
             self.add_attribute(
                 PyTango.Attr(aname+'_ld',PyTango.DevString,PyTango.AttrWriteType.READ),
                                self.read_dyn_attr,None,self.is_dyn_attr_allowed)              
             
+            self.add_attribute(
+                PyTango.Attr(aname+'_rg',PyTango.DevString,PyTango.AttrWriteType.READ),
+                               self.read_dyn_attr,None,self.is_dyn_attr_allowed)                 
+            
             #Then add the data to Cache values, so IsDataReady will return True
             t = fn.now()
             self.RemoveCachedAttribute(attribute)
             self.AttrData[attribute] = (t,atformat,attype,values)
             print('Done: %s,%s,%s,%s,%d'%(attribute,t,atformat,attype,len(values)))
         except:
             print(traceback.format_exc())
@@ -261,26 +278,26 @@
         self.AttrData,self.reader = fandango.CaselessDict(),None #Created here to be init() proof
         PyExtractor.init_device(self)
 
 #------------------------------------------------------------------
 #    Device destructor
 #------------------------------------------------------------------
     def delete_device(self):
-        print time.ctime()+"[Device delete_device method] for device",self.get_name()
+        print(time.ctime()+"[Device delete_device method] for device",self.get_name())
         self.reader.stop()
         #del self.reader
-        print 'Waiting 10 seconds'
+        print('Waiting 10 seconds')
         time.sleep(10.)
-        print 'Finished'
+        print('Finished')
 
 #------------------------------------------------------------------
 #    Device initialization
 #------------------------------------------------------------------
     def init_device(self):
-        print time.ctime()+"In ", self.get_name(), "::init_device()"
+        print(time.ctime()+"In ", self.get_name(), "::init_device()")
         self.counter = 0
         self.set_state(PyTango.DevState.ON)
         self.get_device_properties(self.get_device_class())
         if not self.reader: 
             self.reader = PyTangoArchiving.reader.ReaderProcess(self.DbSchema)
         if self.AttrData: self.RemoveCachedAttributes()
 
@@ -304,15 +321,15 @@
 #    PyExtractor read/write attribute methods
 #
 #==================================================================
 #------------------------------------------------------------------
 #    Read Attribute Hardware
 #------------------------------------------------------------------
     def read_attr_hardware(self,data):
-        #print time.ctime()+"In ", self.get_name(), "::read_attr_hardware()"
+        #print(time.ctime()+"In ", self.get_name(), "::read_attr_hardware()")
         pass
 
 
 
 
 #==================================================================
 #
@@ -326,15 +343,15 @@
         Arguments to be AttrName, StartDate, StopDate, Synchronous
         
         If Synchronous is missing or False, data is buffered into attributes, which names are returned
         If True or Yes, all the data is returned when ready
         
         Data returned will be (rows,[t0,v0,t1,v1,t2,v2,...])
         """
-        print time.ctime()+"In ", self.get_name(), "::GetAttDataBetweenDates(%s)"%argin
+        print(time.ctime()+"In ", self.get_name(), "::GetAttDataBetweenDates(%s)"%argin)
         #    Add your own code here
         size = 0
         aname = argin[0]
         tag = self.attr2tag(aname)
         dates = self.dates2times(argin[1:3])
         RW = False
         synch = fn.searchCl('yes|true',str(argin[3:4]))
@@ -345,15 +362,15 @@
             decimate=True, cache=self.UseApiCache)
         self.counter+=1
         print(self.counter)
         
         argout = [fn.shape(attrs),[a for a in attrs]]
         
         if not synch:
-          print '\t%s'%argout
+          print('\t%s'%argout)
           return argout
       
         else:
           while not self.IsDataReady(aname):
             fandango.wait(0.1)
           data = self.AttrData[aname][-1]
           for t,v in data:
@@ -362,63 +379,63 @@
           return [fn.shape(data),argout]
         
     def GetCachedAttribute(self,argin):
         n,a = self.get_name(),self.attr2tag(argin)
         return [n+'/'+a+s for s in ('','_r','_t')] 
 
     def RemoveCachedAttribute(self, argin):
-        print time.ctime()+"In ", self.get_name(), "::RemoveCachedAttribute(%s)"%argin
+        print(time.ctime()+"In ", self.get_name(), "::RemoveCachedAttribute(%s)"%argin)
         #    Add your own code here
         argin = self.tag2attr(argin)
         if argin in self.AttrData:
             data = self.AttrData.pop(argin)
             del data
         else:
             print('\tAttribute %s not in AttrData!!!!'%argin)
         if False:
             #All this part disabled as it doesn't work well in PyTango 7.2.2
             try:
                 attrlist = self.get_device_attr().get_attribute_list()
                 attrlist = [a.get_name().lower() for a in attrlist]
-                print 'Attributelist: %s'%[str(a) for a in attrlist]
+                print('Attributelist: %s'%[str(a) for a in attrlist])
             except:
-                print traceback.format_exc()
+                print(traceback.format_exc())
             aname = argin.replace('/','__').lower()
             for s in ('','_r','_t',''):#,'_w'):
                 try:
                     if aname in attrlist:
                         self.remove_attribute(aname+s)
                     else:
                         print('%s attribute does not exist!'%aname)
-                except Exception,e: 
+                except Exception as e: 
                     print('\tremove_attribute(%s): %s'%(aname+s,e))
         return
 
     def RemoveCachedAttributes(self):
-        print "In ", self.get_name(), "::RemoveCachedAttributes()"
+        print("In ", self.get_name(), "::RemoveCachedAttributes()")
         #    Add your own code here
         remove = [a for a,v in self.AttrData.items() if v[0]<fn.now()-self.ExpireTime]
-        for a in self.AttrData.keys()[:]:
+        for a in list(self.AttrData.keys()):
             self.RemoveCachedAttribute(a)
 
     def IsArchived(self, argin):
-        print "In ", self.get_name(), "::IsArchived()"
+        print("In ", self.get_name(), "::IsArchived()")
         #    Add your own code here
         return self.reader.is_attribute_archived(argin)
 
     def IsDataReady(self, argin):
-        print "In ", self.get_name(), "::IsDataReady(%s)"%argin
+        print("In ", self.get_name(), "::IsDataReady(%s)"%argin)
         #    Add your own code here
         aname = self.tag2attr(argin)
         argout = aname in self.AttrData
-        print '\tIsDataReady(%s == %s): %s'%(argin,aname,argout)
+        print('\tIsDataReady(%s == %s): %s'%(argin,aname,argout))
         return argout
 
     def GetCurrentArchivedAtt(self):
-        print "In ", self.get_name(), "::GetCurrentArchivedAtt()"
+        print("In ", self.get_name(), "::GetCurrentArchivedAtt()")
         #    Add your own code here
         return self.reader.get_attributes(active=True)
       
     @Cached(depth=30,expire=10.)      
     def GetCurrentQueries(self):
         print("In "+self.get_name()+"::GetCurrentQueries()")
         
@@ -550,27 +567,32 @@
 
 #------------------------------------------------------------------
 #    PyExtractorClass Constructor
 #------------------------------------------------------------------
     def __init__(self, name):
         PyTango.DeviceClass.__init__(self, name)
         self.set_type(name);
-        print "In PyExtractorClass  constructor"
+        print("In PyExtractorClass  constructor")
 
 #==================================================================
 #
 #    PyExtractor class main method
 #
 #==================================================================
-if __name__ == '__main__':
+
+def main(args = []):
     try:
-        py = PyTango.Util(sys.argv)
+        args = args or sys.argv
+        py = PyTango.Util(args)
         py.add_TgClass(PyExtractorClass,PyExtractor,'PyExtractor')
 
         U = PyTango.Util.instance()
         U.server_init()
         U.server_run()
 
-    except PyTango.DevFailed,e:
-        print '-------> Received a DevFailed exception:',e
-    except Exception,e:
-        print '-------> An unforeseen exception occured....',e
+    except PyTango.DevFailed as e:
+        print('-------> Received a DevFailed exception:',e)
+    except Exception as e:
+        print('-------> An unforeseen exception occured....',e)
+    
+if __name__ == '__main__':
+    main()
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/widget/ui/TaurusAttributeChooser.ui` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/ui/TaurusAttributeChooser.ui`

 * *Files identical despite different names*

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/widget/ArchivingBrowser.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/ArchivingBrowser.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,44 @@
 ##
 #############################################################################
 
 __doc__ = """ABBA, Archiving Best Browser for Alba"""
 
 import re,sys,os,time,traceback,threading
 import PyTango
-import fandango
-import fandango.functional as fun
+import fandango as fn
 from fandango.log import tracer
 
+#############################################################################
+
 import taurus
-from fandango.qt import Qt,Qwt5
-from taurus.qt.qtgui.plot import TaurusTrend,TaurusPlot
+
+QT_API=os.getenv('QT_API')
+USE_PYQTGRAPH=os.getenv('USE_PYQTGRAPH')
+USE_QWT=str(QT_API).lower() in ('pyqt','pyqt4') and not USE_PYQTGRAPH
+if USE_QWT:
+    print('Loading taurus pyqwt')
+    try:
+        from fandango.qt import Qwt5
+        from taurus.qt.qtgui.qwt5 import TaurusTrend,TaurusPlot
+    except:
+        USE_QWT=False
+
+if not USE_QWT:
+    print('Loading taurus pyqtgraph')
+    #from taurus.qt.qtgui.plot import TaurusTrend,TaurusPlot
+    from taurus.qt.qtgui.tpg import TaurusTrend,TaurusPlot
+    
+DEBUG=bool(os.getenv('DEBUG'))
+    
+print('QT_API: %s' % QT_API)
+print('USE_PYQTGRAPH: %s' % USE_PYQTGRAPH)
+print('TaurusTrend: %s' % TaurusTrend)
+print('TaurusPlot: %s' % TaurusPlot)
+    
 from taurus.qt.qtgui.panel import TaurusDevicePanel
 from taurus.qt.qtgui.panel import TaurusValue
 from taurus.qt.qtcore.util.emitter import SingletonWorker
 
 try:
     # taurus 4
     from taurus.core.tango.util import tangoFormatter
@@ -46,60 +69,64 @@
 except:
     try:
         # Tau / Taurus < 3.4
         from taurus.qt.qtgui.display import TaurusValueLabel as TaurusLabel
     except:
         # Taurus > 3.4
         from taurus.qt.qtgui.display import TaurusLabel
+        
+#############################################################################
+
+from fandango.qt import Qt,getColorsForValue
+from fandango.qt import QGridTable, QDictToolBar
 
 try:
     from PyTangoArchiving.widget.tree import TaurusModelChooser
 except:
     traceback.print_exc()
     TaurusModelChooser = None
+    
+#############################################################################    
 
 def get_distinct_domains(l):
     return sorted(set(str(s).upper().split('/')[0] for s in l))
 
 def launch(script,args=[]):
     import os
     f = '%s %s &'%(script,' '.join(args))
-    print 'launch(%s)'%f
+    print('launch(%s)'%f)
     os.system(f)
-
-from fandango.qt import QGridTable, QDictToolBar
-
-###############################################################################
+    
 ###############################################################################
 
 class MyScrollArea(Qt.QScrollArea):
     def setChildrenPanel(self,child):
         self._childrenPanel = child
     def childrenPanel(self):
         return getattr(self,'_childrenPanel',None)
     def resizeEvent(self,event):
         Qt.QScrollArea.resizeEvent(self,event)
         if self.childrenPanel():
             w,h = self.width()-15,self.childrenPanel().height()
-            #print 'AttributesPanel.ScrollArea.resize(%s,%s)'%(w,h)
+            #print('AttributesPanel.ScrollArea.resize(%s,%s)'%(w,h))
             self.childrenPanel().resize(w,h)
 
 PARENT_KLASS = QGridTable #Qt.QFrame #Qt.QWidget
 class AttributesPanel(PARENT_KLASS):
     
     _domains = ['ALL EPS']+['LI','LT']+['LT%02d'%i for i in range(1,3)]+['SR%02d'%i for i in range(1,17)]
-    _fes = [f for f in get_distinct_domains(fandango.get_database().get_device_exported('fe*')) if fun.matchCl('fe[0-9]',f)]
+    _fes = [f for f in get_distinct_domains(fn.get_database().get_device_exported('fe*')) if fn.matchCl('fe[0-9]',f)]
     
     LABELS = 'Label/Value Device Attribute Alias Archiving Check'.split()
     SIZES = [500, 150, 90, 90, 120, 40]
     STRETCH = [8, 4, 4, 4, 2, 1]
     
     def __init__(self,parent=None,devices=None):
-        #print '~'*80
-        tracer('In AttributesPanel()')
+        #print('~'*80)
+        if DEBUG: tracer('In AttributesPanel()')
         PARENT_KLASS.__init__(self,parent)
         self.setSizePolicy(Qt.QSizePolicy(Qt.QSizePolicy.Ignored,Qt.QSizePolicy.Ignored))
         self.worker = SingletonWorker(parent=self,cursor=True,sleep=50.,start=True)
         #self.worker.log.setLogLevel(self.worker.log.Debug)
         self.filters=('','','') #server/device/attribute
         self.devices=devices or []
         self.setValues(None)
@@ -129,21 +156,19 @@
             #'Test Device': self.popMenu.addAction(Qt.QIcon(),"Test Device",self.onTestDevice)
             }
         #if hasattr(self,'setFrameStyle'):
             #self.setFrameStyle(self.Box)
         try:
             import PyTangoArchiving
             self.reader = PyTangoArchiving.Reader('*')
-            #self.hreader = self.reader.configs['hdb']
-            #self.treader = self.reader.configs.get('tdb',self.hreader)
         except:
             traceback.print_exc()
             
     def __del__(self):
-        print 'AttributesPanel.__del__'
+        print('AttributesPanel.__del__')
         QGridTable.__del__(self)
         
     def setItem(self,x,y,item,spanx=1,spany=1,align=None,model=None):
         align = align or Qt.Qt.AlignLeft
         try:
             if model:
                 item._model = model
@@ -200,14 +225,15 @@
           model = model or self.getCurrentModel()
           self.trend.addModels([model])
         except:
           Qt.QMessageBox.warning(self,"ups!",traceback.format_exc())        
           
     def addSelectedToTrend(self):
         try:
+            if DEBUG: tracer()
             y = self.columnCount()-1
             models = []
             for x in range(self.rowCount()):
                 item = self.itemAt(x,y).widget()
                 m = getattr(item,'_model','')
                 if m and item.isChecked():
                     models.append(m)
@@ -232,54 +258,66 @@
     def setValues(self,values,filters=None):
         """ filters will be a tuple containing several regular expressions to match """
         #print('In AttributesPanel.setValues([%s])'%len(values or []))
         if values is None:
            self.generateTable([])
         elif True: #filters is None:
             self.generateTable(values)
-        #print 'In AttributesPanel.setValues(...): done'
+        #print('In AttributesPanel.setValues(...): done')
         return
             
     def generateTable(self,values):
-        
+        if DEBUG: tracer()
         #thermocouples = thermocouples if thermocouples is not None else self.thermocouples
         self.setRowCount(len(values))
         self.setColumnCount(5)
         #self.vheaders = []
         self.offset = 0
         self.widgetbuffer = []
         
         for i,tc in enumerate(sorted(values)):
-            #print 'setTableRow(%s,%s)'%(i,tc)
-            model,device,attribute,alias,archived,ok = tc
-            model,device,attribute,alias = map(str.upper,(model,device,attribute,alias))
+            #print('setTableRow(%s,%s)'%(i,tc))
+            model,device,attribute,alias,archived,label = tc
+            model,device,attribute,alias = map(str.lower,(model,device,attribute,alias))
             #self.vheaders.append(model)
+
             def ITEM(m,model='',size=0):
-                q = fandango.qt.Draggable(Qt.QLabel)(m)
+                q = fn.qt.Draggable(Qt.QLabel)(m)
                 if size is not 0:
                     q.setMinimumWidth(size) #(.7*950/5.)
-                q._model = model
+                q._model = model or m
                 q._archived = archived
                 q.setDragEventCallback(lambda s=q:s._model)
                 return q
+            
             ###################################################################
             qf = Qt.QFrame()
             qf.setLayout(Qt.QGridLayout())
             qf.setMinimumWidth(self.SIZES[0])
             qf.setSizePolicy(Qt.QSizePolicy.Expanding,Qt.QSizePolicy.Fixed)
             #Order changed, it is not clear if it has to be done before or after adding TaurusValue selfect
             self.setCellWidget(i+self.offset,0,qf) 
             
             #print('Adding item: %s, %s, %s, %s, %s' % (model,device,attribute,alias,archived))
-            if ok:
+            ok = fn.check_attribute(model,brief=False,timeout=500)# is not None
+            print(ok)
+            ok = ok if not isinstance(ok,Exception) else None 
+            if False:
                 tv = TaurusValue() #TaurusValueLabel()
                 qf.layout().addWidget(tv,0,0)
                 tv.setParent(qf)
+            elif ok:
+                import PyTangoArchiving.widget.panel as ptawp
+                tv = ptawp.TaurusSingleValue()
+                tv.setModel(model)
+                self.setItem(i+self.offset,0,tv)
             else:
-                self.setItem(i+self.offset,0,ITEM(model,model))
+                label = str(label)+'(-)' if label else ''
+                tv = ITEM(label+'(-)',model)
+                self.setItem(i+self.offset,0,tv)
                 
             devlabel = ITEM(device,model,self.SIZES[1])
             self.setItem(i+self.offset,1,devlabel)
             self.setItem(i+self.offset,2,ITEM(attribute,model,self.SIZES[2]))
             self.setItem(i+self.offset,3,ITEM(alias,model,self.SIZES[3]))
 
             from PyTangoArchiving.widget.panel import showArchivingModes,show_history
@@ -291,60 +329,64 @@
             q = Qt.QPushButton(txt)
             q.setFixedWidth(self.SIZES[-2])
             q.setToolTip("""%s<br><br><pre>
               'HDB' : Archived and updated, push to export values
               'hdb' : Archiving stopped, push to export values
               '...' : Not archived
               </pre>"""%txt)
-            self.connect(q, Qt.SIGNAL("pressed ()"), 
-                lambda a=self.reader.get_attribute_alias(model),o=q: 
-                 setattr(q,'w',show_history(a))) #showArchivingModes(a,parent=self)))
+            cb = (lambda a=self.reader.get_attribute_alias(model),o=q: 
+                 setattr(q,'w',show_history(a))) #showArchivingModes(a,parent=self)))) 
+            try:
+                self.connect(q, Qt.SIGNAL("pressed ()"), cb) 
+            except:
+                self.q.pressed.connect(cb)
+                
             self.setItem(i+self.offset,4,q)
             
             qc = Qt.QCheckBox()
             qc.setFixedWidth(self.SIZES[-1])
             self.setItem(i+self.offset,5,qc,1,1,Qt.Qt.AlignCenter,model)
 
-            if ok:
+            if isinstance(tv,TaurusValue): #ok:
                 #print('Setting Model %s'%model)
                 #ADDING WIDGETS IN BACKGROUND DIDN'T WORKED, I JUST CAN SET MODELS FROM THE WORKER
                 try:
                     if self.worker:
                         self.worker.put([(lambda w=tv,m=model:w.setModel(m))])
-                        #print 'worker,put,%s'%str(model)
+                        #print('worker,put,%s'%str(model))
                     else:
                         tv.setModel(model)
                 except: 
-                    print traceback.format_exc()
+                    print(traceback.format_exc())
                 self.models.append(tv)
                 
             #self.widgetbuffer.extend([qf,self.itemAt(i+self.offset,1),self.itemAt(i+self.offset,2),self.itemAt(i+self.offset,3),self.itemAt(i+self.offset,4)])
-            fandango.threads.Event().wait(.02)
+            fn.threads.Event().wait(.02)
             
         if len(values):
             def setup(o=self):
                 [o.setRowHeight(i,20) for i in range(o.rowCount())]
                 #o.setColumnWidth(0,350)
                 o.update()
                 o.repaint()
-                #print o.rowCount()
+                #print(o.rowCount())
                 o.show()
                 
             setup(self)
             
         if self.worker:
-            print( '%s.next()' % (self.worker) )
-            self.worker.next()
+            print( '%s.__next__()' % (self.worker) )
+            self.worker.__next__()
             
         #threading.Event().wait(10.)
         tracer('Out of generateTable()')
             
     def clear(self):
         try:
-            #print('In AttributesPanel.clear()')
+            if DEBUG: tracer('In AttributesPanel.clear()')
             for m in self.models: 
                 m.setModel(None)
             self.models = []
             self.setValues(None)
             #QGridTable.clear(self)
             def deleteItems(layout):
                 if layout is not None:
@@ -368,15 +410,15 @@
     MAX_ATTRIBUTES = 1500
     
     LABELS = AttributesPanel.LABELS
     SIZES = AttributesPanel.SIZES
     STRETCH = AttributesPanel.STRETCH
     
     def __init__(self,parent=None,domains=None,regexp='*pnv-*',USE_SCROLL=True,USE_TREND=False):
-        print('%s: ArchivingBrowser()' % fun.time2str())
+        if DEBUG: tracer(obj='ArchivingBrowser',msg='init()')
         Qt.QWidget.__init__(self,parent)
         self.setupUi(USE_SCROLL=USE_SCROLL, USE_TREND=USE_TREND, SHOW_OPTIONS=False)
         self.load_all_devices()
         try:
             import PyTangoArchiving
             self.reader = PyTangoArchiving.Reader('*') 
             self.archattrs = sorted(set(self.reader.get_attributes()))
@@ -384,90 +426,109 @@
         except:
             traceback.print_exc()
             
         self.extras = []
         #self.domains = domains if domains else ['MAX','ANY','LI/LT','BO/BT']+['SR%02d'%i for i in range(1,17)]+['FE%02d'%i for i in (1,2,4,9,11,13,22,24,29,34)]
         #self.combo.addItems((['Choose...']+self.domains) if len(self.domains)>1 else self.domains)
         self.connectSignals()
-        print('%s: ArchivingBrowser(): done' % fun.time2str())
+        if DEBUG: tracer(msg='ArchivingBrowser(): done')
         
     def load_all_devices(self,filters='*'):
-        import fandango
-        self.tango = fandango.get_database()
-        self.alias_devs = fandango.defaultdict_fromkey(
+        if DEBUG: tracer(obj=self)
+        import fandango as fn #needed by subprocess
+        self.tango = fn.get_database()
+        self.alias_devs = fn.defaultdict_fromkey(
                 lambda k,s=self: str(s.tango.get_device_alias(k)))
         self.archattrs = []
         self.archdevs = []
         #print('In load_all_devices(%s)...'%str(filters))
-        devs = fandango.tango.get_all_devices()
+        devs = fn.tango.get_all_devices()
         if filters!='*': 
-            devs = [d for d in devs if fandango.matchCl(
+            devs = [d for d in devs if fn.matchCl(
                         filters.replace(' ','*'),d,extend=True)]
         self.all_devices = devs
         self.all_domains = sorted(set(a.split('/')[0] for a in devs))
         self.all_families = sorted(set(a.split('/')[1] for a in devs))
 
         members = []
         for a in devs:
             try:
                 members.append(a.split('/')[2])
             except:
                 # Wrong names in DB? yes, they are
-                pass #print '%s is an invalid name!'%a
+                pass #print('%s is an invalid name!'%a)
         members = sorted(set(members))
         
         self.all_members = sorted(set(e for m in members 
                 for e in re.split('[-_0-9]',m) 
-                if not fandango.matchCl('^[0-9]+([ABCDE][0-9]+)?$',e)))
+                if not fn.matchCl('^[0-9]+([ABCDE][0-9]+)?$',e)))
 
-        #print 'Loading alias list ...'
+        #print('Loading alias list ...')
         self.all_alias = self.tango.get_device_alias_list('*')
         #self.alias_devs =  dict((str(self.tango.get_device_alias(a)).lower(),a) for a in self.all_alias)
-        tracer('Loading (%s) finished.'%(filters))
+        if DEBUG: tracer(obj=self,msg='Loading (%s) finished.'%(filters))
         
-    def load_attributes(self,servfilter,devfilter,attrfilter,warn=True,exclude = ('dserver','tango*admin','sys*database','tmp','archiving')):
-        tracer('In load_attributes(%s,%s,%s)'%(servfilter,devfilter,attrfilter))
+    def load_attributes(self,servfilter,devfilter,attrfilter,warn=True,
+        exclude = ('dserver','tango*admin','sys*database','tmp','archiving')):
         
-        servfilter,devfilter,attrfilter = servfilter.replace(' ','*').strip(),devfilter.replace(' ','*'),attrfilter.replace(' ','*')
-        attrfilter = attrfilter or 'state'
-        devfilter = devfilter or attrfilter
+        servfilter = servfilter.replace(' ','*').strip()
+        attrfilter = (attrfilter or 'state').replace(' ','*')
+        devfilter = (devfilter or attrfilter).replace(' ','*')
+
+        #Solve fqdn issues
+        devfilter = devfilter.replace('tango://','')
+        if ':' in devfilter:
+            tracer('ArchivingBrowser ignores tango host filters')
+            devfilter = fn.clsub(fn.tango.rehost,'',devfilter)
+            
+        if DEBUG: tracer(obj=self,msg=
+            'In load_attributes(%s,%s,%s)'%(servfilter,devfilter,attrfilter))            
+
         archive = self.dbcheck.isChecked()
         all_devs = self.all_devices if not archive else self.archdevs
-        all_devs = [d for d in all_devs if not any(d.startswith(e) for e in exclude) or any(d.startswith(e) and fun.matchCl(e,devfilter) for e in exclude)]
+        all_devs = [d for d in all_devs if not 
+                    any(d.startswith(e) for e in exclude) 
+                    or any(d.startswith(e) 
+                    and fn.matchCl(e,devfilter) for e in exclude)]
+
         if servfilter.strip('.*'):
-            sdevs = map(str.lower,fandango.Astor(servfilter).get_all_devices())
+            sdevs = map(str.lower,fn.Astor(servfilter).get_all_devices())
             all_devs = [d for d in all_devs if d in sdevs]
+            
         #print('In load_attributes(%s,%s,%s): Searching through %d %s names'
               #%(servfilter,devfilter,attrfilter,len(all_devs),
                 #'server' if servfilter else 'device'))
+                
         if devfilter.strip().strip('.*'):
-            devs = [d for d in all_devs if (fandango.searchCl(devfilter,d,extend=True))]
+            devs = [d for d in all_devs if 
+                    (fn.searchCl(devfilter,d,extend=True))]
             print('\tFound %d devs, Checking alias ...'%(len(devs)))
             alias,alias_devs = [],[]
             if '&' in devfilter:
                 alias = self.all_alias
             else:
                 for df in devfilter.split('|'):
                     alias.extend(self.tango.get_device_alias_list('*%s*'%df.strip()))
             if alias: 
                 print('\t%d alias found'%len(alias))
-                alias_devs.extend(self.alias_devs[a] for a in alias if fun.searchCl(devfilter,a,extend=True))
+                alias_devs.extend(self.alias_devs[a] for a in alias if fn.searchCl(devfilter,a,extend=True))
                 print('\t%d alias_devs found'%len(alias_devs))
                 #if not self.alias_devs:
                     #self.alias_devs =  dict((str(self.tango.get_device_alias(a)).lower(),a) for a in self.all_alias)
-                #devs.extend(d for d,a in self.alias_devs.items() if fandango.searchCl(devfilter,a) and (not servfilter or d in all_devs))
+                #devs.extend(d for d,a in self.alias_devs.items() if fn.searchCl(devfilter,a) and (not servfilter or d in all_devs))
                 devs.extend(d for d in alias_devs if not servfilter.strip('.*') or d in all_devs)
         else:
             devs = all_devs
             
         devs = sorted(set(devs))
         self.matching_devs = devs
-        print('In load_attributes(%s,%s,%s): %d devices found'%(servfilter,devfilter,attrfilter,len(devs)))
+        if DEBUG: tracer(obj=self,msg=
+            'In load_attributes(%s,%s,%s): %d devices found'%(servfilter,devfilter,attrfilter,len(devs)))
 
-        if False and not len(devs) and not archive:
+        if not len(devs) and not archive:
             #Devices do not actually exist, but may exist in archiving ...
             #Option disabled, was mostly useless
             self.dbcheck.setChecked(True)
             return self.load_attributes(servfilter,devfilter,attrfilter,warn=False)
         
         if len(devs)>self.MAX_DEVICES and warn:
             Qt.QMessageBox.warning(self, "Warning" , "Your search (%s,%s) matches too many devices!!! (%d); please refine your search\n\n%s\n..."%(devfilter,attrfilter,len(devs),'\n'.join(devs[:30])))
@@ -484,23 +545,23 @@
                 dp = taurus.Device(d)
                 if not archive:
                     dp.ping()
                     tcs = [t for t in dp.get_attribute_list()]
                 else:
                     tcs = [a.split('/')[-1] for a in self.archattrs if a.startswith(d+'/')]
 
-                matches = [t for t in tcs if fandango.searchCl(attrfilter,t,extend=True)]
+                matches = [t for t in tcs if fn.searchCl(attrfilter,t,extend=True)]
 
                 for t in sorted(tcs):
                     if not self.dbcheck.isChecked() or not matches: 
                         label = dp.get_attribute_config(t).label
                     else: 
                         label = t
                         
-                    if t in matches or fandango.searchCl(attrfilter,label,extend=True):
+                    if t in matches or fn.searchCl(attrfilter,label,extend=True):
                         if self.archivecheck.isChecked() \
                                 and not self.reader.is_attribute_archived(d+'/'+t):
                             continue
                         
                         if d in self.alias_devs: 
                             alias = self.alias_devs[d]
                         else:
@@ -522,55 +583,60 @@
                     self.matching_attributes[d+'/state'] = (d,d,'state',None) #A None label means device-not-readable
                     
         if warn and len(self.matching_attributes)>30:
             r = Qt.QMessageBox.warning(self, "Message" , "(%s) matches %d attributes."%(attrfilter,len(self.matching_attributes)),Qt.QMessageBox.Ok|Qt.QMessageBox.Cancel)
             if r==Qt.QMessageBox.Cancel:
                 return {}
         if not len(self.matching_attributes):
-            Qt.QMessageBox.warning(self, "Warning", "No matching attribute has been found in %s." % ('Archiving DB' if archive else 'Tango DB (try Archiving option)'))
+            Qt.QMessageBox.warning(self, "Warning", "No matching attribute has been found in %s." % ('Archiving DB' if archive else 'Tango DB (try DB Cache option)'))
+            
         if failed_devs:
             print('\t%d failed devs!!!: %s'%(len(failed_devs),failed_devs))
             if warn:
                 Qt.QMessageBox.warning(self, "Warning" , 
                     "%d devices were not running:\n"%len(failed_devs) +'\n'.join(failed_devs[:10]+(['...'] if len(failed_devs)>10 else []) ))
         
-        tracer('\t%d attributes found'%len(self.matching_attributes))
+        if DEBUG: tracer(obj=self,msg=
+            '\t%d attributes found'%len(self.matching_attributes))
         return self.matching_attributes
         
     def setupUi(self,USE_SCROLL=False, SHOW_OPTIONS=False, USE_TREND=False):
+        if DEBUG: tracer(obj=self)
         self.setWindowTitle('Tango Finder : Search Attributes and Archiving')
         self.setLayout(Qt.QVBoxLayout())
         self.setMinimumWidth(950)#550)
         #self.setMinimumHeight(700)
         
         self.layout().setAlignment(Qt.Qt.AlignTop)
         self.browser = Qt.QFrame()
         self.browser.setLayout(Qt.QVBoxLayout())
         
         self.chooser = Qt.QTabWidget()
-        self.chooser.setTabPosition(self.chooser.West if SHOW_OPTIONS else self.chooser.North)
+        self.chooser.setTabPosition(self.chooser.West 
+                    if SHOW_OPTIONS else self.chooser.North)
         #self.combo = Qt.QComboBox() # Combo used for domains, currently disabled
 
         self.searchbar = Qt.QFrame()
         self.searchbar.setLayout(Qt.QGridLayout()) 
 
         #self.label = Qt.QLabel('Type a part of device name and a part of attribute name, use "*" or " " as wildcards:')
         #self.layout().addWidget(self.label)
         
         self.ServerFilter = Qt.QLineEdit()
         self.ServerFilter.setMaximumWidth(250)
-        self.DeviceFilter = fandango.qt.Dropable(Qt.QLineEdit)()
-        self.DeviceFilter.setSupportedMimeTypes(fandango.qt.TAURUS_DEV_MIME_TYPE)
-        self.AttributeFilter = fandango.qt.Dropable(Qt.QLineEdit)()
-        self.AttributeFilter.setSupportedMimeTypes([fandango.qt.TAURUS_ATTR_MIME_TYPE,fandango.qt.TEXT_MIME_TYPE])
+        self.DeviceFilter = fn.qt.Dropable(Qt.QLineEdit)()
+        self.DeviceFilter.setSupportedMimeTypes(fn.qt.TAURUS_DEV_MIME_TYPE)
+        self.AttributeFilter = fn.qt.Dropable(Qt.QLineEdit)()
+        self.AttributeFilter.setSupportedMimeTypes(
+            [fn.qt.TAURUS_ATTR_MIME_TYPE,fn.qt.TEXT_MIME_TYPE])
         self.update = Qt.QPushButton('Update')
         self.archivecheck = Qt.QCheckBox("Only archived")
         self.archivecheck.setChecked(False)
         self.dbcheck = Qt.QCheckBox("DB cache")
-        self.dbcheck.setChecked(False)
+        self.dbcheck.setChecked(True)
 
         self.searchbar.layout().addWidget(Qt.QLabel(
             'Enter Device and Attribute filters using wildcards '
             '(e.g. li/ct/plc[0-9]+ / ^stat*$ & !status ) and push Update'),0,0,3,13)
         
         [self.searchbar.layout().addWidget(o,x,y,h,w) for o,x,y,h,w in (
             (Qt.QLabel("Device or Alias:"),4,0,1,1),(self.DeviceFilter,4,1,1,4),
@@ -582,15 +648,16 @@
         if SHOW_OPTIONS:
             self.options = Qt.QWidget() #self.searchbar
             self.options.setLayout(Qt.QGridLayout())
             separator = lambda x:Qt.QLabel(' '*x)
             row = 1
             [self.options.layout().addWidget(o,x,y,h,w) for o,x,y,h,w in (
                 #separator(120),Qt.QLabel("Options: "),separator(5),
-                (Qt.QLabel("Server: "),row,0,1,1),(self.ServerFilter,row,1,1,4),(Qt.QLabel(''),row,2,1,11)
+                (Qt.QLabel("Server: "),row,0,1,1),
+                (self.ServerFilter,row,1,1,4),(Qt.QLabel(''),row,2,1,11)
                 )]
             #self.panel = generate_table(load_all_thermocouples('SR14')[-1])
             self.optiontab = Qt.QTabWidget()
             self.optiontab.addTab(self.searchbar,'Filters')
             self.optiontab.addTab(self.options,'Options')
             self.optiontab.setMaximumHeight(100)
             self.optiontab.setTabPosition(self.optiontab.North)
@@ -599,15 +666,15 @@
         else: 
             self.browser.layout().addWidget(self.searchbar)
             
         self.toppan = Qt.QWidget(self)
         self.toppan.setLayout(Qt.QVBoxLayout())
 
         if USE_SCROLL:
-            print '*'*30 + ' USE_SCROLL=True '+'*'*30
+            print('*'*30 + ' USE_SCROLL=True '+'*'*30)
             ## TO USE SCROLL, HEADER HAS BEEN SET AS A SEPARATE WIDGET
             #self.header = QGridTable(self.toppan)
             #self.header.setHorizontalHeaderLabels(self.LABELS)
             #self.header.setColumnWidth(0,350)
             self.headers = []
             self.header = Qt.QWidget(self.toppan)
             self.header.setLayout(Qt.QHBoxLayout())
@@ -618,62 +685,87 @@
                     #ql.setFixedWidth(s)
                 #else:
                     #ql.setSizePolicy(Qt.QSizePolicy.MinimumExpanding,Qt.QSizePolicy.Fixed)
                 self.header.layout().addWidget(ql)
                 
             self.toppan.layout().addWidget(self.header)            
             
-            self._scroll = MyScrollArea(self.toppan)#Qt.QScrollArea(self)
-            self._background = AttributesPanel(self._scroll) #At least a panel should be kept (never deleted) in background to not crash the worker!
+            self._scroll = MyScrollArea(self.toppan)
+            #At least a panel should be kept (never deleted) in background to not crash the worker!
+            self._background = AttributesPanel(self._scroll) 
+            
             self.panel = None
             self._scroll.setChildrenPanel(self.panel)
             self._scroll.setWidget(self.panel)
             self._scroll.setMaximumHeight(700)
             self.toppan.layout().addWidget(self._scroll)
             self.attrpanel = self._background
         else:
             self.panel = AttributesPanel(self.toppan)
             self.toppan.layout().addWidget(self.panel)
             self.attrpanel = self.panel
             
-        self.toppan.layout().addWidget(Qt.QLabel('Drag any attribute from the first column into the trend or any taurus widget you want:'))
+        self.toppan.layout().addWidget(Qt.QLabel(
+            'If drag&drop fails, PLEASE USE RIGHT-CLICK ON THE NAME'
+            ' OF THE ATTRIBUTE OR CHECKBOX!!'))
         
         self.browser.layout().addWidget(self.toppan)
         self.chooser.addTab(self.browser,'Search ...')
         
         if USE_TREND:
             self.split = Qt.QSplitter(Qt.Qt.Vertical)
             self.split.setHandleWidth(25)
             self.split.addWidget(self.chooser)
             
-            from taurus.qt.qtgui.plot import TaurusTrend
-            from PyTangoArchiving.widget.trend import ArchivingTrend,ArchivingTrendWidget
-            self.trend = ArchivingTrendWidget() #TaurusArchivingTrend()
-            self.trend.setUseArchiving(True)
-            self.trend.showLegend(True)
+            if DEBUG: tracer(obj=self,msg='import trends')
+            if "qwt" in str(TaurusPlot.__bases__).lower():
+                from PyTangoArchiving.widget.trend import ArchivingTrend,ArchivingTrendWidget
+                self.trend = ArchivingTrendWidget() #TaurusArchivingTrend()
+                self.trend.setUseArchiving(True)
+                self.trend.showLegend(True)
+                
+            else: #PyQtGraph
+                try:
+                    from taurus_tangoarchiving.widget.tpgarchivingwidget import \
+                        ArchivingWidget
+                except:
+                    from PyTangoArchiving.widget.tpgarchivingwidget import \
+                        ArchivingWidget
+                
+                self.trend = ArchivingWidget()
+                
             self.attrpanel.trend = self.trend
+            if DEBUG: tracer(obj=self,msg='trends loaded')
 
             if TaurusModelChooser is not None:
+                tracer(obj=self,msg='Setting up Taurus Chooser ...')
                 self.treemodel = TaurusModelChooser(parent=self.chooser)
                 self.chooser.addTab(self.treemodel,'Tree')
-                self.treemodel.updateModels.connect(self.trend.addModels)
+                try:
+                    self.treemodel.updateModels.connect(self.trend.addModels)
+                except:
+                    traceback.print_exc()
                 #self.treemodel.connect(self.treemodel,Qt.SIGNAL('updateModels'),self.trend.addModels)      
             else:
                 tracer('TaurusModelChooser not available!')
             
             self.split.addWidget(self.trend)
             self.layout().addWidget(self.split)
         else:
             self.layout().addWidget(self.chooser)
         type(self)._persistent_ = self
+        if DEBUG: tracer(obj=self,msg='done')
         
     def connectSignals(self):
         #self.combo.connect(self.combo, Qt.SIGNAL("currentIndexChanged (const QString&)"), self.comboIndexChanged)
         #self.connect(self.combo, Qt.SIGNAL("currentIndexChanged (const QString&)"), self.comboIndexChanged)
-        self.connect(self.update, Qt.SIGNAL("pressed ()"), self.updateSearch)
+        try:
+            self.connect(self.update, Qt.SIGNAL("pressed ()"), self.updateSearch)
+        except:
+            self.update.pressed.connect(self.updateSearch)
         #if len(self.domains)==1: self.emit(Qt.SIGNAL("currentIndexChanged (const QString&)"),Qt.QString(self.domains[0]))
         
     def open_new_trend(self):
         from taurus.qt.qtgui.plot import TaurusTrend
         tt = TaurusTrend()
         tt.show()
         self.extras.append(tt)
@@ -710,21 +802,21 @@
             traceback.print_exc()
         
     def closeEvent(self,evt):
         Qt.QWidget.closeEvent(self,evt)
         type(self)._persistent_ = None
     
     #def __del__(self):
-        #print 'In ValvesChooser.del()'
+        #print('In ValvesChooser.del()')
         ##try: Qt.QWidget.__del__(self)
         ##except: pass
         #type(self)._persistent_ = None
         
     def comboIndexChanged(self,text=None):
-        #print 'In comboIndexChanged(...)'
+        #print('In comboIndexChanged(...)')
         pass
         
     def splitFilters(self,filters):
         if filters.count(',')>1: filters.replace(',',' ')
         if ',' in filters: filters = filters.split(',')
         elif ';' in filters: filters = filters.split(';')
         elif filters.count('/') in (1,3): filters = filters.rsplit('/',1)
@@ -735,15 +827,16 @@
     def setModel(self,model):
         model = str(model).strip()
         if model: self.updateSearch(model)
     
     def updateSearch(self,*filters):
         #Text argument applies only to device/attribute filter; not servers
         try:
-            #print('In updateSearch(%s[%d])'%(filters,len(filters)))
+            if DEBUG: tracer(obj=self,msg=
+                'In updateSearch(%s[%d])'%(filters,len(filters)))
             if len(filters)>2:
                 filters = [' '.join(filters[:-1]),filters[-1]]
             if len(filters)==1: 
                 filters = ['']+self.splitFilters(filters[0])
             elif len(filters)==2:
                 filters = ['']+list(filters)
             elif len(filters)==3:
@@ -774,34 +867,39 @@
             else:
                 old = self.panel
                 if self.panel:
                   if hasattr(self,'_scroll'): self._scroll.setWidget(None)
                   self.panel.setParent(None)
                   self.panel = None
                 if not self.panel: 
-                    self.panel = AttributesPanel(self._scroll,devices=self.all_devices)
+                    self.panel = AttributesPanel(
+                        self._scroll,devices=self.all_devices)
                     self.attrpanel = self.panel
                     if hasattr(self,'trend'): 
                         self.attrpanel.trend = self.trend
                 else: 
                     self.panel.clear()
                 if old: 
                   old.clear()
                   old.deleteLater() #Must be done after creating the new one!!
-                table = [] #model,device,attribute,alias,archived,ok
-                #ATTRIBUTES ARE FILTERED HERE!! <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
+                  
+                table = [] #model,device,attribute,alias,archived,label
+
+                #ATTRIBUTES ARE FILTERED HERE!! <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
                 for k,v in self.load_attributes(*filters).items():
+                    #load_attributes = (d,alias,t,label)
                     try: 
                         archived = self.reader.is_attribute_archived(k)
-                    except Exception,e: 
+                    except Exception as e: 
                         print('Archiving not available!:\n %s'
                               %traceback.format_exc())
                         archived = []
                     #print(k,v,archived)
-                    table.append((k,v[0],v[2],v[1],archived,v[3] is not None))
+                    #model,device,attribute,alias,archived,label
+                    table.append((k,v[0],v[2],v[1],archived,v[3]))
                     
                 self.panel.setValues(sorted(table))
                 
                 if hasattr(self,'_scroll'): 
                     self._scroll.setWidget(self.panel)
                     #self.panel.setParent(self._scroll) #IT DOESNT WORK
                     self._scroll.setChildrenPanel(self.panel)
@@ -821,35 +919,34 @@
                             #p = Qt.QSizePolicy(Qt.QSizePolicy.Expanding,Qt.QSizePolicy.Fixed)
                             #w.setSizePolicy(p)
                     #except:
                         #traceback.print_exc()
                         
             self.adjustColumns()
                     
-        except Exception,e:
+        except Exception as e:
             #traceback.print_exc()
             Qt.QMessageBox.warning(self, "Warning" , "There's something wrong in your search (%s), please simplify the string"%traceback.format_exc())
+        if DEBUG: tracer(obj=self,msg='done')
         return
                 
 ModelSearchWidget = ArchivingBrowser
 
 def main(args=None):
     """
     --range=YYYY/MM/DD_HH:mm,XXh
     """
     import sys
     
     opts = dict(a.split('=',1) for a in args if a.startswith('-'))
-    print(opts)
     args = [a for a in args if not a.startswith('-')]
-    print(args)    
     
     #from taurus.qt.qtgui.container import TaurusMainWindow
     tmw = Qt.QMainWindow() #TaurusMainWindow()
-    tmw.setWindowTitle('Tango Attribute Search (%s)'%(os.getenv('TANGO_HOST')))
+    tmw.setWindowTitle('Tango Attribute Search (%s)'%(fn.get_tango_host()))
     table = ArchivingBrowser(domains=args,USE_SCROLL=True,USE_TREND=True)
     tmw.setCentralWidget(table)
     
     use_toolbar = True
     if use_toolbar:
         toolbar = QDictToolBar(tmw)
         toolbar.set_toolbar([
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/widget/dialogs.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/dialogs.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,53 +30,66 @@
 import traceback
 import platform
 import PyTango
 import fandango as fn
 
 import PyTangoArchiving
 import PyTangoArchiving.utils as utils
-from PyTangoArchiving.reader import Reader,ReaderProcess
+from PyTangoArchiving.reader import Reader,ReaderProcess,DECIMATION_MODES
 
 ## WARNING: AVOID TO IMPORT TAURUS OR QT OUTSIDE ANY METHOD OR CLASS, BE GREEN!
 #from taurus.qt.qtgui.plot import TaurusTrend
 
 from history import show_history
 from fandango.objects import BoundDecorator, Cached
 from fandango.debug import Timed
 from fandango.dicts import defaultdict
-from fandango import SingletonMap,str2time, time2str
+from fandango import SingletonMap, str2time, time2str
 
 from fandango.qt import Qt,Qwt5,QTextBuffer,setDialogCloser,QWidgetWithLayout
 
-import taurus
-from taurus.qt.qtgui.plot import TaurusTrend
-from taurus.qt.qtgui.base import TaurusBaseWidget
-from taurus.qt.qtgui.container import TaurusWidget,TaurusGroupBox
+try:
+    import taurus
+    from taurus.qt.qtgui.plot import TaurusTrend
+    from taurus.qt.qtgui.base import TaurusBaseWidget
+    from taurus.qt.qtgui.container import TaurusWidget,TaurusGroupBox
+except:
+    taurus = fn.Object()
+    TaurusTrend = TaurusBaseWidget = TaurusWidget = TaurusGroupBox = taurus
 
 USE_MULTIPROCESS=False
 try:
     prop = PyTango.Database().get_class_property('HdbExtractor',
                                         ['Multiprocess'])['Multiprocess']
     if any(a in str(prop).lower() for a in ('true','1')):
         USE_MULTIPROCESS=True
     elif any(fn.matchCl(p,platform.node()) for p in prop):
         USE_MULTIPROCESS=True
 except:
-    print traceback.format_exc()
-print 'Multiprocess:%s'%USE_MULTIPROCESS
+    print(traceback.format_exc())
+print('Multiprocess:%s'%USE_MULTIPROCESS)
 
-DECIMATION_MODES = [
-    #('Hide Nones',fn.arrays.notnone),
-    ('Pick One',fn.arrays.pickfirst),
-    ('Minimize Noise',fn.arrays.mindiff),
-    ('Maximize Peaks',fn.arrays.maxdiff),
-    ('Average Values',fn.arrays.average),
-    ('In Client', False),
-    ('RAW',None),        
-    ]
+##############################################################################
+# Matplotlib code
+
+def plot_two_arrays(arr1,arr2,start=None,stop=None):
+    import matplotlib.pyplot as plt
+    plt.figure()
+    x0,x1 = min((arr1[0][0],arr2[0][0])),max((arr1[-1][0],arr2[-1][0]))
+    y0,y1 = min(t[1] for t in arr1+arr2),max(t[1] for t in arr1+arr2)
+    plt.subplot(131)
+    plt.plot([v[0] for v in arr1],[v[1] for v in arr1])
+    plt.axis([x0,x1,y0,y1])
+    plt.subplot(132)
+    plt.plot([v[0] for v in arr2],[v[1] for v in arr2])
+    plt.axis([x0,x1,y0,y1])
+    plt.show()
+    
+##############################################################################
+# TaurusTrend (Qwt) Code
 
 def getTrendObject(trend_set):
     return trend_set if hasattr(trend_set,'axisScaleDiv') else getObjectParent(trend_set)
 
 def getObjectParent(obj):
     return getattr(obj,'_parent',None) or obj.parent()
         
@@ -93,23 +106,28 @@
     
 def parseTrendModel(model):
     """ Attribute Name Parsing, Returns a tango_host,attribute,model tuple """
     modelobj = model
     if type(model) not in (str,):
         try: model = model.getFullName()
         except: 
-            try: model = model.getModelName()
-            except Exception,e:
-                print e+'\n'+'getArchivedTrendValues():model(%s).getModelName() failed\, using str(model)'%model
+            try: 
+                model = model.getModelName()
+            except Exception as e:
+                # minor error, depending on taurus version
+                #print('parseTrendModel(): model(%s).getModelName()'
+                      #' failed: \n\t%s'% (model, str(e)))
                 model = str(model)
     if '{' not in model: #Excluding "eval-like" models
         params = utils.parse_tango_model(model,fqdn=True)
-        tango_host,attribute = '%s:%s'%(params['host'],params['port']),'%s/%s'%(params['devicename'],params['attributename'])
+        tango_host,attribute = ('%s:%s'%(params['host'],params['port']),
+            '%s/%s'%(params['devicename'],params['attributename']))
     else:
-        tango_host,attribute='',modelobj.getSimpleName() if hasattr(modelobj,'getSimpleName') else model.split(';')[-1]
+        tango_host,attribute = '',(modelobj.getSimpleName() 
+            if hasattr(modelobj,'getSimpleName') else model.split(';')[-1])
 
     model = fn.tango.get_full_name(model,fqdn=True)
     return tango_host,attribute,model
 
 class MenuActionAppender(BoundDecorator):
     #self._showArchivingDialogAction = Qt.QAction("Show Archiving Dialog", None)
     #self.trend.connect(self._showArchivingDialogAction, Qt.SIGNAL("triggered()"), self.show_dialog)
@@ -219,41 +237,43 @@
         self._reloadbutton.connect(self._reloadbutton,Qt.SIGNAL('clicked()'),self.logger.resetBuffers)
         self._decimatecombo = Qt.QComboBox()
         self._decimatecombo.addItems([t[0] for t in DECIMATION_MODES])
         self._decimatecombo.setCurrentIndex(0)
         self._nonescheck = Qt.QCheckBox('Remove Nones')
         self._nonescheck.setChecked(True)
         self._nonescheck.connect(self._nonescheck,Qt.SIGNAL('toggled(bool)'),self.toggle_nones)
-        self._windowedit = Qt.QLineEdit()
-        self._windowedit.setText('0')
+        self._period = Qt.QLineEdit()
+        self._period.setText('AUTO')
 
         dl = Qt.QGridLayout()
         dl.addWidget(Qt.QLabel('Decimation method:'),0,0,1,2)
         dl.addWidget(self._decimatecombo,0,3,1,2)
         dl.addWidget(Qt.QLabel('Fixed Period (0=AUTO)'),1,0,1,1)
-        dl.addWidget(self._windowedit,1,1,1,1)
+        dl.addWidget(self._period,1,1,1,1)
         dl.addWidget(self._nonescheck,1,2,1,2)
         self.layout().addLayout(dl)
         
     def toggle_nones(self,checked=False):
         return True        
 
     def getDecimation(self):
         # The decimation method must be a function that takes a series of values and return a single value that summarizes the interval
         try:
             t = str(self._decimatecombo.currentText())
             m = dict(DECIMATION_MODES)[t]
+            if m is True:
+                m = str(self._period.text()).strip()
             self.logger.info('Decimation mode: %s,%s'%(m,t))
             return m
         except:
             self.logger.warning(traceback.format_exc())
             return None
         
     def getPeriod(self):
-        return float(self._windowedit.text())
+        return float(self._period.text())
         
     def getNonesCheck(self):
         return self._nonescheck.isChecked()
     
 class QReloadDialog(Qt.QDialog,QReloadWidget):
     
     def __init__(self, parent, logger, trend=None):
@@ -627,19 +647,27 @@
             1m : X minutes
             1h : X hours
             1d : X days
             1w : X weeks
             1y : X years
             """)
         self.xRangeCB.setCurrentIndex(1)
-        self.xApply = Qt.QPushButton("Refresh")
-        self.layout().addWidget(QWidgetWithLayout(self,child=[self.xLabelStart,self.xEditStart]))
-        self.layout().addWidget(QWidgetWithLayout(self,child=[self.xLabelRange,self.xRangeCB]))
-        self.layout().addWidget(QWidgetWithLayout(self,child=[self.xApply]))
-        trend.connect(self.xApply,Qt.SIGNAL("clicked()"),self.refreshAction)
+        self.xRefresh = Qt.QPushButton("Refresh")
+        self.layout().addWidget(QWidgetWithLayout(
+            self,child=[self.xLabelStart,self.xEditStart]))
+        self.layout().addWidget(QWidgetWithLayout(
+            self,child=[self.xLabelRange,self.xRangeCB]))
+        self.layout().addWidget(QWidgetWithLayout(
+            self,child=[self.xRefresh]))
+        trend.connect(self.xRefresh,Qt.SIGNAL("clicked()"),
+                      self.onRefreshButton)
+        self.xRangeCB.connect(self.xRangeCB, Qt.SIGNAL("currentIndexChanged(int)"),
+                    self.onRangeChanged)
+        self.xRangeCB.connect(self.xRangeCB, Qt.SIGNAL("editTextChanged"),
+                    self.onRangeChanged)
         
         if hasattr(self._trend,'getArchivedTrendLogger'):
             self.logger = self._trend.getArchivedTrendLogger()
             self.xInfo = Qt.QPushButton("Expert")        
             self.layout().addWidget(QWidgetWithLayout(self,child=[self.xInfo]))
             trend.connect(self.xInfo,Qt.SIGNAL("clicked()"),self.logger.show_dialog)
         
@@ -659,15 +687,54 @@
                 #ms = Qt.QMessageBox.warning(trend,"Error!",traceback.format_exc())
                 
         return
         
     def setTitle(self,title):
         self.setWindowTitle(title)
         
-    def refreshAction(self):
+    def getStartDate(self):
+        try:
+            t = str(self.xEditStart.text())
+            if t == self.DEFAULT_START:
+                return None
+            return str2time(t)
+        except:
+            traceback.print_exc()
+        
+    def getRange(self):
+        try:
+            return str2time(str(self.xRangeCB.currentText()))
+        except:
+            traceback.print_exc()
+    
+    def setStartDate(self, start):
+        if isinstance(start,(int,float)):
+            start = time2str(start)
+        self.xEditStart.setText(start)
+        
+    def setRange(self, end):
+        self.xRangeCB.setEditText(end)      
+        
+    def onRangeChanged(self):
+        t0, t1 = self.getStartDate(), self.getRange()
+        print('onRangeChanged(%s,%s)' % (t0,t1))
+        if t0 is None:
+            self.setStartDate(time.time()-abs(t1))
+        else:
+            t1 = t0 + abs(t1)
+            #If asked range goes into the future it is corrected
+            if t1 > time.time() + 600:
+                r, t1 = t1 - t0, time.time() + 600
+                t0 = t1 - r
+                self.setStartDate(t0)
+        print('\t\t(%s,%s)' % (t0,t1))
+        return t0, t1
+        
+    def onRefreshButton(self):
+        self.onRangeChanged()
         self._trend.applyNewDates()
         try:
             date = str2time(str(self.xEditStart.text()))
         except:
             try:
                 date = getTrendBounds(self._trend)[0]
                 self.xEditStart.setText(time2str(date))
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/widget/history.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/history.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,15 +84,15 @@
   def set_default_dates(klass,start,end):
     klass.DefaultStart = start
     klass.DefaultEnd = end
 
   @staticmethod
   def setup_table(attribute,start,stop,values):
   
-      print 'drawing table from %d values: %s ...' %( len(values),values[:2])
+      print('drawing table from %d values: %s ...' %( len(values),values[:2]))
       twi = Qt.QWidget()
       twi.setLayout(Qt.QVBoxLayout())
       tab = Qt.QTableWidget()
       tab.setWindowTitle('%s: %s to %s' % (attribute,start,stop))       
       twi.setWindowTitle('%s: %s to %s' % (attribute,start,stop))       
       tab.setRowCount(len(values))
       tab.setColumnCount(3)
@@ -119,17 +119,17 @@
 
   @classmethod
   def show_new_dialog(klass,attribute,schema='*',parent=None,dates=[]):
       try:
           if not Qt.QApplication.instance(): Qt.QApplication([])
       except:
           pass
-      print 'in Vacca.widgets.show_history(%s)'
+      print('in Vacca.widgets.show_history(%s)')
       
-      print 'getting archiving readers ...'
+      print('getting archiving readers ...')
       from PyTangoArchiving import Reader
       rd = Reader(schema.lower())
       hdb = Reader('hdb')
       tdb = Reader('tdb')
       attribute = str(attribute).lower()
       
       try:
@@ -138,15 +138,15 @@
           dates = map(epoch2str,dates)
       except:
           traceback.print_exc()
           dates = epoch2str(),epoch2str()
 
       schemas = rd.is_attribute_archived(attribute,preferent=False)
       if schemas:
-          print '%s is being archived' % attribute
+          print('%s is being archived' % attribute)
           di = Qt.QDialog(parent)
           wi = di #QtGui.QWidget(di)
           wi.setLayout(Qt.QGridLayout())
           begin = Qt.QLineEdit()
           begin.setText(dates[0])
           end = Qt.QLineEdit()
           end.setText(dates[1])
@@ -173,15 +173,15 @@
           wil.addWidget(vfilter,6,1,1,1)
           buttons = Qt.QDialogButtonBox(wi)
           buttons.addButton(Qt.QPushButton("Export"),Qt.QDialogButtonBox.AcceptRole)
 
           bt = Qt.QPushButton("Apply")
           buttons.addButton(bt,Qt.QDialogButtonBox.ApplyRole)
           def set_schema(r=rd,a=attribute,qs=qschema):
-              print 'setting schema ...'
+              print('setting schema ...')
               schema = str(qs.currentText()).strip()
               r.set_preferred_schema(a,schema)
               
           buttons.connect(bt,Qt.SIGNAL('clicked()'),set_schema)
 
           buttons.addButton(Qt.QPushButton("Close"),Qt.QDialogButtonBox.RejectRole)
 
@@ -189,40 +189,40 @@
           #    |Qt.QDialogButtonBox.Open|Qt.QDialogButtonBox.Close)
           wi.connect(buttons,Qt.SIGNAL('accepted()'),wi.accept)
           wi.connect(buttons,Qt.SIGNAL('rejected()'),wi.reject)
           wi.layout().addWidget(buttons,7,0,1,2)
           
           def check_values():
               di.exec_()
-              print 'checking schema ...'
+              print('checking schema ...')
               schema = str(qschema.currentText()).strip()
               if schema != '*':
                     rd.set_preferred_schema(attribute,schema)              
               if di.result():
-                  print 'checking result ...'
+                  print('checking result ...')
                   try:
                       start,stop = str(begin.text()),str(end.text())
                       try: tf = int(str(tfilter.text()))
                       except: tf = 0
                       vf = vfilter.isChecked()
                       if not all(re.match('[0-9]+-[0-9]+-[0-9]+ [0-9]+:[0-9]+:[0-9]+',str(s).strip()) for s in (start,stop)):
-                          print 'dates are wrong ...'
+                          print('dates are wrong ...')
                           Qt.QMessageBox.warning(None,'Show archiving', 'Dates seem not in %s format'%(tformat), Qt.QMessageBox.Ok)
                           return check_values()
                       else:
-                          print 'getting values ...'
-                          print 'using %s reader' % rd.schema
+                          print('getting values ...')
+                          print('using %s reader' % rd.schema)
                           values = rd.get_attribute_values(attribute,str2epoch(start),str2epoch(stop))
                           if not len(values) and schema=='*' and hdb.is_attribute_archived(attribute,active=True):
-                              print 'tdb failed, retrying with hdb'
+                              print('tdb failed, retrying with hdb')
                               values = hdb.get_attribute_values(attribute,str2epoch(start),str2epoch(stop))
                           if vf:
                               values = fandango.arrays.decimate_array(values)
                           if tf:
-                              print 'Filtering %d values (1/%dT)'%(len(values),tf)
+                              print('Filtering %d values (1/%dT)'%(len(values),tf))
                               values = fandango.arrays.filter_array(values,window=tf) #,begin=start,end=stop)
 
                           twi = klass.setup_table(attribute,start,stop,values)
                           klass.set_default_dates(str2epoch(start),str2epoch(stop))
                           
                           button = Qt.QPushButton('Save to file')
                           button2 = Qt.QPushButton('Send to email')
@@ -231,57 +231,57 @@
                               try:
                                   options = {'sep':'\\t','arrsep': '\\ ','linesep':'\\n'}
                                   import codecs
                                   dd = QOptionDialog(model=options,title='CSV Options')
                                   dd.exec_()
                                   for k,v in options.items():
                                     options[k] = codecs.escape_decode(str(v))[0]
-                                  print options
+                                  print(options)
                                 
                                   filename = Qt.QFileDialog.getSaveFileName(parent,
                                       'File to save',
                                       '/data/'+PyTangoArchiving.files.get_data_filename(var,data,'csv','human'),
                                       'CSV files (*.csv)')
                                   
                                   PyTangoArchiving.files.save_data_file(var,data,filename,format='csv',**options)
                                   if edit:
                                     try: os.system('gedit %s &'%filename)
                                     except: pass
                                   return filename
-                              except Exception,e:
+                              except Exception as e:
                                   Qt.QMessageBox.warning(None, "Warning" , "Unable to save %s\n:%s"%(filename,e))
                                   
                           def send_by_email(var=attribute,data=values,parent=twi):
                               #subject,text,receivers,sender='',attachments=None,trace=False):
                               try:
                                 receivers,ok = Qt.QInputDialog.getText(None,'Send by email','to:')
                                 if ok:
                                   filename = str(save_to_file(var,data,parent,edit=False))
                                   fandango.linos.sendmail(filename,attribute,receivers=str(receivers),attachments=[filename])
-                              except Exception,e:
+                              except Exception as e:
                                 Qt.QMessageBox.warning(None, "Warning" , "Unable to send %s\n:%s"%(filename,e))
                               
                           #button.setTextAlignment(Qt.Qt.AlignCenter)
                           twi.connect(button, Qt.SIGNAL("pressed ()"), save_to_file)
                           twi.layout().addWidget(button)
                           twi.connect(button2, Qt.SIGNAL("pressed ()"), send_by_email)
                           twi.layout().addWidget(button2)                        
                           twi.show()
 
                           TABS.append(twi)
                           twi.connect(twi,Qt.SIGNAL('close()'),lambda o=twi: TABS.remove(o))
-                          print 'show_history done ...'
+                          print('show_history done ...')
                           return twi
-                  except Exception,e:
-                      print traceback.format_exc()
+                  except Exception as e:
+                      print(traceback.format_exc())
                       Qt.QMessageBox.warning(None, "Warning" , "Unable to retrieve the values (%s), sorry"%e)
               else:
-                  print 'dialog closed'
+                  print('dialog closed')
                   return None
-          print 'asking for dates ...'
+          print('asking for dates ...')
           return check_values()
       else:
           Qt.QMessageBox.warning(None,'Show archiving', 'Attribute %s is not being archived'%attribute, Qt.QMessageBox.Ok)
           
 def show_history(*args,**kwargs):
   """ This method is a wrapper for HistoryDialog.show_new_dialog """
   print('%s: PyTangoArchiving.widget.history.show_history(...)'%time2str())
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/widget/models.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/models.py`

 * *Files identical despite different names*

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/widget/panel.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/panel.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,30 +23,31 @@
 ##
 #############################################################################
 
 ## author: srubio@cells.es, 2015
 
 import PyTango
 import re,sys,os,time,traceback,threading
-import fandango,fandango as F
+import fandango,fandango as fn
 import fandango.qt as fqt
 from fandango.qt import Qt
+from fandango.tango import AttrQuality
 import fandango.functional as fun
 from threading import Thread
 import PyTangoArchiving as pta
 from PyTangoArchiving.widget.history import show_history
 from PyTangoArchiving.common import modes_to_string
 
 def showTestDevice(device=None):
     import os
     os.system('tg_devtest %s&'%(device))
 
 def showDeviceInfo(device,parent=None):
     device = device or str(self.current_item._model.rsplit('/',1)[0])
-    info = F.tango.get_device_info(device).items()
+    info = fn.tango.get_device_info(device).items()
     Qt.QMessageBox.warning(parent, "%s Info"%device , '\n'.join('%s : %s'%i for i in info))
     
 def showArchivingModes(model,parent=None,schemas=('HDB','TDB')):
     print('onShowArchivingModes(%s)'%model)
     #DIALOG MUST BE ALWAYS SHOWN, EVEN FOR NON-ARCHIVED ATTRIBUTES!
     #w = Qt.QWidget() 
     w = Qt.QDialog()
@@ -59,14 +60,167 @@
      ws[s].setSchema(s)
      ws[s].setModel(model)
      w.layout().addWidget(ws[s])
     w.exec_()
     #w.show()
     return w
 
+class TaurusSingleValue(Qt.QWidget):
+    
+    def __init__(self,parent=None):
+        Qt.QWidget.__init__(self,parent)
+        self.setLayout(Qt.QHBoxLayout())
+        self.model = ''
+        self.device = ''
+        #self.label = Qt.QLabel()
+        self.label = fn.qt.Draggable(Qt.QLabel)()#(m)
+        self.label.setDragEventCallback(lambda s=self.label:s._model)
+        self.label.setFixedWidth(350)
+        self.value = Qt.QLabel()
+        self.value.setFixedWidth(150)
+        self.units = Qt.QLabel()
+        self.units.setFixedWidth(50)
+        self.setWindowTitle('TaurusSingleValue')
+        map(self.layout().addWidget,(self.label,self.value,self.units))
+        
+    def setColor(self,color):
+        #pLabel->setStyleSheet("QLabel { background-color : red; color : blue; }");
+        self.value.setStyleSheet("QLabel { background-color: %s; "
+                                 "qproperty-alignment: AlignRight; }" % str(color))
+        
+    def setModel(self, model):
+        try:
+            self.model = str(model).lower()
+            print('TaurusSingleValue.setModel(%s)' % self.model)
+            self.setWindowTitle(self.model)
+            self.rvalue = fn.tango.check_attribute(model)
+            if isinstance(self.value,Exception):
+                raise self.rvalue
+            mp = fn.tango.parse_tango_model(self.model)
+            self.device = mp.devicename
+            self.config = fn.tango.get_attribute_config(model)
+            self.label.setText(self.device+'/'+(
+                self.config.label or mp.attrname))
+            self.label.setToolTip(self.model)
+            self.label.setModel(self.model)
+            self.units.setText(str(self.config.unit).replace('No unit',''))
+            svalue = self.config.format or '%s'
+            value = getattr(self.rvalue,'value',self.rvalue)
+            quality = getattr(self.rvalue,'quality',AttrQuality.ATTR_INVALID)
+            try:
+                if self.model.lower().endswith('/state'):
+                    
+                    svalue = str(fn.tango.DevState.values[value])
+                    if svalue in ('CLOSE','ALARM','FAULT'):
+                        quality = AttrQuality.ATTR_WARNING
+                    elif svalue in ('INIT','UNKNOWN'):
+                        quality = AttrQuality.ATTR_INVALID
+                    else:
+                        quality = AttrQuality.ATTR_VALID
+                        
+                else:
+                    if fn.isSequence(value) or '%' not in svalue:
+                        svalue = str(value).strip()[:40]
+                    else:
+                        if isinstance(value,float) and value < 1e-2:
+                            svalue = '%e'
+                        svalue = (svalue % value).strip()[:40]
+                    
+            except Exception as e:
+                svalue = str(e)[:20]+'...'
+                
+            self.value.setText(svalue)
+            self.value.setToolTip(
+                str(value))
+            self.setColor({
+                AttrQuality.ATTR_VALID: 'lightgreen',
+                AttrQuality.ATTR_INVALID: 'lightgrey',
+                AttrQuality.ATTR_ALARM: 'red',
+                AttrQuality.ATTR_WARNING: 'orange',
+                AttrQuality.ATTR_CHANGING: 'lightblue',
+                }[quality])
+            print(self.model,svalue,quality)
+            
+        except Exception as e:
+            print(self.model,self.rvalue)
+            traceback.print_exc()
+            self.setColor('grey')
+            self.label.setText(str(model))
+            self.value.setText(str(e)[:25])
+            self.value.setToolTip(str(e))
+            self.units.setText('')
+            
+    def setLabelConfig(self,*args,**kwargs):
+        pass
+            
+class TaurusSingleValueForm(Qt.QScrollArea):
+    
+    def __init__(self,parent=None):
+        Qt.QScrollArea.__init__(self,parent)  
+        #Qt.QWidget.__init__(self,parent)
+        self.main = Qt.QWidget(self)
+        self.main.setLayout(Qt.QVBoxLayout())        
+        #self.setWidget(self.main)
+        self.resize(500,600)
+        self.setWindowTitle('TaurusSingleValue')
+        self.models = []
+        self.widgets = []
+        #self.show()
+
+        
+    def clear(self):
+        while len(self.widgets):
+            w = self.widgets.pop()
+            self.main.layout().removeWidget(w)
+        
+    def setModels(self, args):
+        self.clear()
+        try:
+            print('TaurusSingleValueForm.setModels(%s)' % str(args))
+            if fn.isString(args):
+                args = fn.find_attributes(args)        
+            if fn.isSequence(fn.first(args)):
+                args = list(args)[0]                
+            print('setModels(%s)' % args)
+            for m in sorted(args):
+                w = TaurusSingleValue()
+                w.setModel(m)
+                self.main.layout().addWidget(w)
+                self.widgets.append(w)
+            #self.main.show()
+            self.setWidget(self.main)
+            #self.resize(400,600)        
+            self.show()
+            print('TaurusSingleValueForm.setModels(%s)' % 'done')
+        except:
+            traceback.print_exc()
+        
+    setModel = setModels
+    
+    def getItems(self):
+        return self.widgets
+        
+    def setWithButtons(self, arg):
+        pass
+            
+    @staticmethod
+    def main(args):
+        import fandango.qt as fqt
+        #args = fn.toList(args)
+        app = fqt.getApplication()
+        dialog = Qt.QDialog()
+        form = TaurusSingleValueForm()
+        form.setModels(args)
+        dialog.setLayout(Qt.QVBoxLayout())
+        dialog.layout().addWidget(form)
+        #form.show()
+        dialog.show()
+        app.exec_()
+        
+
 class QArchivingMode(fqt.Dropable(Qt.QFrame)):
   __help__ = """
   <strong>Archiving Types</strong>&nbsp;
   <ul><li><strong>HDB (historic)</strong>: This mode of archiving will keep the information stored 
   forever, the archiving periodicity is limited to not faster than 10 seconds.</li>
   <li><strong>TDB (temporary)</strong>: The information is stored in round-buffer and will be kept 
   only for few days, this database will allow a periodicity not faster than 1 second.</li></ul>
@@ -212,15 +366,15 @@
           #print((i,j,modes[m][j]))
         else:
           t.setText('')
     if 'archiver' in modes:
       try:
         db = self.reader.get_database()
         attr_id = modes.get('ID')
-        date = db.get_table_updates(db.get_table_name(attr_id)).values()[0]
+        date = db.get_table_updates(fn.first(db.get_table_name(attr_id)).values())
         if date<time.time()-600: date = '<b>%s</b>' % fun.time2str(date)
         else: date = fun.time2str(date)
         dev = modes['archiver']
         self.archiver.setText('%s(%s,%s)'%(dev,attr_id,date))
         self.archiver.setContextCallbacks({
           'Test Device':fun.partial(showTestDevice,device=dev),
           'Show Info':fun.partial(showDeviceInfo,device=dev),
@@ -260,15 +414,15 @@
     return modes
   
   def applyModes(self):
     self.logger().show()
     #Qt.QApplication.instance().setOverrideCursor(Qt.QCursor(Qt.Qt.WaitCursor))
     try:
       attr = self.getModel()
-      v = F.check_attribute(attr,brief=True)
+      v = fn.check_attribute(attr,brief=True)
       if isinstance(v,(type(None),Exception)): 
         Qt.QMessageBox.warning(self,"Warning","%s is not readable nor archivable"%attr)
         self.logger().hide()
         return
       if fun.isSequence(v) or fun.isString(v):
         Qt.QMessageBox.warning(self,"Warning","%s array type is not supported"%attr)
         self.logger().hide()
@@ -338,15 +492,15 @@
     
   @staticmethod
   def _test(schema = None, model = None, multirow = None):
     print('_test',schema,model,multirow)
     if multirow is None:
       w = QArchivingMode()
     else:
-      w = QArchivingMode(multirow=F.str2bool(multirow))
+      w = QArchivingMode(multirow=fn.str2bool(multirow))
     if schema:
       w.setSchema(schema)
     if model:
       w.setModel(model)
     w.show()
     return w    
     
@@ -378,37 +532,40 @@
     if msg == self.last_msg: 
         msg = '+1'
     else: 
         self.last_msg = msg
         if self.logger:
             try:
                 if severity not in self.log_objs: self.log_objs[severity] = \
-                    getattr(self.logger,severity,(lambda m,s=severity:'%s:%s: %s'%(s.upper(),F.time2str(),m)))
+                    getattr(self.logger,severity,
+                    (lambda m,s=severity:'%s:%s: %s' % (
+                        s.upper(),fn.time2str(),m)))
                 self.log_objs[severity](msg)
             except: pass
     if self.dialog():
         if msg!='+1': 
-            msg = '%s:%s: %s'%(severity.upper(),F.time2str(),msg)
+            msg = '%s:%s: %s'%(severity.upper(),fn.time2str(),msg)
         if self.filters:
-            msg = (F.filtersmart(msg,self.filters) or [''])[0]
+            msg = (fn.filtersmart(msg,self.filters) or [''])[0]
         if msg:
             self.dialog().append(msg)
               
   def setLogLevel(self,level): self.loglevel = level
   def getLogLevel(self): return self.loglevel
   def trace(self,msg): self.log('trace',msg)
   def debug(self,msg): self.log('debug',msg)
   def info(self,msg): self.log('info',msg)
   def warning(self,msg): self.log('warning',msg)
   def alarm(self,msg): self.log('alarm',msg)
   def error(self,msg): self.log('error',msg)    
    
 if __name__ == '__main__':
   import sys
-  app = fqt.getApplication()
-  m = Qt.QWidget()
-  m.setLayout(Qt.QVBoxLayout())
-  w = QArchivingMode._test(*sys.argv[1:])
-  m.layout().addWidget(Qt.QLabel(str(sys.argv)))
-  m.layout().addWidget(w)
-  m.show()
-  app.exec_()
+  TaurusSingleValueForm.main(sys.argv[1:])
+  #app = fqt.getApplication()
+  #m = Qt.QWidget()
+  #m.setLayout(Qt.QVBoxLayout())
+  #w = QArchivingMode._test(*sys.argv[1:])
+  #m.layout().addWidget(Qt.QLabel(str(sys.argv)))
+  #m.layout().addWidget(w)
+  #m.show()
+  #app.exec_()
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/widget/resources.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/resources.py`

 * *Files identical despite different names*

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/widget/taurusattributechooser.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/taurusattributechooser.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         """Fill the devices list"""
 
         device= str(self.ui.lineEdit.text())
         
         try:
             items = list(self.getDb().get_device_exported(device))
 
-        except Exception,e:
+        except Exception as e:
             self.warning('Unable to contact with device %s: %s'%(device,str(e)))
             items=[]
 
         self.ui.devList.clear()
         self.ui.devList.addItems(items)
         #self.connect(self.ui.devList, Qt.SIGNAL("itemClicked ( QListWidgetItem * )"), self.setAttributes)
         self.connect(self.ui.devList, Qt.SIGNAL("itemSelectionChanged ()"), self.setAttributes)
@@ -132,15 +132,15 @@
 
         device= str(self.ui.lineEdit.text())
         device += '*'
         
         try:
             items = list(self.getDb().get_device_exported(device))
 
-        except Exception,e:
+        except Exception as e:
             self.warning('Unable to contact with device %s: %s'%(device,str(e)))
             items=[]
 
         self.ui.devList.clear()
         self.ui.devList.addItems(items)
         #self.connect(self.ui.devList, Qt.SIGNAL("itemClicked ( QListWidgetItem * )"), self.setAttributes)
         self.connect(self.ui.devList, Qt.SIGNAL("itemSelectionChanged ()"), self.setAttributes)
@@ -151,15 +151,15 @@
         
         self.ui.attrList.clear()
         self.dev_name = str(self.ui.devList.currentItem().text())
         
         try:
             items=[str(a.name) for a in PyTango.DeviceProxy(self.dev_name).attribute_list_query()]
             
-        except Exception,e:
+        except Exception as e:
             self.warning('Unable to contact with device %s: %s'%(self.dev_name,str(e)))
             items=[]
         
         items.sort(key=lambda x:x.lower()) #sort the attributes (case insensitive!)
         
         for i in range(len(items)):
             self.ui.attrList.addItem(items[i])
@@ -167,15 +167,15 @@
     def addButtonClicked(self):
         """Put all the items in the selectedItems list into the selectedItemsComplete list, with the device name"""
         
         if self.isSingleAttrMode():  #if we are in single attr mode, we want to replace instead of adding attributes
             self.selectedItemsComplete = CaselessList([])
             self.ui.final_List.clear()
             
-        #print self.ui.attrList.selectedItems()
+        #print(self.ui.attrList.selectedItems())
         self.selectedItems = self.ui.attrList.selectedItems()
         for i in range(len(self.selectedItems)):
             aux = str(self.dev_name) + "/" + str(self.selectedItems[i].text())
             if (aux not in self.selectedItemsComplete):
                 self.selectedItemsComplete.append(aux)
 
         self.updateList(self.selectedItemsComplete)
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/widget/tdbwidget.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/tdbwidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def setAttributes(self):
         """Fill the attributes list"""
         import PyTango
         self.ui.attrList.clear()
         self.dev_name = str(self.ui.devList.currentItem().text())
         try:
             items=[str(a.name) for a in PyTango.DeviceProxy(self.dev_name).attribute_list_query()]
-        except Exception,e:
+        except Exception as e:
             self.warning('Unable to contact with device %s: %s'%(self.dev_name,str(e)))
             items=[]
         items.sort(key=lambda x:x.lower()) #sort the attributes (case insensitive!)
         
         for i in range(len(items)): 
             fullname=str(self.dev_name+'/'+items[i]).lower()
             item=Qt.QListWidgetItem()
@@ -36,15 +36,15 @@
 
     def setNewDevName(self):
         """Fill the devices list"""
         device= str(self.ui.lineEdit.text())
         device += '*'
         try:
             items = list(self.getDb().get_device_exported(device))
-        except Exception,e:
+        except Exception as e:
             self.warning('Unable to contact with device %s: %s'%(device,str(e)))
             items=[]
         self.ui.devList.clear()
         devs=set([d.rsplit('/',1)[0].lower() for d in self.beingArchived])
         for i in items:
           item=Qt.QListWidgetItem()
           item.setText(str(i))
@@ -68,25 +68,25 @@
         return self.model
 
     def onButtonClicked(self):
         self.show_history(self.getModel())
 
     def show_history(self, attribute):
         TABS=[]
-        print 'getting archiving readers ...'
+        print('getting archiving readers ...')
         from PyTangoArchiving import Reader
         hdb = Reader(db='hdb',schema='hdb')
         tdb = Reader(db='tdb',schema='tdb')
         tformat = '%Y-%m-%d %H:%M:%S'
         str2epoch = lambda s: time.mktime(time.strptime(s,tformat))
         epoch2str = lambda f: time.strftime(tformat,time.localtime(f))
         attribute = attribute.lower()
 
         if attribute in hdb.get_attributes() or attribute in tdb.get_attributes():
-            print '%s is being archived' % attribute
+            print('%s is being archived' % attribute)
             di = Qt.QDialog()
             wi = di #QtGui.QWidget(di)
             wi.setLayout(Qt.QGridLayout())
             begin = Qt.QLineEdit()
             begin.setText(epoch2str(time.time()-3600))
             end = Qt.QLineEdit()
             end.setText(epoch2str(time.time()))
@@ -100,49 +100,49 @@
             wi.connect(buttons,Qt.SIGNAL('accepted()'),wi.accept)
             wi.connect(buttons,Qt.SIGNAL('rejected()'),wi.reject)
             wi.layout().addWidget(buttons,3,0,1,2)
 
             def check_values():
                 di.exec_()
                 if di.result():
-                    print 'checking result ...'
+                    print('checking result ...')
                     start,stop = str(begin.text()),str(end.text())
                     if not all(re.match('[0-9]+-[0-9]+-[0-9]+ [0-9]+:[0-9]+:[0-9]+',str(s).strip()) for s in (start,stop)):
-                        print 'dates are wrong ...'
+                        print('dates are wrong ...')
                         Qt.QMessageBox.warning(None,'Show archiving', 'Dates seem not in %s format'%(tformat), Qt.QMessageBox.Ok)
                         return check_values()
                     else:
-                        print 'getting values ...'
+                        print('getting values ...')
                         reader = tdb if str2epoch(start)>(time.time()-5*24*3600.) and attribute in tdb.get_attributes() else hdb
-                        print 'using %s reader' % reader.schema
+                        print('using %s reader' % reader.schema)
                         values = reader.get_attribute_values(attribute,str2epoch(start),str2epoch(stop))
                         if not len(values) and reader is tdb and attribute in hdb.get_attributes():
-                            print 'tdb failed, retrying with hdb'
+                            print('tdb failed, retrying with hdb')
                             values = hdb.get_attribute_values(attribute,str2epoch(start),str2epoch(stop))
-                        print 'drawing table from %d values' % len(values)
+                        print('drawing table from %d values' % len(values))
                         tab = Qt.QTableWidget()
                         tab.setWindowTitle('%s: %s to %s' % (attribute,start,stop))
                         tab.setRowCount(len(values))
                         tab.setColumnCount(2)
                         tab.setHorizontalHeaderLabels(['TIME','VALUE'])
                         for i,tup in enumerate(values):
                             date,value = tup
                             tab.setItem(i,0,Qt.QTableWidgetItem(epoch2str(date)))
                             tab.setItem(i,1,Qt.QTableWidgetItem(str(value)))
                         tab.show()
                         tab.resizeColumnsToContents()
                         tab.horizontalHeader().setStretchLastSection(True)
                         TABS.append(tab)
                         tab.connect(tab,Qt.SIGNAL('close()'),lambda o=tab: TABS.remove(o))
-                        print 'show_history done ...'
+                        print('show_history done ...')
                         return tab
                 else:
-                    print 'dialog closed'
+                    print('dialog closed')
                     return None
-            print 'asking for dates ...'
+            print('asking for dates ...')
             return check_values()
         else:
             Qt.QMessageBox.warning(None,'Show archiving', 'Attribute %s is not being archived'%attribute, Qt.QMessageBox.Ok) 
 
 class Ui_Form(object):
     def setupUi(self, Form):
         Form.setObjectName("Form")
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/widget/tests.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import sys
 
 from fandango.qt import Qt
 from taurus.qt.qtgui.container import TaurusWidget, TaurusMainWindow
-from PyTangoArchiving.widget import ContextToolBar
-from PyTangoArchiving.widget.snapdialogs import LoadForm 
 
 BO_DEVICES = ['BO/PC/BEND',                                                                                  
 
  'BO/PC/QH01',                                                                                  
 
  'BO/PC/QH02',
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/widget/trend.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/widget/trend.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,33 +69,33 @@
         })
 except: pass
 
 from PyTangoArchiving.reader import STARTUP
 global STARTUP_DELAY
 STARTUP_DELAY = 0.
 
-MAX_QUERY_TIME = 3600*24*10
-MAX_QUERY_LENGTH = int(1e5)
+MAX_QUERY_TIME = 3600*24*1000 #DISABLING THE BUNCHING SYSTEM (doesnt work)
+MAX_QUERY_LENGTH = 65536*1024 #int(1e7)
 MIN_REFRESH_PERIOD = 3.
 MIN_WINDOW = 60
 
 ZONES = fn.Struct({'BEGIN':0,'MIDDLE':1,'END':2})
 
 def dateHasChanged(prev,curr=None):
     v = all(curr) and (not prev or not any(prev[:2]) 
                         or any(abs(x-y)>MIN_WINDOW 
                                 for x,y in zip(curr,prev)))
     return v
 
 class ArchivingTrendWidget(TaurusGroupBox):
     def __init__(self, parent = None, designMode = False):
-        TaurusGroupBox.__init__(self, parent, designMode)
+        TaurusGroupBox.__init__(self, parent) #, designMode)
         self.setTitle('Archiving Trend')
         self.setLayout(Qt.QVBoxLayout())
-        self._trend = ArchivingTrend(parent=self,designMode = designMode)
+        self._trend = ArchivingTrend(parent=self) #,designMode = designMode)
         self._datesWidget = DatesWidget(trend=self._trend,parent=self,
             layout=Qt.QHBoxLayout)
         self._trend._datesWidget = self._datesWidget
         self.layout().addWidget(self._trend)
         self.layout().addWidget(self._datesWidget)
         self._datesWidget.show()
       
@@ -118,16 +118,16 @@
          #(lambda o:o._zoomBack())),
         ('_setAxisFormatOption','Set Y Axis Format',(lambda o:o._showAxisFormatDialog())),
         ('_pausedOption','Pause (P)',(lambda o:o.setPaused(not o.isPaused()))),
         ]
   
     def __init__(self, parent = None, designMode = False):
         actions = [a[1] for a in MenuActionAppender.ACTIONS]
-        print '>'*80+'\n'+str(MenuActionAppender.ACTIONS)
-        TaurusTrend.__init__(self,parent,designMode)
+        print('>'*80+'\n'+str(MenuActionAppender.ACTIONS))
+        TaurusTrend.__init__(self,parent) #,designMode)
         self.resetDefaultCurvesTitle()
         self.setXDynScale(True)
         self.setXIsTime(True)
         self.setUseArchiving(True)
         self.setModelInConfig(False)
         self.disconnect(self.axisWidget(self.xBottom), Qt.SIGNAL("scaleDivChanged ()"), self._scaleChangeWarning)
         #ArchivedTrendLogger(self,tango_host=fn.get_tango_host(fqdn=True),multiprocess=USE_MULTIPROCESS)
@@ -270,113 +270,88 @@
             self.replot()
         except:
             ms = Qt.QMessageBox.warning(self,"Error!",traceback.format_exc())
         
     def applyNewDates(self,dates=None):
         """
         Dates could be a tuple (start,end) or just (end,)
+        
+        #If two dates are passed, they are start and end
+        #If a single date is passed, then it is just the range
         """
         try:
-            #self.setForcedReadingPeriod(3000)
-            #self.setPaused(True)
-            ui = self._datesWidget
             logger = self.getArchivedTrendLogger()
+            # Update/Pause the Trend could cause unexpected behaviours!
+            #   self.setForcedReadingPeriod(3000)
+            #   self.setPaused(True)
+            
             if dates is not None:
-                ui.xRangeCB.setEditText(dates[-1])
-                end = dates[-1]
-            else:
-                end = str(ui.xRangeCB.currentText())
-
-            if dates is not None and len(dates)>1:
-                ui.xEditStart.setText(dates[0])
-                start = dates[0]
+                self._datesWidget.setRange(dates[-1])
+                if len(dates)>1:
+                    self._datesWidget.setStartDate(dates[0])
+                
+            t0 = self._datesWidget.getStartDate()
+            t1 = self._datesWidget.getRange()
+            logger.warning('applyNewDates(%s,%s)'%(t0, t1))
+        
+            if t0 is None: # start date is relative
+                now = time.time()
+                t0, t1 = time.time()-abs(t1), time.time()
             else:
-                start = str(ui.xEditStart.text())
-            
-            logger.warning('applyNewDates(%s,%s)'%(start,end))
-            
-            try: t0 = str2time(start)
-            except: t0 = None
-            try: t1 = str2time(end)
-            except: t1 = None
-        
-            if t1 is not None:
-                if t0 is None:
-                    now = time.time()
-                    t0,t1 = time.time()-t1,time.time()
-                else:
-                    if t0<0: t0 = time.time()+t0
-                    t0,t1 = t0,t0+t1
-                    try:
-                        if t1 > time.time() + 600:
-                            #If asked range goes into the future it is corrected
-                            r = t1-t0
-                            t1 = time.time() + 600
-                            t0 = t1 - r
-                            ui.xEditStart.setText(time2str(t0))
-                    except:
-                        traceback.print_exc()
+                t0 = t0 if t0>0 else time.time() + t0
+                t0, t1 = t0, t0 + abs(t1)
                 
             if t0 < fn.now() < t1 and t1-t0 > utils.MAX_RESOLUTION:
+                # For periods > 3h set readings at 10s
                 self.setForcedReadingPeriod(10000.)
                     
             if t1-t0 > 365*86400:
                 v = Qt.QMessageBox.warning(self,'Warning!',
                     'Reading an interval so big may hung your PC!!',
                     Qt.QMessageBox.Ok|Qt.QMessageBox.Cancel)
             
                 if t0 < 1000 or v == Qt.QMessageBox.Cancel:
                     return
         
             if t0 is not None:
-                
                 logger.warning('applyNewDates(%s,%s)'%(fn.time2str(t0),fn.time2str(t1)))
                 #Set Axis Scale already triggers Check Buffers!!!!
                 self.setAxisScale(Qwt5.QwtPlot.xBottom, t0, t1)
 
             ## DONT EVER APPLY SETPAUSED(TRUE); IT WILL NO ALLOW QT TO REFRESH
-            
             #logger.warning('Setting XDynScale != Paused = %s' % str(t1<time.time()))
             #self.setXDynScale(t1>time.time()) #%It causes weird effects
             #self.setPaused(t1<time.time())
                 
             self.emit(Qt.SIGNAL("refreshData"))
-            
         except:
             ms = Qt.QMessageBox.warning(self,"Error!",traceback.format_exc())
         
     def resetDefaultCurvesTitle(self):
         '''resets the defaultCurvesTitle property to '<label>'
 
         .. seealso:: :meth:`setDefaultCurvesTitle`'''
         self.setDefaultCurvesTitle('<label><[trend_index]><br>(<dev_name>/<attr_name>)')
         #self.setDefaultCurvesTitle('<label><[trend_index]>')
     
     def showDatesWidget(self,show=True):
         try:
             ui = getattr(self,'_datesWidget',None)
-            #try:
-                #ui.parent()
-            #except:
-                #self.warning(traceback.format_exc())
-                #ui = None
+
             if not ui:
                 self._datesWidget = Qt.QDialog()
                 self._datesWidget.setLayout(Qt.QVBoxLayout())
                 dw = DatesWidget(self)#,self.legend(),Qt.QVBoxLayout())
                 self._datesWidget.layout().addWidget(dw)
             
-            if show: self._datesWidget.show()
-            #else: self._datesWidget.hide()
+            if show: 
+                self._datesWidget.show()
             self.replot()
             return
-            #xMin = self.parent.axisScaleDiv(Qwt5.QwtPlot.xBottom).lowerBound()
-            #xMax = self.parent.axisScaleDiv(Qwt5.QwtPlot.xBottom).upperBound()
-            #if self.parent.getXIsTime():
-                    #self.ui.xEditMin.setText(time.strftime('%Y/%m/%d %H:%M:%S',time.localtime(int(xMin))))
+
         except:
             ms = Qt.QMessageBox.warning(self,"Error!",traceback.format_exc())
         
     def pickDataPoint(self, pos, scope=20, showMarker=True, targetCurveNames=None):
         '''Finds the pyxel-wise closest data point to the given position. The
         valid search space is constrained by the scope and targetCurveNames
         parameters.
@@ -445,23 +420,23 @@
             pickedCurveTitle = self.getCurveTitle(pickedCurveName)
             self.replot()
             label=self._pickedMarker.label()
             import PyQt4.Qwt5,PyQt4.Qt
             from datetime import datetime
             ax = pickedAxes[1]
             yformat = self.getAxisLabelFormat(ax) or "%.5g"
-            print yformat
+            print(yformat)
             s = "'%s'[%i]:\n\t (t=%s, y="+yformat+")"
             if self.getXIsTime():
                 data = (pickedCurveTitle,pickedIndex,datetime.fromtimestamp(picked.x()).ctime(),picked.y())
             else:
                 data = (pickedCurveTitle,pickedIndex,picked.x(),picked.y())
             try:
               infotxt = s%data
-              print infotxt
+              print(infotxt)
             except:
               traceback.print_exc()
               infotxt = "'%s'[%i]:\n\t (t=%s, y=%.5g)"%data
 
             label.setText(infotxt)
             fits = label.textSize().width()<self.size().width()
             if fits:
@@ -517,15 +492,15 @@
             history_ = parent.attribute_history(model.getSimpleName(), int(total))
             lasttime = 0
             if self._history:
                 lasttime = time2epoch(self._history[-1].time)
             history = [ h for h in history_ if lasttime<time2epoch(h.time) ]
             self.info(', %d values, %d are new'%(len(history_),len(history)))
             self._history=(self._history+history)[int(-total):]
-    except Exception,e: 
+    except Exception as e: 
         self.debug('Unexpected exception in TauTrendSet.handleEvent: '+str(e))
         self.traceback()
         #self._history = []
     return history
         
 def getTrendDimensions(self,value=None):
     if value is not None:
@@ -611,36 +586,37 @@
     This method implements decimation of archived and actual values 
     when filling trend buffers
     It should also allow to patch non correlative inserts of archived data 
     (inserting instead of extendLeft)
     """
     self.warning('In updateTrendBuffers(...)')
     t = []
+    ntrends = 1
     try:
         #self.curves_lock.acquire()
         import numpy,datetime,PyTangoArchiving.utils as utils
         from taurus.core.util.containers import ArrayBuffer
         logger = logger or self
         logmsg = lambda m: (fn.printf(m),self.warning(m)) #logger.warning
         trend_set = self
         parent = getattr(logger,'trend',logger)
         fromHistoryBuffer = data is not None and len(data) and hasattr(data[0],'time')
         
         if data is not None and len(data): 
             ###Adding archiving values
             try:
                 #It may clean existing buffers!
-                ntrends = self._checkDataDimensions(data[0].value 
-                                if fromHistoryBuffer else data[0][1]) 
+                value = data[0].value if fromHistoryBuffer else data[0][1]
+                ntrends = self._checkDataDimensions(value) 
             except:
                 logmsg(str(data[0]))
                 raise
             
             newsize = checkTrendBuffers(self,data,logger)
-            logger.warning('reader.updateTrendBuffers(): filling Buffer')
+            logger.warning('reader.updateTrendBuffers(%s): filling Buffer with %s' % (ntrends, newsize))
             try:
                 if fromHistoryBuffer:
                     t = numpy.zeros(len(data), dtype=float)
                     y = numpy.zeros((len(data), ntrends), dtype=float)#self._yBuffer.dtype)
                     t[:] = [v.time.totime() for v in data]
                     y[:] = [v.value for v in data]
                 else:
@@ -650,15 +626,15 @@
                         y = numpy.array([v[1] for v in data], dtype=float)
                     else:
                         y = numpy.zeros((len(data), ntrends), dtype=float)
                         for i,v in enumerate(data):
                             # Iterating will avoid getting stuck in errors
                             try:
                                 y[i] = v[1]
-                            except Exception,e:
+                            except Exception as e:
                                 logmsg(e)
                                 
                 overlap = ((len(t) and numpy.max(t) or 0) > 
                             (len(self._xBuffer) and numpy.min(self._xBuffer) 
                                 or fn.END_OF_TIME ))
                 minstep = abs(t[-1] - t[0]) / 1081.
                 logger.warning('In updateTrendBuffers('
@@ -705,42 +681,42 @@
                             len(t) and time2str(t[0]),
                             len(t) and time2str(t[-1]),
                             len(t) or 0,
                             fromHistoryBuffer,minstep))
                         
                 #logger.warning('new data length: %s, (%s,%s), (%s,%s)' 
                                #% (len(t), t[0], t[-1], y[0], y[-1]))
-            except Exception,e:
+            except Exception as e:
                 import traceback #Import is needed!
                 logger.warning('\tUnable to convert buffers[%d]! %s: %s'
                         %(ntrends,data and data[0],traceback.format_exc()))
                 t = []
             
             pending = getattr(getattr(logger,'reader',None),'callbacks',None)
             if not pending:
                 Qt.QApplication.instance().restoreOverrideCursor()
                 
             emitHistoryChanged(self)
             
-    except Exception,e:
+    except Exception as e:
         import traceback
         logger.warning('updateBuffer failed: %s'%(traceback.format_exc()))
     finally:
         print('-'*80)
         pass #self.curves_lock.release()
 
     return len(t)
         
 QT_CONNECTIONS = defaultdict(list)
 
 def replaceQtConnection(qobj,signal,callback):
     import functools
     for i,t in enumerate(QT_CONNECTIONS[signal][:]):
         if t[0]==qobj:
-            print 'disconnecting(%s,%s,%s)'%(qobj,signal,t[1])
+            print('disconnecting(%s,%s,%s)'%(qobj,signal,t[1]))
             qobj.disconnect(qobj,Qt.SIGNAL(signal),t[1])
             #qobj.disconnect(qobj,Qt.SIGNAL(signal),0,0)
             QT_CONNECTIONS[signal].remove(t)
     qobj.connect(qobj,Qt.SIGNAL(signal),callback)
     QT_CONNECTIONS[signal].append((qobj,callback))
 
 def getArchivedTrendValues(trend_set,model,start_date=0,stop_date=None,
@@ -776,15 +752,14 @@
         insert=False ; but always True when called from a TaurusTrendSet
         
     """
     import functools
     logger_obj = trend_set
     t00 = time.time()
     N = 0
-    trend_set.debug('In getArchivedTrendValues(%s) ...' % str(model))
     
     try:
         tango_host,attribute,model = parseTrendModel(model)
         parent = getTrendObject(trend_set)
         logger_obj = ArchivedTrendLogger(parent,tango_host=tango_host,
             multiprocess=multiprocess, value_setter = getArchivedTrendValues)
         
@@ -905,21 +880,31 @@
             'lasts=%s, getting new data (previous[%s]:%s at %s)'%(
             attribute,start_date,fn.time2str(start_date),stop_date,
             fn.time2str(stop_date),forced,reader.schema,lasts and lasts[0],
             model,lasts,lasts[-1]))
         logger_obj.debug('prev %s != curr %s' % (lasts,args))
         
         Qt.QApplication.instance().restoreOverrideCursor()
+        
+        # decimation = method, decimate = whether to decimate or not
         decimation = logger_obj.getDecimation()
-        if not decimation:
+        logger_obj.warning('decimation = %s' % str(decimation))
+        if not decimation: # RAW or client-side
             if decimation is not None: #RAW
                 if logger_obj.getNonesCheck(): 
                     decimation = fn.arrays.notnone
                 elif decimate: 
                     decimation = PyTangoArchiving.reader.data_has_changed
+        if decimation:
+            if decimation in ('AUTO','0'):
+                decimation = (stop_date - start_date) / utils.MAX_RESOLUTION
+            if fn.isNumber(decimation):
+                decimation = int(decimation)            
+                    
+        logger_obj.warning('decimation = %s' % str(decimation))
             
         if not multiprocess or not isinstance(reader,ReaderProcess):
             Qt.QApplication.instance().setOverrideCursor(
                                     Qt.QCursor(Qt.Qt.WaitCursor))
             
             ###################################################################
             tr = fn.now()
@@ -931,14 +916,16 @@
                 'trend.%s.get_attribute_values(%s,%s,%s,%s,%s):'
                     '\n\t%d %s readings in %f s: %s ...\n' % (reader.schema,
                     model,time2str(start_date),time2str(stop_date),
                     decimation,N,len(history),reader.schema,fn.now()-tr,
                     ','.join([str(s) for s in history[:3]]) ))
                     
             #logger_obj.warning('%s , %s , %s' % (start_date,bounds[0],start_date<=bounds[0]))
+
+            # THIS CHECK IS ONLY FOR BUNCHED QUERIES (N!=0)
             if ((0 < len(history) < abs(N) and area>(.11,.05)[zone==ZONES.MIDDLE])
                 or start_date<=bounds[0]):
                 # Windowed query was finished, stop refreshing
                 check = fn.tango.check_attribute(model,readable=True)
                 #logger_obj.warning(check)
                 if not check:
                     logger_obj.warning('Pausing %s ...'%attribute)
@@ -1046,26 +1033,26 @@
         tt.setXDynScale(True)
         tt.setXIsTime(True)
         tt.setUseArchiving(True)
         tt.setModelInConfig(False)
         tt.disconnect(tt.axisWidget(tt.xBottom), 
             Qt.SIGNAL("scaleDivChanged ()"), tt._scaleChangeWarning)
         xMax = time.time() #tt.axisScaleDiv(Qwt5.QwtPlot.xBottom).upperBound()
-        rg = length #abs(self.str2deltatime(str(self.ui.xRangeCB.currentText())))
+        rg = length
         xMin=xMax-rg
         tt.setAxisScale(Qwt5.QwtPlot.xBottom,xMin, xMax)
         if n_trends>1: qw.layout().addWidget(tt)
         elif show: tt.show()
       tt1 = trends[0]
       if models: 
           tt1.setModel(models)
           tt1.setWindowTitle(str(models))
     except:
-        print 'Exception in set_pressure_trend(%s)'%tt
-        print traceback.format_exc()
+        print('Exception in set_pressure_trend(%s)'%tt)
+        print(traceback.format_exc())
     if show and n_trends>1: qw.show()
     return qw if n_trends>1 else tt1
         
 ###############################################################################
             
 if __name__ == "__main__":
     import sys
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/__init__.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,66 +35,78 @@
 </li></ul><ul><li>Start/Stop Archiving devices in the appropiated order.
 </li></ul><ul><li>Increase the capabilities of configuration and diagnostic.
 </li></ul><ul><li>Import/Export .csv and .xml files between the archiving and 
     the database.
 
 """
 
-RELEASE = (6,4,0)
+import os, sys, traceback
+
+try:
+    __RELEASE__ = open(os.path.dirname(os.path.abspath(__file__)
+                                       ) + '/VERSION').read().strip()
+except Exception as e:
+    __RELEASE__ = '6.X+'
+
+import traceback, os
+try:
+  v = __RELEASE__.split('.')
+  RELEASE = tuple(map(int,v))
+except:
+  traceback.print_exc()
+  print('Unable to read PyTangoArchiving.VERSION')
 
 ARCHIVING_TYPES = ['hdb','tdb','snap']
 ARCHIVING_CLASSES =     ['HdbArchiver','TdbArchiver','SnapArchiver',
                     'HdbExtractor','TdbExtractor','SnapExtractor',
                     'ArchivingManager','SnapManager',
                     #'HdbArchivingWatcher','TdbArchivingWatcher',
                     ]
 MAX_SERVERS_FOR_CLASS=5
 MIN_ARCHIVING_PERIOD=10
 
 import fandango as fn
 
-import utils
-import dbs
-import common
+from . import utils
+from . import dbs
+from . import common
 #import reader ; should be loaded the last
-import archiving
-import files
+from . import archiving
+from . import files
 
-from common import CommonAPI
-from common import getSingletonAPI as getCommonAPI
-from schemas import Schemas
-from archiving import ArchivingAPI,ArchivedAttribute
-from utils import check_attribute
-from check import check_archiving_schema
-from files import GetConfigFiles,LoadArchivingConfiguration,\
+from .dbs import get_host_databases
+from .common import CommonAPI
+from .common import getSingletonAPI as getCommonAPI
+from .schemas import Schemas, get_archiving_hosts
+from .archiving import ArchivingAPI,ArchivedAttribute
+from .utils import check_attribute
+try:
+    from .check import check_archiving_schema, check_db_schema
+except:
+    traceback.print_exc()
+    print('failed to load check module (not critical)')
+
+from . files import GetConfigFiles,LoadArchivingConfiguration,\
     CheckArchivingConfiguration,ParseCSV,StopArchivingConfiguration
 
 __all__=['reader','archiving','utils','files','common']
 
 try:
-    import snap
-    from snap import SnapDB,SnapAPI
-    __all__.extend(('snap',))#'SnapDB','SnapAPI'))
-except:
-    print('Unable to import snap')
-
-try:
-   import hdbpp
-   from hdbpp import HDBpp, multi
-   from hdbpp.multi import start_archiving_for_attributes, \
-       get_last_values_for_attributes
-  
+   from . import hdbpp
+   from .hdbpp import HDBpp, multi
+   from .hdbpp.multi import start_archiving_for_attributes, \
+       get_last_values_for_attributes, get_hdbpp_databases
 except:
    print('Unable to import hdbpp') 
 
 api = Schemas.getApi #ArchivingAPI
 
 #Order matters!, it should be the last import
-import reader
-from reader import Reader,getArchivedTrendValues
+from . import reader
+from .reader import Reader,getArchivedTrendValues
 
 """
 Some interesting queries;
 
 select ID,full_name from adt;
 select ID,archiver,start_date,stop_date from amt;
 select ID,full_name,data_type,writable from adt;
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/archiving.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/archiving.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,19 +139,19 @@
     ArchivingAPI(schema,host=None,user='browser',passwd='browser',classes=[],LogLevel='info',load=False,values=False)
     """
     KEEPING_PERIOD = 5*24*60*60 # Time, in seconds, that the data will be kept in TDB database
     EXPORT_PERIOD = 10*60 # Time, in seconds, that TDB data will be buffered before inserting in MySQL
     SCHEMAS = ('hdb','tdb')
     
     def __init__(self,schema,host=None,user='browser',passwd='browser',
-                 classes=[],LogLevel='info',load=False,values=False,
+                 classes=[],LogLevel='warning',load=False,values=False,
                  dedicated=False, tango_host='',logger=None, ):
 
         self.schema = schema.lower()
-        assert self.schema in self.SCHEMAS, 'UnknownSchema_%s'%schema
+        #assert self.schema in self.SCHEMAS, 'UnknownSchema_%s'%schema
         CommonAPI.__init__(self,self.schema,host,user,passwd,
                 classes=self.get_archiving_classes(),LogLevel=LogLevel,
                 load=load,logger=logger)
         
         self.tango_host = tango_host or fandango.get_tango_host()
         self.db = ArchivingDB(self.schema,self.host,self.user,self.passwd)
         self.load_all(values=values,dedicated=load and dedicated,servers=load)
@@ -161,43 +161,43 @@
         self.ArchivingClasses = [k for k in ARCHIVING_CLASSES if self.schema in k.lower()]
         if self.schema!='snap': self.ArchivingClasses.append('ArchivingManager')
         return self.ArchivingClasses
     
     def __clean_extractor(self,extractor,vattr=None):
         ''' removing dynamic attributes from extractor devices ...'''
         #self.log.debug('In PyTangoArchiving.Reader.__cleanExtractor(): removing dynamic attributes')
-        print 'In PyTangoArchiving.Reader.__cleanExtractor(): removing dynamic attributes'
+        print('In PyTangoArchiving.Reader.__cleanExtractor(): removing dynamic attributes')
         if isinstance(extractor,PyTango.DeviceProxy): 
             name,proxy=extractor.dev_name(),extractor
         else: 
             name,proxy=extractor,self.get_servers().proxies[extractor]
         if vattr: proxy.RemoveDynamicAttribute(vattr)
         else: proxy.RemoveDynamicAttributes()              
         
     def __extractorCommand(self,extractor=None,command='',args=[]):
-        if not command: raise Exception,'Reader__extractorCommand:CommandArgumentRequired!'
+        if not command: raise Exception('Reader__extractorCommand:CommandArgumentRequired!')
         if not extractor: extractor = self.get_extractor()
         extractor.ping()
         try:
-            print 'in Reader.__extractorCommand: calling HdbExtractor command %s(%s)'%(command,args)            
+            print('in Reader.__extractorCommand: calling HdbExtractor command %s(%s)'%(command,args))            
             result = extractor.command_inout(*([command]+(args and [args] or [])))
-        except PyTango.DevFailed, e:
+        except PyTango.DevFailed as  e:
             #e.args[0]['reason'],e.args[0]['desc'],e.args[0]['origin']
             reason = '__len__' in dir(e.args[0]) and e.args[0]['reason'] or e.args[0]
             if 'Broken pipe' in str(reason):
                 extractor.init()
                 result = extractor.command_inout(*([command]+(args and [args] or [])))
             elif 'MEMORY_ERROR' in str(reason):
                 self.clean_extractor()
                 extractor.init()                
-                raise Exception,'Extractor_%s'%reason
+                raise Exception('Extractor_%s'%reason)
             else:
-                print traceback.format_exc()
-                raise Exception,'Reader__extractorCommand:Failed(%s)!'% str(e)
-        print 'in Reader.__extractorCommand: command finished'
+                print(traceback.format_exc())
+                raise Exception('Reader__extractorCommand:Failed(%s)!'% str(e))
+        print('in Reader.__extractorCommand: command finished')
         return result
                 
     #----------------------------------------------------------------------------------------------
     # METHODS TO GET/SET ARCHIVING INFORMATION    
     
     def get_archived_attributes(self,attrs=None):
         #return self.__extractorCommand(self.get_extractor(),'GetCurrentArchivedAtt')
@@ -218,15 +218,17 @@
             self.load_attribute_modes()
         if not attribute_list: attribute_list = sorted(self.attributes)
         elif isinstance(attribute_list,str): attribute_list = [attribute_list]
         attribute_list = ['/'.join(a.split('/')[-4:]) for a in attribute_list]
         return dict((a,self[a].archiver) for a in attribute_list)
 
     def get_archivers_load(self):
-        '''def getArchiversLoad(self,schema): return a dict with archiver:load for the given schema'''
+        '''
+        return a dict with archiver:load for the given schema
+        '''
         archivers = defaultdict(list)
         [archivers[self[a].archiver.lower()].append(a) for a in self]
         return archivers
     
     def get_attribute_by_ID(self,ID):
         for a in self.attributes.values():
             if a.ID==ID: return a
@@ -244,21 +246,21 @@
         '''
         dbattrs = self.attributes
         newattributes=[]
         for a,v in attribute_list.items():
             if a in dbattrs:
                 modes=v['modes']
                 dbmodes=dbattrs[a].extractModeString()
-                #print a,':',modes
-                #print '\tDB:',dbmodes
+                #print(a,':',modes)
+                #print('\tDB:',dbmodes)
                 for k,v in modes.items():
                     if k not in dbmodes: continue
                     else:
                         if len(modes[k])!=len(dbmodes[k]) or any(modes[k][i]>dbmodes[k][i] for i in range(len(modes[k]))):
-                            #print a,':',k,'=',v,' vs DB:',dbmodes[k]
+                            #print(a,':',k,'=',v,' vs DB:',dbmodes[k])
                             self.log.debug('%s:%s = %s vs DB: %s'%(str(a),str(k),str(v),str(dbmodes[k])))
                 pass
             else:
                 self.log.debug('%s,New attribute!: %s'%(a,v))
                 newattributes.append(a)
         return newattributes    
 
@@ -302,15 +304,15 @@
         return self.proxies[archiver].command_inout('StateDetailed')     
     
     @staticmethod
     def check_modes(schema,modes,min_periodic=0,min_absolute=.01,min_relative=1):
         """ modes must be a dictionary in the form: {'MODE_X':[params]} 
         This is Tango!!! ... so periods must be milliseconds!
         """
-        #print 'ArchivingAPI.check_modes(%s,%s)'%(schema,modes)
+        #print('ArchivingAPI.check_modes(%s,%s)'%(schema,modes))
         if type(modes) in (int,float): modes = {'MODE_P':[modes]}
         porder = ['MODE_P','MODE_A','MODE_R','MODE_T','MODE_C','MODE_D','MODE_E']        
         arch_type = schema.lower() #'hdb' or 'tdb'
         min_periodic = min_periodic or (('MODE_R' in modes or 'MODE_A' in modes) and (30000 if schema.lower()=='tdb' else 5000)) or (10000 if schema.lower()=='hdb' else 1000)
         max_periodic = (('MODE_R' in modes or 'MODE_A' in modes) and 43200000) or (60000 if schema.lower()=='tdb' else 3600000)
         new_modes = {}
         corrections = 0
@@ -388,15 +390,15 @@
                 if ac.data_format!=ad.data_format:
                     self.log.warning('Attribute %s Format differs between Tango(%s) and ADT(%s)'% \
                         (attr,PyTango.AttrDataFormat.values[ac.data_type],PyTango.AttrDataFormat.values[ad.data_type]))
                 #Checking WRITE type
                 if ac.writable!=ad.writable:
                     self.log.warning('Attribute %s WriteType differs between Tango(%s) and ADT(%s)'% \
                         (attr,PyTango.AttrWriteType.values[ac.writable],PyTango.AttrWriteType.values[ad.writable]))
-            except Exception,e:
+            except Exception as e:
                 self.log.warning('Unable to get AttributeConfig for %s: %s'%(attr,str(e)))
         return repaired      
                   
     def check_archivers(self,archivers=[], load=False):
         """ This method checks if archiver devices are effectively running (StateDetailed should not trigger exception) 
         
         :return: {Archiver:True/None/False} # It will return True if device is Ok, 
@@ -493,15 +495,15 @@
                                         except: diff = 0
                                         self.log.warning('FAILED %s(%s)(%s):%s(%s)\n\t between %s and %s;\n\t delay =  %s; diff = %s = %1.1f%%' %
                                             (type(v1).__name__,attribute,archiver,mode,params,time.ctime(t0),time.ctime(t1),(t1-t0-period),diff,abs(100.*diff/v0) if (diff and v0) else 0))
                                     errors[attribute][mode].append(t1)
                             t0,v0 = t1,v1
                         if errors[attribute]: errors[attribute]=dict(errors[attribute])
                         else: errors.pop(attribute)
-            except Exception,e:
+            except Exception as e:
                 #self.log.warning('FAILED %s(%s) ... %s'%(attribute,archiver,traceback.format_exc()))#e))
                 self.log.warning('FAILED %s(%s,%s); line %d:  %s'%(attribute,archiver,modes,sys.exc_info()[2].tb_lineno,e))
                 if 'Commands out of sync' in str(e): 
                     self.db.renewMySQLconnection()
                     return self.check_attributes_errors(attributes,hours,load,exclude,lazy=True)
                 else: errors[attribute] = dict([(m,[0]) for m in modes])
         self.log.warning('In check_attributes_errors(...): %d attributes checked, %d errors found'%(len(attributes),len(errors)))
@@ -518,15 +520,15 @@
     def get_attribute_values(self,attribute,start_date,stop_date=None,asHistoryBuffer=False):
         ''' THIS METHOD IS DEPRECATED ... USE PyTangoArchiving.Reader object instead
         def attr_getValues(self,attribute,start_date,stop_date=None):
         This method uses an H/TdbExtractor DeviceServer to get the values from the database.
         The format of values returned is [(epoch,value),]
         The flag 'asHistoryBuffer' forces to return the rawHistBuffer returned by the DS.
         '''
-        raise Exception,'Deprecated_by_PyTangoArchiving.Reader.get_attribute_values'
+        raise Exception('Deprecated_by_PyTangoArchiving.Reader.get_attribute_values')
         
         if not stop_date: stop_date=time.time()
         self.log.debug( 'in getArchivedValues(%s) ...'%self.schema)
         if type(start_date) is not str: start_date=time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(start_date))
         if type(stop_date) is not str: stop_date=time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(stop_date))
         extractor=self.get_extractor()
         self.log.debug( 'GetAttDataBetweenDates(',str([attribute,start_date,stop_date]),')')
@@ -610,15 +612,15 @@
                     dp.set_timeout_millis(timeout)
                     dp.ping()
                 def retry_command(comm,retries=retries):
                     """ Function added to do commands with retries. """
                     e0 = None
                     for x in reversed(range(retries)):
                         try: return comm()
-                        except Exception,e: 
+                        except Exception as e: 
                             e0 = e0 or e
                             self.log.error('%s_archiving(...): %s command_inout failed, %d retries left' % (action.lower(),str(comm),x))
                             if 'IllegalStateException' in str(e): 
                                 self.log.warning('java.lang.IllegalStateException?... probably worked, reload attribute_modes and check api[a].archiver')
                                 break
                             elif not x: raise e0
                             time.sleep(10.)
@@ -647,17 +649,17 @@
                             sserver = self.get_servers().get_device_server(self.attributes[a].archiver)
                             modified_archivers.add(sserver)
                             self.log.info('Server %s added to restart list'%sserver)
                     print(archiver,archatts,stoplist)
                 #Stopping archiving
                 if stoplist:
                     self.log.info('Stopping archiving for %s attribs ...'%(len(stoplist)<100 and stoplist or str(len(stoplist))))
-                    #print 'Stopping archiving for %s attribs ...'%(len(stoplist)<100 and stoplist or str(len(stoplist)))
+                    #print('Stopping archiving for %s attribs ...'%(len(stoplist)<100 and stoplist or str(len(stoplist))))
                     try: retry_command(lambda dp=dp:dp.command_inout('ArchivingStop%s'%self.schema.upper(),stoplist))
-                    except Exception,e:
+                    except Exception as e:
                         if action=='stop': raise e
                         else: self.log.info('ArchivingStop%s failed ... '%self.schema.upper())
                 elif action=='stop': self.log.warning('No attributes were stop! (not archived or archiver not running)')
     
                 time.sleep(1.)
                 #Starting archiving
                 if attribute_list and action.lower().strip() == 'start':
@@ -686,22 +688,22 @@
                     if any(a not in self for a in attribute_list):
                         self.load_attribute_descriptions()
                         self.load_attribute_properties()
                     self.load_attribute_modes(attribute_list) 
                     check_result(attribute_list,action)
                 self.log.debug('Out of %s_archiving(...)'%(action))
                 return True
-            except PyTango.DevFailed,e:
+            except PyTango.DevFailed as e:
                 try:
                     if any(['supported' in a.desc.lower() for a in e.args]):
                         self.log.warning()
                 except:pass
                 PyTango.Except.print_exception(e)
                 return False
-            except Exception,e:
+            except Exception as e:
                 exstring = traceback.format_exc()
                 self.log.warning('Exception occurred and catched at %s_archiving: %s'%(action,exstring))
                 self.log.warning('Last exception was: \n'+str(e)+'\n')
                 return False
         pass
     
     def stop_archiving(self,attribute_list,load=True,retries=1,max_errors=3,kill=False,max_list=5): 
@@ -750,26 +752,26 @@
         self.db.renewMySQLconnection()
         if servers: self.load_servers()
         self.load_attribute_descriptions(attributes)
         if properties: self.load_attribute_properties() #Not frequently used and slow to load
         self.load_attribute_modes(attributes)
         if dedicated: 
             try: self.dedicated = self.load_dedicated_archivers()
-            except Exception,e: self.log.warning('Unable to get dedicated archivers: %s'%traceback.format_exc())
+            except Exception as e: self.log.warning('Unable to get dedicated archivers: %s'%traceback.format_exc())
         if values: self.load_last_values(n=1)
 
     def load_attribute_descriptions(self,attributes=None):
         try:
           self.log.info('Loading attributes description from %s database ...'%self.schema)
           if attributes is None:
             lines=self.db.get_attribute_descriptions()
           else:
             lines=[l for a in attributes for l in self.db.get_attribute_descriptions(a)]
           for line in lines:
-              #print str(line)
+              #print(str(line))
               attribute,ID,data_type,data_format,writable=line
               if attribute not in self.attributes:
                   self.attributes[attribute]=ArchivedAttribute(name=attribute,device=attribute.rsplit('/',1)[0],Type=self.schema)
               self.attributes[attribute].setID(ID)
               self.attributes[attribute].setConfig(data_type,data_format,writable)
               #self.attributes[attribute].archiver=line[2]
               #self.log.debug( 'Attribute configuration is {%s,%s,%s}'%tuple(
@@ -834,15 +836,15 @@
                 self.log.debug( 'Attribute %s Status loaded: %s,%s,%s'%tuple(
                     [a+':'+str(getattr(self.attributes[att.name],a)) for a in ['name','archiver','start_date','archiving_mode']]))
             else:
                 self.attributes[att.name].setArchiver('') #This allows to differentiate not archived attributes
         
         return dict((a,self.attributes[a].modes) for a in attributes)
     
-    def load_last_values(self,attribute=None,n=1,cache=0):
+    def load_last_values(self,attribute=None,n=1,cache=0,epoch=fun.END_OF_TIME):
         ''' def DB_getLastNValues(self,attribute,n=1):
         attribute argument could be an string, list or 'ALL' for updating all atributes
         The method returns N registers (1 by def.) ordered BY TIME DESC! (last first)
         The AttributesList.lastValue is updated
         The cache attribute must be integer, values newer than (now - cache) will not be updated
         :returns:  [[t0,v0],[t-1,v-1]]
         '''
@@ -854,15 +856,15 @@
             self.log.warning( 'attribute list is empty, try load_attributes_descriptions()')
             return None
         elif fandango.isIterable(attribute): 
             self.log.info('Getting last [%d] attributes values from %s database ...'%(len(attribute or self.attributes),self.schema))
             #self.log.debug('Getting values for a list of attributes ...')
             values = {}
             for att in (type(attribute) in [list,set] and attribute or self.attributes):
-                values[att] = self.load_last_values(att, n, cache)
+                values[att] = self.load_last_values(att, n, cache, epoch=epoch)
                 self.log.debug('Last values acquired for %s'%att)
                 if not values[att] and att in self.attributes and self.attributes[att].archiver: 
                     self.log.info('Attribute %s archived by %s has no values in archiving database!'%(str(att),str(self.attributes[att].archiver)))
             #IT SHOULD BE SORTED BY TIME!!!
             return values
         
         attribute = '/'.join(attribute.split('/')[-4:])
@@ -874,23 +876,24 @@
             self.log.debug('Preparing query for  %s ...'%attribute)
             att=self.attributes[attribute]
             #self.log.debug('Preparing query for  %s ...'%att)
             if n==1 and cache and att.last_date>now-int(cache):
                 lines = [[fandango.time2date(att.last_date),att.last_value]]
             else:
                 try:
-                    lines = self.db.get_last_attribute_values(att.table,n)
+                    lines = self.db.get_last_attribute_values(att.table,n,epoch=epoch)
                     if len(lines):
                         value,date=lines[0][1],time.mktime(lines[0][0].timetuple())+1e-6*lines[0][0].microsecond
                         self.attributes[attribute].setLastValue(value,date)
-                        if self.attributes[attribute].archiver and date<(now-max([3600]+[mode[0]/1000. for mode in self[attribute].modes.values()])): 
+                        if ((epoch is None or epoch > now) and self.attributes[attribute].archiver and 
+                            date<(now-max([3600]+[mode[0]/1000. for mode in self[attribute].modes.values()]))):
                             self.log.debug('%s (%s) has no values since %s.'%(attribute,self.attributes[attribute].archiver,time.ctime(date)))
                     elif self.attributes[attribute].archiver:
                         self.log.error('No values has been found for attribute %s!'%attribute)
-                except Exception,e:
+                except Exception as e:
                     self.log.error('Exception while acquiring data from MySQL for attribute %s:\n%s'%(attribute,traceback.format_exc()))
                     self.attributes[attribute].exception='%s:%s'%(time.ctime(),str(e))
             return lines
                 
     def load_attribute_values(self,attribute,start_date,stop_date):
         if not self.attributes:
             self.log.warning( 'ERROR!: loadAttributesDescriptionFIRST!')
@@ -1041,31 +1044,31 @@
                             self.tango.put_device_property(di.name,{'isDedicated':True,'reservedAttributes':assigned[next_archiver]})
                             if self.schema.lower()=='tdb':
                                 props = self.tango.get_class_property('TdbArchiver',['DbPath','DsPath','DiaryPath'])
                                 self.tango.put_device_property(di.name,props)
                     x,iarchiver = x+len(attribs),iarchiver+1
                 iserver+=1
                 iarchiver=1
-            print ''
+            print('')
             
         [self.servers.load_by_name(k) for k in self.get_archiving_classes()]
         
         ## Returns a dictionary with {archiver:[attributes]} for all archivers in the given hosts
         return assigned
 
 
     ###########################################################################################################
     # Old dedicated code
     ###########################################################################################################    
         
         #archivers=self.get_archivers_load()
         #if archivers:
-            #print 'Loads of existing archivers are: '
+            #print('Loads of existing archivers are: ')
             #for n,l in archivers.items():
-            #if l: print '%s:\t%d'%(n,l)
+            #if l: print('%s:\t%d'%(n,l))
         
         ##Using the result of api.DB_loadAttrStatus() instead   #creating a dictionary {attribute:archiver}
         #previous_archiver={}
         #for a in api.attributes.values():
             #if a.archiver: previous_archiver[a.name.lower()]=a.archiver
         
         ##Getting the previous dedicated variables introduced in the archiving system
@@ -1082,120 +1085,120 @@
         #for a in atts:
             #archiver,host,label,serial='','','',1
             #dev=a.rsplit('/',1)[0]
             #host=attrslist[a]['host']
             
             ##Create regular expression for finding a suitable archiver
             #if dev in dedicated.keys():
-            #print 'The device %s has a dedicated archiver.'%dev
+            #print('The device %s has a dedicated archiver.'%dev)
             #label = dedicated[dev]
             #reg = ('(.*?%s.*?%s-)([0-9]{2,2})'%(host,label)).lower()
             #server='%sArchiver/%s_%s'%('Hdb' if arch_type=='hdb' else 'Tdb',host,label)
-            ##print 'The attribute %s is dedicated for %s/%s'%(a,host,label)
+            ##print('The attribute %s is dedicated for %s/%s'%(a,host,label))
             #else:
-            ##print 'The attributes is not dedicated, uses generic archivers'
+            ##print('The attributes is not dedicated, uses generic archivers')
             #reg = ('(.*-)([0-9]{1,2})')
             #server='%sArchiver/%s'%('Hdb' if arch_type=='hdb' else 'Tdb',host)
             
             #if a.lower() in previous_archiver.keys() and re.match(reg,previous_archiver[a.lower()].lower()):
             ##Keeping the same archiver that was being used previously
             #archiver=previous_archiver[a.lower()]
-            #print 'Attribute %s will use the same archiver %s'%(a,archiver)
+            #print('Attribute %s will use the same archiver %s'%(a,archiver))
             
             ##DEPRECATED BECAUSE THE API DOESN'T RESPECT THE EXECUTABLE NAME CASE
             ##try:
                 ##server=api.API_getProxy(archiver).info().server_id
             ##except Exception,e:
-                ##print e
+                ##print(e)
             
             ##Adding to mod_hosts the server with not_running archivers
             #if not api.server_Ping(archiver):
                 #if host not in mod_hosts: mod_hosts[host]={}
                 #if server not in mod_hosts[host]: mod_hosts[host][server]=[]
-                #print 'Archiver %s exists but is not running, it must be started!'%(archiver)
+                #print('Archiver %s exists but is not running, it must be started!'%(archiver))
                 #mod_hosts[host][server].append(archiver)
             #else:  
             ##Creating a new link archiver-attribute
-            ##print 'Creating a new Archiver-Attribute link (%s) for %s'%(reg,a)
+            ##print('Creating a new Archiver-Attribute link (%s) for %s'%(reg,a))
             #match = [arch for arch in archivers if re.match(reg,arch)]
             ##To an existing archiving server ... (could need a new archiver instance)
             #if match:
                 #match.sort()#Getting the last of the matching archiver names
                 #suitable = [m for m in match if archivers[m]<MAX_INSTANCE_LOAD]
                 #lastmatch = re.match(reg,match[-1])
                 ##With Full Load
                 #if not suitable:
                 #archiver='%s%02d'%(lastmatch.groups()[0],(int(lastmatch.groups()[-1])+1))
-                ##print 'Archiver %s overloaded (%d), creating %s'%(lastmatch.group(),archivers[lastmatch.group()],archiver)
+                ##print('Archiver %s overloaded (%d), creating %s'%(lastmatch.group(),archivers[lastmatch.group()],archiver))
                 ##Reusable
                 #else: 
                 #archiver=suitable[0]
-                ##print 'Suitable archiver %s found for attribute %s,' % (str(archiver),a)
+                ##print('Suitable archiver %s found for attribute %s,' % (str(archiver),a))
                 #archivers[archiver]+=1
                 ##DEPRECATED BECAUSE THE API DOESN'T RESPECT THE EXECUTABLE NAME CASE
                 ##try:
                 ##dp=PyTango.DeviceProxy(archiver if suitable else lastmatch.group())
                 ##server=dp.info().server_id
-                ##print 'Server name got from TangoDB : %s'%server
+                ##print('Server name got from TangoDB : %s'%server)
                 ##except Exception,e:
                 ###Using the name previously generated
                 ##pass
             ##To a New Dedicated Archiver ...
             #elif dev in dedicated.keys():
                 #archiver='%sArchiver/%s/%s-01'%('Hdb' if arch_type=='hdb' else 'Tdb',host,label)
                 #server='%sArchiver/%s_%s'%('Hdb' if arch_type=='hdb' else 'Tdb',host,label)
             #else:
-                #print 'No matching archiver has been found for %s'%a
+                #print('No matching archiver has been found for %s'%a)
         
             ##Adding to mod_hosts the server with new,not_running or dedicated archivers
             #if archiver not in archivers.keys() or not api.server_Ping(archiver) or dev in dedicated.keys():
                 #if host not in mod_hosts: mod_hosts[host]={}
                 #if server not in mod_hosts[host]: mod_hosts[host][server]=[]
                 #if not (dev in dedicated.keys()): #The archiver is new or not running
                 #if archiver not in archivers.keys(): #Creating new archivers if necessary
-                    #print 'Creating new archiver %s on %s'%(archiver,server)
+                    #print('Creating new archiver %s on %s'%(archiver,server))
                     #di = DbDevInfo()
                     #di.name,di._class,di.server = archiver,'%sArchiver'%('Hdb' if arch_type=='hdb' else 'Tdb',),server
                     #api.db.add_device(di)
                     #archivers[archiver.lower()]=1
                     #archiver_properties[archiver.lower()]={}
                 #else: #It means that server_Ping has failed! 
-                    #print 'Archiver %s exists but is not running, it must be started!'%(archiver)
+                    #print('Archiver %s exists but is not running, it must be started!'%(archiver))
                 #mod_hosts[host][server].append(archiver)
                 #else:
                     #pass
                 #pass
                 
             #if dev in dedicated.keys():
                 ##Update isDedicated and reservedAttributes properties if necessary
-                ##print 'archiver_properties length is %d vs %d archivers'%(len(archiver_properties),len(archivers))
+                ##print('archiver_properties length is %d vs %d archivers'%(len(archiver_properties),len(archivers)))
                 #for arch,d in archiver_properties.items():
                 #if arch==archiver.lower():
                     #if 'reservedAttributes' not in d: 
-                    ##print 'Adding default Dedicated properties to archiver %s'%(arch)
+                    ##print('Adding default Dedicated properties to archiver %s'%(arch))
                     #d['reservedAttributes']=[]
                     #if 'isDedicated' not in d or not d['isDedicated']: d['isDedicated']=['TRUE']
                     #if a not in d['reservedAttributes']:
-                    #print 'Adding attribute %s to archiver %s'%(a,arch)
+                    #print('Adding attribute %s to archiver %s'%(a,arch))
                     #d['reservedAttributes'].append(a)
                     #if archiver not in mod_hosts[host][server]: mod_hosts[host][server].append(archiver)
                     #if archiver not in mod_archivers: mod_archivers.append(archiver)
                     #else:
-                    #print 'The attribute %s was already assigned to archiver %s; but it doesnt appear to be the actual archiver!!!'%(a,arch)
+                    #print('The attribute %s was already assigned to archiver %s; but it doesnt appear to be the actual archiver!!!'%(a,arch))
                     #if archiver not in mod_hosts[host][server]: mod_hosts[host][server].append(archiver)
                     #if archiver not in mod_archivers: mod_archivers.append(archiver)
                 #elif 'reservedAttributes' in d and a in d['reservedAttributes']:
-                    #print 'Removing attribute %s from archiver %s'%(a,arch)
+                    #print('Removing attribute %s from archiver %s'%(a,arch))
                     #d['reservedAttributes'].remove(a)
                     ##@TODO: When host information for existing servers become readable
                     ## this lines must be changed.
                     #mod_hosts[host][server].append(arch)
                     #if arch not in mod_archivers: mod_archivers.append(arch)
                 #elif ('reservedAttributes' not in d or not len(d['reservedAttributes'])) and 'isDedicated' in d and 'TRUE' in d['isDedicated']:
-                    #print 'Removing isDedicated property from archiver %s'%(arch)
+                    #print('Removing isDedicated property from archiver %s'%(arch))
                     #d['reservedAttributes']=[]
                     #d['isDedicated']=['FALSE']
                     #mod_hosts[host][server].append(arch)
                     #if arch not in mod_archivers: mod_archivers.append(arch)
                 ##Updating the modified properties
                 #archiver_properties[arch]=d
                 
@@ -1205,21 +1208,21 @@
             #if arch_type.lower()=='tdb':
             #if archiver in archiver_properties.keys():
                 #val = archiver_properties[archiver]
             #else: archiver_properties[archiver],val = {},{}
             #pathprops=['DbPath','DiaryPath','DsPath']
             #tdbpath='/tmp/archiving/tdb'
             #if any(p not in val or val[p][0]!=tdbpath for p in pathprops):
-                #print 'Updating TdbPath properties of %s'%archiver
+                #print('Updating TdbPath properties of %s'%archiver)
                 #[archiver_properties[archiver].__setitem__(p,[tdbpath]) for p in pathprops]
                 #if host not in mod_hosts: mod_hosts[host]={}
                 #if server not in mod_hosts[host]: mod_hosts[host][server]=[]
                 #if archiver not in mod_hosts[host][server]: mod_hosts[host][server].append(archiver)
                 #if archiver not in mod_archivers: mod_archivers.append(archiver)
             #pass #End of checking each attribute archiver
             
-        #print 'Updating properties of %d archivers ...'%(len(mod_archivers))
+        #print('Updating properties of %d archivers ...'%(len(mod_archivers)))
         #for archiver in mod_archivers:
-            ##print 'Updating properties of %s: %s'%(archiver,str(archiver_properties[archiver]))
+            ##print('Updating properties of %s: %s'%(archiver,str(archiver_properties[archiver])))
             #api.db.put_device_property(archiver,archiver_properties[archiver])
         #return mod_hosts
         pass
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/common.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,43 +34,46 @@
 import datetime
 from random import randrange
 
 import PyTangoArchiving
 from PyTangoArchiving import ARCHIVING_CLASSES,ARCHIVING_TYPES,MAX_SERVERS_FOR_CLASS,MIN_ARCHIVING_PERIOD
 from PyTangoArchiving.utils import *
 
-import fandango
+import fandango as fn
 from fandango.dicts import CaselessDict,CaselessDefaultDict
 from fandango.log import Logger
 from fandango.objects import Object
 
-from utils import PyTango,ServersDict
+from .utils import PyTango,ServersDict
     
 def int2DevState(n): return str(PyTango.DevState.values[n])    
 def int2DevType(n): return str(PyTango.ArgType.values[n])    
 
-class CommonAPI(Object,fandango.SingletonMap):
-    """ This class provides common methods for managing a Soleil-like database (for either archiving or snapshoting)
+class CommonAPI(Object,fn.SingletonMap):
+    """ 
+    This class provides common methods for managing a Soleil-like database 
+    (for either archiving or snapshoting)
     The methods starting by "get" retrieve values using ArchivingDSs
     The methods starting by "load" access directly to MySQL database
     """
     #ArchivingTypes = ARCHIVING_TYPES
     #ArchivingClasses = ARCHIVING_CLASSES
     
     MAX_SERVERS_FOR_CLASS=5
     MIN_ARCHIVING_PERIOD=10
     
-    def __init__(self,schema,host=None,user='browser',passwd='browser',classes=[],LogLevel='info',load=True,logger=None):
+    def __init__(self,schema,host=None,user='browser',passwd='browser',
+                 classes=[],LogLevel='WARNING',load=True,logger=None):
         """
         """
         self.log = logger or Logger('ArchivingAPI(%s)'%schema,format='%(levelname)-8s %(asctime)s %(name)s: %(message)s')
         self.log.setLogLevel(LogLevel)
         self.log.debug('Logger streams initialized (error,warning,info,debug)')
 
-        self.tango = fandango.get_database() #access to Tango database
+        self.tango = fn.get_database() #access to Tango database
         self.api = self #hook used by legacy packages
         self.servers = None
         self.schema = str(schema).lower()
         self.user,self.passwd = user,passwd
         
         if host is None:
             prop = self.tango.get_class_property('%sArchiver'%schema,['DbHost'])['DbHost']
@@ -82,39 +85,39 @@
             #if 'TANGO_HOST' in os.environ:
             #    self.host=os.environ['TANGO_HOST'].split(':')[0]
         else: self.host=host
         
         self.dbs={} #pointers to Archiving databases
         
         self.ArchivingClasses = classes or self.get_archiving_classes()
-        self.ArchiverClass = (k for k in self.ArchivingClasses if 'Archiver' in k).next()
-        self.ManagerClass = (k for k in self.ArchivingClasses if 'Manager' in k).next()
-        self.ExtractorClass = (k for k in self.ArchivingClasses if 'Extractor' in k).next()
-        try: self.WatcherClass = (k for k in self.ArchivingClasses if 'Watcher' in k).next()
+        self.ArchiverClass = fn.first((k for k in self.ArchivingClasses if 'Archiver' in k),'')
+        self.ManagerClass = fn.first((k for k in self.ArchivingClasses if 'Manager' in k),'')
+        self.ExtractorClass = fn.first((k for k in self.ArchivingClasses if 'Extractor' in k),'')
+        try: self.WatcherClass = fn.first((k for k in self.ArchivingClasses if 'Watcher' in k),'')
         except: self.WatcherClass = None
         
         self.loads=CaselessDefaultDict(lambda k:0) #a dict with the archiving load for each device
         self.attributes=CaselessDict() #a dict of ArchivedAttribute objects        
         self.dedicated = CaselessDefaultDict(lambda k:set()) #Dictionary for keeping the attributes reserved for each archiver
         
         if load and self.host and self.ArchivingClasses: 
           self.load_servers()
           
     ## The ArchivingAPI is an iterator through archived attributes
     def __getitem__(self,k): 
-        k = k if k.count('/')<=3 else fandango.tango.get_normal_name(k)
+        k = k if k.count('/')<=3 else fn.tango.get_normal_name(k)
         return self.attributes.__getitem__(k)
     def __contains__(self,k): 
-        k = k if k.count('/')<=3 else fandango.tango.get_normal_name(k)
+        k = k if k.count('/')<=3 else fn.tango.get_normal_name(k)
         return self.attributes.__contains__(k)
     def get(self,k): 
-        k = k if k.count('/')<=3 else fandango.tango.get_normal_name(k)
+        k = k if k.count('/')<=3 else fn.tango.get_normal_name(k)
         return self.attributes.get(k)
     def has_key(self,k): 
-        k = k if k.count('/')<=3 else fandango.tango.get_normal_name(k)
+        k = k if k.count('/')<=3 else fn.tango.get_normal_name(k)
         return self.attributes.has_key(k)
     #[setattr(self,method,lambda k,meth=method:getattr(self.attributes,meth)(k)) for method in ('__getitem__','__contains__','get','has_key')]
     def __iter__(self): return self.attributes.__iter__()
     def iteritems(self): return self.attributes.iteritems()
     def keys(self): return self.attributes.keys()
     def values(self): return self.attributes.values()
     def __len__(self): return len(self.attributes.keys())
@@ -173,20 +176,20 @@
         if not remaining: 
           self.servers.load_by_name(klass)
           remaining = self.servers.get_class_devices(klass)
         while remaining: #for i in range(len(self.extractors)):
             next = randrange(len(remaining))
             devname = remaining.pop(next)
             device = self.servers.proxies[devname]
-            print devname
+            print(devname)
             try:
                 device.ping()
                 device.set_timeout_millis(timeout)
                 break
-            except Exception,e: 
+            except Exception as e: 
                 self.log.info('%s unreachable: %s'%(devname,str(e)))
         return device
 
     def get_manager(self):
         ''' returns a DeviceProxy object '''
         d = self.get_random_device(self.ManagerClass)
         return d
@@ -231,19 +234,19 @@
 def repair_dedicated_attributes(api,attrs=None,load=True,restart=False):
     api.load_attribute_modes()
     tdedi = api.load_dedicated_archivers()
     tdediattrs = dict((a,d) for d,v in tdedi.items() for a in v)
     newconfig = dict((a,tdediattrs[a]) for a in (attrs or tdediattrs) if a in tdediattrs and a in api and api[a].archiver and tdediattrs[a]!=api[a].archiver)
     #rows = dict((a,tdb.db.Query('select ID,archiver,start_date from amt where STOP_DATE is NULL and ID=%d'%api[a].ID)) for a in newconfig.keys() if a in api)
     if restart:
-        astor = fandango.Astor('ArchivingManager/1')
+        astor = fn.Astor('ArchivingManager/1')
         astor.load_from_devs_list(list(set([api[a].archiver for a in newconfig]+newconfig.values())))
         astor.stop_servers()
     if load:
-        print 'Updating %d dedicated attributes in amt.'%len(newconfig)
+        print('Updating %d dedicated attributes in amt.'%len(newconfig))
         for a,d in newconfig.items():
             api.db.Query("update amt set archiver='%s' where ID=%d and STOP_DATE is NULL"%(d,api[a].ID))
     if restart:
         astor.start_servers()
     return newconfig
   
 def check_archived_attribute_names(device='*',attribute='*',schema='hdb'):
@@ -354,58 +357,58 @@
 
     rateDS = 5
     nDS = 20
     a=0
     for m in range(1,nDS+1):
         for n in range(1,rateDS+1):
             member = 'archiving/hdbarchiver/'+'%02d'%m+'-'+'%02d'%n
-            print 'Reporting HdbArchiver: ',member
+            print('Reporting HdbArchiver: ',member)
             dp=DeviceProxy(member)
-            #print '\tStatus is:\n\t', dp.command_inout('Status')
-            #print '\tState detailed is:\n\t', dp.command_inout('StateDetailed')
-            print '\tScalar Charge is:\n\t', dp.read_attribute('scalar_charge').value
+            #print('\tStatus is:\n\t', dp.command_inout('Status'))
+            #print('\tState detailed is:\n\t', dp.command_inout('StateDetailed'))
+            print('\tScalar Charge is:\n\t', dp.read_attribute('scalar_charge').value)
             a=a+dp.read_attribute('scalar_charge').value
     
-    print 'Total Scalar Charge is ... ',a
+    print('Total Scalar Charge is ... ',a)
 
 def KillAllServers(klass = 'HdbArchiver'):
     processes = linos.shell_command('ps uax').split('\n')
     archivers = [s for s in processes if '%s.%s'%(klass,klass) in s]
     for a in archivers:
-        print 'Killing %s' % a[1:]
+        print('Killing %s' % a[1:])
         pid = a.split()[1]
         linos.shell_command('kill -9 %s'%pid)
         
 def force_stop_attributes(schema,attr_list):
     """
     This method will stop archivers, modify tables, and restart archivers to ensure that archiving is stop.
     """
     import fandango
     api = PyTangoArchiving.ArchivingAPI(schema)
     attr_list = [a for a in attr_list if a in api and api[a].archiver]
     arch = list(set(api[a].archiver for a in attr_list))
-    astor = fandango.Astor()
+    astor = fn.Astor()
     astor.load_from_devs_list(arch)
     astor.stop_servers()
     for s in attr_list:
         query = "update amt set stop_date=now() where ID = %s and stop_date is NULL"%api[s].ID
-        print query
+        print(query)
         api.db.Query(query)
     astor.start_servers()  
     
 def restart_attributes_archivers(schema,attributes,action=False):
     import PyTangoArchiving
     api = PyTangoArchiving.api(schema)
-    devs = fandango.defaultdict(list)
+    devs = fn.defaultdict(list)
     [devs[api[a].archiver].append(a) for a in attributes]
     if not action:
       print('%d archivers to restart, call with action=True to execute it'%len(devs))
     else:
       print('Restarting %d archivers'%len(devs))
-      astor = fandango.Astor()
+      astor = fn.Astor()
       astor.load_from_devs_list(devs.keys())
       astor.stop_servers()
       time.sleep(10.)
       astor.start_servers()
     return dict((k,len(v)) for k,v in devs.items())
 
 def tdb_to_hdb(attribute,start=0,stop=fun.END_OF_TIME,modes={},delete=False):
@@ -426,20 +429,20 @@
         api.load_attribute_descriptions()
     db = hdb.get_database()
     table = db.get_table_name(db.get_attribute_ID(attribute))
     import_into_db(db,table,values,delete)    
     
     
 def get_average_read_time(api='hdb',period=10*3600*24,N=100):
-    if fandango.isString(api):
+    if fn.isString(api):
         import PyTangoArchiving
         api = PyTangoArchiving.ArchivingAPI(api)
     reader = api.get_reader()
     active = [a for a in api.get_archived_attributes() if api[a].data_type not in (1,8)]
-    target = [active[i] for i in fandango.randomize(range(len(active)))][:int(2*N)]
+    target = [active[i] for i in fn.randomize(range(len(active)))][:int(2*N)]
     stats = []
     navg,tavg,count = 0,0,0
     print('testing %s %s attributes'%(len(target),api.schema))
     for t in target:
         if count == N: 
             break
         t0 = time.time()
@@ -465,41 +468,43 @@
     backtrackers = []
     now = time.time()
     if not api: api = archiving.ArchivingAPI(schema)
     get_size = lambda a: api.db.Query('select count(*) from %s'%api[a].table)[0][0]
     schema = api.schema.lower()
     for aname in (attributes or api.keys()):
         try:
-            #print 'Checking %s'%aname
+            #print('Checking %s'%aname)
             attr = api[aname]
             if not attr.archiver: continue
             api.load_last_values(attr.name)
             if not attr.last_date: continue
             if attr.last_date<(now-3600): continue
             size = get_size(aname)
             if not size: continue
             limits = (size-nvalues,nvalues) if schema=='hdb' else (0,nvalues)
             query = 'select time from %s limit %d,%d'%(attr.table,limits[0],limits[1])
-            print "%s.db.Query('%s')"%(schema,query)
+            print("%s.db.Query('%s')"%(schema,query))
             values = api.db.Query(query)
-            #print values
+            #print(values)
             iterator = values if schema=='hdb' else list(reversed(values))
             for i,v in enumerate(iterator[1:]):
                 if fun.date2time(v[0])<fun.date2time(iterator[i][0]):
                     backtrackers.append(aname)
-                    print '%s ATTRIBUTE IS BACKTRACKING!!!:'# %s < %s'%(aname,v[0],iterator[i][0])
-                    try: print '\t%d: %s'%(i,iterator[i+2][0])
-                    except: pass
-                    print '\t%d: %s'%(i,iterator[i+1][0]) #v[0]
-                    print '\t%d: %s'%(i,iterator[i][0])
-                    if i: print '\t%d: %s'%(i,iterator[i-1][0])
-                    if i>1: print '\t%d: %s'%(i,iterator[i-2][0])
+                    print('%s ATTRIBUTE IS BACKTRACKING!!!' % aname) #: %s < %s'%(aname,v[0],iterator[i][0]))
+                    try: 
+                        print('\t%d: %s'%(i,iterator[i+2][0]))
+                    except: 
+                        pass
+                    print('\t%d: %s'%(i,iterator[i+1][0]))
+                    print('\t%d: %s'%(i,iterator[i][0]))
+                    if i: print('\t%d: %s'%(i,iterator[i-1][0]))
+                    if i>1: print('\t%d: %s'%(i,iterator[i-2][0]))
                     break
         except:
-            print 'check_backtracking(%s,%s): Failed! \n%s'%(schema,aname,traceback.format_exc())
+            print('check_backtracking(%s,%s): Failed! \n%s'%(schema,aname,traceback.format_exc()))
     return list(set(backtrackers))
 
 #########################################################################################    
     
 ###############################################################################
 
 def getSingletonAPI(*args,**kwargs):
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/dbs.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/dbs.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,61 +29,59 @@
 import MySQLdb,sys
 
 import fandango
 import fandango as fn
 from fandango.objects import Object
 from fandango.log import Logger
 import PyTangoArchiving.utils as utils
+import os.path
 
 try:
     from fandango.db import FriendlyDB
 except:
-    raise Exception,'import FriendlyDB failed, is MySQLdb module installed?'
-
+    raise Exception('import FriendlyDB failed( is MySQLdb module installed?')
 
+def get_host_databases(host,user='',password='',
+                       exclude_db='(mysql|*_schema)'): #|tdb*'):
+    user = user or utils.DEFAULT_USER
+    password = password or utils.DEFAULT_PASS
+    db = FriendlyDB(host=host,db_name='information_schema',
+                        user=user, passwd=password)
+    dbs = dict.fromkeys([d[0] for d in 
+                db.Query('select distinct TABLE_SCHEMA from TABLES')
+                if not fn.clmatch(exclude_db,d[0])])
+    for d in dbs:
+        try:
+            db = FriendlyDB(host=host,db_name=d,
+                        user=user, passwd=password)
+            s = db.getDbSize()
+            dbs[d] = s,'%6.4fG' % (s/1e9)
+        except:
+            dbs[d] = 0,'%s_not_allowed?'%user
+            
+    return dbs
+            
 
 class ArchivingDB(FriendlyDB):
     """ 
     Class for managing the direct access to the database 
-    """
-    
-    #def __init__(self,api,db_name,user='',passwd='', host=''):
-        #if not api or not database:
-            #self.log.error('ArchivingAPI and database are required arguments '
-            # 'for ArchivingDB initialization!')
-            #return
-        #self.api=api
-        #self.db_name=db_name
-        #self.host=api.host
-        #self.log=Logger('ArchivingDB(%s)'%db_name)
-        #self.setUser(user,passwd)
-        #self.__initMySQLconection()
-    #def setUser(self,user,passwd):
-        #self.user=user
-        #self.passwd=passwd
-    #def cursor(self):
-        #return self.db.cursor()
-    #def __initMySQLconnection(self):
-        #try:
-            #self.db=MySQLdb.connect(db=self.db_name,host=self.host,user=self.user,passwd=self.passwd)
-        #except Exception,e:
-            #self.log.error( 'Unable to create a MySQLdb connection to "%s"@%s.%s: %s'%(self.user,self.host,self.db_name,str(e)))
+    """    
             
     def check(self):
         return bool(self.Query('describe adt'))
     
     @staticmethod
     def get_table_name(ID):
         ID = int(ID)
         return 'att_%05d'%ID if ID<10000 else 'att_%06d'%ID
         
     def get_attribute_ID(self,name):
         #return fandango.first(self.get_attributes_IDs(name).values())
         try:
-            return self.get_attributes_IDs(name).values()[0]
+            return fn.first(self.get_attributes_IDs(name).values())
         except Exception as e:
             print(name,e)
             raise e
     
     def get_attributes_IDs(self,name=''):
         q =  "select full_name,ID from adt"+(" where full_name like '%s'"%name if name else '')
         return dict((a.lower(),v) for a,v in self.Query(q))
@@ -159,28 +157,31 @@
         else:
             result = {}
             for row in val:
                 result[row['ID']] = dict((k,row[k]) for k in ('ID','archiver','start_date','stop_date'))
                 result[row['ID']].update((k,[row[j] for j in v]) for k,v in self.AMT_COLUMNS.items() if '_mod' in k and row[k])
             return result if len(result)!=1 else result.popitem()[1]
     
-    def get_last_attribute_values(self,table,n,check_table=False):
+    def get_last_attribute_values(self,table,n,check_table=False,epoch=fn.END_OF_TIME):
         """
         Check table set to False as sometimes order of insertion is not the same as expected, BE CAREFUL WITH THIS ARGUMENT!
         """
-        query = table
+        query,where = table,''
         if check_table:
             table_size = self.getTableSize(table)
             if table_size>1e3:
                 x = max((2*n,20))
                 query = '(select * from %s limit %d,%d)'%(table,table_size-x,x)
-        if 'read_value' in self.getTableCols(table):
-            return self.Query('SELECT time,read_value from %s T order by T.time desc limit %d'%(query,n))
-        else:
-            return self.Query('SELECT time,value from %s T order by T.time desc limit %d'%(query,n))
+        epoch = fn.str2time(epoch) if fn.isString(epoch) else epoch
+        if epoch not in (None, fn.END_OF_TIME):
+            where = " where T.time < '%s' " % (fn.time2str(epoch))
+        what = 'SELECT time'
+        what += (',value',',read_value')['read_value' in self.getTableCols(table)]
+        return self.Query('%s from %s T %s order by T.time desc limit %d' % (
+            what, query, where, n))
     
     def get_attribute_values(self,table,start_date=None,stop_date=None,
                              desc=False,N=0,unixtime=True):
         """
         This method returns values between dates from a given table.
         If stop_date is not given, then anything above start_date is returned.
         desc controls the sorting of values
@@ -249,49 +250,169 @@
                         else ("varchar(255)" if atype in (ArgType.DevString,ArgType.DevBoolean,) 
                         else ("double")))
                 if awrite in (AttrWriteType.READ,AttrWriteType.WRITE):
                     query += "`value` " + stype + " default NULL "
                 else:
                     query += "`read_value` " + stype + " default NULL, "+"`write_value` " + stype + " default NULL"
                 query += ") ENGINE = MyIsam" #CRITICAL!!!
-                print 'Creating %s: %s'%(a,query)
+                print('Creating %s: %s'%(a,query))
                 self.Query(query)
                 done[a]=query
         return done.keys()
     
     def clean_attribute_modes(self,date):
         """
         Cleanup all unactive modes from DB if stop_date is older than date
         """
         try: 
             self.db.Query("DELETE FROM amt WHERE stop_date IS NOT NULL AND stop_date < '%s'"%date)
-        except Exception,e: 
-            print 'ArchivingDB(%s).clean_attribute_modes(%s) failed!: %s'%(self.db_name,date,e)
+        except Exception as e: 
+            print('ArchivingDB(%s).clean_attribute_modes(%s) failed!: %s'%(self.db_name,date,e))
             return False
         return True
     
+    def clean_old_tables(self, tables, date):
+        """
+        Cleanup all unactive modes from DB if stop_date is older than date
+        """
+    
     def get_table_updates(self,name=''):
         if name and not str(name).startswith('att_'):
             n = self.get_table_name(name if isinstance(name,int) else self.get_attribute_ID(name))
-            print '%s => %s'  % (name,n)
+            print('%s => %s'  % (name,n))
             name = n
         q = 'select table_name,update_time from information_schema.tables where table_schema like "%s"'%self.db_name
         if name: q+=" and table_name like '%s'"%name
         updates = dict((a,fandango.date2time(t) if t else 0) for a,t in self.Query(q))
         return updates
 
 
 ###############################################################################
 
 ###############################################################################
 # DB Methods
 
 SCHEMAS = ('hdb','tdb','snap')
+CONFIG_TABLES = ('adt apt att_conf att_conf_data_type att_parameter '
+            'att_error_desc ast context list snapshot').split()
 
 from fandango import time2date,str2time
+
+def mysqldump_by_date(schema, user, passwd, folder, start, stop, options = '',
+                      tables = None, compress = True, delete = True, host = ''):
+    """
+    This method creates a backup between selected dates for each table 
+    of the selected database.
+    
+    All dump files are exported to the same folder, and a compressed file
+    is created at the end.
+    
+    Deleting of temporary files created (folder/*dmp) must be done manually.
+
+    Dumps can be executed from external hosts passing "--host=HOSTNAME" option from shell:
+    
+         > python3 -m PyTangoArchiving.dbs mysqldump_by_date $DBNAME $DBUSER $DBPASS \
+              $FOLDER $DATE1 $DATE2 --host=$HOSTNAME options="$OPTIONS"
+    """
+    print('mysqldump_by_date(%s,,,folder=%s,%s,%s,compress=%s,delete=%s,tables=%s,options=%s)'
+          % (schema, folder, start, stop, compress, delete, tables, options))
+    t,e = start,stop
+    print(t,e)
+    start = start if fn.isString(start) else fn.time2str(start)
+    stop = stop if fn.isString(stop) else fn.time2str(stop)
+    
+    if isinstance(options,list):
+        options = ' '.join(options)
+    if not host and "-h " in options:
+        l = options.split()
+        host = l[l.index('-h')+1]
+    if not tables:
+        db = FriendlyDB(schema,user=user,passwd=passwd,host=host)
+        tables = db.getTables()
+
+    print('mysqldump_by_date(%s): %d tables to backup between %s and %s' 
+          % (schema,len(tables),start,stop))
+
+    if not os.path.isdir(folder):
+        print('mkdir %s' % folder)
+        os.mkdir(folder)
+        
+    t0 = fn.now()
+    filenames = []
+    
+    for t in sorted(tables):
+        currops = options
+        filename = ('%s/%s-%s-%s-%s.dmp' 
+            % (folder,schema,t,start.split()[0],stop.split()[0]))
+        cols = db.getTableCols(t)
+        col = [c for c in ('int_time','time','data_time') if c in cols] 
+        if col and col[0] == 'int_time':
+            where = " %s >= %s and %s < %s " % (
+                col[0],fn.str2time(start),col[0],fn.str2time(stop))
+        elif col:
+            where = " %s >= '%s' and %s < '%s' " % (col[0],start,col[0],stop)
+        else:
+            where = ""
+        if t in CONFIG_TABLES:
+            currops += " --add-drop-table "
+        else:
+            currops += ""
+        if host and not any(_ in currops for _ in ("-h "+host,"--host="+host)):
+            currops += " --host="+host
+            
+        mysqldump(schema,user,passwd,filename,t,where,options=currops)
+        filenames.append(filename)
+        
+    t1 = fn.now()
+        
+    ext = ('part.' if fn.str2time(stop) > fn.now() else '') + 'tgz'
+    dext = '.dmp'
+    if compress:
+        # doing it on separate files ...
+        #for f in filenames:
+            #cmd = 'tar zcvf %s.tgz %s' % (f,f)
+            #print(cmd)
+            #fn.linos.shell_command(cmd)
+        #dext+='.tgz' 
+
+        filename = ('%s/%s-%s-%s.%s' 
+            % (folder,schema,start.split()[0],stop.split()[0],ext))
+        cmd = 'tar zcvf %s %s/*%s' % (filename,folder,dext)
+        print(cmd)
+        fn.linos.shell_command(cmd)
+
+    if compress and delete:
+        cmd = 'rm -rf %s/*.dmp*' % folder
+        print(cmd)
+        fn.linos.shell_command(cmd)
+        
+    t2 = fn.now()
+    print('Backup took %d seconds' % int(t1-t0))
+    print('Compression took %d seconds' % int(t2-t1))
+        
+    return filename
+
+def mysqldump(schema,user,password,filename,tables='',where='',options=''):
+    """
+    Executes efficient mysqldump on listed tables
+
+    Dumps can be executed from external hosts passing "-h HOSTNAME" option
+    """
+    cmd = ("mysqldump --single-transaction --force --compact --no-create-db "
+            "--skip-lock-tables --complete-insert --quick %s -u %s -p%s" 
+            % (options,user,password))
+    cmd += " " + schema
+    if where:
+        cmd += ' --where=" %s"' % where
+    if tables:
+        cmd += ' --tables '+(' '.join(tables) if fn.isSequence(tables) 
+                             else str(tables).replace(',',' '))
+    cmd += ' > '+filename
+    print(cmd)
+    fn.linos.shell_command(cmd)
     
 def repair_attribute_name(attr):
     """
     Remove "weird" characters from attribute names
     """
     import re
     return re.sub('[^a-zA-Z-_\/0-9\*]','',attr)
@@ -311,19 +432,24 @@
     updates = db.Query('select table_name,update_time from information_schema.tables where table_schema like "%s"'%api.schema)
     updates = dict((a,fun.date2time(t) if t else 0) for a,t in updates)    
     return updates
 
 def get_partitions_from_query(db, q):
     eq = 'explain partitions '+q
     c = db.Query(eq,export=False)
-    i = (i for i,r in enumerate(c.description) if 'partitions' in str(r)).next()
+    i = (i for i,r in enumerate(c.description) if 'partitions' in str(r)).__next__()
     r = c.fetchone()[i]
     c.close()
     return r
 
+def delete_partition_data(db, table, partition):
+    q = 'alter table %s truncate partition %s' % (table,partition)
+    print(q)
+    db.Query(q)
+
 def decimate_db_table_by_time(db,table,att_id,tstart,tend,period=1,
         id_column="att_conf_id",time_column='data_time',min_to_delete=3,
         optimize = False):
     """
     This simplified method will remove all values in a table that are nearer than a given period
     It doesnt analyze values, it just gets the last value within the interval
     
@@ -374,16 +500,14 @@
     if optimize:# or (goods[-1] - goods[0]) > 86400*5:
         rq = 'alter table %s optimize partition %s' % (table,partitions)
         print(rq)
         db.Query(rq)
         print('Optimizing took %d seconds' % (fn.now()-t2))
         
     return s1-s0
-    
-    
 
 def decimate_db_table(db,table,host='',user='',passwd='',start=0,end=0,period=300,iteration=1000,condition='',cols=None,us=True,test=False, repeated = False):
     """ 
     This method will remove all values from a MySQL table that seem duplicated 
     in time or value.
     All values with a difference in time lower than period will be kept.
     
@@ -523,15 +647,15 @@
     table = table name
     data = [(time,value)] array
     offset = offset to apply to time values
     delete = boolean, if True the data between t0 and t-1 will be deleted from db before inserting.
     """
     #raise '@TODO:TEST THIS IN ARCHIVING02 BEFORE COMMIT'
     from fandango import time2str,date2str,date2time
-    print 'import_into_db(%s,%s,[%s],%s,%s)'%(db,table,len(data),delete,offset)
+    print('import_into_db(%s,%s,[%s],%s,%s)'%(db,table,len(data),delete,offset))
     if delete: 
         limits = data[0][0],data[-1][0]
         t = db.Query("select count(*) from %s where time between '%s' and '%s'"%(table,time2str(limits[0]),time2str(limits[1])))[0]
         print('deleting %s values from %s'%(t,table))
         db.Query("delete from %s where time between '%s' and '%s'"%(table,time2str(limits[0]),time2str(limits[1])))
     if not db.Query('SHOW INDEX from %s'%table):
         try: db.Query('create index time on  %s (time)'%table)
@@ -542,18 +666,18 @@
         #q = "INSERT INTO %s VALUES('%s',%s)"%(table,t[0],t[1])
         #db.Query(q)
     l,total = [],0
     for i,d in enumerate(data):
         l.append(d)
         if not (len(data)-(i+1))%100:
             q = "INSERT INTO `%s` VALUES %s ;"%(table,', '.join("('%s',%s)"%(fun.time2str(d[0]+offset),d[1] if 'none' not in str(d[1]).lower() else 'NULL') for d in l))
-            #print q[:160]
+            #print(q[:160])
             db.Query(q)
             total += len(l)
-            print i,len(l),total
+            print(i,len(l),total)
             l = []
     return total,len(data)
 
     #net = fandango.db.FriendlyDB('net6020a',user='...',passwd='...')
     #hdb = PyTangoArchiving.archiving.ArchivingAPI('hdb')
     #dev_table = dict((t[1].lower()[:4],t[0].lower()) for t in net.Query('select device,id from devices'))
     #def insert_data(r,offset,delete=''):
@@ -575,72 +699,72 @@
 def RepairColumnNames():
     db = MySQLdb.connect(db='hdb',user='root')
     q = db.cursor()
     
     q.execute('select ID,full_name,writable from adt')
     adt=q.fetchall()
     
-    print 'There are %d attribute_ID registered in the database'%len(adt)
+    print('There are %d attribute_ID registered in the database'%len(adt))
     done=0
     for line in adt:
         ID = line[0]
         full_name = line[1]
         writable = line[2]
-        print 'ID %05d: %s, w=%d'%(ID,full_name,writable)
+        print('ID %05d: %s, w=%d'%(ID,full_name,writable))
         q.execute('describe %s'%get_table_name(ID))
         describe=q.fetchall()
         col_name=describe[1][0]
         col_type=describe[1][1]
         if writable==int(PyTango.AttrWriteType.READ) and col_name!='value':
             query='ALTER TABLE %s CHANGE COLUMN %s value %s AFTER time'%(get_table_name(ID),col_name,col_type)
-            print 'query: ',query
+            print('query: ',query)
             q.execute(query)
             done+=1
             
-    print 'Attributes repaired: %d'%done    
+    print('Attributes repaired: %d'%done)    
                 
 ##@}
 
 def listLastTdbTime():
     db = MySQLdb.connect(db='tdb')
     q = db.cursor()
     q.execute('show tables')
     #It returns a TUPLE of TUPLES!!!, not a list!
     alltables = q.fetchall()
     
     q.execute('select ID,archiver from amt where stop_date is NULL')
     attribs = q.fetchall()
     
     attrtables = [ get_table_name(i[0]) for i in attribs ]
-    print str(len(attribs))+' attributes being archived.'
+    print(str(len(attribs))+' attributes being archived.')
     
-    print 'Searching newest/oldest timestamps on attribute tables ...'
+    print('Searching newest/oldest timestamps on attribute tables ...')
     results = []
     tmin,tmax = None,None
     
     for i,a in enumerate(attrtables):
         q.execute('select max(time),min(time) from '+a);
         #q.execute('select time from '+a+' order by time desc limit 1')
         #type returned is datetime.datetime
         row = q.fetchone()
         date,date2 = row[0],row[1]
         if tmax is None or date>tmax:
             tmax = date
         if tmin is None or date2<tmin:
             tmin = date2
         results.append((date,date2,a))
-        print '\r%05d/%05d:\tOldest:%s;\tNewest:%s'%(i,len(attrtables),str(tmin),str(tmax)),
+        print('\r%05d/%05d:\tOldest:%s;\tNewest:%s'%(i,len(attrtables),str(tmin),str(tmax)),)
         sys.stdout.flush()
         
     results.sort()
     """
-    print 'The last updated time found in database is '+str(results[0][1])+'-'+str(results[0][0])
-    print 'Difference with newest is '+str(results.pop()[0]-results[0][0])
+    print('The last updated time found in database is '+str(results[0][1])+'-'+str(results[0][0]))
+    print('Difference with newest is '+str(results.pop()[0]-results[0][0]))
     
-    print '\n'
+    print('\n')
     """
     
     
 def RemoveWrongValues(db,table,column,null_value,ranges,dates,extra_clauses='',check=False):
     ''' Sets the specified null_value for all values in columnd out of specified ranges
     Usage (for removing all temperatures above 200 degrees): 
      * RemoveWrongValues('hdb','att_00001','value',None,[0,200])
@@ -664,41 +788,41 @@
     else: query = "UPDATE %s SET %s=%s" % (table,column,null_value is None and 'NULL' or null_value)
     where = " WHERE (%s" % ("%s > %s"%(column,max_))
     where += min_ is not None and " OR %s < %s)" % (column,min_) or ")"
     where += " AND (time BETWEEN '%s' AND '%s')" % (start,stop)
     if extra_clauses:
         where = " AND (%s)" % extra_clauses
 
-    print 'the query is : ', query+where
+    print('the query is : ', query+where)
     q.execute(query+where)
     if check:
         result = q.fetchone()[0]
-        print 'result is %s; type is %s'%(result,type(result))
-        print 'Values to remove: %d'%int(result)
+        print('result is %s; type is %s'%(result,type(result)))
+        print('Values to remove: %d'%int(result))
     else:
         result = True
     db.close()
     return result
     
     
     #adt=q.fetchall()    
-    #print 'There are %d attribute_ID registered in the database'%len(adt)
+    #print('There are %d attribute_ID registered in the database'%len(adt))
     #done=0
     #for line in adt:
         #ID = line[0]
         #full_name = line[1]
         #writable = line[2]
-        #print 'ID %05d: %s, w=%d'%(ID,full_name,writable)
+        #print('ID %05d: %s, w=%d'%(ID,full_name,writable))
         #q.execute('describe att_%05d'%ID)
         #describe=q.fetchall()
         #col_name=describe[1][0]
         #col_type=describe[1][1]
         #if writable==int(PyTango.AttrWriteType.READ) and col_name!='value':
             #query='ALTER TABLE att_%05d CHANGE COLUMN %s value %s AFTER time'%(ID,col_name,col_type)
-            #print 'query: ',query
+            #print('query: ',query)
             #q.execute(query)
             #done+=1
             
     
 def rename_archived_attributes(attribs,load=False,restart=False,modes={'MODE_P':[10000]},schemas=('hdb','tdb')):
     """
     Renaming attributes in archiving 
@@ -727,15 +851,15 @@
         dedicated = dict((a,api[a].dedicated.lower()) for a in targets if api[a].dedicated)
         print('>> update dedicated')
         properties = []
         for arch in set(dedicated.values()):
             prop = map(str.lower,api.tango.get_device_property(arch,['reservedAttributes'])['reservedAttributes'])
             nprop = [attribs.get(p,p) for p in prop]
             properties.append((arch,nprop))
-        print properties
+        print(properties)
         if load: [api.tango.put_device_property(arch,{'reservedAttributes':nprop}) for arch,nprop in properties]
             
         #Store the list of modes, 
         #NOP!, instead we will try to use the new modes provided as argument.
         #modes = dict.fromkeys(modes_to_string(api[a].modes) for a in targets)
         #[modes.__setitem__(k,[attribs[a] for a in targets if modes_to_string(api[a].modes)==k]) for k in modes.keys()]
         
@@ -753,15 +877,15 @@
                 queries = []
                 for name in atts:
                     ID = targets[name]
                     name = attribs[name]
                     device,att_name = name.rsplit('/',1)
                     domain,member,family = device.split('/')
                     queries.append("update adt set full_name='%s',device='%s',domain='%s',family='%s',member='%s',att_name='%s' where ID=%d" % (name,device,domain,family,member,att_name,ID))
-                print '\n'.join(queries[:10]+['...'])
+                print('\n'.join(queries[:10]+['...']))
                 if load: [api.db.Query(query) for query in queries]
             print('>> start %s archivers '%server)
             if load: 
                 time.sleep(10)
                 astor.start_servers(server)
                 
         if load:
@@ -805,19 +929,22 @@
                 if eq: att_name = eq[0]
             #full_name = device+'/'+str(att_name) #Using real device name does not solve the problem when attributes are being re-inserted
             device = dev.upper() if upper else dev.lower()
             full_name = device+'/'+str(att_name)
             if full_name.rsplit('/',1)[0] == fname.rsplit('/',1)[0]: continue #Nothing to update
             domain,family,member = device.split('/')
             q = "update adt set domain = '%s',family = '%s',member = '%s',device = '%s',full_name = '%s', att_name = '%s' where id=%s" % (domain,family,member,device,full_name,att_name,ID)
-            print "%s: %s"%(fname,q)
+            print("%s: %s"%(fname,q))
             if update: db.Query(q) 
-        except Exception,e:
-            print '%s: %s'%(fname,e)
-            print traceback.format_exc()
+        except Exception as e:
+            print('%s: %s'%(fname,e))
+            print(traceback.format_exc())
             break
             failed += 1
     
     if update: db.Query('COMMIT')
     ok = len(allnames)-failed
-    if update: print '%d names updated' % (len(attrlist or allnames)-failed)
+    if update: print('%d names updated' % (len(attrlist or allnames)-failed))
     return ok    
+
+if __name__ == '__main__':
+    print(fn.call(locals_=locals()))
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/files.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 from PyTangoArchiving.common import modes_to_string, modes_to_dict
 
 
 ARCHIVING_CONFIGS =  os.environ.get('ARCHIVING_CONFIGS','/data/Archiving/Config')
 RESULT = {} # Last result of each test is stored for convenience
 
 def GetConfigFiles(folder=ARCHIVING_CONFIGS,mask='.*.csv'):
-    print 'In GetConfigFiles(%s,%s)' % (folder,mask)
+    print('In GetConfigFiles(%s,%s)' % (folder,mask))
     return sorted(['%s/%s'%(folder,f) for f in os.listdir(folder) if fun.matchCl(fun.toRegexp(mask),f)])
 
 def getAPI(schema,dedicated=False):
     """ 
     :param schema: hdb/tdb
     """
     api = PyTangoArchiving.ArchivingAPI(schema,load=False) #lightweight api
@@ -87,15 +87,15 @@
     """
     RESULT = {} #PyTangoArchiving.files.RESULT
     #RESULT.clear()
     
     ###########################################################################
     # Loading a list of schemas
     if fun.isRegexp(schema):
-        print '>>> %s is a regexp, Loading each matching schema separately'%schema
+        print('>>> %s is a regexp, Loading each matching schema separately'%schema)
         for s in PyTangoArchiving.ArchivingAPI.SCHEMAS:
             if not fun.matchCl(fun.toRegexp(schema),s): continue
             else: RESULT[s]=LoadArchivingConfiguration(filename,s,launch,force,stop,dedicated,check,overwrite,centralized,failed,unavailable,hosts,api,filters,exclude)
         return RESULT
 
     ###########################################################################
     # Loading a single schema
@@ -105,34 +105,34 @@
     tstart = time.time()
     
     if schema and schema.lower() not in filters.get('type','').lower(): 
         filters['type'] = filters.get('type') and '(%s|%s)'%(filters['type'],schema) or schema
     if 'stop' not in exclude.get('type','').lower(): 
         exclude['type'] = exclude.get('type') and '(%s|%s)'%(exclude['type'],'stop') or 'stop'
                 
-    print '>>> In LoadArchivingConfiguration(%s,%s,launch=%s,dedicated=%s,force=%s,overwrite=%s,filters=%s,exclude=%s)'\
-        %((filename,schema,launch,dedicated,force,overwrite,filters,exclude,))
+    print('>>> In LoadArchivingConfiguration(%s,%s,launch=%s,dedicated=%s,force=%s,overwrite=%s,filters=%s,exclude=%s)'\
+        %((filename,schema,launch,dedicated,force,overwrite,filters,exclude,)))
     
     if dedicated:
         raise Exception('Launch DedicateArchiversFromConfiguration(config,schema,hosts,centralized) first!')
         #DedicateArchiversFromConfiguration(config,schema=schema,launch=launch,filters=filters,exclude=exclude,hosts=hosts,centralized=centralized)
     
     config = ParseCSV(filename,filters=filters,exclude=exclude) # Attributes not for this schema will be pruned    
     n_all = len(config)
-    print '>>> %d attributes read from %s file'%(len(config),filename)
+    print('>>> %d attributes read from %s file'%(len(config),filename))
     api = api or getAPI(schema)
     
     if check:
-        print '>>> Pruning attributes not available ...'
+        print('>>> Pruning attributes not available ...')
         unavailable.extend([attr for attr in config if not utils.check_attribute(attr,readable=False)])#True)])
         if unavailable:
-            print '\n%d attributes are not available!!!\n' % len(unavailable)
+            print('\n%d attributes are not available!!!\n' % len(unavailable))
             if force: 
                 [config.pop(att) for att in unavailable]
-            else: raise Exception, 'Attributes not available: %s'%fun.list2str(unavailable)    
+            else: raise Exception( 'Attributes not available: %s'%fun.list2str(unavailable))    
     
     #Attributes classified by Mode config
     modes = defaultdict(list)    
     for k,v in sorted(config.items()): 
         mode = modes_to_string(api.check_modes(schema,v[schema.upper()]))
         modes[mode].append(k)
     
@@ -140,15 +140,15 @@
     archivers_to_restart = set()
     if launch or stop:
         #Archiving started in groups of 10 attributes
         for mode in sorted(modes.keys()):
             alist = modes[mode] #We will modify the list on the run
             done = []
             if not overwrite: 
-                print 'NOTE: Only those attributes not already archived will be modified in the database.'
+                print('NOTE: Only those attributes not already archived will be modified in the database.')
                 alist = [a for a in alist if a not in api or not api.attributes[a].archiver]
             else:
                 archs = set(api[a].archiver for a in alist if a in api and api[a].archiver)
                 archivers_to_restart.update(api.servers.get_device_server(d) for d in archs)
             devs = defaultdict(list)
             [devs[a.rsplit('/',1)[0]].append(a) for a in alist] #The devices will be inserted separately for each device
             for dev,attributes in sorted(devs.items()):
@@ -156,46 +156,46 @@
                 for i in range(1+int((len(attributes)-1)/10)): 
                     attrs = attributes[i*10:(i+1)*10]
                     if stop:
                         if api.stop_archiving(attrs,load=False):
                             done.extend(attrs)
                         else:
                             if force: failed.extend(attrs)
-                            else: raise Exception,'Archiving stop failed for: %s'%(attrs)
+                            else: raise Exception('Archiving stop failed for: %s'%(attrs))
                     if launch:
                         if api.start_archiving(attrs,modes_to_dict(mode),load=False,retries=1):
                             done.extend(attrs)
                         else:
                             if force: failed.extend(attrs)
-                            else: raise Exception,'Archiving start failed for: %s'%(attrs)
+                            else: raise Exception('Archiving start failed for: %s'%(attrs))
             modes[mode] = done
         api.load_all(values=False,dedicated=dedicated)
         
     ##Final Report
     if unavailable: 
-        print 'Attributes not available: %s'%fun.list2str(unavailable)
+        print('Attributes not available: %s'%fun.list2str(unavailable))
     if failed: 
-        print 'Attributes unable to start/stop archiving: %s' % fun.list2str(failed)
+        print('Attributes unable to start/stop archiving: %s' % fun.list2str(failed))
         RESULT['FAILED'] = failed
     #failed.extend(unavailable)
     if not launch: 
-        print ('THE ARCHIVING OF THE ATTRIBUTES HAS NOT BEEN PROCESSED, EXECUTE LoadArchivingConfiguration(%s,launch=True) TO DO IT'%filename)
+        print(('THE ARCHIVING OF THE ATTRIBUTES HAS NOT BEEN PROCESSED, EXECUTE LoadArchivingConfiguration(%s,launch=True) TO DO IT'%filename))
     else: 
-        print '-'*80
-        print ('%d attributes requested, %d have been introduced into archiving, %d failed, %d unavailable' %(n_all,n_all-len(unavailable)-len(failed),len(failed),len(unavailable)))
+        print('-'*80)
+        print(('%d attributes requested, %d have been introduced into archiving, %d failed, %d unavailable' %(n_all,n_all-len(unavailable)-len(failed),len(failed),len(unavailable))))
         if archivers_to_restart:
-            print '-'*80
-            print 'Restarting %d archivers that have been modified ...'%len(archivers_to_restart)
+            print('-'*80)
+            print('Restarting %d archivers that have been modified ...'%len(archivers_to_restart))
             api.servers.stop_servers(archivers_to_restart)
             time.sleep(5.)
             api.servers.start_servers(archivers_to_restart)
-            print 'DONE'
-            print '-'*80
+            print('DONE')
+            print('-'*80)
     
-    print 'LoadArchivingConfiguration finished in %f minutes.' % ((time.time()-tstart)/60.)
+    print('LoadArchivingConfiguration finished in %f minutes.' % ((time.time()-tstart)/60.))
     RESULT.update(modes)
     return None if silent else RESULT
     
 def DedicateArchiversFromConfiguration(filename, schema,launch=True,restart=False,force=False,filters=None,exclude=None,hosts=None,centralized=False,load=True):
     ''' This is the function used to load a list of attributes and hosts 
     **NOTE**: The function must be called separately for each archiving type LoadArchivingConfiguration(..,schema='hdb' or 'tdb')
     
@@ -233,83 +233,83 @@
             if schema and schema.lower() not in filters.get('type','').lower(): 
                 filters['type'] = filters.get('type') and '(%s|%s)'%(filters['type'],schema) or schema
             if 'stop' not in exclude.get('type','').lower(): 
                 exclude['type'] = exclude.get('type') and '(%s|%s)'%(exclude['type'],'stop') or 'stop'
             config = ParseCSV(filename,filters=filters,exclude=exclude) # Attributes not for this schema will be pruned        
     ###################################################################################################
         
-    print ('In DedicateArchiversFromConfiguration(%s,schema=%s,centralized=%s,filters=%s,exclude=%s)'%(filename,schema,centralized,filters,exclude))        
-    print '>>> Configuring dedicated archiving, creating new archiver servers and starting them if needed ...'
+    print(('In DedicateArchiversFromConfiguration(%s,schema=%s,centralized=%s,filters=%s,exclude=%s)'%(filename,schema,centralized,filters,exclude)))        
+    print('>>> Configuring dedicated archiving, creating new archiver servers and starting them if needed ...')
     assigned = api.load_dedicated_archivers()
     
     #Filtering already assigned or unexistent attributes
     for k,v in sorted(config.items()): 
         if any(k.lower() in atts for dev,atts in assigned.items()): continue
         dev,attr = k.lower().rsplit('/',1)
         if dev not in all_devs or fandango.check_device(dev) and attr not in map(str.lower,fandango.get_device(dev).get_attribute_list()):
             if not force:
-                print '%s attribute doesnt exist!'%k
+                print('%s attribute doesnt exist!'%k)
                 return
         else:
             hosts[v['host'].lower().split('.')[0]].append(k.lower())
         
     if not any(hosts.values()):
-        print 'Dedicated archiving not changed ...'
+        print('Dedicated archiving not changed ...')
         if not force: return
 
     if launch:
         ########################################################
         assigned = api.set_dedicated_archivers(hosts,20 if schema.lower()=='tdb' else 30,create=launch) #<----------------All the properties changes are done here!
         ########################################################
         
         # Restarting modified servers and archiving manager
         try:
             if restart:
                 manager = api.servers.get_device_server(api.get_manager().name())
                 api.servers.stop_servers(manager)
-                print 'ArchivingManager stop, restarting archivers ...'
+                print('ArchivingManager stop, restarting archivers ...')
                 all_servers = list(set([api.servers.get_device_server(archiver) for archiver,attrs in assigned.items() if attrs]))
                 
                 for host,vals in hosts.items():
                     servers = [s for s in all_servers if host.split('.')[0].lower() in s.lower()]
-                    print 'Restarting the Dedicated archiving servers in host %s: %s' % (host,servers)
+                    print('Restarting the Dedicated archiving servers in host %s: %s' % (host,servers))
                     for server in servers:
                         try:
                             if api.servers[server].ping() is not None: api.servers.stop_servers(server)
-                        except Exception,e: print 'The server may be not running: %s'%str(e)
-                        print 'waiting some seconds for stop_servers ...'
+                        except Exception as e: print('The server may be not running: %s'%str(e))
+                        print('waiting some seconds for stop_servers ...')
                         time.sleep(10.)
                     for server in servers:
                         try:
                             api.servers.start_servers(server,centralized or host,wait=30.)
-                            print 'waiting some seconds for start_servers ...'
+                            print('waiting some seconds for start_servers ...')
                             time.sleep(10.)
                             api.servers.set_server_level(server,centralized or host,4)
                             time.sleep(1.)
-                        except Exception,e:
+                        except Exception as e:
                             if not force:
                                 raise e
                             else:
-                                print 'UNABLE TO RESTART %s'%server
+                                print('UNABLE TO RESTART %s'%server)
                                 [[failed.append(a) for a in assigned.get(d,[]) if a not in failed] for d in api.servers[server].get_device_list()]
                 time.sleep(10.)
                 api.servers.start_servers(manager,wait=30.)
-                print 'waiting some seconds after ArchivingManager restart ...'
+                print('waiting some seconds after ArchivingManager restart ...')
                 time.sleep(10.)
             else:
-                print '!!! %sArchiver and ArchivingManager devices must be restarted to finish the setup !!!' % schema
-        except Exception,e:
-            print traceback.format_exc()
-            print 'Dedicated Archiving failed! ... restarting the ArchivingManager'
+                print('!!! %sArchiver and ArchivingManager devices must be restarted to finish the setup !!!' % schema)
+        except Exception as e:
+            print(traceback.format_exc())
+            print('Dedicated Archiving failed! ... restarting the ArchivingManager')
             if launch: api.servers.start_servers(manager,wait=60.)
             raise Exception('Dedicated Archiving failed!')
         if load: api.load_all(values=False,dedicated=True)
-        print 'Dedicated archiving configuration finished ...'
+        print('Dedicated archiving configuration finished ...')
     else:
-        print 'Dedicated archiving have been verified but not executed; you must repeat command with launch=True'
+        print('Dedicated archiving have been verified but not executed; you must repeat command with launch=True')
     return hosts
     
 class ModeCheckNotImplemented(Exception): 
     pass    
     
     
 REPORT_LEGEND = {
@@ -340,15 +340,15 @@
         'lost':'attributes not assigned to any archiver',
         'retried':'attributes which archiving have been restarted in the last cycle',
         'diff':'attributes which configuration differ from files', 
         'missing':'attributes never added to archiving',
         'triable':'missing attributes ready to be added',
         'polizon':'attributes from same devices that are being archived but not declared in this file.',
     """
-    print "In CheckArchivingConfiguration(%s,restart=%s)" % ((filename,schema,period,filters,exclude),restart)
+    print("In CheckArchivingConfiguration(%s,restart=%s)" % ((filename,schema,period,filters,exclude),restart))
     result,now = {},time.time()    
     tload,t0 = 0,0
     filters = fun.notNone(filters,{})
     exclude = fun.notNone(exclude,{})
     
     if schema and schema.lower() not in filters.get('type','').lower(): 
         filters['type'] = filters.get('type') and '(%s|%s)'%(filters['type'],schema) or schema
@@ -362,15 +362,15 @@
     archivers = dict.fromkeys(list(set(api[a].archiver for a in attributes if a in api and api[a].archiver)),0)
     idles = [k for k,v in api.check_archivers(archivers.keys()).items() if not v] #Getting all archivers not running properly
     
     devices = [a.rsplit('/',1)[0] for a in attributes]
     STATS = defaultdict(list)
     STATS['all'] = attributes.keys()
     #ok,unavailable,late,missing,triable,diff,retried,lost,hung,dedicated = [],[],[],[],[],[],[],[],[],[]
-    print "Checking %s attributes ..." % len(attributes)
+    print("Checking %s attributes ..." % len(attributes))
     retriable = defaultdict(list)
     valuable = []
     for att,modes in attributes.items():
         try:
             available = utils.check_attribute(att,readable=False,timeout=2*3600)#True) #I do not want to exclude piranis!!!
             attIsNone = not available or isinstance(available,PyTango.DevFailed) or getattr(available,'value',None) is None
             archived = att in api and api[att].archiver
@@ -378,32 +378,32 @@
             if not available: 
                 STATS['unavailable'].append(att) 
             elif archived:
                 valuable.append((att,modes,attIsNone))
             elif att in api: 
                 #Was archived in the past
                 STATS['lost'].append(att)
-                print '%s is LOST, no archiver assigned!'%(att)
+                print('%s is LOST, no archiver assigned!'%(att))
                 if restart:
                     #Dedicated configuration is not done here!! ... this is just for restarting temporarily unavailable attributes
                     retriable[modes_to_string(api.check_modes(api.schema,modes))].append(att)
             else:
                 #Never archived before
                 STATS['missing'].append(att)
                 if available: STATS['triable'].append(att)
-        except ModeCheckNotImplemented,e: 
+        except ModeCheckNotImplemented as e: 
                 raise e
-        except Exception,e: 
-                print 'In CheckArchivingConfiguration(...): %s check failed!: %s' % (att,e)
+        except Exception as e: 
+                print('In CheckArchivingConfiguration(...): %s check failed!: %s' % (att,e))
                 STATS['missing'].append(att)
     
     t0 = time.time()
     all_values = api.load_last_values([t[0] for t in valuable],cache=period)
     tload+=time.time()-t0
-    print '\t%2.2f seconds loading values.'%tload
+    print('\t%2.2f seconds loading values.'%tload)
     for att,modes,attIsNone in valuable:
         try:
             if api[att].dedicated: STATS['dedicated'].append(att)
             max_period = max([2*600]+[period]+[mode[0]/1000. for mode in api[att].modes.values()]) 
             vals = all_values[att] #api.load_last_values(att,cache=max_period)
             date = utils.date2time(vals[0][0]) if vals else 0
             value = vals[0][1] if vals else None
@@ -414,86 +414,86 @@
             else:
                 # Sometimes it's better to restart the archiver device, it will be done if its rate is <0
                 # It it is not, then the hung attributes will be added to retry list (see end of this method)
                 if date>=(now-5*max_period) and value is not None: #(24*3600) 
                     STATS['late'].append(att)
                 else: 
                     STATS['hung'].append(att)
-                    #print '%s is HUNG, %s not updated since %s, archiver = %s'%(att,value,time.ctime(date),api[att].archiver)
+                    #print('%s is HUNG, %s not updated since %s, archiver = %s'%(att,value,time.ctime(date),api[att].archiver))
                 archivers[api[att].archiver]-=1
                 
             if check_conf:
                 mode_to_str = lambda m: (
                     modes_to_string(api.check_modes(api.schema,
                         m if 'MODE_A' not in m and 'MODE_R' not in m else dict((k,v) for k,v in m.items() if k!='MODE_P'),
                         )))
                 m1,m2 = mode_to_str(api.check_modes(api.schema,modes)),mode_to_str(api[att].modes)
                 if m1!=m2:
-                    #print '%s.modes differ: file:"%s"!=db:"%s"' % (att,m1,m2)
+                    #print('%s.modes differ: file:"%s"!=db:"%s"' % (att,m1,m2))
                     STATS['diff'].append(att)
             if check_modes:
                 raise ModeCheckNotImplemented
-        except ModeCheckNotImplemented,e: 
+        except ModeCheckNotImplemented as e: 
                 raise e
-        except Exception,e: 
-                print 'In CheckArchivingConfiguration(...): %s check failed!: %s' % (att,e)
+        except Exception as e: 
+                print('In CheckArchivingConfiguration(...): %s check failed!: %s' % (att,e))
                 STATS['missing'].append(att)
                 
     STATS['polizon'] = [a for a in api.attributes if a.rsplit('/',1)[0] in devices and api[a].archiver and a not in attributes]
-    if STATS['polizon']: print '%d Attributes not in list but archived from same devices'%len(STATS['polizon'])
+    if STATS['polizon']: print('%d Attributes not in list but archived from same devices'%len(STATS['polizon']))
     
     summary = ', '.join(['%s:%s'%(k.upper(),len(v)) for k,v in sorted(STATS.items()) if v])
     STATS = dict((k,sorted(l)) for k,l in STATS.items())        
     STATS['rate'] = (float(len(STATS['ok'])+len(STATS.get('unavailable')))/len(STATS['all'])) if (STATS.get('ok') and STATS.get('all')) else 0.
-    print ('CheckArchivingConfiguration(%s,%s): attribute check in %2.2f seconds:'%(filename,schema,time.time()-now))+'\n\t'+summary
+    print(('CheckArchivingConfiguration(%s,%s): attribute check in %2.2f seconds:'%(filename,schema,time.time()-now))+'\n\t'+summary)
     
     if restart and (idles or STATS.get('hung',[]) or retriable):
         STATS['retried'] = []
         now = time.time()
         api.load_servers()
         api.load_attribute_modes()
         idles.extend([a for a,v in archivers.items() if v<0 and a not in idles])
         
         if idles: 
-            print '---> Restarting %d faulty archivers: %s' % (len(idles),idles)
+            print('---> Restarting %d faulty archivers: %s' % (len(idles),idles))
             servers = list(set(api.servers.get_device_server(d) for d in idles))
-            print '------> Restarting %d faulty servers: %s' % (len(servers),servers)
+            print('------> Restarting %d faulty servers: %s' % (len(servers),servers))
             api.servers.kill_servers(servers)
             time.sleep(5.)
             api.servers.start_servers(list(set(api.servers.get_device_server(d) for d in idles)))
             
-            print '%s ---> Waiting for archivers to restart ...'%time.ctime()
+            print('%s ---> Waiting for archivers to restart ...'%time.ctime())
             nn = time.time()
             while time.time()<(nn+150):
                 try: 
                     api.servers.proxies[idles[-1]].state()
                     break
                 except: pass
                 finally: time.sleep(10.)
             api.load_attribute_modes()
         
         ## hung attributes will be retried depending on their archiver rate (if rate is <0 the archiver will be restarted instead)
         for att in STATS.get('hung',[]):
             if not api[att].archiver or api[att].archiver not in idles: #Adding not-idle attributes to retriable list
                 modes = attributes[att]
                 retriable[modes_to_string(api.check_modes(api.schema,modes))].append(att)
-        print '%s ---> Restarting %d archiving modes'%(time.ctime(),len(retriable))
+        print('%s ---> Restarting %d archiving modes'%(time.ctime(),len(retriable)))
         
         for modes,attrs in retriable.items():
-            print '%s ---> Restarting %s archiving for %d attributes' % (time.ctime(),modes,len(attrs))
+            print('%s ---> Restarting %s archiving for %d attributes' % (time.ctime(),modes,len(attrs)))
             try: 
                 modes = modes_to_dict(modes)
                 targets = [a for a in attrs if not api[a].archiver or api[a].archiver not in idles]
                 if targets: 
                     if not api.start_archiving(targets,modes,load=False):
                         '--------> start_archiving(%s) failed with no exception'%targets
                     STATS['retried'].extend(targets)
-            except: print traceback.format_exc()
+            except: print(traceback.format_exc())
 
-        print '%s: %s[%s] restart finished after %s seconds'%(time.ctime(),filename,len(STATS['retried']),time.time()-now)
+        print('%s: %s[%s] restart finished after %s seconds'%(time.ctime(),filename,len(STATS['retried']),time.time()-now))
         
     return STATS
    
 def CheckConfigFilesForSchema(schema):
     import PyTangoArchiving as pta
     tables = pta.dbs.get_table_updates()
     api = pta.ArchivingAPI(schema)
@@ -532,20 +532,20 @@
     :param schema: hdb/tdb
     """
     if not api:
         api = PyTangoArchiving.ArchivingAPI(schema,load=False) #lightweight api
         api.load_attribute_descriptions()
         api.load_attribute_modes()    
     config = ParseCSV(filename,schema=api.schema)
-    print 'In StopArchivingConfiguration(%s): %d attributes found' % (filename,len(config))
+    print('In StopArchivingConfiguration(%s): %d attributes found' % (filename,len(config)))
     devices = set([c.rsplit('/',1)[0].lower() for c in config])
     for dev in devices:
         attrs = [a for a in api if a.startswith(dev) and api[a].archiver]
         if attrs: api.stop_archiving(attrs,load=False)
-        else: print 'No attributes currently archived for %s' % dev
+        else: print('No attributes currently archived for %s' % dev)
         time.sleep(3.)
     api.load_all(values=False)
     return
     
 import re
 
 def ExportToCSV(api,mask,filename):
@@ -555,25 +555,25 @@
     vcs = dict([(k,v) for k,v in api.attributes.items() if re.match(mask,k)])
     
     f = open(filename,'w')
     
     devices = defaultdict(dict)
     for a,v in vcs.items():
         try: devices[a.rsplit('/',1)[0]][a.rsplit('/',1)[-1]+';'+str(v.extractModeString(v.modes))]=v
-        except Exception,e: '%s failed: %s' % (a,str(e))
+        except Exception as e: '%s failed: %s' % (a,str(e))
     
     modes = defaultdict(dict)
     for d in devices:
         modes[str(sorted(devices[d].keys()))][d]=devices[d]
     
     values = []
     values.append(['#dserver host','domain/family/member','attribute','double/long/short/boolean/string/spectrum','periodic/absolute/relative'])
     for mode,devices in sorted(modes.items()):
-        model = sorted(devices.keys())[0]
-        default = devices[model].values()[0].modes.get('MODE_P',[300000])[0] /1000
+        model = fn.first(sorted(devices.keys()))
+        default = fn.first(devices[model].values()).modes.get('MODE_P',[300000])[0] /1000
         values.append(['',model,'@DEFAULT','','periodic',default])
         for a,v in sorted(devices[model].items()):
             for m,p in sorted(v.modes.items()):
                 if m=='MODE_P' and len(v.modes)>1:continue
                 line = ['','',v.name.rsplit('/',1)[-1],str(v.data_type)]
                 line.append({'MODE_P':'periodic','MODE_R':'relative','MODE_A':'absolute'}[m])
                 line.append(str(p[0]/1000))
@@ -623,15 +623,15 @@
 def save_data_file(var,data,filename='',folder='',format='pck',**kwargs): #format in 'pck' or 'csv'
     """
     This method will be use to export archived data to 'csv' or 'pck' formats.
     Kwargs can be used to pass arguments to Reader.export_to_text
     """
     path = folder+'/'+(filename or get_data_filename(var,data,format))
     kwargs = kwargs or {'arrsep':' '}
-    print 'Saving %d registers to %s ...'%(len(data),path)
+    print('Saving %d registers to %s ...'%(len(data),path))
     if format == 'csv':
         text = PyTangoArchiving.Reader.export_to_text({var:data},**kwargs)
         open(path,'w').write(text)
     else:
         pickle.dump(data,open(path,'w'))
     return path            
             
@@ -660,29 +660,29 @@
     filters,exclude = fun.notNone(fandango.CaselessDict(filters),{}),fun.notNone(fandango.CaselessDict(exclude),{'type':'stop'})
     if schema and schema.lower() not in filters.get('type','').lower(): 
         filters['type'] = filters.get('type') and '(%s|%s)'%(filters['type'],schema) or schema
     if filters.get('device') and not filters.get('name'): filters['name'] = filters['device']
     if 'name' not in filters and 'attribute' in filters: filters['name'] = filters['attribute']
     
     def trace(msg):
-        if log: print msg
+        if log: print(msg)
     trace('In ParseCSV(%s,%s,%s,-%s) ...'%(filename,schema,filters,exclude))
     
     config = CSVArray()
     config.trace = log
     config.load(filename,comment='#')
     assert len(config.rows)>1, 'File is empty!'
     
     headers=['Device','Host','Attribute','Type','ArchivingMode','Periode','MinRange','MaxRange']
     trace('Searching headers ...')
     head=config.get(0)
   
     def checkHeaders():
         if not all(h in ''.join(head) for h in headers):
-            print 'WRONG FILE HEADERS!'
+            print('WRONG FILE HEADERS!')
             exit()
     
     for h in head:
       if not h: 
         trace('In ParseCSV, empty headers!?: %s'%head)
         break
       else:
@@ -690,38 +690,38 @@
         config.fill(head=h)
     config.setOffset(1)
   
     trace('Getting attributes from the file ...')
     # it returns the list of device names and the lines that matches for each
     hosts=config.getAsTree(lastbranch='ArchivingMode')#config.get(head='Device',distinct=True)
     if not hosts: 
-        print 'NO HOSTS FOUND IN %s!!!' % filename
+        print('NO HOSTS FOUND IN %s!!!' % filename)
         return {}
     
     ## Parsing the params to create a Context
     #-------------------------------------------------
     defaultparams = {'@LABEL':'User_Code-0X','@AUTHOR':'Who?','@DATE':'When?','@DESCRIPTION':'What?',}#'@REASON':'Why?'} ## Reason became deprecated
     transparams = {'@LABEL':'name','@AUTHOR':'author','@DATE':'time','@DESCRIPTION':'description',}#'@REASON':'reason'} ## Reason became deprecated
     for p,v in defaultparams.items():
         if not fun.inCl(p,hosts): raise Exception('PARAMS_ERROR','%s NOT FOUND'%p) 
         elif not hosts[p]:  raise Exception('PARAMS_ERROR','%s IS EMPTY'%p) 
-        elif hosts[p].keys()[0]==v: raise Exception('PARAMS_ERROR','%s NOT INITIALIZED (%s)'%(p,v)) 
-        defaultparams[p]=hosts.pop(p).keys()[0]
-        context[p]=defaultparams[p]
+        elif fn.first(hosts[p].keys())==v: raise Exception('PARAMS_ERROR','%s NOT INITIALIZED (%s)'%(p,v)) 
+        defaultparams[p] = fn.first(hosts.pop(p).keys())
+        context[p] = defaultparams[p]
         if p=='@DATE':
             t,time_fmts = None,['%Y-%m-%d', '%Y-%m-%d %H:%M', '%y-%m-%d', '%y-%m-%d %H:%M', 
                                 '%Y/%m/%d','%Y/%m/%d %H:%M','%y/%m/%d','%y/%m/%d %H:%M',
                                 '%d-%m-%Y' ,'%d-%m-%Y %H:%M' ,'%d-%m-%y' ,'%d-%m-%y %H:%M' ,
                                 '%d/%m/%Y','%d/%m/%Y %H:%M','%d/%m/%y','%d/%m/%y %H:%M',
                                 '%m-%d-%Y' ,'%m-%d-%Y %H:%M','%m-%d-%y' ,'%m-%d-%y %H:%M',
                                 '%m/%d/%Y','%m/%d/%Y %H:%M','%m/%d/%y','%m/%d/%y %H:%M',
                                 ]
             for tf in time_fmts:
                 try:
-                    #print 'trying format %s'%str(tf)
+                    #print('trying format %s'%str(tf))
                     t = time.strftime('%Y-%m-%d',time.strptime(context[p],tf))
                     break
                 except: pass
             if t is not None: context[transparams[p]]=t
             else: raise Exception('PARAMS_ERROR','@DATE format cannot be parsed!: %s'%str(context[p]))
 
     ##Reading the archiving modes
@@ -729,28 +729,28 @@
     attrslist = {}
     archmodes={'PERIODIC':'MODE_P','ABSOLUTE':'MODE_A','RELATIVE':'MODE_R','THRESHOLD':'MODE_T','CALC':'MODE_C','EXTERNAL':'MODE_E'}
     all_devs = fandango.CaselessDict() #{}
     [all_devs.update(devs) for devs in hosts.values()] #Used for @COPY tag
     host = ''
     pops = []
     for khost,devs in sorted(hosts.items()):
-        #print 'khost,devs: %s,%s'%(khost,devs)
+        #print('khost,devs: %s,%s'%(khost,devs))
         for dev,attributes in sorted(devs.items()):
-            #print 'dev,attributes: %s,%s'%(dev,attributes)
-            #print 'reading device %s:%s'%(dev,str(attributes))
+            #print('dev,attributes: %s,%s'%(dev,attributes))
+            #print('reading device %s:%s'%(dev,str(attributes)))
             '''Doing all the checks needed before adding any attribute'''
             dev = dev.lower()
             if dev.strip() == 'device': continue
             elif '/' not in dev:
                 dev,alias = utils.translate_attribute_alias(dev).rsplit('/',1)[0],dev
                 all_devs[dev] = all_devs[alias]
             if khost.upper() == '@HOST': 
                 try: host = utils.get_device_host(dev).split('.')[0]
-                except Exception,e: 
-                    print e
+                except Exception as e: 
+                    print(e)
                     host = ''
             elif khost!=host:
                 trace('Getting devices from host %s'%khost)
                 host = khost
             if not host: 
                 trace('Unable to get host for %s!!!' % dev)
             
@@ -758,60 +758,60 @@
                     if ':' in a: 
                         dev2 = a.split(':')[1].strip()
                     else:
                         raise Exception('COPY macro must be declared in the way @COPY:a/tango/device')
                     if dev2:
                         if dev2 not in all_devs: 
                             raise Exception('AttributesNotDefinedFor:%s'%dev2)
-                        #print '%s: copying attributes from %s: %s'%(dev,dev2,all_devs[dev2])
+                        #print('%s: copying attributes from %s: %s'%(dev,dev2,all_devs[dev2]))
                         [attributes.__setitem__(k,v) for k,v in all_devs[dev2].items() if k and k not in attributes]
                         attributes.pop(a)
             
             if any('@DELETE' in a or '@STOP' in a for a in attributes): #If a @DELETE or @STOP is found as single attribute all dev. attributes are stopped
                 deletelist.append(dev)
             
             DEFAULT_MODE = {'MODE_P':[300000]} ##seconds in CSV's are converted to milliseconds
             DEFAULT_CONFIG = defaultdict(lambda:dict(DEFAULT_MODE.items()))
             # Getting attributes with @DEFAULT clause
             for a,tipus in attributes.items():
-                #print 'a,tipus:  %s,%s'%(a,tipus)
+                #print('a,tipus:  %s,%s'%(a,tipus))
                 if '@DEFAULT' not in a: continue
-                if not tipus or not tipus.values()[0]: 
-                    print 'Wrong format assigning defaults for %s device' % dev
+                if not tipus or not fn.first(tipus.values()):
+                    print('Wrong format assigning defaults for %s device' % dev)
                     continue
                 for schema,modes in tipus.items():
                     trace('schema,modes: %s,%s'%(schema,modes))
                     for mode,params in modes.items():
                         trace('mode,params:  %s,%s'%(mode,params))
                         mode =  archmodes.get(mode.upper(),mode)
                         DEFAULT_CONFIG[schema.upper()][mode] = [float(p) for p in params if p]
             if 'HDB' not in DEFAULT_CONFIG: DEFAULT_CONFIG['HDB'] = DEFAULT_CONFIG['']
             if 'TDB' not in DEFAULT_CONFIG: DEFAULT_CONFIG['TDB'] = DEFAULT_CONFIG['']
             if DEFAULT_CONFIG: trace('DEFAULT_CONFIG for %s archiving is: %s' % (dev,DEFAULT_CONFIG.items()))
         
             for attribute,modes in sorted(attributes.items()):
-                #print 'attribute,modes:  %s,%s'%(attribute,modes)
+                #print('attribute,modes:  %s,%s'%(attribute,modes))
                 if '@DEFAULT' in attribute: continue
                 attribute = attribute.lower()
                 
                 # applying filters to obtained attributes
                 if filters or exclude:
                     if ( ('name' in filters and not fun.matchCl(fun.toRegexp(filters['name']),dev+'/'+attribute)) or
                         ('name' in exclude and fun.matchCl(fun.toRegexp(exclude['name']),dev+'/'+attribute)) ):
-                        #print '%s filtered by %s'%(attribute,filters)
+                        #print('%s filtered by %s'%(attribute,filters))
                         continue
                 
                 if not modes and DEFAULT_CONFIG: #No schema or modes defined
                     trace('\treading attribute %s: using default modes %s'%(attribute,str(DEFAULT_CONFIG)))
                     #attrslist[dev+'/'+attribute]={'host':host,'type':tipus,'modes':config}
                     attrslist[dev+'/'+attribute]=dict([('host',host)]+list(DEFAULT_CONFIG.items()))
                 else:
                     attrslist[dev+'/'+attribute]={'host':host}
                     for mode,mode_params in modes.items():
-                        #print '%s,%s'%(mode,mode_params)
+                        #print('%s,%s'%(mode,mode_params))
                         tipus=mode.upper()
                         if not mode_params: #Schema defined but not modes
                             config = DEFAULT_CONFIG.get(tipus,DEFAULT_CONFIG.get('',{})).copy()
                             if config:
                                 new_config = PyTangoArchiving.ArchivingAPI.check_modes(tipus,config)
                                 if new_config!=config: 
                                     #print('Modes corrected from %s to %s'%(sorted(config.items()),sorted(new_config.items())))
@@ -819,71 +819,72 @@
                                 trace('\treading attribute %s: using %s default modes %s'%(attribute,tipus,config))
                                 attrslist[dev+'/'+attribute]={'host':host,tipus:config}
                             else:
                                 trace('\treading attribute %s: no %s default mode declared'%(attribute,tipus))
                         else: #Both schema and modes defined
                             config = DEFAULT_CONFIG.get(tipus,DEFAULT_MODE).copy()
                             #And modes is overriden by its own member
-                            #modes=modes.values()[0]
                             modes = mode_params #{'relative': ['15', '1', '1']}
                             try:
-                                firstmode,firstparam=modes.keys()[0],mode_params.values()[0][0]
-                            except Exception,e:
-                                print attribute,modes,mode,mode_params
+                                #firstmode,firstparam=modes.keys()[0],mode_params.values()[0][0]
+                                firstmode = fn.first(modes.keys())
+                                firstparam = fn.first(modem_params.values())[0]
+                            except Exception as e:
+                                print(attribute,modes,mode,mode_params)
                                 raise e
                             if any(a.startswith('@') for a in [attribute,firstmode,tipus]):
                                     if attribute=='@DEDICATED':
                                         dedicated[dev]=tipus
                                     elif any(c in ['@STOP','@DELETE'] for c in [firstmode,tipus]):
                                         deletelist.append(dev+'/'+attribute)
                             else:
                                     #Adding always a default value to the list of modes.
                                     #if 'MODE_P' not in config: config.update(DEFAULT_MODE.items())
                                     for mode,params in mode_params.items():
                                         if not mode: continue
-                                        #print '\treading mode %s:%s'%(mode,str(params))
+                                        #print('\treading mode %s:%s'%(mode,str(params)))
                                         mode=mode.upper() #MODE_P,MODE_R,MODE_A,...
                                         if mode in archmodes:
                                                 mode=archmodes[mode]
                                         elif mode not in archmodes.values():
-                                                print 'Unknown mode!: ',mode
+                                                print('Unknown mode!: ',mode)
                                                 continue
                                         params = [float(p) for p in params if p]
                                         if params: params[0] = 1000.*params[0] #Converting periods from seconds to milliseconds
                                         config[mode]=params
                                     #attrslist[dev+'/'+attribute]={'host':host,'type':tipus,'modes':config}
                                     new_config = PyTangoArchiving.ArchivingAPI.check_modes(tipus,config)
                                     if new_config!=config: 
                                         trace('Modes corrected from %s to %s'%(sorted(config.items()),sorted(new_config.items())))
                                         config = new_config
                                     attrslist[dev+'/'+attribute][tipus.upper()]=config
-                #print '\t\tattrslist[%s/%s]=%s'%(dev,attribute,attrslist[dev+'/'+attribute])
+                #print('\t\tattrslist[%s/%s]=%s'%(dev,attribute,attrslist[dev+'/'+attribute]))
                                     
     trace('applying filters (%s / %s) to obtained attributes'%(filters,exclude))
     if filters or exclude:
         def_keys = ('host',) #Keys unfilterable
         keys = attrslist.keys()
         pops = []
         for attribute in keys:
             if ( ('name' in filters and not fun.matchCl(fun.toRegexp(filters['name']),attribute)) or
                  ('name' in exclude and fun.matchCl(fun.toRegexp(exclude['name']),attribute)) ):
-                print '%s filtered by %s'%(attribute,filters)
+                print('%s filtered by %s'%(attribute,filters))
                 pops.append(attribute)
             else:
                 modes = attrslist[attribute].keys()
-                #print 'filter check: attribute,modes: %s,%s'%(attribute,modes)
+                #print('filter check: attribute,modes: %s,%s'%(attribute,modes))
                 for mode in modes:
                     if mode in def_keys: continue
                     if ( ('type' in filters and not fun.matchCl(filters['type'],mode)) or
                          (mode in filters and not fun.matchCl(filters[mode],str(modes[mode]))) ):
-                            #print '%s/%s filtered by filters %s'%(attribute,mode,filters)
+                            #print('%s/%s filtered by filters %s'%(attribute,mode,filters))
                             attrslist[attribute].pop(mode,None)
                     if ( ('type' in exclude and fun.matchCl(exclude['type'],mode)) or
                          (mode in exclude and fun.matchCl(filters[mode],str(modes[mode]))) ):
-                            #print '%s/%s excluded by filters %s'%(attribute,mode,exclude)
+                            #print('%s/%s excluded by filters %s'%(attribute,mode,exclude))
                             attrslist[attribute].pop(mode,None)
                 if not [k for k in attrslist[attribute] if k not in def_keys]:
                     trace('%s filtered by %s'%(attribute,filters))
                     pops.append(attribute)
         trace('%d attributes filtered out by %s/%s'%(len(pops),filters,exclude))
         for attribute in pops:
             attrslist.pop(attribute)
@@ -900,15 +901,15 @@
 #END OF ParseCSV
 #############################################################################################################            
 # Import/export from mambo
 
 HDBModes={'MODE_P':4,'MODE_R':5,'MODE_A':0,'MODE_D':2,'MODE_T':6}
 
 def export2csv(attrslist,filename):
-    raise Exception,'NotImplemented'
+    raise Exception('NotImplemented')
 
 def attrs2ac(attrslist,acname):
     '''Converts and attribute list in an AC (mambo xml) file
     attrslist: list of attributes/archiving_modes to be added in the file
     acname: XMLDocument where the configuration is going to be stored
     '''
     impl = minidom.getDOMImplementation()
@@ -974,15 +975,15 @@
     
     fc=newdoc.firstChild
     fc.appendChild(newdoc.createTextNode('\n'))
     for attribute,modes in attrslist.items():
         fc.appendChild(createAttributeNode(newdoc,attribute,modes))
         fc.appendChild(newdoc.createTextNode('\n'))
         
-    print newdoc.toxml()
+    print(newdoc.toxml())
     return newdoc
 
 def readArchivingConfigurationFromDB(htype='hdb'):
     ''' Using the ArchivingAPI this function reads the Status of each attribute from the amt table of the database and returns a dictionary with the actual configurations
     The structure of the dictionary is {start_date_epoch:{attrname:[archivingmodes],...},...}
     '''
     pass            
@@ -1042,22 +1043,26 @@
     sys.exit(-1)
     
 def main(args):
     #@todo: this script features can be part of ctarchiving script
     if not args: 
         exxit()
         
-    action = args[0]
+    action = args[0].lower()
     filenames = args[1:]
-    if len(args)>2:
-        schema = filenames.pop(-1)
-    else:
-        schema = raw_input('Schema?').strip() or ''
     
-    if all(map(os.path.isfile,filenames)):
+    if os.path.isfile(filenames[0]):
+        
+        if not os.path.isfile(filenames[-1]):
+            schema = filenames.pop(-1)
+        else:
+            csv = ParseCSV(filename)
+            schemas = sorted(map(str.lower,set(k for v in csv.values() 
+                    for k in v.keys() if hasattr(v,'values'))))
+            schema = raw_input('Schema (%s)?'%'/'.join(schemas)).strip() or ''        
     
         if action in ('load','check'):
             attrs = ParseCSV(filename,schema,log=False)
             if action in 'check' and schema: 
                 from PyTangoArchiving import ArchivingAPI
                 api = ArchivingAPI(schema)
                 for a in sorted(attrs):
@@ -1066,27 +1071,48 @@
                 
         if action in ('load',):
             LoadArchivingConfiguration(filename,schema,launch=True,
                                        force='force' in args)
             
     else:
         import fandango.tango as ft
-        if schema and all(map(ft.parse_tango_model,filenames)):
-            api = PyTangoArchiving.ArchivingAPI(schema)
+        models = set(a for f in filenames for a in ft.find_attributes(f))
+        models = sorted(map(str.lower,models))
+        print('Tango attributes: %s' % str(models))
+        try:
+            if 'check' in action:
+                rd = PyTangoArchiving.Reader(log='WARNING')
+                for m in models:
+                    if rd.is_attribute_archived(m):
+                        print('%s: {Schema:Last Value}' % m)
+                        vals = rd.load_last_values(m) 
+                        print('\t%s' % vals)
+                    
+            else:
+                schema = (
+                    fun.first(fun.filtersmart(filenames,
+                                                   PyTangoArchiving.Schemas)) 
+                    or raw_input('Which database (hdb/tdb/hdbvc/...)?') 
+                    or '')
+                period = fun.first(filter(fun.isNumber, filenames), None)
+                api = PyTangoArchiving.ArchivingAPI(schema)
+
+                if 'start' in action:
+                    modes = period or eval(
+                        raw_input('Archiving period in ms?')) or None
+                    api.start_archiving(models,modes)
 
-            if 'start' in action.lower():
-                modes = eval(raw_input('Archiving modes?'))
-                api.start_archiving(filenames,modes)
+                elif 'stop' in action:
+                    api.stop_archiving(filenames)
+                    
+                else: 
+                    raise Exception('unknown action %s' % action)
 
-            if 'stop' in action.lower():
-                api.stop_archiving(filenames)
-                
-            if 'check' in action.lower():
-                print(api.load_last_values(filenames))
-        else:
+        except:
             print('Unknown args: %s' % filenames)
+            import traceback
+            traceback.print_exc()
             exxit()
         
 
 if __name__ == '__main__':
-    print sys.argv
     main(sys.argv[1:])
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/reader.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,61 +22,76 @@
 #############################################################################
 
 """
 PyTangoArchiving.reader: This module provides the Reader object; 
 a lightweigth api for archiving clients and/or scripts.
 """
 
-import traceback,time,os,re
+import traceback,time,os,re,datetime
+import multiprocessing
 from random import randrange
 from collections import defaultdict
 
 import fandango
+import fandango as fn
 from fandango.objects import Object,SingletonMap,Cached
-from fandango.log import Logger
-import fandango.functional as fun
+from fandango.log import Logger, Debugged
 
 from fandango.dicts import CaselessDict, SortedDict
 from fandango.linos import check_process,get_memory
 from fandango.tango import ( get_tango_host,parse_tango_model, get_full_name,
     get_normal_name, get_free_property,get_class_property,get_device_property)
+from fandango.threads import SubprocessMethod, AsynchronousFunction
 
-from PyTangoArchiving.utils import * #PyTango, patch_booleans
+from PyTangoArchiving.utils import * #PyTango, patch_booleans, extract_array_index
 import PyTangoArchiving.utils as utils
 
 from PyTangoArchiving.dbs import ArchivingDB, get_table_name
 from PyTangoArchiving.common import DB_MODES, translate_attribute_modes
 from PyTangoArchiving.schemas import Schemas
-import MySQLdb,MySQLdb.cursors,datetime
 
 __test__ = {}
 
 STARTUP = time.time()
 def getArchivedTrendValues(*args,**kwargs):
     """ For backwards compatibility, preload TaurusTrend layer """
     try:
-        from PyTangoArchiving.widget.trend import getArchivedTrendValues
-        return getArchivedTrendValues(*args,**kwargs)
+        import PyTangoArchiving.widget.trend as pwt
+        return pwt.getArchivedTrendValues(*args,**kwargs)
     except:
         traceback.print_exc()
         return []
-
+    
 ###############################################################################
 # Helpers
+
+DECIMATION_MODES = [
+    #('Hide Nones',fn.arrays.notnone),
+    ('Period',True), # <<< DEFAULT
+    ('Pick One',fn.arrays.pickfirst), 
+    ('Minimize Noise',fn.arrays.mindiff),
+    ('Maximize Peaks',fn.arrays.maxdiff),
+    ('Average Values',fn.arrays.average),
+    ('In Client', False),
+    ('RAW',None),        
+    ]
     
 def expandEvalAttribute(attribute):
     if '{' not in attribute: return []
     else: return [a.strip('{}') for a in re.findall('[\{][^\{]*[\}]',attribute)]
                 
 def isAttributeArchived(attribute,reader=None,schema=''):
     """
     This method returns whether an attribute contains values or not in the database.
     The attribute could be no longer archived, but if there's data to retrieve 
     it will return True
     """
+    print('isAttributeArchived is DEPRECATED, '
+        'use just Reader().is_attribute_archived instead')
+    
     reader = reader or Reader(schema)
     reader.debug('In PyTangoArchiving.reader.isAttributeArchived(%s)'%attribute)
     try:
       if expandEvalAttribute(attribute):
           return all(isAttributeArchived(a) for a in expandEvalAttribute(a))
       attribute = reader.alias.get(attribute,attribute)
       attribute = attribute.lower().split('[')[0]
@@ -94,24 +109,23 @@
 
       (reader.available_attributes if value else reader.failed_attributes
             ).append(attribute)
       return value
 
     except:
       return False
-  
     
 def getArchivingReader(attr_list=None,start_date=0,stop_date=0,
                        hdb=None,tdb=None,logger=None,tango='',schema=''): 
     """
+    This method is deprecated by reader.is_attribute_archived
     It returns the most suitable reader for a list of attributes
-    
     It is done counting the fail/errors per schema
     """
-    attr_list = fun.toList(attr_list or [])
+    attr_list = fn.toList(attr_list or [])
     try:
       schemas = Schemas.SCHEMAS or Schemas.load()
     except:
       schemas = ['hdb','tdb']
       
     pref = set(Reader.get_preferred_schema(a) for a in attr_list)    
     if any(pref): #schema set by history dialog
@@ -128,14 +142,15 @@
 
     log('getArchivingReader(%s): %s'%(attr_list,schemas.keys()))
     a,failed = '',fandango.defaultdict(int)
     
     #By default, it iterates over sorted Schemas.SCHEMAS
     for name in schemas:
       try:
+        self.log.info('getSchema(%s)' % name)
         data = Schemas.getSchema(name,tango=tango,logger=log)
         if data is None: continue #Unreached schema
       
         ## Backwards compatibility
         if 'tdb' in (name,data.get('schema'),data.get('dbname')):
           if not data.get('reader'):
             data['reader'] = tdb or Reader('tdb',tango_host=tango,logger=logger)
@@ -151,34 +166,37 @@
         
         for a in attr_list:
           log('getArchivingReader(%s): trying on %s'%(a,name))
           if not Schemas.checkSchema(name,a,start_date,stop_date):
             log('getArchivingReader(%s,%s,%s): not in %s schema!'%(
               a,start_date,stop_date,name))
             failed[name]+=1
+            
           elif not data['reader'].is_attribute_archived(a):
             log('getArchivingReader(%s,%s): not archived!'%(name,a))
             failed[name]+=1
             
-      except Exception,e:
+      except Exception as e:
         log('getArchivingReader(%s,%s): failed!: %s'%(
             name,a,traceback.format_exc()))
         failed[name]+=1
           
       if not failed[name]: 
         if log: log('getArchivingReader(): Using %s'%name)
         return data['reader']
     
     #Return the best match
     failed = sorted((c,n) for n,c in failed.items())
     if failed and failed[0][0]!=len(attr_list):
         rd = data[failed[0][1]].get('reader')
         if log: 
             log('getArchivingReader(): Using %s'%failed[0][1])
+
         return rd
+
     return None
     
     ##@TODO: OLD CODE, TO BE REMOVED IN NEXT RELEASE
     #hdb,tdb = hdb or Reader('hdb',logger=logger),tdb or Reader('tdb',logger=logger)
     #attr_list = map(tdb.get_attribute_alias,attr_list if fandango.isSequence(attr_list) else [attr_list])
     #intdb,inhdb = all(map(tdb.is_attribute_archived,attr_list)),any(map(hdb.is_attribute_archived,attr_list))
     #now = time.time()
@@ -226,17 +244,16 @@
     #__singleton__ = None
     #@classmethod
     #def singleton(cls,*p,**k):
         #if not cls.__singleton__: 
             #cls.__singleton__ = cls(*p,**k)
         #return cls.__singleton__
     
-    RetentionPeriod = 3*24*3600
-    ExportPeriod = 600
-    CacheTime = 600
+    RetentionPeriod = 3*24*3600 # for TDB compatibility
+    ExportPeriod = 600 # for TDB compatibility
     DefaultSchemas = ['hdb','tdb',] #'snap',) 
                      #'*','all') @TODO: Snap should be readable by Reader
     ValidArgs = ['db','config','servers','schema','timeout',
                  'log','logger','tango_host','alias_file']
     
     Preferred = CaselessDict() #Store specific attribute/schema user preferences
     
@@ -263,30 +280,34 @@
         if 'schema' in k: key+=':'+(k['schema'] or '').replace('*','') # or (not k.get('db','') and '*'))
         if 'tango_host' in k: key+=':'+(k['tango_host'] or get_tango_host())
         if not key: 
             key = SingletonMap.parse_instance_key(cls,*p,**k)
         return key
             
     def __init__(self,db='*',config='',servers = None, schema = None,
-                 timeout=300000,log='INFO',logger=None,tango_host=None,
-                 multihost=False,alias_file=''):
+                 timeout=300000,log='WARNING',logger=None,tango_host=None,
+                 multihost=True,alias_file=''):
         '''@param config must be an string like user:passwd@host'''
         if not logger:
             self.log = Logger('%s.Reader'%schema,
                 format='%(levelname)-8s %(asctime)s %(name)s: %(message)s')
             self.log.setLogLevel(log)
         else: 
             self.log = logger
         
         self.configs = SortedDict()
         if schema is None: schema = db
         if schema is not None and db=='*': db = schema
         if any(s in ('*','all') for s in (db,schema)): db,schema = '*','*'
-        self.log.debug('In PyTangoArchiving.Reader.__init__(%s)' 
-                       % (schema or db or '...'))        
+        
+        sch = Schemas.get(schema)
+        if sch and not config: config = sch.get('config','')
+        
+        self.log.debug('In PyTangoArchiving.Reader.__init__(%s, %s)'
+                       % (schema or db or '...', config))        
         self.db_name = db
         self._last_db = ''
         self.dbs = {}
         self.alias,self.servers,self.extractors = {},{},[]
         self.schema = schema if schema is not None else (
             [s for s in self.DefaultSchemas if s in db.lower()] or ['*'])[0]
         self.tango_host = tango_host or get_tango_host()
@@ -304,36 +325,40 @@
         self.default = dprops.get(props[-1]) or dprops.get(props[0])
         
         #Initializing Database connection
         if '*' in (self.db_name,self.schema):
             self.init_universal(logger)
         else: 
             self.init_for_schema(self.schema or self.db_name,config,servers)
-            
+
         try:
             alias_file = alias_file or get_alias_file()       
             self.alias = alias_file and read_alias_file(alias_file)
-        except Exception,e: 
+        except Exception as e:
             self.log.warning('Unable to read alias file %s: %s'%(alias_file,e))
 
         #Initializing the state machine        
         self.reset() 
         
     @fandango.Catched
     def init_for_schema(self,schema,config='',servers=[]):
-        print('%s.init_for_schema(%s,%s)' % (self.schema,schema,config))
+        self.log.info('%s.init_for_schema(%s,%s)' 
+                       % (self.schema,schema,config))
 
         if not config and schema in Schemas.keys():
-                #raise 'NotImplemented!, Use generic Reader() instead'
+                #raise 'NotImplemented!( Use generic Reader() instead')
                 sch = Schemas.getSchema(schema)
-                sch = map(sch.get,('user','passwd','host','db_name'))
-                if all(sch): config = '%s:%s@%s/%s' % tuple(sch)
+                sch = list(map(sch.get,('user','passwd','host','db_name')))
+                if all(sch): 
+                    self.log.info('parsing ' + str(sch))
+                    config = '%s:%s@%s/%s' % tuple(sch)
                 
         if not config and schema in ('hdb','tdb'):
             try:
+                self.log.info('load %sextractor properties' % self.schema)
                 prop = '%sextractor'%self.schema
                 prop = self.tango.get_class_property(prop,['DbConfig'])
                 config = '\n'.join(prop['DbConfig'] or [''])
             except: 
                 pass
             if not config and self.default: 
                 config = '\n'.join(self.default)
@@ -341,44 +366,46 @@
         if config:
             self.configs.update( (0 if '<' not in c 
                 else str2epoch(c.split('<')[0]),c.split('<')[-1]) 
                 for c in config.split() )
             
         if not config and self.db_name in Schemas.keys() \
                 and self.schema not in ('hdb','tdb'):
-            raise 'NotImplemented!, Use generic Reader() instead'
+            raise 'NotImplemented!( Use generic Reader() instead)'
+        
+        self.log.info('%s configs: %s' % (schema,self.configs))
 
         ## THIS METHOD OF CHECKING HDB++ IS FLAWED!! (and unused) @TODO
         #if any(a.lower() in s for s in map(str,(self.db_name,schema,config)) 
                #for a in ('hdbpp','hdb++','hdblite')):
-        if schema.lower() not in ('*','hdb','tdb'):
+        if 'hdbpp' in str(Schemas.get(schema)).lower():
             self.is_hdbpp = True
             c = sorted(self.configs.items())[-1][-1]
             self.db_name = c.split('/')[-1] if '/' in c else schema
-            self.log.debug("Created HDB++ reader")
+            self.log.info("Created HDB++ reader")
         else:
-            self.log.debug("Created '%s' reader"%self.db_name)
+            self.log.info("Created '%s' reader"%self.db_name)
         
-        if self.schema.lower() == 'tdb': 
-            #RetentionPeriod must be updated for all generic readers
-            try:
-                prop = self.tango.get_class_property('TdbArchiver',
-                                ['RetentionPeriod'])['RetentionPeriod']
-                prop = prop[0] if prop else 'days/3'
-                Reader.RetentionPeriod = max((Reader.RetentionPeriod,
-                                eval('1./(%s)'%prop,{'days':1./(3600*24)})))
-            except Exception,e: 
-                self.log.warning('Error on RetentionPeriod: %s'%e)
+        #if self.schema.lower() == 'tdb': 
+            ##RetentionPeriod must be updated for all generic readers
+            #try:
+                #prop = self.tango.get_class_property('TdbArchiver',
+                                #['RetentionPeriod'])['RetentionPeriod']
+                #prop = prop[0] if prop else 'days/3'
+                #Reader.RetentionPeriod = max((Reader.RetentionPeriod,
+                                #eval('1./(%s)'%prop,{'days':1./(3600*24)})))
+            #except Exception,e: 
+                #self.log.warning('Error on RetentionPeriod: %s'%e)
             
         #Initializing archiver extractors proxies
         if self.get_database() is None:
             from fandango.servers import ServersDict
             self.servers = servers or ServersDict(logger=self.log)
             #self.servers.log.setLogLevel(log)
-            if self.tango_host == os.getenv('TANGO_HOST'):
+            if self.tango_host == fn.get_tango_host():
                 self.servers.load_by_name('%sextractor'%schema)
                 self.extractors = self.servers.get_class_devices(
                     ['TdbExtractor','HdbExtractor'][schema=='hdb'])
             else:
                 self.extractors = list(self.tango.get_device_exported(
                     '*%sextractor*'%self.schema))        
         
@@ -391,71 +418,92 @@
         for s in Schemas.SCHEMAS:
             #if (s in self.DefaultSchemas 
                     #and any(c.startswith(s.lower()) for c in tclasses)):
                 #self.configs[s] = Reader(s,logger=logger)
 
             #else:
             sch = Schemas.getSchema(s,logger=self.log)
-            if sch: 
+            if sch and sch.get('reader') is not None: 
                 self.configs[sch.get('schema')] = sch.get('reader')
             else:
                 self.log.warning('%s schema not loaded!' % s)
 
-        self.log.debug("... created")        
+        self.log.debug("... created")
         
         
     def __del__(self):
-        for k in self.dbs.keys()[:]:
-            o = self.dbs.pop(k)
-            del o
+        if getattr(self,'dbs',None):
+            for k in list(self.dbs.keys()):
+                o = self.dbs.pop(k)
+                del o
         
     def reset(self):
         self.log.debug('Reader.reset()')
         self.last_dates = defaultdict(lambda:(1e10,0))
         if hasattr(self,'state'):
             [db.renewMySQLconnection() for db in self.dbs.values()]
         self.last_retry = 0
         self.available_attributes = []
         self.current_attributes = []
         self.failed_attributes = []
         self.attr_schemas = fandango.defaultdict(list)
-        self.cache.clear()
+        self.clear_cache()
         if self.extractors or self.dbs or self.configs:
             self.state = PyTango.DevState.INIT
         else:
             self.state = PyTango.DevState.FAULT
             self.log.info('No available extractors found, '
                 'PyTangoArchiving.Reader disabled')
                 
     def get_database(self,epoch=-1):
+        """
+        This method should provide the current connection object to DB
+        """
+        self.log.info('%s.get_database(%s)' % (self.schema,epoch))
         try:
-            if epoch<0: epoch = time.time()
-            config = sorted((e,c) for e,c in self.configs.items() if e<=epoch)[-1][-1]
-        except Exception,e:
-            #traceback.print_exc()
-            self.log.warning('Unable to get DB(%s,%s) config at %s, using Java Extractors.\n%s'%(self.db_name,self.schema,epoch,e))
+            if epoch<-1: 
+                epoch = time.time()-epoch
+            elif epoch==-1 or epoch is None:
+                epoch = time.time()
+            
+            config = sorted((e,c) for e,c in self.configs.items() 
+                            if e<=epoch)
+            config = (config if len(config) 
+                    else sorted(self.configs.items()))[-1]
+            if fn.isSequence(config):
+                config = config[-1]            
+            #self.log.info('config: %s' % str(config))
+        except Exception as e:
+            #[fn.printf(t) for t in self.configs.items()]
+            traceback.print_exc()
+            self.log.warning('Unable to get DB(%s,%s) config at %s'
+                             %(self.db_name,self.schema,epoch))
             return None
-        #print('get_database(%s)' % self.schema)
         try:
             user,host = '@' in config and config.split('@',1)\
                 or (config,os.getenv('HOSTNAME'))
             user,passwd = ':' in user and user.split(':',1) or (user,'')
             host,db_name = host.split('/') if '/' in host \
                 else (host,self.db_name)
-            #(self.log.info if len(self.configs)>1 else self.log.debug)('Accessing MySQL using config = %s:...@%s/%s' % (user,host,db_name))
+            #(self.log.info if len(self.configs)>1 else self.log.debug)(
+            # 'Accessing MySQL using config = %s:...@%s/%s' 
+            # % (user,host,db_name))
         except:
             self.log.warning('Wrong format of DB config: %s.\n%s'%(config,traceback.format_exc()))
             return None
         try:
             if (host,db_name) not in self.dbs:
                 if self.is_hdbpp:
                     from PyTangoArchiving.hdbpp import HDBpp
                     self.dbs[(host,db_name)] = HDBpp(db_name,host,user,passwd)
                 else: 
-                    self.dbs[(host,db_name)] = ArchivingDB(db_name,host,user,passwd,loglevel=self.log.getLogLevel(),default_cursor=MySQLdb.cursors.SSCursor)
+                    import MySQLdb.cursors
+                    self.dbs[(host,db_name)] = ArchivingDB(db_name,host,user,
+                        passwd,loglevel=self.log.getLogLevel(),
+                        default_cursor=MySQLdb.cursors.SSCursor)
                 
             if '%s@%s'%(db_name,host) != self._last_db:
                 self._last_db = '%s@%s'%(db_name,host)
                 self.log.debug('In get_database(%s): %s'%(epoch,self._last_db))
             return self.dbs[(host,db_name)]
         except:
             self.log.warning('Unable to access MySQL using config = %s:...@%s/%s\n%s' % (user,host,db_name,traceback.format_exc()))
@@ -485,119 +533,108 @@
                 self.state = states[False]
         
         return (self.state!=PyTango.DevState.FAULT)
         
     #################################################################################################
     #################################################################################################
                 
-    def get_extractor(self,check=True,attribute=''):
-        """ Gets a random extractor device."""
-        #Try Unified Reader
-        if self.db_name=='*':
-            return self.configs[('tdb' if self.configs['tdb'].is_attribute_archived(attribute) else 'hdb')].get_extractor(check,attribute)
-        
-        extractor = None
-        if (check and not self.check_state()) or not self.extractors:
-            self.log.warning('get_extractor(): Archiving seems not available')
-            return None
-        
-        # First tries to get the previously used extractor, if it 
-        # is not available then searches for a new one ....
-        if attribute and attribute in self.attr_extracted:
-            extractor = self.servers.proxies[self.attr_extracted[attribute]]
-            try:
-                extractor.ping()
-                extractor.set_timeout_millis(self.timeout)
-            except Exception,e: extractor = None
-            
-        if not extractor:
-            remaining = self.extractors[:]
-            while remaining: #for i in range(len(self.extractors)):
-                next = randrange(len(remaining))
-                devname = remaining.pop(next)
-                if ':' not in devname: devname = self.tango_host +'/' +devname
-                extractor = self.servers.proxies[devname]
-                try:
-                    extractor.ping()
-                    extractor.set_timeout_millis(self.timeout)
-                    break
-                except Exception,e: 
-                    self.log.debug(traceback.format_exc())
+    #def get_extractor(self,check=True,attribute=''):
+        #""" Gets a random extractor device."""
+        ##Try Unified Reader
+        #if self.db_name=='*':
+            #return self.configs[
+                #('tdb' if self.configs['tdb'].is_attribute_archived(attribute) 
+                 #else 'hdb')].get_extractor(check,attribute)
+        
+        #extractor = None
+        #if (check and not self.check_state()) or not self.extractors:
+            #self.log.warning('get_extractor(): Archiving seems not available')
+            #return None
+        
+        ## First tries to get the previously used extractor, if it 
+        ## is not available then searches for a new one ....
+        #if attribute and attribute in self.attr_extracted:
+            #extractor = self.servers.proxies[self.attr_extracted[attribute]]
+            #try:
+                #extractor.ping()
+                #extractor.set_timeout_millis(self.timeout)
+            #except Exception,e: extractor = None
+            
+        #if not extractor:
+            #remaining = self.extractors[:]
+            #while remaining: #for i in range(len(self.extractors)):
+                #next = randrange(len(remaining))
+                #devname = remaining.pop(next)
+                #if ':' not in devname: devname = self.tango_host +'/' +devname
+                #extractor = self.servers.proxies[devname]
+                #try:
+                    #extractor.ping()
+                    #extractor.set_timeout_millis(self.timeout)
+                    #break
+                #except Exception,e: 
+                    #self.log.debug(traceback.format_exc())
                     
-        self.state = PyTango.DevState.ON if extractor else PyTango.DevState.FAULT
-        return extractor    
+        #self.state = PyTango.DevState.ON if extractor else PyTango.DevState.FAULT
+        #return extractor    
         
-    @Cached(depth=10,expire=15.)
-    def get_attributes(self,active=False):
-        """ Queries the database for the current list of archived attributes."""
-        self.log.debug('get_attributes(%s)'%active)
+    @Cached(depth=20,expire=60.,log=False)
+    def get_attributes(self,active=False,regexp=''):
+        """ 
+        Queries the database for the current list of archived attributes.
+        arguments:
+            active: True/False: attributes currently archived
+            regexp: '' :filter for attributes to retrieve
+        """
         t0 = now()
-
-        if self.available_attributes and self.current_attributes \
-                and time.time()<(self.updated+self.CacheTime):
-            return (self.available_attributes,self.current_attributes)[active]
-
-        self.log.debug('%s: In Reader(%s).get_attributes(): '
-            'last update was at %s'%(time.ctime(),self.schema,self.updated))
+        self.log.debug('%s In Reader(%s).get_attributes(%s,%s): last update was at %s'
+            %(self,self.schema,active,regexp,self.updated))
         self.log.debug('multihost = %s' % self.multihost)
         
         get_model = self.get_attribute_model
         get_models = lambda l: sorted(set(map(get_model,l)))
         
-        self.available_attributes, self.current_attributes = [],[]
+        self.available_attributes = []
+        self.current_attributes = []
         
         #Try Unified Reader
         if self.db_name=='*':    
             for c,x in self.configs.items():
-                self.log.debug('Getting %s attributes' % c)
-                for act in (True,False):
+                self.log.info('Getting %s attributes' % c)
+                for act in set((True,False)):
                     try:
+                        if act and not Schemas.checkSchema(c):
+                            continue
                         attrs = x.get_attributes(active=act)
-                        self.log.debug('%d' % len(attrs))
-                        self.log.debug('parse models')
-                        attrs = map(self.get_attribute_model,attrs)
-                        self.log.debug('%d' % len(attrs))
-                        self.log.debug('union')
+                        attrs = list(map(self.get_attribute_model,attrs))
                         if act:
                             self.current_attributes.extend(attrs)
-                            self.log.debug('%d' % len(self.current_attributes))
                         else:
                             self.available_attributes.extend(attrs)
-                            self.log.debug('%d' % len(self.available_attributes))
-                            self.log.debug('update schemas')
                             [self.attr_schemas[a].append(c) for a in attrs
                              if c not in self.attr_schemas[a]]
                     except:
                         self.log.warning('Unable to get %s attributes:\n %s' 
                             % (c, traceback.format_exc()))
                         
                 self.log.debug('%d' % len(self.available_attributes))
-                self.log.debug(self.available_attributes and self.available_attributes[0])
-                self.log.debug(self.available_attributes and self.available_attributes[-1])
                 
-            self.log.debug('sorting')
             self.available_attributes = sorted(set(self.available_attributes))
-            self.current_attributes = sorted(set(self.current_attributes))                
+            self.current_attributes = sorted(set(self.current_attributes))
+            n0 = len(self.current_attributes)
+            dups = n0 - len(self.current_attributes) 
+            if dups:
+                self.log.info('%d attributes actively archived by multiple DBs' % dups)            
         else:
-            if self.get_database(): #Using a database Query
-                t1 = now()
-                self.log.debug('query')
-                avs = self.get_database().get_attribute_names(active=False)
-                currs = self.get_database().get_attribute_names(active=True)
-                self.log.debug('models')
-                self.available_attributes = map(get_model,avs)
-                self.current_attributes = map(get_model,currs)
-
-            elif self.extractors: #Using extractors
-                attrs = self.__extractorCommand(self.get_extractor(), 
-                                            'GetCurrentArchivedAtt')
-                self.current_attributes = map(get_model,attrs)
-                self.available_attributes = self.current_attributes
-                
-            self.log.debug('schemas')
+            t1 = now()
+            self.log.info('Getting %s attributes' % self.db_name)
+            avs = self.get_database().get_attribute_names(active=False)
+            currs = self.get_database().get_attribute_names(active=True)
+            self.available_attributes.extend(map(get_model,avs))
+            self.current_attributes.extend(map(get_model,currs))
+            
             for a in self.available_attributes:
                 self.attr_schemas[a] = [self.schema]
 
         #This match is already done by isAttributeArchived and it interferres
         #with get_attribute_alias()
         #self.log.debug('Updating %d aliases' % len(self.alias))
         #for a,m in self.alias.items():
@@ -605,58 +642,65 @@
             #if m in self.current_attributes:
                 #self.current_attributes.append(get_model(a))
             #if m in self.available_attributes:
                 #self.available_attributes.append(get_model(a))
                 #self.attr_schemas[a] = [s for s in Schemas.SCHEMAS if a in
                     #(self.attr_schemas[a]+self.attr_schemas[m])]
             
-        self.log.debug('sorting')
         self.available_attributes = sorted(set(self.available_attributes))
         self.current_attributes = sorted(set(self.current_attributes))
         self.updated = now()
-        self.log.debug('In Reader(%s).get_attributes(): '
+        self.log.debug('Out of Reader(%s).get_attributes(): '
             '%s attributes available in the database (+%ds)'
             % (self.schema,len(self.available_attributes),self.updated-t0))
         
-        return (self.available_attributes,self.current_attributes)[active]
+        r = (self.available_attributes,self.current_attributes)[active]
+        #self.log.debug('get_attributes(%s,%s)' % (len(r), regexp))
+        return sorted(fn.filtersmart(r,regexp) if regexp else r)
     
     #@Cached(depth=10000,expire=86400)
     def get_attribute_model(self,attribute):
         """
         Returns normal/full name depending on multihost mode
         """
-        #return (get_normal_name,get_full_name)[self.multihost](attribute)
+        ##return fn.tango.get_fqdn_name(attribute)        
+        ##return (get_normal_name,get_full_name)[self.multihost](attribute)
+        
         attribute = attribute.lower()
         if not self.multihost and attribute.count('/')>=3:
             return '/'.join(attribute.split('/')[-4:])
         if self.multihost and attribute.count(':')==2:
             return attribute
-        #self.log.debug('parsing(%s)' % attribute)
+        
         m = parse_tango_model(attribute)
-        return (m.simplename,m.fullname)[self.multihost]
+        r = (m.simplename,m.fullname)[self.multihost]
+        #self.log.debug('get_attribute_model(%s,multihost=%s): %s' 
+                       #% (attribute,self.multihost,r))
+        return r
 
     @Cached(depth=10000,expire=60.)        
     def get_attribute_alias(self,model):
         #Check if attribute has an alias
         try:
             attribute = str(model)
             attribute = (expandEvalAttribute(attribute) or [attribute])[0]
-            self.get_attributes()
+            self.get_attributes(False,'')
             attribute = attribute.lower()
             if attribute in self.current_attributes:
+                # if archived, alias is never returned!
                 return attribute
-            elif attribute in self.alias:
+            if attribute in self.alias:
                 attribute = self.alias.get(attribute)
             elif attribute:
                 attribute = utils.translate_attribute_alias(attribute)
                 if attribute != str(model):
                     attribute,alias = \
                         self.get_attribute_alias(attribute),attribute
 
-        except Exception,e:
+        except Exception as e:
              print('Unable to find alias for %s: %s'%(model,str(e)[:40]))
         return attribute
                 
     @Cached(depth=10000,expire=60.)
     def get_attribute_modes(self,attribute,force=False):
         """ Returns mode configuration, accepts wildcards """
         attribute = self.get_attribute_alias(attribute)
@@ -666,70 +710,90 @@
                 self.modes[attribute] = dict((translate_attribute_modes(k),v) 
                     for k,v in 
                         self.get_database().get_attribute_modes(
                             attribute,asDict=True).items()
                         if k in DB_MODES or k.lower() in ('archiver','id'))
             else:
                 self.modes[attribute] = {}
-                schemas = self.is_attribute_archived(attribute)
+                schemas = self.is_attribute_archived(attribute,active=True)
                 for s in schemas:
                     c = self.configs[s]
                     try:
                         m = c.get_attribute_modes(attribute,force)
                     except:
                         m = {}
                     self.modes[attribute][s] = m
                     
         return self.modes[attribute]
     
     @Cached(depth=10000,expire=60.)
-    def is_attribute_archived(self,attribute,active=False,preferent=True):
+    #@fn.log.Debugged
+    def is_attribute_archived(self,attribute,active=False,preferent=True,
+        start = None, stop = None):
         """ 
+        is_attribute_archived(attribute, active=False, preferent=True, 
+            start = None, stop = None)
         This method uses two list caches to avoid redundant device 
         proxy calls, launch .reset() to clean those lists. 
         """
 
-        if self.is_hdbpp: # NEVER CALLED IF setting reader=HDBpp(...)
-            self.log.warning('HDBpp.is_attribute_archived() OVERRIDE!!')
-            return True
+        #if self.is_hdbpp: # NEVER CALLED IF setting reader=HDBpp(...)
+            #self.log.warning('HDBpp.is_attribute_archived() OVERRIDE!!')
+            #return True
         
         if expandEvalAttribute(attribute):
             return all(self.is_attribute_archived(a,active) 
                        for a in expandEvalAttribute(attribute))
-
-        self.get_attributes() #Updated cached lists
+        
+        if fn.isSequence(attribute):
+            return dict((a,self.is_attribute_archived(a,active,preferent,start,
+                stop)) for a in attribute)
+
+        self.log.debug('is_attribute_archived(%s)' 
+                       % str((attribute,active,preferent,start,stop)))
+        self.get_attributes(False,'') #Updated cached lists
         attr = self.get_attribute_alias(attribute)
-        attr = self.get_attribute_model(attribute)
+        attr = self.get_attribute_model(attr)
+        if attr!=attribute:
+            self.log.info('%s => %s' % (attribute, attr))
         
         if self.db_name=='*':
             # Universal reader
+            if active:
+                start,stop = start or fn.now()-86400,stop or fn.now()
             pref = self.get_preferred_schema(attr)
             if preferent and pref not in (None,'*'): 
+                self.log.debug('preferred schema for %s: %s' % ())
                 return [pref]
-            elif len(self.attr_schemas[attr]):
-                return self.attr_schemas[attr]
+            elif not any((active, start, stop)) \
+                    and len(self.attr_schemas[attr]):
+                return self.attr_schemas[attr]       
             else:
                 sch = []
                 for a,c in self.configs.items():
                     if a == self.db_name: continue
                     try:
-                        if (c and (a not in Schemas.keys() or
-                                Schemas.checkSchema(a,attr)) 
-                            and c.is_attribute_archived(attr,active)):
-                            sch.append(a)
+                        check = Schemas.checkSchema(a, attr, start=start, stop=stop)
+                        self.log.debug('%s.checkSchema(%s): %s' % (c,(bool(c),a,attr,start,stop),check))
+                        if (c and (a not in Schemas.keys() or check)):
+                            check = c.is_attribute_archived(attr,active)
+                            self.log.debug('%s.is_attribute_archived(%s,%s): %s'
+                                           % (c,attr,active,check))
+                            if check:
+                                sch.append(a)
                     except: 
                         self.log.warning('%s archiving not available'%a)
                         self.log.warning(traceback.format_exc())
                         
                 return tuple(sch) 
                 #return tuple(a for a in self.configs if self.configs.get(a) \
                 #and (a not in Schemas.keys() or Schemas.checkSchema(a,attribute))
                 #and self.configs[a].is_attribute_archived(attribute,active))
         else:
-            # Schema reader
+            # Schema reader, alias takes precedence
             # first remove array indexes
             if (attr in (self.current_attributes if active 
                     else self.available_attributes)):
                 return attr
             
             else: #Reloading attribute lists
                 alias = self.get_attribute_alias(attr)
@@ -740,37 +804,62 @@
                 cache = (self.current_attributes if active 
                     else self.available_attributes)
                 if self.get_attribute_model(alias) in cache:
                     return True
                 
         return False
                 
-    def load_last_values(self,attribute,schema=None,epoch=None):
-        """ Returns the last values stored for each schema """
+    def load_last_values(self,attribute,schema=None,n=1,epoch=None,
+                         active=False, brief=False):
+        """
+        Returns the last values stored for each schema
+        
+        active = True will search on schemas currently running only        
+        brief = True will return only the most updated
+
+        schemas: may be None (check all), a maximum number or a list
+        epoch: max date to search
+        n: number of values to return
+        """
         result = dict()
+        if not schema and self.db_name != '*':
+            schema = self.db_name
+            
         if fandango.isSequence(attribute):
-            for attr in attribute:
-                result[attr] = self.load_last_values(attr,schema,epoch)
+            result.update((a,self.load_last_values(a, n=n, active=active or brief, 
+                schema = schema, epoch = epoch, brief=brief)) for a in attribute)
             return result
-        elif schema is None:
-            schemas = self.is_attribute_archived(attribute)
+        elif schema is None or fn.isNumber(schema):
+            schemas = self.is_attribute_archived(attribute, active=active or brief)
+            if fn.isNumber(schema):
+                schemas = schemas[:schema]    
         else:
-            schemas = fandango.toList(schema)
+            schemas = [s for s in fandango.toList(schema)
+                if Schemas.getApi(s).is_attribute_archived(
+                    attribute, active=active or brief)]
+            
+        self.log.debug('load_last_values(%s,%s)' % (attribute,schemas))
+        
         for s in schemas:
             api = Schemas.getApi(s)
-            vs = api.load_last_values(attribute)
+            self.log.debug('Reader(%s).load_last_values(%s,%s,%s)' % (s,attribute,n,epoch))
+            vs = api.load_last_values(attribute, n=n, epoch=epoch)
             vs = vs.values() if hasattr(vs,'values') else vs
-            r = vs and vs[0]
+            r = vs and fn.first(vs)
             if r and isinstance(r[0],datetime.datetime):
-                r = [fun.date2time(r[0]),r[1],(r[2:3] or [None])[0],
-                     fun.date2str(r[0])]
+                r = [fn.date2time(r[0]),r[1],(r[2:3] or [None])[0],
+                     fn.date2str(r[0])]
             result[s] = r
+            
+        if brief and result:
+            result = sorted(list(t[0:3])+[s] for s,t in result.items() if t)
+            result = result and result[-1]
+
         return result
         
-        
     def get_last_attribute_dates(self,attribute):
         """ 
         This method returns the last cached start/stop dates 
         returned for an attribute.
         """
         if expandEvalAttribute(attribute):
             return sorted(self.get_last_attribute_dates(a) 
@@ -780,42 +869,61 @@
                           for s in ('tdb','hdb'))[-1]
         else:
             return self.last_dates[attribute]
           
     @staticmethod
     def get_time_interval(start_date,stop_date):
         """
-        This method will take any valid input time format and will return four values:
+        This method will take any valid input time format and 
+        will return four values:
+        
         start_date,start_time,stop_date,stop_time
         """
-        start_time = start_date if isinstance(start_date,(int,float)) \
+        start_time = start_date if isinstance(start_date,(long,int,float)) \
                             else (start_date and str2epoch(start_date) or 0)
-        stop_time = stop_date if isinstance(stop_date,(int,float)) \
+        stop_time = stop_date if isinstance(stop_date,(long,int,float)) \
                                 else (stop_date and str2epoch(stop_date) or 0)
         if not start_time or 0<=start_time<START_OF_TIME:
             raise Exception('StartDateTooOld(%s)'%start_date)
         elif start_time<0: 
             start_time = time.time()+start_time
         if not stop_time: #Query optimized to get the latest values
             stop_time,GET_LAST = time.time(),True
         else:
-            if stop_time<0: stop_time = time.time()+stop_time
+            if stop_time<0: 
+                stop_time = time.time()+stop_time
             GET_LAST = False
 
         start_date,stop_date = epoch2str(start_time),epoch2str(stop_time)
         if not start_time<stop_time: 
             raise Exception('StartDateMustBeLowerThanStopDate(%s,%s)'
                             %(start_date,stop_date))
         
         return start_date,start_time,stop_date,stop_time
-        
+    
+    def get_attribute_frequency(self,attribute,start=None,stop=None,schemas=None,n=10):
+        """ 
+        gets n values and computes frequency 
+        """
+        if start and stop:
+            vals = self.get_attribute_values(attribute,start,stop)
+        else:
+            vals = self.load_last_values(attribute,schema=schemas,active=True,n=n)
+            if len(vals):
+                vals = sorted((len(v),k,v) for k,v in vals.items())[-1][-1]
+                
+        if len(vals)>2:
+            return abs(float(len(vals))/(vals[-1][0]-vals[0][0]))
+        else:
+            return 0
         
     def get_attribute_values(self,attribute,start_date,stop_date=None,
             asHistoryBuffer=False,decimate=False,notNone=False,N=0,
-            cache=True,fallback=True):
+            cache=True,fallback=True,schemas=None, subprocess=True,
+            lasts=False, timeout=3600):
         '''         
         This method reads values for an attribute between specified dates.
         This method may use MySQL queries or an H/TdbExtractor DeviceServer to 
         get the values from the database.
         The format of values returned is [(epoch,value),]
         The flag 'asHistoryBuffer' forces to return the rawHistBuffer 
         returned by the DS.
@@ -823,24 +931,29 @@
         :param attributes: list of attributes
         :param start_date: timestamp of the first value
         :param stop_date: timestamp of the last value
         :param asHistoryBuffer: return a history buffer object instead 
                 of a list (for trends)
         :param N: if N>0, only the last N values will be returned
                   if N<0, values will be extracted from the end of the query
-        :param decimate: remove repeated values, False by default but True 
-                when called from trends
+        :param decimate: False by default, when True it remove repeated values,
+                when having a value it keeps 1 value every N seconds
         
         :return: a list with values (History or tuple values depending of args)
         '''
+        self.log.debug('get_attribute_values(%s, %s, %s, %s, %s, %s, %s, %s, %s, %s)'
+            % (attribute, start_date, stop_date, asHistoryBuffer, decimate, 
+               notNone, N, cache, fallback, schemas))
+            
         if not self.check_state(): 
             self.log.info('In PyTangoArchiving.Reader.get_attribute_values:'
                 ' Archiving not available!')
             return []
 
+        attribute = str(attribute)
         start_date,start_time,stop_date,stop_time = \
             self.get_time_interval(start_date,stop_date)
           
         GET_LAST = 0 < (time.time()-stop_time) < 3
         
         l1,l2 = start_time,stop_time
         self.last_dates[attribute] = l1,l2
@@ -860,31 +973,32 @@
         
         cache = self.cache if cache else {}
         if cache:
             self.log.debug('Checking Keys in Cache: %s'%self.cache.keys())
                 
             margin = max((60.,.01*abs(l2-l1)))
             nearest = [(a,s1,s2,h,d) for a,s1,s2,h,d in self.cache 
-                if a==attr and h==asHistoryBuffer and d==bool(decimate) 
+                if a==attr and h==asHistoryBuffer and d==str(decimate or '') 
                 and (s1-margin<=l1 and l2<=s2+margin)]
             if nearest: 
                 attr,l1,l2,asHistoryBuffer,decimate = nearest[0]
                 
-            ckey = (attr,l1,l2,asHistoryBuffer,bool(decimate))
+            ckey = (attr,l1,l2,asHistoryBuffer,str(decimate or ''))
             values = cache.get(ckey,False)
             
             #any(len(v)>1e7 for v in self.cache.values()) or 
             if get_memory()>1e9:
                 self.log.warning('... Reader.cache clear()')
                 self.cache.clear()
             
             if values:
                 self.log.info('Reusing Cached values for (%s)' % (str(ckey)))
-                if array_index: #Array index is an string or None
-                    values = self.extract_array_index(
+                #Array index is an string or None
+                if array_index: 
+                    values = extract_array_index(
                                 values,array_index,decimate,asHistoryBuffer)                
                 return values     
         
         ######################################################################    
         # Evaluating Taurus Formulas : 
         #   it overrides the whole get_attribute process
         
@@ -900,145 +1014,271 @@
             vals = dict((k,fandango.arrays.filter_array(v,window=resolution)) 
                             for k,v in self.get_attributes_values(
                                 attributes,start_date,stop_date).items())
             cvals = self.correlate_values(vals,resolution=resolution,
                                 rule=choose_last_value)#(lambda t1,t2,tt:t2))
 
             values,error = [],False
-            for i,t in enumerate(cvals.values()[0]):
+            for i,t in enumerate(fn.first(cvals.values())):
                 v = None
                 try:
                     pars = dict((getId(k),v[i][1]) for k,v in cvals.items())
                     if None not in pars.values(): v = eval(attribute,pars)
                 except:
                     if not error: traceback.print_exc()
                     error = True
                 values.append((t[0],v))
             
         #######################################################################
         # Generic Reader, using PyTangoArchiving.Schemas properties
         
         elif self.db_name=='*':
-          
-            rd = getArchivingReader(attribute,start_time,stop_time,
-                  self.configs.get('hdb',None),self.configs.get('tdb',None),
-                  logger=self.log)
-            if not rd: 
-                self.log.warning('In get_attribute_values(%s): '
-                  'No valid schema at %s'%(attribute,start_date))
-                return []
-            #@debug
-            self.log.warning('In get_attribute_values(%s): '
-              'Using %s schema at %s'%(attribute,rd.schema,start_date))
-
-            #@TODO, implemented classes should have polimorphic methods
-            values = rd.get_attribute_values(attribute,start_date,stop_date,
-                    asHistoryBuffer=asHistoryBuffer,decimate=decimate,
-                    notNone=notNone,N=N)
-            
-            # If no data, it just tries the next database
-            if fallback and (values is None or not len(values)): 
-                sch = self.is_attribute_archived(attribute)[1:]
-                while not len(values) and len(sch):
-                    self.log.warning('In get_attribute_values(%s,%s,%s)(%s): '
-                      'fallback to %s as %s returned no data'%(
-                        attribute,start_date,stop_date,rd.schema,
-                        sch[0], rd.schema))
-                    values = self.configs[sch[0]].get_attribute_values(
-                        attribute,start_date,stop_date,
-                        asHistoryBuffer=asHistoryBuffer,decimate=decimate,N=N)
-                    sch = sch[1:]
-          
-        # END OF GENERIC CODE
-        #######################################################################
+            if subprocess:
+                self.log.info('Getting %s values in a background process ...' 
+                          % attribute)
+                #load caches before spawning processes
+                alias = self.get_attribute_alias(attribute)
+                [self.is_attribute_archived(a) for a in (alias,attribute)]
+                
+            values,ints = [],[]
+            density = 100. # avg thermocouple array density
+            i0 = start_time
+            while True:
+                end_time = (stop_time,i0 + MAX_QUERY_ROWS/density)[subprocess]
+                v0 = len(values)
+                i1 = min((end_time,stop_time))
+                d0,d1 = fn.time2str(i0),fn.time2str(i1)
+                self.log.info('getting %s - %s (%f vals/sec)' % (d0,d1,density))
+
+                # decimation done in sub-readers
+                args = (attribute, d0, d1, i0, i1,
+                        asHistoryBuffer, decimate, notNone, N, cache, 
+                        fallback, schemas, lasts if not(len(ints)) else False)
+                if subprocess:
+                    values.extend(SubprocessMethod(
+                        self.get_attribute_values_from_any,
+                        *args,
+                        sp_timeout = timeout, sp_callback = None))
+                else:
+                    values.extend(self.get_attribute_values_from_any(*args))
+                
+                density = get_density(values) or 10. #safer calcullation
+                ints.append((i0,i1))
+                i0 = i1
+                
+                if end_time >= stop_time:
+                    break
+                else:
+                    fn.wait(.1)
+            
+            #split = 5*86400
+            #ints = range(int(start_time),int(stop_time),split)
+            #ints.append(stop_time)
+            #ints = zip(ints,ints[1:])
+            #for i0,i1 in ints:
+                #d0,d1 = fn.time2str(i0),fn.time2str(i1)
+                #self.log.info('getting %s - %s' % (d0,d1))
+                ## decimation done in sub-readers
+                #args = (attribute, d0, d1, i0, i1,
+                        #asHistoryBuffer, decimate, notNone, N, cache, 
+                        #fallback, schemas, not(len(values)))
+                #if subprocess:
+                    #values.extend(SubprocessMethod(
+                        #self.get_attribute_values_from_any,
+                        #*args,
+                        #timeout = 3600, callback = None))
+                #else:
+                    #values.extend(self.get_attribute_values_from_any(*args))
+
+                #fn.wait(.1)
+
+            self.log.info('obtained %d values in %d steps' % (len(values),len(ints)))
           
         #######################################################################
         # HDB/TDB Specific Code
         else:
-            
             alias = self.get_attribute_alias(attribute).lower()
             #Needed to record last read values for both alias and real name
             attribute,alias = alias,attribute 
-            #@debug
-            self.log.warning('In PyTangoArchiving.Reader.get_attribute_values'
+            self.log.debug('In PyTangoArchiving.Reader.get_attribute_values'
                 '(%s,%s,%s,%s)'%(self.db_name,attribute,start_date,stop_date))
             
             #Checks if the attribute is a member of an array 
             array_index = re.search('\[([0-9]+)\]',attribute) 
             if array_index: 
                 attribute = attribute.replace(array_index.group(),'')
                 #Gets the index as an string
                 array_index = array_index.groups()[0] 
             
             self.last_dates[alias] = l1,l2
             db = self.get_database(l1)
             
             ###################################################################
             # QUERYING NEW HDB/TDB VALUES
-            if not db:
-                ##USING JAVA EXTRACTORS
-                values = self.get_extractor_values(attribute, start_date, 
-                                        stop_date, decimate, asHistoryBuffer)
-            else:
-                values = self.get_attribute_values_from_db(attribute, db,
-                            start_date, stop_date, decimate, 
-                            asHistoryBuffer, N, notNone, GET_LAST)
-                
-        #######################################################################
-        #DECIMATION IS DONE HERE
-        
-        l0,t1 = len(values),time.time()
-        if l0 > 128 and decimate:
-            decimate,window = decimate if isSequence(decimate) \
-                                        else (decimate,'0')
-            if isString(decimate):
-                try: 
-                    decimate = eval(decimate)
-                except:
-                    self.log.warning('Decimation(%s)?: %s'
-                        % (decimate, traceback.format_exc()))
-                        
-            ## Decimation by data_has_changed is done always
-            values = decimation(values, decimate, window=window, 
-                                logger_obj=self.log)
-                
-            #@debug
-            self.log.warning('\tDecimated %s[%d > %d] in %s s' 
-                    % (attribute,l0,len(values),time.time()-t1))
-            t1 = time.time()
-                    
+            #if not db:
+                ###USING JAVA EXTRACTORS
+                #values = self.get_extractor_values(attribute, start_date, 
+                                        #stop_date, decimate, asHistoryBuffer)
+            values = self.get_attribute_values_from_hdb(attribute, db,
+                        start_date, stop_date, decimate, 
+                        asHistoryBuffer, N, notNone, GET_LAST)
+            
+            values = self.decimate_values(values, decimate)
+
         #Simulating DeviceAttributeHistory structs
         if asHistoryBuffer:
-            values = [FakeAttributeHistory(*v) for v in values]                
-                    
+            values = [FakeAttributeHistory(*v[:3]) for v in values]                
+            
         #Array index is an string or None
         if array_index: 
-            values = self.extract_array_index(values,array_index,
-                                                decimate,asHistoryBuffer)
+            values = extract_array_index(values,array_index,
+                                                decimate) #,asHistoryBuffer)
                 
         #######################################################################
         # SAVE THE CACHE
         if cache:
             self.cache[(attribute,l1,l2,asHistoryBuffer,bool(decimate))
-                    ] = values[:]                
+                    ] = values[:]      
+            
+        self.log.debug('Out of get_attribute_values(): %d values' %
+                         len(values))
+
+        return values
+    
+    #@Debugged
+    def get_attribute_values_from_any(self, attribute, start_date, 
+        stop_date, start_time, stop_time, asHistoryBuffer=False, 
+        decimate=False, notNone=False, N=0, cache=True, fallback=True,
+        schemas = None, lasts = True):
+        if schemas is not None:
+            schemas = fn.toList(schemas) if schemas is not None else []        
+    
+        self.log.debug(str((self.db_name, len(self.current_attributes), attribute, True, start_time, stop_time, schemas)))
+        df = self.is_attribute_archived(attribute, preferent = True, start = start_time, stop = stop_time) 
+        self.log.debug(str(df))
+        sch = [s for s in self.is_attribute_archived(
+            attribute, preferent = True, start = start_time, stop = stop_time) 
+            #if (not schemas or s in schemas)
+            ]
+        
+        if not sch: 
+            self.log.warning('In get_attribute_values_from_any(%s): '
+                'No valid schema at %s'%(attribute,start_date))
+            return []
+        
+        self.log.info('In get_attribute_values_from_any(%s, %s, %s, %s)' % (
+            attribute, sch, start_date, stop_date))
+        rd = Schemas.getReader(sch.pop(0))
+        #@debug
+        self.log.debug('Using %s schema at %s'%(rd.schema,start_date))
+        
+        ## @TODO, this if is True if attribute is archived on alias only
+        # all this double-checks are slowing down queries, a solution
+        # must be found (is_attribute_archived on list?)
+        if not rd.is_attribute_archived(attribute):
+            # Stored in preferred schema via alias
+            attr = self.get_attribute_alias(attribute)
+            attr = self.get_attribute_model(attr)
+            if attr!=attribute:
+                self.log.info('%s => %s' % (attribute, attr))
+                attribute = attr
+
+        #@TODO, implemented classes should have polimorphic methods
+        values = rd.get_attribute_values(attribute,start_date,stop_date,
+                asHistoryBuffer=asHistoryBuffer,decimate=decimate,
+                notNone=notNone,N=N)
+        if len(values):
+            self.log.debug('%d values: %s,...'
+                % (len(values),str(values[0])))
+        
+        # If no data, it just tries the next database
+        if fallback:
+            if (values is None or not len(values)): 
+                gaps = [(start_time,stop_time)]
+            else:
+                r = max((300,.1*(stop_time-start_time)))
+                gaps = get_gaps(values,r,
+                                start = start_time if not N else 0,
+                                stop = stop_time if not N else 0)
+                self.log.debug('get_gaps(%d): %d gaps' % (len(values),len(gaps)))
+
+            fallback = []
+
+            for gap0,gap1 in gaps:
+                prev = rd.schema #every iter searches through all schemas on each gap
+                sch = [s for s in self.is_attribute_archived(attribute, 
+                    start = gap0, stop = gap1, preferent=False)
+                    if (s != prev and (not schemas or s in schemas))]
+                if not sch: 
+                    break
+                self.log.warning('trying fallbacks: %s' % str(sch))
+                gapvals = []
+
+                while not len(gapvals) and len(sch):
+                    self.log.info(#'In get_attribute_values(%s,%s,%s)(%s): '
+                    'fallback to %s as %s returned no data in (%s,%s)'%(
+                        #attribute,gap0,gap1,prev,
+                        sch[0],rd.schema,time2str(gap0),time2str(gap1)))
+                    
+                    gapvals = self.configs[sch[0]
+                        ].get_attribute_values(attribute,gap0,gap1,N=N,
+                        asHistoryBuffer=asHistoryBuffer,decimate=decimate)
+                        
+                    prev,sch = sch[0],sch[1:]
+
+                if len(gapvals):
+                    fallback.extend(gapvals)
+               
+            if len(fallback):
+                tf = fn.now()
+                values = sorted(values+fallback)
+                self.log.debug('Adding %d values from fallback took '
+                    '%f seconds' % (len(fallback),fn.now()-tf))
+            
+            # Loading last values to fill initial gap
+            if decimate:
+                gap = start_time + (decimate if fn.isNumber(decimate) 
+                   else (stop_time-start_time)/utils.MAX_RESOLUTION)
+            else:
+                gap = start_time + 60.
+                
+            if lasts and (not len(values) or not len(values[0]) or values[0][0] > gap):
+                self.log.warning('No %s values at %s, loading previous values' % (
+                    attribute, fn.time2str(start_time)))
+                lasts = self.load_last_values(attribute, epoch=start_time)
+                lasts = [v for k,v in lasts.items() if 
+                        k not in ('hdb','tdb') and v is not None and len(v)]
+                lasts = sorted(t for t in lasts if t and len(t))
+                if len(lasts): 
+                    values.insert(0,tuple(lasts[-1][
+                        :len(values[0]) if values else 2]))
 
+        values = self.decimate_values(values, decimate)
+        #self.log.setLogLevel()
         return values
     
-    def get_attribute_values_from_db(self, attribute, db, 
+    def get_attribute_values_from_hdb(self, attribute, db, 
             start_date, stop_date, decimate, asHistoryBuffer, 
             N, notNone, GET_LAST):
         """
         Query MySQL HDB/TDB databases to extract the attribute data
         """
         # CHOOSING DATABASE METHODS
         if not self.is_hdbpp:
+            self.log.debug('get_attribute_values_from_hdb(%s,%s)' % 
+                (attribute, db))
+            attribute = fn.first([a for a in db.get_attribute_names(active=False)
+                if fn.tango.get_simple_name(a) == fn.tango.get_simple_name(attribute)],
+                'attribute')
             try:
                 full_name,ID,data_type,data_format,writable = \
                     db.get_attribute_descriptions(attribute)[0]
-            except Exception,e: 
+            except Exception as e: 
+                print(attribute)
+                traceback.print_exc()
                 raise Exception('%s_AttributeNotArchived: %s'
                                 %(attribute,e))
 
             data_type,data_format = (utils.cast_tango_type(
                 PyTango.CmdArgType.values[data_type]),
                 PyTango.AttrDataFormat.values[data_format])
             
@@ -1052,50 +1292,52 @@
             data_type = float
             data_format = PyTango.AttrDataFormat.SCALAR
 
         #######################################################################
         # QUERYING THE DATABASE 
         #@TODO: This retrying should be moved down to ArchivingDB class instead
         retries,t0,s0,s1 = 0,time.time(),start_date,stop_date
-        while retries<2 and t0>(time.time()-10):
+        MAX_RETRIES = 2
+        while retries<MAX_RETRIES and t0>(time.time()-10):
             if retries: 
                 #(reshape/retry to avoid empty query bug in python-mysql)
-                self.log.warning('\tQuery (%s,%s,%s) returned 0 values, '
-                                 'retrying ...' % (attribute,s0,s1))
+                self.log.debug('\t%s Query (%s,%s,%s) returned 0 values, '
+                                 'retrying ...' % (self.schema,attribute,s0,s1))
                 s0,s1 = epoch2str(str2epoch(s0)-30),epoch2str(str2epoch(s1)+30) 
             result = method(table,s0,s1 if not GET_LAST else None,
                             N=N,unixtime=True)
             if len(result): 
                 if retries:
                     result = [r for r in result if start_date<=r[0]<=stop_date]
                 break
             retries+=1
 
         if not result: 
-            self.log.warning('Empty query after %d retries? (%s) = [0] in %ss'
-                % (retries,str((table,start_date,stop_date,GET_LAST,N,0)),
+            self.log.warning('Empty %s query after %d retries? (%s) = [0] in %ss'
+                % (self.schema,retries,str((table,start_date,stop_date,GET_LAST,N,0)),
                    time.time()-t0))
             return []
         
         l0 = len(result)
         t1 = time.time()
         #@debug
         self.log.info('\tQuery(%s,%s,%s,%s,%s) = [%d] in %s s'
                        %(table,start_date,stop_date,GET_LAST,N,l0,t1-t0))       
         self.last_reads = result and (result[0][0],result[-1][0]) or (1e10,1e10)
         
         try:
             values = self.extract_mysql_data(result,
                             data_type,data_format,notNone)
             values = patch_booleans(values)
-        except Exception,e:
+        except Exception as e:
             self.log.info(traceback.format_exc())
             raise Exception('Reader.UnableToConvertData(%s,format=%s)'
                             % (attribute,data_format),str(e))
         
+        self.log.info('get_from_db(%s)' % str(len(values) and values[0]))
         return values
     
     def extract_mysql_data(self, result, data_type, data_format, notNone):
         # CASTING DATATYPES AND DECIMATION
         #Returning a list of (epoch,value) tuples
         values = []
         t1 = time.time()
@@ -1134,75 +1376,90 @@
         elif notNone:
             values = [(w[0],w[ix]) for w in result if w[ix] is not None]
         else:
             values = [(w[0],w[ix]) for w in result]
 
         #@debug
         self.log.info('\tParsed [%d] in %s s'%(len(values),time.time()-t1))
-
-        return values    
-        
-    def extract_array_index(self,values,array_index,decimate=False,asHistoryBuffer=False):
-        # Applying array_index to the obtained results, it has to be applied after attribute loading to allow reusing cache in array-indexed attributes
-        last,l0 = (0,None),len(values)
-        
-        self.log.debug('Applying array_index(%s) to the obtained results'%array_index)
-        array_index = int(array_index)
-        new_values = [] # We create a new list on purpose to not modify the cached values
-        fin = (lambda v: (v.time,v.value[array_index] if v.value is not None and len(v.value)>array_index else None)) if asHistoryBuffer \
-            else (lambda v: (v[0],v[1][array_index] if v[1] is not None and len(v[1])>array_index else None))
-        fcmp = (lambda l: (l[0].tv_sec,l[1])) if asHistoryBuffer else (lambda l: l)
-        fout = (lambda vv: FakeAttributeHistory(*(vv))) if asHistoryBuffer else (lambda vv: vv)
-        for i,v in enumerate(values):
-            try:
-                if v is None: continue
-                vv = fin(v)
-                next = ((values[i+1] and fin(values[i+1]) or None) if i+1<l0 else None)
-                if not decimate or next is None or not new_values or data_has_changed(fcmp(vv),fcmp(last),fcmp(next)):
-                    new_values.append(fout(vv))
-                    last = vv
-            except Exception,e:
-                self.log.warning('reader.get_attribute_values(...,asHistoryBuffer=%s): Unable to parse %d[%s]:(%s); %s'%(asHistoryBuffer,i,array_index,v,traceback.format_exc()))
-        if decimate:
-            self.log.info('\tIn extract_array_index(...).raw: decimated repeated values in spectrum ... %s -> %s'%(l0,len(new_values)))
-        return new_values
+        return values       
+    
+    def decimate_values(self, values, decimate):
+        """ 
+        proxy method to parse arguments for utils.decimation 
+        Removal of None values is always done
+        Decimation by data_has_changed is done always
+        Decimation on window is only done if decimate is callable (pickfirst)
+        """
+        l0 = len(values)
+        if len(values) > 128 and decimate: 
+            decimate,window = decimate if isSequence(decimate) \
+                                        else (decimate,'0')
+            if isString(decimate):
+                try: 
+                    decimate = eval(decimate)
+                except:
+                    self.log.info('Decimation(%s)?: %s'
+                        % (decimate, traceback.format_exc()))
+            
+            values = utils.decimation(values, decimate, window=window, 
+                                logger_obj=self.log)
+            self.log.debug('decimate([%d],%s):[%d]' % (l0,decimate,len(values)))
+            
+        return values
     
-    def get_attributes_values(self,attributes,start_date,stop_date=None,correlate=False,
-                              asHistoryBuffer=False,trace = False, text = False, N=0):
+    def get_attributes_values(self,attributes,start_date,stop_date=None,
+            asHistoryBuffer=False,decimate=False,notNone=False,N=0,
+            cache=True,fallback=True,schemas=None,
+            correlate=False, trace = False, text = False, subprocess=True,
+            lasts=False):
         """ 
         This method reads values for a list of attributes between specified dates.
         
         :param attributes: list of attributes
         :param start_date: timestamp of the first value
         :param stop_date: timestamp of the last value
         :param correlate: group values by time using first attribute timestamps
         :param asHistoryBuffer: return a history buffer object instead of a list (for trends)
-        :param trace: print out the values obtained
+        
         :param text: return a tabulated text instead of a dictionary of values
         :param N: if N>0, only the last N values will be returned
+        :param trace: print(out the values obtained)
         
         :return: a dictionary with the values of each attribute or (if text=True) a text with tabulated columns
         
         """
-        if not attributes: raise Exception('Empty List!')
-        start = time.time()
-        values = dict([(attr,self.get_attribute_values(attr,start_date,stop_date,asHistoryBuffer,N=N)) for attr in attributes])
-        self.log.debug('Query finished in %d milliseconds'%(1000*(time.time()-start)))
+        if not attributes: 
+            raise Exception('Empty List!')
+        t0= time.time()
+        self.log.debug('get_attributes_values(...)')
+        start_date,start_time,stop_date,stop_time = \
+            self.get_time_interval(start_date,stop_date)        
+        
+        values = dict([(attr,
+            self.get_attribute_values(attr, start_date, stop_date,
+                        asHistoryBuffer, decimate, notNone, N,
+                        cache, fallback, schemas, subprocess=subprocess,
+                        lasts=lasts))
+                        for attr in attributes])
+        self.log.debug('Query finished in %d milliseconds'%(1000*(time.time()-t0)))
         if correlate or text:
+            self.log.debug('correlate ...')
             if len(attributes)>1:
-                table = self.correlate_values(values,str2time(stop_date),resolution=(correlate if correlate is not True and fun.isNumber(correlate)  else None))
+                table = self.correlate_values(values,str2time(stop_date),
+                    resolution=(correlate if correlate is not True 
+                                and fn.isNumber(correlate)  else None))
             else:
                 table = values
             if trace or text: 
                 csv = self.export_to_text(table,order=list(attributes))
                 if text: return csv
-                elif trace: print csv
+                elif trace: print(csv)
             return table
         else:
-            if trace: print values
+            if trace: print(values)
             return values
           
     @staticmethod
     def export_to_text(table,order=None,**kwargs):
         """
         It will convert a [(timestamp,value)] array in a CSV-like text.
         Order will be used to set the order to data columns (date and timestamp will be always first and second).
@@ -1215,25 +1472,38 @@
           
         """
         sep = kwargs.get('sep','\t')
         arrsep = kwargs.get('arrsep',kwargs.get('separator',', '))
         linesep = kwargs.get('linesep','\n')
         
         start = time.time()
-        if not hasattr(table,'keys'): table = {'attribute':table}
-        if not order or not all(k in order for k in table): keys = list(sorted(table.keys()))
-        else: keys = sorted(table.keys(),key=order.index)
+        if not hasattr(table,'keys'): 
+            table = {'attribute':table}
+        if not order or not all(k in order for k in table): 
+            keys = list(sorted(table.keys()))
+        else: 
+            keys = sorted(table.keys(),key=order.index)
+
         csv = sep.join(['date','time']+keys)+linesep
+
         def value_to_text(s):
-          v = (str(s) if not fandango.isSequence(s) else arrsep.join(map(str,s))).replace('None','')
+          v = (str(s) if not fandango.isSequence(s) 
+                    else arrsep.join(map(str,s))).replace('None','')
           return v
-        time_to_text = lambda t: time2str(t,cad='%Y-%m-%d_%H:%M:%S')+('%0.3f'%(t%1)).lstrip('0') #taurustrend timestamp format
-        for i in range(len(table.values()[0])):
-            csv+=sep.join([time_to_text(table.values()[0][i][0]),str(table.values()[0][i][0])]+[value_to_text(table[k][i][1]) for k in keys])
+
+        time_to_text = lambda t: (time2str(t,cad='%Y-%m-%d_%H:%M:%S')
+            +('%0.3f'%(t%1)).lstrip('0')) #taurustrend timestamp format
+        
+        ml = min(len(v) for v in table.values())
+        for i in range(ml): 
+            csv+=sep.join([time_to_text(fn.first(table.values())[i][0]),
+                    str(fn.first(table.values())[i][0])]
+                +[value_to_text(table[k][i][1]) for k in keys])
             csv+=linesep
+            
         print('Text file generated in %d milliseconds'%(1000*(time.time()-start)))
         return csv
 
     def correlate_values(self,values,stop=None,resolution=None,debug=False,rule=None,MAX_VALUES=50000):
         ''' Correlates values to have all epochs in all columns
         :param values:  {curve_name:[values]}
         :param resolution: two epochs with difference smaller than resolution will be considered equal
@@ -1255,16 +1525,16 @@
             if avg < 10: resolution = 1
             elif 10 <= avg<60: resolution = 10
             elif 60 <= avg<600: resolution = 60
             elif 600 <= avg<3600: resolution = 600
             else: resolution = 3600 #defaults
             self.log.info('correlate_values(...) resolution set to %2.3f -> %d s'%(avg,resolution))
         assert resolution>.1, 'Resolution must be > 0'
-        if rule is None: rule = fun.partial(choose_first_value,tmin=-resolution*10)
-        #if rule is None: rule = fun.partial(choose_last_max_value,tmin=-resolution*10)
+        if rule is None: rule = fn.partial(choose_first_value,tmin=-resolution*10)
+        #if rule is None: rule = fn.partial(choose_last_max_value,tmin=-resolution*10)
         
         epochs = range(int(first-resolution),int(last+resolution),int(resolution))
         for k,data in values.items():
             self.log.info('Correlating %s->%s values from %s'%(len(data),len(epochs),k))
             i,v,end = 0,data[0] if data else (first,None),data[-1][0] if data else (last,None)
 
             for t in epochs:
@@ -1307,16 +1577,16 @@
         try: 
             extractor = self.get_extractor(attribute=attribute)
             #self.clean_extractor(extractor)
             result = self.__extractorCommand(extractor,'GetAttDataBetweenDates',[attribute,start_date,stop_date])
             vattr,vsize=str(result[1][0]),int(result[0][0])
             time.sleep(0.2)
             if vattr not in [a.name for a in extractor.attribute_list_query()]:
-                raise Exception,'%s_NotIn%sAttributeList'%(vattr,extractor.name())
-            self.log.debug( '\treading last value of attribute %s'%vattr)
+                raise Exception('%s_NotIn%sAttributeList' % (i,vattr(extractor.name())))
+            self.log.debug( '\treading last value of attribute %s' % vattr)
             last_value = extractor.read_attribute(vattr).value
             self.log.debug('\treading %s attribute history values of %s (last_value = %s)'% (vsize,vattr,last_value))
             history=extractor.attribute_history(vattr,vsize)
             if N>0: history = history[-N:]
             #DECIMATION IS DONE HERE ##########################################################################
             if decimate:
                 nhist,l0 = [],len(history)
@@ -1324,80 +1594,85 @@
                     #if not i or h.value!=history[i-1].value or ((i+1)<l0 and history[i+1].value!=h.value) or h.time.tv_sec>=(300+nhist[-1].time.tv_sec):
                     if not i or data_has_changed(h_to_tuple(h),h_to_tuple(history[i-1]),h_to_tuple(history[i+1]) if i+1<l0 else None):
                         nhist.append(h)
                 self.log.debug('\tIn get_attribute_values(%s,...).extractor: decimated repeated results ... %s -> %s'%(attribute,len(history),len(nhist)))
                 history = nhist
             #Sorting extracted values
             try: history=[v for t,u,v in sorted((h.time.tv_sec,h.time.tv_usec,h) for h in history)]
-            except Exception,e: self.log.error('Unable to sort history values: %s'%e)
+            except Exception as e: self.log.error('Unable to sort history values: %s'%e)
             
             self.clean_extractor(extractor,vattr)
             self.attr_extracted[attribute]=(lambda s: s if ':' in s else self.tango_host+'/'+s)(extractor.name())
-        except Exception,e: 
+        except Exception as e: 
             self.log.warning( traceback.format_exc())
-            raise Exception,'Archiving.Reader_ExtractorFailed(%s)!:%s' % (extractor.name(),str(e))
+            raise Exception('Archiving.Reader_ExtractorFailed(%s)!:%s' % (extractor.name(),str(e)))
         if int(PyTango.__version__.split('.')[0])>=7:
             values = asHistoryBuffer and history or [(ctime2time(h.time),h.value) for h in history]
             self.last_reads = history and (ctime2time(history[0].time),ctime2time(history[-1].time)) or (1e10,1e10)
         else:
             values = asHistoryBuffer and history or [(ctime2time(h.value.time),h.value.value) for h in history]
             self.last_reads = history and (ctime2time(history[0].value.time),ctime2time(history[-1].value.time)) or (1e10,1e10)
 
         return values
+    
+    def clear_cache(self):
+        self.cache.clear()
+        for m in dir(self):
+            try:
+                m = getattr(self,m)
+                if fn.isCallable(m) and hasattr(m,'cache'):
+                    m.cache.clear()
+            except:
+                traceback.print_exc()
         
     def clean_extractor(self,extractor,vattr=None):
         ''' removing dynamic attributes from extractor devices ...'''
         #self.log.debug('In PyTangoArchiving.Reader.__cleanExtractor(): removing dynamic attributes')
         self.log.debug( 'In PyTangoArchiving.Reader.__cleanExtractor(): removing dynamic attributes')
         self.log.debug( '%s(%s)'%(type(extractor),extractor) )
         if hasattr(extractor,'dev_name'):
             name,proxy=extractor.dev_name(),extractor
         else: 
             name,proxy=str(extractor),self.servers.proxies[str(extractor)]
         if vattr: proxy.RemoveDynamicAttribute(vattr)
         else: proxy.RemoveDynamicAttributes()
         
-    #def __initMySQLconnection(self):
-        #try: self.db = MySQLdb.connect(db=self.db_name,host=self.host,user=self.user,passwd=self.passwd)
-        #except Exception,e:
-            #self.log.error( 'Unable to create a MySQLdb connection to "%s"@%s.%s: %s'%(self.user,self.host,self.db_name,traceback.format_exc()))
-            #self.db = None
-            
     def __extractorCommand(self,extractor=None,command='',args=[]):
-        if not command: raise Exception,'Reader__extractorCommand:CommandArgumentRequired!'
+        if not command: raise Exception('Reader__extractorCommand:CommandArgumentRequired!')
         if not extractor: extractor = self.get_extractor()
         extractor.ping()        
         try:
             self.log.debug( 'in damn Reader.__extractorCommand: calling HdbExtractor(%s).%s(%s)'%(extractor.name(),command,args))
             result = extractor.command_inout(*([command]+(args and [args] or [])))
-        except PyTango.DevFailed, e:
+        except PyTango.DevFailed as  e:
             #e.args[0]['reason'],e.args[0]['desc'],e.args[0]['origin']
             reason = '__len__' in dir(e.args[0]) and e.args[0]['reason'] or e.args[0]
             if 'Broken pipe' in str(reason):
                 extractor.init()
                 result = extractor.command_inout(*([command]+(args and [args] or [])))
             elif 'MEMORY_ERROR' in str(reason):
-                #raise Exception,'Extractor_%s'%reason
+                #raise Exception('Extractor_%s'%reason)
                 self.clean_extractor(extractor.name())
                 extractor.init()
                 result = extractor.command_inout(*([command]+(args and [args] or [])))
             else:
                 self.log.warning(traceback.format_exc())
-                raise Exception,'Reader__extractorCommand:Failed(%s)!'% str(e)
+                raise Exception('Reader__extractorCommand:Failed(%s)!'% str(e))
         #self.log.debug( 'in Reader.__extractorCommand: command finished')
         return result
             
 #################################################################################################
 # Multiprocess Class for Reader
 #################################################################################################
 
 class ReaderByBunches(Reader):
     """
     Class that splits in bunches every query done against the database.
-    It allows only database queries; not extractor
+    It allows only database queries; not extractor devices
+    It uses multiprocessing and threading to run queries in parallel
     """
     DEFAULT_BUNCH_SIZE = 1000
     def init_buncher(self):
         self._process_event,self._threading_event,self._command_event = multiprocessing.Event(),threading.Event(),threading.Event()
         self._receiver = threading.Thread(target=self._receive_data)
         self._receiver.daemon = True #Therefore, keep_alive routines should not be needed!
         self._last_alive = time.time()
@@ -1451,15 +1726,15 @@
                             try:
                                 self.debug('\tlaunching callback %s'%callback)
                                 callback(query)
                             except:
                                 self.warning('\tError in %s callback %s!'%(key,callback))
                                 self.warning(traceback.format_exc())
                         self.callbacks.pop(key)
-            except Exception,e:
+            except Exception as e:
                 self.warning('\tError in thread!\n%s'%(traceback.format_exc()))
             self._threading_event.wait(0.1)
         self.log.info('Exiting PyTangoArchiving.ReaderProcess()._receive_data thread')
         
     def _send_query(self,key,query,callback):
         assert self.alive()
         if key not in self.callbacks: 
@@ -1487,17 +1762,15 @@
         :param asHistoryBuffer: return a history buffer object instead of a list (for trends)
         :param N: if N>0, only the last N values will be returned
         :param decimate: remove repeated values, False by default but True when called from trends
         
         :return: a list with values (History or tuple values depending of args)
 
         """
-        #Previous implementation was discarded due to this exception
-        #raise Exception("MySQLdb.SSCursor.fetchmany failed due to (2013, 'Lost connection to MySQL server during query')")
-        assert self.alive()
+        if not self.alive(): raise Exception('DeadThread!')
         """
         This method will just put the query in the queue
         """
         decimate,window = decimate if isSequence(decimate) else (decimate,'0')
         if callable(decimate): decimate = decimate.__module__+'.'+decimate.__name__
         query = {'attribute':attribute,'start_date':start_date,'stop_date':stop_date,'asHistoryBuffer':asHistoryBuffer,'decimate':(decimate,window),'N':N}
         assert hasattr(callback,'__call__'),'2nd argument must be callable'
@@ -1546,21 +1819,21 @@
         if self.logger: [setattr(self,f,getattr(logger,f)) for f in ('debug','info','warning','error')]
         self.info('In ReaderProcess(%s)'%([db,config,servers,schema,timeout,log,logger,tango_host,alias_file]))
 
         #Reader Part
         self.available_attributes,self.failed_attributes,self.asked_attributes = [],[],[]
         self.last_dates = defaultdict(lambda:(1e10,0))
         self.updated,self.last_retry = 0,0
-        self.tango_host = tango_host or os.getenv('TANGO_HOST')
+        self.tango_host = tango_host or fn.get_tango_host()
         self.tango = PyTango.Database(*self.tango_host.split(':'))
 
         try:
             alias_file = alias_file or get_alias_file()       
             self.alias = alias_file and read_alias_file(alias_file)
-        except Exception,e: 
+        except Exception as e: 
             self.log.warning('Unable to read alias file %s: %s'%(alias_file,e))
 
         if schema is not None and db=='*': db = schema
         if any(s in ('*','all') for s in (db,schema)): db,schema = '*','*'
         self.state = PyTango.DevState.INIT
         self.schema = schema
         
@@ -1586,18 +1859,20 @@
         self.stop()
         type(self).__base__.__del__(self)
     
     def start(self):
         self._reader.start()
         self._receiver.start()
         self.get_attributes()
+        
     def stop(self):
         self.info('ReaderProces().stop()')
         self._process_event.set(),self._threading_event.set()
         self._pipe1.close(),self._pipe2.close() 
+        
     def alive(self):
         if not self._reader.is_alive():
             raise Exception('ReaderProcess is not Alive!!! (last contact at %s)'%time.ctime(self._last_alive))
         self._last_alive = time.time()
         return self._last_alive
     
     # Protected methods
@@ -1609,15 +1884,15 @@
     def _reader_process(db,config,servers,schema,timeout,log,logger,tango_host,alias_file,pipe,event,alive=ALIVE_PERIOD):
         
         reader = Reader(db=db,config=config,servers=servers,schema=schema,timeout=timeout,
                         log=log,logger=logger,
                         tango_host=tango_host,alias_file=alias_file,
                         )
         self = Logger()
-        reader.log.setLogLevel('INFO')
+        #reader.log.setLogLevel('INFO')
         last_alive = time.time()
         while not event.is_set(): #and (pipe.poll() or time.time()<(last_alive+2*alive)): #Alive should not be needed if process is daemonic
             if pipe.poll(.1):
                 self.debug('PyTangoArchiving.ReaderProcess(): receiving ...')
                 key,query = pipe.recv()
                 try:
                     if time.time()<(last_alive+2*alive): #if key=='ALIVE':
@@ -1667,15 +1942,15 @@
                             try:
                                 self.debug('\tlaunching callback %s'%callback)
                                 callback(query)
                             except:
                                 self.warning('\tError in %s callback %s!'%(key,callback))
                                 self.warning(traceback.format_exc())
                         self.callbacks.pop(key)
-            except Exception,e:
+            except Exception as e:
                 self.warning('\tError in thread!\n%s'%(traceback.format_exc()))
             self._threading_event.wait(0.1)
         self.info('Exiting PyTangoArchiving.ReaderProcess()._receive_data thread')
         
     def _send_query(self,key,query,callback):
         assert self.alive()
         if key not in self.callbacks:
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/schemas.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/schemas.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,189 +23,334 @@
 
 """
 PyTangoArchiving.schemas: This module provides the Schemas object; 
 a singleton to detect and manage multiple archiving schemas.
 """
 
 import traceback,time,re
-import fandango
-import fandango.functional as fun
-from fandango import clmatch
+import fandango as fn
+from fandango import clmatch, clsearch, time2str, str2time
+
+from PyTangoArchiving.utils import parse_property, overlap
+import PyTangoArchiving.dbs as dbs
 
 import sys
-EXPERT_MODE = True
-    #any(a in str(sys.argv) for a in 
-        #('ArchivingBrowser.py','ctarchiving','taurustrend',
-         #'taurusfinder','ctsearch','ipython', 'test','-c',
-         #'archiving2csv','archiving2plot','matlab','PyExtractor'))
          
-class SchemaDict(dict):
+def get_archiving_hosts():
+    """
+    It returns hosts declared in schemas
+    """
+    hosts = [v.get('host',None) for v in Schemas().values()]
+    return list(sorted(set(hosts)))
+
+def get_host_schemas(host):
+    return sorted(k for k,v in Schemas.items() if host == v.get('host',None))
+         
+class SchemaDict(dict): #fn.Struct):
+    
+    ## The .get method seems to work differently in Struct and Dict!
+    
+    #def __init__(self,other,load=False):
+        #super(SchemaDict,self).__init__(**other)
+        #self._load = load
     
     def __getitem__(self,key):
+        
+        if key=='dbname':
+            v = super(SchemaDict,self).get('db_name',None)
+            if v is None:
+                v = super(SchemaDict,self).get('schema',None)
+            return v
+
         if key=='reader':
-            r = dict.get(self,'reader',None)
+            r = super(SchemaDict,self).get('reader',None)
             #print('%s.get(%s)' % (self['schema'],key))
+            
+            # if self._load and 
             if isinstance(r,str):
                 self['reader'] = Schemas.getReader(self['schema'],self.copy())
                 #print(self['reader'])
-        return dict.__getitem__(self,key)
+                
+        return super(SchemaDict,self).__getitem__(key)
     
     def get(self,key,default=None):
         try:
             return self.__getitem__(key)
         except:
             return default
-        
-    #def __getattribute__(self,name):
-        #if name in dict.keys(self):
-            #return self.__getitem__(name)
-        #else:
-            #return dict.__getattribute__(self,name)
     
         
 class Schemas(object):
     """ Schemas kept in a singleton object """
     
-    SCHEMAS = fandango.SortedDict()
-    MODULES = {'fandango':fun,'fun':fun} #Limited access to fandango library
-    LOCALS = fandango.functional.__dict__.copy()
+    SCHEMAS = fn.SortedDict()
+    #Limited access to fandango library
+    MODULES = {'fandango':fn.functional,'fn':fn.functional,'fun':fn.functional} 
+    LOCALS = fn.functional.__dict__.copy()
+    
+    def __init__(self):
+        self.load()
     
     @classmethod
     def __contains__(k,o):
         return o in k.SCHEMAS.keys()
     
     @classmethod
     def keys(k):
         if not k.SCHEMAS: 
             k.load()
         return k.SCHEMAS.keys()
     
     @classmethod
+    def values(k):
+        if not k.SCHEMAS: 
+            k.load()
+        return k.SCHEMAS.values()
+    
+    @classmethod
+    def items(k):
+        if not k.SCHEMAS: 
+            k.load()
+        return k.SCHEMAS.items()
+    
+    @classmethod
+    def __iter__():
+        """ TODO: iter() does not work in classes!"""
+        return k.SCHEMAS.__iter__()
+    
+    @classmethod
+    def __contains__(k,key):
+        return k.SCHEMAS.__contains__(key)
+    
+    @classmethod
+    def __getitem__(k,key):
+        return k.SCHEMAS.__getitem__(key)
+    
+    @classmethod
+    def get(k,key,default=None):
+        if not k.SCHEMAS: 
+            k.load()        
+        return k.SCHEMAS.get(key,default)
+    
+    @classmethod
+    @fn.Cached(expire=60.)
     def load(k,tango='',prop='',logger=None):
-        tangodb = fandango.tango.get_database(tango)
-        schemas = prop or tangodb.get_property(
-            'PyTangoArchiving','Schemas')['Schemas']
-        if not schemas:
-          schemas = ['tdb','hdb']
-          tangodb.put_property('PyTangoArchiving',{'Schemas':schemas})
-        print('Loading schemas from Tango Db ... (%s)'%','.join(schemas)) 
-        [k.getSchema(schema,tango,write=True,logger=logger)
-            for schema in schemas]
-        return k.SCHEMAS
+        #print('PyTangoArchiving.Schemas.load()')
+        try:
+            tangodb = fn.tango.get_database(tango)
+            props = prop or tangodb.get_property('PyTangoArchiving',
+                        ['DbSchemas','Schemas'])
+
+            try:
+                schemas = props.get('DbSchemas',[])
+            except:
+                print('PyTangoArchiving.DbSchemas not initialized')
+                schemas = []
+                
+            if not schemas:
+                schemas = props.get('Schemas', []) or []
+
+            if not schemas:
+                schemas = ['hdbpp']
+                tangodb.put_property('PyTangoArchiving',{'DbSchemas':schemas})
+            else:
+                schemas = filter(bool,[s.split('#')[0].strip() for s in schemas])
+
+            #print('Loading %s from tango@%s ... ' % (pname, tangodb.get_db_host()))
+
+            [k.getSchema(schema,tango,write=True,logger=logger) 
+                for schema in schemas]
+
+            return k.SCHEMAS
+
+        except:
+            traceback.print_exc()
+            return []
     
     @classmethod
     def pop(k,key):
         k.SCHEMAS.pop(key)
     
     @classmethod
     def _load_object(k,obj,dct):
         rd = obj
         m = rd.split('(')[0].rsplit('.',1)[0]
         c = rd[len(m)+1:]
         if m not in k.MODULES:
-            fandango.evalX('import %s'%m,modules=k.MODULES)
+            fn.evalX('import %s'%m,modules=k.MODULES)
         #print('getSchema(%s): load %s reader'%(schema,dct.get('reader')))
-        return fandango.evalX(obj, modules=k.MODULES, _locals=dct)
+        return fn.evalX(obj, modules=k.MODULES, _locals=dct)
     
     @classmethod
-    def getReader(k,schema,dct):
+    def getReader(k,schema,dct=None):
         # This method initializes a reader object from Schema config
         # It does not update the Schema object, just returns a reader
         
-        dct = dct if dct is not None else k.getSchema(schema)
+        dct = dct if dct is not None else k.getSchema(
+            schema if fn.isString(schema) else schema.get('schema'))
         rd = dct.get('reader',dct.get('api'))
 
         if rd and isinstance(rd,str):
             try:
                 #print('Schemas.getReader(%s): instantiating reader' % schema)
                 
                 rd = k._load_object(rd,dct)
-                print('getReader(%s): %s' % (schema,type(rd)))
+                #print('getReader(%s): %s' % (schema,type(rd)))
                 if not hasattr(rd,'is_attribute_archived'):
                     rd.is_attribute_archived = lambda *a,**k:True
                 if not hasattr(rd,'get_attributes'):
                     rd.get_attributes = lambda *a,**k:[]
                 if not hasattr(rd,'get_attribute_values'):
                     if dct['method']:
                         rd.get_attribute_values = getattr(rd,dct['method'])
-                if not hasattr(rd,'schema'): 
+                if not hasattr(rd,'schema'):
                     rd.schema = schema
             except:
                 print('getReader(%s) failed!' % schema)
-                traceback.print_exc()                    
+                #traceback.print_exc()
+                rd = None
         
         return rd
         
     
     @classmethod
     def getSchema(k,schema,tango='',prop='',logger=None, write=False):
-        
-        if schema.startswith('#') and EXPERT_MODE:
-            schema = schema.strip('#')
-            print('%s is enabled'%schema)
-
+        """
+        Get schema specs as defined in Tango.FreePropertis.DbSchemas
+        """
         if schema in k.SCHEMAS:
             # Failed schemas should be also returned (to avoid unneeded retries)
             return k.SCHEMAS[schema]
         
-        dct = SchemaDict({'schema':schema,'dbname':schema,
-               'match':clmatch,'clmatch':clmatch})
+        dct = {'match':clmatch,'clmatch':clmatch}
+        if ';' in schema:
+            schema,dct = schema.split(';',1)
+            dct = dict(d.split('=',1) for d in dct.split(';'))
+        dct['schema'] = schema
+        dct = SchemaDict(dct)
+        props = []
 
         try:
-            tango = fandango.tango.get_database(tango)
-            props = prop or tango.get_property('PyTangoArchiving',schema)[schema]
-            assert len(props)
-            if fandango.isSequence(props):
-                props = [map(str.strip,t.split('=',1)) for t in props]
+            tango = fn.tango.get_database(tango)
+            props = prop or tango.get_property('PyTangoArchiving',
+                                               schema)[schema]
+            if not len(props): 
+                #raise Exception('Empty Property!')
+                return {}
+            if fn.isSequence(props):
+                props = dict(map(str.strip,t.split('=',1)) for t in props)
+            if 'check' in dct:
+                props.pop('check')
             dct.update(props)
             dct['logger'] = logger
 
-        except Exception,e:
+        except Exception as e:
             print('getSchema(%s): failed!'%schema)
-            if logger: 
-                exc = traceback.format_exc()
-                try: logger.warning(exc)
-                except: print(exc)
+            print(dct,props)
+            exc = traceback.format_exc()
+            try: 
+                logger.warning(exc)
+            except: 
+                print(exc)
             dct = None
         
         if write:
             k.SCHEMAS[schema] = dct
+
         return dct
     
     @classmethod
-    def checkSchema(k,schema,attribute='',start=None,end=None):
-      #print('In reader.Schemas.checkSchema(%s,%s,%s,%s)'%(schema,attribute,start,end))
-      schema = k.getSchema(schema)
-      if not schema: return False
-      f = schema.get('check')
-      if not f: 
-        v = True
-      else:
+    def getSchemasForAttribute(attr,start=0,stop=fn.END_OF_TIME):
+        """
+        returns a fallback schema chain for the given dates
+        """
+        #print('getSchemasForAttribute(%s)' % attr)
+        return [s for s in k.SCHEMAS if k.checkSchema(s,attr,start,stop)]
+        
+    
+    @classmethod
+    def checkSchema(k, schema, attribute=None, start=None, stop=None, f=None):
+        if not f:
+            if not isinstance(schema, SchemaDict):
+                schema = k.getSchema(schema)
+                #print('getSchema(): %s' % str(schema))
+            if not schema: 
+                return False
+            
+            f = schema.get('check')
+            if not f: 
+                print('%s has no check function' % str(schema))
+                return True
+
         try:
-          now = time.time()
-          start = fun.notNone(start,now-1)
-          end = fun.notNone(end,now)
-          k.LOCALS.update({'attribute':attribute.lower(),
-                'match':clmatch,'clmatch':clmatch,
-                'start':start,'end':end,'now':now,
-                'reader':schema.get('reader',schema.get('api')),
-                'schema':schema.get('schema'),
-                'dbname':schema.get('dbname',schema.get('schema','')),
-                })
-          #print('(%s)%%(%s)'%(f,[t for t in k.LOCALS.items() if t[0] in f]))
-          v =fun.evalX(f,k.LOCALS,k.MODULES)
+            now = time.time()
+            start = (str2time(start) if fn.isString(start) 
+                     else fn.notNone(start,now-1))
+            stop = (str2time(stop) if fn.isString(stop) 
+                    else fn.notNone(stop,now))
+            xmatch = lambda e,a: (True if a is None 
+                                  else clmatch(e,a,extend=True))
+            sattr =  (attribute or '').lower()
+            k.LOCALS.update({
+                    'attr': sattr,
+                    'attribute': sattr,
+                    'device':sattr.rsplit('/',1)[0],
+                    'match':lambda r: xmatch(r,attribute),
+                    'clmatch':xmatch,
+                    'overlap':overlap,
+                    'time2str':time2str,'str2time':str2time,
+                    't2s':time2str,'s2t':str2time,
+                    'start':start,'stop':stop,'now':now,
+                    'begin':start,'end':stop,'NOW':now,
+                    'interval':(start,stop),
+                    'period':(stop-start),
+                    'reader':schema.get('reader',schema.get('api')),
+                    'schema':schema.get('schema'),
+                    'dbname':schema.get('dbname',
+                        schema.get('db_name',schema.get('schema',''))),
+                    })
+            if 'reader' in f:
+                k.getReader(schema.get('schema'))
+            if 'api' in f:
+                k.getApi(schema.get('schema'))
+                
+            #print('In reader.Schemas.checkSchema(%s,%s,%s,%s): %s'
+                #% (schema,attribute,start,stop,f))                
+            #print('(%s)%%(%s)'%(f,[t for t in k.LOCALS.items() if t[0] in f]))
+            try:
+                if not clsearch('(s2t|str2time)',f):
+                    if clsearch(fn.redate,f):
+                        f = fn.clsub(fn.redate,str2time,f)
+                    if clsearch(fn.RAW_TIME,f):
+                        f = fn.clsub(fn.RAW_TIME,str2time,f)
+            except:
+                #traceback.print_exc()
+                pass
+            
+            #print('eval(%s)' % str(f))
+            v = fn.evalX(f,k.LOCALS,k.MODULES)
+            #print('%s(%s)' % (type(v),v))
         except:
-          traceback.print_exc()
-          v =False
-      #print('checkSchema(%s): %s'%(schema,v))
-      return v
+            print('checkSchema(%s,%s) failed!' % (schema,attribute))
+            traceback.print_exc()
+            v = False
+
+        #print('checkSchema(%s): %s'%(schema,v))
+        return v
   
     @classmethod
     def getApi(k,schema):
-        schema = k.getSchema(schema)
-        if schema is not None:
-            api = schema.get('api','PyTangoArchiving.ArchivingAPI')
-            if fun.isString(api): api = k._load_object(api,schema)
-            return api(schema['schema']) if isinstance(api,type) else api
+        if schema == '*':
+            import PyTangoArchiving.reader
+            return PyTangoArchiving.reader.Reader()
+        elif fn.isString(schema):
+            schema = k.getSchema(schema)
+            if schema is not None:
+                api = schema.get('api','PyTangoArchiving.ArchivingAPI')
+                if fn.isString(api): 
+                    api = k._load_object(api,schema)
+                return api(schema['schema']) if isinstance(api,type) else api
+        else:
+            return schema
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/utils.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,57 +28,61 @@
 
 import time,datetime,os,re,traceback,xml,sys,functools
 from random import randrange
 import MySQLdb
 
 TRACE = False
 
-import fandango
+import fandango as fn
 from fandango.db import FriendlyDB
 import fandango.functional as fun
 
 from fandango.functional import ( isString,isSequence,isCallable,
     str2time, str2epoch, clmatch, time2str, epoch2str, now,
-    ctime2time, mysql2time, NaN )
+    ctime2time, mysql2time, NaN, first, last ) # Mandatory imports!!!
 
 from fandango.functional import ( date2time,date2str,mysql2time,ctime2time,
-    time2str,isNumber,clmatch,isCallable )
+    time2str,isNumber,clmatch,isCallable ) # Mandatory imports!!!
 
 import fandango.linos as linos
-from fandango.dicts import SortedDict, CaselessDict
-
+from fandango.dicts import SortedDict, CaselessDict # Mandatory imports!!!
+from fandango.log import printf, Logger
 from fandango.functional import reldiff,absdiff,seqdiff
 from fandango.arrays import decimate_custom,decimate_array
 
+try:
+    DEFAULT_USER = get_free_property('PyTangoArchiving','DEFAULT_USER') or 'manager'
+    DEFAULT_PASS = get_free_property('PyTangoArchiving','DEFAULT_PASS') or ''
+except:
+    DEFAULT_USER = 'manager'
+    DEFAULT_PASS = ''
+
 ###############################################################################
 # Conditional imports to avoid PyTango dependency
 
 try:
     import PyTango
+    from fandango.tango import *
     from fandango.servers import ServersDict
-    from fandango.device import get_matching_attributes,check_device,check_attribute,get_distinct_devices
-    from fandango.device import get_distinct_domains,get_distinct_members, \
-            get_distinct_families,get_distinct_attributes
-    from fandango.device import get_device_host
-    from fandango.tango import parse_tango_model,cast_tango_type
 except:
     PyTango=ServersDict=check_attribute=None 
     
 ###############################################################################    
     
 class FakeAttributeHistory():
     def __init__(self,date,value):
         self.value = value
         self.time = PyTango.TimeVal(date) if not isinstance(date,PyTango.TimeVal) else date
     def __repr__(self): 
         return 'fbHistory(value=%s,time=%s)'%(self.value,self.time)
     
 ###############################################################################    
 
-class CatchedAndLogged(fandango.objects.Decorator):
+
+class CatchedAndLogged(fn.objects.Decorator):
     """
     based on fandango.objects.Cached
     in the future it should replace Catched decorator
     """
     def __init__(self,target=None,log=True,throw=False,default=None):
         self.log = log
         self.throw = throw
@@ -119,20 +123,22 @@
         
     def __get__(self,obj,objtype=None):
         """
         This bounding method will be called only when decorating an
         instance method
         """
         from types import MethodType
-        return MethodType(self,obj,objtype)        
+        if fn.py3:
+            return MethodType(self, obj)
+        else:
+            return MethodType(self, obj, objtype)              
         
 ###############################################################################        
     
 def get_alias_file(schema = ''):
-    from fandango.tango import get_free_property,get_class_property
     if not schema or schema in ('*',''):
         alias_file = get_free_property('PyTangoArchiving','AliasFile')
     else:
         alias_file = get_class_property('%sextractor'%schema,'AliasFile')
         if isSequence(alias_file) and len(alias_file):
             alias_file = alias_file[0]
         if not alias_file:
@@ -145,22 +151,22 @@
     # Reading the Alias file
     # The format of the file will be:
     #   Alias                                   Attribute
     #   sr01/vc/eps-plc-01/sr01_vc_tc_s0112     sr01/vc/eps-plc-01/thermocouples[11]
     alias = CaselessDict()
     if alias_file:
         try:
-            csv = fandango.arrays.CSVArray(alias_file)
+            csv = fn.arrays.CSVArray(alias_file)
             csv.setOffset(1)
             for i in range(csv.size()[0]):
                 line = csv.getd(i)
                 try: alias[line['Alias']] = line['Attribute']
                 except: pass
             if trace: print('%d Attribute alias loaded from %s' % (len(alias),alias_file))
-        except Exception,e:
+        except Exception as e:
             print('Unable to parse AliasFile: %s\n%s'%(alias_file,traceback.format_exc()))
             alias.clear()
     return alias        
         
 ###############################################################################
 # Reporting
 
@@ -169,15 +175,15 @@
     This method returns attribute changes ordered by time (event_list format)
     Attributes can be passed as a list or as a formula (TangoEval) or both. 
     If a formula is available the evaluated value will be added at each row of the list.
     """
     from PyTangoArchiving import Reader
     from fandango import isSequence,isString,TangoEval
     rd = Reader()
-    te = fandango.TangoEval()
+    te = fn.TangoEval()
 
     if isString(attributes) and formula is None:
         try:
             formula = attributes
             attributes = sorted(set('%s/%s'%t[:2] for t in te.parse_variables(formula)))
             if len(attributes)==1: formula = None
         except:
@@ -194,22 +200,48 @@
         cache,parsed = {},te.parse_formula(formula)
         for i,event in enumerate(buffer):
             cache[event[1]] = event[2]
             f = te.eval(parsed,cache) if all(k in cache for k in attributes) else None
             buffer[i] = (event[0],event[1],event[2],f)
             
     return buffer
-                    
+
+def parse_property(name,value):
+    """
+    Parses properties in the format 'name(;|\n)key=value(;|\n)key=value'
+    Used by HDB++ config and archivers
+    """
+    if '\n' in value:
+        value = value.split('\n')
+    elif ';' in value:
+        value = value.split(';')
+    else:
+        value = [value]
+
+    r = {'name': (value.pop(0) if '=' not in value[0] else name) }
+    value = [v.strip().split('=',1) for v in value]
+    r.update((v[0],v[-1]) for v in value)
+
+    return r
+
+WILDCARDS = '^$*+?{\|' #r'[]()
+def is_regexp(seq,wildcards=WILDCARDS):
+    """ 
+    This function is just a hint, use it with care. 
+    This function is an overload of the one in fandango, for convenience
+    """
+    return any(c in wildcards for c in seq)
+    
 def translate_attribute_alias(attribute):
     full = 'tango://' in attribute
     attribute = attribute.replace('tango://','')
     if ':' in attribute.split('/')[0]: 
         attribute = attribute.split('/',1)[-1] #removing tango_host
     if attribute.count('/') in (0,1):
-        dev = fandango.get_device_for_alias(attribute.split('/')[0]) or ''
+        dev = fn.get_device_for_alias(attribute.split('/')[0]) or ''
         attribute = dev if '/' not in attribute else dev+'/'+attribute.split('/')[1]
     if attribute.count('/') == 2: 
         if any(attribute.lower().startswith(s+'/') for s in ('ioregister','pc','expchan',)):
             attribute+='/value'
         elif any(attribute.lower().startswith(s+'/') for s in ('motor','mg','pm',)):
             attribute+='/position'
         else:
@@ -227,26 +259,42 @@
     if fun.isSequence(v): 
        return list
     if fun.isBool(v): 
        return bool
     if any(s in str(type(v).__name__.lower()) for s in ('int','short','long')):
        return int
     return float
+
+def get_attribute_type_table(attribute):
+    try:
+        ttype,fformat,rread = fn.tango.get_attribute_info(attribute)[0][:3]
+        fformat = 'scalar' if 'SCALAR' in str(fformat) else 'array'
+        ttype = str(ttype).lower()
+        rread = 'rw' if 'WRITE' in str(rread) else 'ro'
+        r = 'att_%s_%s_%s' % (fformat,ttype,rread)
+        #print('%s => %s' % (attribute,r))
+    except Exception as e:
+        traceback.print_exc()
+        r = ''
+        raise e
+    return r
+        
+    
   
 def get_only_scalar_attributes(model,exclude_strings=True):
     """
     This method will filter out all attributes that are either Arrays or Strings.
     Model can be a device name, a regexp expression or a list of attributes.
     """
     if fun.isSequence(model):
         attrs = model
     elif fun.isRegexp(model):
-        attrs = fandango.get_matching_attributes(model)
+        attrs = fn.get_matching_attributes(model)
     else:
-        attrs = fandango.get_matching_attributes(model+'/*')
+        attrs = fn.get_matching_attributes(model+'/*')
     
     exclude = [list] + ([str] if exclude_strings else [])
     return [a for a in attrs if get_attribute_pytype(a) not in exclude]
     
 
 ###############################################################################
 
@@ -255,32 +303,142 @@
 
 ###############################################################################
 # Decimation/Conversion methods
 
 isNaN = lambda f: 'nan' in str(f).lower()
 RULE_LAST = lambda v,w: sorted([v,w])[-1]
 RULE_MAX = lambda v,w: (max((v[0],w[0])),max((v[1],w[1])))
-START_OF_TIME = time.time()-10*365*24*3600 #Archiving reading limited to last 10 years.
-MAX_RESOLUTION = 10*1080.
+START_OF_TIME = str2time('2001-01-01') #time.time()-20*365*24*3600 #Archiving reading limited to last 20 years.
+MAX_RESOLUTION = 2*1080.
+MAX_QUERY_ROWS = 10e6
+
+def overlap(int1,int2):
+    """
+    returns whether two date intervals overlap
+    both intervals should be tuples of dates (start,stop)
+    """
+    int1,int2 = map(str2time,int1),map(str2time,int2)
+    if int1[0] < int2[0] < int1[1]:
+        return True
+    elif int1[0] < int2[1] < int1[1]:
+        return True
+    elif int2[0] < int1[0] < int2[1]:
+        return True
+    elif int2[0] < int1[1] < int2[1]:
+        return True
+    else:
+        return False
+
+def get_days_in_interval(*args):
+    """
+    args may be a list of timestamps or just start,stop dates
+    """
+    if len(args)==2:
+        if fun.isString(args[0]):
+            start,stop = str2time(args[0]),str2time(args[1])
+        else:
+            start,stop = args[0],args[1]
+        times = range(int(start),int(stop+86400),86400)
+    else:
+        times = args[0]
+    days = sorted(set(list(d.split()[0] for d in map(time2str,times))))
+    return days
+
+def get_months_in_interval(*args):
+    """
+    args may be a list of timestamps or just start,stop dates
+    """
+    days = get_days_in_interval(*args)
+    return sorted(set(d.rsplit('-',1)[0]+'-01' for d in days))
+
+def get_next_month(date):
+    if not fun.isString(date):
+        date = time2str(date)
+    year,month,day = map(int,date.split()[0].split('-'))
+    if month<12:
+        return '%04d-%02d-%02d' % (year,month+1,1)
+    else:
+        return '%04d-%02d-%02d' % (year+1,1,1)
+
+def split_interval_in_months(start,stop,cut=True):
+    """
+    returns a list of start,stop tuples for each month in the interval
+    if cut is True, then first and last interval are adjusted to start,stop
+    """
+    
+    months = get_months_in_interval(start,stop)
+    months.append(get_next_month(months[-1]))
+    months = zip(months,months[1:])
+    months = list(list((str2time(b),str2time(e)-1)) for b,e in months)
+    if cut:
+        months[0][0],months[-1][-1] = start,stop
+    return months
 
-def get_jumps(values):
-    jumps = [(values[i][0],values[i+1][0]) for i in range(len(values)-1) if 120<(values[i+1][0]-values[i][0])]
-    return [[time.ctime(d) for d in j] for j in jumps]
+def split_interval(start,stop,jump):
+    starts = range(int(start),int(stop),int(jump))
+    print(starts)
+    return [(s,starts[i+1]) for i,s in enumerate(starts[:-1])]
+    
+#def get_jumps(values):
+    #"""
+    ###DEPRECATED by get_gaps
+    #return time in ctime format whenever two points are separated 
+    #for more than 2 minutes
+    #"""
+    #jumps = [(values[i][0],values[i+1][0]) for i in range(len(values)-1) 
+             #if 120<(values[i+1][0]-values[i][0])]
+    #return [[time.ctime(d) for d in j] for j in jumps]
+
+def get_gaps(values, min_gap=5*24*3600, start=None, stop=None):
+    """
+    return time intervals in buffer where time distance is bigger than min_gap
+    """
+    if start and stop and not len(values):
+        print('get_gaps, no values in interval')
+        return [(start,stop)]
+    elif not any((len(values),start,stop)):
+        print('get_gaps, no values')
+        return []        
+        
+    gaps = [(values[i][0],v[0]) for i,v in enumerate(values[1:])
+                if min_gap < (v[0]-values[i][0])]
+    
+    if start and values[0][0] >  start + min_gap:
+        gaps.insert(0,(start,values[0][0]))
+    if stop and values[-1][0] < stop - min_gap:
+        gaps.append((values[-1][0],stop))
+    
+    return gaps
+
+def get_density(values):
+    """
+    returns the number of values/second (expanding arrays)
+    """
+    if not len(values):
+        return 0
+    t0 = values[0][0]
+    t1 = values[-1][0]
+    if t0==t1:
+        return 1
+    v = fun.first((v[1] for v in values if v[1] is not None),default=None)
+    if fun.isSequence(v):
+        return len(values)*len(v)/(t1-t0)
+    return len(values)/(t1-t0)
 
 def get_failed(values):
     i,failed = 0,[]
     while i<len(values)-1:
         if not isNaN(values[i][1]) and isNaN(values[i+1][1]):
-            print 'found error at %s' % time.ctime(values[i+1][0])
+            print('found error at %s' % time.ctime(values[i+1][0]))
             try:
-                next = (j for j in range(i+1,len(values)) if not isNaN(values[j][1])).next()
-                failed.append((values[i][0],values[i+1][0],values[next][0]))
-                i=next
+                nxt = (j for j in range(i+1,len(values)) if not isNaN(values[j][1])).__next__()
+                failed.append((values[i][0],values[i+1][0],values[nxt][0]))
+                i = nxt
             except StopIteration: #Unable to find the next valid value
-                print 'no more values found afterwards ...'
+                print('no more values found afterwards ...')
                 failed.append((values[i][0],values[i+1][0],-1))
                 break
         i+=1
     return [[time.ctime(d) for d in j] for j in failed]
         
 def data_has_changed(val,prv,nxt=None,t=300):
     """ 
@@ -288,84 +446,94 @@
     any value that preceeds a change is considered a change
     any time increment above 300 seconds is considered a change
     """
     return (val[1]!=prv[1] 
                     or (nxt is not None and nxt[1]!=prv[1]) 
                     or val[0]>(prv[0]+t))
 
-def decimation(history,method,window='0',logger_obj=None, N=1080):
+def decimation(history,method,window='0',logger_obj=None, N=MAX_RESOLUTION):
     """
     Nones and NaNs are always removed if this method is called
     
     history: array of data
-    method: method or callable
+    method: method, callable or interval, from fn.arrays
     window: string for time
     logger_obj: ArchivedTrendLogger or similar
     N: max array size to return
     """
     t0 = time.time()
     l0 = len(history)
     if not l0:
         return history
     
-    trace = getattr(logger_obj,'warning',fandango.printf)
-    try: 
-        window = str2time(window or '0') 
+    trace = getattr(logger_obj,'warning',fn.printf)
+    try:
+        if not isinstance(window,(int,float)):
+            window = str2time(window or '0') 
     except: 
         window = 0
+
+    if isNumber(method) and not window:
+        method, window = fn.arrays.pickfirst, float(method)
         
     start_date,stop_date = float(history[0][0]),float(history[-1][0])
 
     ## Decimation by data_has_changed is ALWAYS done
     if len(history): #method is not None
         nv = []
         #sq = isSequence(history[0][1])
         for i,v in enumerate(history):
             if (v[1] not in (None,NaN)# is not None and (sq or not isNaN(v[1]))
-                    #and (i in (0,l0-1,l0-2) or 
-                        #data_has_changed(history[i-1],v,history[i+1]))
+                    and (i in (0,l0-1,l0-2) or 
+                        data_has_changed(history[i-1],v,history[i+1]))
                     ):
                 nv.append(v)
         t1 = time.time()
-        trace('Removed %d (None,NaN, Rep) values in %fs'
+        if l0!=len(nv):
+            trace('Removed %d repeated values in %fs'
               %(l0-len(nv),t1-t0))
 
         t0,i,c,lh = t1,0,0,len(history)
         while i<len(history):
             if history[c] in (None,NaN):
                 history.pop(c)
             else:
                 c+=1
             i+=1
         t1 = time.time()
-        trace('Removed %d (None,NaN, Rep) values in %fs'
+        if l0!=len(history):
+            trace('Removed %d (None,NaN) values in %fs'
               %(l0-len(history),t1-t0))
         history = nv   
         
-    if (method and isCallable(method) and method!=data_has_changed 
-        and len(history) and type(history[0][-1]) in (int,float,bool)): #type(None)):
+    if (method and isCallable(method) and len(history)):
         # Data is filtered applying an averaging at every "window" interval.
         # As range() only accept integers the minimum window is 1 second.
         # It means that filtering 3 hours will implicitly prune millis data.        
-        #DATA FROM EVAL IS ALREADY FILTERED; SHOULD NOT PASS THROUGH HERE        
+        #DATA FROM EVAL IS ALREADY FILTERED; SHOULD NOT PASS THROUGH HERE
         
-        wmin = max(1.,(stop_date-start_date)/(10*1080.))
+        if type(history[0][-1]) not in (int,float,bool):
+            method = fn.arrays.pickfirst
+            trace('Decimation forced to %s' % method)
+        
+        wmin = max(1.,(stop_date-start_date)/(2*MAX_RESOLUTION))
         wauto = max(1.,(stop_date-start_date)/(10*N))
         trace('WMIN,WUSER,WAUTO = %s,%s,%s'%(wmin,window,wauto))
         window = wauto if not window else max((wmin,window))
         
-        if len(history) > (stop_date-start_date)/window:
-            history = fandango.arrays.filter_array(
+        if len(history) > float(stop_date-start_date)/window:
+            history = fn.arrays.filter_array(
                 data=history,window=window,method=method)
             t2 = time.time()
             trace('Decimated %d values to %d in %f seconds '
                   '(%s,%s)'
                   %(l0,len(history),t2-t1,method,window))
     else:
-        trace('Decimation is not callable')
+        #trace('Decimation(%s) is not callable' % method)
+        pass
             
     return history
 
 def choose_first_value(v,w,t=0,tmin=-300):
     """ 
     Args are v,w for values and t for point to calcullate; 
     tmin is the min epoch to be considered valid
@@ -441,28 +609,77 @@
     82,
     '24.3, 22.6, 21.7, 21.4, 19.4, 20.9, 20.1, 20.7, 21.8, 21.5, 20.3, 19.1, 19.8, 20.0, 20.2, 20.0, 20.1, 19.4, 20.0, 20.6, 20.8, 19.8, 19.8, 19.0, 19.7, 20.4, 21.1, 20.4, 20.2, 18.7, 20.3, 20.5, 20.4, 20.2, 21.0, 19.2, 20.6, 19.8, 20.8, 20.3, 21.5, 20.0, 19.8, 19.0, 19.3, 20.4, 20.0, 19.9, 19.7, 18.6, 19.2, 20.5, 20.6, 20.5, 19.2, 20.1, 19.4, 20.5, 20.7, 19.4, 19.8, 19.0, 19.9, 20.1, 20.7, 20.1, 21.6, 20.6, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0'))
 DevState
     (datetime.datetime(2013, 1, 11, 18, 9, 41), 3.0),
 """    
 
 def h_to_tuple(T):
-    return (T.time.tv_sec,T.value if not hasattr(T.value,'__len__') else tuple(T.value)) #if data_format == PyTango.AttrDataFormat.SPECTRUM:
+    #if data_format == PyTango.AttrDataFormat.SPECTRUM:
+    return (T.time.tv_sec,T.value if not hasattr(T.value,'__len__') 
+            else tuple(T.value)) 
+
 def get_mysql_value(v):
-    return (mysql2time(v[0]),v[1 if len(v)<4 else 2]) #Date and read value (excluding dimension?!?)
+    #Date and read value (excluding dimension?!?)
+    return (mysql2time(v[0]),v[1 if len(v)<4 else 2]) 
+
 def listToHistoryBuffer(values):
     return [FakeAttributeHistory(*v) for v in values]
+
 def mysql2array(v,data_type,default=None):
-    #lambda v: [(s.strip() and data_type(s.strip()) or (0.0 if data_type in (int,float) else None)) for s in str(v[1]).split(',')]
-    return [data_type(x) if x else default for x in map(str.strip,str(v).split(','))]
+    #lambda v: [(s.strip() and data_type(s.strip()) 
+    #  or (0.0 if data_type in (int,float) else None)) 
+    #  for s in str(v[1]).split(',')]
+    return [data_type(x) if x else default 
+            for x in map(str.strip,str(v).split(','))]
+
 def mysql2bool(v):
     v = str(v)
     if v in ('','None','none','null','NULL'): return None 
     if v in ('1','1.0','True','true'): return 1 
     return 0
 
+        
+def extract_array_index(values,array_index,decimate=False,asHistoryBuffer=False):
+    """
+    Applying array_index to the obtained results, it has to be applied after 
+    attribute loading to allow reusing cache in array-indexed attributes
+    
+    decimate is just evaluated as True/False
+    """
+    last,l0 = (0,None),len(values)
+    
+    # Check if it has been already parsed
+    for r in values:
+        if r[1] is not None:
+            if not fn.isSequence(r[1]):
+                return values
+            break
+    
+    #print('extract_array_index(%s) to the obtained results'%array_index)
+    array_index = int(array_index)
+    new_values = [] # We create a new list on purpose to not modify the cached values
+    fin = ((lambda v: (v.time,v.value[array_index] if v.value is not None and len(v.value)>array_index else None)) 
+            if asHistoryBuffer else 
+                (lambda v: (v[0],v[1][array_index] if v[1] is not None and len(v[1])>array_index else None)))
+    fcmp = (lambda l: (l[0].tv_sec,l[1])) if asHistoryBuffer else (lambda l: l)
+    fout = (lambda vv: FakeAttributeHistory(*(vv))) if asHistoryBuffer else (lambda vv: vv)
+    for i,v in enumerate(values):
+        try:
+            if v is None: continue
+            vv = fin(v)
+            nxt = ((values[i+1] and fin(values[i+1]) or None) if i+1<l0 else None)
+            if not decimate or nxt is None or not new_values or data_has_changed(fcmp(vv),fcmp(last),fcmp(nxt)):
+                new_values.append(fout(vv))
+                last = vv
+        except Exception as e:
+            print('extract_array_index(...,asHistoryBuffer=%s): Unable to parse %d[%s]:(%s); %s'%(asHistoryBuffer,i,array_index,v,traceback.format_exc()))
+    if decimate:
+        print('\tIn extract_array_index(...).raw: decimated repeated values in spectrum ... %s -> %s'%(l0,len(new_values)))
+    return new_values
+
 
 ###############################################################################
 # Numpy based methods for decimation/filtering
             
 def to_array(l):
     """
     returns l as a numpy array; replacing None values by NaN
@@ -507,15 +724,15 @@
         sdata = data.take(time_index,0)
         if decimate:
             sdata = np.compress(
                 get_array_steps(get_col(sdata,0), 
                                 minstep = minstep, as_index = as_index),
                                 sdata,0)
             
-        print time.time()-t0
+        print(time.time()-t0)
         return sdata
     
 def get_array_steps(array,minstep=0.001,as_index=False):
     # Gets an integer with all differences > minstep
     # It calcullates steps and adds True at the beginning
     as_index = False
     print('get_array_steps(%s,%s,%s)'%(len(array),minstep,as_index))
@@ -583,15 +800,15 @@
         #try:
             ### But this step crashes with nans!!
             #diff1 = np.insert(np.abs(vs[:-1]-vs[1:])>diff,0,True) #Different from next value
             #diff2 = np.append(np.abs(vs[1:]-vs[:-1])>diff,True) #Different from previous value
         #except TypeError,e:
             #diff1 = np.insert(np.abs(vs[:-1]!=vs[1:]),0,True)
             #diff2 = np.append(np.abs(vs[1:]!=vs[:-1]),True)
-        ##print 'diff1,diff2,nans: %d,%d,%d'%tuple(len(np.nonzero(a)[0]) for a in (diff1,diff2,nans))
+        ##print('diff1,diff2,nans: %d,%d,%d'%tuple(len(np.nonzero(a)[0]) for a in (diff1,diff2,nans)))
         #array = array[diff1|diff2|nans]
     #return array
         
 def patch_booleans(history,trace=TRACE):
     if trace: 
         print('In patch_booleans(%d,%s)'%(len(history),(history or ('',))[0]))
     fromHistoryBuffer = len(history) and hasattr(history[0],'time')
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving/web.py` & `PyTangoArchiving-9.2.5/PyTangoArchiving/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,20 +83,20 @@
         except:
             raise Exception('Unknown data source!')
     else:
         raise Exception('Unknown data source!')
     
     if begin:
         try:
-            i = (i for i,t in enumerate(vals) if t[0]>=begin).next()
+            i = (i for i,t in enumerate(vals) if t[0]>=begin).__next__()
             vals = vals[i:]
         except: pass
     if end:
         try:
-            i = (i for i,t in enumerate(vals) if t[0]>=end).next()
+            i = (i for i,t in enumerate(vals) if t[0]>=end).__next__()
             vals = vals[:i]
         except: pass
     
     if decimate:
         if len(vals)>MAX_DATA_SIZE:
             vals = decimate_array(vals,fixed_size=MAX_DATA_SIZE,fixed_rate=100)
         
@@ -112,15 +112,15 @@
         <script type="text/javascript" src="$JS/plugins/jqplot.dateAxisRenderer.min.js"></script>
         <link rel="stylesheet" type="text/css" href="$JS/jquery.jqplot.css" />
         """.replace('$JS',JS_PATH)
 
 def jqplot(title,vals,y2vals=None,xvals=None):
     #USING jqPlot instead of Qt
     ats = sorted(vals.keys())
-    print 'JQPlot(%s,%s)'%(len(ats),','.join(ats))
+    print('JQPlot(%s,%s)'%(len(ats),','.join(ats)))
     js = JS_PATH
     includes = JS_INCLUDES
     jqplot = """
         <div id="chartdiv" style="height:100%;width:100%; "></div>
         <script class="code" type="text/javascript">
         //var line1=[['2008-08-12 4:00',4], ['2008-09-12 4:00',6.5], ['2008-10-12 4:00',5.7], ['2008-11-12 4:00',9], ['2008-12-12 4:00',8.2]];
         //var line1 = [['2012-09-17 16:44', -0.24086535644531001], ['2012-09-17 16:44', -0.166169769287108], ['2012-09-17 16:45', -0.097435409545898494]];
@@ -198,15 +198,15 @@
     data = str([
         list([fandango.time2str(t[0]),t[1]] for t in vals[k]) for k in ats]
         )
     return jqplot.replace('$DATA',data).replace('$SERIES',series).replace('$TITLE',title)
 
 if __name__=='__main__':
     args = sys.argv[1:]
-    filename = (a for a in args if 'html' in a).next()
+    filename = (a for a in args if 'html' in a).__next__()
     title = ([a.split('=',1)[-1] for a in args if a.startswith('--title=')] or ['Data Report'])[0]
     model = [a for a in args if not a.startswith('--') and not a.endswith('.html')]
     vals = dict((get_varname(m) or m,get_plotable_values(m,decimate=False)) for m in model)
     for k in vals.keys():
         if not vals[k]: vals.pop(k)
     print('Writing %s report ...'%filename)
     f = open(filename,'w')
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving.egg-info/PKG-INFO` & `PyTangoArchiving-9.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyTangoArchiving
-Version: 8.5.2
+Version: 9.2.5
 Summary: Python bindings for Tango Control System Archiving
 Home-page: UNKNOWN
 Author: Sergi Rubio
 Author-email: srubio@cells.es
 License: GPL-3.0
 Description: This package allows to: 
         * Integrate Hdb and Snap archiving with other python/PyTango tools.
```

### Comparing `PyTangoArchiving-8.5.2/PyTangoArchiving.egg-info/SOURCES.txt` & `PyTangoArchiving-9.2.5/PyTangoArchiving.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,82 @@
 AUTHORS
-CHANGES
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
+./PyTangoArchiving/scripts/PyExtractor
 ./PyTangoArchiving/scripts/archiving2csv
 ./PyTangoArchiving/scripts/archiving2plot
 ./PyTangoArchiving/scripts/archiving_service
 ./PyTangoArchiving/scripts/ctarchiving
-./PyTangoArchiving/scripts/ctsnaps
 ./PyTangoArchiving/scripts/taurusfinder
 PyTangoArchiving/VERSION
 PyTangoArchiving/__init__.py
 PyTangoArchiving/archiving.py
 PyTangoArchiving/check.py
 PyTangoArchiving/common.py
 PyTangoArchiving/dbs.py
 PyTangoArchiving/files.py
 PyTangoArchiving/reader.py
 PyTangoArchiving/schemas.py
-PyTangoArchiving/snap.py
-PyTangoArchiving/tests.py
 PyTangoArchiving/utils.py
 PyTangoArchiving/web.py
 PyTangoArchiving.egg-info/PKG-INFO
 PyTangoArchiving.egg-info/SOURCES.txt
 PyTangoArchiving.egg-info/dependency_links.txt
 PyTangoArchiving.egg-info/entry_points.txt
 PyTangoArchiving.egg-info/not-zip-safe
 PyTangoArchiving.egg-info/requires.txt
 PyTangoArchiving.egg-info/top_level.txt
 PyTangoArchiving/hdbpp/__init__.py
+PyTangoArchiving/hdbpp/alter_datetime.sql
+PyTangoArchiving/hdbpp/api.py
+PyTangoArchiving/hdbpp/check_and_recover_attributes.py
 PyTangoArchiving/hdbpp/config.py
-PyTangoArchiving/hdbpp/create_partitions.py
+PyTangoArchiving/hdbpp/create_hdb++_mysql.sql
+PyTangoArchiving/hdbpp/create_hdbpp_devices.py
 PyTangoArchiving/hdbpp/decimate.py
+PyTangoArchiving/hdbpp/maintenance.py
 PyTangoArchiving/hdbpp/multi.py
-PyTangoArchiving/hdbpp/read.py
+PyTangoArchiving/hdbpp/periodic.py
+PyTangoArchiving/hdbpp/privileges.sh
+PyTangoArchiving/hdbpp/privileges.sql
+PyTangoArchiving/hdbpp/query.py
+PyTangoArchiving/hdbpp/subscribe_attributes.py
+PyTangoArchiving/scripts/THIS_FOLDER_SHOULD_NOT_HAVE__init.py
+PyTangoArchiving/scripts/__init__.py
+PyTangoArchiving/scripts/alter_snap_db.py
+PyTangoArchiving/scripts/archiver_health_check.py
+PyTangoArchiving/scripts/archiving_load.py
+PyTangoArchiving/scripts/archiving_report.py
+PyTangoArchiving/scripts/archiving_transfer.py
+PyTangoArchiving/scripts/check_db_growth.py
+PyTangoArchiving/scripts/check_partitions.py
+PyTangoArchiving/scripts/db_repair.py
+PyTangoArchiving/scripts/decimate_table.py
+PyTangoArchiving/scripts/inspect_hdbpp_hosts.py
+PyTangoArchiving/scripts/start_hdbpp_archivers.py
 PyTangoArchiving/servers/__init__.py
 PyTangoArchiving/servers/PyExtractor/PyExtractor.py
 PyTangoArchiving/servers/PyExtractor/__init__.py
+PyTangoArchiving/servers/SchemaManager/SchemaManager.py
+PyTangoArchiving/servers/SchemaManager/__init__.py
 PyTangoArchiving/widget/ArchivingBrowser.py
 PyTangoArchiving/widget/__init__.py
 PyTangoArchiving/widget/dialogs.py
 PyTangoArchiving/widget/history.py
 PyTangoArchiving/widget/models.py
 PyTangoArchiving/widget/panel.py
 PyTangoArchiving/widget/progress.py
 PyTangoArchiving/widget/resources.py
+PyTangoArchiving/widget/resources.qrc
 PyTangoArchiving/widget/taurusattributechooser.py
 PyTangoArchiving/widget/tdbwidget.py
 PyTangoArchiving/widget/tests.py
+PyTangoArchiving/widget/tpgarchivingwidget.py
 PyTangoArchiving/widget/tree.py
 PyTangoArchiving/widget/trend.py
-PyTangoArchiving/widget/snaps/__init__.py
-PyTangoArchiving/widget/snaps/contexttoolbar.py
-PyTangoArchiving/widget/snaps/snapbutton.py
-PyTangoArchiving/widget/snaps/snapdialogs.py
-PyTangoArchiving/widget/snaps/snaps.py
-PyTangoArchiving/widget/snaps/toolbar.py
-PyTangoArchiving/widget/snaps/ui/__init__.py
-PyTangoArchiving/widget/snaps/ui/core.py
-PyTangoArchiving/widget/snaps/ui/diff.py
-PyTangoArchiving/widget/snaps/ui/modify.py
+PyTangoArchiving/widget/resources/add.png
+PyTangoArchiving/widget/resources/open.png
+PyTangoArchiving/widget/resources/save.png
 PyTangoArchiving/widget/ui/TaurusAttributeChooser.ui
 PyTangoArchiving/widget/ui/__init__.py
```

### Comparing `PyTangoArchiving-8.5.2/LICENSE` & `PyTangoArchiving-9.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTangoArchiving-8.5.2/README.rst` & `PyTangoArchiving-9.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `PyTangoArchiving-8.5.2/setup.py` & `PyTangoArchiving-9.2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # Always prefer setuptools over distutils
-import os, imp
+import os, imp, sys
 from setuptools import setup, find_packages
 
 __doc__ = """
 
 To install as system package:
 
   python setup.py install
@@ -20,58 +20,61 @@
   RU=/opt/control
   python setup.py egg_info --egg-base=tmp install --root=$RU/files --no-compile \
     --install-lib=lib/python/site-packages --install-scripts=ds
 
 -------------------------------------------------------------------------------
 """
 
-print(__doc__)
+if 'help' in str(sys.argv):
+  print(__doc__)
+
+with open('PyTangoArchiving/VERSION') as f:
+  __version = f.read().strip()
 
-version = open('PyTangoArchiving/VERSION').read().strip()
 scripts = []
 license = 'GPL-3.0'
 
 f = './PyTangoArchiving/scripts/'
 scripts = [
 f+'taurusfinder',
 f+'ctarchiving',
-f+'ctsnaps',
 f+'archiving2csv',
 f+'archiving2plot',
 #f+'archiving_report.py',
 f+'archiving_service',
+f+'PyExtractor',
 #f+'archiver_health_check.py',
 #f+'cleanTdbFiles',
 #f+'db_repair.py',
 ]
 
 entry_points = {
         'console_scripts': [
-            #'CopyCatDS = PyTangoArchiving.interface.CopyCatDS:main',
+            #'PyExtractor = PyTangoArchiving.servers.PyExtractor.PyExtractor',
         ],
 }
 
 # EXTRA FILES ARE ADDED IN MANIFEST.in, not here
 
-#package_data = {
-#    'PyTangoArchiving': [#'VERSION','README',
-#         './VERSION',
+package_data = {
+    'PyTangoArchiving': [#'VERSION','README',
+         './VERSION',
          #'./CHANGES',
 #         './widget/ui/TaurusAttributeChooser.ui',
          #'./widget/resources/*',
          #'./widget/resources.qrc',
          #'./widget/snaps/ui/*',
          #'./widget/snaps/doc/snapimg/*png',
          #'./widget/snaps/README',
-#         ],
-#}
+         ],
+}
 
 setup(
     name="PyTangoArchiving",
-    version=str(version),
+    version=__version,
     license=license,
     packages=find_packages(),
     description="Python bindings for Tango Control System Archiving",
     long_description="This package allows to: \n"
     "* Integrate Hdb and Snap archiving with other python/PyTango tools.\n"
     "* Start/Stop Archiving devices in the appropiated order.\n"
     "* Increase the capabilities of configuration and diagnostic.\n"
@@ -91,10 +94,10 @@
         'Topic :: Software Development :: Libraries',
     ],
     platforms=[ "Linux" ],
     scripts=scripts,
     entry_points=entry_points,
     include_package_data=True,
     #package_data=package_data,
-    install_requires=['fandango','PyTango','MySQL-python'],
+    install_requires=['fandango>=14.6.0','PyTango'],
     zip_safe=False
   )
```

### Comparing `PyTangoArchiving-8.5.2/PKG-INFO` & `PyTangoArchiving-9.2.5/PyTangoArchiving.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyTangoArchiving
-Version: 8.5.2
+Version: 9.2.5
 Summary: Python bindings for Tango Control System Archiving
 Home-page: UNKNOWN
 Author: Sergi Rubio
 Author-email: srubio@cells.es
 License: GPL-3.0
 Description: This package allows to: 
         * Integrate Hdb and Snap archiving with other python/PyTango tools.
```

