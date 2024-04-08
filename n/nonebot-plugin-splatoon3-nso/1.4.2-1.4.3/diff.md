# Comparing `tmp/nonebot_plugin_splatoon3_nso-1.4.2.tar.gz` & `tmp/nonebot_plugin_splatoon3_nso-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_splatoon3_nso-1.4.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_splatoon3_nso-1.4.3.tar", max compression
```

## Comparing `nonebot_plugin_splatoon3_nso-1.4.2.tar` & `nonebot_plugin_splatoon3_nso-1.4.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1066 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/LICENSE
--rw-r--r--   0        0        0    12316 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/README.md
--rw-r--r--   0        0        0     5589 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/__init__.py
--rw-r--r--   0        0        0     2817 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/config.py
--rw-r--r--   0        0        0        0 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/__init__.py
--rw-r--r--   0        0        0    18107 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/data_source.py
--rw-r--r--   0        0        0     7111 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/db_sqlite.py
--rw-r--r--   0        0        0     5015 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/transfer.py
--rw-r--r--   0        0        0     3721 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/utils.py
--rw-r--r--   0        0        0      439 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/__init__.py
--rw-r--r--   0        0        0     4095 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/admin.py
--rw-r--r--   0        0        0    16296 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/b_or_c_tools.py
--rw-r--r--   0        0        0    19576 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/battle.py
--rw-r--r--   0        0        0     7951 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/coop.py
--rw-r--r--   0        0        0     5203 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/__init__.py
--rw-r--r--   0        0        0     3613 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/else_cron.py
--rw-r--r--   0        0        0     3545 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/event_top.py
--rw-r--r--   0        0        0    11040 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/report.py
--rw-r--r--   0        0        0     9115 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/stat_ink.py
--rw-r--r--   0        0        0     2874 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/user_friends.py
--rw-r--r--   0        0        0      671 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/utils.py
--rw-r--r--   0        0        0     6460 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/x_player.py
--rw-r--r--   0        0        0     8411 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/history.py
--rw-r--r--   0        0        0    14441 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/last.py
--rw-r--r--   0        0        0    15462 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/login.py
--rw-r--r--   0        0        0    21068 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/my.py
--rw-r--r--   0        0        0    13044 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/push.py
--rw-r--r--   0        0        0     3433 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/qq_md.py
--rw-r--r--   0        0        0     7951 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/report.py
--rw-r--r--   0        0        0     2747 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/screenshot.py
--rw-r--r--   0        0        0    12992 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/send_msg.py
--rw-r--r--   0        0        0    10179 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/top.py
--rw-r--r--   0        0        0    10994 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/utils.py
--rw-r--r--   0        0        0    31357 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/en-GB.json
--rw-r--r--   0        0        0    36257 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/ja-JP.json
--rw-r--r--   0        0        0    34122 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/ko-KR.json
--rw-r--r--   0        0        0    30879 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/zh-CN.json
--rw-r--r--   0        0        0    31079 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/zh-TW.json
--rw-r--r--   0        0        0      708 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/md.css
--rw-r--r--   0        0        0   461502 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/sp3bot-login.gif
--rw-r--r--   0        0        0        0 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/__init__.py
--rw-r--r--   0        0        0    26214 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/iksm.py
--rw-r--r--   0        0        0     5301 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/splatnet_image.py
--rw-r--r--   0        0        0    22564 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/splatoon.py
--rw-r--r--   0        0        0     6299 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/utils.py
--rw-r--r--   0        0        0     4077 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/util.py
--rw-r--r--   0        0        0       61 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/__init__.py
--rw-r--r--   0        0        0     3448 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/bot.py
--rw-r--r--   0        0        0     6127 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/http.py
--rw-r--r--   0        0        0     4106 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/time.py
--rw-r--r--   0        0        0     1838 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/utils.py
--rw-r--r--   0        0        0      969 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/pyproject.toml
--rw-r--r--   0        0        0    13429 1970-01-01 00:00:00.000000 nonebot_plugin_splatoon3_nso-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-08 09:08:38.669298 nonebot_plugin_splatoon3_nso-1.4.3/LICENSE
+-rw-r--r--   0        0        0    12316 2024-04-08 09:08:38.669298 nonebot_plugin_splatoon3_nso-1.4.3/README.md
+-rw-r--r--   0        0        0     5589 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/__init__.py
+-rw-r--r--   0        0        0     2817 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/config.py
+-rw-r--r--   0        0        0        0 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/data/__init__.py
+-rw-r--r--   0        0        0    18107 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/data/data_source.py
+-rw-r--r--   0        0        0     7111 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/data/db_sqlite.py
+-rw-r--r--   0        0        0     5015 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/data/transfer.py
+-rw-r--r--   0        0        0     3721 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/data/utils.py
+-rw-r--r--   0        0        0      439 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/__init__.py
+-rw-r--r--   0        0        0     4095 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/admin.py
+-rw-r--r--   0        0        0    16296 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/b_or_c_tools.py
+-rw-r--r--   0        0        0    19576 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/battle.py
+-rw-r--r--   0        0        0     8115 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/coop.py
+-rw-r--r--   0        0        0     5203 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/__init__.py
+-rw-r--r--   0        0        0     3613 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/else_cron.py
+-rw-r--r--   0        0        0     3545 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/event_top.py
+-rw-r--r--   0        0        0    11040 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/report.py
+-rw-r--r--   0        0        0     9115 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/stat_ink.py
+-rw-r--r--   0        0        0     2874 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/user_friends.py
+-rw-r--r--   0        0        0      671 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/utils.py
+-rw-r--r--   0        0        0     6460 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/x_player.py
+-rw-r--r--   0        0        0     8411 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/history.py
+-rw-r--r--   0        0        0    14441 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/last.py
+-rw-r--r--   0        0        0    15509 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/login.py
+-rw-r--r--   0        0        0    21068 2024-04-08 09:08:38.673298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/my.py
+-rw-r--r--   0        0        0    13044 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/push.py
+-rw-r--r--   0        0        0     3433 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/qq_md.py
+-rw-r--r--   0        0        0     7951 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/report.py
+-rw-r--r--   0        0        0     2747 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/screenshot.py
+-rw-r--r--   0        0        0    12992 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/send_msg.py
+-rw-r--r--   0        0        0    10179 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/top.py
+-rw-r--r--   0        0        0    10994 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/utils.py
+-rw-r--r--   0        0        0    31357 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/i18n/en-GB.json
+-rw-r--r--   0        0        0    36257 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/i18n/ja-JP.json
+-rw-r--r--   0        0        0    34122 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/i18n/ko-KR.json
+-rw-r--r--   0        0        0    30879 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/i18n/zh-CN.json
+-rw-r--r--   0        0        0    31079 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/i18n/zh-TW.json
+-rw-r--r--   0        0        0      708 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/md.css
+-rw-r--r--   0        0        0   461502 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/sp3bot-login.gif
+-rw-r--r--   0        0        0        0 2024-04-08 09:08:38.677298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/s3s/__init__.py
+-rw-r--r--   0        0        0    26214 2024-04-08 09:08:38.681298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/s3s/iksm.py
+-rw-r--r--   0        0        0     5301 2024-04-08 09:08:38.681298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/s3s/splatnet_image.py
+-rw-r--r--   0        0        0    22564 2024-04-08 09:08:38.681298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/s3s/splatoon.py
+-rw-r--r--   0        0        0     6299 2024-04-08 09:08:38.681298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/s3s/utils.py
+-rw-r--r--   0        0        0     4077 2024-04-08 09:08:38.681298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/util.py
+-rw-r--r--   0        0        0       61 2024-04-08 09:08:38.681298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/utils/__init__.py
+-rw-r--r--   0        0        0     3448 2024-04-08 09:08:38.681298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/utils/bot.py
+-rw-r--r--   0        0        0     6127 2024-04-08 09:08:38.681298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/utils/http.py
+-rw-r--r--   0        0        0     4106 2024-04-08 09:08:38.681298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/utils/time.py
+-rw-r--r--   0        0        0     1838 2024-04-08 09:08:38.681298 nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/utils/utils.py
+-rw-r--r--   0        0        0      969 2024-04-08 09:08:38.681298 nonebot_plugin_splatoon3_nso-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0    13429 1970-01-01 00:00:00.000000 nonebot_plugin_splatoon3_nso-1.4.3/PKG-INFO
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/LICENSE` & `nonebot_plugin_splatoon3_nso-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/README.md` & `nonebot_plugin_splatoon3_nso-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/__init__.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/config.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/data_source.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/data/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/db_sqlite.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/data/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/transfer.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/data/transfer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/utils.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/data/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/admin.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/admin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/b_or_c_tools.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/b_or_c_tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/battle.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/battle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/coop.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/coop.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,12 +180,17 @@
         p_name = f'~~我是马赛克~~'
 
     player_code, player_name = get_game_sp_id_and_name(p['player'])
     if is_myself:
         p_name, icon = await get_user_name_color(p_name, player_code, is_myself=True)
     else:
         p_name, icon = await get_user_name_color(player_name, player_code)
