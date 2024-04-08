# Comparing `tmp/feapder-1.9.0b2.tar.gz` & `tmp/feapder-1.9.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feapder-1.9.0b2.tar", last modified: Tue Nov  7 11:44:38 2023, max compression
+gzip compressed data, was "feapder-1.9.1b1.tar", last modified: Mon Apr  8 04:47:30 2024, max compression
```

## Comparing `feapder-1.9.0b2.tar` & `feapder-1.9.1b1.tar`

### file list

```diff
@@ -1,234 +1,235 @@
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.778252 feapder-1.9.0b2/
--rw-r--r--   0 liubo      (501) staff       (20)     1102 2021-08-04 13:29:34.000000 feapder-1.9.0b2/LICENSE
--rw-r--r--   0 liubo      (501) staff       (20)      231 2021-08-12 03:51:27.000000 feapder-1.9.0b2/MANIFEST.in
--rw-r--r--   0 liubo      (501) staff       (20)     4828 2023-11-07 11:44:38.777435 feapder-1.9.0b2/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)     4382 2023-09-15 11:36:15.000000 feapder-1.9.0b2/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.544931 feapder-1.9.0b2/feapder/
--rw-r--r--   0 liubo      (501) staff       (20)       11 2023-11-07 11:20:46.000000 feapder-1.9.0b2/feapder/VERSION
--rw-r--r--   0 liubo      (501) staff       (20)      815 2023-06-28 09:14:32.000000 feapder-1.9.0b2/feapder/__init__.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.549954 feapder-1.9.0b2/feapder/buffer/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.9.0b2/feapder/buffer/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)    14555 2023-11-07 11:42:36.000000 feapder-1.9.0b2/feapder/buffer/item_buffer.py
--rw-r--r--   0 liubo      (501) staff       (20)     5436 2023-11-07 11:18:56.000000 feapder-1.9.0b2/feapder/buffer/request_buffer.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.555026 feapder-1.9.0b2/feapder/commands/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.0b2/feapder/commands/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     3824 2023-06-28 09:14:32.000000 feapder-1.9.0b2/feapder/commands/cmdline.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.562415 feapder-1.9.0b2/feapder/commands/create/
--rw-r--r--   0 liubo      (501) staff       (20)      543 2021-09-02 10:23:23.000000 feapder-1.9.0b2/feapder/commands/create/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      975 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/commands/create/create_cookies.py
--rw-r--r--   0 liubo      (501) staff       (20)      670 2021-02-08 06:31:07.000000 feapder-1.9.0b2/feapder/commands/create/create_init.py
--rw-r--r--   0 liubo      (501) staff       (20)     6004 2022-09-07 03:39:37.000000 feapder-1.9.0b2/feapder/commands/create/create_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     1366 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/commands/create/create_json.py
--rw-r--r--   0 liubo      (501) staff       (20)     1106 2021-09-02 10:23:23.000000 feapder-1.9.0b2/feapder/commands/create/create_params.py
--rw-r--r--   0 liubo      (501) staff       (20)     1360 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/commands/create/create_project.py
--rw-r--r--   0 liubo      (501) staff       (20)      693 2021-08-04 13:29:34.000000 feapder-1.9.0b2/feapder/commands/create/create_setting.py
--rw-r--r--   0 liubo      (501) staff       (20)     3648 2022-09-07 03:39:37.000000 feapder-1.9.0b2/feapder/commands/create/create_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     4288 2023-06-28 09:14:30.000000 feapder-1.9.0b2/feapder/commands/create/create_table.py
--rw-r--r--   0 liubo      (501) staff       (20)     3984 2022-10-21 10:06:04.000000 feapder-1.9.0b2/feapder/commands/create_builder.py
--rw-r--r--   0 liubo      (501) staff       (20)     1354 2023-06-28 09:14:31.000000 feapder-1.9.0b2/feapder/commands/retry.py
--rw-r--r--   0 liubo      (501) staff       (20)     5514 2022-10-21 10:06:04.000000 feapder-1.9.0b2/feapder/commands/shell.py
--rw-r--r--   0 liubo      (501) staff       (20)     2572 2023-06-28 09:14:31.000000 feapder-1.9.0b2/feapder/commands/zip.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.569300 feapder-1.9.0b2/feapder/core/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.9.0b2/feapder/core/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     6240 2022-12-01 11:29:17.000000 feapder-1.9.0b2/feapder/core/base_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)     3256 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/core/collector.py
--rw-r--r--   0 liubo      (501) staff       (20)     2807 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/core/handle_failed_items.py
--rw-r--r--   0 liubo      (501) staff       (20)     1733 2023-06-28 09:14:31.000000 feapder-1.9.0b2/feapder/core/handle_failed_requests.py
--rw-r--r--   0 liubo      (501) staff       (20)    32962 2023-08-18 08:40:56.000000 feapder-1.9.0b2/feapder/core/parser_control.py
--rw-r--r--   0 liubo      (501) staff       (20)    21488 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/core/scheduler.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.574971 feapder-1.9.0b2/feapder/core/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)      417 2022-07-25 12:58:57.000000 feapder-1.9.0b2/feapder/core/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     4372 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/core/spiders/air_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    49433 2023-09-05 03:48:50.000000 feapder-1.9.0b2/feapder/core/spiders/batch_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    13420 2023-06-28 09:14:32.000000 feapder-1.9.0b2/feapder/core/spiders/spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    27875 2023-06-28 09:14:32.000000 feapder-1.9.0b2/feapder/core/spiders/task_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.581580 feapder-1.9.0b2/feapder/db/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-12-21 10:30:46.000000 feapder-1.9.0b2/feapder/db/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1117 2023-06-28 09:14:30.000000 feapder-1.9.0b2/feapder/db/memorydb.py
--rw-r--r--   0 liubo      (501) staff       (20)    13606 2021-12-04 11:42:58.000000 feapder-1.9.0b2/feapder/db/mongodb.py
--rw-r--r--   0 liubo      (501) staff       (20)    10810 2023-09-26 08:50:29.000000 feapder-1.9.0b2/feapder/db/mysqldb.py
--rw-r--r--   0 liubo      (501) staff       (20)    29545 2023-08-18 08:40:56.000000 feapder-1.9.0b2/feapder/db/redisdb.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.587263 feapder-1.9.0b2/feapder/dedup/
--rw-r--r--   0 liubo      (501) staff       (20)     6616 2022-09-25 13:50:01.000000 feapder-1.9.0b2/feapder/dedup/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      901 2022-09-25 13:50:01.000000 feapder-1.9.0b2/feapder/dedup/basefilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     4133 2023-06-28 09:14:32.000000 feapder-1.9.0b2/feapder/dedup/bitarray.py
--rw-r--r--   0 liubo      (501) staff       (20)    12518 2022-09-25 13:50:01.000000 feapder-1.9.0b2/feapder/dedup/bloomfilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     2309 2023-06-28 09:14:32.000000 feapder-1.9.0b2/feapder/dedup/expirefilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     1854 2023-06-28 09:14:32.000000 feapder-1.9.0b2/feapder/dedup/litefilter.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.612443 feapder-1.9.0b2/feapder/network/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.0b2/feapder/network/__init__.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.618542 feapder-1.9.0b2/feapder/network/downloader/
--rw-r--r--   0 liubo      (501) staff       (20)      299 2023-06-28 09:14:32.000000 feapder-1.9.0b2/feapder/network/downloader/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     3217 2023-06-28 09:14:31.000000 feapder-1.9.0b2/feapder/network/downloader/_playwright.py
--rw-r--r--   0 liubo      (501) staff       (20)     1440 2022-09-09 06:16:43.000000 feapder-1.9.0b2/feapder/network/downloader/_requests.py
--rw-r--r--   0 liubo      (501) staff       (20)     3093 2023-06-28 09:14:31.000000 feapder-1.9.0b2/feapder/network/downloader/_selenium.py
--rw-r--r--   0 liubo      (501) staff       (20)      694 2022-09-07 03:39:37.000000 feapder-1.9.0b2/feapder/network/downloader/base.py
--rw-r--r--   0 liubo      (501) staff       (20)     4341 2023-06-28 09:14:31.000000 feapder-1.9.0b2/feapder/network/item.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.620532 feapder-1.9.0b2/feapder/network/proxy_pool/
--rw-r--r--   0 liubo      (501) staff       (20)      200 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/network/proxy_pool/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      797 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/network/proxy_pool/base.py
--rw-r--r--   0 liubo      (501) staff       (20)     2033 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/network/proxy_pool/proxy_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)    23025 2023-08-18 08:40:56.000000 feapder-1.9.0b2/feapder/network/proxy_pool_old.py
--rw-r--r--   0 liubo      (501) staff       (20)    17887 2023-09-21 06:40:54.000000 feapder-1.9.0b2/feapder/network/request.py
--rw-r--r--   0 liubo      (501) staff       (20)    12743 2023-06-28 09:14:32.000000 feapder-1.9.0b2/feapder/network/response.py
--rw-r--r--   0 liubo      (501) staff       (20)     5661 2023-06-28 09:14:31.000000 feapder-1.9.0b2/feapder/network/selector.py
--rw-r--r--   0 liubo      (501) staff       (20)   130399 2023-06-28 08:50:40.000000 feapder-1.9.0b2/feapder/network/user_agent.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.623978 feapder-1.9.0b2/feapder/network/user_pool/
--rw-r--r--   0 liubo      (501) staff       (20)      329 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/network/user_pool/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     6397 2023-06-28 09:14:31.000000 feapder-1.9.0b2/feapder/network/user_pool/base_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)    10762 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/network/user_pool/gold_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     5377 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/network/user_pool/guest_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     8648 2023-06-28 09:14:32.000000 feapder-1.9.0b2/feapder/network/user_pool/normal_user_pool.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.627338 feapder-1.9.0b2/feapder/pipelines/
--rw-r--r--   0 liubo      (501) staff       (20)     1382 2021-09-23 09:22:51.000000 feapder-1.9.0b2/feapder/pipelines/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1392 2022-09-25 13:50:01.000000 feapder-1.9.0b2/feapder/pipelines/console_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2405 2021-09-23 09:22:51.000000 feapder-1.9.0b2/feapder/pipelines/mongo_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2088 2021-04-08 03:41:12.000000 feapder-1.9.0b2/feapder/pipelines/mysql_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)      363 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/requirements.txt
--rw-r--r--   0 liubo      (501) staff       (20)    11074 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.632474 feapder-1.9.0b2/feapder/templates/
--rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.0b2/feapder/templates/.DS_Store
--rw-r--r--   0 liubo      (501) staff       (20)      592 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/templates/air_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)     2083 2022-09-07 03:39:38.000000 feapder-1.9.0b2/feapder/templates/batch_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)      353 2021-12-22 05:53:07.000000 feapder-1.9.0b2/feapder/templates/item_template.tmpl
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.636552 feapder-1.9.0b2/feapder/templates/project_template/
--rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.0b2/feapder/templates/project_template/.DS_Store
--rw-r--r--   0 liubo      (501) staff       (20)     1574 2021-08-04 13:29:34.000000 feapder-1.9.0b2/feapder/templates/project_template/CHECK_DATA.md
--rw-r--r--   0 liubo      (501) staff       (20)       81 2021-08-04 13:29:34.000000 feapder-1.9.0b2/feapder/templates/project_template/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.637240 feapder-1.9.0b2/feapder/templates/project_template/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.0b2/feapder/templates/project_template/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     2089 2021-09-02 10:23:23.000000 feapder-1.9.0b2/feapder/templates/project_template/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     9079 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/templates/project_template/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.637698 feapder-1.9.0b2/feapder/templates/project_template/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.0b2/feapder/templates/project_template/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      808 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/templates/spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.9.0b2/feapder/templates/task_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)      365 2022-09-19 07:00:37.000000 feapder-1.9.0b2/feapder/templates/update_item_template.tmpl
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.664661 feapder-1.9.0b2/feapder/utils/
--rw-r--r--   0 liubo      (501) staff       (20)      135 2021-08-04 13:29:34.000000 feapder-1.9.0b2/feapder/utils/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1959 2021-02-07 13:26:42.000000 feapder-1.9.0b2/feapder/utils/custom_argparse.py
--rw-r--r--   0 liubo      (501) staff       (20)     2537 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/utils/email_sender.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.667174 feapder-1.9.0b2/feapder/utils/js/
--rw-r--r--   0 liubo      (501) staff       (20)     6344 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/utils/js/intercept.js
--rw-r--r--   0 liubo      (501) staff       (20)   166307 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/utils/js/stealth.min.js
--rw-r--r--   0 liubo      (501) staff       (20)     8468 2023-06-28 09:47:12.000000 feapder-1.9.0b2/feapder/utils/log.py
--rw-r--r--   0 liubo      (501) staff       (20)    16820 2023-06-28 09:14:32.000000 feapder-1.9.0b2/feapder/utils/metrics.py
--rw-r--r--   0 liubo      (501) staff       (20)     2123 2021-08-12 03:51:27.000000 feapder-1.9.0b2/feapder/utils/perfect_dict.py
--rw-r--r--   0 liubo      (501) staff       (20)     3670 2022-06-10 02:51:23.000000 feapder-1.9.0b2/feapder/utils/redis_lock.py
--rw-r--r--   0 liubo      (501) staff       (20)    74173 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/utils/tools.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.672506 feapder-1.9.0b2/feapder/utils/webdriver/
--rw-r--r--   0 liubo      (501) staff       (20)      380 2023-06-28 09:14:30.000000 feapder-1.9.0b2/feapder/utils/webdriver/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     9344 2023-08-18 08:40:56.000000 feapder-1.9.0b2/feapder/utils/webdriver/playwright_driver.py
--rw-r--r--   0 liubo      (501) staff       (20)    18034 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/utils/webdriver/selenium_driver.py
--rw-r--r--   0 liubo      (501) staff       (20)     2579 2023-09-15 11:36:15.000000 feapder-1.9.0b2/feapder/utils/webdriver/webdirver.py
--rw-r--r--   0 liubo      (501) staff       (20)     3282 2023-06-28 09:14:31.000000 feapder-1.9.0b2/feapder/utils/webdriver/webdriver_pool.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.547719 feapder-1.9.0b2/feapder.egg-info/
--rw-r--r--   0 liubo      (501) staff       (20)     4828 2023-11-07 11:44:38.000000 feapder-1.9.0b2/feapder.egg-info/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)     6133 2023-11-07 11:44:38.000000 feapder-1.9.0b2/feapder.egg-info/SOURCES.txt
--rw-r--r--   0 liubo      (501) staff       (20)        1 2023-11-07 11:44:38.000000 feapder-1.9.0b2/feapder.egg-info/dependency_links.txt
--rw-r--r--   0 liubo      (501) staff       (20)       61 2023-11-07 11:44:38.000000 feapder-1.9.0b2/feapder.egg-info/entry_points.txt
--rw-r--r--   0 liubo      (501) staff       (20)      435 2023-11-07 11:44:38.000000 feapder-1.9.0b2/feapder.egg-info/requires.txt
--rw-r--r--   0 liubo      (501) staff       (20)        8 2023-11-07 11:44:38.000000 feapder-1.9.0b2/feapder.egg-info/top_level.txt
--rw-r--r--   0 liubo      (501) staff       (20)       38 2023-11-07 11:44:38.778468 feapder-1.9.0b2/setup.cfg
--rw-r--r--   0 liubo      (501) staff       (20)     2103 2023-09-15 11:36:15.000000 feapder-1.9.0b2/setup.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.687885 feapder-1.9.0b2/tests/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.690885 feapder-1.9.0b2/tests/air-spider/
--rw-r--r--   0 liubo      (501) staff       (20)     1218 2023-09-05 06:59:45.000000 feapder-1.9.0b2/tests/air-spider/test_air_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     1075 2023-06-28 09:14:30.000000 feapder-1.9.0b2/tests/air-spider/test_air_spider_filter.py
--rw-r--r--   0 liubo      (501) staff       (20)     1094 2023-06-28 09:14:32.000000 feapder-1.9.0b2/tests/air-spider/test_air_spider_item.py
--rw-r--r--   0 liubo      (501) staff       (20)      648 2023-09-15 11:36:15.000000 feapder-1.9.0b2/tests/air-spider/test_render_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.693241 feapder-1.9.0b2/tests/batch-spider/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.699870 feapder-1.9.0b2/tests/batch-spider/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2021-09-03 07:47:43.000000 feapder-1.9.0b2/tests/batch-spider/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      586 2021-09-12 14:22:50.000000 feapder-1.9.0b2/tests/batch-spider/items/spider_data_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     2020 2023-06-09 12:31:43.000000 feapder-1.9.0b2/tests/batch-spider/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2227 2021-09-02 10:23:23.000000 feapder-1.9.0b2/tests/batch-spider/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.701739 feapder-1.9.0b2/tests/batch-spider/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       31 2021-02-08 08:09:47.000000 feapder-1.9.0b2/tests/batch-spider/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1575 2023-06-28 09:14:32.000000 feapder-1.9.0b2/tests/batch-spider/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      851 2021-02-08 08:29:51.000000 feapder-1.9.0b2/tests/batch-spider/table.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.695470 feapder-1.9.0b2/tests/batch-spider-integration/
--rw-r--r--   0 liubo      (501) staff       (20)      746 2021-03-03 03:39:52.000000 feapder-1.9.0b2/tests/batch-spider-integration/batch_spider_integration_task.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.696055 feapder-1.9.0b2/tests/batch-spider-integration/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.9.0b2/tests/batch-spider-integration/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1686 2021-12-30 08:52:14.000000 feapder-1.9.0b2/tests/batch-spider-integration/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.9.0b2/tests/batch-spider-integration/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.698443 feapder-1.9.0b2/tests/batch-spider-integration/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.9.0b2/tests/batch-spider-integration/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      581 2021-03-18 02:19:03.000000 feapder-1.9.0b2/tests/batch-spider-integration/spiders/sina_news_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)      584 2021-03-18 02:19:03.000000 feapder-1.9.0b2/tests/batch-spider-integration/spiders/tencent_news_parser.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.702402 feapder-1.9.0b2/tests/db/
--rw-r--r--   0 liubo      (501) staff       (20)      373 2021-03-06 15:13:19.000000 feapder-1.9.0b2/tests/db/test_redis.py
--rw-r--r--   0 liubo      (501) staff       (20)     2087 2021-03-18 02:19:03.000000 feapder-1.9.0b2/tests/jd_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     1011 2021-12-01 05:56:45.000000 feapder-1.9.0b2/tests/mongo_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.704406 feapder-1.9.0b2/tests/spider/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.753377 feapder-1.9.0b2/tests/spider/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2022-01-27 08:13:00.000000 feapder-1.9.0b2/tests/spider/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      358 2021-12-22 05:05:06.000000 feapder-1.9.0b2/tests/spider/items/spider_data_item.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.754294 feapder-1.9.0b2/tests/spider/log/
--rw-r--r--   0 liubo      (501) staff       (20)     1719 2021-08-11 01:59:56.000000 feapder-1.9.0b2/tests/spider/log/haha.log
--rw-r--r--   0 liubo      (501) staff       (20)      296 2022-08-31 02:19:25.000000 feapder-1.9.0b2/tests/spider/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2676 2023-06-28 09:14:30.000000 feapder-1.9.0b2/tests/spider/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.757547 feapder-1.9.0b2/tests/spider/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       42 2021-02-21 15:44:20.000000 feapder-1.9.0b2/tests/spider/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      985 2022-10-25 08:22:40.000000 feapder-1.9.0b2/tests/spider/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      612 2021-08-04 13:29:34.000000 feapder-1.9.0b2/tests/spider/spiders/test_spider2.py
--rw-r--r--   0 liubo      (501) staff       (20)      320 2021-02-08 08:40:34.000000 feapder-1.9.0b2/tests/spider/table.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.710959 feapder-1.9.0b2/tests/spider-integration/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.749286 feapder-1.9.0b2/tests/spider-integration/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.9.0b2/tests/spider-integration/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      517 2021-12-30 08:51:43.000000 feapder-1.9.0b2/tests/spider-integration/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.9.0b2/tests/spider-integration/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.751722 feapder-1.9.0b2/tests/spider-integration/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.9.0b2/tests/spider-integration/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      470 2023-03-29 13:31:04.000000 feapder-1.9.0b2/tests/spider-integration/spiders/sina_news_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)      456 2021-09-24 05:52:08.000000 feapder-1.9.0b2/tests/spider-integration/spiders/tencent_news_parser.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.758450 feapder-1.9.0b2/tests/task-spider/
--rw-r--r--   0 liubo      (501) staff       (20)     2133 2023-06-28 09:14:32.000000 feapder-1.9.0b2/tests/task-spider/test_task_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.761693 feapder-1.9.0b2/tests/test-debugger/
--rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.0b2/tests/test-debugger/.DS_Store
--rw-r--r--   0 liubo      (501) staff       (20)       81 2023-06-28 09:14:32.000000 feapder-1.9.0b2/tests/test-debugger/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.762697 feapder-1.9.0b2/tests/test-debugger/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2023-06-28 09:14:32.000000 feapder-1.9.0b2/tests/test-debugger/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      352 2023-06-28 09:14:32.000000 feapder-1.9.0b2/tests/test-debugger/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     8791 2023-09-15 11:36:15.000000 feapder-1.9.0b2/tests/test-debugger/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.764034 feapder-1.9.0b2/tests/test-debugger/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       33 2023-06-28 09:14:32.000000 feapder-1.9.0b2/tests/test-debugger/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      724 2023-06-28 09:14:32.000000 feapder-1.9.0b2/tests/test-debugger/spiders/test_debugger.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.767690 feapder-1.9.0b2/tests/test-pipeline/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.769832 feapder-1.9.0b2/tests/test-pipeline/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2021-03-18 02:19:03.000000 feapder-1.9.0b2/tests/test-pipeline/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      586 2021-03-18 02:19:03.000000 feapder-1.9.0b2/tests/test-pipeline/items/spider_data_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     1250 2022-09-07 03:39:38.000000 feapder-1.9.0b2/tests/test-pipeline/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     1416 2021-04-08 03:41:12.000000 feapder-1.9.0b2/tests/test-pipeline/pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2021-09-02 10:23:23.000000 feapder-1.9.0b2/tests/test-pipeline/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.771903 feapder-1.9.0b2/tests/test-pipeline/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       31 2021-03-30 02:34:20.000000 feapder-1.9.0b2/tests/test-pipeline/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1514 2021-03-18 02:19:03.000000 feapder-1.9.0b2/tests/test-pipeline/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      851 2021-03-18 02:19:03.000000 feapder-1.9.0b2/tests/test-pipeline/table.sql
--rw-r--r--   0 liubo      (501) staff       (20)      796 2023-09-19 02:11:49.000000 feapder-1.9.0b2/tests/test.py
--rw-r--r--   0 liubo      (501) staff       (20)     3140 2023-06-28 09:14:32.000000 feapder-1.9.0b2/tests/test_dedup.py
--rw-r--r--   0 liubo      (501) staff       (20)      991 2023-09-21 06:41:27.000000 feapder-1.9.0b2/tests/test_download_midware.py
--rw-r--r--   0 liubo      (501) staff       (20)      469 2021-09-02 10:22:59.000000 feapder-1.9.0b2/tests/test_lock.py
--rw-r--r--   0 liubo      (501) staff       (20)      329 2023-06-28 09:47:12.000000 feapder-1.9.0b2/tests/test_log.py
--rw-r--r--   0 liubo      (501) staff       (20)     1229 2023-06-28 09:14:32.000000 feapder-1.9.0b2/tests/test_metrics.py
--rw-r--r--   0 liubo      (501) staff       (20)     4678 2021-12-01 05:56:51.000000 feapder-1.9.0b2/tests/test_mongodb.py
--rw-r--r--   0 liubo      (501) staff       (20)      232 2021-10-14 08:25:11.000000 feapder-1.9.0b2/tests/test_mysqldb.py
--rw-r--r--   0 liubo      (501) staff       (20)     1086 2023-06-28 09:14:31.000000 feapder-1.9.0b2/tests/test_playwright.py
--rw-r--r--   0 liubo      (501) staff       (20)     3477 2023-06-28 09:14:30.000000 feapder-1.9.0b2/tests/test_playwright2.py
--rw-r--r--   0 liubo      (501) staff       (20)      660 2022-10-28 07:20:27.000000 feapder-1.9.0b2/tests/test_rander.py
--rw-r--r--   0 liubo      (501) staff       (20)      769 2021-07-08 11:51:50.000000 feapder-1.9.0b2/tests/test_rander2.py
--rw-r--r--   0 liubo      (501) staff       (20)      519 2022-09-14 07:25:07.000000 feapder-1.9.0b2/tests/test_rander3.py
--rw-r--r--   0 liubo      (501) staff       (20)     1990 2023-09-15 11:36:15.000000 feapder-1.9.0b2/tests/test_rander_xhr.py
--rw-r--r--   0 liubo      (501) staff       (20)      148 2021-08-12 03:51:27.000000 feapder-1.9.0b2/tests/test_redisdb.py
--rw-r--r--   0 liubo      (501) staff       (20)     1634 2022-09-25 13:50:01.000000 feapder-1.9.0b2/tests/test_request.py
--rw-r--r--   0 liubo      (501) staff       (20)      637 2021-04-08 03:41:12.000000 feapder-1.9.0b2/tests/test_spider_params.py
--rw-r--r--   0 liubo      (501) staff       (20)      593 2022-07-25 12:58:57.000000 feapder-1.9.0b2/tests/test_task.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.773138 feapder-1.9.0b2/tests/test_template/
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.9.0b2/tests/test_template/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      429 2022-05-17 07:19:13.000000 feapder-1.9.0b2/tests/test_tools.py
--rw-r--r--   0 liubo      (501) staff       (20)     1011 2022-09-07 09:10:23.000000 feapder-1.9.0b2/tests/test_webdriver.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-11-07 11:44:38.776513 feapder-1.9.0b2/tests/user_pool/
--rw-r--r--   0 liubo      (501) staff       (20)     2423 2022-06-10 02:51:23.000000 feapder-1.9.0b2/tests/user_pool/test_gold_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     2121 2022-06-10 02:51:23.000000 feapder-1.9.0b2/tests/user_pool/test_guest_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     1427 2022-06-10 02:51:23.000000 feapder-1.9.0b2/tests/user_pool/test_normal_user_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.773420 feapder-1.9.1b1/
+-rw-r--r--   0 liubo      (501) staff       (20)     1102 2021-08-04 13:29:34.000000 feapder-1.9.1b1/LICENSE
+-rw-r--r--   0 liubo      (501) staff       (20)      231 2021-08-12 03:51:27.000000 feapder-1.9.1b1/MANIFEST.in
+-rw-r--r--   0 liubo      (501) staff       (20)     4828 2024-04-08 04:47:30.773050 feapder-1.9.1b1/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)     4382 2023-09-15 11:36:15.000000 feapder-1.9.1b1/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.594898 feapder-1.9.1b1/feapder/
+-rw-r--r--   0 liubo      (501) staff       (20)       11 2024-04-08 04:47:09.000000 feapder-1.9.1b1/feapder/VERSION
+-rw-r--r--   0 liubo      (501) staff       (20)      815 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/__init__.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.604452 feapder-1.9.1b1/feapder/buffer/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/buffer/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)    14555 2024-03-19 11:52:17.000000 feapder-1.9.1b1/feapder/buffer/item_buffer.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5436 2024-03-19 11:52:17.000000 feapder-1.9.1b1/feapder/buffer/request_buffer.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.609740 feapder-1.9.1b1/feapder/commands/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b1/feapder/commands/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3824 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/commands/cmdline.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.618214 feapder-1.9.1b1/feapder/commands/create/
+-rw-r--r--   0 liubo      (501) staff       (20)      543 2021-09-02 10:23:23.000000 feapder-1.9.1b1/feapder/commands/create/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      975 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/commands/create/create_cookies.py
+-rw-r--r--   0 liubo      (501) staff       (20)      670 2021-02-08 06:31:07.000000 feapder-1.9.1b1/feapder/commands/create/create_init.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6004 2022-09-07 03:39:37.000000 feapder-1.9.1b1/feapder/commands/create/create_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1366 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/commands/create/create_json.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1106 2021-09-02 10:23:23.000000 feapder-1.9.1b1/feapder/commands/create/create_params.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1360 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/commands/create/create_project.py
+-rw-r--r--   0 liubo      (501) staff       (20)      693 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/commands/create/create_setting.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3648 2022-09-07 03:39:37.000000 feapder-1.9.1b1/feapder/commands/create/create_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4288 2023-06-28 09:14:30.000000 feapder-1.9.1b1/feapder/commands/create/create_table.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3984 2022-10-21 10:06:04.000000 feapder-1.9.1b1/feapder/commands/create_builder.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1354 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/commands/retry.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5514 2022-10-21 10:06:04.000000 feapder-1.9.1b1/feapder/commands/shell.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2572 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/commands/zip.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.626825 feapder-1.9.1b1/feapder/core/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/core/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6501 2024-03-18 02:39:32.000000 feapder-1.9.1b1/feapder/core/base_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3256 2024-03-19 11:52:17.000000 feapder-1.9.1b1/feapder/core/collector.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2807 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/core/handle_failed_items.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1733 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/core/handle_failed_requests.py
+-rw-r--r--   0 liubo      (501) staff       (20)    32962 2024-03-19 11:52:17.000000 feapder-1.9.1b1/feapder/core/parser_control.py
+-rw-r--r--   0 liubo      (501) staff       (20)    21531 2024-03-19 12:14:49.000000 feapder-1.9.1b1/feapder/core/scheduler.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.633720 feapder-1.9.1b1/feapder/core/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)      417 2022-07-25 12:58:57.000000 feapder-1.9.1b1/feapder/core/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4395 2024-03-19 12:15:05.000000 feapder-1.9.1b1/feapder/core/spiders/air_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    49433 2023-09-05 03:48:50.000000 feapder-1.9.1b1/feapder/core/spiders/batch_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    13420 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/core/spiders/spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    27875 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/core/spiders/task_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.638615 feapder-1.9.1b1/feapder/db/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-12-21 10:30:46.000000 feapder-1.9.1b1/feapder/db/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1117 2023-06-28 09:14:30.000000 feapder-1.9.1b1/feapder/db/memorydb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    15961 2024-03-18 02:57:07.000000 feapder-1.9.1b1/feapder/db/mongodb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    10959 2024-04-08 04:45:21.000000 feapder-1.9.1b1/feapder/db/mysqldb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    30873 2024-03-18 02:56:54.000000 feapder-1.9.1b1/feapder/db/redisdb.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.644278 feapder-1.9.1b1/feapder/dedup/
+-rw-r--r--   0 liubo      (501) staff       (20)     6616 2022-09-25 13:50:01.000000 feapder-1.9.1b1/feapder/dedup/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      901 2022-09-25 13:50:01.000000 feapder-1.9.1b1/feapder/dedup/basefilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4511 2023-12-11 13:13:43.000000 feapder-1.9.1b1/feapder/dedup/bitarray.py
+-rw-r--r--   0 liubo      (501) staff       (20)    12518 2022-09-25 13:50:01.000000 feapder-1.9.1b1/feapder/dedup/bloomfilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2309 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/dedup/expirefilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1854 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/dedup/litefilter.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.653090 feapder-1.9.1b1/feapder/network/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b1/feapder/network/__init__.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.660464 feapder-1.9.1b1/feapder/network/downloader/
+-rw-r--r--   0 liubo      (501) staff       (20)      299 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/network/downloader/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3217 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/network/downloader/_playwright.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1440 2022-09-09 06:16:43.000000 feapder-1.9.1b1/feapder/network/downloader/_requests.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3093 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/network/downloader/_selenium.py
+-rw-r--r--   0 liubo      (501) staff       (20)      694 2022-09-07 03:39:37.000000 feapder-1.9.1b1/feapder/network/downloader/base.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4341 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/network/item.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.662831 feapder-1.9.1b1/feapder/network/proxy_pool/
+-rw-r--r--   0 liubo      (501) staff       (20)      200 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/network/proxy_pool/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      797 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/network/proxy_pool/base.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2033 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/network/proxy_pool/proxy_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)    23025 2023-08-18 08:40:56.000000 feapder-1.9.1b1/feapder/network/proxy_pool_old.py
+-rw-r--r--   0 liubo      (501) staff       (20)    18070 2024-03-18 03:14:24.000000 feapder-1.9.1b1/feapder/network/request.py
+-rw-r--r--   0 liubo      (501) staff       (20)    12743 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/network/response.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5661 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/network/selector.py
+-rw-r--r--   0 liubo      (501) staff       (20)   130399 2023-06-28 08:50:40.000000 feapder-1.9.1b1/feapder/network/user_agent.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.667036 feapder-1.9.1b1/feapder/network/user_pool/
+-rw-r--r--   0 liubo      (501) staff       (20)      329 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/network/user_pool/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6397 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/network/user_pool/base_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)    10762 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/network/user_pool/gold_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5377 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/network/user_pool/guest_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     8648 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/network/user_pool/normal_user_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.670041 feapder-1.9.1b1/feapder/pipelines/
+-rw-r--r--   0 liubo      (501) staff       (20)     1382 2021-09-23 09:22:51.000000 feapder-1.9.1b1/feapder/pipelines/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1392 2022-09-25 13:50:01.000000 feapder-1.9.1b1/feapder/pipelines/console_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2405 2021-09-23 09:22:51.000000 feapder-1.9.1b1/feapder/pipelines/mongo_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2088 2021-04-08 03:41:12.000000 feapder-1.9.1b1/feapder/pipelines/mysql_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)      363 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/requirements.txt
+-rw-r--r--   0 liubo      (501) staff       (20)    11184 2024-03-18 02:46:57.000000 feapder-1.9.1b1/feapder/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.675492 feapder-1.9.1b1/feapder/templates/
+-rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.1b1/feapder/templates/.DS_Store
+-rw-r--r--   0 liubo      (501) staff       (20)      592 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/templates/air_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)     2083 2022-09-07 03:39:38.000000 feapder-1.9.1b1/feapder/templates/batch_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)      353 2021-12-22 05:53:07.000000 feapder-1.9.1b1/feapder/templates/item_template.tmpl
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.679257 feapder-1.9.1b1/feapder/templates/project_template/
+-rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.1b1/feapder/templates/project_template/.DS_Store
+-rw-r--r--   0 liubo      (501) staff       (20)     1574 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/templates/project_template/CHECK_DATA.md
+-rw-r--r--   0 liubo      (501) staff       (20)       81 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/templates/project_template/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.679977 feapder-1.9.1b1/feapder/templates/project_template/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b1/feapder/templates/project_template/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2089 2021-09-02 10:23:23.000000 feapder-1.9.1b1/feapder/templates/project_template/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     9191 2024-03-18 02:47:28.000000 feapder-1.9.1b1/feapder/templates/project_template/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.680330 feapder-1.9.1b1/feapder/templates/project_template/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b1/feapder/templates/project_template/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      808 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/templates/spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.9.1b1/feapder/templates/task_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)      365 2022-09-19 07:00:37.000000 feapder-1.9.1b1/feapder/templates/update_item_template.tmpl
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.687044 feapder-1.9.1b1/feapder/utils/
+-rw-r--r--   0 liubo      (501) staff       (20)      135 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/utils/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1959 2021-02-07 13:26:42.000000 feapder-1.9.1b1/feapder/utils/custom_argparse.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2537 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/utils/email_sender.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.690464 feapder-1.9.1b1/feapder/utils/js/
+-rw-r--r--   0 liubo      (501) staff       (20)     6344 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/utils/js/intercept.js
+-rw-r--r--   0 liubo      (501) staff       (20)   166307 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/utils/js/stealth.min.js
+-rw-r--r--   0 liubo      (501) staff       (20)     8468 2023-06-28 09:47:12.000000 feapder-1.9.1b1/feapder/utils/log.py
+-rw-r--r--   0 liubo      (501) staff       (20)    16820 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/utils/metrics.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2123 2021-08-12 03:51:27.000000 feapder-1.9.1b1/feapder/utils/perfect_dict.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3714 2023-11-22 02:36:32.000000 feapder-1.9.1b1/feapder/utils/redis_lock.py
+-rw-r--r--   0 liubo      (501) staff       (20)      796 2024-03-19 12:13:54.000000 feapder-1.9.1b1/feapder/utils/tail_thread.py
+-rw-r--r--   0 liubo      (501) staff       (20)    74948 2024-03-18 02:46:57.000000 feapder-1.9.1b1/feapder/utils/tools.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.697296 feapder-1.9.1b1/feapder/utils/webdriver/
+-rw-r--r--   0 liubo      (501) staff       (20)      380 2023-06-28 09:14:30.000000 feapder-1.9.1b1/feapder/utils/webdriver/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     9344 2023-08-18 08:40:56.000000 feapder-1.9.1b1/feapder/utils/webdriver/playwright_driver.py
+-rw-r--r--   0 liubo      (501) staff       (20)    18034 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/utils/webdriver/selenium_driver.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2579 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/utils/webdriver/webdirver.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3282 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/utils/webdriver/webdriver_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.600585 feapder-1.9.1b1/feapder.egg-info/
+-rw-r--r--   0 liubo      (501) staff       (20)     4828 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)     6162 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/SOURCES.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/dependency_links.txt
+-rw-r--r--   0 liubo      (501) staff       (20)       61 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/entry_points.txt
+-rw-r--r--   0 liubo      (501) staff       (20)      435 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/requires.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        8 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/top_level.txt
+-rw-r--r--   0 liubo      (501) staff       (20)       38 2024-04-08 04:47:30.773511 feapder-1.9.1b1/setup.cfg
+-rw-r--r--   0 liubo      (501) staff       (20)     2103 2023-09-15 11:36:15.000000 feapder-1.9.1b1/setup.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.720090 feapder-1.9.1b1/tests/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.723770 feapder-1.9.1b1/tests/air-spider/
+-rw-r--r--   0 liubo      (501) staff       (20)     1218 2024-03-18 03:14:21.000000 feapder-1.9.1b1/tests/air-spider/test_air_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1075 2023-06-28 09:14:30.000000 feapder-1.9.1b1/tests/air-spider/test_air_spider_filter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1094 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/air-spider/test_air_spider_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)      648 2023-09-15 11:36:15.000000 feapder-1.9.1b1/tests/air-spider/test_render_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.727772 feapder-1.9.1b1/tests/batch-spider/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.737319 feapder-1.9.1b1/tests/batch-spider/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2021-09-03 07:47:43.000000 feapder-1.9.1b1/tests/batch-spider/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      586 2021-09-12 14:22:50.000000 feapder-1.9.1b1/tests/batch-spider/items/spider_data_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2020 2023-06-09 12:31:43.000000 feapder-1.9.1b1/tests/batch-spider/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2227 2021-09-02 10:23:23.000000 feapder-1.9.1b1/tests/batch-spider/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.739157 feapder-1.9.1b1/tests/batch-spider/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       31 2021-02-08 08:09:47.000000 feapder-1.9.1b1/tests/batch-spider/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1575 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/batch-spider/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      851 2021-02-08 08:29:51.000000 feapder-1.9.1b1/tests/batch-spider/table.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.731798 feapder-1.9.1b1/tests/batch-spider-integration/
+-rw-r--r--   0 liubo      (501) staff       (20)      746 2021-03-03 03:39:52.000000 feapder-1.9.1b1/tests/batch-spider-integration/batch_spider_integration_task.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.732840 feapder-1.9.1b1/tests/batch-spider-integration/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.9.1b1/tests/batch-spider-integration/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1686 2021-12-30 08:52:14.000000 feapder-1.9.1b1/tests/batch-spider-integration/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.9.1b1/tests/batch-spider-integration/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.735652 feapder-1.9.1b1/tests/batch-spider-integration/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.9.1b1/tests/batch-spider-integration/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      581 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/batch-spider-integration/spiders/sina_news_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)      584 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/batch-spider-integration/spiders/tencent_news_parser.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.740019 feapder-1.9.1b1/tests/db/
+-rw-r--r--   0 liubo      (501) staff       (20)      373 2021-03-06 15:13:19.000000 feapder-1.9.1b1/tests/db/test_redis.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2087 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/jd_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1011 2021-12-01 05:56:45.000000 feapder-1.9.1b1/tests/mongo_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.742300 feapder-1.9.1b1/tests/spider/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.748578 feapder-1.9.1b1/tests/spider/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2022-01-27 08:13:00.000000 feapder-1.9.1b1/tests/spider/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      358 2021-12-22 05:05:06.000000 feapder-1.9.1b1/tests/spider/items/spider_data_item.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.749588 feapder-1.9.1b1/tests/spider/log/
+-rw-r--r--   0 liubo      (501) staff       (20)     1719 2021-08-11 01:59:56.000000 feapder-1.9.1b1/tests/spider/log/haha.log
+-rw-r--r--   0 liubo      (501) staff       (20)      296 2022-08-31 02:19:25.000000 feapder-1.9.1b1/tests/spider/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2676 2024-01-09 02:59:22.000000 feapder-1.9.1b1/tests/spider/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.752646 feapder-1.9.1b1/tests/spider/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       42 2021-02-21 15:44:20.000000 feapder-1.9.1b1/tests/spider/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      985 2024-03-18 03:04:19.000000 feapder-1.9.1b1/tests/spider/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      612 2021-08-04 13:29:34.000000 feapder-1.9.1b1/tests/spider/spiders/test_spider2.py
+-rw-r--r--   0 liubo      (501) staff       (20)      320 2021-02-08 08:40:34.000000 feapder-1.9.1b1/tests/spider/table.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.743641 feapder-1.9.1b1/tests/spider-integration/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.744313 feapder-1.9.1b1/tests/spider-integration/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.9.1b1/tests/spider-integration/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      517 2021-12-30 08:51:43.000000 feapder-1.9.1b1/tests/spider-integration/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.9.1b1/tests/spider-integration/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.746754 feapder-1.9.1b1/tests/spider-integration/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.9.1b1/tests/spider-integration/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      470 2023-03-29 13:31:04.000000 feapder-1.9.1b1/tests/spider-integration/spiders/sina_news_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)      456 2021-09-24 05:52:08.000000 feapder-1.9.1b1/tests/spider-integration/spiders/tencent_news_parser.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.753615 feapder-1.9.1b1/tests/task-spider/
+-rw-r--r--   0 liubo      (501) staff       (20)     2133 2024-03-18 02:54:15.000000 feapder-1.9.1b1/tests/task-spider/test_task_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.757910 feapder-1.9.1b1/tests/test-debugger/
+-rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.1b1/tests/test-debugger/.DS_Store
+-rw-r--r--   0 liubo      (501) staff       (20)       81 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test-debugger/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.759039 feapder-1.9.1b1/tests/test-debugger/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test-debugger/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      352 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test-debugger/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     8791 2023-09-15 11:36:15.000000 feapder-1.9.1b1/tests/test-debugger/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.760925 feapder-1.9.1b1/tests/test-debugger/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       33 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test-debugger/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      724 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test-debugger/spiders/test_debugger.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.765163 feapder-1.9.1b1/tests/test-pipeline/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.766820 feapder-1.9.1b1/tests/test-pipeline/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/test-pipeline/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      586 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/test-pipeline/items/spider_data_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1250 2022-09-07 03:39:38.000000 feapder-1.9.1b1/tests/test-pipeline/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1416 2021-04-08 03:41:12.000000 feapder-1.9.1b1/tests/test-pipeline/pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2021-09-02 10:23:23.000000 feapder-1.9.1b1/tests/test-pipeline/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.768618 feapder-1.9.1b1/tests/test-pipeline/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       31 2021-03-30 02:34:20.000000 feapder-1.9.1b1/tests/test-pipeline/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1514 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/test-pipeline/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      851 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/test-pipeline/table.sql
+-rw-r--r--   0 liubo      (501) staff       (20)      796 2023-09-19 02:11:49.000000 feapder-1.9.1b1/tests/test.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3140 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test_dedup.py
+-rw-r--r--   0 liubo      (501) staff       (20)      991 2023-09-21 06:41:27.000000 feapder-1.9.1b1/tests/test_download_midware.py
+-rw-r--r--   0 liubo      (501) staff       (20)      469 2021-09-02 10:22:59.000000 feapder-1.9.1b1/tests/test_lock.py
+-rw-r--r--   0 liubo      (501) staff       (20)      329 2023-06-28 09:47:12.000000 feapder-1.9.1b1/tests/test_log.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1229 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test_metrics.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4678 2021-12-01 05:56:51.000000 feapder-1.9.1b1/tests/test_mongodb.py
+-rw-r--r--   0 liubo      (501) staff       (20)      232 2021-10-14 08:25:11.000000 feapder-1.9.1b1/tests/test_mysqldb.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1086 2023-06-28 09:14:31.000000 feapder-1.9.1b1/tests/test_playwright.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3477 2023-06-28 09:14:30.000000 feapder-1.9.1b1/tests/test_playwright2.py
+-rw-r--r--   0 liubo      (501) staff       (20)      660 2022-10-28 07:20:27.000000 feapder-1.9.1b1/tests/test_rander.py
+-rw-r--r--   0 liubo      (501) staff       (20)      769 2021-07-08 11:51:50.000000 feapder-1.9.1b1/tests/test_rander2.py
+-rw-r--r--   0 liubo      (501) staff       (20)      519 2022-09-14 07:25:07.000000 feapder-1.9.1b1/tests/test_rander3.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1990 2023-09-15 11:36:15.000000 feapder-1.9.1b1/tests/test_rander_xhr.py
+-rw-r--r--   0 liubo      (501) staff       (20)      148 2023-11-22 02:35:16.000000 feapder-1.9.1b1/tests/test_redisdb.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1634 2022-09-25 13:50:01.000000 feapder-1.9.1b1/tests/test_request.py
+-rw-r--r--   0 liubo      (501) staff       (20)      637 2021-04-08 03:41:12.000000 feapder-1.9.1b1/tests/test_spider_params.py
+-rw-r--r--   0 liubo      (501) staff       (20)      593 2022-07-25 12:58:57.000000 feapder-1.9.1b1/tests/test_task.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.769438 feapder-1.9.1b1/tests/test_template/
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.9.1b1/tests/test_template/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      429 2022-05-17 07:19:13.000000 feapder-1.9.1b1/tests/test_tools.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1011 2022-09-07 09:10:23.000000 feapder-1.9.1b1/tests/test_webdriver.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.772086 feapder-1.9.1b1/tests/user_pool/
+-rw-r--r--   0 liubo      (501) staff       (20)     2423 2022-06-10 02:51:23.000000 feapder-1.9.1b1/tests/user_pool/test_gold_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2121 2022-06-10 02:51:23.000000 feapder-1.9.1b1/tests/user_pool/test_guest_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1427 2022-06-10 02:51:23.000000 feapder-1.9.1b1/tests/user_pool/test_normal_user_pool.py
```

### Comparing `feapder-1.9.0b2/LICENSE` & `feapder-1.9.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/PKG-INFO` & `feapder-1.9.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feapder
-Version: 1.9.0b2
+Version: 1.9.1b1
 Summary: feapder是一款支持分布式、批次采集、数据防丢、报警丰富的python爬虫框架
 Home-page: https://github.com/Boris-code/feapder.git
 Author: Boris
 Author-email: feapder@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `feapder-1.9.0b2/README.md` & `feapder-1.9.1b1/README.md`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/__init__.py` & `feapder-1.9.1b1/feapder/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/buffer/item_buffer.py` & `feapder-1.9.1b1/feapder/buffer/item_buffer.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/buffer/request_buffer.py` & `feapder-1.9.1b1/feapder/buffer/request_buffer.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/cmdline.py` & `feapder-1.9.1b1/feapder/commands/cmdline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/create/__init__.py` & `feapder-1.9.1b1/feapder/commands/create/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/create/create_cookies.py` & `feapder-1.9.1b1/feapder/commands/create/create_cookies.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/create/create_init.py` & `feapder-1.9.1b1/feapder/commands/create/create_init.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/create/create_item.py` & `feapder-1.9.1b1/feapder/commands/create/create_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/create/create_json.py` & `feapder-1.9.1b1/feapder/commands/create/create_json.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/create/create_params.py` & `feapder-1.9.1b1/feapder/commands/create/create_params.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/create/create_project.py` & `feapder-1.9.1b1/feapder/commands/create/create_project.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/create/create_setting.py` & `feapder-1.9.1b1/feapder/commands/create/create_setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/create/create_spider.py` & `feapder-1.9.1b1/feapder/commands/create/create_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/create/create_table.py` & `feapder-1.9.1b1/feapder/commands/create/create_table.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/create_builder.py` & `feapder-1.9.1b1/feapder/commands/create_builder.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/retry.py` & `feapder-1.9.1b1/feapder/commands/retry.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/shell.py` & `feapder-1.9.1b1/feapder/commands/shell.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/commands/zip.py` & `feapder-1.9.1b1/feapder/commands/zip.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/core/base_parser.py` & `feapder-1.9.1b1/feapder/core/base_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,39 +9,42 @@
 """
 import os
 
 import feapder.utils.tools as tools
 from feapder.db.mysqldb import MysqlDB
 from feapder.network.item import UpdateItem
 from feapder.utils.log import log
+from feapder.network.request import Request
+from feapder.network.response import Response
+from feapder.utils.perfect_dict import PerfectDict
 
 
 class BaseParser(object):
     def start_requests(self):
         """
         @summary: 添加初始url
         ---------
         ---------
         @result: yield Request()
         """
 
         pass
 
-    def download_midware(self, request):
+    def download_midware(self, request: Request):
         """
         @summary: 下载中间件 可修改请求的一些参数, 或可自定义下载，然后返回 request, response
         ---------
         @param request:
         ---------
         @result: return request / request, response
         """
 
         pass
 
-    def validate(self, request, response):
+    def validate(self, request: Request, response: Response):
         """
         @summary: 校验函数, 可用于校验response是否正确
         若函数内抛出异常，则重试请求
         若返回True 或 None，则进入解析函数
         若返回False，则抛弃当前请求
         可通过request.callback_name 区分不同的回调函数，编写不同的校验逻辑
         ---------
