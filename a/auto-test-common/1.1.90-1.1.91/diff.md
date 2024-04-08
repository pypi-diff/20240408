# Comparing `tmp/auto-test-common-1.1.90.tar.gz` & `tmp/auto-test-common-1.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-1.1.90.tar", last modified: Fri Mar 29 08:52:39 2024, max compression
+gzip compressed data, was "auto-test-common-1.1.91.tar", last modified: Mon Apr  8 03:28:51 2024, max compression
```

## Comparing `auto-test-common-1.1.90.tar` & `auto-test-common-1.1.91.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.617162 auto-test-common-1.1.90/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-03-29 08:52:39.617277 auto-test-common-1.1.90/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.598222 auto-test-common-1.1.90/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-03-29 08:52:39.000000 auto-test-common-1.1.90/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1726 2024-03-29 08:52:39.000000 auto-test-common-1.1.90/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-03-29 08:52:39.000000 auto-test-common-1.1.90/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-03-29 08:52:39.000000 auto-test-common-1.1.90/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      653 2024-03-29 08:52:39.000000 auto-test-common-1.1.90/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-03-29 08:52:39.000000 auto-test-common-1.1.90/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.598547 auto-test-common-1.1.90/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.90/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.599784 auto-test-common-1.1.90/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.90/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11452 2024-03-26 09:07:48.000000 auto-test-common-1.1.90/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.90/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.90/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.601093 auto-test-common-1.1.90/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.90/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5492 2024-03-20 02:00:33.000000 auto-test-common-1.1.90/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.90/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.90/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.601634 auto-test-common-1.1.90/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.90/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.90/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.604757 auto-test-common-1.1.90/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.90/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    24668 2024-03-26 09:07:48.000000 auto-test-common-1.1.90/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)    11059 2024-03-26 08:31:29.000000 auto-test-common-1.1.90/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.90/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.606750 auto-test-common-1.1.90/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.90/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.90/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.90/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.90/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.90/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.90/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.90/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.607693 auto-test-common-1.1.90/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.90/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.90/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.90/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.609988 auto-test-common-1.1.90/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.90/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.90/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.90/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.90/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.90/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2355 2024-01-08 05:26:01.000000 auto-test-common-1.1.90/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.90/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.610499 auto-test-common-1.1.90/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.90/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.90/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.612224 auto-test-common-1.1.90/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.90/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.90/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.90/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.90/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.90/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.90/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-03-29 08:52:39.616873 auto-test-common-1.1.90/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.90/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.90/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.90/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10535 2024-03-28 06:14:38.000000 auto-test-common-1.1.90/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.90/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.90/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    12350 2024-03-20 05:29:19.000000 auto-test-common-1.1.90/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.90/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.90/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.90/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.90/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.90/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.90/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      444 2024-03-29 08:52:39.617894 auto-test-common-1.1.90/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.90/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.739527 auto-test-common-1.1.91/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-08 03:28:51.739667 auto-test-common-1.1.91/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.685574 auto-test-common-1.1.91/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-08 03:28:51.000000 auto-test-common-1.1.91/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-08 03:28:51.000000 auto-test-common-1.1.91/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-08 03:28:51.000000 auto-test-common-1.1.91/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-08 03:28:51.000000 auto-test-common-1.1.91/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-08 03:28:51.000000 auto-test-common-1.1.91/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-08 03:28:51.000000 auto-test-common-1.1.91/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.685944 auto-test-common-1.1.91/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.91/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.689392 auto-test-common-1.1.91/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.91/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11452 2024-03-26 09:07:48.000000 auto-test-common-1.1.91/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.91/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.91/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.693366 auto-test-common-1.1.91/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.91/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7097 2024-04-08 00:59:41.000000 auto-test-common-1.1.91/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.91/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.91/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.694541 auto-test-common-1.1.91/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.91/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.91/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.701731 auto-test-common-1.1.91/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.91/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    24668 2024-03-26 09:07:48.000000 auto-test-common-1.1.91/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)    11059 2024-03-26 08:31:29.000000 auto-test-common-1.1.91/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.91/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.708582 auto-test-common-1.1.91/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.91/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.91/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.91/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.91/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.91/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.91/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.91/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.710329 auto-test-common-1.1.91/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.91/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.91/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.91/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.716636 auto-test-common-1.1.91/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.91/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.91/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.91/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.91/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.91/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2355 2024-01-08 05:26:01.000000 auto-test-common-1.1.91/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.91/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.717747 auto-test-common-1.1.91/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.91/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.91/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.725133 auto-test-common-1.1.91/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.91/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.91/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.91/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.91/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.91/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.91/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-08 03:28:51.738474 auto-test-common-1.1.91/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.91/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.91/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.91/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.91/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.91/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.91/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    12350 2024-03-20 05:29:19.000000 auto-test-common-1.1.91/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.91/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.91/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.91/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.91/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.91/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.91/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-08 03:28:51.740443 auto-test-common-1.1.91/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.91/setup.py
```

### Comparing `auto-test-common-1.1.90/PKG-INFO` & `auto-test-common-1.1.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.90
+Version: 1.1.91
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.90/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-1.1.91/auto_test_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.90
+Version: 1.1.91
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.90/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-1.1.91/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/auto_test_common.egg-info/requires.txt` & `auto-test-common-1.1.91/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/autotest/base_requests.py` & `auto-test-common-1.1.91/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/autotest/handle_allure.py` & `auto-test-common-1.1.91/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/autotest/handle_assert.py` & `auto-test-common-1.1.91/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/common/constant.py` & `auto-test-common-1.1.91/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/common/test.py` & `auto-test-common-1.1.91/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/config/config.py` & `auto-test-common-1.1.91/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/data/data_process.py` & `auto-test-common-1.1.91/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/data/handle_common.py` & `auto-test-common-1.1.91/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/data/template_data.py` & `auto-test-common-1.1.91/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/db/handle_db.py` & `auto-test-common-1.1.91/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/db/handle_db_batch.py` & `auto-test-common-1.1.91/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/db/handle_mongo.py` & `auto-test-common-1.1.91/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/db/handle_mysqldb.py` & `auto-test-common-1.1.91/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/db/handle_oracle.py` & `auto-test-common-1.1.91/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/db/handle_sqlserver.py` & `auto-test-common-1.1.91/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/driver/ui_page.py` & `auto-test-common-1.1.91/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/file/ReadFile.py` & `auto-test-common-1.1.91/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/file/handle_excel.py` & `auto-test-common-1.1.91/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/file/handle_file.py` & `auto-test-common-1.1.91/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/file/handle_reques.py` & `auto-test-common-1.1.91/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/file/handle_system.py` & `auto-test-common-1.1.91/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/file/handle_yaml.py` & `auto-test-common-1.1.91/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/mq/handle_rabbit.py` & `auto-test-common-1.1.91/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plat/ATF_platform.py` & `auto-test-common-1.1.91/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plat/jenkin_platform.py` & `auto-test-common-1.1.91/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plat/jira_platform.py` & `auto-test-common-1.1.91/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plat/mysql_platform.py` & `auto-test-common-1.1.91/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plat/service_platform.py` & `auto-test-common-1.1.91/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plugin/allure_plugin.py` & `auto-test-common-1.1.91/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plugin/assert_plugin.py` & `auto-test-common-1.1.91/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plugin/atf_plugin.py` & `auto-test-common-1.1.91/common/plugin/atf_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,45 +7,48 @@
 from loguru import logger
 from common.data.handle_common import get_system_key,print_info,print_debug
 from common.plat.jira_platform import JiraPlatForm
 from common.plugin.data_bus import DataBus
 from common.common.constant import Constant
 from common.plat.ATF_platform import ATFPlatForm
 from common.autotest.handle_allure import allure_step