+    # 辅助投蛋数
+    if p['goldenAssistCount']:
+        golden = f"{p['goldenDeliverCount']}({p['goldenAssistCount']})"
+    else:
+        golden = f"{p['goldenDeliverCount']}"
 
-    t = f"|x{p['defeatEnemyCount']}| {p['goldenDeliverCount']} |{p['rescuedCount']}d |" \
+    t = f"|x{p['defeatEnemyCount']}| {golden} |{p['rescuedCount']}d |" \
         f"{p['rescueCount']}r|{p['deliverCount']} | {uniform} {p_name}|{weapon}|{icon}|"
 
     return t
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/__init__.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/else_cron.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/else_cron.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/event_top.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/event_top.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/report.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/report.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/stat_ink.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/stat_ink.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/user_friends.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/user_friends.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/utils.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/x_player.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/cron/x_player.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/history.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/history.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/last.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/last.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/login.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     logger.info(f'get login url: {url}')
     logger.info(f'auth_code_verifier: {auth_code_verifier}')
     if url:
         msg = ''
         if isinstance(bot, Tg_Bot):
             msg = "Navigate to this URL in your browser:\n" \
                   f"{url}"
+            await bot.send(event, message=msg)
 
         elif isinstance(bot, All_BOT):
             msg = "风险告知:小鱿鱿所使用的nso查询本质上为第三方nso软件，此类第三方调用可能会导致nso鱿鱼圈被封禁，目前未观察到游戏连带被禁的情况。(要怪请去怪乌贼研究所)\n" \
                   "若继续完成以下登录流程，则视为您已知晓此风险并继续使用nso查询\n\n"
             msg += "登录流程: 在浏览器中打开下面链接（移动端复制链接至其他浏览器,\n" \
                    "登陆后，在显示红色的选择此人按钮时，右键红色按钮(手机端长按复制)\n" \
                    "复制其链接后发送给机器人，链接是一串npf开头的文本(两分钟内有效！)"
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/my.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/my.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,21 +92,21 @@
 现有点数 | {card['regularPoint']}
 打工次数 | {card['playCount']}
 金鲑鱼卵 | {card['goldenDeliverCount']} {gdpc}
 鲑鱼卵 | {card['deliverCount']} {dpc}
 头目鲑鱼 | {card['defeatBossCount']} {boss_per_cnt}
 救援次数 | {card['rescueCount']} {rpc}
 累计点数 | {card['totalPoint']} {ppc}