@@ -49,40 +52,40 @@
         @param response:
         ---------
         @result: True / None / False
         """
 
         pass
 
-    def parse(self, request, response):
+    def parse(self, request: Request, response: Response):
         """
         @summary: 默认的解析函数
         ---------
         @param request:
         @param response:
         ---------
         @result:
         """
 
         pass
 
-    def exception_request(self, request, response, e):
+    def exception_request(self, request: Request, response: Response, e: Exception):
         """
         @summary: 请求或者parser里解析出异常的request
         ---------
         @param request:
         @param response:
         @param e: 异常
         ---------
         @result: request / callback / None (返回值必须可迭代)
         """
 
         pass
 
-    def failed_request(self, request, response, e):
+    def failed_request(self, request: Request, response: Response, e: Exception):
         """
         @summary: 超过最大重试次数的request
         可返回修改后的request  若不返回request，则将传进来的request直接人redis的failed表。否则将修改后的request入failed表
         ---------
         @param request:
         @param response:
         @param e: 异常
@@ -131,15 +134,15 @@
         """
         @summary: 添加任务, 每次启动start_monitor 都会调用，且在init_task之前调用
         ---------
         ---------
         @result:
         """
 
-    def start_requests(self, task):
+    def start_requests(self, task: PerfectDict):
         """
         @summary:
         ---------
         @param task: 任务信息 list
         ---------
         @result:
         """