-from common.db.handle_mongo import MongoDB
 import os
 
 
+
 class ATFPlugin(object):
 
     @classmethod
     def db_ops(self,_key, _sql, env: str = Constant.ENV, des: str = "数据库操作"):
         DataBus.save_init_data()
         allure_step(des,f'SQL语句:{_sql}')
         return ServicePlatForm.db_ops(_key, _sql, env)
 
     @classmethod
     def mongo_db(self,_key,env: str = Constant.ENV):
         """
             返回MongoDB实例
         """
+        from common.db.handle_mongo import MongoDB
         return MongoDB.mongo_db(_key,env)
 
     @classmethod
     def mongo_collection(self, _key, _collection, env: str = Constant.ENV):
         """
             返回MongoDB集合
         """
+        from common.db.handle_mongo import MongoDB
         return MongoDB.mongo_collection(_key, _collection, env)
 
     @classmethod
     def mongo_find(self, _key, _collection, _query, type:str = "", limit:int = 0, _sort:str = "", env: str = Constant.ENV):
         """
             返回查询结果
         """
+        from common.db.handle_mongo import MongoDB
         return MongoDB.mongo_find(_key, _collection, _query, type, limit, _sort, env)
 
     @classmethod
     def sendResult(self, report_html_path: str = TEST_TARGET_REPORT_PATH):
         if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() != '脚本同步':
             DataBus.save_init_data()
             ATFPlatForm.syncCycleBasic()
@@ -203,16 +206,15 @@
 
 
 
 
 
 
 
-if __name__ == '__main__':
-    print(ATFPlugin.mongo_collection('mucem','mucem',env='test'))
+
```

### Comparing `auto-test-common-1.1.90/common/plugin/data_bus.py` & `auto-test-common-1.1.91/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plugin/data_plugin.py` & `auto-test-common-1.1.91/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plugin/file_plugin.py` & `auto-test-common-1.1.91/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plugin/hooks_plugin.py` & `auto-test-common-1.1.91/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plugin/pytest_playwright.py` & `auto-test-common-1.1.91/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plugin/pytest_plugin.py` & `auto-test-common-1.1.91/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plugin/template_plugin.py` & `auto-test-common-1.1.91/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/common/plugin/yaml_plugin.py` & `auto-test-common-1.1.91/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.90/setup.py` & `auto-test-common-1.1.91/setup.py`

 * *Files identical despite different names*