-鳞片 | 🥉{p['bronze']} 🥈{p['silver']} 🏅️{p['gold']}"""
+鳞片 | 🏅️{p['gold']} 🥈{p['silver']} 🥉{p['bronze']}"""
 
         if from_group:
             coop_msg = f"""当前打工段位 | {level}
 打工次数 | {card['playCount']}
 头目鲑鱼 | {card['defeatBossCount']} {boss_per_cnt}
-鳞片 | 🥉{p['bronze']} 🥈{p['silver']} 🏅️{p['gold']}"""
+鳞片 | 🏅️{p['gold']} 🥈{p['silver']} 🥉{p['bronze']}"""
 
     ar = (history.get('xMatchMaxAr') or {}).get('power') or 0  # 区域
     lf = (history.get('xMatchMaxLf') or {}).get('power') or 0  # 塔楼
     gl = (history.get('xMatchMaxGl') or {}).get('power') or 0  # 鱼虎
     cl = (history.get('xMatchMaxCl') or {}).get('power') or 0  # 蛤蜊
     x_msg = '||'
     if any([ar, lf, gl, cl]) and not from_group:
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/push.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/push.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/qq_md.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/qq_md.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/report.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/report.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/screenshot.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/screenshot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/send_msg.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/send_msg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/top.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/top.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/utils.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/handle/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/en-GB.json` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/i18n/en-GB.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/ja-JP.json` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/i18n/ja-JP.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/ko-KR.json` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/i18n/ko-KR.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/zh-CN.json` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/zh-TW.json` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/i18n/zh-TW.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/md.css` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/md.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/sp3bot-login.gif` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/resource/sp3bot-login.gif`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/iksm.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/s3s/iksm.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/splatnet_image.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/s3s/splatnet_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/splatoon.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/s3s/splatoon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/utils.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/s3s/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/util.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/bot.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/utils/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/http.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/utils/http.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/time.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/utils/time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/utils.py` & `nonebot_plugin_splatoon3_nso-1.4.3/nonebot_plugin_splatoon3_nso/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-BOT_VERSION = "2.6.2"
+BOT_VERSION = "2.6.3"
 DIR_RESOURCE = f"{os.path.abspath(os.path.join(__file__, os.pardir, os.pardir))}/resource"
 plugin_release_time = "2024-01-30 02:35:58"  # 预留  2.0.0重构版nso插件发布时间，预计发布时对全部用户先显示一周，之后再判断用户创建时间
 
 
 def multiple_replace(text, _dict):
     """批量替换文本"""
     for key in _dict:
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/pyproject.toml` & `nonebot_plugin_splatoon3_nso-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-splatoon3-nso"
-version = "1.4.2"
+version = "1.4.3"
 description = "一个基于nonebot2框架的splatoon3游戏nso数据查询插件"
 authors = ["cypas <ayano05@outlook.com>"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_splatoon3_nso"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.2/PKG-INFO` & `nonebot_plugin_splatoon3_nso-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-splatoon3-nso
-Version: 1.4.2
+Version: 1.4.3
 Summary: 一个基于nonebot2框架的splatoon3游戏nso数据查询插件
 Author: cypas
 Author-email: ayano05@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-splatoon3-nso Version: 1.4.2
+Metadata-Version: 2.1 Name: nonebot-plugin-splatoon3-nso Version: 1.4.3
 Summary: ä¸ä¸ªåºäºnonebot2æ¡æ¶çsplatoon3æ¸¸ænsoæ°æ®æ¥è¯¢æä»¶
 Author: cypas Author-email: ayano05@outlook.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: Pillow
 (==9.5.0) Requires-Dist: SQLAlchemy (>=2.0.25,<3.0.0) Requires-Dist:
 beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: httpx (>=0.24.1,<0.25.0)
```