```

### Comparing `feapder-1.9.0b2/feapder/core/collector.py` & `feapder-1.9.1b1/feapder/core/collector.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/core/handle_failed_items.py` & `feapder-1.9.1b1/feapder/core/handle_failed_items.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/core/handle_failed_requests.py` & `feapder-1.9.1b1/feapder/core/handle_failed_requests.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/core/parser_control.py` & `feapder-1.9.1b1/feapder/core/parser_control.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/core/scheduler.py` & `feapder-1.9.1b1/feapder/core/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,31 +13,32 @@
 
 import feapder.setting as setting
 import feapder.utils.tools as tools
 from feapder.buffer.item_buffer import ItemBuffer
 from feapder.buffer.request_buffer import RequestBuffer
 from feapder.core.base_parser import BaseParser
 from feapder.core.collector import Collector
-from feapder.core.handle_failed_requests import HandleFailedRequests
 from feapder.core.handle_failed_items import HandleFailedItems
+from feapder.core.handle_failed_requests import HandleFailedRequests
 from feapder.core.parser_control import ParserControl
 from feapder.db.redisdb import RedisDB
 from feapder.network.item import Item
 from feapder.network.request import Request
 from feapder.utils import metrics
 from feapder.utils.log import log
 from feapder.utils.redis_lock import RedisLock
+from feapder.utils.tail_thread import TailThread
 
 SPIDER_START_TIME_KEY = "spider_start_time"
 SPIDER_END_TIME_KEY = "spider_end_time"
 SPIDER_LAST_TASK_COUNT_RECORD_TIME_KEY = "last_task_count_record_time"
 HEARTBEAT_TIME_KEY = "heartbeat_time"
 
 
-class Scheduler(threading.Thread):
+class Scheduler(TailThread):
     __custom_setting__ = {}
 
     def __init__(
         self,
         redis_key=None,
         thread_count=None,
         begin_callback=None,
```

### Comparing `feapder-1.9.0b2/feapder/core/spiders/air_spider.py` & `feapder-1.9.1b1/feapder/core/spiders/air_spider.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,28 @@
 ---------
 @summary: 基于内存队列的爬虫，不支持分布式
 ---------
 @author: Boris
 @email: boris_liu@foxmail.com
 """
 
-from threading import Thread
-
 import feapder.setting as setting
 import feapder.utils.tools as tools
 from feapder.buffer.item_buffer import ItemBuffer
 from feapder.buffer.request_buffer import AirSpiderRequestBuffer
 from feapder.core.base_parser import BaseParser
 from feapder.core.parser_control import AirSpiderParserControl
 from feapder.db.memorydb import MemoryDB
 from feapder.network.request import Request
 from feapder.utils import metrics
 from feapder.utils.log import log
+from feapder.utils.tail_thread import TailThread
 
 
-class AirSpider(BaseParser, Thread):
+class AirSpider(BaseParser, TailThread):
     __custom_setting__ = {}
 
     def __init__(self, thread_count=None):
         """
         基于内存队列的爬虫，不支持分布式
         :param thread_count: 线程数
         """
```

### Comparing `feapder-1.9.0b2/feapder/core/spiders/batch_spider.py` & `feapder-1.9.1b1/feapder/core/spiders/batch_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/core/spiders/spider.py` & `feapder-1.9.1b1/feapder/core/spiders/spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/core/spiders/task_spider.py` & `feapder-1.9.1b1/feapder/core/spiders/task_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/db/memorydb.py` & `feapder-1.9.1b1/feapder/db/memorydb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/db/mongodb.py` & `feapder-1.9.1b1/feapder/db/mongodb.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @email:  mkdir700@gmail.com
 """
 import re
 from typing import List, Dict, Optional
 from urllib import parse
 
 import pymongo
-from pymongo import MongoClient
+from pymongo import MongoClient, UpdateOne
 from pymongo.collection import Collection
 from pymongo.database import Database
 from pymongo.errors import DuplicateKeyError, BulkWriteError
 
 import feapder.setting as setting
 from feapder.utils.log import log
 
@@ -327,14 +327,78 @@
                     e, condition
                 )
             )
             return False
         else:
             return True
 
+    def update_many(self, coll_name, data: Dict, condition: Dict, upsert: bool = False):
+        """
+        批量更新
+        Args:
+            coll_name: 集合名
+            data: 单条数据 {"xxx":"xxx"}
+            condition: 更新条件 {"_id": "xxxx"}
+            upsert: 数据不存在则插入,默认为 False
+
+        Returns: True / False
+        """
+        try:
+            collection = self.get_collection(coll_name)
+            collection.update_many(condition, {"$set": data}, upsert=upsert)
+        except Exception as e:
+            log.error(
+                """
+                error:{}
+                condition: {}
+            """.format(
+                    e, condition
+                )
+            )
+            return False
+        else:
+            return True
+
+    def update_batch(
+        self,
+        coll_name: str,
+        update_data_list: List[Dict],
+        condition_field: str,
+        upsert: bool = False,
+    ):
+        """
+        批量更新数据
+        Args:
+            coll_name: 集合名
+            update_data_list: 更新数据列表
+            condition_field: 更新条件字段
+            upsert: 数据不存在则插入，默认为 False
+
+        Returns: 更新行数
+
+        """
+        if not update_data_list:
+            return 0
+
+        collection = self.get_collection(coll_name)
+        bulk_operations = []
+
+        for update_data in update_data_list:
+            condition = {condition_field: update_data.get(condition_field)}
+            update_operation = UpdateOne(
+                condition, {"$set": update_data}, upsert=upsert
+            )
+            bulk_operations.append(update_operation)
+        try:
+            result = collection.bulk_write(bulk_operations, ordered=False)
+            return result.modified_count + result.upserted_count
+        except BulkWriteError as e:
+            log.error(f"Bulk write error: {e.details}")
+            return 0
+
     def delete(self, coll_name, condition: Dict) -> bool:
         """
         删除
         Args:
             coll_name: 集合名
             condition: 查找条件
         Returns: True / False
@@ -416,7 +480,19 @@
         index_keys = self.get_index_key(coll_name, index_name)
 
         condition = {key: data.get(key) for key in index_keys}
         return condition
 
     def __getattr__(self, name):
         return getattr(self.db, name)
+
+
+if __name__ == "__main__":
+    update_data_list = [{"_id": "1", "status": 1}, {"_id": "2", "status": 1}]
+    mongo = MongoDB()
+    updated_count = mongo.update_batch("your_table_name", update_data_list, "_id")
+    print(f"Updated {updated_count} documents.")
+
+    id_list = ["1", "2"]
+    result = mongo.update_many(
+        "your_table_name", {"status": 1}, {"_id": {"$in": id_list}}
+    )
```

### Comparing `feapder-1.9.0b2/feapder/db/mysqldb.py` & `feapder-1.9.1b1/feapder/db/mysqldb.py`

 * *Files 9% similar despite different names*

```diff
@@ -296,103 +296,110 @@
                 % (e, sql)
             )
         finally:
             self.close_connection(conn, cursor)
 
         return affect_count
 
-    def add_batch_smart(self, table, datas: List[Dict], **kwargs):
+    def add_batch_smart(self, table, datas: List[Dict], **kwargs) -> int:
         """
         批量添加数据, 直接传递list格式的数据，不用拼sql
         Args:
             table: 表名
             datas: 列表 [{}, {}, {}]
             **kwargs:
 
         Returns: 添加行数
 
         """
         sql, datas = make_batch_sql(table, datas, **kwargs)
         return self.add_batch(sql, datas)
 
-    def update(self, sql):
+    def update(self, sql) -> int:
+        affect_count = None
         conn, cursor = None, None
 
         try:
             conn, cursor = self.get_connection()
-            cursor.execute(sql)
+            affect_count = cursor.execute(sql)
             conn.commit()
         except Exception as e:
             log.error(
                 """
                 error:%s
                 sql:  %s
             """
                 % (e, sql)
             )
-            return False
-        else:
-            return True
         finally:
             self.close_connection(conn, cursor)
 
-    def update_smart(self, table, data: Dict, condition):
+        return affect_count
+
+    def update_smart(self, table, data: Dict, condition) -> int:
         """
         更新, 不用拼sql
         Args:
             table: 表名
             data: 数据 {"xxx":"xxx"}
             condition: 更新条件 where后面的条件，如 condition='status=1'
 
-        Returns: True / False
+        Returns: 影响行数
 
         """
         sql = make_update_sql(table, data, condition)
         return self.update(sql)
 
-    def delete(self, sql):
+    def delete(self, sql) -> int:
         """
         删除
         Args:
             sql:
 
-        Returns: True / False
+        Returns: 影响行数
 
         """
+        affect_count = None
         conn, cursor = None, None
         try:
             conn, cursor = self.get_connection()
-            cursor.execute(sql)
+            affect_count = cursor.execute(sql)
             conn.commit()
         except Exception as e:
             log.error(
                 """
                 error:%s
                 sql:  %s
             """
                 % (e, sql)
             )
-            return False
-        else:
-            return True
         finally:
             self.close_connection(conn, cursor)
 
-    def execute(self, sql):
+        return affect_count
+
+    def execute(self, sql) -> int:
+        """
+
+        Args:
+            sql:
+
+        Returns: 影响行数
+        """
+        affect_count = None
         conn, cursor = None, None
         try:
             conn, cursor = self.get_connection()
-            cursor.execute(sql)
+            affect_count = cursor.execute(sql)
             conn.commit()
         except Exception as e:
             log.error(
                 """
                 error:%s
                 sql:  %s
             """
                 % (e, sql)
             )
-            return False
-        else:
-            return True
         finally:
             self.close_connection(conn, cursor)
+
+        return affect_count
```

### Comparing `feapder-1.9.0b2/feapder/db/redisdb.py` & `feapder-1.9.1b1/feapder/db/redisdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 ---------
 @summary: 操作redis数据库
 ---------
 @author: Boris
 """
 import os
 import time
+from typing import Union, List
 
 import redis
 from redis.connection import Encoder as _Encoder
 from redis.exceptions import ConnectionError, TimeoutError
 from redis.exceptions import DataError
 from redis.sentinel import Sentinel
 
@@ -739,35 +740,49 @@
 
     def hget_count(self, table):
         return self._redis.hlen(table)
 
     def hkeys(self, table):
         return self._redis.hkeys(table)
 
-    def setbit(self, table, offsets, values):
+    def hvals(self, key):
+        return self._redis.hvals(key)
+
+    def setbit(
+        self, table, offsets: Union[int, List[int]], values: Union[int, List[int]]
+    ):
         """
-        设置字符串数组某一位的值， 返回之前的值
-        @param table:
+        设置字符串数组某一位的值，返回之前的值
+        @param table: Redis key
         @param offsets: 支持列表或单个值
         @param values: 支持列表或单个值
         @return: list / 单个值
         """
         if isinstance(offsets, list):
-            if not isinstance(values, list):
-                values = [values] * len(offsets)
+            if isinstance(values, int):
+                # 使用lua脚本，数据是一起传给redis的，降低了网络开销，但redis会阻塞
+                script = """
+                            local value = table.remove(ARGV, 1)
+                            local offsets = ARGV
+                            local results = {}
+                            for i, offset in ipairs(offsets) do
+                                results[i] = redis.call('SETBIT', KEYS[1], offset, value)
+                            end
+                            return results
+                        """
+                return self._redis.eval(script, 1, table, values, *offsets)
             else:
                 assert len(offsets) == len(values), "offsets值要与values值一一对应"
+                pipe = self._redis.pipeline()
+                pipe.multi()
 
-            pipe = self._redis.pipeline()
-            pipe.multi()
-
-            for offset, value in zip(offsets, values):
-                pipe.setbit(table, offset, value)
+                for offset, value in zip(offsets, values):
+                    pipe.setbit(table, offset, value)
 
-            return pipe.execute()
+                return pipe.execute()
 
         else:
             return self._redis.setbit(table, offsets, values)
 
     def getbit(self, table, offsets):
         """
         取字符串数组某一位的值
@@ -786,14 +801,28 @@
         else:
             return self._redis.getbit(table, offsets)
 
     def bitcount(self, table):
         return self._redis.bitcount(table)
 
     def strset(self, table, value, **kwargs):
+        """
+        设置键值
+        Args:
+            table:
+            value:
+            **kwargs:
+                ex: Union[None, int, timedelta] = ..., 设置键的过期时间为 second 秒
+                px: Union[None, int, timedelta] = ..., 设置键的过期时间为 millisecond 毫秒
+                nx: bool = ..., 只有键不存在时，才对键进行设置操作
+                xx: bool = ..., 只有键已经存在时，才对键进行设置操作
+                keepttl: bool = ..., 保留键的过期时间
+        Returns:
+
+        """
         return self._redis.set(table, value, **kwargs)
 
     def str_incrby(self, table, value):
         return self._redis.incrby(table, value)
 
     def strget(self, table):
         return self._redis.get(table)
```

### Comparing `feapder-1.9.0b2/feapder/dedup/__init__.py` & `feapder-1.9.1b1/feapder/dedup/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/dedup/basefilter.py` & `feapder-1.9.1b1/feapder/dedup/basefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/dedup/bitarray.py` & `feapder-1.9.1b1/feapder/dedup/bitarray.py`

 * *Files 7% similar despite different names*

```diff
@@ -123,15 +123,26 @@
     def set(self, offsets, values):
         """
         设置字符串数字某一位的值， 返回之前的值
         @param offsets: 支持列表或单个值
         @param values: 支持列表或单个值
         @return: list / 单个值
         """
-        return self.redis_db.setbit(self.name, offsets, values)
+        # 对offsets进行分片，最大100000个
+        results = []
+        batch_size = 170000
+        for i in range(0, len(offsets), batch_size):
+            results.extend(
+                self.redis_db.setbit(
+                    self.name,
+                    offsets[i : i + batch_size],
+                    values[i : i + batch_size] if isinstance(values, list) else values,
+                )
+            )
+        return results
 
     def get(self, offsets):
         return self.redis_db.getbit(self.name, offsets)
 
     def count(self, value=True):
         # 先查redis的缓存，若没有 在统计数量
         count = self.redis_db.strget(self.count_cached_name)
```

### Comparing `feapder-1.9.0b2/feapder/dedup/bloomfilter.py` & `feapder-1.9.1b1/feapder/dedup/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/dedup/expirefilter.py` & `feapder-1.9.1b1/feapder/dedup/expirefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/dedup/litefilter.py` & `feapder-1.9.1b1/feapder/dedup/litefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/downloader/_playwright.py` & `feapder-1.9.1b1/feapder/network/downloader/_playwright.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/downloader/_requests.py` & `feapder-1.9.1b1/feapder/network/downloader/_requests.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/downloader/_selenium.py` & `feapder-1.9.1b1/feapder/network/downloader/_selenium.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/downloader/base.py` & `feapder-1.9.1b1/feapder/network/downloader/base.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/item.py` & `feapder-1.9.1b1/feapder/network/item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/proxy_pool/base.py` & `feapder-1.9.1b1/feapder/network/proxy_pool/base.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/proxy_pool/proxy_pool.py` & `feapder-1.9.1b1/feapder/network/proxy_pool/proxy_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/proxy_pool_old.py` & `feapder-1.9.1b1/feapder/network/proxy_pool_old.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/request.py` & `feapder-1.9.1b1/feapder/network/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,20 @@
         @return:
         """
         self.__dict__[key] = value
 
         if key in self.__class__.__REQUEST_ATTRS__:
             self.requests_kwargs[key] = value
 
+    # def __getattr__(self, item):
+    #     try:
+    #         return self.__dict__[item]
+    #     except:
+    #         raise AttributeError("Request has no attribute %s" % item)
+
     def __lt__(self, other):
         return self.priority < other.priority
 
     @property
     def _proxies_pool(self):
         if not self.__class__.proxies_pool:
             self.__class__.proxies_pool = tools.import_cls(setting.PROXY_POOL)()
```

### Comparing `feapder-1.9.0b2/feapder/network/response.py` & `feapder-1.9.1b1/feapder/network/response.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/selector.py` & `feapder-1.9.1b1/feapder/network/selector.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/user_agent.py` & `feapder-1.9.1b1/feapder/network/user_agent.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/user_pool/base_user_pool.py` & `feapder-1.9.1b1/feapder/network/user_pool/base_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/user_pool/gold_user_pool.py` & `feapder-1.9.1b1/feapder/network/user_pool/gold_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/user_pool/guest_user_pool.py` & `feapder-1.9.1b1/feapder/network/user_pool/guest_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/network/user_pool/normal_user_pool.py` & `feapder-1.9.1b1/feapder/network/user_pool/normal_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/pipelines/__init__.py` & `feapder-1.9.1b1/feapder/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/pipelines/console_pipeline.py` & `feapder-1.9.1b1/feapder/pipelines/console_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/pipelines/mongo_pipeline.py` & `feapder-1.9.1b1/feapder/pipelines/mongo_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/pipelines/mysql_pipeline.py` & `feapder-1.9.1b1/feapder/pipelines/mysql_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/setting.py` & `feapder-1.9.1b1/feapder/setting.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,16 @@
     filter_type=3,  # 永久去重（BloomFilter） = 1 、内存去重（MemoryFilter） = 2、 临时去重（ExpireFilter）= 3、 轻量去重（LiteFilter）= 4
     expire_time=2592000,  # 过期时间1个月
 )
 
 # 报警 支持钉钉、飞书、企业微信、邮件
 # 钉钉报警
 DINGDING_WARNING_URL = ""  # 钉钉机器人api
-DINGDING_WARNING_PHONE = ""  # 报警人 支持列表，可指定多个
+DINGDING_WARNING_PHONE = ""  # 被@的群成员手机号，支持列表，可指定多个。
+DINGDING_WARNING_USER_ID = ""  # 被@的群成员userId，支持列表，可指定多个
 DINGDING_WARNING_ALL = False  # 是否提示所有人， 默认为False
 DINGDING_WARNING_SECRET = None  # 加签密钥
 # 飞书报警
 # https://open.feishu.cn/document/ukTMukTMukTM/ucTM5YjL3ETO24yNxkjN#e1cdee9f
 FEISHU_WARNING_URL = ""  # 飞书机器人api
 FEISHU_WARNING_USER = None  # 报警人 {"open_id":"ou_xxxxx", "name":"xxxx"} 或 [{"open_id":"ou_xxxxx", "name":"xxxx"}]
 FEISHU_WARNING_ALL = False  # 是否提示所有人， 默认为False
```

### Comparing `feapder-1.9.0b2/feapder/templates/.DS_Store` & `feapder-1.9.1b1/feapder/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/templates/air_spider_template.tmpl` & `feapder-1.9.1b1/feapder/templates/air_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/templates/batch_spider_template.tmpl` & `feapder-1.9.1b1/feapder/templates/batch_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/templates/project_template/.DS_Store` & `feapder-1.9.1b1/feapder/templates/project_template/.DS_Store`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/templates/project_template/CHECK_DATA.md` & `feapder-1.9.1b1/feapder/templates/project_template/CHECK_DATA.md`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/templates/project_template/main.py` & `feapder-1.9.1b1/feapder/templates/project_template/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/templates/project_template/setting.py` & `feapder-1.9.1b1/feapder/templates/project_template/setting.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,15 +143,16 @@
 #     filter_type=3,  # 永久去重（BloomFilter） = 1 、内存去重（MemoryFilter） = 2、 临时去重（ExpireFilter）= 3、 轻量去重（LiteFilter）= 4
 #     expire_time=2592000,  # 过期时间1个月
 # )
 #
 # # 报警 支持钉钉、飞书、企业微信、邮件
 # # 钉钉报警
 # DINGDING_WARNING_URL = ""  # 钉钉机器人api
-# DINGDING_WARNING_PHONE = ""  # 报警人 支持列表，可指定多个
+# DINGDING_WARNING_PHONE = ""  # 被@的群成员手机号，支持列表，可指定多个。
+# DINGDING_WARNING_USER_ID = ""  # 被@的群成员userId，支持列表，可指定多个
 # DINGDING_WARNING_ALL = False  # 是否提示所有人， 默认为False
 # DINGDING_WARNING_SECRET = None  # 加签密钥
 # # 飞书报警
 # # https://open.feishu.cn/document/ukTMukTMukTM/ucTM5YjL3ETO24yNxkjN#e1cdee9f
 # FEISHU_WARNING_URL = ""  # 飞书机器人api
 # FEISHU_WARNING_USER = None  # 报警人 {"open_id":"ou_xxxxx", "name":"xxxx"} 或 [{"open_id":"ou_xxxxx", "name":"xxxx"}]
 # FEISHU_WARNING_ALL = False  # 是否提示所有人， 默认为False
```

### Comparing `feapder-1.9.0b2/feapder/templates/spider_template.tmpl` & `feapder-1.9.1b1/feapder/templates/spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/templates/task_spider_template.tmpl` & `feapder-1.9.1b1/feapder/templates/task_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/utils/custom_argparse.py` & `feapder-1.9.1b1/feapder/utils/custom_argparse.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/utils/email_sender.py` & `feapder-1.9.1b1/feapder/utils/email_sender.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/utils/js/intercept.js` & `feapder-1.9.1b1/feapder/utils/js/intercept.js`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/utils/js/stealth.min.js` & `feapder-1.9.1b1/feapder/utils/js/stealth.min.js`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/utils/log.py` & `feapder-1.9.1b1/feapder/utils/log.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/utils/metrics.py` & `feapder-1.9.1b1/feapder/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/utils/perfect_dict.py` & `feapder-1.9.1b1/feapder/utils/perfect_dict.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/utils/redis_lock.py` & `feapder-1.9.1b1/feapder/utils/redis_lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     def __enter__(self):
         if not self.locked:
             self.acquire()
             if self.locked:
                 # 延长锁的时间
                 thread = threading.Thread(target=self.prolong_life)
-                thread.setDaemon(True)
+                thread.daemon = True
                 thread.start()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop_prolong_life = True
         self.release()
 
@@ -79,19 +79,20 @@
             # 尝试加锁
             if self.redis_conn.set(self.lock_key, time.time(), nx=True, ex=5):
                 self.locked = True
                 break
 
             if self.wait_timeout > 0:
                 if time.time() - start > self.wait_timeout:
-                    log.info("加锁失败")
+                    log.debug("获取锁失败")
                     break
             else:
+                log.debug("获取锁失败")
                 break
-            log.debug("等待加锁: {} wait:{}".format(self, time.time() - start))
+            log.debug("等待锁: {} wait:{}".format(self, time.time() - start))
             if self.wait_timeout > 10:
                 time.sleep(5)
             else:
                 time.sleep(1)
         return
 
     def release(self):
```

### Comparing `feapder-1.9.0b2/feapder/utils/tools.py` & `feapder-1.9.1b1/feapder/utils/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 Created on 2018-09-06 14:21
 ---------
 @summary: 工具
 ---------
 @author: Boris
 @email: boris_liu@foxmail.com
 """
-import hmac
 import asyncio
 import base64
 import calendar
 import codecs
 import configparser  # 读配置文件的
 import datetime
 import functools
 import hashlib
+import hmac
 import html
 import importlib
 import json
 import os
 import pickle
 import random
 import re
@@ -2463,43 +2463,73 @@
         else:
             freq_limit_record[key] = time.time()
 
     return False
 
 
 def dingding_warning(
-    message, message_prefix=None, rate_limit=None, url=None, user_phone=None, secret=None
+    message,
+    *,
+    message_prefix=None,
+    rate_limit=None,
+    url=None,
+    user_phone=None,
+    user_id=None,
+    secret=None,
 ):
+    """
+    钉钉报警，user_phone与user_id 二选一即可
+    Args:
+        message:
+        message_prefix: 消息摘要，用于去重
+        rate_limit: 包名频率，单位秒，相同的报警内容在rate_limit时间内只会报警一次
+        url: 钉钉报警url
+        user_phone: 被@的群成员手机号，支持列表，可指定多个。
+        user_id: 被@的群成员userId，支持列表，可指定多个
+        secret: 钉钉报警加签密钥
+    Returns:
+
+    """
     # 为了加载最新的配置
     rate_limit = rate_limit if rate_limit is not None else setting.WARNING_INTERVAL
     url = url or setting.DINGDING_WARNING_URL
     user_phone = user_phone or setting.DINGDING_WARNING_PHONE
+    user_id = user_id or setting.DINGDING_WARNING_USER_ID
     secret = secret or setting.DINGDING_WARNING_SECRET
     if secret:
         timestamp = str(round(time.time() * 1000))
-        secret_enc = secret.encode('utf-8')
-        string_to_sign_enc = f'{timestamp}\n{secret}'.encode('utf-8')
-        hmac_code = hmac.new(secret_enc, string_to_sign_enc, digestmod=hashlib.sha256).digest()
+        secret_enc = secret.encode("utf-8")
+        string_to_sign_enc = f"{timestamp}\n{secret}".encode("utf-8")
+        hmac_code = hmac.new(
+            secret_enc, string_to_sign_enc, digestmod=hashlib.sha256
+        ).digest()
         sign = urllib.parse.quote_plus(base64.b64encode(hmac_code))
         url = f"{url}&timestamp={timestamp}&sign={sign}"
 
     if not all([url, message]):
         return
 
     if reach_freq_limit(rate_limit, url, user_phone, message_prefix or message):
         log.info("报警时间间隔过短，此次报警忽略。 内容 {}".format(message))
         return
 
     if isinstance(user_phone, str):
         user_phone = [user_phone] if user_phone else []
 
+    if isinstance(user_id, str):
+        user_id = [user_id] if user_id else []
+
     data = {
         "msgtype": "text",
         "text": {"content": message},
-        "at": {"atMobiles": user_phone, "isAtAll": setting.DINGDING_WARNING_ALL},
+        "at": {
+            "atMobiles": user_phone,
+            "atUserIds": user_id,
+            "isAtAll": setting.DINGDING_WARNING_ALL,
+        },
     }
 
     headers = {"Content-Type": "application/json"}
 
     try:
         response = requests.post(
             url, headers=headers, data=json.dumps(data).encode("utf8")
```

### Comparing `feapder-1.9.0b2/feapder/utils/webdriver/playwright_driver.py` & `feapder-1.9.1b1/feapder/utils/webdriver/playwright_driver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/utils/webdriver/selenium_driver.py` & `feapder-1.9.1b1/feapder/utils/webdriver/selenium_driver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/utils/webdriver/webdirver.py` & `feapder-1.9.1b1/feapder/utils/webdriver/webdirver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder/utils/webdriver/webdriver_pool.py` & `feapder-1.9.1b1/feapder/utils/webdriver/webdriver_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/feapder.egg-info/PKG-INFO` & `feapder-1.9.1b1/feapder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feapder
-Version: 1.9.0b2
+Version: 1.9.1b1
 Summary: feapder是一款支持分布式、批次采集、数据防丢、报警丰富的python爬虫框架
 Home-page: https://github.com/Boris-code/feapder.git
 Author: Boris
 Author-email: feapder@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `feapder-1.9.0b2/feapder.egg-info/SOURCES.txt` & `feapder-1.9.1b1/feapder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 feapder/utils/__init__.py
 feapder/utils/custom_argparse.py
 feapder/utils/email_sender.py
 feapder/utils/log.py
 feapder/utils/metrics.py
 feapder/utils/perfect_dict.py
 feapder/utils/redis_lock.py
+feapder/utils/tail_thread.py
 feapder/utils/tools.py
 feapder/utils/js/intercept.js
 feapder/utils/js/stealth.min.js
 feapder/utils/webdriver/__init__.py
 feapder/utils/webdriver/playwright_driver.py
 feapder/utils/webdriver/selenium_driver.py
 feapder/utils/webdriver/webdirver.py
```

### Comparing `feapder-1.9.0b2/setup.py` & `feapder-1.9.1b1/setup.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/air-spider/test_air_spider.py` & `feapder-1.9.1b1/tests/air-spider/test_air_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/air-spider/test_air_spider_filter.py` & `feapder-1.9.1b1/tests/air-spider/test_air_spider_filter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/air-spider/test_air_spider_item.py` & `feapder-1.9.1b1/tests/air-spider/test_air_spider_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/air-spider/test_render_spider.py` & `feapder-1.9.1b1/tests/air-spider/test_render_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/batch-spider/items/spider_data_item.py` & `feapder-1.9.1b1/tests/batch-spider/items/spider_data_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/batch-spider/main.py` & `feapder-1.9.1b1/tests/batch-spider/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/batch-spider/setting.py` & `feapder-1.9.1b1/tests/batch-spider/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/batch-spider/spiders/test_spider.py` & `feapder-1.9.1b1/tests/batch-spider/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/batch-spider/table.sql` & `feapder-1.9.1b1/tests/batch-spider/table.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/batch-spider-integration/batch_spider_integration_task.sql` & `feapder-1.9.1b1/tests/batch-spider-integration/batch_spider_integration_task.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/batch-spider-integration/main.py` & `feapder-1.9.1b1/tests/batch-spider-integration/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/batch-spider-integration/setting.py` & `feapder-1.9.1b1/tests/batch-spider-integration/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/batch-spider-integration/spiders/sina_news_parser.py` & `feapder-1.9.1b1/tests/batch-spider-integration/spiders/sina_news_parser.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/batch-spider-integration/spiders/tencent_news_parser.py` & `feapder-1.9.1b1/tests/batch-spider-integration/spiders/tencent_news_parser.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/jd_spider.py` & `feapder-1.9.1b1/tests/jd_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/mongo_spider.py` & `feapder-1.9.1b1/tests/mongo_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/spider/log/haha.log` & `feapder-1.9.1b1/tests/spider/log/haha.log`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/spider/setting.py` & `feapder-1.9.1b1/tests/spider/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/spider/spiders/test_spider.py` & `feapder-1.9.1b1/tests/spider/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/spider/spiders/test_spider2.py` & `feapder-1.9.1b1/tests/spider/spiders/test_spider2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/spider-integration/main.py` & `feapder-1.9.1b1/tests/spider-integration/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/spider-integration/setting.py` & `feapder-1.9.1b1/tests/spider-integration/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/task-spider/test_task_spider.py` & `feapder-1.9.1b1/tests/task-spider/test_task_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test-debugger/.DS_Store` & `feapder-1.9.1b1/tests/test-debugger/.DS_Store`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test-debugger/setting.py` & `feapder-1.9.1b1/tests/test-debugger/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test-debugger/spiders/test_debugger.py` & `feapder-1.9.1b1/tests/test-debugger/spiders/test_debugger.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test-pipeline/items/spider_data_item.py` & `feapder-1.9.1b1/tests/test-pipeline/items/spider_data_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test-pipeline/main.py` & `feapder-1.9.1b1/tests/test-pipeline/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test-pipeline/pipeline.py` & `feapder-1.9.1b1/tests/test-pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test-pipeline/setting.py` & `feapder-1.9.1b1/tests/test-pipeline/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test-pipeline/spiders/test_spider.py` & `feapder-1.9.1b1/tests/test-pipeline/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test-pipeline/table.sql` & `feapder-1.9.1b1/tests/test-pipeline/table.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test.py` & `feapder-1.9.1b1/tests/test.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_dedup.py` & `feapder-1.9.1b1/tests/test_dedup.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_download_midware.py` & `feapder-1.9.1b1/tests/test_download_midware.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_metrics.py` & `feapder-1.9.1b1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_mongodb.py` & `feapder-1.9.1b1/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_playwright.py` & `feapder-1.9.1b1/tests/test_playwright.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_playwright2.py` & `feapder-1.9.1b1/tests/test_playwright2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_rander.py` & `feapder-1.9.1b1/tests/test_rander.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_rander2.py` & `feapder-1.9.1b1/tests/test_rander2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_rander3.py` & `feapder-1.9.1b1/tests/test_rander3.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_rander_xhr.py` & `feapder-1.9.1b1/tests/test_rander_xhr.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_request.py` & `feapder-1.9.1b1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_spider_params.py` & `feapder-1.9.1b1/tests/test_spider_params.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_task.py` & `feapder-1.9.1b1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_template/test_spider.py` & `feapder-1.9.1b1/tests/test_template/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/test_webdriver.py` & `feapder-1.9.1b1/tests/test_webdriver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/user_pool/test_gold_user_pool.py` & `feapder-1.9.1b1/tests/user_pool/test_gold_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/user_pool/test_guest_user_pool.py` & `feapder-1.9.1b1/tests/user_pool/test_guest_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.0b2/tests/user_pool/test_normal_user_pool.py` & `feapder-1.9.1b1/tests/user_pool/test_normal_user_pool.py`

 * *Files identical despite different names*

