# Comparing `tmp/TikTokLive-6.0.3.tar.gz` & `tmp/TikTokLive-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/isaackogan/PycharmProjects/TikTokLive/dist/.tmp-widspjq4/TikTokLive-6.0.3.tar", last modified: Fri Mar 22 01:05:05 2024, max compression
+gzip compressed data, was "/Users/isaackogan/PycharmProjects/TikTokLive/dist/.tmp-imn6ynu3/TikTokLive-6.0.4.tar", last modified: Mon Apr  8 20:01:17 2024, max compression
```

## Comparing `TikTokLive-6.0.3.tar` & `TikTokLive-6.0.4.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.187503 TikTokLive-6.0.3/
--rw-r--r--   0 isaackogan   (501) staff       (20)     1068 2024-02-22 06:19:06.000000 TikTokLive-6.0.3/LICENSE
--rw-r--r--   0 isaackogan   (501) staff       (20)    17099 2024-03-22 01:05:05.187069 TikTokLive-6.0.3/PKG-INFO
--rw-r--r--   0 isaackogan   (501) staff       (20)    15967 2024-03-22 01:02:48.000000 TikTokLive-6.0.3/README.md
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.170130 TikTokLive-6.0.3/TikTokLive/
--rw-r--r--   0 isaackogan   (501) staff       (20)       43 2024-02-22 03:47:28.000000 TikTokLive-6.0.3/TikTokLive/__init__.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.173959 TikTokLive-6.0.3/TikTokLive/client/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-11 08:02:27.000000 TikTokLive-6.0.3/TikTokLive/client/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    15014 2024-03-22 00:19:18.000000 TikTokLive-6.0.3/TikTokLive/client/client.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      534 2024-02-24 20:23:34.000000 TikTokLive-6.0.3/TikTokLive/client/errors.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     4209 2024-02-24 20:23:34.000000 TikTokLive-6.0.3/TikTokLive/client/logger.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.175073 TikTokLive-6.0.3/TikTokLive/client/web/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-20 23:59:08.000000 TikTokLive-6.0.3/TikTokLive/client/web/__init__.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.177084 TikTokLive-6.0.3/TikTokLive/client/web/routes/
--rw-r--r--   0 isaackogan   (501) staff       (20)      294 2024-02-24 22:21:11.000000 TikTokLive-6.0.3/TikTokLive/client/web/routes/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      925 2024-02-24 20:23:34.000000 TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_gift_list.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      619 2024-02-24 20:23:34.000000 TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_image.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     3152 2024-02-24 22:45:50.000000 TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_is_live.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1868 2024-02-24 20:23:34.000000 TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_room_id.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1024 2024-02-24 20:23:34.000000 TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_room_info.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     5175 2024-02-28 18:42:42.000000 TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_sign.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     6065 2024-02-24 20:23:34.000000 TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_video.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     4728 2024-02-24 22:37:48.000000 TikTokLive-6.0.3/TikTokLive/client/web/web_base.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1356 2024-02-24 22:37:48.000000 TikTokLive-6.0.3/TikTokLive/client/web/web_client.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2607 2024-02-24 20:23:34.000000 TikTokLive-6.0.3/TikTokLive/client/web/web_settings.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.177424 TikTokLive-6.0.3/TikTokLive/client/ws/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2024-02-03 19:50:49.000000 TikTokLive-6.0.3/TikTokLive/client/ws/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     7748 2024-03-22 01:02:42.000000 TikTokLive-6.0.3/TikTokLive/client/ws/ws_client.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.178620 TikTokLive-6.0.3/TikTokLive/events/
--rw-r--r--   0 isaackogan   (501) staff       (20)      567 2024-02-22 06:22:04.000000 TikTokLive-6.0.3/TikTokLive/events/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      439 2024-02-24 20:23:34.000000 TikTokLive-6.0.3/TikTokLive/events/base_event.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2316 2024-02-24 20:23:34.000000 TikTokLive-6.0.3/TikTokLive/events/custom_events.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     7061 2024-02-28 19:23:41.000000 TikTokLive-6.0.3/TikTokLive/events/proto_events.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.179488 TikTokLive-6.0.3/TikTokLive/proto/
--rw-r--r--   0 isaackogan   (501) staff       (20)       55 2024-02-04 07:15:00.000000 TikTokLive-6.0.3/TikTokLive/proto/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1819 2024-02-28 18:54:40.000000 TikTokLive-6.0.3/TikTokLive/proto/custom_proto.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    98737 2024-02-04 08:14:43.000000 TikTokLive-6.0.3/TikTokLive/proto/tiktok_proto.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.186479 TikTokLive-6.0.3/TikTokLive.egg-info/
--rw-r--r--   0 isaackogan   (501) staff       (20)    17099 2024-03-22 01:05:05.000000 TikTokLive-6.0.3/TikTokLive.egg-info/PKG-INFO
--rw-r--r--   0 isaackogan   (501) staff       (20)     1677 2024-03-22 01:05:05.000000 TikTokLive-6.0.3/TikTokLive.egg-info/SOURCES.txt
--rw-r--r--   0 isaackogan   (501) staff       (20)        1 2024-03-22 01:05:05.000000 TikTokLive-6.0.3/TikTokLive.egg-info/dependency_links.txt
--rw-r--r--   0 isaackogan   (501) staff       (20)      162 2024-03-22 01:05:05.000000 TikTokLive-6.0.3/TikTokLive.egg-info/requires.txt
--rw-r--r--   0 isaackogan   (501) staff       (20)       28 2024-03-22 01:05:05.000000 TikTokLive-6.0.3/TikTokLive.egg-info/top_level.txt
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.181037 TikTokLive-6.0.3/TikTokLiveLegacy/
--rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 TikTokLive-6.0.3/TikTokLiveLegacy/__init__.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.183182 TikTokLive-6.0.3/TikTokLiveLegacy/client/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-06-16 17:56:57.000000 TikTokLive-6.0.3/TikTokLiveLegacy/client/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    22144 2024-03-22 00:18:26.000000 TikTokLive-6.0.3/TikTokLiveLegacy/client/base.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     7425 2023-06-16 17:56:57.000000 TikTokLive-6.0.3/TikTokLiveLegacy/client/client.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2032 2024-02-17 18:22:43.000000 TikTokLive-6.0.3/TikTokLiveLegacy/client/config.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    10349 2024-02-22 06:31:30.000000 TikTokLive-6.0.3/TikTokLiveLegacy/client/httpx.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     4736 2024-02-22 06:29:21.000000 TikTokLive-6.0.3/TikTokLiveLegacy/client/wsclient.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.184359 TikTokLive-6.0.3/TikTokLiveLegacy/proto/
--rw-r--r--   0 isaackogan   (501) staff       (20)       50 2023-06-16 17:56:57.000000 TikTokLive-6.0.3/TikTokLiveLegacy/proto/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    46393 2023-06-16 17:56:57.000000 TikTokLive-6.0.3/TikTokLiveLegacy/proto/tiktok_schema_pb2.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     3003 2024-02-22 06:29:21.000000 TikTokLive-6.0.3/TikTokLiveLegacy/proto/utilities.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-03-22 01:05:05.186022 TikTokLive-6.0.3/TikTokLiveLegacy/types/
--rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 TikTokLive-6.0.3/TikTokLiveLegacy/types/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     3362 2023-06-16 17:56:57.000000 TikTokLive-6.0.3/TikTokLiveLegacy/types/errors.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    16175 2024-02-22 06:29:21.000000 TikTokLive-6.0.3/TikTokLiveLegacy/types/events.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    15122 2024-02-22 06:29:21.000000 TikTokLive-6.0.3/TikTokLiveLegacy/types/objects.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1023 2023-06-16 17:56:57.000000 TikTokLive-6.0.3/TikTokLiveLegacy/types/utilities.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1350 2024-02-24 20:23:34.000000 TikTokLive-6.0.3/TikTokLiveLegacy/utilities.py
--rw-r--r--   0 isaackogan   (501) staff       (20)       38 2024-03-22 01:05:05.187563 TikTokLive-6.0.3/setup.cfg
--rw-r--r--   0 isaackogan   (501) staff       (20)     1937 2024-03-22 01:03:51.000000 TikTokLive-6.0.3/setup.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.894157 TikTokLive-6.0.4/
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1068 2024-02-22 06:19:06.000000 TikTokLive-6.0.4/LICENSE
+-rw-r--r--   0 isaackogan   (501) staff       (20)    17700 2024-04-08 20:01:17.893797 TikTokLive-6.0.4/PKG-INFO
+-rw-r--r--   0 isaackogan   (501) staff       (20)    16568 2024-04-01 02:18:03.000000 TikTokLive-6.0.4/README.md
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.878011 TikTokLive-6.0.4/TikTokLive/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       43 2024-02-22 03:47:28.000000 TikTokLive-6.0.4/TikTokLive/__init__.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.880232 TikTokLive-6.0.4/TikTokLive/client/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-11 08:02:27.000000 TikTokLive-6.0.4/TikTokLive/client/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    16353 2024-04-08 19:55:17.000000 TikTokLive-6.0.4/TikTokLive/client/client.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      658 2024-04-01 02:16:57.000000 TikTokLive-6.0.4/TikTokLive/client/errors.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     4209 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/client/logger.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.881298 TikTokLive-6.0.4/TikTokLive/client/web/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-20 23:59:08.000000 TikTokLive-6.0.4/TikTokLive/client/web/__init__.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.884333 TikTokLive-6.0.4/TikTokLive/client/web/routes/
+-rw-r--r--   0 isaackogan   (501) staff       (20)      303 2024-04-08 19:26:24.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      925 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_gift_list.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      619 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_image.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2355 2024-04-08 19:57:30.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_is_live.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2803 2024-04-08 19:57:30.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_room_id_api.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1889 2024-04-08 19:26:01.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_room_id_html.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1424 2024-04-08 19:50:54.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_room_info.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     5209 2024-04-03 17:28:04.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_sign.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     6065 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_video.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     4918 2024-04-08 19:22:45.000000 TikTokLive-6.0.4/TikTokLive/client/web/web_base.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1532 2024-04-08 19:57:30.000000 TikTokLive-6.0.4/TikTokLive/client/web/web_client.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2607 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/client/web/web_settings.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.884686 TikTokLive-6.0.4/TikTokLive/client/ws/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2024-02-03 19:50:49.000000 TikTokLive-6.0.4/TikTokLive/client/ws/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     7748 2024-03-22 01:02:42.000000 TikTokLive-6.0.4/TikTokLive/client/ws/ws_client.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.886070 TikTokLive-6.0.4/TikTokLive/events/
+-rw-r--r--   0 isaackogan   (501) staff       (20)      567 2024-02-22 06:22:04.000000 TikTokLive-6.0.4/TikTokLive/events/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      439 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/events/base_event.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2316 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/events/custom_events.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     7061 2024-02-28 19:23:41.000000 TikTokLive-6.0.4/TikTokLive/events/proto_events.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.887176 TikTokLive-6.0.4/TikTokLive/proto/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       55 2024-02-04 07:15:00.000000 TikTokLive-6.0.4/TikTokLive/proto/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1819 2024-02-28 18:54:40.000000 TikTokLive-6.0.4/TikTokLive/proto/custom_proto.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    98737 2024-02-04 08:14:43.000000 TikTokLive-6.0.4/TikTokLive/proto/tiktok_proto.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.893387 TikTokLive-6.0.4/TikTokLive.egg-info/
+-rw-r--r--   0 isaackogan   (501) staff       (20)    17700 2024-04-08 20:01:17.000000 TikTokLive-6.0.4/TikTokLive.egg-info/PKG-INFO
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1732 2024-04-08 20:01:17.000000 TikTokLive-6.0.4/TikTokLive.egg-info/SOURCES.txt
+-rw-r--r--   0 isaackogan   (501) staff       (20)        1 2024-04-08 20:01:17.000000 TikTokLive-6.0.4/TikTokLive.egg-info/dependency_links.txt
+-rw-r--r--   0 isaackogan   (501) staff       (20)      162 2024-04-08 20:01:17.000000 TikTokLive-6.0.4/TikTokLive.egg-info/requires.txt
+-rw-r--r--   0 isaackogan   (501) staff       (20)       28 2024-04-08 20:01:17.000000 TikTokLive-6.0.4/TikTokLive.egg-info/top_level.txt
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.888722 TikTokLive-6.0.4/TikTokLiveLegacy/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/__init__.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.890691 TikTokLive-6.0.4/TikTokLiveLegacy/client/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    22144 2024-03-22 00:18:26.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/base.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     7425 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/client.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2032 2024-02-17 18:22:43.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/config.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    10349 2024-02-22 06:31:30.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/httpx.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     4736 2024-02-22 06:29:21.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/wsclient.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.891751 TikTokLive-6.0.4/TikTokLiveLegacy/proto/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       50 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/proto/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    46393 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/proto/tiktok_schema_pb2.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     3003 2024-02-22 06:29:21.000000 TikTokLive-6.0.4/TikTokLiveLegacy/proto/utilities.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.892996 TikTokLive-6.0.4/TikTokLiveLegacy/types/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/types/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     3362 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/types/errors.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    16175 2024-02-22 06:29:21.000000 TikTokLive-6.0.4/TikTokLiveLegacy/types/events.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    15122 2024-02-22 06:29:21.000000 TikTokLive-6.0.4/TikTokLiveLegacy/types/objects.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1023 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/types/utilities.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1350 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLiveLegacy/utilities.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)       38 2024-04-08 20:01:17.894212 TikTokLive-6.0.4/setup.cfg
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1937 2024-04-08 20:00:14.000000 TikTokLive-6.0.4/setup.py
```

### Comparing `TikTokLive-6.0.3/LICENSE` & `TikTokLive-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/PKG-INFO` & `TikTokLive-6.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 5469 6b54  : 2.1.Name: TikT
 00000020: 6f6b 4c69 7665 0a56 6572 7369 6f6e 3a20  okLive.Version: 
-00000030: 362e 302e 330a 5375 6d6d 6172 793a 2054  6.0.3.Summary: T
+00000030: 362e 302e 340a 5375 6d6d 6172 793a 2054  6.0.4.Summary: T
 00000040: 696b 546f 6b20 4c69 7665 2050 7974 686f  ikTok Live Pytho
 00000050: 6e20 436c 6965 6e74 0a48 6f6d 652d 7061  n Client.Home-pa
 00000060: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000070: 7562 2e63 6f6d 2f69 7361 6163 6b6f 6761  ub.com/isaackoga
 00000080: 6e2f 5469 6b54 6f6b 4c69 7665 0a44 6f77  n/TikTokLive.Dow
 00000090: 6e6c 6f61 642d 5552 4c3a 2068 7474 7073  nload-URL: https
 000000a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6973  ://github.com/is
 000000b0: 6161 636b 6f67 616e 2f54 696b 546f 6b4c  aackogan/TikTokL
 000000c0: 6976 652f 7265 6c65 6173 6573 2f74 6167  ive/releases/tag
-000000d0: 2f76 362e 302e 330a 4175 7468 6f72 3a20  /v6.0.3.Author: 
+000000d0: 2f76 362e 302e 340a 4175 7468 6f72 3a20  /v6.0.4.Author: 
 000000e0: 4973 6161 6320 4b6f 6761 6e0a 4175 7468  Isaac Kogan.Auth
 000000f0: 6f72 2d65 6d61 696c 3a20 696e 666f 4069  or-email: info@i
 00000100: 7361 6163 6b6f 6761 6e2e 636f 6d0a 4c69  saackogan.com.Li
 00000110: 6365 6e73 653a 204d 4954 0a4b 6579 776f  cense: MIT.Keywo
 00000120: 7264 733a 2074 696b 746f 6b2c 7469 6b74  rds: tiktok,tikt
 00000130: 6f6b 206c 6976 652c 7079 7468 6f6e 332c  ok live,python3,
 00000140: 6170 692c 756e 6f66 6669 6369 616c 0a43  api,unofficial.C
@@ -134,936 +134,974 @@
 00000850: 2f65 3258 7750 4e54 4242 7229 2061 6e64  /e2XwPNTBBr) and
 00000860: 2076 6973 6974 0a74 6865 205b 6023 7079   visit.the [`#py
 00000870: 2d73 7570 706f 7274 605d 2868 7474 7073  -support`](https
 00000880: 3a2f 2f64 6973 636f 7264 2e67 672f 756a  ://discord.gg/uj
 00000890: 6136 5361 6a44 7864 290a 6368 616e 6e65  a6SajDxd).channe
 000008a0: 6c20 666f 7220 7175 6573 7469 6f6e 732c  l for questions,
 000008b0: 2063 6f6e 7472 6962 7574 696f 6e73 2061   contributions a
-000008c0: 6e64 2069 6465 6173 2e0a 0a23 2323 2043  nd ideas...### C
-000008d0: 6f6e 7369 6465 7220 446f 6e61 7469 6e67  onsider Donating
-000008e0: 203c 330a 0a49 276d 2061 2032 6e64 2d79   <3..I'm a 2nd-y
-000008f0: 6561 7220 4269 6f6c 6f67 7920 7374 7564  ear Biology stud
-00000900: 656e 7420 696e 2075 6e69 7665 7273 6974  ent in universit
-00000910: 7920 7768 6f20 6c69 6b65 7320 746f 2070  y who likes to p
-00000920: 726f 6772 616d 2066 6f72 2066 756e 2e20  rogram for fun. 
-00000930: 506c 6561 7365 2063 6f6e 7369 6465 7220  Please consider 
-00000940: 7375 7070 6f72 7469 6e67 2064 6576 656c  supporting devel
-00000950: 6f70 6d65 6e74 0a74 6872 6f75 6768 2061  opment.through a
-00000960: 2073 6d61 6c6c 2064 6f6e 6174 696f 6e20   small donation 
-00000970: 6174 205b 6874 7470 733a 2f2f 7777 772e  at [https://www.
-00000980: 6275 796d 6561 636f 6666 6565 2e63 6f6d  buymeacoffee.com
-00000990: 2f69 7361 6163 6b6f 6761 6e5d 2868 7474  /isaackogan](htt
-000009a0: 7073 3a2f 2f77 7777 2e62 7579 6d65 6163  ps://www.buymeac
-000009b0: 6f66 6665 652e 636f 6d2f 6973 6161 636b  offee.com/isaack
-000009c0: 6f67 616e 292e 2041 6e79 7468 696e 670a  ogan). Anything.
-000009d0: 796f 7520 6361 6e20 6f66 6665 7220 7769  you can offer wi
-000009e0: 6c6c 2067 6f20 746f 7761 7264 7320 7363  ll go towards sc
-000009f0: 686f 6f6c 2026 2064 6576 656c 6f70 6d65  hool & developme
-00000a00: 6e74 2063 6f73 7473 2066 6f72 2054 696b  nt costs for Tik
-00000a10: 546f 6b4c 6976 652c 2077 6869 6368 2068  TokLive, which h
-00000a20: 6173 2074 616b 656e 2068 756e 6472 6564  as taken hundred
-00000a30: 7320 6f66 2068 6f75 7273 206f 6620 7469  s of hours of ti
-00000a40: 6d65 2074 6f20 6275 696c 642e 0a0a 2323  me to build...##
-00000a50: 2320 4f74 6865 7220 4c61 6e67 7561 6765  # Other Language
-00000a60: 730a 0a54 696b 546f 6b4c 6976 6520 6973  s..TikTokLive is
-00000a70: 2061 7661 696c 6162 6c65 2069 6e20 7365   available in se
-00000a80: 7665 7261 6c20 616c 7465 726e 6174 6520  veral alternate 
-00000a90: 7072 6f67 7261 6d6d 696e 6720 6c61 6e67  programming lang
-00000aa0: 7561 6765 733a 0a0a 2d20 2a2a 4e6f 6465  uages:..- **Node
-00000ab0: 2e4a 533a 2a2a 205b 6874 7470 733a 2f2f  .JS:** [https://
-00000ac0: 6769 7468 7562 2e63 6f6d 2f7a 6572 6f64  github.com/zerod
-00000ad0: 7974 7261 7368 2f54 696b 546f 6b2d 4c69  ytrash/TikTok-Li
-00000ae0: 7665 2d43 6f6e 6e65 6374 6f72 5d28 6874  ve-Connector](ht
-00000af0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000b00: 2f7a 6572 6f64 7974 7261 7368 2f54 696b  /zerodytrash/Tik
-00000b10: 546f 6b2d 4c69 7665 2d43 6f6e 6e65 6374  Tok-Live-Connect
-00000b20: 6f72 290a 2d20 2a2a 4a61 7661 3a2a 2a20  or).- **Java:** 
-00000b30: 5b68 7474 7073 3a2f 2f67 6974 6875 622e  [https://github.
-00000b40: 636f 6d2f 6a77 6465 7665 6c6f 7065 722f  com/jwdeveloper/
-00000b50: 5469 6b54 6f6b 2d4c 6976 652d 4a61 7661  TikTok-Live-Java
-00000b60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000b70: 2e63 6f6d 2f6a 7764 6576 656c 6f70 6572  .com/jwdeveloper
-00000b80: 2f54 696b 546f 6b2d 4c69 7665 2d4a 6176  /TikTok-Live-Jav
-00000b90: 6129 0a2d 202a 2a43 232f 556e 6974 793a  a).- **C#/Unity:
-00000ba0: 2a2a 205b 6874 7470 733a 2f2f 6769 7468  ** [https://gith
-00000bb0: 7562 2e63 6f6d 2f66 7261 6e6b 7648 6f6f  ub.com/frankvHoo
-00000bc0: 6639 332f 5469 6b54 6f6b 4c69 7665 5368  f93/TikTokLiveSh
-00000bd0: 6172 705d 2868 7474 7073 3a2f 2f67 6974  arp](https://git
-00000be0: 6875 622e 636f 6d2f 6672 616e 6b76 486f  hub.com/frankvHo
-00000bf0: 6f66 3933 2f54 696b 546f 6b4c 6976 6553  of93/TikTokLiveS
-00000c00: 6861 7270 290a 2d20 2a2a 476f 3a2a 2a20  harp).- **Go:** 
-00000c10: 5b68 7474 7073 3a2f 2f67 6974 6875 622e  [https://github.
-00000c20: 636f 6d2f 4461 7669 6e63 6962 6c65 2f67  com/Davincible/g
-00000c30: 6f74 696b 746f 6b6c 6976 655d 2868 7474  otiktoklive](htt
-00000c40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000c50: 4461 7669 6e63 6962 6c65 2f67 6f74 696b  Davincible/gotik
-00000c60: 746f 6b6c 6976 6529 0a2d 202a 2a52 7573  toklive).- **Rus
-00000c70: 743a 2a2a 205b 6874 7470 733a 2f2f 6769  t:** [https://gi
-00000c80: 7468 7562 2e63 6f6d 2f6a 7764 6576 656c  thub.com/jwdevel
-00000c90: 6f70 6572 2f54 696b 546f 6b4c 6976 6552  oper/TikTokLiveR
-00000ca0: 7573 745d 2868 7474 7073 3a2f 2f67 6974  ust](https://git
-00000cb0: 6875 622e 636f 6d2f 6a77 6465 7665 6c6f  hub.com/jwdevelo
-00000cc0: 7065 722f 5469 6b54 6f6b 4c69 7665 5275  per/TikTokLiveRu
-00000cd0: 7374 290a 0a23 2320 5461 626c 6520 6f66  st)..## Table of
-00000ce0: 2043 6f6e 7465 6e74 730a 0a2d 205b 446f   Contents..- [Do
-00000cf0: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-00000d00: 7073 3a2f 2f69 7361 6163 6b6f 6761 6e2e  ps://isaackogan.
-00000d10: 6769 7468 7562 2e69 6f2f 5469 6b54 6f6b  github.io/TikTok
-00000d20: 4c69 7665 2f29 0a2d 205b 4578 616d 706c  Live/).- [Exampl
-00000d30: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-00000d40: 7562 2e63 6f6d 2f69 7361 6163 6b6f 6761  ub.com/isaackoga
-00000d50: 6e2f 5469 6b54 6f6b 4c69 7665 2f74 7265  n/TikTokLive/tre
-00000d60: 652f 6d61 7374 6572 2f65 7861 6d70 6c65  e/master/example
-00000d70: 7329 0a2d 205b 5769 6b69 5d28 6874 7470  s).- [Wiki](http
-00000d80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
-00000d90: 7361 6163 6b6f 6761 6e2f 5469 6b54 6f6b  saackogan/TikTok
-00000da0: 4c69 7665 2f77 696b 6929 200a 2d20 5b4c  Live/wiki) .- [L
-00000db0: 6963 656e 7369 6e67 5d28 236c 6963 656e  icensing](#licen
-00000dc0: 7365 290a 2d20 5b43 6f6e 7472 6962 7574  se).- [Contribut
-00000dd0: 6f72 735d 2823 636f 6e74 7269 6275 746f  ors](#contributo
-00000de0: 7273 290a 0a23 2320 4765 7474 696e 6720  rs)..## Getting 
-00000df0: 5374 6172 7465 640a 0a31 2e20 496e 7374  Started..1. Inst
-00000e00: 616c 6c20 7468 6520 6d6f 6475 6c65 2076  all the module v
-00000e10: 6961 2070 6970 2066 726f 6d20 7468 6520  ia pip from the 
-00000e20: 5b50 7950 695d 2868 7474 7073 3a2f 2f70  [PyPi](https://p
-00000e30: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000e40: 5469 6b54 6f6b 4c69 7665 2f29 2072 6570  TikTokLive/) rep
-00000e50: 6f73 6974 6f72 790a 0a60 6060 7368 656c  ository..```shel
-00000e60: 6c20 7363 7269 7074 0a70 6970 2069 6e73  l script.pip ins
-00000e70: 7461 6c6c 2054 696b 546f 6b4c 6976 650a  tall TikTokLive.
-00000e80: 6060 600a 0a32 2e20 4372 6561 7465 2079  ```..2. Create y
-00000e90: 6f75 7220 6669 7273 7420 6368 6174 2063  our first chat c
-00000ea0: 6f6e 6e65 6374 696f 6e0a 0a60 6060 7079  onnection..```py
-00000eb0: 7468 6f6e 0a66 726f 6d20 5469 6b54 6f6b  thon.from TikTok
-00000ec0: 4c69 7665 2069 6d70 6f72 7420 5469 6b54  Live import TikT
-00000ed0: 6f6b 4c69 7665 436c 6965 6e74 0a66 726f  okLiveClient.fro
-00000ee0: 6d20 5469 6b54 6f6b 4c69 7665 2e65 7665  m TikTokLive.eve
-00000ef0: 6e74 7320 696d 706f 7274 2043 6f6e 6e65  nts import Conne
-00000f00: 6374 4576 656e 742c 2043 6f6d 6d65 6e74  ctEvent, Comment
-00000f10: 4576 656e 740a 0a23 2043 7265 6174 6520  Event..# Create 
-00000f20: 7468 6520 636c 6965 6e74 0a63 6c69 656e  the client.clien
-00000f30: 743a 2054 696b 546f 6b4c 6976 6543 6c69  t: TikTokLiveCli
-00000f40: 656e 7420 3d20 5469 6b54 6f6b 4c69 7665  ent = TikTokLive
-00000f50: 436c 6965 6e74 2875 6e69 7175 655f 6964  Client(unique_id
-00000f60: 3d22 4069 7361 6163 6b6f 677a 2229 0a0a  ="@isaackogz")..
-00000f70: 0a23 204c 6973 7465 6e20 746f 2061 6e20  .# Listen to an 
-00000f80: 6576 656e 7420 7769 7468 2061 2064 6563  event with a dec
-00000f90: 6f72 6174 6f72 210a 4063 6c69 656e 742e  orator!.@client.
-00000fa0: 6f6e 2843 6f6e 6e65 6374 4576 656e 7429  on(ConnectEvent)
-00000fb0: 0a61 7379 6e63 2064 6566 206f 6e5f 636f  .async def on_co
-00000fc0: 6e6e 6563 7428 6576 656e 743a 2043 6f6e  nnect(event: Con
-00000fd0: 6e65 6374 4576 656e 7429 3a0a 2020 2020  nectEvent):.    
-00000fe0: 7072 696e 7428 6622 436f 6e6e 6563 7465  print(f"Connecte
-00000ff0: 6420 746f 2040 7b65 7665 6e74 2e75 6e69  d to @{event.uni
-00001000: 7175 655f 6964 7d20 2852 6f6f 6d20 4944  que_id} (Room ID
-00001010: 3a20 7b63 6c69 656e 742e 726f 6f6d 5f69  : {client.room_i
-00001020: 647d 2229 0a0a 0a23 204f 722c 2061 6464  d}")...# Or, add
-00001030: 2069 7420 6d61 6e75 616c 6c79 2076 6961   it manually via
-00001040: 2022 636c 6965 6e74 2e61 6464 5f6c 6973   "client.add_lis
-00001050: 7465 6e65 7228 2922 0a61 7379 6e63 2064  tener()".async d
-00001060: 6566 206f 6e5f 636f 6d6d 656e 7428 6576  ef on_comment(ev
-00001070: 656e 743a 2043 6f6d 6d65 6e74 4576 656e  ent: CommentEven
-00001080: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-00001090: 7072 696e 7428 6622 7b65 7665 6e74 2e75  print(f"{event.u
-000010a0: 7365 722e 6e69 636b 6e61 6d65 7d20 2d3e  ser.nickname} ->
-000010b0: 207b 6576 656e 742e 636f 6d6d 656e 747d   {event.comment}
-000010c0: 2229 0a0a 0a63 6c69 656e 742e 6164 645f  ")...client.add_
-000010d0: 6c69 7374 656e 6572 2843 6f6d 6d65 6e74  listener(Comment
-000010e0: 4576 656e 742c 206f 6e5f 636f 6d6d 656e  Event, on_commen
-000010f0: 7429 0a0a 6966 205f 5f6e 616d 655f 5f20  t)..if __name__ 
-00001100: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0a20  == '__main__':. 
-00001110: 2020 2023 2052 756e 2074 6865 2063 6c69     # Run the cli
-00001120: 656e 7420 616e 6420 626c 6f63 6b20 7468  ent and block th
-00001130: 6520 6d61 696e 2074 6872 6561 640a 2020  e main thread.  
-00001140: 2020 2320 6177 6169 7420 636c 6965 6e74    # await client
-00001150: 2e73 7461 7274 2829 2074 6f20 7275 6e20  .start() to run 
-00001160: 6e6f 6e2d 626c 6f63 6b69 6e67 0a20 2020  non-blocking.   
-00001170: 2063 6c69 656e 742e 7275 6e28 290a 6060   client.run().``
-00001180: 600a 0a46 6f72 206d 6f72 6520 7175 6963  `..For more quic
-00001190: 6b73 7461 7274 2065 7861 6d70 6c65 732c  kstart examples,
-000011a0: 2073 6565 2074 6865 205b 6578 616d 706c   see the [exampl
-000011b0: 6573 2066 6f6c 6465 725d 2868 7474 7073  es folder](https
-000011c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6973  ://github.com/is
-000011d0: 6161 636b 6f67 616e 2f54 696b 546f 6b4c  aackogan/TikTokL
-000011e0: 6976 652f 7472 6565 2f6d 6173 7465 722f  ive/tree/master/
-000011f0: 6578 616d 706c 6573 290a 7072 6f76 6964  examples).provid
-00001200: 6564 2069 6e20 7468 6520 736f 7572 6365  ed in the source
-00001210: 2074 7265 652e 0a0a 2323 2050 6172 616d   tree...## Param
-00001220: 6574 6572 730a 0a7c 2050 6172 616d 204e  eters..| Param N
-00001230: 616d 6520 7c20 5265 7175 6972 6564 207c  ame | Required |
-00001240: 2044 6566 6175 6c74 207c 2044 6573 6372   Default | Descr
-00001250: 6970 7469 6f6e 2020 2020 2020 2020 2020  iption          
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001320: 2020 2020 207c 0a7c 2d2d 2d2d 2d2d 2d2d       |.|--------
-00001330: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d7c  ----|----------|
-00001340: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
-00001350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001420: 2d2d 2d2d 2d7c 0a7c 2075 6e69 7175 655f  -----|.| unique_
-00001430: 6964 2020 7c20 5965 7320 2020 2020 207c  id  | Yes      |
-00001440: 204e 2f41 2020 2020 207c 2054 6865 2075   N/A     | The u
-00001450: 6e69 7175 6520 7573 6572 6e61 6d65 206f  nique username o
-00001460: 6620 7468 6520 6272 6f61 6463 6173 7465  f the broadcaste
-00001470: 722e 2059 6f75 2063 616e 2066 696e 6420  r. You can find 
-00001480: 7468 6973 206e 616d 6520 696e 2074 6865  this name in the
-00001490: 2055 524c 206f 6620 7468 6520 7573 6572   URL of the user
-000014a0: 2e20 466f 7220 6578 616d 706c 652c 2074  . For example, t
-000014b0: 6865 2060 756e 6971 7565 5f69 6460 2066  he `unique_id` f
-000014c0: 6f72 205b 6068 7474 7073 3a2f 2f77 7777  or [`https://www
-000014d0: 2e74 696b 746f 6b2e 636f 6d2f 4069 7361  .tiktok.com/@isa
-000014e0: 6163 6b6f 677a 605d 2868 7474 7073 3a2f  ackogz`](https:/
-000014f0: 2f77 7777 2e74 696b 746f 6b2e 636f 6d2f  /www.tiktok.com/
-00001500: 4069 7361 6163 6b6f 677a 2920 776f 756c  @isaackogz) woul
-00001510: 6420 6265 2060 6973 6161 636b 6f67 7a60  d be `isaackogz`
-00001520: 2e20 2020 207c 0a7c 2077 6562 5f70 726f  .    |.| web_pro
-00001530: 7879 2020 7c20 4e6f 2020 2020 2020 207c  xy  | No       |
-00001540: 2060 4e6f 6e65 6020 207c 2054 696b 546f   `None`  | TikTo
-00001550: 6b4c 6976 6520 7375 7070 6f72 7473 2070  kLive supports p
-00001560: 726f 7879 696e 6720 4854 5450 2072 6571  roxying HTTP req
-00001570: 7565 7374 732e 2054 6869 7320 7061 7261  uests. This para
-00001580: 6d65 7465 7220 6163 6365 7074 7320 616e  meter accepts an
-00001590: 2060 6874 7470 782e 5072 6f78 7960 2e20   `httpx.Proxy`. 
-000015a0: 4e6f 7465 2074 6861 7420 6966 2079 6f75  Note that if you
-000015b0: 2064 6f20 7573 6520 6120 7072 6f78 7920   do use a proxy 
-000015c0: 796f 7520 6d61 7920 6265 2073 7562 6a65  you may be subje
-000015d0: 6374 2074 6f20 7265 6475 6365 6420 636f  ct to reduced co
-000015e0: 6e6e 6563 7469 6f6e 206c 696d 6974 7320  nnection limits 
-000015f0: 6174 2074 696d 6573 206f 6620 6869 6768  at times of high
-00001600: 206c 6f61 642e 2020 2020 2020 2020 2020   load.          
-00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001620: 2020 2020 207c 0a7c 2077 735f 7072 6f78       |.| ws_prox
-00001630: 7920 2020 7c20 4e6f 2020 2020 2020 207c  y   | No       |
-00001640: 2060 4e6f 6e65 6020 207c 2054 696b 546f   `None`  | TikTo
-00001650: 6b4c 6976 6520 7375 7070 6f72 7473 2070  kLive supports p
-00001660: 726f 7879 696e 6720 7468 6520 7765 6273  roxying the webs
-00001670: 6f63 6b65 7420 636f 6e6e 6563 7469 6f6e  ocket connection
-00001680: 2e20 5468 6973 2070 6172 616d 6574 6572  . This parameter
-00001690: 2061 6363 6570 7473 2061 6e20 6068 7474   accepts an `htt
-000016a0: 7078 2e50 726f 7879 602e 2055 7369 6e67  px.Proxy`. Using
-000016b0: 2074 6869 7320 7072 6f78 7920 7769 6c6c   this proxy will
-000016c0: 206e 6576 6572 2062 6520 7375 626a 6563   never be subjec
-000016d0: 7420 746f 2072 6564 7563 6564 2063 6f6e  t to reduced con
-000016e0: 6e65 6374 696f 6e20 6c69 6d69 7473 2e20  nection limits. 
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001720: 2020 2020 207c 0a7c 2077 6562 5f6b 7761       |.| web_kwa
-00001730: 7267 7320 7c20 4e6f 2020 2020 2020 207c  rgs | No       |
-00001740: 2060 7b7d 6020 2020 207c 2055 6e64 6572   `{}`    | Under
-00001750: 2074 6865 2073 6365 6e65 732c 2074 6865   the scenes, the
-00001760: 2054 696b 546f 6b4c 6976 6520 4854 5450   TikTokLive HTTP
-00001770: 2063 6c69 656e 7420 7573 6573 2074 6865   client uses the
-00001780: 205b 6068 7474 7078 605d 2868 7474 7073   [`httpx`](https
-00001790: 3a2f 2f67 6974 6875 622e 636f 6d2f 656e  ://github.com/en
-000017a0: 636f 6465 2f68 7474 7078 2920 6c69 6272  code/httpx) libr
-000017b0: 6172 792e 2041 7267 756d 656e 7473 2070  ary. Arguments p
-000017c0: 6173 7365 6420 746f 2060 7765 625f 6b77  assed to `web_kw
-000017d0: 6172 6773 6020 7769 6c6c 2062 6520 666f  args` will be fo
-000017e0: 7277 6172 6420 7468 6520 7468 6520 756e  rward the the un
-000017f0: 6465 726c 7969 6e67 2048 5454 5020 636c  derlying HTTP cl
-00001800: 6965 6e74 2e20 2020 2020 2020 2020 2020  ient.           
-00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001820: 2020 2020 207c 0a7c 2077 735f 6b77 6172       |.| ws_kwar
-00001830: 6773 2020 7c20 4e6f 2020 2020 2020 207c  gs  | No       |
-00001840: 2060 7b7d 6020 2020 207c 2055 6e64 6572   `{}`    | Under
-00001850: 2074 6865 2073 6365 6e65 732c 2054 696b   the scenes, Tik
-00001860: 546f 6b4c 6976 6520 7573 6573 2074 6865  TokLive uses the
-00001870: 205b 6077 6562 736f 636b 6574 7360 5d28   [`websockets`](
-00001880: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001890: 6f6d 2f70 7974 686f 6e2d 7765 6273 6f63  om/python-websoc
-000018a0: 6b65 7473 2f77 6562 736f 636b 6574 7329  kets/websockets)
-000018b0: 206c 6962 7261 7279 2074 6f20 636f 6e6e   library to conn
-000018c0: 6563 7420 746f 2054 696b 546f 6b2e 2041  ect to TikTok. A
-000018d0: 7267 756d 656e 7473 2070 6173 7365 6420  rguments passed 
-000018e0: 746f 2060 7773 5f6b 7761 7267 7360 2077  to `ws_kwargs` w
-000018f0: 696c 6c20 6265 2066 6f72 7761 7264 6564  ill be forwarded
-00001900: 2074 6f20 7468 6520 756e 6465 726c 7969   to the underlyi
-00001910: 6e67 2057 6562 536f 636b 6574 2063 6c69  ng WebSocket cli
-00001920: 656e 742e 207c 0a0a 2323 204d 6574 686f  ent. |..## Metho
-00001930: 6473 0a0a 4120 6054 696b 546f 6b4c 6976  ds..A `TikTokLiv
-00001940: 6543 6c69 656e 7460 206f 626a 6563 7420  eClient` object 
-00001950: 636f 6e74 6169 6e73 2074 6865 2066 6f6c  contains the fol
-00001960: 6c6f 7769 6e67 2069 6d70 6f72 7461 6e74  lowing important
-00001970: 206d 6574 686f 6473 3a0a 0a7c 204d 6574   methods:..| Met
-00001980: 686f 6420 4e61 6d65 2020 7c20 4e6f 7465  hod Name  | Note
-00001990: 7320 2020 7c20 4465 7363 7269 7074 696f  s   | Descriptio
-000019a0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a40: 207c 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.|------------
-00001a50: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  --|---------|---
-00001a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b00: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2072 756e  ---------|.| run
-00001b10: 2020 2020 2020 2020 2020 7c20 4e2f 4120            | N/A 
-00001b20: 2020 2020 7c20 436f 6e6e 6563 7420 746f      | Connect to
-00001b30: 2074 6865 206c 6976 6573 7472 6561 6d20   the livestream 
-00001b40: 616e 6420 626c 6f63 6b20 7468 6520 6d61  and block the ma
-00001b50: 696e 2074 6872 6561 642e 2054 6869 7320  in thread. This 
-00001b60: 6973 2062 6573 7420 666f 7220 736d 616c  is best for smal
-00001b70: 6c20 7363 7269 7074 732e 2020 2020 2020  l scripts.      
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bb0: 2020 2020 2020 2020 2020 207c 0a7c 2061             |.| a
-00001bc0: 6464 5f6c 6973 7465 6e65 7220 7c20 4e2f  dd_listener | N/
-00001bd0: 4120 2020 2020 7c20 4164 6473 2061 6e20  A     | Adds an 
-00001be0: 2a61 7379 6e63 6872 6f6e 6f75 732a 206c  *asynchronous* l
-00001bf0: 6973 7465 6e65 7220 6675 6e63 7469 6f6e  istener function
-00001c00: 2028 6f72 2c20 796f 7520 6361 6e20 6465   (or, you can de
-00001c10: 636f 7261 7465 2061 2066 756e 6374 696f  corate a functio
-00001c20: 6e20 7769 7468 2060 4063 6c69 656e 742e  n with `@client.
-00001c30: 6f6e 2822 3c65 7665 6e74 3e22 2960 2920  on("<event>")`) 
-00001c40: 616e 6420 7461 6b65 7320 7477 6f20 7061  and takes two pa
-00001c50: 7261 6d65 7465 7273 2c20 616e 2065 7665  rameters, an eve
-00001c60: 6e74 206e 616d 6520 616e 6420 7468 6520  nt name and the 
-00001c70: 7061 796c 6f61 642c 2061 6e20 4162 7374  payload, an Abst
-00001c80: 7261 6374 4576 656e 7420 7c7c 0a7c 2063  ractEvent ||.| c
-00001c90: 6f6e 6e65 6374 2020 2020 2020 7c20 6061  onnect      | `a
-00001ca0: 7379 6e63 6020 7c20 436f 6e6e 6563 7473  sync` | Connects
-00001cb0: 2074 6f20 7468 6520 7469 6b74 6f6b 206c   to the tiktok l
-00001cc0: 6976 6520 6368 6174 2077 6869 6c65 2062  ive chat while b
-00001cd0: 6c6f 636b 696e 6720 7468 6520 6375 7272  locking the curr
-00001ce0: 656e 7420 6675 7475 7265 2e20 5768 656e  ent future. When
-00001cf0: 2074 6865 2063 6f6e 6e65 6374 696f 6e20   the connection 
-00001d00: 656e 6473 2028 652e 672e 206c 6976 6573  ends (e.g. lives
-00001d10: 7472 6561 6d20 6973 206f 7665 7229 2c20  tream is over), 
-00001d20: 7468 6520 6675 7475 7265 2069 7320 7265  the future is re
-00001d30: 6c65 6173 6564 2e20 2020 2020 2020 2020  leased.         
-00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d50: 2020 207c 0a7c 2073 7461 7274 2020 2020     |.| start    
-00001d60: 2020 2020 7c20 6061 7379 6e63 6020 7c20      | `async` | 
-00001d70: 436f 6e6e 6563 7473 2074 6f20 7468 6520  Connects to the 
-00001d80: 6c69 7665 2063 6861 7420 7769 7468 6f75  live chat withou
-00001d90: 7420 626c 6f63 6b69 6e67 2074 6865 206d  t blocking the m
-00001da0: 6169 6e20 7468 7265 6164 2e20 5468 6973  ain thread. This
-00001db0: 2072 6574 7572 6e73 2061 6e20 6061 7379   returns an `asy
-00001dc0: 6e63 696f 2e54 6173 6b60 206f 626a 6563  ncio.Task` objec
-00001dd0: 7420 7769 7468 2074 6865 2063 6c69 656e  t with the clien
-00001de0: 7420 6c6f 6f70 2e20 2020 2020 2020 2020  t loop.         
+000008c0: 6e64 2069 6465 6173 2e0a 0a23 2323 2045  nd ideas...### E
+000008d0: 6e74 6572 7072 6973 6520 4163 6365 7373  nterprise Access
+000008e0: 0a0a 2d20 546f 6b65 6e73 2074 6f20 7363  ..- Tokens to sc
+000008f0: 7261 7065 2041 4e59 2054 696b 546f 6b20  rape ANY TikTok 
+00000900: 5552 4c20 2869 2e65 2e20 6665 7463 6820  URL (i.e. fetch 
+00000910: 7072 6f66 696c 6573 2c20 2076 6964 656f  profiles,  video
+00000920: 732c 2063 6f6d 6d65 6e74 732c 2065 7463  s, comments, etc
+00000930: 2e29 0a2d 2049 6e63 7265 6173 6564 2054  .).- Increased T
+00000940: 696b 546f 6b20 4c49 5645 2072 6174 6520  ikTok LIVE rate 
+00000950: 6c69 6d69 7473 2028 692e 652e 2061 6269  limits (i.e. abi
+00000960: 6c69 7479 2074 6f20 3130 3030 7320 6f66  lity to 1000s of
+00000970: 2063 6c69 656e 7473 2070 6572 2068 6f75   clients per hou
+00000980: 7229 0a0a 3c64 6976 2061 6c69 676e 3d22  r)..<div align="
+00000990: 6c65 6674 223e 0a20 2020 203c 6120 6872  left">.    <a hr
+000009a0: 6566 3d22 6874 7470 733a 2f2f 6575 6c65  ef="https://eule
+000009b0: 7273 7472 6561 6d2e 636f 6d22 2074 6172  rstream.com" tar
+000009c0: 6765 743d 225f 626c 616e 6b22 3e0a 2020  get="_blank">.  
+000009d0: 2020 2020 2020 3c64 6976 3e0a 2020 2020        <div>.    
+000009e0: 2020 2020 2020 2020 3c62 3e45 756c 6572          <b>Euler
+000009f0: 7374 7265 616d 3c2f 623e 206f 6666 6572  stream</b> offer
+00000a00: 7320 7061 6964 2070 6c61 6e73 2066 6f72  s paid plans for
+00000a10: 2065 6e74 6572 7072 6973 6573 2066 6f72   enterprises for
+00000a20: 2069 6e63 7265 6173 6564 2054 696b 546f   increased TikTo
+00000a30: 6b4c 6976 6520 6163 6365 7373 2026 2054  kLive access & T
+00000a40: 696b 546f 6b20 4150 4920 746f 6b65 6e73  ikTok API tokens
+00000a50: 2066 6f72 2064 6174 6120 636f 6c6c 6563   for data collec
+00000a60: 7469 6f6e 0a20 2020 2020 2020 203c 2f64  tion.        </d
+00000a70: 6976 3e0a 2020 2020 2020 2020 3c62 722f  iv>.        <br/
+00000a80: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
+00000a90: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+00000aa0: 7562 2e63 6f6d 2f69 7361 6163 6b6f 6761  ub.com/isaackoga
+00000ab0: 6e2f 5469 6b54 6f6b 4c69 7665 2f61 7373  n/TikTokLive/ass
+00000ac0: 6574 732f 3635 3836 3931 3036 2f62 3536  ets/65869106/b56
+00000ad0: 6365 6638 392d 3564 3837 2d34 6632 662d  cef89-5d87-4f2f-
+00000ae0: 6163 3365 2d30 3638 3561 6632 3162 3238  ac3e-0685af21b28
+00000af0: 6429 2220 7769 6474 683d 2231 3030 2220  d)" width="100" 
+00000b00: 616c 743d 2245 756c 6572 7374 7265 616d  alt="Eulerstream
+00000b10: 223e 0a20 2020 203c 2f61 3e0a 3c2f 6469  ">.    </a>.</di
+00000b20: 763e 0a0a 2323 2320 436f 6e73 6964 6572  v>..### Consider
+00000b30: 2044 6f6e 6174 696e 6720 3c33 0a0a 4927   Donating <3..I'
+00000b40: 6d20 6120 326e 642d 7965 6172 2042 696f  m a 2nd-year Bio
+00000b50: 6c6f 6779 2073 7475 6465 6e74 2069 6e20  logy student in 
+00000b60: 756e 6976 6572 7369 7479 2077 686f 206c  university who l
+00000b70: 696b 6573 2074 6f20 7072 6f67 7261 6d20  ikes to program 
+00000b80: 666f 7220 6675 6e2e 2050 6c65 6173 6520  for fun. Please 
+00000b90: 636f 6e73 6964 6572 2073 7570 706f 7274  consider support
+00000ba0: 696e 6720 6465 7665 6c6f 706d 656e 740a  ing development.
+00000bb0: 7468 726f 7567 6820 6120 736d 616c 6c20  through a small 
+00000bc0: 646f 6e61 7469 6f6e 2061 7420 5b68 7474  donation at [htt
+00000bd0: 7073 3a2f 2f77 7777 2e62 7579 6d65 6163  ps://www.buymeac
+00000be0: 6f66 6665 652e 636f 6d2f 6973 6161 636b  offee.com/isaack
+00000bf0: 6f67 616e 5d28 6874 7470 733a 2f2f 7777  ogan](https://ww
+00000c00: 772e 6275 796d 6561 636f 6666 6565 2e63  w.buymeacoffee.c
+00000c10: 6f6d 2f69 7361 6163 6b6f 6761 6e29 2e20  om/isaackogan). 
+00000c20: 416e 7974 6869 6e67 0a79 6f75 2063 616e  Anything.you can
+00000c30: 206f 6666 6572 2077 696c 6c20 676f 2074   offer will go t
+00000c40: 6f77 6172 6473 2073 6368 6f6f 6c20 2620  owards school & 
+00000c50: 6465 7665 6c6f 706d 656e 7420 636f 7374  development cost
+00000c60: 7320 666f 7220 5469 6b54 6f6b 4c69 7665  s for TikTokLive
+00000c70: 2c20 7768 6963 6820 6861 7320 7461 6b65  , which has take
+00000c80: 6e20 6875 6e64 7265 6473 206f 6620 686f  n hundreds of ho
+00000c90: 7572 7320 6f66 2074 696d 6520 746f 2062  urs of time to b
+00000ca0: 7569 6c64 2e0a 0a23 2323 204f 7468 6572  uild...### Other
+00000cb0: 204c 616e 6775 6167 6573 0a0a 5469 6b54   Languages..TikT
+00000cc0: 6f6b 4c69 7665 2069 7320 6176 6169 6c61  okLive is availa
+00000cd0: 626c 6520 696e 2073 6576 6572 616c 2061  ble in several a
+00000ce0: 6c74 6572 6e61 7465 2070 726f 6772 616d  lternate program
+00000cf0: 6d69 6e67 206c 616e 6775 6167 6573 3a0a  ming languages:.
+00000d00: 0a2d 202a 2a4e 6f64 652e 4a53 3a2a 2a20  .- **Node.JS:** 
+00000d10: 5b68 7474 7073 3a2f 2f67 6974 6875 622e  [https://github.
+00000d20: 636f 6d2f 7a65 726f 6479 7472 6173 682f  com/zerodytrash/
+00000d30: 5469 6b54 6f6b 2d4c 6976 652d 436f 6e6e  TikTok-Live-Conn
+00000d40: 6563 746f 725d 2868 7474 7073 3a2f 2f67  ector](https://g
+00000d50: 6974 6875 622e 636f 6d2f 7a65 726f 6479  ithub.com/zerody
+00000d60: 7472 6173 682f 5469 6b54 6f6b 2d4c 6976  trash/TikTok-Liv
+00000d70: 652d 436f 6e6e 6563 746f 7229 0a2d 202a  e-Connector).- *
+00000d80: 2a4a 6176 613a 2a2a 205b 6874 7470 733a  *Java:** [https:
+00000d90: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7764  //github.com/jwd
+00000da0: 6576 656c 6f70 6572 2f54 696b 546f 6b2d  eveloper/TikTok-
+00000db0: 4c69 7665 2d4a 6176 615d 2868 7474 7073  Live-Java](https
+00000dc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a77  ://github.com/jw
+00000dd0: 6465 7665 6c6f 7065 722f 5469 6b54 6f6b  developer/TikTok
+00000de0: 2d4c 6976 652d 4a61 7661 290a 2d20 2a2a  -Live-Java).- **
+00000df0: 4323 2f55 6e69 7479 3a2a 2a20 5b68 7474  C#/Unity:** [htt
+00000e00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000e10: 6672 616e 6b76 486f 6f66 3933 2f54 696b  frankvHoof93/Tik
+00000e20: 546f 6b4c 6976 6553 6861 7270 5d28 6874  TokLiveSharp](ht
+00000e30: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000e40: 2f66 7261 6e6b 7648 6f6f 6639 332f 5469  /frankvHoof93/Ti
+00000e50: 6b54 6f6b 4c69 7665 5368 6172 7029 0a2d  kTokLiveSharp).-
+00000e60: 202a 2a47 6f3a 2a2a 205b 6874 7470 733a   **Go:** [https:
+00000e70: 2f2f 6769 7468 7562 2e63 6f6d 2f44 6176  //github.com/Dav
+00000e80: 696e 6369 626c 652f 676f 7469 6b74 6f6b  incible/gotiktok
+00000e90: 6c69 7665 5d28 6874 7470 733a 2f2f 6769  live](https://gi
+00000ea0: 7468 7562 2e63 6f6d 2f44 6176 696e 6369  thub.com/Davinci
+00000eb0: 626c 652f 676f 7469 6b74 6f6b 6c69 7665  ble/gotiktoklive
+00000ec0: 290a 2d20 2a2a 5275 7374 3a2a 2a20 5b68  ).- **Rust:** [h
+00000ed0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ee0: 6d2f 6a77 6465 7665 6c6f 7065 722f 5469  m/jwdeveloper/Ti
+00000ef0: 6b54 6f6b 4c69 7665 5275 7374 5d28 6874  kTokLiveRust](ht
+00000f00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000f10: 2f6a 7764 6576 656c 6f70 6572 2f54 696b  /jwdeveloper/Tik
+00000f20: 546f 6b4c 6976 6552 7573 7429 0a0a 2323  TokLiveRust)..##
+00000f30: 2054 6162 6c65 206f 6620 436f 6e74 656e   Table of Conten
+00000f40: 7473 0a0a 2d20 5b44 6f63 756d 656e 7461  ts..- [Documenta
+00000f50: 7469 6f6e 5d28 6874 7470 733a 2f2f 6973  tion](https://is
+00000f60: 6161 636b 6f67 616e 2e67 6974 6875 622e  aackogan.github.
+00000f70: 696f 2f54 696b 546f 6b4c 6976 652f 290a  io/TikTokLive/).
+00000f80: 2d20 5b45 7861 6d70 6c65 735d 2868 7474  - [Examples](htt
+00000f90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000fa0: 6973 6161 636b 6f67 616e 2f54 696b 546f  isaackogan/TikTo
+00000fb0: 6b4c 6976 652f 7472 6565 2f6d 6173 7465  kLive/tree/maste
+00000fc0: 722f 6578 616d 706c 6573 290a 2d20 5b57  r/examples).- [W
+00000fd0: 696b 695d 2868 7474 7073 3a2f 2f67 6974  iki](https://git
+00000fe0: 6875 622e 636f 6d2f 6973 6161 636b 6f67  hub.com/isaackog
+00000ff0: 616e 2f54 696b 546f 6b4c 6976 652f 7769  an/TikTokLive/wi
+00001000: 6b69 2920 0a2d 205b 4c69 6365 6e73 696e  ki) .- [Licensin
+00001010: 675d 2823 6c69 6365 6e73 6529 0a2d 205b  g](#license).- [
+00001020: 436f 6e74 7269 6275 746f 7273 5d28 2363  Contributors](#c
+00001030: 6f6e 7472 6962 7574 6f72 7329 0a0a 2323  ontributors)..##
+00001040: 2047 6574 7469 6e67 2053 7461 7274 6564   Getting Started
+00001050: 0a0a 312e 2049 6e73 7461 6c6c 2074 6865  ..1. Install the
+00001060: 206d 6f64 756c 6520 7669 6120 7069 7020   module via pip 
+00001070: 6672 6f6d 2074 6865 205b 5079 5069 5d28  from the [PyPi](
+00001080: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00001090: 2f70 726f 6a65 6374 2f54 696b 546f 6b4c  /project/TikTokL
+000010a0: 6976 652f 2920 7265 706f 7369 746f 7279  ive/) repository
+000010b0: 0a0a 6060 6073 6865 6c6c 2073 6372 6970  ..```shell scrip
+000010c0: 740a 7069 7020 696e 7374 616c 6c20 5469  t.pip install Ti
+000010d0: 6b54 6f6b 4c69 7665 0a60 6060 0a0a 322e  kTokLive.```..2.
+000010e0: 2043 7265 6174 6520 796f 7572 2066 6972   Create your fir
+000010f0: 7374 2063 6861 7420 636f 6e6e 6563 7469  st chat connecti
+00001100: 6f6e 0a0a 6060 6070 7974 686f 6e0a 6672  on..```python.fr
+00001110: 6f6d 2054 696b 546f 6b4c 6976 6520 696d  om TikTokLive im
+00001120: 706f 7274 2054 696b 546f 6b4c 6976 6543  port TikTokLiveC
+00001130: 6c69 656e 740a 6672 6f6d 2054 696b 546f  lient.from TikTo
+00001140: 6b4c 6976 652e 6576 656e 7473 2069 6d70  kLive.events imp
+00001150: 6f72 7420 436f 6e6e 6563 7445 7665 6e74  ort ConnectEvent
+00001160: 2c20 436f 6d6d 656e 7445 7665 6e74 0a0a  , CommentEvent..
+00001170: 2320 4372 6561 7465 2074 6865 2063 6c69  # Create the cli
+00001180: 656e 740a 636c 6965 6e74 3a20 5469 6b54  ent.client: TikT
+00001190: 6f6b 4c69 7665 436c 6965 6e74 203d 2054  okLiveClient = T
+000011a0: 696b 546f 6b4c 6976 6543 6c69 656e 7428  ikTokLiveClient(
+000011b0: 756e 6971 7565 5f69 643d 2240 6973 6161  unique_id="@isaa
+000011c0: 636b 6f67 7a22 290a 0a0a 2320 4c69 7374  ckogz")...# List
+000011d0: 656e 2074 6f20 616e 2065 7665 6e74 2077  en to an event w
+000011e0: 6974 6820 6120 6465 636f 7261 746f 7221  ith a decorator!
+000011f0: 0a40 636c 6965 6e74 2e6f 6e28 436f 6e6e  .@client.on(Conn
+00001200: 6563 7445 7665 6e74 290a 6173 796e 6320  ectEvent).async 
+00001210: 6465 6620 6f6e 5f63 6f6e 6e65 6374 2865  def on_connect(e
+00001220: 7665 6e74 3a20 436f 6e6e 6563 7445 7665  vent: ConnectEve
+00001230: 6e74 293a 0a20 2020 2070 7269 6e74 2866  nt):.    print(f
+00001240: 2243 6f6e 6e65 6374 6564 2074 6f20 407b  "Connected to @{
+00001250: 6576 656e 742e 756e 6971 7565 5f69 647d  event.unique_id}
+00001260: 2028 526f 6f6d 2049 443a 207b 636c 6965   (Room ID: {clie
+00001270: 6e74 2e72 6f6f 6d5f 6964 7d22 290a 0a0a  nt.room_id}")...
+00001280: 2320 4f72 2c20 6164 6420 6974 206d 616e  # Or, add it man
+00001290: 7561 6c6c 7920 7669 6120 2263 6c69 656e  ually via "clien
+000012a0: 742e 6164 645f 6c69 7374 656e 6572 2829  t.add_listener()
+000012b0: 220a 6173 796e 6320 6465 6620 6f6e 5f63  ".async def on_c
+000012c0: 6f6d 6d65 6e74 2865 7665 6e74 3a20 436f  omment(event: Co
+000012d0: 6d6d 656e 7445 7665 6e74 2920 2d3e 204e  mmentEvent) -> N
+000012e0: 6f6e 653a 0a20 2020 2070 7269 6e74 2866  one:.    print(f
+000012f0: 227b 6576 656e 742e 7573 6572 2e6e 6963  "{event.user.nic
+00001300: 6b6e 616d 657d 202d 3e20 7b65 7665 6e74  kname} -> {event
+00001310: 2e63 6f6d 6d65 6e74 7d22 290a 0a0a 636c  .comment}")...cl
+00001320: 6965 6e74 2e61 6464 5f6c 6973 7465 6e65  ient.add_listene
+00001330: 7228 436f 6d6d 656e 7445 7665 6e74 2c20  r(CommentEvent, 
+00001340: 6f6e 5f63 6f6d 6d65 6e74 290a 0a69 6620  on_comment)..if 
+00001350: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+00001360: 6169 6e5f 5f27 3a0a 2020 2020 2320 5275  ain__':.    # Ru
+00001370: 6e20 7468 6520 636c 6965 6e74 2061 6e64  n the client and
+00001380: 2062 6c6f 636b 2074 6865 206d 6169 6e20   block the main 
+00001390: 7468 7265 6164 0a20 2020 2023 2061 7761  thread.    # awa
+000013a0: 6974 2063 6c69 656e 742e 7374 6172 7428  it client.start(
+000013b0: 2920 746f 2072 756e 206e 6f6e 2d62 6c6f  ) to run non-blo
+000013c0: 636b 696e 670a 2020 2020 636c 6965 6e74  cking.    client
+000013d0: 2e72 756e 2829 0a60 6060 0a0a 466f 7220  .run().```..For 
+000013e0: 6d6f 7265 2071 7569 636b 7374 6172 7420  more quickstart 
+000013f0: 6578 616d 706c 6573 2c20 7365 6520 7468  examples, see th
+00001400: 6520 5b65 7861 6d70 6c65 7320 666f 6c64  e [examples fold
+00001410: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
+00001420: 7562 2e63 6f6d 2f69 7361 6163 6b6f 6761  ub.com/isaackoga
+00001430: 6e2f 5469 6b54 6f6b 4c69 7665 2f74 7265  n/TikTokLive/tre
+00001440: 652f 6d61 7374 6572 2f65 7861 6d70 6c65  e/master/example
+00001450: 7329 0a70 726f 7669 6465 6420 696e 2074  s).provided in t
+00001460: 6865 2073 6f75 7263 6520 7472 6565 2e0a  he source tree..
+00001470: 0a23 2320 5061 7261 6d65 7465 7273 0a0a  .## Parameters..
+00001480: 7c20 5061 7261 6d20 4e61 6d65 207c 2052  | Param Name | R
+00001490: 6571 7569 7265 6420 7c20 4465 6661 756c  equired | Defaul
+000014a0: 7420 7c20 4465 7363 7269 7074 696f 6e20  t | Description 
+000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001580: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  |------------|--
+00001590: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
+000015a0: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
+000015b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000015c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000015d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000015e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000015f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
+00001680: 7c20 756e 6971 7565 5f69 6420 207c 2059  | unique_id  | Y
+00001690: 6573 2020 2020 2020 7c20 4e2f 4120 2020  es      | N/A   
+000016a0: 2020 7c20 5468 6520 756e 6971 7565 2075    | The unique u
+000016b0: 7365 726e 616d 6520 6f66 2074 6865 2062  sername of the b
+000016c0: 726f 6164 6361 7374 6572 2e20 596f 7520  roadcaster. You 
+000016d0: 6361 6e20 6669 6e64 2074 6869 7320 6e61  can find this na
+000016e0: 6d65 2069 6e20 7468 6520 5552 4c20 6f66  me in the URL of
+000016f0: 2074 6865 2075 7365 722e 2046 6f72 2065   the user. For e
+00001700: 7861 6d70 6c65 2c20 7468 6520 6075 6e69  xample, the `uni
+00001710: 7175 655f 6964 6020 666f 7220 5b60 6874  que_id` for [`ht
+00001720: 7470 733a 2f2f 7777 772e 7469 6b74 6f6b  tps://www.tiktok
+00001730: 2e63 6f6d 2f40 6973 6161 636b 6f67 7a60  .com/@isaackogz`
+00001740: 5d28 6874 7470 733a 2f2f 7777 772e 7469  ](https://www.ti
+00001750: 6b74 6f6b 2e63 6f6d 2f40 6973 6161 636b  ktok.com/@isaack
+00001760: 6f67 7a29 2077 6f75 6c64 2062 6520 6069  ogz) would be `i
+00001770: 7361 6163 6b6f 677a 602e 2020 2020 7c0a  saackogz`.    |.
+00001780: 7c20 7765 625f 7072 6f78 7920 207c 204e  | web_proxy  | N
+00001790: 6f20 2020 2020 2020 7c20 604e 6f6e 6560  o       | `None`
+000017a0: 2020 7c20 5469 6b54 6f6b 4c69 7665 2073    | TikTokLive s
+000017b0: 7570 706f 7274 7320 7072 6f78 7969 6e67  upports proxying
+000017c0: 2048 5454 5020 7265 7175 6573 7473 2e20   HTTP requests. 
+000017d0: 5468 6973 2070 6172 616d 6574 6572 2061  This parameter a
+000017e0: 6363 6570 7473 2061 6e20 6068 7474 7078  ccepts an `httpx
+000017f0: 2e50 726f 7879 602e 204e 6f74 6520 7468  .Proxy`. Note th
+00001800: 6174 2069 6620 796f 7520 646f 2075 7365  at if you do use
+00001810: 2061 2070 726f 7879 2079 6f75 206d 6179   a proxy you may
+00001820: 2062 6520 7375 626a 6563 7420 746f 2072   be subject to r
+00001830: 6564 7563 6564 2063 6f6e 6e65 6374 696f  educed connectio
+00001840: 6e20 6c69 6d69 7473 2061 7420 7469 6d65  n limits at time
+00001850: 7320 6f66 2068 6967 6820 6c6f 6164 2e20  s of high load. 
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001880: 7c20 7773 5f70 726f 7879 2020 207c 204e  | ws_proxy   | N
+00001890: 6f20 2020 2020 2020 7c20 604e 6f6e 6560  o       | `None`
+000018a0: 2020 7c20 5469 6b54 6f6b 4c69 7665 2073    | TikTokLive s
+000018b0: 7570 706f 7274 7320 7072 6f78 7969 6e67  upports proxying
+000018c0: 2074 6865 2077 6562 736f 636b 6574 2063   the websocket c
+000018d0: 6f6e 6e65 6374 696f 6e2e 2054 6869 7320  onnection. This 
+000018e0: 7061 7261 6d65 7465 7220 6163 6365 7074  parameter accept
+000018f0: 7320 616e 2060 6874 7470 782e 5072 6f78  s an `httpx.Prox
+00001900: 7960 2e20 5573 696e 6720 7468 6973 2070  y`. Using this p
+00001910: 726f 7879 2077 696c 6c20 6e65 7665 7220  roxy will never 
+00001920: 6265 2073 7562 6a65 6374 2074 6f20 7265  be subject to re
+00001930: 6475 6365 6420 636f 6e6e 6563 7469 6f6e  duced connection
+00001940: 206c 696d 6974 732e 2020 2020 2020 2020   limits.        
+00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001980: 7c20 7765 625f 6b77 6172 6773 207c 204e  | web_kwargs | N
+00001990: 6f20 2020 2020 2020 7c20 607b 7d60 2020  o       | `{}`  
+000019a0: 2020 7c20 556e 6465 7220 7468 6520 7363    | Under the sc
+000019b0: 656e 6573 2c20 7468 6520 5469 6b54 6f6b  enes, the TikTok
+000019c0: 4c69 7665 2048 5454 5020 636c 6965 6e74  Live HTTP client
+000019d0: 2075 7365 7320 7468 6520 5b60 6874 7470   uses the [`http
+000019e0: 7860 5d28 6874 7470 733a 2f2f 6769 7468  x`](https://gith
+000019f0: 7562 2e63 6f6d 2f65 6e63 6f64 652f 6874  ub.com/encode/ht
+00001a00: 7470 7829 206c 6962 7261 7279 2e20 4172  tpx) library. Ar
+00001a10: 6775 6d65 6e74 7320 7061 7373 6564 2074  guments passed t
+00001a20: 6f20 6077 6562 5f6b 7761 7267 7360 2077  o `web_kwargs` w
+00001a30: 696c 6c20 6265 2066 6f72 7761 7264 2074  ill be forward t
+00001a40: 6865 2074 6865 2075 6e64 6572 6c79 696e  he the underlyin
+00001a50: 6720 4854 5450 2063 6c69 656e 742e 2020  g HTTP client.  
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001a80: 7c20 7773 5f6b 7761 7267 7320 207c 204e  | ws_kwargs  | N
+00001a90: 6f20 2020 2020 2020 7c20 607b 7d60 2020  o       | `{}`  
+00001aa0: 2020 7c20 556e 6465 7220 7468 6520 7363    | Under the sc
+00001ab0: 656e 6573 2c20 5469 6b54 6f6b 4c69 7665  enes, TikTokLive
+00001ac0: 2075 7365 7320 7468 6520 5b60 7765 6273   uses the [`webs
+00001ad0: 6f63 6b65 7473 605d 2868 7474 7073 3a2f  ockets`](https:/
+00001ae0: 2f67 6974 6875 622e 636f 6d2f 7079 7468  /github.com/pyth
+00001af0: 6f6e 2d77 6562 736f 636b 6574 732f 7765  on-websockets/we
+00001b00: 6273 6f63 6b65 7473 2920 6c69 6272 6172  bsockets) librar
+00001b10: 7920 746f 2063 6f6e 6e65 6374 2074 6f20  y to connect to 
+00001b20: 5469 6b54 6f6b 2e20 4172 6775 6d65 6e74  TikTok. Argument
+00001b30: 7320 7061 7373 6564 2074 6f20 6077 735f  s passed to `ws_
+00001b40: 6b77 6172 6773 6020 7769 6c6c 2062 6520  kwargs` will be 
+00001b50: 666f 7277 6172 6465 6420 746f 2074 6865  forwarded to the
+00001b60: 2075 6e64 6572 6c79 696e 6720 5765 6253   underlying WebS
+00001b70: 6f63 6b65 7420 636c 6965 6e74 2e20 7c0a  ocket client. |.
+00001b80: 0a23 2320 4d65 7468 6f64 730a 0a41 2060  .## Methods..A `
+00001b90: 5469 6b54 6f6b 4c69 7665 436c 6965 6e74  TikTokLiveClient
+00001ba0: 6020 6f62 6a65 6374 2063 6f6e 7461 696e  ` object contain
+00001bb0: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
+00001bc0: 696d 706f 7274 616e 7420 6d65 7468 6f64  important method
+00001bd0: 733a 0a0a 7c20 4d65 7468 6f64 204e 616d  s:..| Method Nam
+00001be0: 6520 207c 204e 6f74 6573 2020 207c 2044  e  | Notes   | D
+00001bf0: 6573 6372 6970 7469 6f6e 2020 2020 2020  escription      
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c90: 2020 2020 2020 2020 2020 7c0a 7c2d 2d2d            |.|---
+00001ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
+00001cb0: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
+00001cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d60: 2d2d 7c0a 7c20 7275 6e20 2020 2020 2020  --|.| run       
+00001d70: 2020 207c 204e 2f41 2020 2020 207c 2043     | N/A     | C
+00001d80: 6f6e 6e65 6374 2074 6f20 7468 6520 6c69  onnect to the li
+00001d90: 7665 7374 7265 616d 2061 6e64 2062 6c6f  vestream and blo
+00001da0: 636b 2074 6865 206d 6169 6e20 7468 7265  ck the main thre
+00001db0: 6164 2e20 5468 6973 2069 7320 6265 7374  ad. This is best
+00001dc0: 2066 6f72 2073 6d61 6c6c 2073 6372 6970   for small scrip
+00001dd0: 7473 2e20 2020 2020 2020 2020 2020 2020  ts.             
+00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e10: 2020 2020 2020 2020 2020 207c 0a7c 2064             |.| d
-00001e20: 6973 636f 6e6e 6563 7420 2020 7c20 6061  isconnect   | `a
-00001e30: 7379 6e63 6020 7c20 4469 7363 6f6e 6e65  sync` | Disconne
-00001e40: 6374 7320 7468 6520 636c 6965 6e74 2066  cts the client f
-00001e50: 726f 6d20 7468 6520 7765 6273 6f63 6b65  rom the websocke
-00001e60: 7420 6772 6163 6566 756c 6c79 2c20 7072  t gracefully, pr
-00001e70: 6f63 6573 7369 6e67 2072 656d 6169 6e69  ocessing remaini
-00001e80: 6e67 2065 7665 6e74 7320 6265 666f 7265  ng events before
-00001e90: 2065 6e64 696e 6720 7468 6520 636c 6965   ending the clie
-00001ea0: 6e74 206c 6f6f 702e 2020 2020 2020 2020  nt loop.        
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2020 207c 0a0a 2323 2050 726f 7065 7274     |..## Propert
-00001ef0: 6965 730a 0a41 2060 5469 6b54 6f6b 4c69  ies..A `TikTokLi
-00001f00: 7665 436c 6965 6e74 6020 6f62 6a65 6374  veClient` object
-00001f10: 2063 6f6e 7461 696e 7320 7468 6520 666f   contains the fo
-00001f20: 6c6c 6f77 696e 6720 696d 706f 7274 616e  llowing importan
-00001f30: 7420 7072 6f70 6572 7469 6573 3a0a 0a7c  t properties:..|
-00001f40: 2041 7474 7269 6275 7465 204e 616d 6520   Attribute Name 
-00001f50: 7c20 4465 7363 7269 7074 696f 6e20 2020  | Description   
-00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e10: 2020 2020 7c0a 7c20 6164 645f 6c69 7374      |.| add_list
+00001e20: 656e 6572 207c 204e 2f41 2020 2020 207c  ener | N/A     |
+00001e30: 2041 6464 7320 616e 202a 6173 796e 6368   Adds an *asynch
+00001e40: 726f 6e6f 7573 2a20 6c69 7374 656e 6572  ronous* listener
+00001e50: 2066 756e 6374 696f 6e20 286f 722c 2079   function (or, y
+00001e60: 6f75 2063 616e 2064 6563 6f72 6174 6520  ou can decorate 
+00001e70: 6120 6675 6e63 7469 6f6e 2077 6974 6820  a function with 
+00001e80: 6040 636c 6965 6e74 2e6f 6e28 223c 6576  `@client.on("<ev
+00001e90: 656e 743e 2229 6029 2061 6e64 2074 616b  ent>")`) and tak
+00001ea0: 6573 2074 776f 2070 6172 616d 6574 6572  es two parameter
+00001eb0: 732c 2061 6e20 6576 656e 7420 6e61 6d65  s, an event name
+00001ec0: 2061 6e64 2074 6865 2070 6179 6c6f 6164   and the payload
+00001ed0: 2c20 616e 2041 6273 7472 6163 7445 7665  , an AbstractEve
+00001ee0: 6e74 207c 7c0a 7c20 636f 6e6e 6563 7420  nt ||.| connect 
+00001ef0: 2020 2020 207c 2060 6173 796e 6360 207c       | `async` |
+00001f00: 2043 6f6e 6e65 6374 7320 746f 2074 6865   Connects to the
+00001f10: 2074 696b 746f 6b20 6c69 7665 2063 6861   tiktok live cha
+00001f20: 7420 7768 696c 6520 626c 6f63 6b69 6e67  t while blocking
+00001f30: 2074 6865 2063 7572 7265 6e74 2066 7574   the current fut
+00001f40: 7572 652e 2057 6865 6e20 7468 6520 636f  ure. When the co
+00001f50: 6e6e 6563 7469 6f6e 2065 6e64 7320 2865  nnection ends (e
+00001f60: 2e67 2e20 6c69 7665 7374 7265 616d 2069  .g. livestream i
+00001f70: 7320 6f76 6572 292c 2074 6865 2066 7574  s over), the fut
+00001f80: 7572 6520 6973 2072 656c 6561 7365 642e  ure is released.
 00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fe0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00001ff0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
-00002000: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
-00002010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-000020a0: 0a7c 2072 6f6f 6d5f 6964 2020 2020 2020  .| room_id      
-000020b0: 2020 7c20 5468 6520 526f 6f6d 2049 4420    | The Room ID 
-000020c0: 6f66 2074 6865 206c 6976 6573 7472 6561  of the livestrea
-000020d0: 6d20 726f 6f6d 2074 6865 2063 6c69 656e  m room the clien
-000020e0: 7420 6973 2063 7572 7265 6e74 6c79 2063  t is currently c
-000020f0: 6f6e 6e65 6374 6564 2074 6f2e 2020 2020  onnected to.    
-00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fa0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00001fb0: 7374 6172 7420 2020 2020 2020 207c 2060  start        | `
+00001fc0: 6173 796e 6360 207c 2043 6f6e 6e65 6374  async` | Connect
+00001fd0: 7320 746f 2074 6865 206c 6976 6520 6368  s to the live ch
+00001fe0: 6174 2077 6974 686f 7574 2062 6c6f 636b  at without block
+00001ff0: 696e 6720 7468 6520 6d61 696e 2074 6872  ing the main thr
+00002000: 6561 642e 2054 6869 7320 7265 7475 726e  ead. This return
+00002010: 7320 616e 2060 6173 796e 6369 6f2e 5461  s an `asyncio.Ta
+00002020: 736b 6020 6f62 6a65 6374 2077 6974 6820  sk` object with 
+00002030: 7468 6520 636c 6965 6e74 206c 6f6f 702e  the client loop.
+00002040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002070: 2020 2020 7c0a 7c20 6469 7363 6f6e 6e65      |.| disconne
+00002080: 6374 2020 207c 2060 6173 796e 6360 207c  ct   | `async` |
+00002090: 2044 6973 636f 6e6e 6563 7473 2074 6865   Disconnects the
+000020a0: 2063 6c69 656e 7420 6672 6f6d 2074 6865   client from the
+000020b0: 2077 6562 736f 636b 6574 2067 7261 6365   websocket grace
+000020c0: 6675 6c6c 792c 2070 726f 6365 7373 696e  fully, processin
+000020d0: 6720 7265 6d61 696e 696e 6720 6576 656e  g remaining even
+000020e0: 7473 2062 6566 6f72 6520 656e 6469 6e67  ts before ending
+000020f0: 2074 6865 2063 6c69 656e 7420 6c6f 6f70   the client loop
+00002100: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
 00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002150: 7c0a 7c20 7765 6220 2020 2020 2020 2020  |.| web         
-00002160: 2020 207c 2054 6865 2054 696b 546f 6b20     | The TikTok 
-00002170: 4854 5450 2063 6c69 656e 742e 2054 6869  HTTP client. Thi
-00002180: 7320 636c 6965 6e74 2068 6173 2061 206c  s client has a l
-00002190: 6f74 206f 6620 7573 6566 756c 2072 6f75  ot of useful rou
-000021a0: 7465 7320 796f 7520 7368 6f75 6c64 2065  tes you should e
-000021b0: 7870 6c6f 7265 2120 2020 2020 2020 2020  xplore!         
+00002130: 2020 2020 2020 2020 2020 2020 7c0a 0a23              |..#
+00002140: 2320 5072 6f70 6572 7469 6573 0a0a 4120  # Properties..A 
+00002150: 6054 696b 546f 6b4c 6976 6543 6c69 656e  `TikTokLiveClien
+00002160: 7460 206f 626a 6563 7420 636f 6e74 6169  t` object contai
+00002170: 6e73 2074 6865 2066 6f6c 6c6f 7769 6e67  ns the following
+00002180: 2069 6d70 6f72 7461 6e74 2070 726f 7065   important prope
+00002190: 7274 6965 733a 0a0a 7c20 4174 7472 6962  rties:..| Attrib
+000021a0: 7574 6520 4e61 6d65 207c 2044 6573 6372  ute Name | Descr
+000021b0: 6970 7469 6f6e 2020 2020 2020 2020 2020  iption          
 000021c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 207c 0a7c 2063 6f6e 6e65 6374 6564 2020   |.| connected  
-00002210: 2020 2020 7c20 5768 6574 6865 7220 796f      | Whether yo
-00002220: 7520 6172 6520 6375 7272 656e 746c 7920  u are currently 
-00002230: 636f 6e6e 6563 7465 6420 746f 2074 6865  connected to the
-00002240: 206c 6976 6573 7472 6561 6d2e 2020 2020   livestream.    
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022b0: 2020 7c0a 7c20 6c6f 6767 6572 2020 2020    |.| logger    
-000022c0: 2020 2020 207c 2054 6865 2069 6e74 6572       | The inter
-000022d0: 6e61 6c20 6c6f 6767 6572 2075 7365 6420  nal logger used 
-000022e0: 6279 2054 696b 546f 6b4c 6976 652e 2059  by TikTokLive. Y
-000022f0: 6f75 2063 616e 2075 7365 2060 636c 6965  ou can use `clie
-00002300: 6e74 2e6c 6f67 6765 722e 7365 744c 6576  nt.logger.setLev
-00002310: 656c 282e 2e2e 2960 206d 6574 686f 6420  el(...)` method 
-00002320: 746f 2065 6e61 626c 6520 636c 6965 6e74  to enable client
-00002330: 2064 6562 7567 2e20 2020 2020 2020 2020   debug.         
-00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002360: 2020 207c 0a7c 2072 6f6f 6d5f 696e 666f     |.| room_info
-00002370: 2020 2020 2020 7c20 526f 6f6d 2069 6e66        | Room inf
-00002380: 6f72 6d61 7469 6f6e 2074 6861 7420 6973  ormation that is
-00002390: 2072 6574 7269 6576 6564 2066 726f 6d20   retrieved from 
-000023a0: 5469 6b54 6f6b 2077 6865 6e20 796f 7520  TikTok when you 
-000023b0: 7573 6520 6120 636f 6e6e 6563 7469 6f6e  use a connection
-000023c0: 206d 6574 686f 6420 2865 2e67 2e20 6063   method (e.g. `c
-000023d0: 6c69 656e 742e 636f 6e6e 6563 7460 2920  lient.connect`) 
-000023e0: 7769 7468 2074 6865 206b 6579 776f 7264  with the keyword
-000023f0: 2061 7267 756d 656e 7420 6066 6574 6368   argument `fetch
-00002400: 5f72 6f6f 6d5f 696e 666f 3d54 7275 6560  _room_info=True`
-00002410: 202e 2020 7c0a 7c20 6769 6674 5f69 6e66   .  |.| gift_inf
-00002420: 6f20 2020 2020 207c 2045 7874 7261 2067  o      | Extra g
-00002430: 6966 7420 696e 666f 726d 6174 696f 6e20  ift information 
-00002440: 7468 6174 2069 7320 7265 7472 6965 7665  that is retrieve
-00002450: 6420 6672 6f6d 2054 696b 546f 6b20 7768  d from TikTok wh
-00002460: 656e 2079 6f75 2075 7365 2061 2063 6f6e  en you use a con
-00002470: 6e65 6374 696f 6e20 6d65 7468 6f64 2028  nection method (
-00002480: 652e 672e 2060 636c 6965 6e74 2e72 756e  e.g. `client.run
-00002490: 6029 2077 6974 6820 7468 6520 6b65 7977  `) with the keyw
-000024a0: 6f72 6420 6172 6775 6d65 6e74 2060 6665  ord argument `fe
-000024b0: 7463 685f 6769 6674 5f69 6e66 6f3d 5472  tch_gift_info=Tr
-000024c0: 7565 602e 207c 0a0a 0a23 2320 5765 6244  ue`. |...## WebD
-000024d0: 6566 6175 6c74 730a 0a54 696b 546f 6b4c  efaults..TikTokL
-000024e0: 6976 6520 6861 7320 6120 7365 7269 6573  ive has a series
-000024f0: 206f 6620 676c 6f62 616c 2064 6566 6175   of global defau
-00002500: 6c74 7320 7573 6564 2074 6f20 6372 6561  lts used to crea
-00002510: 7465 2074 6865 2048 5454 5020 636c 6965  te the HTTP clie
-00002520: 6e74 2077 6869 6368 2079 6f75 2063 616e  nt which you can
-00002530: 2063 7573 746f 6d69 7a65 2e20 466f 7220   customize. For 
-00002540: 696e 666f 206f 6e20 686f 7720 746f 2073  info on how to s
-00002550: 6574 2074 6865 7365 2070 6172 616d 6574  et these paramet
-00002560: 6572 732c 2073 6565 0a74 6865 205b 7765  ers, see.the [we
-00002570: 625f 6465 6661 756c 7473 2e70 795d 2868  b_defaults.py](h
-00002580: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002590: 6d2f 6973 6161 636b 6f67 616e 2f54 696b  m/isaackogan/Tik
-000025a0: 546f 6b4c 6976 652f 626c 6f62 2f6d 6173  TokLive/blob/mas
-000025b0: 7465 722f 6578 616d 706c 6573 2f77 6562  ter/examples/web
-000025c0: 5f64 6566 6175 6c74 732e 7079 2920 6578  _defaults.py) ex
-000025d0: 616d 706c 652e 0a0a 7c20 5061 7261 6d65  ample...| Parame
-000025e0: 7465 7220 2020 2020 2020 2020 2020 7c20  ter           | 
-000025f0: 5479 7065 2020 207c 2044 6573 6372 6970  Type   | Descrip
-00002600: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002680: 2020 2020 2020 7c0a 7c2d 2d2d 2d2d 2d2d        |.|-------
-00002690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
-000026a0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-000026b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002730: 2d2d 2d2d 2d2d 7c0a 7c20 7469 6b74 6f6b  ------|.| tiktok
-00002740: 5f61 7070 5f75 726c 2020 2020 2020 7c20  _app_url      | 
-00002750: 6073 7472 6020 207c 2054 6865 2054 696b  `str`  | The Tik
-00002760: 546f 6b20 6170 7020 5552 4c20 2860 6874  Tok app URL (`ht
-00002770: 7470 733a 2f2f 7777 772e 7469 6b74 6f6b  tps://www.tiktok
-00002780: 2e63 6f6d 6029 2075 7365 6420 746f 2073  .com`) used to s
-00002790: 6372 6170 6520 7468 6520 726f 6f6d 2e20  crape the room. 
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027e0: 2020 2020 2020 7c0a 7c20 7469 6b74 6f6b        |.| tiktok
-000027f0: 5f73 6967 6e5f 7572 6c20 2020 2020 7c20  _sign_url     | 
-00002800: 6073 7472 6020 207c 2054 6865 205b 7369  `str`  | The [si
-00002810: 676e 6174 7572 6520 7365 7276 6572 5d28  gnature server](
-00002820: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002830: 6f6d 2f69 7361 6163 6b6f 6761 6e2f 5469  om/isaackogan/Ti
-00002840: 6b54 6f6b 4c69 7665 2f77 696b 692f 416c  kTokLive/wiki/Al
-00002850: 6c2d 4162 6f75 742d 5369 676e 6174 7572  l-About-Signatur
-00002860: 6573 2920 7573 6564 2074 6f20 6765 6e65  es) used to gene
-00002870: 7261 7465 2074 6f6b 656e 7320 746f 2063  rate tokens to c
-00002880: 6f6e 6e65 6374 2074 6f20 5469 6b54 6f6b  onnect to TikTok
-00002890: 4c69 7665 2e20 7c0a 7c20 7469 6b74 6f6b  Live. |.| tiktok
-000028a0: 5f77 6562 6361 7374 5f75 726c 2020 7c20  _webcast_url  | 
-000028b0: 6073 7472 6020 207c 2054 6865 2054 696b  `str`  | The Tik
-000028c0: 546f 6b20 6c69 7665 7374 7265 616d 2055  Tok livestream U
-000028d0: 524c 2028 6068 7474 7073 3a2f 2f77 6562  RL (`https://web
-000028e0: 6361 7374 2e74 696b 746f 6b2e 636f 6d60  cast.tiktok.com`
-000028f0: 2920 7768 6572 6520 6c69 7665 7374 7265  ) where livestre
-00002900: 616d 7320 6361 6e20 6265 2061 6363 6573  ams can be acces
-00002910: 7365 6420 6672 6f6d 2e20 2020 2020 2020  sed from.       
-00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002940: 2020 2020 2020 7c0a 7c20 636c 6965 6e74        |.| client
-00002950: 5f70 6172 616d 7320 2020 2020 2020 7c20  _params       | 
-00002960: 6064 6963 7460 207c 2054 6865 2055 524c  `dict` | The URL
-00002970: 2070 6172 616d 6574 6572 7320 6164 6465   parameters adde
-00002980: 6420 6f6e 2074 6f20 5469 6b54 6f6b 2072  d on to TikTok r
-00002990: 6571 7565 7374 7320 6672 6f6d 2074 6865  equests from the
-000029a0: 2048 5454 5020 636c 6965 6e74 2e20 2020   HTTP client.   
-000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2020 2020 2020 7c0a 7c20 636c 6965 6e74        |.| client
-00002a00: 5f68 6561 6465 7273 2020 2020 2020 7c20  _headers      | 
-00002a10: 6064 6963 7460 207c 2054 6865 2068 6561  `dict` | The hea
-00002a20: 6465 7273 2061 6464 6564 206f 6e20 746f  ders added on to
-00002a30: 2054 696b 546f 6b20 7265 7175 6573 7473   TikTok requests
-00002a40: 2066 726f 6d20 7468 6520 4854 5450 2063   from the HTTP c
-00002a50: 6c69 656e 742e 2020 2020 2020 2020 2020  lient.          
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002aa0: 2020 2020 2020 7c0a 7c20 7469 6b74 6f6b        |.| tiktok
-00002ab0: 5f73 6967 6e5f 6170 695f 6b65 7920 7c20  _sign_api_key | 
-00002ac0: 6073 7472 6020 207c 2041 2067 6c6f 6261  `str`  | A globa
-00002ad0: 6c20 7761 7920 6f66 2073 6574 7469 6e67  l way of setting
-00002ae0: 2074 6865 2060 7369 676e 5f61 7069 5f6b   the `sign_api_k
-00002af0: 6579 6020 7061 7261 6d65 7465 722e 2020  ey` parameter.  
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b50: 2020 2020 2020 7c0a 0a23 2320 4576 656e        |..## Even
-00002b60: 7473 0a0a 4576 656e 7473 2063 616e 2062  ts..Events can b
-00002b70: 6520 6c69 7374 656e 6564 2074 6f20 7573  e listened to us
-00002b80: 696e 6720 6120 6465 636f 7261 746f 7220  ing a decorator 
-00002b90: 6f72 206e 6f6e 2d64 6563 6f72 6174 6f72  or non-decorator
-00002ba0: 206d 6574 686f 6420 6361 6c6c 2e20 5468   method call. Th
-00002bb0: 6520 666f 6c6c 6f77 696e 6720 6578 616d  e following exam
-00002bc0: 706c 6573 2069 6c6c 7573 7472 6174 6520  ples illustrate 
-00002bd0: 686f 7720 796f 7520 6361 6e20 6c69 7374  how you can list
-00002be0: 656e 2074 6f20 616e 2065 7665 6e74 3a0a  en to an event:.
-00002bf0: 0a60 6060 7079 7468 6f6e 0a40 636c 6965  .```python.@clie
-00002c00: 6e74 2e6f 6e28 4c69 6b65 4576 656e 7429  nt.on(LikeEvent)
-00002c10: 0a61 7379 6e63 2064 6566 206f 6e5f 6c69  .async def on_li
-00002c20: 6b65 2865 7665 6e74 3a20 4c69 6b65 4576  ke(event: LikeEv
-00002c30: 656e 7429 202d 3e20 4e6f 6e65 3a0a 2020  ent) -> None:.  
-00002c40: 2020 2e2e 2e0a 0a61 7379 6e63 2064 6566    .....async def
-00002c50: 206f 6e5f 636f 6d6d 656e 7428 6576 656e   on_comment(even
-00002c60: 743a 2043 6f6d 6d65 6e74 4576 656e 7429  t: CommentEvent)
-00002c70: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2e2e   -> None:.    ..
-00002c80: 2e0a 0a63 6c69 656e 742e 6164 645f 6c69  ...client.add_li
-00002c90: 7374 656e 6572 2843 6f6d 6d65 6e74 4576  stener(CommentEv
-00002ca0: 656e 742c 206f 6e5f 636f 6d6d 656e 7429  ent, on_comment)
-00002cb0: 0a60 6060 0a0a 5468 6572 6520 6172 6520  .```..There are 
-00002cc0: 7477 6f20 7479 7065 7320 6f66 2065 7665  two types of eve
-00002cd0: 6e74 732c 205b 6043 7573 746f 6d45 7665  nts, [`CustomEve
-00002ce0: 6e74 605d 2868 7474 7073 3a2f 2f67 6974  nt`](https://git
-00002cf0: 6875 622e 636f 6d2f 6973 6161 636b 6f67  hub.com/isaackog
-00002d00: 616e 2f54 696b 546f 6b4c 6976 652f 626c  an/TikTokLive/bl
-00002d10: 6f62 2f6d 6173 7465 722f 5469 6b54 6f6b  ob/master/TikTok
-00002d20: 4c69 7665 2f65 7665 6e74 732f 6375 7374  Live/events/cust
-00002d30: 6f6d 5f65 7665 6e74 732e 7079 2920 0a65  om_events.py) .e
-00002d40: 7665 6e74 7320 616e 6420 5b60 5072 6f74  vents and [`Prot
-00002d50: 6f45 7665 6e74 605d 2868 7474 7073 3a2f  oEvent`](https:/
-00002d60: 2f67 6974 6875 622e 636f 6d2f 6973 6161  /github.com/isaa
-00002d70: 636b 6f67 616e 2f54 696b 546f 6b4c 6976  ckogan/TikTokLiv
-00002d80: 652f 626c 6f62 2f6d 6173 7465 722f 5469  e/blob/master/Ti
-00002d90: 6b54 6f6b 4c69 7665 2f65 7665 6e74 732f  kTokLive/events/
-00002da0: 7072 6f74 6f5f 6576 656e 7473 2e70 7929  proto_events.py)
-00002db0: 2065 7665 6e74 732e 0a42 6f74 6820 6265   events..Both be
-00002dc0: 6c6f 6e67 2074 6f20 7468 6520 5469 6b54  long to the TikT
-00002dd0: 6f6b 4c69 7665 2060 4576 656e 7460 2074  okLive `Event` t
-00002de0: 7970 6520 616e 6420 6361 6e20 6265 206c  ype and can be l
-00002df0: 6973 7465 6e65 6420 746f 2e20 5468 6520  istened to. The 
-00002e00: 666f 6c6c 6f77 696e 6720 6576 656e 7473  following events
-00002e10: 2061 7265 2061 7661 696c 6162 6c65 3a0a   are available:.
-00002e20: 0a23 2323 2043 7573 746f 6d20 4576 656e  .### Custom Even
-00002e30: 7473 0a0a 2d20 6043 6f6e 6e65 6374 4576  ts..- `ConnectEv
-00002e40: 656e 7460 202d 2054 7269 6767 6572 6564  ent` - Triggered
-00002e50: 2077 6865 6e20 7468 6520 5765 6263 6173   when the Webcas
-00002e60: 7420 636f 6e6e 6563 7469 6f6e 2069 7320  t connection is 
-00002e70: 696e 6974 6961 7465 640a 2d20 6044 6973  initiated.- `Dis
-00002e80: 636f 6e6e 6563 7445 7665 6e74 6020 2d20  connectEvent` - 
-00002e90: 5472 6967 6765 7265 6420 7768 656e 2074  Triggered when t
-00002ea0: 6865 2057 6562 6361 7374 2063 6f6e 6e65  he Webcast conne
-00002eb0: 6374 696f 6e20 636c 6f73 6573 2028 696e  ction closes (in
-00002ec0: 636c 7564 696e 6720 7468 6520 6c69 7665  cluding the live
-00002ed0: 7374 7265 616d 2065 6e64 696e 6729 0a2d  stream ending).-
-00002ee0: 2060 4c69 7665 456e 6445 7665 6e74 6020   `LiveEndEvent` 
-00002ef0: 2d20 5472 6967 6765 7265 6420 7768 656e  - Triggered when
-00002f00: 2074 6865 206c 6976 6573 7472 6561 6d20   the livestream 
-00002f10: 656e 6473 0a2d 2060 4c69 7665 5061 7573  ends.- `LivePaus
-00002f20: 6545 7665 6e74 6020 2d20 5472 6967 6765  eEvent` - Trigge
-00002f30: 7265 6420 7768 656e 2074 6865 206c 6976  red when the liv
-00002f40: 6573 7472 6561 6d20 6973 2070 6175 7365  estream is pause
-00002f50: 640a 2d20 604c 6976 6555 6e70 6175 7365  d.- `LiveUnpause
-00002f60: 4576 656e 7460 202d 2054 7269 6767 6572  Event` - Trigger
-00002f70: 6564 2077 6865 6e20 7468 6520 6c69 7665  ed when the live
-00002f80: 7374 7265 616d 2069 7320 756e 7061 7573  stream is unpaus
-00002f90: 6564 0a2d 2060 466f 6c6c 6f77 4576 656e  ed.- `FollowEven
-00002fa0: 7460 202d 2054 7269 6767 6572 6564 2077  t` - Triggered w
-00002fb0: 6865 6e20 6120 7573 6572 2069 6e20 7468  hen a user in th
-00002fc0: 6520 6c69 7665 7374 7265 616d 2066 6f6c  e livestream fol
-00002fd0: 6c6f 7773 2074 6865 2073 7472 6561 6d65  lows the streame
-00002fe0: 720a 2d20 6053 6861 7265 4576 656e 7460  r.- `ShareEvent`
-00002ff0: 202d 2054 7269 6767 6572 6564 2077 6865   - Triggered whe
-00003000: 6e20 6120 7573 6572 2073 6861 7265 7320  n a user shares 
-00003010: 7468 6520 6c69 7665 7374 7265 616d 0a2d  the livestream.-
-00003020: 2060 5765 6273 6f63 6b65 7452 6573 706f   `WebsocketRespo
-00003030: 6e73 6545 7665 6e74 6020 2d20 5472 6967  nseEvent` - Trig
-00003040: 6765 7265 6420 7768 656e 2061 6e79 2065  gered when any e
-00003050: 7665 6e74 2069 7320 7265 6365 6976 6564  vent is received
-00003060: 2028 636f 6e74 6169 6e73 2074 6865 2065   (contains the e
-00003070: 7665 6e74 290a 2d20 6055 6e6b 6e6f 776e  vent).- `Unknown
-00003080: 4576 656e 7460 202d 2041 6e20 696e 7374  Event` - An inst
-00003090: 616e 6365 206f 6620 6057 6562 736f 636b  ance of `Websock
-000030a0: 6574 5265 7370 6f6e 7365 4576 656e 7460  etResponseEvent`
-000030b0: 2074 6872 6f77 6e20 7768 656e 6576 6572   thrown whenever
-000030c0: 2061 6e20 6576 656e 7420 646f 6573 206e   an event does n
-000030d0: 6f74 2068 6176 6520 616e 2065 7869 7374  ot have an exist
-000030e0: 696e 6720 6465 6669 6e69 7469 6f6e 2c20  ing definition, 
-000030f0: 7573 6566 756c 2066 6f72 2064 6562 7567  useful for debug
-00003100: 6769 6e67 0a0a 2323 2320 5072 6f74 6f20  ging..### Proto 
-00003110: 4576 656e 7473 0a0a 4966 2079 6f75 206b  Events..If you k
-00003120: 6e6f 7720 7768 6174 2061 6e20 6576 656e  now what an even
-00003130: 7420 646f 6573 2c20 5b6d 616b 6520 6120  t does, [make a 
-00003140: 7075 6c6c 2072 6571 7565 7374 5d28 6874  pull request](ht
-00003150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003160: 2f69 7361 6163 6b6f 6761 6e2f 5469 6b54  /isaackogan/TikT
-00003170: 6f6b 4c69 7665 2f70 756c 6c73 2920 616e  okLive/pulls) an
-00003180: 6420 6164 6420 7468 6520 6465 7363 7269  d add the descri
-00003190: 7074 696f 6e2e 200a 0a2d 2060 4769 6674  ption. ..- `Gift
-000031a0: 4576 656e 7460 202d 2054 7269 6767 6572  Event` - Trigger
-000031b0: 6564 2077 6865 6e20 6120 6769 6674 2069  ed when a gift i
-000031c0: 7320 7365 6e74 2074 6f20 7468 6520 7374  s sent to the st
-000031d0: 7265 616d 6572 0a2d 2060 476f 616c 5570  reamer.- `GoalUp
-000031e0: 6461 7465 4576 656e 7460 202d 2054 7269  dateEvent` - Tri
-000031f0: 6767 6572 6564 2077 6865 6e20 7468 6520  ggered when the 
-00003200: 7375 6273 6372 6962 6572 2067 6f61 6c20  subscriber goal 
-00003210: 6973 2075 7064 6174 6564 0a2d 2060 436f  is updated.- `Co
-00003220: 6e74 726f 6c45 7665 6e74 6020 2d20 5472  ntrolEvent` - Tr
-00003230: 6967 6765 7265 6420 7768 656e 2061 2073  iggered when a s
-00003240: 7472 6561 6d20 6163 7469 6f6e 206f 6363  tream action occ
-00003250: 7572 7320 2865 2e67 2e20 4c69 7665 7374  urs (e.g. Livest
-00003260: 7265 616d 2073 7461 7274 2c20 656e 6429  ream start, end)
-00003270: 0a2d 2060 4c69 6b65 4576 656e 7460 202d  .- `LikeEvent` -
-00003280: 2054 7269 6767 6572 6564 2077 6865 6e20   Triggered when 
-00003290: 7468 6520 7374 7265 616d 2072 6563 6569  the stream recei
-000032a0: 7665 7320 6120 6c69 6b65 0a2d 2060 5375  ves a like.- `Su
-000032b0: 6273 6372 6962 6545 7665 6e74 6020 2d20  bscribeEvent` - 
-000032c0: 5472 6967 6765 7265 6420 7768 656e 2073  Triggered when s
-000032d0: 6f6d 656f 6e65 2073 7562 7363 7269 6265  omeone subscribe
-000032e0: 7320 746f 2074 6865 2054 696b 546f 6b20  s to the TikTok 
-000032f0: 6372 6561 746f 720a 2d20 6050 6f6c 6c45  creator.- `PollE
-00003300: 7665 6e74 6020 2d20 5472 6967 6765 7265  vent` - Triggere
-00003310: 6420 7768 656e 2074 6865 2063 7265 6174  d when the creat
-00003320: 6f72 206c 6175 6e63 6865 7320 6120 6e65  or launches a ne
-00003330: 7720 706f 6c6c 0a2d 2060 436f 6d6d 656e  w poll.- `Commen
-00003340: 7445 7665 6e74 6020 2d20 5472 6967 6765  tEvent` - Trigge
-00003350: 7265 6420 7768 656e 2061 2063 6f6d 6d65  red when a comme
-00003360: 6e74 2069 7320 7365 6e74 2069 6e20 7468  nt is sent in th
-00003370: 6520 7374 7265 616d 0a2d 2060 526f 6f6d  e stream.- `Room
-00003380: 4576 656e 7460 202d 204d 6573 7361 6765  Event` - Message
-00003390: 7320 6272 6f61 6463 6173 7465 6420 746f  s broadcasted to
-000033a0: 2061 6c6c 2075 7365 7273 2069 6e20 7468   all users in th
-000033b0: 6520 726f 6f6d 2028 652e 672e 2022 5765  e room (e.g. "We
-000033c0: 6c63 6f6d 6520 746f 2054 696b 546f 6b20  lcome to TikTok 
-000033d0: 4c49 5645 2122 290a 2d20 6045 6d6f 7465  LIVE!").- `Emote
-000033e0: 4368 6174 4576 656e 7460 202d 2054 7269  ChatEvent` - Tri
-000033f0: 6767 6572 6564 2077 6865 6e20 6120 6375  ggered when a cu
-00003400: 7374 6f6d 2065 6d6f 7465 2069 7320 7365  stom emote is se
-00003410: 6e74 2069 6e20 7468 6520 6368 6174 0a2d  nt in the chat.-
-00003420: 2060 456e 7665 6c6f 7065 4576 656e 7460   `EnvelopeEvent`
-00003430: 202d 2054 7269 6767 6572 6564 2065 7665   - Triggered eve
-00003440: 7279 2074 696d 6520 736f 6d65 6f6e 6520  ry time someone 
-00003450: 7365 6e64 7320 6120 7472 6561 7375 7265  sends a treasure
-00003460: 2063 6865 7374 0a2d 2060 536f 6369 616c   chest.- `Social
-00003470: 4576 656e 7460 202d 2054 7269 6767 6572  Event` - Trigger
-00003480: 6564 2077 6865 6e20 6120 7573 6572 2073  ed when a user s
-00003490: 6861 7265 7320 7468 6520 7374 7265 616d  hares the stream
-000034a0: 206f 7220 666f 6c6c 6f77 7320 7468 6520   or follows the 
-000034b0: 686f 7374 0a2d 2060 5175 6573 7469 6f6e  host.- `Question
-000034c0: 4e65 7745 7665 6e74 6020 2d20 5472 6967  NewEvent` - Trig
-000034d0: 6765 7265 6420 6576 6572 7920 7469 6d65  gered every time
-000034e0: 2073 6f6d 656f 6e65 2061 736b 7320 6120   someone asks a 
-000034f0: 6e65 7720 7175 6573 7469 6f6e 2076 6961  new question via
-00003500: 2074 6865 2071 7565 7374 696f 6e20 6665   the question fe
-00003510: 6174 7572 652e 0a2d 2060 4c69 7665 496e  ature..- `LiveIn
-00003520: 7472 6f45 7665 6e74 6020 2d20 5472 6967  troEvent` - Trig
-00003530: 6765 7265 6420 7768 656e 2061 206c 6976  gered when a liv
-00003540: 6520 696e 7472 6f20 6d65 7373 6167 6520  e intro message 
-00003550: 6170 7065 6172 730a 2d20 604c 696e 6b4d  appears.- `LinkM
-00003560: 6963 4172 6d69 6573 4576 656e 7460 202d  icArmiesEvent` -
-00003570: 2054 7269 6767 6572 6564 2077 6865 6e20   Triggered when 
-00003580: 6120 5469 6b54 6f6b 2062 6174 746c 6520  a TikTok battle 
-00003590: 7573 6572 2072 6563 6569 7665 7320 706f  user receives po
-000035a0: 696e 7473 0a2d 2060 4c69 6e6b 4d69 6342  ints.- `LinkMicB
-000035b0: 6174 746c 6545 7665 6e74 6020 2d20 5472  attleEvent` - Tr
-000035c0: 6967 6765 7265 6420 7768 656e 2061 2054  iggered when a T
-000035d0: 696b 546f 6b20 6261 7474 6c65 2069 7320  ikTok battle is 
-000035e0: 7374 6172 7465 640a 2d20 604a 6f69 6e45  started.- `JoinE
-000035f0: 7665 6e74 6020 2d20 5472 6967 6765 7265  vent` - Triggere
-00003600: 6420 7768 656e 2061 2075 7365 7220 6a6f  d when a user jo
-00003610: 696e 7320 7468 6520 6c69 7665 7374 7265  ins the livestre
-00003620: 616d 0a2d 2060 4c69 6e6b 4d69 6346 616e  am.- `LinkMicFan
-00003630: 5469 636b 6574 4d65 7468 6f64 4576 656e  TicketMethodEven
-00003640: 7460 0a2d 2060 4c69 6e6b 4d69 634d 6574  t`.- `LinkMicMet
-00003650: 686f 6445 7665 6e74 600a 2d20 6042 6172  hodEvent`.- `Bar
-00003660: 7261 6765 4576 656e 7460 0a2d 2060 4361  rageEvent`.- `Ca
-00003670: 7074 696f 6e45 7665 6e74 600a 2d20 6049  ptionEvent`.- `I
-00003680: 6d44 656c 6574 6545 7665 6e74 600a 2d20  mDeleteEvent`.- 
-00003690: 6052 6f6f 6d55 7365 7253 6571 4576 656e  `RoomUserSeqEven
-000036a0: 7460 202d 2043 7572 7265 6e74 2076 6965  t` - Current vie
-000036b0: 7765 7220 636f 756e 7420 696e 666f 726d  wer count inform
-000036c0: 6174 696f 6e0a 2d20 6052 616e 6b55 7064  ation.- `RankUpd
-000036d0: 6174 6545 7665 6e74 600a 2d20 6052 616e  ateEvent`.- `Ran
-000036e0: 6b54 6578 7445 7665 6e74 600a 2d20 6048  kTextEvent`.- `H
-000036f0: 6f75 726c 7952 616e 6b45 7665 6e74 600a  ourlyRankEvent`.
-00003700: 2d20 6055 6e61 7574 686f 7269 7a65 644d  - `UnauthorizedM
-00003710: 656d 6265 7245 7665 6e74 600a 2d20 604d  emberEvent`.- `M
-00003720: 6573 7361 6765 4465 7465 6374 4576 656e  essageDetectEven
-00003730: 7460 0a2d 2060 4f65 634c 6976 6553 686f  t`.- `OecLiveSho
-00003740: 7070 696e 6745 7665 6e74 600a 2d20 6052  ppingEvent`.- `R
-00003750: 6f6f 6d50 696e 4576 656e 7460 0a2d 2060  oomPinEvent`.- `
-00003760: 5379 7374 656d 4576 656e 7460 0a2d 2060  SystemEvent`.- `
-00003770: 4c69 6e6b 4576 656e 7460 0a2d 2060 4c69  LinkEvent`.- `Li
-00003780: 6e6b 4c61 7965 7245 7665 6e74 600a 0a23  nkLayerEvent`..#
-00003790: 2323 2053 7065 6369 616c 2045 7665 6e74  ## Special Event
-000037a0: 730a 0a23 2323 2060 4769 6674 4576 656e  s..### `GiftEven
-000037b0: 7460 0a0a 5472 6967 6765 7265 6420 6576  t`..Triggered ev
-000037c0: 6572 7920 7469 6d65 2061 2067 6966 7420  ery time a gift 
-000037d0: 6172 7269 7665 732e 2045 7874 7261 2069  arrives. Extra i
-000037e0: 6e66 6f72 6d61 7469 6f6e 2063 616e 2062  nformation can b
-000037f0: 6520 676c 6561 6d65 6420 6672 6f6d 2074  e gleamed from t
-00003800: 6865 2060 6176 6169 6c61 626c 655f 6769  he `available_gi
-00003810: 6674 7360 2063 6c69 656e 7420 6174 7472  fts` client attr
-00003820: 6962 7574 652e 0a3e 202a 2a4e 4f54 453a  ibute..> **NOTE:
-00003830: 2a2a 2055 7365 7273 2068 6176 6520 7468  ** Users have th
-00003840: 6520 6361 7061 6269 6c69 7479 2074 6f20  e capability to 
-00003850: 7365 6e64 2067 6966 7473 2069 6e20 6120  send gifts in a 
-00003860: 7374 7265 616b 2e20 5468 6973 2069 6e63  streak. This inc
-00003870: 7265 6173 6573 2074 6865 2060 6576 656e  reases the `even
-00003880: 742e 6769 6674 2e72 6570 6561 745f 636f  t.gift.repeat_co
-00003890: 756e 7460 2076 616c 7565 2075 6e74 696c  unt` value until
-000038a0: 2074 6865 0a3e 2075 7365 7220 7465 726d   the.> user term
-000038b0: 696e 6174 6573 2074 6865 2073 7472 6561  inates the strea
-000038c0: 6b2e 2044 7572 696e 6720 7468 6973 2074  k. During this t
-000038d0: 696d 6520 6e65 7720 6769 6674 2065 7665  ime new gift eve
-000038e0: 6e74 7320 6172 6520 7472 6967 6765 7265  nts are triggere
-000038f0: 6420 6167 6169 6e20 616e 6420 6167 6169  d again and agai
-00003900: 6e20 7769 7468 2061 6e0a 3e20 696e 6372  n with an.> incr
-00003910: 6561 7365 6420 6065 7665 6e74 2e67 6966  eased `event.gif
-00003920: 742e 7265 7065 6174 5f63 6f75 6e74 6020  t.repeat_count` 
-00003930: 7661 6c75 652e 2049 7420 7368 6f75 6c64  value. It should
-00003940: 2062 6520 6e6f 7465 6420 7468 6174 2061   be noted that a
-00003950: 6674 6572 2074 6865 2065 6e64 206f 6620  fter the end of 
-00003960: 6120 7374 7265 616b 2c20 6120 6669 6e61  a streak, a fina
-00003970: 6c20 6769 6674 2065 7665 6e74 2069 730a  l gift event is.
-00003980: 3e20 7472 6967 6765 7265 642c 2077 6869  > triggered, whi
-00003990: 6368 2073 6967 6e61 6c73 2074 6865 2065  ch signals the e
-000039a0: 6e64 206f 6620 7468 6520 7374 7265 616b  nd of the streak
-000039b0: 2077 6974 6820 6065 7665 6e74 2e72 6570   with `event.rep
-000039c0: 6561 745f 656e 6460 3a60 3160 2e20 5468  eat_end`:`1`. Th
-000039d0: 6520 666f 6c6c 6f77 696e 6720 6861 6e64  e following hand
-000039e0: 6c65 7273 2073 686f 7720 686f 7720 796f  lers show how yo
-000039f0: 7520 6361 6e20 6465 616c 2077 6974 6820  u can deal with 
-00003a00: 7468 6973 2069 6e20 796f 7572 2063 6f64  this in your cod
-00003a10: 652e 0a0a 5573 696e 6720 7468 6520 6c6f  e...Using the lo
-00003a20: 772d 6c65 7665 6c20 6469 7265 6374 2070  w-level direct p
-00003a30: 726f 746f 3a0a 6060 6070 7974 686f 6e0a  roto:.```python.
-00003a40: 4063 6c69 656e 742e 6f6e 2847 6966 7445  @client.on(GiftE
-00003a50: 7665 6e74 290a 6173 796e 6320 6465 6620  vent).async def 
-00003a60: 6f6e 5f67 6966 7428 6576 656e 743a 2047  on_gift(event: G
-00003a70: 6966 7445 7665 6e74 293a 0a20 2020 2023  iftEvent):.    #
-00003a80: 2049 6620 6974 2773 2074 7970 6520 3120   If it's type 1 
-00003a90: 616e 6420 7468 6520 7374 7265 616b 2069  and the streak i
-00003aa0: 7320 6f76 6572 0a20 2020 2069 6620 6576  s over.    if ev
-00003ab0: 656e 742e 6769 6674 2e69 6e66 6f2e 7479  ent.gift.info.ty
-00003ac0: 7065 203d 3d20 313a 0a20 2020 2020 2020  pe == 1:.       
-00003ad0: 2069 6620 6576 656e 742e 6769 6674 2e69   if event.gift.i
-00003ae0: 735f 7265 7065 6174 696e 6720 3d3d 2031  s_repeating == 1
-00003af0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00003b00: 696e 7428 6622 7b65 7665 6e74 2e75 7365  int(f"{event.use
-00003b10: 722e 756e 6971 7565 5f69 647d 2073 656e  r.unique_id} sen
-00003b20: 7420 7b65 7665 6e74 2e67 6966 742e 636f  t {event.gift.co
-00003b30: 756e 747d 7820 5c22 7b65 7665 6e74 2e67  unt}x \"{event.g
-00003b40: 6966 742e 696e 666f 2e6e 616d 657d 5c22  ift.info.name}\"
-00003b50: 2229 0a0a 2020 2020 2320 4974 2773 206e  ")..    # It's n
-00003b60: 6f74 2074 7970 6520 312c 2077 6869 6368  ot type 1, which
-00003b70: 206d 6561 6e73 2069 7420 6361 6e27 7420   means it can't 
-00003b80: 6861 7665 2061 2073 7472 6561 6b20 2620  have a streak & 
-00003b90: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
-00003ba0: 206f 7665 720a 2020 2020 656c 6966 2065   over.    elif e
-00003bb0: 7665 6e74 2e67 6966 742e 696e 666f 2e74  vent.gift.info.t
-00003bc0: 7970 6520 213d 2031 3a0a 2020 2020 2020  ype != 1:.      
-00003bd0: 2020 7072 696e 7428 6622 7b65 7665 6e74    print(f"{event
-00003be0: 2e75 7365 722e 756e 6971 7565 5f69 647d  .user.unique_id}
-00003bf0: 2073 656e 7420 5c22 7b65 7665 6e74 2e67   sent \"{event.g
-00003c00: 6966 742e 696e 666f 2e6e 616d 657d 5c22  ift.info.name}\"
-00003c10: 2229 0a60 6060 0a0a 5573 696e 6720 7468  ").```..Using th
-00003c20: 6520 5469 6b54 6f6b 4c69 7665 2065 7874  e TikTokLive ext
-00003c30: 656e 6465 6420 7072 6f74 6f3a 0a60 6060  ended proto:.```
-00003c40: 7079 7468 6f6e 0a40 636c 6965 6e74 2e6f  python.@client.o
-00003c50: 6e28 2267 6966 7422 290a 6173 796e 6320  n("gift").async 
-00003c60: 6465 6620 6f6e 5f67 6966 7428 6576 656e  def on_gift(even
-00003c70: 743a 2047 6966 7445 7665 6e74 293a 0a20  t: GiftEvent):. 
-00003c80: 2020 2023 2053 7472 6561 6b61 626c 6520     # Streakable 
-00003c90: 6769 6674 2026 2073 7472 6561 6b20 6973  gift & streak is
-00003ca0: 206f 7665 720a 2020 2020 6966 2065 7665   over.    if eve
-00003cb0: 6e74 2e67 6966 742e 7374 7265 616b 6162  nt.gift.streakab
-00003cc0: 6c65 2061 6e64 206e 6f74 2065 7665 6e74  le and not event
-00003cd0: 2e73 7472 6561 6b69 6e67 3a0a 2020 2020  .streaking:.    
-00003ce0: 2020 2020 7072 696e 7428 6622 7b65 7665      print(f"{eve
-00003cf0: 6e74 2e75 7365 722e 756e 6971 7565 5f69  nt.user.unique_i
-00003d00: 647d 2073 656e 7420 7b65 7665 6e74 2e67  d} sent {event.g
-00003d10: 6966 742e 636f 756e 747d 7820 5c22 7b65  ift.count}x \"{e
-00003d20: 7665 6e74 2e67 6966 742e 696e 666f 2e6e  vent.gift.info.n
-00003d30: 616d 657d 5c22 2229 0a0a 2020 2020 2320  ame}\"")..    # 
-00003d40: 4e6f 6e2d 7374 7265 616b 6162 6c65 2067  Non-streakable g
-00003d50: 6966 740a 2020 2020 656c 6966 206e 6f74  ift.    elif not
-00003d60: 2065 7665 6e74 2e67 6966 742e 7374 7265   event.gift.stre
-00003d70: 616b 6162 6c65 3a0a 2020 2020 2020 2020  akable:.        
-00003d80: 7072 696e 7428 6622 7b65 7665 6e74 2e75  print(f"{event.u
-00003d90: 7365 722e 756e 6971 7565 5f69 647d 2073  ser.unique_id} s
-00003da0: 656e 7420 5c22 7b65 7665 6e74 2e67 6966  ent \"{event.gif
-00003db0: 742e 696e 666f 2e6e 616d 657d 5c22 2229  t.info.name}\"")
-00003dc0: 0a0a 6060 600a 0a23 2323 2060 5375 6273  ..```..### `Subs
-00003dd0: 6372 6962 6545 7665 6e74 600a 0a54 6869  cribeEvent`..Thi
-00003de0: 7320 6576 656e 7420 7769 6c6c 206f 6e6c  s event will onl
-00003df0: 7920 6669 7265 2077 6865 6e20 6120 7365  y fire when a se
-00003e00: 7373 696f 6e20 4944 2028 6163 636f 756e  ssion ID (accoun
-00003e10: 7420 6c6f 6769 6e29 2069 7320 7061 7373  t login) is pass
-00003e20: 6564 2074 6f20 7468 6520 4854 5450 2063  ed to the HTTP c
-00003e30: 6c69 656e 7420 2a62 6566 6f72 652a 2063  lient *before* c
-00003e40: 6f6e 6e65 6374 696e 6720 746f 2054 696b  onnecting to Tik
-00003e50: 546f 6b20 4c49 5645 2e0a 596f 7520 6361  Tok LIVE..You ca
-00003e60: 6e20 7365 7420 7468 6520 7365 7373 696f  n set the sessio
-00003e70: 6e20 4944 2077 6974 6820 5b60 636c 6965  n ID with [`clie
-00003e80: 6e74 2e77 6562 2e73 6574 5f73 6573 7369  nt.web.set_sessi
-00003e90: 6f6e 5f69 6428 2e2e 2e29 605d 2868 7474  on_id(...)`](htt
-00003ea0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003eb0: 6973 6161 636b 6f67 616e 2f54 696b 546f  isaackogan/TikTo
-00003ec0: 6b4c 6976 652f 626c 6f62 2f6d 6173 7465  kLive/blob/maste
-00003ed0: 722f 6578 616d 706c 6573 2f6c 6f67 6765  r/examples/logge
-00003ee0: 645f 696e 2e70 7929 2e0a 0a23 2320 4368  d_in.py)...## Ch
-00003ef0: 6563 6b69 6e67 2049 6620 4120 5573 6572  ecking If A User
-00003f00: 2049 7320 4c69 7665 0a0a 4974 2069 7320   Is Live..It is 
-00003f10: 636f 6e73 6964 6572 6564 2069 6e65 6666  considered ineff
-00003f20: 6963 6965 6e74 2074 6f20 7573 6520 7468  icient to use th
-00003f30: 6520 636f 6e6e 6563 7420 6d65 7468 6f64  e connect method
-00003f40: 2074 6f20 6368 6563 6b20 6966 2061 2075   to check if a u
-00003f50: 7365 7220 6973 206c 6976 652e 2049 7420  ser is live. It 
-00003f60: 6973 2062 6574 7465 7220 746f 2075 7365  is better to use
-00003f70: 2074 6865 2064 6564 6963 6174 6564 2060   the dedicated `
-00003f80: 6177 6169 7420 636c 6965 6e74 2e69 735f  await client.is_
-00003f90: 6c69 7665 2829 6020 6d65 7468 6f64 2e20  live()` method. 
-00003fa0: 0a0a 5468 6572 6520 6973 2061 205b 636f  ..There is a [co
-00003fb0: 6d70 6c65 7465 2065 7861 6d70 6c65 5d28  mplete example](
-00003fc0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00003fd0: 6f6d 2f69 7361 6163 6b6f 6761 6e2f 5469  om/isaackogan/Ti
-00003fe0: 6b54 6f6b 4c69 7665 2f62 6c6f 622f 6d61  kTokLive/blob/ma
-00003ff0: 7374 6572 2f65 7861 6d70 6c65 732f 6368  ster/examples/ch
-00004000: 6563 6b5f 6c69 7665 2e70 7929 206f 6620  eck_live.py) of 
-00004010: 686f 7720 746f 2064 6f20 7468 6973 2069  how to do this i
-00004020: 6e20 7468 6520 5b65 7861 6d70 6c65 735d  n the [examples]
-00004030: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00004040: 636f 6d2f 6973 6161 636b 6f67 616e 2f54  com/isaackogan/T
-00004050: 696b 546f 6b4c 6976 652f 7472 6565 2f6d  ikTokLive/tree/m
-00004060: 6173 7465 722f 6578 616d 706c 6573 2920  aster/examples) 
-00004070: 666f 6c64 6572 2e0a 0a23 2320 436f 6e74  folder...## Cont
-00004080: 7269 6275 746f 7273 0a0a 2a20 2a2a 4973  ributors..* **Is
-00004090: 6161 6320 4b6f 6761 6e2a 2a20 2d20 2a43  aac Kogan** - *C
-000040a0: 7265 6174 6f72 2c20 5072 696d 6172 7920  reator, Primary 
-000040b0: 4d61 696e 7461 696e 6572 2c20 616e 6420  Maintainer, and 
-000040c0: 5265 7665 7273 652d 456e 6769 6e65 6572  Reverse-Engineer
-000040d0: 696e 672a 202d 205b 6973 6161 636b 6f67  ing* - [isaackog
-000040e0: 616e 5d28 6874 7470 733a 2f2f 6769 7468  an](https://gith
-000040f0: 7562 2e63 6f6d 2f69 7361 6163 6b6f 6761  ub.com/isaackoga
-00004100: 6e29 0a2a 202a 2a5a 6572 6f64 792a 2a20  n).* **Zerody** 
-00004110: 2d20 2a49 6e69 7469 616c 2052 6576 6572  - *Initial Rever
-00004120: 7365 2d45 6e67 696e 6565 7269 6e67 2050  se-Engineering P
-00004130: 726f 746f 6275 6620 2620 5375 7070 6f72  rotobuf & Suppor
-00004140: 742a 202d 205b 5a65 726f 6479 5d28 6874  t* - [Zerody](ht
-00004150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00004160: 2f7a 6572 6f64 7974 7261 7368 2f29 0a2a  /zerodytrash/).*
-00004170: 202a 2a44 6176 696e 6369 626c 652a 2a20   **Davincible** 
-00004180: 2d20 2a52 6576 6572 7365 2d45 6e67 696e  - *Reverse-Engin
-00004190: 6565 7269 6e67 2053 7472 6561 6d20 446f  eering Stream Do
-000041a0: 776e 6c6f 6164 732a 2020 2d20 5b64 6176  wnloads*  - [dav
-000041b0: 696e 6369 626c 655d 2868 7474 7073 3a2f  incible](https:/
-000041c0: 2f67 6974 6875 622e 636f 6d2f 6461 7669  /github.com/davi
-000041d0: 6e63 6962 6c65 290a 0a53 6565 2061 6c73  ncible)..See als
-000041e0: 6f20 7468 6520 6675 6c6c 206c 6973 7420  o the full list 
-000041f0: 6f66 205b 636f 6e74 7269 6275 746f 7273  of [contributors
-00004200: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004210: 2e63 6f6d 2f69 7361 6163 6b6f 6761 6e2f  .com/isaackogan/
-00004220: 5469 6b54 6f6b 4c69 7665 2f63 6f6e 7472  TikTokLive/contr
-00004230: 6962 7574 6f72 7329 2077 686f 2068 6176  ibutors) who hav
-00004240: 6520 7061 7274 6963 6970 6174 6564 2069  e participated i
-00004250: 6e0a 7468 6973 2070 726f 6a65 6374 2e0a  n.this project..
-00004260: 0a23 2320 4c69 6365 6e73 650a 0a54 6869  .## License..Thi
-00004270: 7320 7072 6f6a 6563 7420 6973 206c 6963  s project is lic
-00004280: 656e 7365 6420 756e 6465 7220 7468 6520  ensed under the 
-00004290: 4d49 5420 4c69 6365 6e73 6520 2d20 7365  MIT License - se
-000042a0: 6520 7468 6520 5b4c 4943 454e 5345 5d28  e the [LICENSE](
-000042b0: 4c49 4345 4e53 4529 2066 696c 6520 666f  LICENSE) file fo
-000042c0: 7220 6465 7461 696c 732e 0a              r details..
+00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002240: 2020 2020 2020 207c 0a7c 2d2d 2d2d 2d2d         |.|------
+00002250: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
+00002260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022f0: 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 726f 6f6d  --------|.| room
+00002300: 5f69 6420 2020 2020 2020 207c 2054 6865  _id        | The
+00002310: 2052 6f6f 6d20 4944 206f 6620 7468 6520   Room ID of the 
+00002320: 6c69 7665 7374 7265 616d 2072 6f6f 6d20  livestream room 
+00002330: 7468 6520 636c 6965 6e74 2069 7320 6375  the client is cu
+00002340: 7272 656e 746c 7920 636f 6e6e 6563 7465  rrently connecte
+00002350: 6420 746f 2e20 2020 2020 2020 2020 2020  d to.           
+00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2020 2020 2020 2020 207c 0a7c 2077 6562           |.| web
+000023b0: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
+000023c0: 6520 5469 6b54 6f6b 2048 5454 5020 636c  e TikTok HTTP cl
+000023d0: 6965 6e74 2e20 5468 6973 2063 6c69 656e  ient. This clien
+000023e0: 7420 6861 7320 6120 6c6f 7420 6f66 2075  t has a lot of u
+000023f0: 7365 6675 6c20 726f 7574 6573 2079 6f75  seful routes you
+00002400: 2073 686f 756c 6420 6578 706c 6f72 6521   should explore!
+00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002450: 2020 2020 2020 2020 2020 7c0a 7c20 636f            |.| co
+00002460: 6e6e 6563 7465 6420 2020 2020 207c 2057  nnected      | W
+00002470: 6865 7468 6572 2079 6f75 2061 7265 2063  hether you are c
+00002480: 7572 7265 6e74 6c79 2063 6f6e 6e65 6374  urrently connect
+00002490: 6564 2074 6f20 7468 6520 6c69 7665 7374  ed to the livest
+000024a0: 7265 616d 2e20 2020 2020 2020 2020 2020  ream.           
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002500: 2020 2020 2020 2020 2020 207c 0a7c 206c             |.| l
+00002510: 6f67 6765 7220 2020 2020 2020 2020 7c20  ogger         | 
+00002520: 5468 6520 696e 7465 726e 616c 206c 6f67  The internal log
+00002530: 6765 7220 7573 6564 2062 7920 5469 6b54  ger used by TikT
+00002540: 6f6b 4c69 7665 2e20 596f 7520 6361 6e20  okLive. You can 
+00002550: 7573 6520 6063 6c69 656e 742e 6c6f 6767  use `client.logg
+00002560: 6572 2e73 6574 4c65 7665 6c28 2e2e 2e29  er.setLevel(...)
+00002570: 6020 6d65 7468 6f64 2074 6f20 656e 6162  ` method to enab
+00002580: 6c65 2063 6c69 656e 7420 6465 6275 672e  le client debug.
+00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+000025c0: 726f 6f6d 5f69 6e66 6f20 2020 2020 207c  room_info      |
+000025d0: 2052 6f6f 6d20 696e 666f 726d 6174 696f   Room informatio
+000025e0: 6e20 7468 6174 2069 7320 7265 7472 6965  n that is retrie
+000025f0: 7665 6420 6672 6f6d 2054 696b 546f 6b20  ved from TikTok 
+00002600: 7768 656e 2079 6f75 2075 7365 2061 2063  when you use a c
+00002610: 6f6e 6e65 6374 696f 6e20 6d65 7468 6f64  onnection method
+00002620: 2028 652e 672e 2060 636c 6965 6e74 2e63   (e.g. `client.c
+00002630: 6f6e 6e65 6374 6029 2077 6974 6820 7468  onnect`) with th
+00002640: 6520 6b65 7977 6f72 6420 6172 6775 6d65  e keyword argume
+00002650: 6e74 2060 6665 7463 685f 726f 6f6d 5f69  nt `fetch_room_i
+00002660: 6e66 6f3d 5472 7565 6020 2e20 207c 0a7c  nfo=True` .  |.|
+00002670: 2067 6966 745f 696e 666f 2020 2020 2020   gift_info      
+00002680: 7c20 4578 7472 6120 6769 6674 2069 6e66  | Extra gift inf
+00002690: 6f72 6d61 7469 6f6e 2074 6861 7420 6973  ormation that is
+000026a0: 2072 6574 7269 6576 6564 2066 726f 6d20   retrieved from 
+000026b0: 5469 6b54 6f6b 2077 6865 6e20 796f 7520  TikTok when you 
+000026c0: 7573 6520 6120 636f 6e6e 6563 7469 6f6e  use a connection
+000026d0: 206d 6574 686f 6420 2865 2e67 2e20 6063   method (e.g. `c
+000026e0: 6c69 656e 742e 7275 6e60 2920 7769 7468  lient.run`) with
+000026f0: 2074 6865 206b 6579 776f 7264 2061 7267   the keyword arg
+00002700: 756d 656e 7420 6066 6574 6368 5f67 6966  ument `fetch_gif
+00002710: 745f 696e 666f 3d54 7275 6560 2e20 7c0a  t_info=True`. |.
+00002720: 0a0a 2323 2057 6562 4465 6661 756c 7473  ..## WebDefaults
+00002730: 0a0a 5469 6b54 6f6b 4c69 7665 2068 6173  ..TikTokLive has
+00002740: 2061 2073 6572 6965 7320 6f66 2067 6c6f   a series of glo
+00002750: 6261 6c20 6465 6661 756c 7473 2075 7365  bal defaults use
+00002760: 6420 746f 2063 7265 6174 6520 7468 6520  d to create the 
+00002770: 4854 5450 2063 6c69 656e 7420 7768 6963  HTTP client whic
+00002780: 6820 796f 7520 6361 6e20 6375 7374 6f6d  h you can custom
+00002790: 697a 652e 2046 6f72 2069 6e66 6f20 6f6e  ize. For info on
+000027a0: 2068 6f77 2074 6f20 7365 7420 7468 6573   how to set thes
+000027b0: 6520 7061 7261 6d65 7465 7273 2c20 7365  e parameters, se
+000027c0: 650a 7468 6520 5b77 6562 5f64 6566 6175  e.the [web_defau
+000027d0: 6c74 732e 7079 5d28 6874 7470 733a 2f2f  lts.py](https://
+000027e0: 6769 7468 7562 2e63 6f6d 2f69 7361 6163  github.com/isaac
+000027f0: 6b6f 6761 6e2f 5469 6b54 6f6b 4c69 7665  kogan/TikTokLive
+00002800: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
+00002810: 6d70 6c65 732f 7765 625f 6465 6661 756c  mples/web_defaul
+00002820: 7473 2e70 7929 2065 7861 6d70 6c65 2e0a  ts.py) example..
+00002830: 0a7c 2050 6172 616d 6574 6572 2020 2020  .| Parameter    
+00002840: 2020 2020 2020 207c 2054 7970 6520 2020         | Type   
+00002850: 7c20 4465 7363 7269 7074 696f 6e20 2020  | Description   
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000028e0: 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|--------------
+000028f0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+00002900: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00002910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00002990: 0a7c 2074 696b 746f 6b5f 6170 705f 7572  .| tiktok_app_ur
+000029a0: 6c20 2020 2020 207c 2060 7374 7260 2020  l      | `str`  
+000029b0: 7c20 5468 6520 5469 6b54 6f6b 2061 7070  | The TikTok app
+000029c0: 2055 524c 2028 6068 7474 7073 3a2f 2f77   URL (`https://w
+000029d0: 7777 2e74 696b 746f 6b2e 636f 6d60 2920  ww.tiktok.com`) 
+000029e0: 7573 6564 2074 6f20 7363 7261 7065 2074  used to scrape t
+000029f0: 6865 2072 6f6f 6d2e 2020 2020 2020 2020  he room.        
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002a40: 0a7c 2074 696b 746f 6b5f 7369 676e 5f75  .| tiktok_sign_u
+00002a50: 726c 2020 2020 207c 2060 7374 7260 2020  rl     | `str`  
+00002a60: 7c20 5468 6520 5b73 6967 6e61 7475 7265  | The [signature
+00002a70: 2073 6572 7665 725d 2868 7474 7073 3a2f   server](https:/
+00002a80: 2f67 6974 6875 622e 636f 6d2f 6973 6161  /github.com/isaa
+00002a90: 636b 6f67 616e 2f54 696b 546f 6b4c 6976  ckogan/TikTokLiv
+00002aa0: 652f 7769 6b69 2f41 6c6c 2d41 626f 7574  e/wiki/All-About
+00002ab0: 2d53 6967 6e61 7475 7265 7329 2075 7365  -Signatures) use
+00002ac0: 6420 746f 2067 656e 6572 6174 6520 746f  d to generate to
+00002ad0: 6b65 6e73 2074 6f20 636f 6e6e 6563 7420  kens to connect 
+00002ae0: 746f 2054 696b 546f 6b4c 6976 652e 207c  to TikTokLive. |
+00002af0: 0a7c 2074 696b 746f 6b5f 7765 6263 6173  .| tiktok_webcas
+00002b00: 745f 7572 6c20 207c 2060 7374 7260 2020  t_url  | `str`  
+00002b10: 7c20 5468 6520 5469 6b54 6f6b 206c 6976  | The TikTok liv
+00002b20: 6573 7472 6561 6d20 5552 4c20 2860 6874  estream URL (`ht
+00002b30: 7470 733a 2f2f 7765 6263 6173 742e 7469  tps://webcast.ti
+00002b40: 6b74 6f6b 2e63 6f6d 6029 2077 6865 7265  ktok.com`) where
+00002b50: 206c 6976 6573 7472 6561 6d73 2063 616e   livestreams can
+00002b60: 2062 6520 6163 6365 7373 6564 2066 726f   be accessed fro
+00002b70: 6d2e 2020 2020 2020 2020 2020 2020 2020  m.              
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002ba0: 0a7c 2063 6c69 656e 745f 7061 7261 6d73  .| client_params
+00002bb0: 2020 2020 2020 207c 2060 6469 6374 6020         | `dict` 
+00002bc0: 7c20 5468 6520 5552 4c20 7061 7261 6d65  | The URL parame
+00002bd0: 7465 7273 2061 6464 6564 206f 6e20 746f  ters added on to
+00002be0: 2054 696b 546f 6b20 7265 7175 6573 7473   TikTok requests
+00002bf0: 2066 726f 6d20 7468 6520 4854 5450 2063   from the HTTP c
+00002c00: 6c69 656e 742e 2020 2020 2020 2020 2020  lient.          
+00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c40: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002c50: 0a7c 2063 6c69 656e 745f 6865 6164 6572  .| client_header
+00002c60: 7320 2020 2020 207c 2060 6469 6374 6020  s      | `dict` 
+00002c70: 7c20 5468 6520 6865 6164 6572 7320 6164  | The headers ad
+00002c80: 6465 6420 6f6e 2074 6f20 5469 6b54 6f6b  ded on to TikTok
+00002c90: 2072 6571 7565 7374 7320 6672 6f6d 2074   requests from t
+00002ca0: 6865 2048 5454 5020 636c 6965 6e74 2e20  he HTTP client. 
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002d00: 0a7c 2074 696b 746f 6b5f 7369 676e 5f61  .| tiktok_sign_a
+00002d10: 7069 5f6b 6579 207c 2060 7374 7260 2020  pi_key | `str`  
+00002d20: 7c20 4120 676c 6f62 616c 2077 6179 206f  | A global way o
+00002d30: 6620 7365 7474 696e 6720 7468 6520 6073  f setting the `s
+00002d40: 6967 6e5f 6170 695f 6b65 7960 2070 6172  ign_api_key` par
+00002d50: 616d 6574 6572 2e20 2020 2020 2020 2020  ameter.         
+00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002da0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002db0: 0a0a 2323 2045 7665 6e74 730a 0a45 7665  ..## Events..Eve
+00002dc0: 6e74 7320 6361 6e20 6265 206c 6973 7465  nts can be liste
+00002dd0: 6e65 6420 746f 2075 7369 6e67 2061 2064  ned to using a d
+00002de0: 6563 6f72 6174 6f72 206f 7220 6e6f 6e2d  ecorator or non-
+00002df0: 6465 636f 7261 746f 7220 6d65 7468 6f64  decorator method
+00002e00: 2063 616c 6c2e 2054 6865 2066 6f6c 6c6f   call. The follo
+00002e10: 7769 6e67 2065 7861 6d70 6c65 7320 696c  wing examples il
+00002e20: 6c75 7374 7261 7465 2068 6f77 2079 6f75  lustrate how you
+00002e30: 2063 616e 206c 6973 7465 6e20 746f 2061   can listen to a
+00002e40: 6e20 6576 656e 743a 0a0a 6060 6070 7974  n event:..```pyt
+00002e50: 686f 6e0a 4063 6c69 656e 742e 6f6e 284c  hon.@client.on(L
+00002e60: 696b 6545 7665 6e74 290a 6173 796e 6320  ikeEvent).async 
+00002e70: 6465 6620 6f6e 5f6c 696b 6528 6576 656e  def on_like(even
+00002e80: 743a 204c 696b 6545 7665 6e74 2920 2d3e  t: LikeEvent) ->
+00002e90: 204e 6f6e 653a 0a20 2020 202e 2e2e 0a0a   None:.    .....
+00002ea0: 6173 796e 6320 6465 6620 6f6e 5f63 6f6d  async def on_com
+00002eb0: 6d65 6e74 2865 7665 6e74 3a20 436f 6d6d  ment(event: Comm
+00002ec0: 656e 7445 7665 6e74 2920 2d3e 204e 6f6e  entEvent) -> Non
+00002ed0: 653a 0a20 2020 202e 2e2e 0a0a 636c 6965  e:.    .....clie
+00002ee0: 6e74 2e61 6464 5f6c 6973 7465 6e65 7228  nt.add_listener(
+00002ef0: 436f 6d6d 656e 7445 7665 6e74 2c20 6f6e  CommentEvent, on
+00002f00: 5f63 6f6d 6d65 6e74 290a 6060 600a 0a54  _comment).```..T
+00002f10: 6865 7265 2061 7265 2074 776f 2074 7970  here are two typ
+00002f20: 6573 206f 6620 6576 656e 7473 2c20 5b60  es of events, [`
+00002f30: 4375 7374 6f6d 4576 656e 7460 5d28 6874  CustomEvent`](ht
+00002f40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002f50: 2f69 7361 6163 6b6f 6761 6e2f 5469 6b54  /isaackogan/TikT
+00002f60: 6f6b 4c69 7665 2f62 6c6f 622f 6d61 7374  okLive/blob/mast
+00002f70: 6572 2f54 696b 546f 6b4c 6976 652f 6576  er/TikTokLive/ev
+00002f80: 656e 7473 2f63 7573 746f 6d5f 6576 656e  ents/custom_even
+00002f90: 7473 2e70 7929 200a 6576 656e 7473 2061  ts.py) .events a
+00002fa0: 6e64 205b 6050 726f 746f 4576 656e 7460  nd [`ProtoEvent`
+00002fb0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002fc0: 2e63 6f6d 2f69 7361 6163 6b6f 6761 6e2f  .com/isaackogan/
+00002fd0: 5469 6b54 6f6b 4c69 7665 2f62 6c6f 622f  TikTokLive/blob/
+00002fe0: 6d61 7374 6572 2f54 696b 546f 6b4c 6976  master/TikTokLiv
+00002ff0: 652f 6576 656e 7473 2f70 726f 746f 5f65  e/events/proto_e
+00003000: 7665 6e74 732e 7079 2920 6576 656e 7473  vents.py) events
+00003010: 2e0a 426f 7468 2062 656c 6f6e 6720 746f  ..Both belong to
+00003020: 2074 6865 2054 696b 546f 6b4c 6976 6520   the TikTokLive 
+00003030: 6045 7665 6e74 6020 7479 7065 2061 6e64  `Event` type and
+00003040: 2063 616e 2062 6520 6c69 7374 656e 6564   can be listened
+00003050: 2074 6f2e 2054 6865 2066 6f6c 6c6f 7769   to. The followi
+00003060: 6e67 2065 7665 6e74 7320 6172 6520 6176  ng events are av
+00003070: 6169 6c61 626c 653a 0a0a 2323 2320 4375  ailable:..### Cu
+00003080: 7374 6f6d 2045 7665 6e74 730a 0a2d 2060  stom Events..- `
+00003090: 436f 6e6e 6563 7445 7665 6e74 6020 2d20  ConnectEvent` - 
+000030a0: 5472 6967 6765 7265 6420 7768 656e 2074  Triggered when t
+000030b0: 6865 2057 6562 6361 7374 2063 6f6e 6e65  he Webcast conne
+000030c0: 6374 696f 6e20 6973 2069 6e69 7469 6174  ction is initiat
+000030d0: 6564 0a2d 2060 4469 7363 6f6e 6e65 6374  ed.- `Disconnect
+000030e0: 4576 656e 7460 202d 2054 7269 6767 6572  Event` - Trigger
+000030f0: 6564 2077 6865 6e20 7468 6520 5765 6263  ed when the Webc
+00003100: 6173 7420 636f 6e6e 6563 7469 6f6e 2063  ast connection c
+00003110: 6c6f 7365 7320 2869 6e63 6c75 6469 6e67  loses (including
+00003120: 2074 6865 206c 6976 6573 7472 6561 6d20   the livestream 
+00003130: 656e 6469 6e67 290a 2d20 604c 6976 6545  ending).- `LiveE
+00003140: 6e64 4576 656e 7460 202d 2054 7269 6767  ndEvent` - Trigg
+00003150: 6572 6564 2077 6865 6e20 7468 6520 6c69  ered when the li
+00003160: 7665 7374 7265 616d 2065 6e64 730a 2d20  vestream ends.- 
+00003170: 604c 6976 6550 6175 7365 4576 656e 7460  `LivePauseEvent`
+00003180: 202d 2054 7269 6767 6572 6564 2077 6865   - Triggered whe
+00003190: 6e20 7468 6520 6c69 7665 7374 7265 616d  n the livestream
+000031a0: 2069 7320 7061 7573 6564 0a2d 2060 4c69   is paused.- `Li
+000031b0: 7665 556e 7061 7573 6545 7665 6e74 6020  veUnpauseEvent` 
+000031c0: 2d20 5472 6967 6765 7265 6420 7768 656e  - Triggered when
+000031d0: 2074 6865 206c 6976 6573 7472 6561 6d20   the livestream 
+000031e0: 6973 2075 6e70 6175 7365 640a 2d20 6046  is unpaused.- `F
+000031f0: 6f6c 6c6f 7745 7665 6e74 6020 2d20 5472  ollowEvent` - Tr
+00003200: 6967 6765 7265 6420 7768 656e 2061 2075  iggered when a u
+00003210: 7365 7220 696e 2074 6865 206c 6976 6573  ser in the lives
+00003220: 7472 6561 6d20 666f 6c6c 6f77 7320 7468  tream follows th
+00003230: 6520 7374 7265 616d 6572 0a2d 2060 5368  e streamer.- `Sh
+00003240: 6172 6545 7665 6e74 6020 2d20 5472 6967  areEvent` - Trig
+00003250: 6765 7265 6420 7768 656e 2061 2075 7365  gered when a use
+00003260: 7220 7368 6172 6573 2074 6865 206c 6976  r shares the liv
+00003270: 6573 7472 6561 6d0a 2d20 6057 6562 736f  estream.- `Webso
+00003280: 636b 6574 5265 7370 6f6e 7365 4576 656e  cketResponseEven
+00003290: 7460 202d 2054 7269 6767 6572 6564 2077  t` - Triggered w
+000032a0: 6865 6e20 616e 7920 6576 656e 7420 6973  hen any event is
+000032b0: 2072 6563 6569 7665 6420 2863 6f6e 7461   received (conta
+000032c0: 696e 7320 7468 6520 6576 656e 7429 0a2d  ins the event).-
+000032d0: 2060 556e 6b6e 6f77 6e45 7665 6e74 6020   `UnknownEvent` 
+000032e0: 2d20 416e 2069 6e73 7461 6e63 6520 6f66  - An instance of
+000032f0: 2060 5765 6273 6f63 6b65 7452 6573 706f   `WebsocketRespo
+00003300: 6e73 6545 7665 6e74 6020 7468 726f 776e  nseEvent` thrown
+00003310: 2077 6865 6e65 7665 7220 616e 2065 7665   whenever an eve
+00003320: 6e74 2064 6f65 7320 6e6f 7420 6861 7665  nt does not have
+00003330: 2061 6e20 6578 6973 7469 6e67 2064 6566   an existing def
+00003340: 696e 6974 696f 6e2c 2075 7365 6675 6c20  inition, useful 
+00003350: 666f 7220 6465 6275 6767 696e 670a 0a23  for debugging..#
+00003360: 2323 2050 726f 746f 2045 7665 6e74 730a  ## Proto Events.
+00003370: 0a49 6620 796f 7520 6b6e 6f77 2077 6861  .If you know wha
+00003380: 7420 616e 2065 7665 6e74 2064 6f65 732c  t an event does,
+00003390: 205b 6d61 6b65 2061 2070 756c 6c20 7265   [make a pull re
+000033a0: 7175 6573 745d 2868 7474 7073 3a2f 2f67  quest](https://g
+000033b0: 6974 6875 622e 636f 6d2f 6973 6161 636b  ithub.com/isaack
+000033c0: 6f67 616e 2f54 696b 546f 6b4c 6976 652f  ogan/TikTokLive/
+000033d0: 7075 6c6c 7329 2061 6e64 2061 6464 2074  pulls) and add t
+000033e0: 6865 2064 6573 6372 6970 7469 6f6e 2e20  he description. 
+000033f0: 0a0a 2d20 6047 6966 7445 7665 6e74 6020  ..- `GiftEvent` 
+00003400: 2d20 5472 6967 6765 7265 6420 7768 656e  - Triggered when
+00003410: 2061 2067 6966 7420 6973 2073 656e 7420   a gift is sent 
+00003420: 746f 2074 6865 2073 7472 6561 6d65 720a  to the streamer.
+00003430: 2d20 6047 6f61 6c55 7064 6174 6545 7665  - `GoalUpdateEve
+00003440: 6e74 6020 2d20 5472 6967 6765 7265 6420  nt` - Triggered 
+00003450: 7768 656e 2074 6865 2073 7562 7363 7269  when the subscri
+00003460: 6265 7220 676f 616c 2069 7320 7570 6461  ber goal is upda
+00003470: 7465 640a 2d20 6043 6f6e 7472 6f6c 4576  ted.- `ControlEv
+00003480: 656e 7460 202d 2054 7269 6767 6572 6564  ent` - Triggered
+00003490: 2077 6865 6e20 6120 7374 7265 616d 2061   when a stream a
+000034a0: 6374 696f 6e20 6f63 6375 7273 2028 652e  ction occurs (e.
+000034b0: 672e 204c 6976 6573 7472 6561 6d20 7374  g. Livestream st
+000034c0: 6172 742c 2065 6e64 290a 2d20 604c 696b  art, end).- `Lik
+000034d0: 6545 7665 6e74 6020 2d20 5472 6967 6765  eEvent` - Trigge
+000034e0: 7265 6420 7768 656e 2074 6865 2073 7472  red when the str
+000034f0: 6561 6d20 7265 6365 6976 6573 2061 206c  eam receives a l
+00003500: 696b 650a 2d20 6053 7562 7363 7269 6265  ike.- `Subscribe
+00003510: 4576 656e 7460 202d 2054 7269 6767 6572  Event` - Trigger
+00003520: 6564 2077 6865 6e20 736f 6d65 6f6e 6520  ed when someone 
+00003530: 7375 6273 6372 6962 6573 2074 6f20 7468  subscribes to th
+00003540: 6520 5469 6b54 6f6b 2063 7265 6174 6f72  e TikTok creator
+00003550: 0a2d 2060 506f 6c6c 4576 656e 7460 202d  .- `PollEvent` -
+00003560: 2054 7269 6767 6572 6564 2077 6865 6e20   Triggered when 
+00003570: 7468 6520 6372 6561 746f 7220 6c61 756e  the creator laun
+00003580: 6368 6573 2061 206e 6577 2070 6f6c 6c0a  ches a new poll.
+00003590: 2d20 6043 6f6d 6d65 6e74 4576 656e 7460  - `CommentEvent`
+000035a0: 202d 2054 7269 6767 6572 6564 2077 6865   - Triggered whe
+000035b0: 6e20 6120 636f 6d6d 656e 7420 6973 2073  n a comment is s
+000035c0: 656e 7420 696e 2074 6865 2073 7472 6561  ent in the strea
+000035d0: 6d0a 2d20 6052 6f6f 6d45 7665 6e74 6020  m.- `RoomEvent` 
+000035e0: 2d20 4d65 7373 6167 6573 2062 726f 6164  - Messages broad
+000035f0: 6361 7374 6564 2074 6f20 616c 6c20 7573  casted to all us
+00003600: 6572 7320 696e 2074 6865 2072 6f6f 6d20  ers in the room 
+00003610: 2865 2e67 2e20 2257 656c 636f 6d65 2074  (e.g. "Welcome t
+00003620: 6f20 5469 6b54 6f6b 204c 4956 4521 2229  o TikTok LIVE!")
+00003630: 0a2d 2060 456d 6f74 6543 6861 7445 7665  .- `EmoteChatEve
+00003640: 6e74 6020 2d20 5472 6967 6765 7265 6420  nt` - Triggered 
+00003650: 7768 656e 2061 2063 7573 746f 6d20 656d  when a custom em
+00003660: 6f74 6520 6973 2073 656e 7420 696e 2074  ote is sent in t
+00003670: 6865 2063 6861 740a 2d20 6045 6e76 656c  he chat.- `Envel
+00003680: 6f70 6545 7665 6e74 6020 2d20 5472 6967  opeEvent` - Trig
+00003690: 6765 7265 6420 6576 6572 7920 7469 6d65  gered every time
+000036a0: 2073 6f6d 656f 6e65 2073 656e 6473 2061   someone sends a
+000036b0: 2074 7265 6173 7572 6520 6368 6573 740a   treasure chest.
+000036c0: 2d20 6053 6f63 6961 6c45 7665 6e74 6020  - `SocialEvent` 
+000036d0: 2d20 5472 6967 6765 7265 6420 7768 656e  - Triggered when
+000036e0: 2061 2075 7365 7220 7368 6172 6573 2074   a user shares t
+000036f0: 6865 2073 7472 6561 6d20 6f72 2066 6f6c  he stream or fol
+00003700: 6c6f 7773 2074 6865 2068 6f73 740a 2d20  lows the host.- 
+00003710: 6051 7565 7374 696f 6e4e 6577 4576 656e  `QuestionNewEven
+00003720: 7460 202d 2054 7269 6767 6572 6564 2065  t` - Triggered e
+00003730: 7665 7279 2074 696d 6520 736f 6d65 6f6e  very time someon
+00003740: 6520 6173 6b73 2061 206e 6577 2071 7565  e asks a new que
+00003750: 7374 696f 6e20 7669 6120 7468 6520 7175  stion via the qu
+00003760: 6573 7469 6f6e 2066 6561 7475 7265 2e0a  estion feature..
+00003770: 2d20 604c 6976 6549 6e74 726f 4576 656e  - `LiveIntroEven
+00003780: 7460 202d 2054 7269 6767 6572 6564 2077  t` - Triggered w
+00003790: 6865 6e20 6120 6c69 7665 2069 6e74 726f  hen a live intro
+000037a0: 206d 6573 7361 6765 2061 7070 6561 7273   message appears
+000037b0: 0a2d 2060 4c69 6e6b 4d69 6341 726d 6965  .- `LinkMicArmie
+000037c0: 7345 7665 6e74 6020 2d20 5472 6967 6765  sEvent` - Trigge
+000037d0: 7265 6420 7768 656e 2061 2054 696b 546f  red when a TikTo
+000037e0: 6b20 6261 7474 6c65 2075 7365 7220 7265  k battle user re
+000037f0: 6365 6976 6573 2070 6f69 6e74 730a 2d20  ceives points.- 
+00003800: 604c 696e 6b4d 6963 4261 7474 6c65 4576  `LinkMicBattleEv
+00003810: 656e 7460 202d 2054 7269 6767 6572 6564  ent` - Triggered
+00003820: 2077 6865 6e20 6120 5469 6b54 6f6b 2062   when a TikTok b
+00003830: 6174 746c 6520 6973 2073 7461 7274 6564  attle is started
+00003840: 0a2d 2060 4a6f 696e 4576 656e 7460 202d  .- `JoinEvent` -
+00003850: 2054 7269 6767 6572 6564 2077 6865 6e20   Triggered when 
+00003860: 6120 7573 6572 206a 6f69 6e73 2074 6865  a user joins the
+00003870: 206c 6976 6573 7472 6561 6d0a 2d20 604c   livestream.- `L
+00003880: 696e 6b4d 6963 4661 6e54 6963 6b65 744d  inkMicFanTicketM
+00003890: 6574 686f 6445 7665 6e74 600a 2d20 604c  ethodEvent`.- `L
+000038a0: 696e 6b4d 6963 4d65 7468 6f64 4576 656e  inkMicMethodEven
+000038b0: 7460 0a2d 2060 4261 7272 6167 6545 7665  t`.- `BarrageEve
+000038c0: 6e74 600a 2d20 6043 6170 7469 6f6e 4576  nt`.- `CaptionEv
+000038d0: 656e 7460 0a2d 2060 496d 4465 6c65 7465  ent`.- `ImDelete
+000038e0: 4576 656e 7460 0a2d 2060 526f 6f6d 5573  Event`.- `RoomUs
+000038f0: 6572 5365 7145 7665 6e74 6020 2d20 4375  erSeqEvent` - Cu
+00003900: 7272 656e 7420 7669 6577 6572 2063 6f75  rrent viewer cou
+00003910: 6e74 2069 6e66 6f72 6d61 7469 6f6e 0a2d  nt information.-
+00003920: 2060 5261 6e6b 5570 6461 7465 4576 656e   `RankUpdateEven
+00003930: 7460 0a2d 2060 5261 6e6b 5465 7874 4576  t`.- `RankTextEv
+00003940: 656e 7460 0a2d 2060 486f 7572 6c79 5261  ent`.- `HourlyRa
+00003950: 6e6b 4576 656e 7460 0a2d 2060 556e 6175  nkEvent`.- `Unau
+00003960: 7468 6f72 697a 6564 4d65 6d62 6572 4576  thorizedMemberEv
+00003970: 656e 7460 0a2d 2060 4d65 7373 6167 6544  ent`.- `MessageD
+00003980: 6574 6563 7445 7665 6e74 600a 2d20 604f  etectEvent`.- `O
+00003990: 6563 4c69 7665 5368 6f70 7069 6e67 4576  ecLiveShoppingEv
+000039a0: 656e 7460 0a2d 2060 526f 6f6d 5069 6e45  ent`.- `RoomPinE
+000039b0: 7665 6e74 600a 2d20 6053 7973 7465 6d45  vent`.- `SystemE
+000039c0: 7665 6e74 600a 2d20 604c 696e 6b45 7665  vent`.- `LinkEve
+000039d0: 6e74 600a 2d20 604c 696e 6b4c 6179 6572  nt`.- `LinkLayer
+000039e0: 4576 656e 7460 0a0a 2323 2320 5370 6563  Event`..### Spec
+000039f0: 6961 6c20 4576 656e 7473 0a0a 2323 2320  ial Events..### 
+00003a00: 6047 6966 7445 7665 6e74 600a 0a54 7269  `GiftEvent`..Tri
+00003a10: 6767 6572 6564 2065 7665 7279 2074 696d  ggered every tim
+00003a20: 6520 6120 6769 6674 2061 7272 6976 6573  e a gift arrives
+00003a30: 2e20 4578 7472 6120 696e 666f 726d 6174  . Extra informat
+00003a40: 696f 6e20 6361 6e20 6265 2067 6c65 616d  ion can be gleam
+00003a50: 6564 2066 726f 6d20 7468 6520 6061 7661  ed from the `ava
+00003a60: 696c 6162 6c65 5f67 6966 7473 6020 636c  ilable_gifts` cl
+00003a70: 6965 6e74 2061 7474 7269 6275 7465 2e0a  ient attribute..
+00003a80: 3e20 2a2a 4e4f 5445 3a2a 2a20 5573 6572  > **NOTE:** User
+00003a90: 7320 6861 7665 2074 6865 2063 6170 6162  s have the capab
+00003aa0: 696c 6974 7920 746f 2073 656e 6420 6769  ility to send gi
+00003ab0: 6674 7320 696e 2061 2073 7472 6561 6b2e  fts in a streak.
+00003ac0: 2054 6869 7320 696e 6372 6561 7365 7320   This increases 
+00003ad0: 7468 6520 6065 7665 6e74 2e67 6966 742e  the `event.gift.
+00003ae0: 7265 7065 6174 5f63 6f75 6e74 6020 7661  repeat_count` va
+00003af0: 6c75 6520 756e 7469 6c20 7468 650a 3e20  lue until the.> 
+00003b00: 7573 6572 2074 6572 6d69 6e61 7465 7320  user terminates 
+00003b10: 7468 6520 7374 7265 616b 2e20 4475 7269  the streak. Duri
+00003b20: 6e67 2074 6869 7320 7469 6d65 206e 6577  ng this time new
+00003b30: 2067 6966 7420 6576 656e 7473 2061 7265   gift events are
+00003b40: 2074 7269 6767 6572 6564 2061 6761 696e   triggered again
+00003b50: 2061 6e64 2061 6761 696e 2077 6974 6820   and again with 
+00003b60: 616e 0a3e 2069 6e63 7265 6173 6564 2060  an.> increased `
+00003b70: 6576 656e 742e 6769 6674 2e72 6570 6561  event.gift.repea
+00003b80: 745f 636f 756e 7460 2076 616c 7565 2e20  t_count` value. 
+00003b90: 4974 2073 686f 756c 6420 6265 206e 6f74  It should be not
+00003ba0: 6564 2074 6861 7420 6166 7465 7220 7468  ed that after th
+00003bb0: 6520 656e 6420 6f66 2061 2073 7472 6561  e end of a strea
+00003bc0: 6b2c 2061 2066 696e 616c 2067 6966 7420  k, a final gift 
+00003bd0: 6576 656e 7420 6973 0a3e 2074 7269 6767  event is.> trigg
+00003be0: 6572 6564 2c20 7768 6963 6820 7369 676e  ered, which sign
+00003bf0: 616c 7320 7468 6520 656e 6420 6f66 2074  als the end of t
+00003c00: 6865 2073 7472 6561 6b20 7769 7468 2060  he streak with `
+00003c10: 6576 656e 742e 7265 7065 6174 5f65 6e64  event.repeat_end
+00003c20: 603a 6031 602e 2054 6865 2066 6f6c 6c6f  `:`1`. The follo
+00003c30: 7769 6e67 2068 616e 646c 6572 7320 7368  wing handlers sh
+00003c40: 6f77 2068 6f77 2079 6f75 2063 616e 2064  ow how you can d
+00003c50: 6561 6c20 7769 7468 2074 6869 7320 696e  eal with this in
+00003c60: 2079 6f75 7220 636f 6465 2e0a 0a55 7369   your code...Usi
+00003c70: 6e67 2074 6865 206c 6f77 2d6c 6576 656c  ng the low-level
+00003c80: 2064 6972 6563 7420 7072 6f74 6f3a 0a60   direct proto:.`
+00003c90: 6060 7079 7468 6f6e 0a40 636c 6965 6e74  ``python.@client
+00003ca0: 2e6f 6e28 4769 6674 4576 656e 7429 0a61  .on(GiftEvent).a
+00003cb0: 7379 6e63 2064 6566 206f 6e5f 6769 6674  sync def on_gift
+00003cc0: 2865 7665 6e74 3a20 4769 6674 4576 656e  (event: GiftEven
+00003cd0: 7429 3a0a 2020 2020 2320 4966 2069 7427  t):.    # If it'
+00003ce0: 7320 7479 7065 2031 2061 6e64 2074 6865  s type 1 and the
+00003cf0: 2073 7472 6561 6b20 6973 206f 7665 720a   streak is over.
+00003d00: 2020 2020 6966 2065 7665 6e74 2e67 6966      if event.gif
+00003d10: 742e 696e 666f 2e74 7970 6520 3d3d 2031  t.info.type == 1
+00003d20: 3a0a 2020 2020 2020 2020 6966 2065 7665  :.        if eve
+00003d30: 6e74 2e67 6966 742e 6973 5f72 6570 6561  nt.gift.is_repea
+00003d40: 7469 6e67 203d 3d20 313a 0a20 2020 2020  ting == 1:.     
+00003d50: 2020 2020 2020 2070 7269 6e74 2866 227b         print(f"{
+00003d60: 6576 656e 742e 7573 6572 2e75 6e69 7175  event.user.uniqu
+00003d70: 655f 6964 7d20 7365 6e74 207b 6576 656e  e_id} sent {even
+00003d80: 742e 6769 6674 2e63 6f75 6e74 7d78 205c  t.gift.count}x \
+00003d90: 227b 6576 656e 742e 6769 6674 2e69 6e66  "{event.gift.inf
+00003da0: 6f2e 6e61 6d65 7d5c 2222 290a 0a20 2020  o.name}\"")..   
+00003db0: 2023 2049 7427 7320 6e6f 7420 7479 7065   # It's not type
+00003dc0: 2031 2c20 7768 6963 6820 6d65 616e 7320   1, which means 
+00003dd0: 6974 2063 616e 2774 2068 6176 6520 6120  it can't have a 
+00003de0: 7374 7265 616b 2026 2069 7320 6175 746f  streak & is auto
+00003df0: 6d61 7469 6361 6c6c 7920 6f76 6572 0a20  matically over. 
+00003e00: 2020 2065 6c69 6620 6576 656e 742e 6769     elif event.gi
+00003e10: 6674 2e69 6e66 6f2e 7479 7065 2021 3d20  ft.info.type != 
+00003e20: 313a 0a20 2020 2020 2020 2070 7269 6e74  1:.        print
+00003e30: 2866 227b 6576 656e 742e 7573 6572 2e75  (f"{event.user.u
+00003e40: 6e69 7175 655f 6964 7d20 7365 6e74 205c  nique_id} sent \
+00003e50: 227b 6576 656e 742e 6769 6674 2e69 6e66  "{event.gift.inf
+00003e60: 6f2e 6e61 6d65 7d5c 2222 290a 6060 600a  o.name}\"").```.
+00003e70: 0a55 7369 6e67 2074 6865 2054 696b 546f  .Using the TikTo
+00003e80: 6b4c 6976 6520 6578 7465 6e64 6564 2070  kLive extended p
+00003e90: 726f 746f 3a0a 6060 6070 7974 686f 6e0a  roto:.```python.
+00003ea0: 4063 6c69 656e 742e 6f6e 2822 6769 6674  @client.on("gift
+00003eb0: 2229 0a61 7379 6e63 2064 6566 206f 6e5f  ").async def on_
+00003ec0: 6769 6674 2865 7665 6e74 3a20 4769 6674  gift(event: Gift
+00003ed0: 4576 656e 7429 3a0a 2020 2020 2320 5374  Event):.    # St
+00003ee0: 7265 616b 6162 6c65 2067 6966 7420 2620  reakable gift & 
+00003ef0: 7374 7265 616b 2069 7320 6f76 6572 0a20  streak is over. 
+00003f00: 2020 2069 6620 6576 656e 742e 6769 6674     if event.gift
+00003f10: 2e73 7472 6561 6b61 626c 6520 616e 6420  .streakable and 
+00003f20: 6e6f 7420 6576 656e 742e 7374 7265 616b  not event.streak
+00003f30: 696e 673a 0a20 2020 2020 2020 2070 7269  ing:.        pri
+00003f40: 6e74 2866 227b 6576 656e 742e 7573 6572  nt(f"{event.user
+00003f50: 2e75 6e69 7175 655f 6964 7d20 7365 6e74  .unique_id} sent
+00003f60: 207b 6576 656e 742e 6769 6674 2e63 6f75   {event.gift.cou
+00003f70: 6e74 7d78 205c 227b 6576 656e 742e 6769  nt}x \"{event.gi
+00003f80: 6674 2e69 6e66 6f2e 6e61 6d65 7d5c 2222  ft.info.name}\""
+00003f90: 290a 0a20 2020 2023 204e 6f6e 2d73 7472  )..    # Non-str
+00003fa0: 6561 6b61 626c 6520 6769 6674 0a20 2020  eakable gift.   
+00003fb0: 2065 6c69 6620 6e6f 7420 6576 656e 742e   elif not event.
+00003fc0: 6769 6674 2e73 7472 6561 6b61 626c 653a  gift.streakable:
+00003fd0: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
+00003fe0: 227b 6576 656e 742e 7573 6572 2e75 6e69  "{event.user.uni
+00003ff0: 7175 655f 6964 7d20 7365 6e74 205c 227b  que_id} sent \"{
+00004000: 6576 656e 742e 6769 6674 2e69 6e66 6f2e  event.gift.info.
+00004010: 6e61 6d65 7d5c 2222 290a 0a60 6060 0a0a  name}\"")..```..
+00004020: 2323 2320 6053 7562 7363 7269 6265 4576  ### `SubscribeEv
+00004030: 656e 7460 0a0a 5468 6973 2065 7665 6e74  ent`..This event
+00004040: 2077 696c 6c20 6f6e 6c79 2066 6972 6520   will only fire 
+00004050: 7768 656e 2061 2073 6573 7369 6f6e 2049  when a session I
+00004060: 4420 2861 6363 6f75 6e74 206c 6f67 696e  D (account login
+00004070: 2920 6973 2070 6173 7365 6420 746f 2074  ) is passed to t
+00004080: 6865 2048 5454 5020 636c 6965 6e74 202a  he HTTP client *
+00004090: 6265 666f 7265 2a20 636f 6e6e 6563 7469  before* connecti
+000040a0: 6e67 2074 6f20 5469 6b54 6f6b 204c 4956  ng to TikTok LIV
+000040b0: 452e 0a59 6f75 2063 616e 2073 6574 2074  E..You can set t
+000040c0: 6865 2073 6573 7369 6f6e 2049 4420 7769  he session ID wi
+000040d0: 7468 205b 6063 6c69 656e 742e 7765 622e  th [`client.web.
+000040e0: 7365 745f 7365 7373 696f 6e5f 6964 282e  set_session_id(.
+000040f0: 2e2e 2960 5d28 6874 7470 733a 2f2f 6769  ..)`](https://gi
+00004100: 7468 7562 2e63 6f6d 2f69 7361 6163 6b6f  thub.com/isaacko
+00004110: 6761 6e2f 5469 6b54 6f6b 4c69 7665 2f62  gan/TikTokLive/b
+00004120: 6c6f 622f 6d61 7374 6572 2f65 7861 6d70  lob/master/examp
+00004130: 6c65 732f 6c6f 6767 6564 5f69 6e2e 7079  les/logged_in.py
+00004140: 292e 0a0a 2323 2043 6865 636b 696e 6720  )...## Checking 
+00004150: 4966 2041 2055 7365 7220 4973 204c 6976  If A User Is Liv
+00004160: 650a 0a49 7420 6973 2063 6f6e 7369 6465  e..It is conside
+00004170: 7265 6420 696e 6566 6669 6369 656e 7420  red inefficient 
+00004180: 746f 2075 7365 2074 6865 2063 6f6e 6e65  to use the conne
+00004190: 6374 206d 6574 686f 6420 746f 2063 6865  ct method to che
+000041a0: 636b 2069 6620 6120 7573 6572 2069 7320  ck if a user is 
+000041b0: 6c69 7665 2e20 4974 2069 7320 6265 7474  live. It is bett
+000041c0: 6572 2074 6f20 7573 6520 7468 6520 6465  er to use the de
+000041d0: 6469 6361 7465 6420 6061 7761 6974 2063  dicated `await c
+000041e0: 6c69 656e 742e 6973 5f6c 6976 6528 2960  lient.is_live()`
+000041f0: 206d 6574 686f 642e 200a 0a54 6865 7265   method. ..There
+00004200: 2069 7320 6120 5b63 6f6d 706c 6574 6520   is a [complete 
+00004210: 6578 616d 706c 655d 2868 7474 7073 3a2f  example](https:/
+00004220: 2f67 6974 6875 622e 636f 6d2f 6973 6161  /github.com/isaa
+00004230: 636b 6f67 616e 2f54 696b 546f 6b4c 6976  ckogan/TikTokLiv
+00004240: 652f 626c 6f62 2f6d 6173 7465 722f 6578  e/blob/master/ex
+00004250: 616d 706c 6573 2f63 6865 636b 5f6c 6976  amples/check_liv
+00004260: 652e 7079 2920 6f66 2068 6f77 2074 6f20  e.py) of how to 
+00004270: 646f 2074 6869 7320 696e 2074 6865 205b  do this in the [
+00004280: 6578 616d 706c 6573 5d28 6874 7470 733a  examples](https:
+00004290: 2f2f 6769 7468 7562 2e63 6f6d 2f69 7361  //github.com/isa
+000042a0: 6163 6b6f 6761 6e2f 5469 6b54 6f6b 4c69  ackogan/TikTokLi
+000042b0: 7665 2f74 7265 652f 6d61 7374 6572 2f65  ve/tree/master/e
+000042c0: 7861 6d70 6c65 7329 2066 6f6c 6465 722e  xamples) folder.
+000042d0: 0a0a 2323 2043 6f6e 7472 6962 7574 6f72  ..## Contributor
+000042e0: 730a 0a2a 202a 2a49 7361 6163 204b 6f67  s..* **Isaac Kog
+000042f0: 616e 2a2a 202d 202a 4372 6561 746f 722c  an** - *Creator,
+00004300: 2050 7269 6d61 7279 204d 6169 6e74 6169   Primary Maintai
+00004310: 6e65 722c 2061 6e64 2052 6576 6572 7365  ner, and Reverse
+00004320: 2d45 6e67 696e 6565 7269 6e67 2a20 2d20  -Engineering* - 
+00004330: 5b69 7361 6163 6b6f 6761 6e5d 2868 7474  [isaackogan](htt
+00004340: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004350: 6973 6161 636b 6f67 616e 290a 2a20 2a2a  isaackogan).* **
+00004360: 5a65 726f 6479 2a2a 202d 202a 496e 6974  Zerody** - *Init
+00004370: 6961 6c20 5265 7665 7273 652d 456e 6769  ial Reverse-Engi
+00004380: 6e65 6572 696e 6720 5072 6f74 6f62 7566  neering Protobuf
+00004390: 2026 2053 7570 706f 7274 2a20 2d20 5b5a   & Support* - [Z
+000043a0: 6572 6f64 795d 2868 7474 7073 3a2f 2f67  erody](https://g
+000043b0: 6974 6875 622e 636f 6d2f 7a65 726f 6479  ithub.com/zerody
+000043c0: 7472 6173 682f 290a 2a20 2a2a 4461 7669  trash/).* **Davi
+000043d0: 6e63 6962 6c65 2a2a 202d 202a 5265 7665  ncible** - *Reve
+000043e0: 7273 652d 456e 6769 6e65 6572 696e 6720  rse-Engineering 
+000043f0: 5374 7265 616d 2044 6f77 6e6c 6f61 6473  Stream Downloads
+00004400: 2a20 202d 205b 6461 7669 6e63 6962 6c65  *  - [davincible
+00004410: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004420: 2e63 6f6d 2f64 6176 696e 6369 626c 6529  .com/davincible)
+00004430: 0a0a 5365 6520 616c 736f 2074 6865 2066  ..See also the f
+00004440: 756c 6c20 6c69 7374 206f 6620 5b63 6f6e  ull list of [con
+00004450: 7472 6962 7574 6f72 735d 2868 7474 7073  tributors](https
+00004460: 3a2f 2f67 6974 6875 622e 636f 6d2f 6973  ://github.com/is
+00004470: 6161 636b 6f67 616e 2f54 696b 546f 6b4c  aackogan/TikTokL
+00004480: 6976 652f 636f 6e74 7269 6275 746f 7273  ive/contributors
+00004490: 2920 7768 6f20 6861 7665 2070 6172 7469  ) who have parti
+000044a0: 6369 7061 7465 6420 696e 0a74 6869 7320  cipated in.this 
+000044b0: 7072 6f6a 6563 742e 0a0a 2323 204c 6963  project...## Lic
+000044c0: 656e 7365 0a0a 5468 6973 2070 726f 6a65  ense..This proje
+000044d0: 6374 2069 7320 6c69 6365 6e73 6564 2075  ct is licensed u
+000044e0: 6e64 6572 2074 6865 204d 4954 204c 6963  nder the MIT Lic
+000044f0: 656e 7365 202d 2073 6565 2074 6865 205b  ense - see the [
+00004500: 4c49 4345 4e53 455d 284c 4943 454e 5345  LICENSE](LICENSE
+00004510: 2920 6669 6c65 2066 6f72 2064 6574 6169  ) file for detai
+00004520: 6c73 2e0a                                ls..
```

### Comparing `TikTokLive-6.0.3/README.md` & `TikTokLive-6.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,29 @@
 allows you to
 connect directly to TikTok with just a username (`@unique_id`). No credentials are required to use TikTokLive.
 
 Join the [TikTokLive discord](https://discord.gg/e2XwPNTBBr) and visit
 the [`#py-support`](https://discord.gg/uja6SajDxd)
 channel for questions, contributions and ideas.
 
+### Enterprise Access
+
+- Tokens to scrape ANY TikTok URL (i.e. fetch profiles,  videos, comments, etc.)
+- Increased TikTok LIVE rate limits (i.e. ability to 1000s of clients per hour)
+
+<div align="left">
+    <a href="https://eulerstream.com" target="_blank">
+        <div>
+            <b>Eulerstream</b> offers paid plans for enterprises for increased TikTokLive access & TikTok API tokens for data collection
+        </div>
+        <br/>
+        <img src="https://github.com/isaackogan/TikTokLive/assets/65869106/b56cef89-5d87-4f2f-ac3e-0685af21b28d)" width="100" alt="Eulerstream">
+    </a>
+</div>
+
 ### Consider Donating <3
 
 I'm a 2nd-year Biology student in university who likes to program for fun. Please consider supporting development
 through a small donation at [https://www.buymeacoffee.com/isaackogan](https://www.buymeacoffee.com/isaackogan). Anything
 you can offer will go towards school & development costs for TikTokLive, which has taken hundreds of hours of time to build.
 
 ### Other Languages
```

### Comparing `TikTokLive-6.0.3/TikTokLive/client/client.py` & `TikTokLive-6.0.4/TikTokLive/client/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
+import inspect
 import logging
 import traceback
 import urllib.parse
 from asyncio import AbstractEventLoop, Task, CancelledError
 from logging import Logger
-from typing import Optional, Type, AsyncIterator, Dict, Any, Tuple, Union, Callable, List
+from typing import Optional, Type, AsyncIterator, Dict, Any, Tuple, Union, Callable, List, Coroutine
 
 from httpx import Proxy
 from pyee import AsyncIOEventEmitter
 from pyee.base import Handler
 
 from TikTokLive.client.errors import AlreadyConnectedError, UserOfflineError, InitialCursorMissingError, \
     WebsocketURLMissingError
@@ -87,41 +88,52 @@
             .replace("@", "", 1) \
             .strip()
 
     async def start(
             self,
             *,
             process_connect_events: bool = True,
-            fetch_room_info: bool = True,
+            fetch_room_info: bool = False,
             fetch_gift_info: bool = False,
+            fetch_live_check: bool = True,
             room_id: Optional[int] = None
     ) -> Task:
         """
         Create a non-blocking connection to TikTok LIVE and return the task
 
         :param process_connect_events: Whether to process initial events sent on room join
         :param fetch_room_info: Whether to fetch room info on join
         :param fetch_gift_info: Whether to fetch gift info on join
+        :param fetch_live_check: Whether to check if the user is live (you almost ALWAYS want this enabled)
         :param room_id: An override to the room ID to connect directly to the livestream and skip scraping the live.
                         Useful when trying to scale, as scraping the HTML can result in TikTok blocks.
         :return: Task containing the heartbeat of the client
 
         """
 
         if self._ws.connected:
             raise AlreadyConnectedError("You can only make one connection per client!")
 
         # <Required> Fetch room ID
-        self._room_id: str = room_id or await self._web.fetch_room_id(self._unique_id)
+        try:
+            self._room_id: str = room_id or await self._web.fetch_room_id_from_html(self._unique_id)
+        except Exception as base_ex:
+            try:
+                self._logger.error("Failed to parse room ID from HTML. Using API fallback.")
+                self._room_id: str = await self._web.fetch_room_id_from_api(self.unique_id)
+            except Exception as super_ex:
+                raise super_ex from base_ex
+
+        # <Optional> Fetch live status
+        if fetch_live_check and not await self._web.fetch_is_live(room_id=self._room_id):
+            raise UserOfflineError()
 
         # <Optional> Fetch room info
         if fetch_room_info:
             self._room_info = await self._web.fetch_room_info()
-            if self._room_info.get("status", 4) == 4:
-                raise UserOfflineError()
 
         # <Optional> Fetch gift info
         if fetch_gift_info:
             self._gift_info = await self._web.fetch_gift_list()
 
         # <Required> Fetch the first response
         webcast_response: WebcastResponse = await self._web.fetch_sign_fetch()
@@ -137,26 +149,43 @@
         if not webcast_response.route_params_map:
             raise WebsocketURLMissingError("Websocket parameters missing.")
 
         # Start the websocket connection & return it
         self._event_loop_task = self._asyncio_loop.create_task(self._client_loop(webcast_response))
         return self._event_loop_task
 
-    async def connect(self, **kwargs) -> Task:
+    async def connect(
+            self,
+            callback: Optional[
+                Union[
+                    Callable[[None], None],
+                    Callable[[None], Coroutine[None, None, None]],
+                    Coroutine[None, None, None],
+                ]
+            ] = None,
+            **kwargs
+    ) -> Task:
         """
         Start a future-blocking connection to TikTokLive
 
+        :param callback: A callback function to run when connected
         :param kwargs: Kwargs to pass to start
         :return: The task, once it's finished
 
         """
 
         task: Task = await self.start(**kwargs)
 
         try:
+            if inspect.iscoroutinefunction(callback):
+                self._asyncio_loop.create_task(callback())
+            elif inspect.isawaitable(callback):
+                self._asyncio_loop.create_task(callback)
+            elif inspect.isfunction(callback):
+                callback()
             await task
         except CancelledError:
             self._logger.debug("The client has been manually stopped with 'client.stop()'.")
 
         return task
 
     def run(self, **kwargs) -> Task:
@@ -279,14 +308,16 @@
         Method that can be used to register a Python function as an event listener
 
         :param event: The event to listen to
         :param f: The function to handle the event
         :return: The generated `pyee.Handler` object
 
         """
+        if isinstance(event, str):
+            return super().add_listener(event=event, f=f)
 
         return super().add_listener(event=event.get_type(), f=f)
 
     def has_listener(self, event: Type[Event]) -> bool:
         """
         Check whether the client is listening to a given event
```

### Comparing `TikTokLive-6.0.3/TikTokLive/client/errors.py` & `TikTokLive-6.0.4/TikTokLive/client/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 class UserOfflineError(RuntimeError):
     """
     Thrown when the requested streamer to watch is offline
 
     """
 
+class AgeRestrictedError(RuntimeError):
+    """
+    Thrown when a LIVE is age restricted. Pass sessionid to bypass.
+    """
 
 class InitialCursorMissingError(RuntimeError):
     """
     Thrown when the cursor for connecting to TikTok is missing (blocked)
 
     """
```

### Comparing `TikTokLive-6.0.3/TikTokLive/client/logger.py` & `TikTokLive-6.0.4/TikTokLive/client/logger.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_gift_list.py` & `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_gift_list.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_image.py` & `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_image.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_is_live.py` & `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_is_live.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,25 @@
 from typing import Optional, List
 
 from httpx import Response
 
+from TikTokLive.client.web.routes.fetch_room_id_api import RoomIdAPIRoute
 from TikTokLive.client.web.web_base import ClientRoute
 from TikTokLive.client.web.web_settings import WebDefaults
 
 
 class InvalidFetchIsLiveRequest(RuntimeError):
     """
     Thrown when the request to check if a user is live fails
 
     """
 
     pass
 
 
-class InvalidLiveUser(RuntimeError):
-    """
-    Thrown when the request to check if a user is live fails because a user has no
-    livestream account (e.g. <1000 followers)
-
-    """
-
-    def __init__(self, unique_id: str, *args):
-        self.unique_id: str = unique_id
-        super().__init__(*args)
-
-
 class FetchIsLiveRoute(ClientRoute):
     """
     Check if a given user is alive through their unique_id or room_id
 
     """
 
     async def __call__(
@@ -83,30 +72,13 @@
         :param unique_id: The unique_id of the user
         :return: Whether they are live
 
         :raises: InvalidLiveUser
 
         """
 
-        response: Response = await self._web.get_response(
-            url=WebDefaults.tiktok_app_url + f"/api-live/user/room/",
-            extra_params=(
-                {
-                    "uniqueId": unique_id,
-                    "sourceType": 54
-                }
-            )
+        response_json: dict = await RoomIdAPIRoute.fetch_user_room_data(
+            web=self._web,
+            unique_id=unique_id
         )
 
-        response_json: dict = response.json()
-
-        # Invalid user
-        if response_json["message"] == "user_not_found":
-            raise InvalidLiveUser(
-                unique_id,
-                (
-                    f"The requested user '{unique_id}' is not capable of going LIVE on TikTok, "
-                    "or has never gone live on TikTok, or does not exist."
-                )
-            )
-
         return response_json["data"]["liveRoom"]["status"] != 4
```

### Comparing `TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_room_id.py` & `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_room_id_html.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import random
 import re
 
 from httpx import Response
 
 from TikTokLive.client.errors import UserOfflineError
 from TikTokLive.client.web.web_base import ClientRoute
 from TikTokLive.client.web.web_settings import WebDefaults
@@ -11,15 +10,15 @@
 class FailedParseRoomIdError(RuntimeError):
     """
     Thrown when the Room ID cannot be parsed
 
     """
 
 
-class RoomIdRoute(ClientRoute):
+class RoomIdHTMLRoute(ClientRoute):
     """
     Route to retrieve the room ID for a user
 
     """
 
     async def __call__(self, unique_id: str) -> str:
         """
@@ -28,15 +27,16 @@
         :param unique_id: The user's username
         :return: The room ID string
 
         """
 
         # Get their livestream HTML
         response: Response = await self._web.get_response(
-            url=WebDefaults.tiktok_app_url + f"/@{unique_id}/live"
+            url=WebDefaults.tiktok_app_url + f"/@{unique_id}/live",
+            base_params=False
         )
 
         # Parse & update the web client
         room_id: str = self.parse_room_id(response.text)
         self._web.params["room_id"] = room_id
         return room_id
```

### Comparing `TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_sign.py` & `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_sign.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                 SignAPIError.ErrorReason.EMPTY_PAYLOAD,
                 f"Sign API returned an empty request. Are you being detected by TikTok?"
             )
 
         elif not response.status_code == 200:
             raise SignAPIError(
                 SignAPIError.ErrorReason.SIGN_NOT_200,
-                f"Failed request to Sign API with status code {response.status_code}."
+                f"Failed request to Sign API with status code {response.status_code} and payload \"{response.read()}\"."
             )
 
         webcast_response: WebcastResponse = WebcastResponse().parse(response.read())
 
         # Update web params & cookies
         self._update_tiktok_cookies(response)
         self._web.params["cursor"] = webcast_response.cursor
```

### Comparing `TikTokLive-6.0.3/TikTokLive/client/web/routes/fetch_video.py` & `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_video.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLive/client/web/web_base.py` & `TikTokLive-6.0.4/TikTokLive/client/web/web_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -63,49 +63,51 @@
         self.params: Dict[str, Any] = {
             **httpx_kwargs.pop("params", {}), **WebDefaults.client_params
         }
 
         return AsyncClient(
             proxies=proxy,
             cookies=self.cookies,
-            params=self.params,
-            headers=self.headers,
             **httpx_kwargs
         )
 
     async def get_response(
             self,
             url: str,
             extra_params: dict = {},
             extra_headers: dict = {},
             client: Optional[httpx.AsyncClient] = None,
+            base_params: bool = True,
+            base_headers: bool = True,
             **kwargs
     ) -> Response:
         """
         Get a response from the underlying `httpx.AsyncClient` client.
 
         :param url: The URL to request
         :param extra_params: Extra parameters to append to the globals
         :param extra_headers: Extra headers to append to the globals
         :param client: An optional override for the `httpx.AsyncClient` client
         :param kwargs: Optional keywords for the `httpx.AsyncClient.get` method
+        :param base_params: Whether to include the base params
+        :param base_headers: Whether to include the base headers
         :return: An `httpx.Response` object
 
         """
 
         # Update UUC param
         self.params["uuc"] = self.__uuc
         self.params["device_id"] = self.generate_device_id()
 
         # Make the request
         return await (client or self._httpx).get(
             url=url,
             cookies=self.cookies,
-            params={**self.params, **extra_params},
-            headers={**self.headers, **extra_headers},
+            params={**(self.params if base_params else {}), **extra_params},
+            headers={**(self.headers if base_headers else {}), **extra_headers},
             **kwargs
         )
 
     async def close(self) -> None:
         """
         Close the HTTP client gracefully
```

### Comparing `TikTokLive-6.0.3/TikTokLive/client/web/web_client.py` & `TikTokLive-6.0.4/TikTokLive/client/web/web_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from TikTokLive.client.web.routes import FetchIsLiveRoute
+from TikTokLive.client.web.routes.fetch_room_id_api import RoomIdAPIRoute
 from TikTokLive.client.web.routes.fetch_video import VideoFetchRoute
 from TikTokLive.client.web.routes.fetch_gift_list import GiftListRoute
 from TikTokLive.client.web.routes.fetch_image import ImageFetchRoute
-from TikTokLive.client.web.routes.fetch_room_id import RoomIdRoute
+from TikTokLive.client.web.routes.fetch_room_id_html import RoomIdHTMLRoute
 from TikTokLive.client.web.routes.fetch_room_info import FetchRoomInfoRoute
 from TikTokLive.client.web.routes.fetch_sign import SignFetchRoute
 from TikTokLive.client.web.web_base import TikTokHTTPClient
 
 
 class TikTokWebClient(TikTokHTTPClient):
     """
@@ -20,14 +21,15 @@
 
         :param kwargs: Arguments to pass to the super-class
 
         """
 
         super().__init__(**kwargs)
 
-        self.fetch_room_id: RoomIdRoute = RoomIdRoute(self)
+        self.fetch_room_id_from_html: RoomIdHTMLRoute = RoomIdHTMLRoute(self)
+        self.fetch_room_id_from_api: RoomIdAPIRoute = RoomIdAPIRoute(self)
         self.fetch_room_info: FetchRoomInfoRoute = FetchRoomInfoRoute(self)
         self.fetch_gift_list: GiftListRoute = GiftListRoute(self)
         self.fetch_image: ImageFetchRoute = ImageFetchRoute(self)
         self.fetch_video: VideoFetchRoute = VideoFetchRoute(self)
         self.fetch_is_live: FetchIsLiveRoute = FetchIsLiveRoute(self)
         self.fetch_sign_fetch: SignFetchRoute = SignFetchRoute(self, self._sign_api_key)
```

### Comparing `TikTokLive-6.0.3/TikTokLive/client/web/web_settings.py` & `TikTokLive-6.0.4/TikTokLive/client/web/web_settings.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLive/client/ws/ws_client.py` & `TikTokLive-6.0.4/TikTokLive/client/ws/ws_client.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLive/events/__init__.py` & `TikTokLive-6.0.4/TikTokLive/events/__init__.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLive/events/custom_events.py` & `TikTokLive-6.0.4/TikTokLive/events/custom_events.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLive/events/proto_events.py` & `TikTokLive-6.0.4/TikTokLive/events/proto_events.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLive/proto/custom_proto.py` & `TikTokLive-6.0.4/TikTokLive/proto/custom_proto.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLive/proto/tiktok_proto.py` & `TikTokLive-6.0.4/TikTokLive/proto/tiktok_proto.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLive.egg-info/PKG-INFO` & `TikTokLive-6.0.4/TikTokLive.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 5469 6b54  : 2.1.Name: TikT
 00000020: 6f6b 4c69 7665 0a56 6572 7369 6f6e 3a20  okLive.Version: 
-00000030: 362e 302e 330a 5375 6d6d 6172 793a 2054  6.0.3.Summary: T
+00000030: 362e 302e 340a 5375 6d6d 6172 793a 2054  6.0.4.Summary: T
 00000040: 696b 546f 6b20 4c69 7665 2050 7974 686f  ikTok Live Pytho
 00000050: 6e20 436c 6965 6e74 0a48 6f6d 652d 7061  n Client.Home-pa
 00000060: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000070: 7562 2e63 6f6d 2f69 7361 6163 6b6f 6761  ub.com/isaackoga
 00000080: 6e2f 5469 6b54 6f6b 4c69 7665 0a44 6f77  n/TikTokLive.Dow
 00000090: 6e6c 6f61 642d 5552 4c3a 2068 7474 7073  nload-URL: https
 000000a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6973  ://github.com/is
 000000b0: 6161 636b 6f67 616e 2f54 696b 546f 6b4c  aackogan/TikTokL
 000000c0: 6976 652f 7265 6c65 6173 6573 2f74 6167  ive/releases/tag
-000000d0: 2f76 362e 302e 330a 4175 7468 6f72 3a20  /v6.0.3.Author: 
+000000d0: 2f76 362e 302e 340a 4175 7468 6f72 3a20  /v6.0.4.Author: 
 000000e0: 4973 6161 6320 4b6f 6761 6e0a 4175 7468  Isaac Kogan.Auth
 000000f0: 6f72 2d65 6d61 696c 3a20 696e 666f 4069  or-email: info@i
 00000100: 7361 6163 6b6f 6761 6e2e 636f 6d0a 4c69  saackogan.com.Li
 00000110: 6365 6e73 653a 204d 4954 0a4b 6579 776f  cense: MIT.Keywo
 00000120: 7264 733a 2074 696b 746f 6b2c 7469 6b74  rds: tiktok,tikt
 00000130: 6f6b 206c 6976 652c 7079 7468 6f6e 332c  ok live,python3,
 00000140: 6170 692c 756e 6f66 6669 6369 616c 0a43  api,unofficial.C
@@ -134,936 +134,974 @@
 00000850: 2f65 3258 7750 4e54 4242 7229 2061 6e64  /e2XwPNTBBr) and
 00000860: 2076 6973 6974 0a74 6865 205b 6023 7079   visit.the [`#py
 00000870: 2d73 7570 706f 7274 605d 2868 7474 7073  -support`](https
 00000880: 3a2f 2f64 6973 636f 7264 2e67 672f 756a  ://discord.gg/uj
 00000890: 6136 5361 6a44 7864 290a 6368 616e 6e65  a6SajDxd).channe
 000008a0: 6c20 666f 7220 7175 6573 7469 6f6e 732c  l for questions,
 000008b0: 2063 6f6e 7472 6962 7574 696f 6e73 2061   contributions a
-000008c0: 6e64 2069 6465 6173 2e0a 0a23 2323 2043  nd ideas...### C
-000008d0: 6f6e 7369 6465 7220 446f 6e61 7469 6e67  onsider Donating
-000008e0: 203c 330a 0a49 276d 2061 2032 6e64 2d79   <3..I'm a 2nd-y
-000008f0: 6561 7220 4269 6f6c 6f67 7920 7374 7564  ear Biology stud
-00000900: 656e 7420 696e 2075 6e69 7665 7273 6974  ent in universit
-00000910: 7920 7768 6f20 6c69 6b65 7320 746f 2070  y who likes to p
-00000920: 726f 6772 616d 2066 6f72 2066 756e 2e20  rogram for fun. 
-00000930: 506c 6561 7365 2063 6f6e 7369 6465 7220  Please consider 
-00000940: 7375 7070 6f72 7469 6e67 2064 6576 656c  supporting devel
-00000950: 6f70 6d65 6e74 0a74 6872 6f75 6768 2061  opment.through a
-00000960: 2073 6d61 6c6c 2064 6f6e 6174 696f 6e20   small donation 
-00000970: 6174 205b 6874 7470 733a 2f2f 7777 772e  at [https://www.
-00000980: 6275 796d 6561 636f 6666 6565 2e63 6f6d  buymeacoffee.com
-00000990: 2f69 7361 6163 6b6f 6761 6e5d 2868 7474  /isaackogan](htt
-000009a0: 7073 3a2f 2f77 7777 2e62 7579 6d65 6163  ps://www.buymeac
-000009b0: 6f66 6665 652e 636f 6d2f 6973 6161 636b  offee.com/isaack
-000009c0: 6f67 616e 292e 2041 6e79 7468 696e 670a  ogan). Anything.
-000009d0: 796f 7520 6361 6e20 6f66 6665 7220 7769  you can offer wi
-000009e0: 6c6c 2067 6f20 746f 7761 7264 7320 7363  ll go towards sc
-000009f0: 686f 6f6c 2026 2064 6576 656c 6f70 6d65  hool & developme
-00000a00: 6e74 2063 6f73 7473 2066 6f72 2054 696b  nt costs for Tik
-00000a10: 546f 6b4c 6976 652c 2077 6869 6368 2068  TokLive, which h
-00000a20: 6173 2074 616b 656e 2068 756e 6472 6564  as taken hundred
-00000a30: 7320 6f66 2068 6f75 7273 206f 6620 7469  s of hours of ti
-00000a40: 6d65 2074 6f20 6275 696c 642e 0a0a 2323  me to build...##
-00000a50: 2320 4f74 6865 7220 4c61 6e67 7561 6765  # Other Language
-00000a60: 730a 0a54 696b 546f 6b4c 6976 6520 6973  s..TikTokLive is
-00000a70: 2061 7661 696c 6162 6c65 2069 6e20 7365   available in se
-00000a80: 7665 7261 6c20 616c 7465 726e 6174 6520  veral alternate 
-00000a90: 7072 6f67 7261 6d6d 696e 6720 6c61 6e67  programming lang
-00000aa0: 7561 6765 733a 0a0a 2d20 2a2a 4e6f 6465  uages:..- **Node
-00000ab0: 2e4a 533a 2a2a 205b 6874 7470 733a 2f2f  .JS:** [https://
-00000ac0: 6769 7468 7562 2e63 6f6d 2f7a 6572 6f64  github.com/zerod
-00000ad0: 7974 7261 7368 2f54 696b 546f 6b2d 4c69  ytrash/TikTok-Li
-00000ae0: 7665 2d43 6f6e 6e65 6374 6f72 5d28 6874  ve-Connector](ht
-00000af0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000b00: 2f7a 6572 6f64 7974 7261 7368 2f54 696b  /zerodytrash/Tik
-00000b10: 546f 6b2d 4c69 7665 2d43 6f6e 6e65 6374  Tok-Live-Connect
-00000b20: 6f72 290a 2d20 2a2a 4a61 7661 3a2a 2a20  or).- **Java:** 
-00000b30: 5b68 7474 7073 3a2f 2f67 6974 6875 622e  [https://github.
-00000b40: 636f 6d2f 6a77 6465 7665 6c6f 7065 722f  com/jwdeveloper/
-00000b50: 5469 6b54 6f6b 2d4c 6976 652d 4a61 7661  TikTok-Live-Java
-00000b60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000b70: 2e63 6f6d 2f6a 7764 6576 656c 6f70 6572  .com/jwdeveloper
-00000b80: 2f54 696b 546f 6b2d 4c69 7665 2d4a 6176  /TikTok-Live-Jav
-00000b90: 6129 0a2d 202a 2a43 232f 556e 6974 793a  a).- **C#/Unity:
-00000ba0: 2a2a 205b 6874 7470 733a 2f2f 6769 7468  ** [https://gith
-00000bb0: 7562 2e63 6f6d 2f66 7261 6e6b 7648 6f6f  ub.com/frankvHoo
-00000bc0: 6639 332f 5469 6b54 6f6b 4c69 7665 5368  f93/TikTokLiveSh
-00000bd0: 6172 705d 2868 7474 7073 3a2f 2f67 6974  arp](https://git
-00000be0: 6875 622e 636f 6d2f 6672 616e 6b76 486f  hub.com/frankvHo
-00000bf0: 6f66 3933 2f54 696b 546f 6b4c 6976 6553  of93/TikTokLiveS
-00000c00: 6861 7270 290a 2d20 2a2a 476f 3a2a 2a20  harp).- **Go:** 
-00000c10: 5b68 7474 7073 3a2f 2f67 6974 6875 622e  [https://github.
-00000c20: 636f 6d2f 4461 7669 6e63 6962 6c65 2f67  com/Davincible/g
-00000c30: 6f74 696b 746f 6b6c 6976 655d 2868 7474  otiktoklive](htt
-00000c40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000c50: 4461 7669 6e63 6962 6c65 2f67 6f74 696b  Davincible/gotik
-00000c60: 746f 6b6c 6976 6529 0a2d 202a 2a52 7573  toklive).- **Rus
-00000c70: 743a 2a2a 205b 6874 7470 733a 2f2f 6769  t:** [https://gi
-00000c80: 7468 7562 2e63 6f6d 2f6a 7764 6576 656c  thub.com/jwdevel
-00000c90: 6f70 6572 2f54 696b 546f 6b4c 6976 6552  oper/TikTokLiveR
-00000ca0: 7573 745d 2868 7474 7073 3a2f 2f67 6974  ust](https://git
-00000cb0: 6875 622e 636f 6d2f 6a77 6465 7665 6c6f  hub.com/jwdevelo
-00000cc0: 7065 722f 5469 6b54 6f6b 4c69 7665 5275  per/TikTokLiveRu
-00000cd0: 7374 290a 0a23 2320 5461 626c 6520 6f66  st)..## Table of
-00000ce0: 2043 6f6e 7465 6e74 730a 0a2d 205b 446f   Contents..- [Do
-00000cf0: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-00000d00: 7073 3a2f 2f69 7361 6163 6b6f 6761 6e2e  ps://isaackogan.
-00000d10: 6769 7468 7562 2e69 6f2f 5469 6b54 6f6b  github.io/TikTok
-00000d20: 4c69 7665 2f29 0a2d 205b 4578 616d 706c  Live/).- [Exampl
-00000d30: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-00000d40: 7562 2e63 6f6d 2f69 7361 6163 6b6f 6761  ub.com/isaackoga
-00000d50: 6e2f 5469 6b54 6f6b 4c69 7665 2f74 7265  n/TikTokLive/tre
-00000d60: 652f 6d61 7374 6572 2f65 7861 6d70 6c65  e/master/example
-00000d70: 7329 0a2d 205b 5769 6b69 5d28 6874 7470  s).- [Wiki](http
-00000d80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
-00000d90: 7361 6163 6b6f 6761 6e2f 5469 6b54 6f6b  saackogan/TikTok
-00000da0: 4c69 7665 2f77 696b 6929 200a 2d20 5b4c  Live/wiki) .- [L
-00000db0: 6963 656e 7369 6e67 5d28 236c 6963 656e  icensing](#licen
-00000dc0: 7365 290a 2d20 5b43 6f6e 7472 6962 7574  se).- [Contribut
-00000dd0: 6f72 735d 2823 636f 6e74 7269 6275 746f  ors](#contributo
-00000de0: 7273 290a 0a23 2320 4765 7474 696e 6720  rs)..## Getting 
-00000df0: 5374 6172 7465 640a 0a31 2e20 496e 7374  Started..1. Inst
-00000e00: 616c 6c20 7468 6520 6d6f 6475 6c65 2076  all the module v
-00000e10: 6961 2070 6970 2066 726f 6d20 7468 6520  ia pip from the 
-00000e20: 5b50 7950 695d 2868 7474 7073 3a2f 2f70  [PyPi](https://p
-00000e30: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000e40: 5469 6b54 6f6b 4c69 7665 2f29 2072 6570  TikTokLive/) rep
-00000e50: 6f73 6974 6f72 790a 0a60 6060 7368 656c  ository..```shel
-00000e60: 6c20 7363 7269 7074 0a70 6970 2069 6e73  l script.pip ins
-00000e70: 7461 6c6c 2054 696b 546f 6b4c 6976 650a  tall TikTokLive.
-00000e80: 6060 600a 0a32 2e20 4372 6561 7465 2079  ```..2. Create y
-00000e90: 6f75 7220 6669 7273 7420 6368 6174 2063  our first chat c
-00000ea0: 6f6e 6e65 6374 696f 6e0a 0a60 6060 7079  onnection..```py
-00000eb0: 7468 6f6e 0a66 726f 6d20 5469 6b54 6f6b  thon.from TikTok
-00000ec0: 4c69 7665 2069 6d70 6f72 7420 5469 6b54  Live import TikT
-00000ed0: 6f6b 4c69 7665 436c 6965 6e74 0a66 726f  okLiveClient.fro
-00000ee0: 6d20 5469 6b54 6f6b 4c69 7665 2e65 7665  m TikTokLive.eve
-00000ef0: 6e74 7320 696d 706f 7274 2043 6f6e 6e65  nts import Conne
-00000f00: 6374 4576 656e 742c 2043 6f6d 6d65 6e74  ctEvent, Comment
-00000f10: 4576 656e 740a 0a23 2043 7265 6174 6520  Event..# Create 
-00000f20: 7468 6520 636c 6965 6e74 0a63 6c69 656e  the client.clien
-00000f30: 743a 2054 696b 546f 6b4c 6976 6543 6c69  t: TikTokLiveCli
-00000f40: 656e 7420 3d20 5469 6b54 6f6b 4c69 7665  ent = TikTokLive
-00000f50: 436c 6965 6e74 2875 6e69 7175 655f 6964  Client(unique_id
-00000f60: 3d22 4069 7361 6163 6b6f 677a 2229 0a0a  ="@isaackogz")..
-00000f70: 0a23 204c 6973 7465 6e20 746f 2061 6e20  .# Listen to an 
-00000f80: 6576 656e 7420 7769 7468 2061 2064 6563  event with a dec
-00000f90: 6f72 6174 6f72 210a 4063 6c69 656e 742e  orator!.@client.
-00000fa0: 6f6e 2843 6f6e 6e65 6374 4576 656e 7429  on(ConnectEvent)
-00000fb0: 0a61 7379 6e63 2064 6566 206f 6e5f 636f  .async def on_co
-00000fc0: 6e6e 6563 7428 6576 656e 743a 2043 6f6e  nnect(event: Con
-00000fd0: 6e65 6374 4576 656e 7429 3a0a 2020 2020  nectEvent):.    
-00000fe0: 7072 696e 7428 6622 436f 6e6e 6563 7465  print(f"Connecte
-00000ff0: 6420 746f 2040 7b65 7665 6e74 2e75 6e69  d to @{event.uni
-00001000: 7175 655f 6964 7d20 2852 6f6f 6d20 4944  que_id} (Room ID
-00001010: 3a20 7b63 6c69 656e 742e 726f 6f6d 5f69  : {client.room_i
-00001020: 647d 2229 0a0a 0a23 204f 722c 2061 6464  d}")...# Or, add
-00001030: 2069 7420 6d61 6e75 616c 6c79 2076 6961   it manually via
-00001040: 2022 636c 6965 6e74 2e61 6464 5f6c 6973   "client.add_lis
-00001050: 7465 6e65 7228 2922 0a61 7379 6e63 2064  tener()".async d
-00001060: 6566 206f 6e5f 636f 6d6d 656e 7428 6576  ef on_comment(ev
-00001070: 656e 743a 2043 6f6d 6d65 6e74 4576 656e  ent: CommentEven
-00001080: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-00001090: 7072 696e 7428 6622 7b65 7665 6e74 2e75  print(f"{event.u
-000010a0: 7365 722e 6e69 636b 6e61 6d65 7d20 2d3e  ser.nickname} ->
-000010b0: 207b 6576 656e 742e 636f 6d6d 656e 747d   {event.comment}
-000010c0: 2229 0a0a 0a63 6c69 656e 742e 6164 645f  ")...client.add_
-000010d0: 6c69 7374 656e 6572 2843 6f6d 6d65 6e74  listener(Comment
-000010e0: 4576 656e 742c 206f 6e5f 636f 6d6d 656e  Event, on_commen
-000010f0: 7429 0a0a 6966 205f 5f6e 616d 655f 5f20  t)..if __name__ 
-00001100: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0a20  == '__main__':. 
-00001110: 2020 2023 2052 756e 2074 6865 2063 6c69     # Run the cli
-00001120: 656e 7420 616e 6420 626c 6f63 6b20 7468  ent and block th
-00001130: 6520 6d61 696e 2074 6872 6561 640a 2020  e main thread.  
-00001140: 2020 2320 6177 6169 7420 636c 6965 6e74    # await client
-00001150: 2e73 7461 7274 2829 2074 6f20 7275 6e20  .start() to run 
-00001160: 6e6f 6e2d 626c 6f63 6b69 6e67 0a20 2020  non-blocking.   
-00001170: 2063 6c69 656e 742e 7275 6e28 290a 6060   client.run().``
-00001180: 600a 0a46 6f72 206d 6f72 6520 7175 6963  `..For more quic
-00001190: 6b73 7461 7274 2065 7861 6d70 6c65 732c  kstart examples,
-000011a0: 2073 6565 2074 6865 205b 6578 616d 706c   see the [exampl
-000011b0: 6573 2066 6f6c 6465 725d 2868 7474 7073  es folder](https
-000011c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6973  ://github.com/is
-000011d0: 6161 636b 6f67 616e 2f54 696b 546f 6b4c  aackogan/TikTokL
-000011e0: 6976 652f 7472 6565 2f6d 6173 7465 722f  ive/tree/master/
-000011f0: 6578 616d 706c 6573 290a 7072 6f76 6964  examples).provid
-00001200: 6564 2069 6e20 7468 6520 736f 7572 6365  ed in the source
-00001210: 2074 7265 652e 0a0a 2323 2050 6172 616d   tree...## Param
-00001220: 6574 6572 730a 0a7c 2050 6172 616d 204e  eters..| Param N
-00001230: 616d 6520 7c20 5265 7175 6972 6564 207c  ame | Required |
-00001240: 2044 6566 6175 6c74 207c 2044 6573 6372   Default | Descr
-00001250: 6970 7469 6f6e 2020 2020 2020 2020 2020  iption          
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001320: 2020 2020 207c 0a7c 2d2d 2d2d 2d2d 2d2d       |.|--------
-00001330: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d7c  ----|----------|
-00001340: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
-00001350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001420: 2d2d 2d2d 2d7c 0a7c 2075 6e69 7175 655f  -----|.| unique_
-00001430: 6964 2020 7c20 5965 7320 2020 2020 207c  id  | Yes      |
-00001440: 204e 2f41 2020 2020 207c 2054 6865 2075   N/A     | The u
-00001450: 6e69 7175 6520 7573 6572 6e61 6d65 206f  nique username o
-00001460: 6620 7468 6520 6272 6f61 6463 6173 7465  f the broadcaste
-00001470: 722e 2059 6f75 2063 616e 2066 696e 6420  r. You can find 
-00001480: 7468 6973 206e 616d 6520 696e 2074 6865  this name in the
-00001490: 2055 524c 206f 6620 7468 6520 7573 6572   URL of the user
-000014a0: 2e20 466f 7220 6578 616d 706c 652c 2074  . For example, t
-000014b0: 6865 2060 756e 6971 7565 5f69 6460 2066  he `unique_id` f
-000014c0: 6f72 205b 6068 7474 7073 3a2f 2f77 7777  or [`https://www
-000014d0: 2e74 696b 746f 6b2e 636f 6d2f 4069 7361  .tiktok.com/@isa
-000014e0: 6163 6b6f 677a 605d 2868 7474 7073 3a2f  ackogz`](https:/
-000014f0: 2f77 7777 2e74 696b 746f 6b2e 636f 6d2f  /www.tiktok.com/
-00001500: 4069 7361 6163 6b6f 677a 2920 776f 756c  @isaackogz) woul
-00001510: 6420 6265 2060 6973 6161 636b 6f67 7a60  d be `isaackogz`
-00001520: 2e20 2020 207c 0a7c 2077 6562 5f70 726f  .    |.| web_pro
-00001530: 7879 2020 7c20 4e6f 2020 2020 2020 207c  xy  | No       |
-00001540: 2060 4e6f 6e65 6020 207c 2054 696b 546f   `None`  | TikTo
-00001550: 6b4c 6976 6520 7375 7070 6f72 7473 2070  kLive supports p
-00001560: 726f 7879 696e 6720 4854 5450 2072 6571  roxying HTTP req
-00001570: 7565 7374 732e 2054 6869 7320 7061 7261  uests. This para
-00001580: 6d65 7465 7220 6163 6365 7074 7320 616e  meter accepts an
-00001590: 2060 6874 7470 782e 5072 6f78 7960 2e20   `httpx.Proxy`. 
-000015a0: 4e6f 7465 2074 6861 7420 6966 2079 6f75  Note that if you
-000015b0: 2064 6f20 7573 6520 6120 7072 6f78 7920   do use a proxy 
-000015c0: 796f 7520 6d61 7920 6265 2073 7562 6a65  you may be subje
-000015d0: 6374 2074 6f20 7265 6475 6365 6420 636f  ct to reduced co
-000015e0: 6e6e 6563 7469 6f6e 206c 696d 6974 7320  nnection limits 
-000015f0: 6174 2074 696d 6573 206f 6620 6869 6768  at times of high
-00001600: 206c 6f61 642e 2020 2020 2020 2020 2020   load.          
-00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001620: 2020 2020 207c 0a7c 2077 735f 7072 6f78       |.| ws_prox
-00001630: 7920 2020 7c20 4e6f 2020 2020 2020 207c  y   | No       |
-00001640: 2060 4e6f 6e65 6020 207c 2054 696b 546f   `None`  | TikTo
-00001650: 6b4c 6976 6520 7375 7070 6f72 7473 2070  kLive supports p
-00001660: 726f 7879 696e 6720 7468 6520 7765 6273  roxying the webs
-00001670: 6f63 6b65 7420 636f 6e6e 6563 7469 6f6e  ocket connection
-00001680: 2e20 5468 6973 2070 6172 616d 6574 6572  . This parameter
-00001690: 2061 6363 6570 7473 2061 6e20 6068 7474   accepts an `htt
-000016a0: 7078 2e50 726f 7879 602e 2055 7369 6e67  px.Proxy`. Using
-000016b0: 2074 6869 7320 7072 6f78 7920 7769 6c6c   this proxy will
-000016c0: 206e 6576 6572 2062 6520 7375 626a 6563   never be subjec
-000016d0: 7420 746f 2072 6564 7563 6564 2063 6f6e  t to reduced con
-000016e0: 6e65 6374 696f 6e20 6c69 6d69 7473 2e20  nection limits. 
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001720: 2020 2020 207c 0a7c 2077 6562 5f6b 7761       |.| web_kwa
-00001730: 7267 7320 7c20 4e6f 2020 2020 2020 207c  rgs | No       |
-00001740: 2060 7b7d 6020 2020 207c 2055 6e64 6572   `{}`    | Under
-00001750: 2074 6865 2073 6365 6e65 732c 2074 6865   the scenes, the
-00001760: 2054 696b 546f 6b4c 6976 6520 4854 5450   TikTokLive HTTP
-00001770: 2063 6c69 656e 7420 7573 6573 2074 6865   client uses the
-00001780: 205b 6068 7474 7078 605d 2868 7474 7073   [`httpx`](https
-00001790: 3a2f 2f67 6974 6875 622e 636f 6d2f 656e  ://github.com/en
-000017a0: 636f 6465 2f68 7474 7078 2920 6c69 6272  code/httpx) libr
-000017b0: 6172 792e 2041 7267 756d 656e 7473 2070  ary. Arguments p
-000017c0: 6173 7365 6420 746f 2060 7765 625f 6b77  assed to `web_kw
-000017d0: 6172 6773 6020 7769 6c6c 2062 6520 666f  args` will be fo
-000017e0: 7277 6172 6420 7468 6520 7468 6520 756e  rward the the un
-000017f0: 6465 726c 7969 6e67 2048 5454 5020 636c  derlying HTTP cl
-00001800: 6965 6e74 2e20 2020 2020 2020 2020 2020  ient.           
-00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001820: 2020 2020 207c 0a7c 2077 735f 6b77 6172       |.| ws_kwar
-00001830: 6773 2020 7c20 4e6f 2020 2020 2020 207c  gs  | No       |
-00001840: 2060 7b7d 6020 2020 207c 2055 6e64 6572   `{}`    | Under
-00001850: 2074 6865 2073 6365 6e65 732c 2054 696b   the scenes, Tik
-00001860: 546f 6b4c 6976 6520 7573 6573 2074 6865  TokLive uses the
-00001870: 205b 6077 6562 736f 636b 6574 7360 5d28   [`websockets`](
-00001880: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001890: 6f6d 2f70 7974 686f 6e2d 7765 6273 6f63  om/python-websoc
-000018a0: 6b65 7473 2f77 6562 736f 636b 6574 7329  kets/websockets)
-000018b0: 206c 6962 7261 7279 2074 6f20 636f 6e6e   library to conn
-000018c0: 6563 7420 746f 2054 696b 546f 6b2e 2041  ect to TikTok. A
-000018d0: 7267 756d 656e 7473 2070 6173 7365 6420  rguments passed 
-000018e0: 746f 2060 7773 5f6b 7761 7267 7360 2077  to `ws_kwargs` w
-000018f0: 696c 6c20 6265 2066 6f72 7761 7264 6564  ill be forwarded
-00001900: 2074 6f20 7468 6520 756e 6465 726c 7969   to the underlyi
-00001910: 6e67 2057 6562 536f 636b 6574 2063 6c69  ng WebSocket cli
-00001920: 656e 742e 207c 0a0a 2323 204d 6574 686f  ent. |..## Metho
-00001930: 6473 0a0a 4120 6054 696b 546f 6b4c 6976  ds..A `TikTokLiv
-00001940: 6543 6c69 656e 7460 206f 626a 6563 7420  eClient` object 
-00001950: 636f 6e74 6169 6e73 2074 6865 2066 6f6c  contains the fol
-00001960: 6c6f 7769 6e67 2069 6d70 6f72 7461 6e74  lowing important
-00001970: 206d 6574 686f 6473 3a0a 0a7c 204d 6574   methods:..| Met
-00001980: 686f 6420 4e61 6d65 2020 7c20 4e6f 7465  hod Name  | Note
-00001990: 7320 2020 7c20 4465 7363 7269 7074 696f  s   | Descriptio
-000019a0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a40: 207c 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.|------------
-00001a50: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  --|---------|---
-00001a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b00: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2072 756e  ---------|.| run
-00001b10: 2020 2020 2020 2020 2020 7c20 4e2f 4120            | N/A 
-00001b20: 2020 2020 7c20 436f 6e6e 6563 7420 746f      | Connect to
-00001b30: 2074 6865 206c 6976 6573 7472 6561 6d20   the livestream 
-00001b40: 616e 6420 626c 6f63 6b20 7468 6520 6d61  and block the ma
-00001b50: 696e 2074 6872 6561 642e 2054 6869 7320  in thread. This 
-00001b60: 6973 2062 6573 7420 666f 7220 736d 616c  is best for smal
-00001b70: 6c20 7363 7269 7074 732e 2020 2020 2020  l scripts.      
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bb0: 2020 2020 2020 2020 2020 207c 0a7c 2061             |.| a
-00001bc0: 6464 5f6c 6973 7465 6e65 7220 7c20 4e2f  dd_listener | N/
-00001bd0: 4120 2020 2020 7c20 4164 6473 2061 6e20  A     | Adds an 
-00001be0: 2a61 7379 6e63 6872 6f6e 6f75 732a 206c  *asynchronous* l
-00001bf0: 6973 7465 6e65 7220 6675 6e63 7469 6f6e  istener function
-00001c00: 2028 6f72 2c20 796f 7520 6361 6e20 6465   (or, you can de
-00001c10: 636f 7261 7465 2061 2066 756e 6374 696f  corate a functio
-00001c20: 6e20 7769 7468 2060 4063 6c69 656e 742e  n with `@client.
-00001c30: 6f6e 2822 3c65 7665 6e74 3e22 2960 2920  on("<event>")`) 
-00001c40: 616e 6420 7461 6b65 7320 7477 6f20 7061  and takes two pa
-00001c50: 7261 6d65 7465 7273 2c20 616e 2065 7665  rameters, an eve
-00001c60: 6e74 206e 616d 6520 616e 6420 7468 6520  nt name and the 
-00001c70: 7061 796c 6f61 642c 2061 6e20 4162 7374  payload, an Abst
-00001c80: 7261 6374 4576 656e 7420 7c7c 0a7c 2063  ractEvent ||.| c
-00001c90: 6f6e 6e65 6374 2020 2020 2020 7c20 6061  onnect      | `a
-00001ca0: 7379 6e63 6020 7c20 436f 6e6e 6563 7473  sync` | Connects
-00001cb0: 2074 6f20 7468 6520 7469 6b74 6f6b 206c   to the tiktok l
-00001cc0: 6976 6520 6368 6174 2077 6869 6c65 2062  ive chat while b
-00001cd0: 6c6f 636b 696e 6720 7468 6520 6375 7272  locking the curr
-00001ce0: 656e 7420 6675 7475 7265 2e20 5768 656e  ent future. When
-00001cf0: 2074 6865 2063 6f6e 6e65 6374 696f 6e20   the connection 
-00001d00: 656e 6473 2028 652e 672e 206c 6976 6573  ends (e.g. lives
-00001d10: 7472 6561 6d20 6973 206f 7665 7229 2c20  tream is over), 
-00001d20: 7468 6520 6675 7475 7265 2069 7320 7265  the future is re
-00001d30: 6c65 6173 6564 2e20 2020 2020 2020 2020  leased.         
-00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d50: 2020 207c 0a7c 2073 7461 7274 2020 2020     |.| start    
-00001d60: 2020 2020 7c20 6061 7379 6e63 6020 7c20      | `async` | 
-00001d70: 436f 6e6e 6563 7473 2074 6f20 7468 6520  Connects to the 
-00001d80: 6c69 7665 2063 6861 7420 7769 7468 6f75  live chat withou
-00001d90: 7420 626c 6f63 6b69 6e67 2074 6865 206d  t blocking the m
-00001da0: 6169 6e20 7468 7265 6164 2e20 5468 6973  ain thread. This
-00001db0: 2072 6574 7572 6e73 2061 6e20 6061 7379   returns an `asy
-00001dc0: 6e63 696f 2e54 6173 6b60 206f 626a 6563  ncio.Task` objec
-00001dd0: 7420 7769 7468 2074 6865 2063 6c69 656e  t with the clien
-00001de0: 7420 6c6f 6f70 2e20 2020 2020 2020 2020  t loop.         
+000008c0: 6e64 2069 6465 6173 2e0a 0a23 2323 2045  nd ideas...### E
+000008d0: 6e74 6572 7072 6973 6520 4163 6365 7373  nterprise Access
+000008e0: 0a0a 2d20 546f 6b65 6e73 2074 6f20 7363  ..- Tokens to sc
+000008f0: 7261 7065 2041 4e59 2054 696b 546f 6b20  rape ANY TikTok 
+00000900: 5552 4c20 2869 2e65 2e20 6665 7463 6820  URL (i.e. fetch 
+00000910: 7072 6f66 696c 6573 2c20 2076 6964 656f  profiles,  video
+00000920: 732c 2063 6f6d 6d65 6e74 732c 2065 7463  s, comments, etc
+00000930: 2e29 0a2d 2049 6e63 7265 6173 6564 2054  .).- Increased T
+00000940: 696b 546f 6b20 4c49 5645 2072 6174 6520  ikTok LIVE rate 
+00000950: 6c69 6d69 7473 2028 692e 652e 2061 6269  limits (i.e. abi
+00000960: 6c69 7479 2074 6f20 3130 3030 7320 6f66  lity to 1000s of
+00000970: 2063 6c69 656e 7473 2070 6572 2068 6f75   clients per hou
+00000980: 7229 0a0a 3c64 6976 2061 6c69 676e 3d22  r)..<div align="
+00000990: 6c65 6674 223e 0a20 2020 203c 6120 6872  left">.    <a hr
+000009a0: 6566 3d22 6874 7470 733a 2f2f 6575 6c65  ef="https://eule
+000009b0: 7273 7472 6561 6d2e 636f 6d22 2074 6172  rstream.com" tar
+000009c0: 6765 743d 225f 626c 616e 6b22 3e0a 2020  get="_blank">.  
+000009d0: 2020 2020 2020 3c64 6976 3e0a 2020 2020        <div>.    
+000009e0: 2020 2020 2020 2020 3c62 3e45 756c 6572          <b>Euler
+000009f0: 7374 7265 616d 3c2f 623e 206f 6666 6572  stream</b> offer
+00000a00: 7320 7061 6964 2070 6c61 6e73 2066 6f72  s paid plans for
+00000a10: 2065 6e74 6572 7072 6973 6573 2066 6f72   enterprises for
+00000a20: 2069 6e63 7265 6173 6564 2054 696b 546f   increased TikTo
+00000a30: 6b4c 6976 6520 6163 6365 7373 2026 2054  kLive access & T
+00000a40: 696b 546f 6b20 4150 4920 746f 6b65 6e73  ikTok API tokens
+00000a50: 2066 6f72 2064 6174 6120 636f 6c6c 6563   for data collec
+00000a60: 7469 6f6e 0a20 2020 2020 2020 203c 2f64  tion.        </d
+00000a70: 6976 3e0a 2020 2020 2020 2020 3c62 722f  iv>.        <br/
+00000a80: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
+00000a90: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+00000aa0: 7562 2e63 6f6d 2f69 7361 6163 6b6f 6761  ub.com/isaackoga
+00000ab0: 6e2f 5469 6b54 6f6b 4c69 7665 2f61 7373  n/TikTokLive/ass
+00000ac0: 6574 732f 3635 3836 3931 3036 2f62 3536  ets/65869106/b56
+00000ad0: 6365 6638 392d 3564 3837 2d34 6632 662d  cef89-5d87-4f2f-
+00000ae0: 6163 3365 2d30 3638 3561 6632 3162 3238  ac3e-0685af21b28
+00000af0: 6429 2220 7769 6474 683d 2231 3030 2220  d)" width="100" 
+00000b00: 616c 743d 2245 756c 6572 7374 7265 616d  alt="Eulerstream
+00000b10: 223e 0a20 2020 203c 2f61 3e0a 3c2f 6469  ">.    </a>.</di
+00000b20: 763e 0a0a 2323 2320 436f 6e73 6964 6572  v>..### Consider
+00000b30: 2044 6f6e 6174 696e 6720 3c33 0a0a 4927   Donating <3..I'
+00000b40: 6d20 6120 326e 642d 7965 6172 2042 696f  m a 2nd-year Bio
+00000b50: 6c6f 6779 2073 7475 6465 6e74 2069 6e20  logy student in 
+00000b60: 756e 6976 6572 7369 7479 2077 686f 206c  university who l
+00000b70: 696b 6573 2074 6f20 7072 6f67 7261 6d20  ikes to program 
+00000b80: 666f 7220 6675 6e2e 2050 6c65 6173 6520  for fun. Please 
+00000b90: 636f 6e73 6964 6572 2073 7570 706f 7274  consider support
+00000ba0: 696e 6720 6465 7665 6c6f 706d 656e 740a  ing development.
+00000bb0: 7468 726f 7567 6820 6120 736d 616c 6c20  through a small 
+00000bc0: 646f 6e61 7469 6f6e 2061 7420 5b68 7474  donation at [htt
+00000bd0: 7073 3a2f 2f77 7777 2e62 7579 6d65 6163  ps://www.buymeac
+00000be0: 6f66 6665 652e 636f 6d2f 6973 6161 636b  offee.com/isaack
+00000bf0: 6f67 616e 5d28 6874 7470 733a 2f2f 7777  ogan](https://ww
+00000c00: 772e 6275 796d 6561 636f 6666 6565 2e63  w.buymeacoffee.c
+00000c10: 6f6d 2f69 7361 6163 6b6f 6761 6e29 2e20  om/isaackogan). 
+00000c20: 416e 7974 6869 6e67 0a79 6f75 2063 616e  Anything.you can
+00000c30: 206f 6666 6572 2077 696c 6c20 676f 2074   offer will go t
+00000c40: 6f77 6172 6473 2073 6368 6f6f 6c20 2620  owards school & 
+00000c50: 6465 7665 6c6f 706d 656e 7420 636f 7374  development cost
+00000c60: 7320 666f 7220 5469 6b54 6f6b 4c69 7665  s for TikTokLive
+00000c70: 2c20 7768 6963 6820 6861 7320 7461 6b65  , which has take
+00000c80: 6e20 6875 6e64 7265 6473 206f 6620 686f  n hundreds of ho
+00000c90: 7572 7320 6f66 2074 696d 6520 746f 2062  urs of time to b
+00000ca0: 7569 6c64 2e0a 0a23 2323 204f 7468 6572  uild...### Other
+00000cb0: 204c 616e 6775 6167 6573 0a0a 5469 6b54   Languages..TikT
+00000cc0: 6f6b 4c69 7665 2069 7320 6176 6169 6c61  okLive is availa
+00000cd0: 626c 6520 696e 2073 6576 6572 616c 2061  ble in several a
+00000ce0: 6c74 6572 6e61 7465 2070 726f 6772 616d  lternate program
+00000cf0: 6d69 6e67 206c 616e 6775 6167 6573 3a0a  ming languages:.
+00000d00: 0a2d 202a 2a4e 6f64 652e 4a53 3a2a 2a20  .- **Node.JS:** 
+00000d10: 5b68 7474 7073 3a2f 2f67 6974 6875 622e  [https://github.
+00000d20: 636f 6d2f 7a65 726f 6479 7472 6173 682f  com/zerodytrash/
+00000d30: 5469 6b54 6f6b 2d4c 6976 652d 436f 6e6e  TikTok-Live-Conn
+00000d40: 6563 746f 725d 2868 7474 7073 3a2f 2f67  ector](https://g
+00000d50: 6974 6875 622e 636f 6d2f 7a65 726f 6479  ithub.com/zerody
+00000d60: 7472 6173 682f 5469 6b54 6f6b 2d4c 6976  trash/TikTok-Liv
+00000d70: 652d 436f 6e6e 6563 746f 7229 0a2d 202a  e-Connector).- *
+00000d80: 2a4a 6176 613a 2a2a 205b 6874 7470 733a  *Java:** [https:
+00000d90: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7764  //github.com/jwd
+00000da0: 6576 656c 6f70 6572 2f54 696b 546f 6b2d  eveloper/TikTok-
+00000db0: 4c69 7665 2d4a 6176 615d 2868 7474 7073  Live-Java](https
+00000dc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a77  ://github.com/jw
+00000dd0: 6465 7665 6c6f 7065 722f 5469 6b54 6f6b  developer/TikTok
+00000de0: 2d4c 6976 652d 4a61 7661 290a 2d20 2a2a  -Live-Java).- **
+00000df0: 4323 2f55 6e69 7479 3a2a 2a20 5b68 7474  C#/Unity:** [htt
+00000e00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000e10: 6672 616e 6b76 486f 6f66 3933 2f54 696b  frankvHoof93/Tik
+00000e20: 546f 6b4c 6976 6553 6861 7270 5d28 6874  TokLiveSharp](ht
+00000e30: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000e40: 2f66 7261 6e6b 7648 6f6f 6639 332f 5469  /frankvHoof93/Ti
+00000e50: 6b54 6f6b 4c69 7665 5368 6172 7029 0a2d  kTokLiveSharp).-
+00000e60: 202a 2a47 6f3a 2a2a 205b 6874 7470 733a   **Go:** [https:
+00000e70: 2f2f 6769 7468 7562 2e63 6f6d 2f44 6176  //github.com/Dav
+00000e80: 696e 6369 626c 652f 676f 7469 6b74 6f6b  incible/gotiktok
+00000e90: 6c69 7665 5d28 6874 7470 733a 2f2f 6769  live](https://gi
+00000ea0: 7468 7562 2e63 6f6d 2f44 6176 696e 6369  thub.com/Davinci
+00000eb0: 626c 652f 676f 7469 6b74 6f6b 6c69 7665  ble/gotiktoklive
+00000ec0: 290a 2d20 2a2a 5275 7374 3a2a 2a20 5b68  ).- **Rust:** [h
+00000ed0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ee0: 6d2f 6a77 6465 7665 6c6f 7065 722f 5469  m/jwdeveloper/Ti
+00000ef0: 6b54 6f6b 4c69 7665 5275 7374 5d28 6874  kTokLiveRust](ht
+00000f00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000f10: 2f6a 7764 6576 656c 6f70 6572 2f54 696b  /jwdeveloper/Tik
+00000f20: 546f 6b4c 6976 6552 7573 7429 0a0a 2323  TokLiveRust)..##
+00000f30: 2054 6162 6c65 206f 6620 436f 6e74 656e   Table of Conten
+00000f40: 7473 0a0a 2d20 5b44 6f63 756d 656e 7461  ts..- [Documenta
+00000f50: 7469 6f6e 5d28 6874 7470 733a 2f2f 6973  tion](https://is
+00000f60: 6161 636b 6f67 616e 2e67 6974 6875 622e  aackogan.github.
+00000f70: 696f 2f54 696b 546f 6b4c 6976 652f 290a  io/TikTokLive/).
+00000f80: 2d20 5b45 7861 6d70 6c65 735d 2868 7474  - [Examples](htt
+00000f90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000fa0: 6973 6161 636b 6f67 616e 2f54 696b 546f  isaackogan/TikTo
+00000fb0: 6b4c 6976 652f 7472 6565 2f6d 6173 7465  kLive/tree/maste
+00000fc0: 722f 6578 616d 706c 6573 290a 2d20 5b57  r/examples).- [W
+00000fd0: 696b 695d 2868 7474 7073 3a2f 2f67 6974  iki](https://git
+00000fe0: 6875 622e 636f 6d2f 6973 6161 636b 6f67  hub.com/isaackog
+00000ff0: 616e 2f54 696b 546f 6b4c 6976 652f 7769  an/TikTokLive/wi
+00001000: 6b69 2920 0a2d 205b 4c69 6365 6e73 696e  ki) .- [Licensin
+00001010: 675d 2823 6c69 6365 6e73 6529 0a2d 205b  g](#license).- [
+00001020: 436f 6e74 7269 6275 746f 7273 5d28 2363  Contributors](#c
+00001030: 6f6e 7472 6962 7574 6f72 7329 0a0a 2323  ontributors)..##
+00001040: 2047 6574 7469 6e67 2053 7461 7274 6564   Getting Started
+00001050: 0a0a 312e 2049 6e73 7461 6c6c 2074 6865  ..1. Install the
+00001060: 206d 6f64 756c 6520 7669 6120 7069 7020   module via pip 
+00001070: 6672 6f6d 2074 6865 205b 5079 5069 5d28  from the [PyPi](
+00001080: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00001090: 2f70 726f 6a65 6374 2f54 696b 546f 6b4c  /project/TikTokL
+000010a0: 6976 652f 2920 7265 706f 7369 746f 7279  ive/) repository
+000010b0: 0a0a 6060 6073 6865 6c6c 2073 6372 6970  ..```shell scrip
+000010c0: 740a 7069 7020 696e 7374 616c 6c20 5469  t.pip install Ti
+000010d0: 6b54 6f6b 4c69 7665 0a60 6060 0a0a 322e  kTokLive.```..2.
+000010e0: 2043 7265 6174 6520 796f 7572 2066 6972   Create your fir
+000010f0: 7374 2063 6861 7420 636f 6e6e 6563 7469  st chat connecti
+00001100: 6f6e 0a0a 6060 6070 7974 686f 6e0a 6672  on..```python.fr
+00001110: 6f6d 2054 696b 546f 6b4c 6976 6520 696d  om TikTokLive im
+00001120: 706f 7274 2054 696b 546f 6b4c 6976 6543  port TikTokLiveC
+00001130: 6c69 656e 740a 6672 6f6d 2054 696b 546f  lient.from TikTo
+00001140: 6b4c 6976 652e 6576 656e 7473 2069 6d70  kLive.events imp
+00001150: 6f72 7420 436f 6e6e 6563 7445 7665 6e74  ort ConnectEvent
+00001160: 2c20 436f 6d6d 656e 7445 7665 6e74 0a0a  , CommentEvent..
+00001170: 2320 4372 6561 7465 2074 6865 2063 6c69  # Create the cli
+00001180: 656e 740a 636c 6965 6e74 3a20 5469 6b54  ent.client: TikT
+00001190: 6f6b 4c69 7665 436c 6965 6e74 203d 2054  okLiveClient = T
+000011a0: 696b 546f 6b4c 6976 6543 6c69 656e 7428  ikTokLiveClient(
+000011b0: 756e 6971 7565 5f69 643d 2240 6973 6161  unique_id="@isaa
+000011c0: 636b 6f67 7a22 290a 0a0a 2320 4c69 7374  ckogz")...# List
+000011d0: 656e 2074 6f20 616e 2065 7665 6e74 2077  en to an event w
+000011e0: 6974 6820 6120 6465 636f 7261 746f 7221  ith a decorator!
+000011f0: 0a40 636c 6965 6e74 2e6f 6e28 436f 6e6e  .@client.on(Conn
+00001200: 6563 7445 7665 6e74 290a 6173 796e 6320  ectEvent).async 
+00001210: 6465 6620 6f6e 5f63 6f6e 6e65 6374 2865  def on_connect(e
+00001220: 7665 6e74 3a20 436f 6e6e 6563 7445 7665  vent: ConnectEve
+00001230: 6e74 293a 0a20 2020 2070 7269 6e74 2866  nt):.    print(f
+00001240: 2243 6f6e 6e65 6374 6564 2074 6f20 407b  "Connected to @{
+00001250: 6576 656e 742e 756e 6971 7565 5f69 647d  event.unique_id}
+00001260: 2028 526f 6f6d 2049 443a 207b 636c 6965   (Room ID: {clie
+00001270: 6e74 2e72 6f6f 6d5f 6964 7d22 290a 0a0a  nt.room_id}")...
+00001280: 2320 4f72 2c20 6164 6420 6974 206d 616e  # Or, add it man
+00001290: 7561 6c6c 7920 7669 6120 2263 6c69 656e  ually via "clien
+000012a0: 742e 6164 645f 6c69 7374 656e 6572 2829  t.add_listener()
+000012b0: 220a 6173 796e 6320 6465 6620 6f6e 5f63  ".async def on_c
+000012c0: 6f6d 6d65 6e74 2865 7665 6e74 3a20 436f  omment(event: Co
+000012d0: 6d6d 656e 7445 7665 6e74 2920 2d3e 204e  mmentEvent) -> N
+000012e0: 6f6e 653a 0a20 2020 2070 7269 6e74 2866  one:.    print(f
+000012f0: 227b 6576 656e 742e 7573 6572 2e6e 6963  "{event.user.nic
+00001300: 6b6e 616d 657d 202d 3e20 7b65 7665 6e74  kname} -> {event
+00001310: 2e63 6f6d 6d65 6e74 7d22 290a 0a0a 636c  .comment}")...cl
+00001320: 6965 6e74 2e61 6464 5f6c 6973 7465 6e65  ient.add_listene
+00001330: 7228 436f 6d6d 656e 7445 7665 6e74 2c20  r(CommentEvent, 
+00001340: 6f6e 5f63 6f6d 6d65 6e74 290a 0a69 6620  on_comment)..if 
+00001350: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+00001360: 6169 6e5f 5f27 3a0a 2020 2020 2320 5275  ain__':.    # Ru
+00001370: 6e20 7468 6520 636c 6965 6e74 2061 6e64  n the client and
+00001380: 2062 6c6f 636b 2074 6865 206d 6169 6e20   block the main 
+00001390: 7468 7265 6164 0a20 2020 2023 2061 7761  thread.    # awa
+000013a0: 6974 2063 6c69 656e 742e 7374 6172 7428  it client.start(
+000013b0: 2920 746f 2072 756e 206e 6f6e 2d62 6c6f  ) to run non-blo
+000013c0: 636b 696e 670a 2020 2020 636c 6965 6e74  cking.    client
+000013d0: 2e72 756e 2829 0a60 6060 0a0a 466f 7220  .run().```..For 
+000013e0: 6d6f 7265 2071 7569 636b 7374 6172 7420  more quickstart 
+000013f0: 6578 616d 706c 6573 2c20 7365 6520 7468  examples, see th
+00001400: 6520 5b65 7861 6d70 6c65 7320 666f 6c64  e [examples fold
+00001410: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
+00001420: 7562 2e63 6f6d 2f69 7361 6163 6b6f 6761  ub.com/isaackoga
+00001430: 6e2f 5469 6b54 6f6b 4c69 7665 2f74 7265  n/TikTokLive/tre
+00001440: 652f 6d61 7374 6572 2f65 7861 6d70 6c65  e/master/example
+00001450: 7329 0a70 726f 7669 6465 6420 696e 2074  s).provided in t
+00001460: 6865 2073 6f75 7263 6520 7472 6565 2e0a  he source tree..
+00001470: 0a23 2320 5061 7261 6d65 7465 7273 0a0a  .## Parameters..
+00001480: 7c20 5061 7261 6d20 4e61 6d65 207c 2052  | Param Name | R
+00001490: 6571 7569 7265 6420 7c20 4465 6661 756c  equired | Defaul
+000014a0: 7420 7c20 4465 7363 7269 7074 696f 6e20  t | Description 
+000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001580: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  |------------|--
+00001590: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
+000015a0: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
+000015b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000015c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000015d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000015e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000015f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
+00001680: 7c20 756e 6971 7565 5f69 6420 207c 2059  | unique_id  | Y
+00001690: 6573 2020 2020 2020 7c20 4e2f 4120 2020  es      | N/A   
+000016a0: 2020 7c20 5468 6520 756e 6971 7565 2075    | The unique u
+000016b0: 7365 726e 616d 6520 6f66 2074 6865 2062  sername of the b
+000016c0: 726f 6164 6361 7374 6572 2e20 596f 7520  roadcaster. You 
+000016d0: 6361 6e20 6669 6e64 2074 6869 7320 6e61  can find this na
+000016e0: 6d65 2069 6e20 7468 6520 5552 4c20 6f66  me in the URL of
+000016f0: 2074 6865 2075 7365 722e 2046 6f72 2065   the user. For e
+00001700: 7861 6d70 6c65 2c20 7468 6520 6075 6e69  xample, the `uni
+00001710: 7175 655f 6964 6020 666f 7220 5b60 6874  que_id` for [`ht
+00001720: 7470 733a 2f2f 7777 772e 7469 6b74 6f6b  tps://www.tiktok
+00001730: 2e63 6f6d 2f40 6973 6161 636b 6f67 7a60  .com/@isaackogz`
+00001740: 5d28 6874 7470 733a 2f2f 7777 772e 7469  ](https://www.ti
+00001750: 6b74 6f6b 2e63 6f6d 2f40 6973 6161 636b  ktok.com/@isaack
+00001760: 6f67 7a29 2077 6f75 6c64 2062 6520 6069  ogz) would be `i
+00001770: 7361 6163 6b6f 677a 602e 2020 2020 7c0a  saackogz`.    |.
+00001780: 7c20 7765 625f 7072 6f78 7920 207c 204e  | web_proxy  | N
+00001790: 6f20 2020 2020 2020 7c20 604e 6f6e 6560  o       | `None`
+000017a0: 2020 7c20 5469 6b54 6f6b 4c69 7665 2073    | TikTokLive s
+000017b0: 7570 706f 7274 7320 7072 6f78 7969 6e67  upports proxying
+000017c0: 2048 5454 5020 7265 7175 6573 7473 2e20   HTTP requests. 
+000017d0: 5468 6973 2070 6172 616d 6574 6572 2061  This parameter a
+000017e0: 6363 6570 7473 2061 6e20 6068 7474 7078  ccepts an `httpx
+000017f0: 2e50 726f 7879 602e 204e 6f74 6520 7468  .Proxy`. Note th
+00001800: 6174 2069 6620 796f 7520 646f 2075 7365  at if you do use
+00001810: 2061 2070 726f 7879 2079 6f75 206d 6179   a proxy you may
+00001820: 2062 6520 7375 626a 6563 7420 746f 2072   be subject to r
+00001830: 6564 7563 6564 2063 6f6e 6e65 6374 696f  educed connectio
+00001840: 6e20 6c69 6d69 7473 2061 7420 7469 6d65  n limits at time
+00001850: 7320 6f66 2068 6967 6820 6c6f 6164 2e20  s of high load. 
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001880: 7c20 7773 5f70 726f 7879 2020 207c 204e  | ws_proxy   | N
+00001890: 6f20 2020 2020 2020 7c20 604e 6f6e 6560  o       | `None`
+000018a0: 2020 7c20 5469 6b54 6f6b 4c69 7665 2073    | TikTokLive s
+000018b0: 7570 706f 7274 7320 7072 6f78 7969 6e67  upports proxying
+000018c0: 2074 6865 2077 6562 736f 636b 6574 2063   the websocket c
+000018d0: 6f6e 6e65 6374 696f 6e2e 2054 6869 7320  onnection. This 
+000018e0: 7061 7261 6d65 7465 7220 6163 6365 7074  parameter accept
+000018f0: 7320 616e 2060 6874 7470 782e 5072 6f78  s an `httpx.Prox
+00001900: 7960 2e20 5573 696e 6720 7468 6973 2070  y`. Using this p
+00001910: 726f 7879 2077 696c 6c20 6e65 7665 7220  roxy will never 
+00001920: 6265 2073 7562 6a65 6374 2074 6f20 7265  be subject to re
+00001930: 6475 6365 6420 636f 6e6e 6563 7469 6f6e  duced connection
+00001940: 206c 696d 6974 732e 2020 2020 2020 2020   limits.        
+00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001980: 7c20 7765 625f 6b77 6172 6773 207c 204e  | web_kwargs | N
+00001990: 6f20 2020 2020 2020 7c20 607b 7d60 2020  o       | `{}`  
+000019a0: 2020 7c20 556e 6465 7220 7468 6520 7363    | Under the sc
+000019b0: 656e 6573 2c20 7468 6520 5469 6b54 6f6b  enes, the TikTok
+000019c0: 4c69 7665 2048 5454 5020 636c 6965 6e74  Live HTTP client
+000019d0: 2075 7365 7320 7468 6520 5b60 6874 7470   uses the [`http
+000019e0: 7860 5d28 6874 7470 733a 2f2f 6769 7468  x`](https://gith
+000019f0: 7562 2e63 6f6d 2f65 6e63 6f64 652f 6874  ub.com/encode/ht
+00001a00: 7470 7829 206c 6962 7261 7279 2e20 4172  tpx) library. Ar
+00001a10: 6775 6d65 6e74 7320 7061 7373 6564 2074  guments passed t
+00001a20: 6f20 6077 6562 5f6b 7761 7267 7360 2077  o `web_kwargs` w
+00001a30: 696c 6c20 6265 2066 6f72 7761 7264 2074  ill be forward t
+00001a40: 6865 2074 6865 2075 6e64 6572 6c79 696e  he the underlyin
+00001a50: 6720 4854 5450 2063 6c69 656e 742e 2020  g HTTP client.  
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001a80: 7c20 7773 5f6b 7761 7267 7320 207c 204e  | ws_kwargs  | N
+00001a90: 6f20 2020 2020 2020 7c20 607b 7d60 2020  o       | `{}`  
+00001aa0: 2020 7c20 556e 6465 7220 7468 6520 7363    | Under the sc
+00001ab0: 656e 6573 2c20 5469 6b54 6f6b 4c69 7665  enes, TikTokLive
+00001ac0: 2075 7365 7320 7468 6520 5b60 7765 6273   uses the [`webs
+00001ad0: 6f63 6b65 7473 605d 2868 7474 7073 3a2f  ockets`](https:/
+00001ae0: 2f67 6974 6875 622e 636f 6d2f 7079 7468  /github.com/pyth
+00001af0: 6f6e 2d77 6562 736f 636b 6574 732f 7765  on-websockets/we
+00001b00: 6273 6f63 6b65 7473 2920 6c69 6272 6172  bsockets) librar
+00001b10: 7920 746f 2063 6f6e 6e65 6374 2074 6f20  y to connect to 
+00001b20: 5469 6b54 6f6b 2e20 4172 6775 6d65 6e74  TikTok. Argument
+00001b30: 7320 7061 7373 6564 2074 6f20 6077 735f  s passed to `ws_
+00001b40: 6b77 6172 6773 6020 7769 6c6c 2062 6520  kwargs` will be 
+00001b50: 666f 7277 6172 6465 6420 746f 2074 6865  forwarded to the
+00001b60: 2075 6e64 6572 6c79 696e 6720 5765 6253   underlying WebS
+00001b70: 6f63 6b65 7420 636c 6965 6e74 2e20 7c0a  ocket client. |.
+00001b80: 0a23 2320 4d65 7468 6f64 730a 0a41 2060  .## Methods..A `
+00001b90: 5469 6b54 6f6b 4c69 7665 436c 6965 6e74  TikTokLiveClient
+00001ba0: 6020 6f62 6a65 6374 2063 6f6e 7461 696e  ` object contain
+00001bb0: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
+00001bc0: 696d 706f 7274 616e 7420 6d65 7468 6f64  important method
+00001bd0: 733a 0a0a 7c20 4d65 7468 6f64 204e 616d  s:..| Method Nam
+00001be0: 6520 207c 204e 6f74 6573 2020 207c 2044  e  | Notes   | D
+00001bf0: 6573 6372 6970 7469 6f6e 2020 2020 2020  escription      
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c90: 2020 2020 2020 2020 2020 7c0a 7c2d 2d2d            |.|---
+00001ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
+00001cb0: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
+00001cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d60: 2d2d 7c0a 7c20 7275 6e20 2020 2020 2020  --|.| run       
+00001d70: 2020 207c 204e 2f41 2020 2020 207c 2043     | N/A     | C
+00001d80: 6f6e 6e65 6374 2074 6f20 7468 6520 6c69  onnect to the li
+00001d90: 7665 7374 7265 616d 2061 6e64 2062 6c6f  vestream and blo
+00001da0: 636b 2074 6865 206d 6169 6e20 7468 7265  ck the main thre
+00001db0: 6164 2e20 5468 6973 2069 7320 6265 7374  ad. This is best
+00001dc0: 2066 6f72 2073 6d61 6c6c 2073 6372 6970   for small scrip
+00001dd0: 7473 2e20 2020 2020 2020 2020 2020 2020  ts.             
+00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e10: 2020 2020 2020 2020 2020 207c 0a7c 2064             |.| d
-00001e20: 6973 636f 6e6e 6563 7420 2020 7c20 6061  isconnect   | `a
-00001e30: 7379 6e63 6020 7c20 4469 7363 6f6e 6e65  sync` | Disconne
-00001e40: 6374 7320 7468 6520 636c 6965 6e74 2066  cts the client f
-00001e50: 726f 6d20 7468 6520 7765 6273 6f63 6b65  rom the websocke
-00001e60: 7420 6772 6163 6566 756c 6c79 2c20 7072  t gracefully, pr
-00001e70: 6f63 6573 7369 6e67 2072 656d 6169 6e69  ocessing remaini
-00001e80: 6e67 2065 7665 6e74 7320 6265 666f 7265  ng events before
-00001e90: 2065 6e64 696e 6720 7468 6520 636c 6965   ending the clie
-00001ea0: 6e74 206c 6f6f 702e 2020 2020 2020 2020  nt loop.        
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2020 207c 0a0a 2323 2050 726f 7065 7274     |..## Propert
-00001ef0: 6965 730a 0a41 2060 5469 6b54 6f6b 4c69  ies..A `TikTokLi
-00001f00: 7665 436c 6965 6e74 6020 6f62 6a65 6374  veClient` object
-00001f10: 2063 6f6e 7461 696e 7320 7468 6520 666f   contains the fo
-00001f20: 6c6c 6f77 696e 6720 696d 706f 7274 616e  llowing importan
-00001f30: 7420 7072 6f70 6572 7469 6573 3a0a 0a7c  t properties:..|
-00001f40: 2041 7474 7269 6275 7465 204e 616d 6520   Attribute Name 
-00001f50: 7c20 4465 7363 7269 7074 696f 6e20 2020  | Description   
-00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e10: 2020 2020 7c0a 7c20 6164 645f 6c69 7374      |.| add_list
+00001e20: 656e 6572 207c 204e 2f41 2020 2020 207c  ener | N/A     |
+00001e30: 2041 6464 7320 616e 202a 6173 796e 6368   Adds an *asynch
+00001e40: 726f 6e6f 7573 2a20 6c69 7374 656e 6572  ronous* listener
+00001e50: 2066 756e 6374 696f 6e20 286f 722c 2079   function (or, y
+00001e60: 6f75 2063 616e 2064 6563 6f72 6174 6520  ou can decorate 
+00001e70: 6120 6675 6e63 7469 6f6e 2077 6974 6820  a function with 
+00001e80: 6040 636c 6965 6e74 2e6f 6e28 223c 6576  `@client.on("<ev
+00001e90: 656e 743e 2229 6029 2061 6e64 2074 616b  ent>")`) and tak
+00001ea0: 6573 2074 776f 2070 6172 616d 6574 6572  es two parameter
+00001eb0: 732c 2061 6e20 6576 656e 7420 6e61 6d65  s, an event name
+00001ec0: 2061 6e64 2074 6865 2070 6179 6c6f 6164   and the payload
+00001ed0: 2c20 616e 2041 6273 7472 6163 7445 7665  , an AbstractEve
+00001ee0: 6e74 207c 7c0a 7c20 636f 6e6e 6563 7420  nt ||.| connect 
+00001ef0: 2020 2020 207c 2060 6173 796e 6360 207c       | `async` |
+00001f00: 2043 6f6e 6e65 6374 7320 746f 2074 6865   Connects to the
+00001f10: 2074 696b 746f 6b20 6c69 7665 2063 6861   tiktok live cha
+00001f20: 7420 7768 696c 6520 626c 6f63 6b69 6e67  t while blocking
+00001f30: 2074 6865 2063 7572 7265 6e74 2066 7574   the current fut
+00001f40: 7572 652e 2057 6865 6e20 7468 6520 636f  ure. When the co
+00001f50: 6e6e 6563 7469 6f6e 2065 6e64 7320 2865  nnection ends (e
+00001f60: 2e67 2e20 6c69 7665 7374 7265 616d 2069  .g. livestream i
+00001f70: 7320 6f76 6572 292c 2074 6865 2066 7574  s over), the fut
+00001f80: 7572 6520 6973 2072 656c 6561 7365 642e  ure is released.
 00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fe0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00001ff0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
-00002000: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
-00002010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-000020a0: 0a7c 2072 6f6f 6d5f 6964 2020 2020 2020  .| room_id      
-000020b0: 2020 7c20 5468 6520 526f 6f6d 2049 4420    | The Room ID 
-000020c0: 6f66 2074 6865 206c 6976 6573 7472 6561  of the livestrea
-000020d0: 6d20 726f 6f6d 2074 6865 2063 6c69 656e  m room the clien
-000020e0: 7420 6973 2063 7572 7265 6e74 6c79 2063  t is currently c
-000020f0: 6f6e 6e65 6374 6564 2074 6f2e 2020 2020  onnected to.    
-00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fa0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00001fb0: 7374 6172 7420 2020 2020 2020 207c 2060  start        | `
+00001fc0: 6173 796e 6360 207c 2043 6f6e 6e65 6374  async` | Connect
+00001fd0: 7320 746f 2074 6865 206c 6976 6520 6368  s to the live ch
+00001fe0: 6174 2077 6974 686f 7574 2062 6c6f 636b  at without block
+00001ff0: 696e 6720 7468 6520 6d61 696e 2074 6872  ing the main thr
+00002000: 6561 642e 2054 6869 7320 7265 7475 726e  ead. This return
+00002010: 7320 616e 2060 6173 796e 6369 6f2e 5461  s an `asyncio.Ta
+00002020: 736b 6020 6f62 6a65 6374 2077 6974 6820  sk` object with 
+00002030: 7468 6520 636c 6965 6e74 206c 6f6f 702e  the client loop.
+00002040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002070: 2020 2020 7c0a 7c20 6469 7363 6f6e 6e65      |.| disconne
+00002080: 6374 2020 207c 2060 6173 796e 6360 207c  ct   | `async` |
+00002090: 2044 6973 636f 6e6e 6563 7473 2074 6865   Disconnects the
+000020a0: 2063 6c69 656e 7420 6672 6f6d 2074 6865   client from the
+000020b0: 2077 6562 736f 636b 6574 2067 7261 6365   websocket grace
+000020c0: 6675 6c6c 792c 2070 726f 6365 7373 696e  fully, processin
+000020d0: 6720 7265 6d61 696e 696e 6720 6576 656e  g remaining even
+000020e0: 7473 2062 6566 6f72 6520 656e 6469 6e67  ts before ending
+000020f0: 2074 6865 2063 6c69 656e 7420 6c6f 6f70   the client loop
+00002100: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
 00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002150: 7c0a 7c20 7765 6220 2020 2020 2020 2020  |.| web         
-00002160: 2020 207c 2054 6865 2054 696b 546f 6b20     | The TikTok 
-00002170: 4854 5450 2063 6c69 656e 742e 2054 6869  HTTP client. Thi
-00002180: 7320 636c 6965 6e74 2068 6173 2061 206c  s client has a l
-00002190: 6f74 206f 6620 7573 6566 756c 2072 6f75  ot of useful rou
-000021a0: 7465 7320 796f 7520 7368 6f75 6c64 2065  tes you should e
-000021b0: 7870 6c6f 7265 2120 2020 2020 2020 2020  xplore!         
+00002130: 2020 2020 2020 2020 2020 2020 7c0a 0a23              |..#
+00002140: 2320 5072 6f70 6572 7469 6573 0a0a 4120  # Properties..A 
+00002150: 6054 696b 546f 6b4c 6976 6543 6c69 656e  `TikTokLiveClien
+00002160: 7460 206f 626a 6563 7420 636f 6e74 6169  t` object contai
+00002170: 6e73 2074 6865 2066 6f6c 6c6f 7769 6e67  ns the following
+00002180: 2069 6d70 6f72 7461 6e74 2070 726f 7065   important prope
+00002190: 7274 6965 733a 0a0a 7c20 4174 7472 6962  rties:..| Attrib
+000021a0: 7574 6520 4e61 6d65 207c 2044 6573 6372  ute Name | Descr
+000021b0: 6970 7469 6f6e 2020 2020 2020 2020 2020  iption          
 000021c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 207c 0a7c 2063 6f6e 6e65 6374 6564 2020   |.| connected  
-00002210: 2020 2020 7c20 5768 6574 6865 7220 796f      | Whether yo
-00002220: 7520 6172 6520 6375 7272 656e 746c 7920  u are currently 
-00002230: 636f 6e6e 6563 7465 6420 746f 2074 6865  connected to the
-00002240: 206c 6976 6573 7472 6561 6d2e 2020 2020   livestream.    
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022b0: 2020 7c0a 7c20 6c6f 6767 6572 2020 2020    |.| logger    
-000022c0: 2020 2020 207c 2054 6865 2069 6e74 6572       | The inter
-000022d0: 6e61 6c20 6c6f 6767 6572 2075 7365 6420  nal logger used 
-000022e0: 6279 2054 696b 546f 6b4c 6976 652e 2059  by TikTokLive. Y
-000022f0: 6f75 2063 616e 2075 7365 2060 636c 6965  ou can use `clie
-00002300: 6e74 2e6c 6f67 6765 722e 7365 744c 6576  nt.logger.setLev
-00002310: 656c 282e 2e2e 2960 206d 6574 686f 6420  el(...)` method 
-00002320: 746f 2065 6e61 626c 6520 636c 6965 6e74  to enable client
-00002330: 2064 6562 7567 2e20 2020 2020 2020 2020   debug.         
-00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002360: 2020 207c 0a7c 2072 6f6f 6d5f 696e 666f     |.| room_info
-00002370: 2020 2020 2020 7c20 526f 6f6d 2069 6e66        | Room inf
-00002380: 6f72 6d61 7469 6f6e 2074 6861 7420 6973  ormation that is
-00002390: 2072 6574 7269 6576 6564 2066 726f 6d20   retrieved from 
-000023a0: 5469 6b54 6f6b 2077 6865 6e20 796f 7520  TikTok when you 
-000023b0: 7573 6520 6120 636f 6e6e 6563 7469 6f6e  use a connection
-000023c0: 206d 6574 686f 6420 2865 2e67 2e20 6063   method (e.g. `c
-000023d0: 6c69 656e 742e 636f 6e6e 6563 7460 2920  lient.connect`) 
-000023e0: 7769 7468 2074 6865 206b 6579 776f 7264  with the keyword
-000023f0: 2061 7267 756d 656e 7420 6066 6574 6368   argument `fetch
-00002400: 5f72 6f6f 6d5f 696e 666f 3d54 7275 6560  _room_info=True`
-00002410: 202e 2020 7c0a 7c20 6769 6674 5f69 6e66   .  |.| gift_inf
-00002420: 6f20 2020 2020 207c 2045 7874 7261 2067  o      | Extra g
-00002430: 6966 7420 696e 666f 726d 6174 696f 6e20  ift information 
-00002440: 7468 6174 2069 7320 7265 7472 6965 7665  that is retrieve
-00002450: 6420 6672 6f6d 2054 696b 546f 6b20 7768  d from TikTok wh
-00002460: 656e 2079 6f75 2075 7365 2061 2063 6f6e  en you use a con
-00002470: 6e65 6374 696f 6e20 6d65 7468 6f64 2028  nection method (
-00002480: 652e 672e 2060 636c 6965 6e74 2e72 756e  e.g. `client.run
-00002490: 6029 2077 6974 6820 7468 6520 6b65 7977  `) with the keyw
-000024a0: 6f72 6420 6172 6775 6d65 6e74 2060 6665  ord argument `fe
-000024b0: 7463 685f 6769 6674 5f69 6e66 6f3d 5472  tch_gift_info=Tr
-000024c0: 7565 602e 207c 0a0a 0a23 2320 5765 6244  ue`. |...## WebD
-000024d0: 6566 6175 6c74 730a 0a54 696b 546f 6b4c  efaults..TikTokL
-000024e0: 6976 6520 6861 7320 6120 7365 7269 6573  ive has a series
-000024f0: 206f 6620 676c 6f62 616c 2064 6566 6175   of global defau
-00002500: 6c74 7320 7573 6564 2074 6f20 6372 6561  lts used to crea
-00002510: 7465 2074 6865 2048 5454 5020 636c 6965  te the HTTP clie
-00002520: 6e74 2077 6869 6368 2079 6f75 2063 616e  nt which you can
-00002530: 2063 7573 746f 6d69 7a65 2e20 466f 7220   customize. For 
-00002540: 696e 666f 206f 6e20 686f 7720 746f 2073  info on how to s
-00002550: 6574 2074 6865 7365 2070 6172 616d 6574  et these paramet
-00002560: 6572 732c 2073 6565 0a74 6865 205b 7765  ers, see.the [we
-00002570: 625f 6465 6661 756c 7473 2e70 795d 2868  b_defaults.py](h
-00002580: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002590: 6d2f 6973 6161 636b 6f67 616e 2f54 696b  m/isaackogan/Tik
-000025a0: 546f 6b4c 6976 652f 626c 6f62 2f6d 6173  TokLive/blob/mas
-000025b0: 7465 722f 6578 616d 706c 6573 2f77 6562  ter/examples/web
-000025c0: 5f64 6566 6175 6c74 732e 7079 2920 6578  _defaults.py) ex
-000025d0: 616d 706c 652e 0a0a 7c20 5061 7261 6d65  ample...| Parame
-000025e0: 7465 7220 2020 2020 2020 2020 2020 7c20  ter           | 
-000025f0: 5479 7065 2020 207c 2044 6573 6372 6970  Type   | Descrip
-00002600: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002680: 2020 2020 2020 7c0a 7c2d 2d2d 2d2d 2d2d        |.|-------
-00002690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
-000026a0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-000026b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002730: 2d2d 2d2d 2d2d 7c0a 7c20 7469 6b74 6f6b  ------|.| tiktok
-00002740: 5f61 7070 5f75 726c 2020 2020 2020 7c20  _app_url      | 
-00002750: 6073 7472 6020 207c 2054 6865 2054 696b  `str`  | The Tik
-00002760: 546f 6b20 6170 7020 5552 4c20 2860 6874  Tok app URL (`ht
-00002770: 7470 733a 2f2f 7777 772e 7469 6b74 6f6b  tps://www.tiktok
-00002780: 2e63 6f6d 6029 2075 7365 6420 746f 2073  .com`) used to s
-00002790: 6372 6170 6520 7468 6520 726f 6f6d 2e20  crape the room. 
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027e0: 2020 2020 2020 7c0a 7c20 7469 6b74 6f6b        |.| tiktok
-000027f0: 5f73 6967 6e5f 7572 6c20 2020 2020 7c20  _sign_url     | 
-00002800: 6073 7472 6020 207c 2054 6865 205b 7369  `str`  | The [si
-00002810: 676e 6174 7572 6520 7365 7276 6572 5d28  gnature server](
-00002820: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002830: 6f6d 2f69 7361 6163 6b6f 6761 6e2f 5469  om/isaackogan/Ti
-00002840: 6b54 6f6b 4c69 7665 2f77 696b 692f 416c  kTokLive/wiki/Al
-00002850: 6c2d 4162 6f75 742d 5369 676e 6174 7572  l-About-Signatur
-00002860: 6573 2920 7573 6564 2074 6f20 6765 6e65  es) used to gene
-00002870: 7261 7465 2074 6f6b 656e 7320 746f 2063  rate tokens to c
-00002880: 6f6e 6e65 6374 2074 6f20 5469 6b54 6f6b  onnect to TikTok
-00002890: 4c69 7665 2e20 7c0a 7c20 7469 6b74 6f6b  Live. |.| tiktok
-000028a0: 5f77 6562 6361 7374 5f75 726c 2020 7c20  _webcast_url  | 
-000028b0: 6073 7472 6020 207c 2054 6865 2054 696b  `str`  | The Tik
-000028c0: 546f 6b20 6c69 7665 7374 7265 616d 2055  Tok livestream U
-000028d0: 524c 2028 6068 7474 7073 3a2f 2f77 6562  RL (`https://web
-000028e0: 6361 7374 2e74 696b 746f 6b2e 636f 6d60  cast.tiktok.com`
-000028f0: 2920 7768 6572 6520 6c69 7665 7374 7265  ) where livestre
-00002900: 616d 7320 6361 6e20 6265 2061 6363 6573  ams can be acces
-00002910: 7365 6420 6672 6f6d 2e20 2020 2020 2020  sed from.       
-00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002940: 2020 2020 2020 7c0a 7c20 636c 6965 6e74        |.| client
-00002950: 5f70 6172 616d 7320 2020 2020 2020 7c20  _params       | 
-00002960: 6064 6963 7460 207c 2054 6865 2055 524c  `dict` | The URL
-00002970: 2070 6172 616d 6574 6572 7320 6164 6465   parameters adde
-00002980: 6420 6f6e 2074 6f20 5469 6b54 6f6b 2072  d on to TikTok r
-00002990: 6571 7565 7374 7320 6672 6f6d 2074 6865  equests from the
-000029a0: 2048 5454 5020 636c 6965 6e74 2e20 2020   HTTP client.   
-000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2020 2020 2020 7c0a 7c20 636c 6965 6e74        |.| client
-00002a00: 5f68 6561 6465 7273 2020 2020 2020 7c20  _headers      | 
-00002a10: 6064 6963 7460 207c 2054 6865 2068 6561  `dict` | The hea
-00002a20: 6465 7273 2061 6464 6564 206f 6e20 746f  ders added on to
-00002a30: 2054 696b 546f 6b20 7265 7175 6573 7473   TikTok requests
-00002a40: 2066 726f 6d20 7468 6520 4854 5450 2063   from the HTTP c
-00002a50: 6c69 656e 742e 2020 2020 2020 2020 2020  lient.          
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002aa0: 2020 2020 2020 7c0a 7c20 7469 6b74 6f6b        |.| tiktok
-00002ab0: 5f73 6967 6e5f 6170 695f 6b65 7920 7c20  _sign_api_key | 
-00002ac0: 6073 7472 6020 207c 2041 2067 6c6f 6261  `str`  | A globa
-00002ad0: 6c20 7761 7920 6f66 2073 6574 7469 6e67  l way of setting
-00002ae0: 2074 6865 2060 7369 676e 5f61 7069 5f6b   the `sign_api_k
-00002af0: 6579 6020 7061 7261 6d65 7465 722e 2020  ey` parameter.  
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b50: 2020 2020 2020 7c0a 0a23 2320 4576 656e        |..## Even
-00002b60: 7473 0a0a 4576 656e 7473 2063 616e 2062  ts..Events can b
-00002b70: 6520 6c69 7374 656e 6564 2074 6f20 7573  e listened to us
-00002b80: 696e 6720 6120 6465 636f 7261 746f 7220  ing a decorator 
-00002b90: 6f72 206e 6f6e 2d64 6563 6f72 6174 6f72  or non-decorator
-00002ba0: 206d 6574 686f 6420 6361 6c6c 2e20 5468   method call. Th
-00002bb0: 6520 666f 6c6c 6f77 696e 6720 6578 616d  e following exam
-00002bc0: 706c 6573 2069 6c6c 7573 7472 6174 6520  ples illustrate 
-00002bd0: 686f 7720 796f 7520 6361 6e20 6c69 7374  how you can list
-00002be0: 656e 2074 6f20 616e 2065 7665 6e74 3a0a  en to an event:.
-00002bf0: 0a60 6060 7079 7468 6f6e 0a40 636c 6965  .```python.@clie
-00002c00: 6e74 2e6f 6e28 4c69 6b65 4576 656e 7429  nt.on(LikeEvent)
-00002c10: 0a61 7379 6e63 2064 6566 206f 6e5f 6c69  .async def on_li
-00002c20: 6b65 2865 7665 6e74 3a20 4c69 6b65 4576  ke(event: LikeEv
-00002c30: 656e 7429 202d 3e20 4e6f 6e65 3a0a 2020  ent) -> None:.  
-00002c40: 2020 2e2e 2e0a 0a61 7379 6e63 2064 6566    .....async def
-00002c50: 206f 6e5f 636f 6d6d 656e 7428 6576 656e   on_comment(even
-00002c60: 743a 2043 6f6d 6d65 6e74 4576 656e 7429  t: CommentEvent)
-00002c70: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2e2e   -> None:.    ..
-00002c80: 2e0a 0a63 6c69 656e 742e 6164 645f 6c69  ...client.add_li
-00002c90: 7374 656e 6572 2843 6f6d 6d65 6e74 4576  stener(CommentEv
-00002ca0: 656e 742c 206f 6e5f 636f 6d6d 656e 7429  ent, on_comment)
-00002cb0: 0a60 6060 0a0a 5468 6572 6520 6172 6520  .```..There are 
-00002cc0: 7477 6f20 7479 7065 7320 6f66 2065 7665  two types of eve
-00002cd0: 6e74 732c 205b 6043 7573 746f 6d45 7665  nts, [`CustomEve
-00002ce0: 6e74 605d 2868 7474 7073 3a2f 2f67 6974  nt`](https://git
-00002cf0: 6875 622e 636f 6d2f 6973 6161 636b 6f67  hub.com/isaackog
-00002d00: 616e 2f54 696b 546f 6b4c 6976 652f 626c  an/TikTokLive/bl
-00002d10: 6f62 2f6d 6173 7465 722f 5469 6b54 6f6b  ob/master/TikTok
-00002d20: 4c69 7665 2f65 7665 6e74 732f 6375 7374  Live/events/cust
-00002d30: 6f6d 5f65 7665 6e74 732e 7079 2920 0a65  om_events.py) .e
-00002d40: 7665 6e74 7320 616e 6420 5b60 5072 6f74  vents and [`Prot
-00002d50: 6f45 7665 6e74 605d 2868 7474 7073 3a2f  oEvent`](https:/
-00002d60: 2f67 6974 6875 622e 636f 6d2f 6973 6161  /github.com/isaa
-00002d70: 636b 6f67 616e 2f54 696b 546f 6b4c 6976  ckogan/TikTokLiv
-00002d80: 652f 626c 6f62 2f6d 6173 7465 722f 5469  e/blob/master/Ti
-00002d90: 6b54 6f6b 4c69 7665 2f65 7665 6e74 732f  kTokLive/events/
-00002da0: 7072 6f74 6f5f 6576 656e 7473 2e70 7929  proto_events.py)
-00002db0: 2065 7665 6e74 732e 0a42 6f74 6820 6265   events..Both be
-00002dc0: 6c6f 6e67 2074 6f20 7468 6520 5469 6b54  long to the TikT
-00002dd0: 6f6b 4c69 7665 2060 4576 656e 7460 2074  okLive `Event` t
-00002de0: 7970 6520 616e 6420 6361 6e20 6265 206c  ype and can be l
-00002df0: 6973 7465 6e65 6420 746f 2e20 5468 6520  istened to. The 
-00002e00: 666f 6c6c 6f77 696e 6720 6576 656e 7473  following events
-00002e10: 2061 7265 2061 7661 696c 6162 6c65 3a0a   are available:.
-00002e20: 0a23 2323 2043 7573 746f 6d20 4576 656e  .### Custom Even
-00002e30: 7473 0a0a 2d20 6043 6f6e 6e65 6374 4576  ts..- `ConnectEv
-00002e40: 656e 7460 202d 2054 7269 6767 6572 6564  ent` - Triggered
-00002e50: 2077 6865 6e20 7468 6520 5765 6263 6173   when the Webcas
-00002e60: 7420 636f 6e6e 6563 7469 6f6e 2069 7320  t connection is 
-00002e70: 696e 6974 6961 7465 640a 2d20 6044 6973  initiated.- `Dis
-00002e80: 636f 6e6e 6563 7445 7665 6e74 6020 2d20  connectEvent` - 
-00002e90: 5472 6967 6765 7265 6420 7768 656e 2074  Triggered when t
-00002ea0: 6865 2057 6562 6361 7374 2063 6f6e 6e65  he Webcast conne
-00002eb0: 6374 696f 6e20 636c 6f73 6573 2028 696e  ction closes (in
-00002ec0: 636c 7564 696e 6720 7468 6520 6c69 7665  cluding the live
-00002ed0: 7374 7265 616d 2065 6e64 696e 6729 0a2d  stream ending).-
-00002ee0: 2060 4c69 7665 456e 6445 7665 6e74 6020   `LiveEndEvent` 
-00002ef0: 2d20 5472 6967 6765 7265 6420 7768 656e  - Triggered when
-00002f00: 2074 6865 206c 6976 6573 7472 6561 6d20   the livestream 
-00002f10: 656e 6473 0a2d 2060 4c69 7665 5061 7573  ends.- `LivePaus
-00002f20: 6545 7665 6e74 6020 2d20 5472 6967 6765  eEvent` - Trigge
-00002f30: 7265 6420 7768 656e 2074 6865 206c 6976  red when the liv
-00002f40: 6573 7472 6561 6d20 6973 2070 6175 7365  estream is pause
-00002f50: 640a 2d20 604c 6976 6555 6e70 6175 7365  d.- `LiveUnpause
-00002f60: 4576 656e 7460 202d 2054 7269 6767 6572  Event` - Trigger
-00002f70: 6564 2077 6865 6e20 7468 6520 6c69 7665  ed when the live
-00002f80: 7374 7265 616d 2069 7320 756e 7061 7573  stream is unpaus
-00002f90: 6564 0a2d 2060 466f 6c6c 6f77 4576 656e  ed.- `FollowEven
-00002fa0: 7460 202d 2054 7269 6767 6572 6564 2077  t` - Triggered w
-00002fb0: 6865 6e20 6120 7573 6572 2069 6e20 7468  hen a user in th
-00002fc0: 6520 6c69 7665 7374 7265 616d 2066 6f6c  e livestream fol
-00002fd0: 6c6f 7773 2074 6865 2073 7472 6561 6d65  lows the streame
-00002fe0: 720a 2d20 6053 6861 7265 4576 656e 7460  r.- `ShareEvent`
-00002ff0: 202d 2054 7269 6767 6572 6564 2077 6865   - Triggered whe
-00003000: 6e20 6120 7573 6572 2073 6861 7265 7320  n a user shares 
-00003010: 7468 6520 6c69 7665 7374 7265 616d 0a2d  the livestream.-
-00003020: 2060 5765 6273 6f63 6b65 7452 6573 706f   `WebsocketRespo
-00003030: 6e73 6545 7665 6e74 6020 2d20 5472 6967  nseEvent` - Trig
-00003040: 6765 7265 6420 7768 656e 2061 6e79 2065  gered when any e
-00003050: 7665 6e74 2069 7320 7265 6365 6976 6564  vent is received
-00003060: 2028 636f 6e74 6169 6e73 2074 6865 2065   (contains the e
-00003070: 7665 6e74 290a 2d20 6055 6e6b 6e6f 776e  vent).- `Unknown
-00003080: 4576 656e 7460 202d 2041 6e20 696e 7374  Event` - An inst
-00003090: 616e 6365 206f 6620 6057 6562 736f 636b  ance of `Websock
-000030a0: 6574 5265 7370 6f6e 7365 4576 656e 7460  etResponseEvent`
-000030b0: 2074 6872 6f77 6e20 7768 656e 6576 6572   thrown whenever
-000030c0: 2061 6e20 6576 656e 7420 646f 6573 206e   an event does n
-000030d0: 6f74 2068 6176 6520 616e 2065 7869 7374  ot have an exist
-000030e0: 696e 6720 6465 6669 6e69 7469 6f6e 2c20  ing definition, 
-000030f0: 7573 6566 756c 2066 6f72 2064 6562 7567  useful for debug
-00003100: 6769 6e67 0a0a 2323 2320 5072 6f74 6f20  ging..### Proto 
-00003110: 4576 656e 7473 0a0a 4966 2079 6f75 206b  Events..If you k
-00003120: 6e6f 7720 7768 6174 2061 6e20 6576 656e  now what an even
-00003130: 7420 646f 6573 2c20 5b6d 616b 6520 6120  t does, [make a 
-00003140: 7075 6c6c 2072 6571 7565 7374 5d28 6874  pull request](ht
-00003150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003160: 2f69 7361 6163 6b6f 6761 6e2f 5469 6b54  /isaackogan/TikT
-00003170: 6f6b 4c69 7665 2f70 756c 6c73 2920 616e  okLive/pulls) an
-00003180: 6420 6164 6420 7468 6520 6465 7363 7269  d add the descri
-00003190: 7074 696f 6e2e 200a 0a2d 2060 4769 6674  ption. ..- `Gift
-000031a0: 4576 656e 7460 202d 2054 7269 6767 6572  Event` - Trigger
-000031b0: 6564 2077 6865 6e20 6120 6769 6674 2069  ed when a gift i
-000031c0: 7320 7365 6e74 2074 6f20 7468 6520 7374  s sent to the st
-000031d0: 7265 616d 6572 0a2d 2060 476f 616c 5570  reamer.- `GoalUp
-000031e0: 6461 7465 4576 656e 7460 202d 2054 7269  dateEvent` - Tri
-000031f0: 6767 6572 6564 2077 6865 6e20 7468 6520  ggered when the 
-00003200: 7375 6273 6372 6962 6572 2067 6f61 6c20  subscriber goal 
-00003210: 6973 2075 7064 6174 6564 0a2d 2060 436f  is updated.- `Co
-00003220: 6e74 726f 6c45 7665 6e74 6020 2d20 5472  ntrolEvent` - Tr
-00003230: 6967 6765 7265 6420 7768 656e 2061 2073  iggered when a s
-00003240: 7472 6561 6d20 6163 7469 6f6e 206f 6363  tream action occ
-00003250: 7572 7320 2865 2e67 2e20 4c69 7665 7374  urs (e.g. Livest
-00003260: 7265 616d 2073 7461 7274 2c20 656e 6429  ream start, end)
-00003270: 0a2d 2060 4c69 6b65 4576 656e 7460 202d  .- `LikeEvent` -
-00003280: 2054 7269 6767 6572 6564 2077 6865 6e20   Triggered when 
-00003290: 7468 6520 7374 7265 616d 2072 6563 6569  the stream recei
-000032a0: 7665 7320 6120 6c69 6b65 0a2d 2060 5375  ves a like.- `Su
-000032b0: 6273 6372 6962 6545 7665 6e74 6020 2d20  bscribeEvent` - 
-000032c0: 5472 6967 6765 7265 6420 7768 656e 2073  Triggered when s
-000032d0: 6f6d 656f 6e65 2073 7562 7363 7269 6265  omeone subscribe
-000032e0: 7320 746f 2074 6865 2054 696b 546f 6b20  s to the TikTok 
-000032f0: 6372 6561 746f 720a 2d20 6050 6f6c 6c45  creator.- `PollE
-00003300: 7665 6e74 6020 2d20 5472 6967 6765 7265  vent` - Triggere
-00003310: 6420 7768 656e 2074 6865 2063 7265 6174  d when the creat
-00003320: 6f72 206c 6175 6e63 6865 7320 6120 6e65  or launches a ne
-00003330: 7720 706f 6c6c 0a2d 2060 436f 6d6d 656e  w poll.- `Commen
-00003340: 7445 7665 6e74 6020 2d20 5472 6967 6765  tEvent` - Trigge
-00003350: 7265 6420 7768 656e 2061 2063 6f6d 6d65  red when a comme
-00003360: 6e74 2069 7320 7365 6e74 2069 6e20 7468  nt is sent in th
-00003370: 6520 7374 7265 616d 0a2d 2060 526f 6f6d  e stream.- `Room
-00003380: 4576 656e 7460 202d 204d 6573 7361 6765  Event` - Message
-00003390: 7320 6272 6f61 6463 6173 7465 6420 746f  s broadcasted to
-000033a0: 2061 6c6c 2075 7365 7273 2069 6e20 7468   all users in th
-000033b0: 6520 726f 6f6d 2028 652e 672e 2022 5765  e room (e.g. "We
-000033c0: 6c63 6f6d 6520 746f 2054 696b 546f 6b20  lcome to TikTok 
-000033d0: 4c49 5645 2122 290a 2d20 6045 6d6f 7465  LIVE!").- `Emote
-000033e0: 4368 6174 4576 656e 7460 202d 2054 7269  ChatEvent` - Tri
-000033f0: 6767 6572 6564 2077 6865 6e20 6120 6375  ggered when a cu
-00003400: 7374 6f6d 2065 6d6f 7465 2069 7320 7365  stom emote is se
-00003410: 6e74 2069 6e20 7468 6520 6368 6174 0a2d  nt in the chat.-
-00003420: 2060 456e 7665 6c6f 7065 4576 656e 7460   `EnvelopeEvent`
-00003430: 202d 2054 7269 6767 6572 6564 2065 7665   - Triggered eve
-00003440: 7279 2074 696d 6520 736f 6d65 6f6e 6520  ry time someone 
-00003450: 7365 6e64 7320 6120 7472 6561 7375 7265  sends a treasure
-00003460: 2063 6865 7374 0a2d 2060 536f 6369 616c   chest.- `Social
-00003470: 4576 656e 7460 202d 2054 7269 6767 6572  Event` - Trigger
-00003480: 6564 2077 6865 6e20 6120 7573 6572 2073  ed when a user s
-00003490: 6861 7265 7320 7468 6520 7374 7265 616d  hares the stream
-000034a0: 206f 7220 666f 6c6c 6f77 7320 7468 6520   or follows the 
-000034b0: 686f 7374 0a2d 2060 5175 6573 7469 6f6e  host.- `Question
-000034c0: 4e65 7745 7665 6e74 6020 2d20 5472 6967  NewEvent` - Trig
-000034d0: 6765 7265 6420 6576 6572 7920 7469 6d65  gered every time
-000034e0: 2073 6f6d 656f 6e65 2061 736b 7320 6120   someone asks a 
-000034f0: 6e65 7720 7175 6573 7469 6f6e 2076 6961  new question via
-00003500: 2074 6865 2071 7565 7374 696f 6e20 6665   the question fe
-00003510: 6174 7572 652e 0a2d 2060 4c69 7665 496e  ature..- `LiveIn
-00003520: 7472 6f45 7665 6e74 6020 2d20 5472 6967  troEvent` - Trig
-00003530: 6765 7265 6420 7768 656e 2061 206c 6976  gered when a liv
-00003540: 6520 696e 7472 6f20 6d65 7373 6167 6520  e intro message 
-00003550: 6170 7065 6172 730a 2d20 604c 696e 6b4d  appears.- `LinkM
-00003560: 6963 4172 6d69 6573 4576 656e 7460 202d  icArmiesEvent` -
-00003570: 2054 7269 6767 6572 6564 2077 6865 6e20   Triggered when 
-00003580: 6120 5469 6b54 6f6b 2062 6174 746c 6520  a TikTok battle 
-00003590: 7573 6572 2072 6563 6569 7665 7320 706f  user receives po
-000035a0: 696e 7473 0a2d 2060 4c69 6e6b 4d69 6342  ints.- `LinkMicB
-000035b0: 6174 746c 6545 7665 6e74 6020 2d20 5472  attleEvent` - Tr
-000035c0: 6967 6765 7265 6420 7768 656e 2061 2054  iggered when a T
-000035d0: 696b 546f 6b20 6261 7474 6c65 2069 7320  ikTok battle is 
-000035e0: 7374 6172 7465 640a 2d20 604a 6f69 6e45  started.- `JoinE
-000035f0: 7665 6e74 6020 2d20 5472 6967 6765 7265  vent` - Triggere
-00003600: 6420 7768 656e 2061 2075 7365 7220 6a6f  d when a user jo
-00003610: 696e 7320 7468 6520 6c69 7665 7374 7265  ins the livestre
-00003620: 616d 0a2d 2060 4c69 6e6b 4d69 6346 616e  am.- `LinkMicFan
-00003630: 5469 636b 6574 4d65 7468 6f64 4576 656e  TicketMethodEven
-00003640: 7460 0a2d 2060 4c69 6e6b 4d69 634d 6574  t`.- `LinkMicMet
-00003650: 686f 6445 7665 6e74 600a 2d20 6042 6172  hodEvent`.- `Bar
-00003660: 7261 6765 4576 656e 7460 0a2d 2060 4361  rageEvent`.- `Ca
-00003670: 7074 696f 6e45 7665 6e74 600a 2d20 6049  ptionEvent`.- `I
-00003680: 6d44 656c 6574 6545 7665 6e74 600a 2d20  mDeleteEvent`.- 
-00003690: 6052 6f6f 6d55 7365 7253 6571 4576 656e  `RoomUserSeqEven
-000036a0: 7460 202d 2043 7572 7265 6e74 2076 6965  t` - Current vie
-000036b0: 7765 7220 636f 756e 7420 696e 666f 726d  wer count inform
-000036c0: 6174 696f 6e0a 2d20 6052 616e 6b55 7064  ation.- `RankUpd
-000036d0: 6174 6545 7665 6e74 600a 2d20 6052 616e  ateEvent`.- `Ran
-000036e0: 6b54 6578 7445 7665 6e74 600a 2d20 6048  kTextEvent`.- `H
-000036f0: 6f75 726c 7952 616e 6b45 7665 6e74 600a  ourlyRankEvent`.
-00003700: 2d20 6055 6e61 7574 686f 7269 7a65 644d  - `UnauthorizedM
-00003710: 656d 6265 7245 7665 6e74 600a 2d20 604d  emberEvent`.- `M
-00003720: 6573 7361 6765 4465 7465 6374 4576 656e  essageDetectEven
-00003730: 7460 0a2d 2060 4f65 634c 6976 6553 686f  t`.- `OecLiveSho
-00003740: 7070 696e 6745 7665 6e74 600a 2d20 6052  ppingEvent`.- `R
-00003750: 6f6f 6d50 696e 4576 656e 7460 0a2d 2060  oomPinEvent`.- `
-00003760: 5379 7374 656d 4576 656e 7460 0a2d 2060  SystemEvent`.- `
-00003770: 4c69 6e6b 4576 656e 7460 0a2d 2060 4c69  LinkEvent`.- `Li
-00003780: 6e6b 4c61 7965 7245 7665 6e74 600a 0a23  nkLayerEvent`..#
-00003790: 2323 2053 7065 6369 616c 2045 7665 6e74  ## Special Event
-000037a0: 730a 0a23 2323 2060 4769 6674 4576 656e  s..### `GiftEven
-000037b0: 7460 0a0a 5472 6967 6765 7265 6420 6576  t`..Triggered ev
-000037c0: 6572 7920 7469 6d65 2061 2067 6966 7420  ery time a gift 
-000037d0: 6172 7269 7665 732e 2045 7874 7261 2069  arrives. Extra i
-000037e0: 6e66 6f72 6d61 7469 6f6e 2063 616e 2062  nformation can b
-000037f0: 6520 676c 6561 6d65 6420 6672 6f6d 2074  e gleamed from t
-00003800: 6865 2060 6176 6169 6c61 626c 655f 6769  he `available_gi
-00003810: 6674 7360 2063 6c69 656e 7420 6174 7472  fts` client attr
-00003820: 6962 7574 652e 0a3e 202a 2a4e 4f54 453a  ibute..> **NOTE:
-00003830: 2a2a 2055 7365 7273 2068 6176 6520 7468  ** Users have th
-00003840: 6520 6361 7061 6269 6c69 7479 2074 6f20  e capability to 
-00003850: 7365 6e64 2067 6966 7473 2069 6e20 6120  send gifts in a 
-00003860: 7374 7265 616b 2e20 5468 6973 2069 6e63  streak. This inc
-00003870: 7265 6173 6573 2074 6865 2060 6576 656e  reases the `even
-00003880: 742e 6769 6674 2e72 6570 6561 745f 636f  t.gift.repeat_co
-00003890: 756e 7460 2076 616c 7565 2075 6e74 696c  unt` value until
-000038a0: 2074 6865 0a3e 2075 7365 7220 7465 726d   the.> user term
-000038b0: 696e 6174 6573 2074 6865 2073 7472 6561  inates the strea
-000038c0: 6b2e 2044 7572 696e 6720 7468 6973 2074  k. During this t
-000038d0: 696d 6520 6e65 7720 6769 6674 2065 7665  ime new gift eve
-000038e0: 6e74 7320 6172 6520 7472 6967 6765 7265  nts are triggere
-000038f0: 6420 6167 6169 6e20 616e 6420 6167 6169  d again and agai
-00003900: 6e20 7769 7468 2061 6e0a 3e20 696e 6372  n with an.> incr
-00003910: 6561 7365 6420 6065 7665 6e74 2e67 6966  eased `event.gif
-00003920: 742e 7265 7065 6174 5f63 6f75 6e74 6020  t.repeat_count` 
-00003930: 7661 6c75 652e 2049 7420 7368 6f75 6c64  value. It should
-00003940: 2062 6520 6e6f 7465 6420 7468 6174 2061   be noted that a
-00003950: 6674 6572 2074 6865 2065 6e64 206f 6620  fter the end of 
-00003960: 6120 7374 7265 616b 2c20 6120 6669 6e61  a streak, a fina
-00003970: 6c20 6769 6674 2065 7665 6e74 2069 730a  l gift event is.
-00003980: 3e20 7472 6967 6765 7265 642c 2077 6869  > triggered, whi
-00003990: 6368 2073 6967 6e61 6c73 2074 6865 2065  ch signals the e
-000039a0: 6e64 206f 6620 7468 6520 7374 7265 616b  nd of the streak
-000039b0: 2077 6974 6820 6065 7665 6e74 2e72 6570   with `event.rep
-000039c0: 6561 745f 656e 6460 3a60 3160 2e20 5468  eat_end`:`1`. Th
-000039d0: 6520 666f 6c6c 6f77 696e 6720 6861 6e64  e following hand
-000039e0: 6c65 7273 2073 686f 7720 686f 7720 796f  lers show how yo
-000039f0: 7520 6361 6e20 6465 616c 2077 6974 6820  u can deal with 
-00003a00: 7468 6973 2069 6e20 796f 7572 2063 6f64  this in your cod
-00003a10: 652e 0a0a 5573 696e 6720 7468 6520 6c6f  e...Using the lo
-00003a20: 772d 6c65 7665 6c20 6469 7265 6374 2070  w-level direct p
-00003a30: 726f 746f 3a0a 6060 6070 7974 686f 6e0a  roto:.```python.
-00003a40: 4063 6c69 656e 742e 6f6e 2847 6966 7445  @client.on(GiftE
-00003a50: 7665 6e74 290a 6173 796e 6320 6465 6620  vent).async def 
-00003a60: 6f6e 5f67 6966 7428 6576 656e 743a 2047  on_gift(event: G
-00003a70: 6966 7445 7665 6e74 293a 0a20 2020 2023  iftEvent):.    #
-00003a80: 2049 6620 6974 2773 2074 7970 6520 3120   If it's type 1 
-00003a90: 616e 6420 7468 6520 7374 7265 616b 2069  and the streak i
-00003aa0: 7320 6f76 6572 0a20 2020 2069 6620 6576  s over.    if ev
-00003ab0: 656e 742e 6769 6674 2e69 6e66 6f2e 7479  ent.gift.info.ty
-00003ac0: 7065 203d 3d20 313a 0a20 2020 2020 2020  pe == 1:.       
-00003ad0: 2069 6620 6576 656e 742e 6769 6674 2e69   if event.gift.i
-00003ae0: 735f 7265 7065 6174 696e 6720 3d3d 2031  s_repeating == 1
-00003af0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00003b00: 696e 7428 6622 7b65 7665 6e74 2e75 7365  int(f"{event.use
-00003b10: 722e 756e 6971 7565 5f69 647d 2073 656e  r.unique_id} sen
-00003b20: 7420 7b65 7665 6e74 2e67 6966 742e 636f  t {event.gift.co
-00003b30: 756e 747d 7820 5c22 7b65 7665 6e74 2e67  unt}x \"{event.g
-00003b40: 6966 742e 696e 666f 2e6e 616d 657d 5c22  ift.info.name}\"
-00003b50: 2229 0a0a 2020 2020 2320 4974 2773 206e  ")..    # It's n
-00003b60: 6f74 2074 7970 6520 312c 2077 6869 6368  ot type 1, which
-00003b70: 206d 6561 6e73 2069 7420 6361 6e27 7420   means it can't 
-00003b80: 6861 7665 2061 2073 7472 6561 6b20 2620  have a streak & 
-00003b90: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
-00003ba0: 206f 7665 720a 2020 2020 656c 6966 2065   over.    elif e
-00003bb0: 7665 6e74 2e67 6966 742e 696e 666f 2e74  vent.gift.info.t
-00003bc0: 7970 6520 213d 2031 3a0a 2020 2020 2020  ype != 1:.      
-00003bd0: 2020 7072 696e 7428 6622 7b65 7665 6e74    print(f"{event
-00003be0: 2e75 7365 722e 756e 6971 7565 5f69 647d  .user.unique_id}
-00003bf0: 2073 656e 7420 5c22 7b65 7665 6e74 2e67   sent \"{event.g
-00003c00: 6966 742e 696e 666f 2e6e 616d 657d 5c22  ift.info.name}\"
-00003c10: 2229 0a60 6060 0a0a 5573 696e 6720 7468  ").```..Using th
-00003c20: 6520 5469 6b54 6f6b 4c69 7665 2065 7874  e TikTokLive ext
-00003c30: 656e 6465 6420 7072 6f74 6f3a 0a60 6060  ended proto:.```
-00003c40: 7079 7468 6f6e 0a40 636c 6965 6e74 2e6f  python.@client.o
-00003c50: 6e28 2267 6966 7422 290a 6173 796e 6320  n("gift").async 
-00003c60: 6465 6620 6f6e 5f67 6966 7428 6576 656e  def on_gift(even
-00003c70: 743a 2047 6966 7445 7665 6e74 293a 0a20  t: GiftEvent):. 
-00003c80: 2020 2023 2053 7472 6561 6b61 626c 6520     # Streakable 
-00003c90: 6769 6674 2026 2073 7472 6561 6b20 6973  gift & streak is
-00003ca0: 206f 7665 720a 2020 2020 6966 2065 7665   over.    if eve
-00003cb0: 6e74 2e67 6966 742e 7374 7265 616b 6162  nt.gift.streakab
-00003cc0: 6c65 2061 6e64 206e 6f74 2065 7665 6e74  le and not event
-00003cd0: 2e73 7472 6561 6b69 6e67 3a0a 2020 2020  .streaking:.    
-00003ce0: 2020 2020 7072 696e 7428 6622 7b65 7665      print(f"{eve
-00003cf0: 6e74 2e75 7365 722e 756e 6971 7565 5f69  nt.user.unique_i
-00003d00: 647d 2073 656e 7420 7b65 7665 6e74 2e67  d} sent {event.g
-00003d10: 6966 742e 636f 756e 747d 7820 5c22 7b65  ift.count}x \"{e
-00003d20: 7665 6e74 2e67 6966 742e 696e 666f 2e6e  vent.gift.info.n
-00003d30: 616d 657d 5c22 2229 0a0a 2020 2020 2320  ame}\"")..    # 
-00003d40: 4e6f 6e2d 7374 7265 616b 6162 6c65 2067  Non-streakable g
-00003d50: 6966 740a 2020 2020 656c 6966 206e 6f74  ift.    elif not
-00003d60: 2065 7665 6e74 2e67 6966 742e 7374 7265   event.gift.stre
-00003d70: 616b 6162 6c65 3a0a 2020 2020 2020 2020  akable:.        
-00003d80: 7072 696e 7428 6622 7b65 7665 6e74 2e75  print(f"{event.u
-00003d90: 7365 722e 756e 6971 7565 5f69 647d 2073  ser.unique_id} s
-00003da0: 656e 7420 5c22 7b65 7665 6e74 2e67 6966  ent \"{event.gif
-00003db0: 742e 696e 666f 2e6e 616d 657d 5c22 2229  t.info.name}\"")
-00003dc0: 0a0a 6060 600a 0a23 2323 2060 5375 6273  ..```..### `Subs
-00003dd0: 6372 6962 6545 7665 6e74 600a 0a54 6869  cribeEvent`..Thi
-00003de0: 7320 6576 656e 7420 7769 6c6c 206f 6e6c  s event will onl
-00003df0: 7920 6669 7265 2077 6865 6e20 6120 7365  y fire when a se
-00003e00: 7373 696f 6e20 4944 2028 6163 636f 756e  ssion ID (accoun
-00003e10: 7420 6c6f 6769 6e29 2069 7320 7061 7373  t login) is pass
-00003e20: 6564 2074 6f20 7468 6520 4854 5450 2063  ed to the HTTP c
-00003e30: 6c69 656e 7420 2a62 6566 6f72 652a 2063  lient *before* c
-00003e40: 6f6e 6e65 6374 696e 6720 746f 2054 696b  onnecting to Tik
-00003e50: 546f 6b20 4c49 5645 2e0a 596f 7520 6361  Tok LIVE..You ca
-00003e60: 6e20 7365 7420 7468 6520 7365 7373 696f  n set the sessio
-00003e70: 6e20 4944 2077 6974 6820 5b60 636c 6965  n ID with [`clie
-00003e80: 6e74 2e77 6562 2e73 6574 5f73 6573 7369  nt.web.set_sessi
-00003e90: 6f6e 5f69 6428 2e2e 2e29 605d 2868 7474  on_id(...)`](htt
-00003ea0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003eb0: 6973 6161 636b 6f67 616e 2f54 696b 546f  isaackogan/TikTo
-00003ec0: 6b4c 6976 652f 626c 6f62 2f6d 6173 7465  kLive/blob/maste
-00003ed0: 722f 6578 616d 706c 6573 2f6c 6f67 6765  r/examples/logge
-00003ee0: 645f 696e 2e70 7929 2e0a 0a23 2320 4368  d_in.py)...## Ch
-00003ef0: 6563 6b69 6e67 2049 6620 4120 5573 6572  ecking If A User
-00003f00: 2049 7320 4c69 7665 0a0a 4974 2069 7320   Is Live..It is 
-00003f10: 636f 6e73 6964 6572 6564 2069 6e65 6666  considered ineff
-00003f20: 6963 6965 6e74 2074 6f20 7573 6520 7468  icient to use th
-00003f30: 6520 636f 6e6e 6563 7420 6d65 7468 6f64  e connect method
-00003f40: 2074 6f20 6368 6563 6b20 6966 2061 2075   to check if a u
-00003f50: 7365 7220 6973 206c 6976 652e 2049 7420  ser is live. It 
-00003f60: 6973 2062 6574 7465 7220 746f 2075 7365  is better to use
-00003f70: 2074 6865 2064 6564 6963 6174 6564 2060   the dedicated `
-00003f80: 6177 6169 7420 636c 6965 6e74 2e69 735f  await client.is_
-00003f90: 6c69 7665 2829 6020 6d65 7468 6f64 2e20  live()` method. 
-00003fa0: 0a0a 5468 6572 6520 6973 2061 205b 636f  ..There is a [co
-00003fb0: 6d70 6c65 7465 2065 7861 6d70 6c65 5d28  mplete example](
-00003fc0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00003fd0: 6f6d 2f69 7361 6163 6b6f 6761 6e2f 5469  om/isaackogan/Ti
-00003fe0: 6b54 6f6b 4c69 7665 2f62 6c6f 622f 6d61  kTokLive/blob/ma
-00003ff0: 7374 6572 2f65 7861 6d70 6c65 732f 6368  ster/examples/ch
-00004000: 6563 6b5f 6c69 7665 2e70 7929 206f 6620  eck_live.py) of 
-00004010: 686f 7720 746f 2064 6f20 7468 6973 2069  how to do this i
-00004020: 6e20 7468 6520 5b65 7861 6d70 6c65 735d  n the [examples]
-00004030: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00004040: 636f 6d2f 6973 6161 636b 6f67 616e 2f54  com/isaackogan/T
-00004050: 696b 546f 6b4c 6976 652f 7472 6565 2f6d  ikTokLive/tree/m
-00004060: 6173 7465 722f 6578 616d 706c 6573 2920  aster/examples) 
-00004070: 666f 6c64 6572 2e0a 0a23 2320 436f 6e74  folder...## Cont
-00004080: 7269 6275 746f 7273 0a0a 2a20 2a2a 4973  ributors..* **Is
-00004090: 6161 6320 4b6f 6761 6e2a 2a20 2d20 2a43  aac Kogan** - *C
-000040a0: 7265 6174 6f72 2c20 5072 696d 6172 7920  reator, Primary 
-000040b0: 4d61 696e 7461 696e 6572 2c20 616e 6420  Maintainer, and 
-000040c0: 5265 7665 7273 652d 456e 6769 6e65 6572  Reverse-Engineer
-000040d0: 696e 672a 202d 205b 6973 6161 636b 6f67  ing* - [isaackog
-000040e0: 616e 5d28 6874 7470 733a 2f2f 6769 7468  an](https://gith
-000040f0: 7562 2e63 6f6d 2f69 7361 6163 6b6f 6761  ub.com/isaackoga
-00004100: 6e29 0a2a 202a 2a5a 6572 6f64 792a 2a20  n).* **Zerody** 
-00004110: 2d20 2a49 6e69 7469 616c 2052 6576 6572  - *Initial Rever
-00004120: 7365 2d45 6e67 696e 6565 7269 6e67 2050  se-Engineering P
-00004130: 726f 746f 6275 6620 2620 5375 7070 6f72  rotobuf & Suppor
-00004140: 742a 202d 205b 5a65 726f 6479 5d28 6874  t* - [Zerody](ht
-00004150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00004160: 2f7a 6572 6f64 7974 7261 7368 2f29 0a2a  /zerodytrash/).*
-00004170: 202a 2a44 6176 696e 6369 626c 652a 2a20   **Davincible** 
-00004180: 2d20 2a52 6576 6572 7365 2d45 6e67 696e  - *Reverse-Engin
-00004190: 6565 7269 6e67 2053 7472 6561 6d20 446f  eering Stream Do
-000041a0: 776e 6c6f 6164 732a 2020 2d20 5b64 6176  wnloads*  - [dav
-000041b0: 696e 6369 626c 655d 2868 7474 7073 3a2f  incible](https:/
-000041c0: 2f67 6974 6875 622e 636f 6d2f 6461 7669  /github.com/davi
-000041d0: 6e63 6962 6c65 290a 0a53 6565 2061 6c73  ncible)..See als
-000041e0: 6f20 7468 6520 6675 6c6c 206c 6973 7420  o the full list 
-000041f0: 6f66 205b 636f 6e74 7269 6275 746f 7273  of [contributors
-00004200: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004210: 2e63 6f6d 2f69 7361 6163 6b6f 6761 6e2f  .com/isaackogan/
-00004220: 5469 6b54 6f6b 4c69 7665 2f63 6f6e 7472  TikTokLive/contr
-00004230: 6962 7574 6f72 7329 2077 686f 2068 6176  ibutors) who hav
-00004240: 6520 7061 7274 6963 6970 6174 6564 2069  e participated i
-00004250: 6e0a 7468 6973 2070 726f 6a65 6374 2e0a  n.this project..
-00004260: 0a23 2320 4c69 6365 6e73 650a 0a54 6869  .## License..Thi
-00004270: 7320 7072 6f6a 6563 7420 6973 206c 6963  s project is lic
-00004280: 656e 7365 6420 756e 6465 7220 7468 6520  ensed under the 
-00004290: 4d49 5420 4c69 6365 6e73 6520 2d20 7365  MIT License - se
-000042a0: 6520 7468 6520 5b4c 4943 454e 5345 5d28  e the [LICENSE](
-000042b0: 4c49 4345 4e53 4529 2066 696c 6520 666f  LICENSE) file fo
-000042c0: 7220 6465 7461 696c 732e 0a              r details..
+00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002240: 2020 2020 2020 207c 0a7c 2d2d 2d2d 2d2d         |.|------
+00002250: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
+00002260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022f0: 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 726f 6f6d  --------|.| room
+00002300: 5f69 6420 2020 2020 2020 207c 2054 6865  _id        | The
+00002310: 2052 6f6f 6d20 4944 206f 6620 7468 6520   Room ID of the 
+00002320: 6c69 7665 7374 7265 616d 2072 6f6f 6d20  livestream room 
+00002330: 7468 6520 636c 6965 6e74 2069 7320 6375  the client is cu
+00002340: 7272 656e 746c 7920 636f 6e6e 6563 7465  rrently connecte
+00002350: 6420 746f 2e20 2020 2020 2020 2020 2020  d to.           
+00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2020 2020 2020 2020 207c 0a7c 2077 6562           |.| web
+000023b0: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
+000023c0: 6520 5469 6b54 6f6b 2048 5454 5020 636c  e TikTok HTTP cl
+000023d0: 6965 6e74 2e20 5468 6973 2063 6c69 656e  ient. This clien
+000023e0: 7420 6861 7320 6120 6c6f 7420 6f66 2075  t has a lot of u
+000023f0: 7365 6675 6c20 726f 7574 6573 2079 6f75  seful routes you
+00002400: 2073 686f 756c 6420 6578 706c 6f72 6521   should explore!
+00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002450: 2020 2020 2020 2020 2020 7c0a 7c20 636f            |.| co
+00002460: 6e6e 6563 7465 6420 2020 2020 207c 2057  nnected      | W
+00002470: 6865 7468 6572 2079 6f75 2061 7265 2063  hether you are c
+00002480: 7572 7265 6e74 6c79 2063 6f6e 6e65 6374  urrently connect
+00002490: 6564 2074 6f20 7468 6520 6c69 7665 7374  ed to the livest
+000024a0: 7265 616d 2e20 2020 2020 2020 2020 2020  ream.           
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002500: 2020 2020 2020 2020 2020 207c 0a7c 206c             |.| l
+00002510: 6f67 6765 7220 2020 2020 2020 2020 7c20  ogger         | 
+00002520: 5468 6520 696e 7465 726e 616c 206c 6f67  The internal log
+00002530: 6765 7220 7573 6564 2062 7920 5469 6b54  ger used by TikT
+00002540: 6f6b 4c69 7665 2e20 596f 7520 6361 6e20  okLive. You can 
+00002550: 7573 6520 6063 6c69 656e 742e 6c6f 6767  use `client.logg
+00002560: 6572 2e73 6574 4c65 7665 6c28 2e2e 2e29  er.setLevel(...)
+00002570: 6020 6d65 7468 6f64 2074 6f20 656e 6162  ` method to enab
+00002580: 6c65 2063 6c69 656e 7420 6465 6275 672e  le client debug.
+00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+000025c0: 726f 6f6d 5f69 6e66 6f20 2020 2020 207c  room_info      |
+000025d0: 2052 6f6f 6d20 696e 666f 726d 6174 696f   Room informatio
+000025e0: 6e20 7468 6174 2069 7320 7265 7472 6965  n that is retrie
+000025f0: 7665 6420 6672 6f6d 2054 696b 546f 6b20  ved from TikTok 
+00002600: 7768 656e 2079 6f75 2075 7365 2061 2063  when you use a c
+00002610: 6f6e 6e65 6374 696f 6e20 6d65 7468 6f64  onnection method
+00002620: 2028 652e 672e 2060 636c 6965 6e74 2e63   (e.g. `client.c
+00002630: 6f6e 6e65 6374 6029 2077 6974 6820 7468  onnect`) with th
+00002640: 6520 6b65 7977 6f72 6420 6172 6775 6d65  e keyword argume
+00002650: 6e74 2060 6665 7463 685f 726f 6f6d 5f69  nt `fetch_room_i
+00002660: 6e66 6f3d 5472 7565 6020 2e20 207c 0a7c  nfo=True` .  |.|
+00002670: 2067 6966 745f 696e 666f 2020 2020 2020   gift_info      
+00002680: 7c20 4578 7472 6120 6769 6674 2069 6e66  | Extra gift inf
+00002690: 6f72 6d61 7469 6f6e 2074 6861 7420 6973  ormation that is
+000026a0: 2072 6574 7269 6576 6564 2066 726f 6d20   retrieved from 
+000026b0: 5469 6b54 6f6b 2077 6865 6e20 796f 7520  TikTok when you 
+000026c0: 7573 6520 6120 636f 6e6e 6563 7469 6f6e  use a connection
+000026d0: 206d 6574 686f 6420 2865 2e67 2e20 6063   method (e.g. `c
+000026e0: 6c69 656e 742e 7275 6e60 2920 7769 7468  lient.run`) with
+000026f0: 2074 6865 206b 6579 776f 7264 2061 7267   the keyword arg
+00002700: 756d 656e 7420 6066 6574 6368 5f67 6966  ument `fetch_gif
+00002710: 745f 696e 666f 3d54 7275 6560 2e20 7c0a  t_info=True`. |.
+00002720: 0a0a 2323 2057 6562 4465 6661 756c 7473  ..## WebDefaults
+00002730: 0a0a 5469 6b54 6f6b 4c69 7665 2068 6173  ..TikTokLive has
+00002740: 2061 2073 6572 6965 7320 6f66 2067 6c6f   a series of glo
+00002750: 6261 6c20 6465 6661 756c 7473 2075 7365  bal defaults use
+00002760: 6420 746f 2063 7265 6174 6520 7468 6520  d to create the 
+00002770: 4854 5450 2063 6c69 656e 7420 7768 6963  HTTP client whic
+00002780: 6820 796f 7520 6361 6e20 6375 7374 6f6d  h you can custom
+00002790: 697a 652e 2046 6f72 2069 6e66 6f20 6f6e  ize. For info on
+000027a0: 2068 6f77 2074 6f20 7365 7420 7468 6573   how to set thes
+000027b0: 6520 7061 7261 6d65 7465 7273 2c20 7365  e parameters, se
+000027c0: 650a 7468 6520 5b77 6562 5f64 6566 6175  e.the [web_defau
+000027d0: 6c74 732e 7079 5d28 6874 7470 733a 2f2f  lts.py](https://
+000027e0: 6769 7468 7562 2e63 6f6d 2f69 7361 6163  github.com/isaac
+000027f0: 6b6f 6761 6e2f 5469 6b54 6f6b 4c69 7665  kogan/TikTokLive
+00002800: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
+00002810: 6d70 6c65 732f 7765 625f 6465 6661 756c  mples/web_defaul
+00002820: 7473 2e70 7929 2065 7861 6d70 6c65 2e0a  ts.py) example..
+00002830: 0a7c 2050 6172 616d 6574 6572 2020 2020  .| Parameter    
+00002840: 2020 2020 2020 207c 2054 7970 6520 2020         | Type   
+00002850: 7c20 4465 7363 7269 7074 696f 6e20 2020  | Description   
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000028e0: 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|--------------
+000028f0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+00002900: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00002910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00002990: 0a7c 2074 696b 746f 6b5f 6170 705f 7572  .| tiktok_app_ur
+000029a0: 6c20 2020 2020 207c 2060 7374 7260 2020  l      | `str`  
+000029b0: 7c20 5468 6520 5469 6b54 6f6b 2061 7070  | The TikTok app
+000029c0: 2055 524c 2028 6068 7474 7073 3a2f 2f77   URL (`https://w
+000029d0: 7777 2e74 696b 746f 6b2e 636f 6d60 2920  ww.tiktok.com`) 
+000029e0: 7573 6564 2074 6f20 7363 7261 7065 2074  used to scrape t
+000029f0: 6865 2072 6f6f 6d2e 2020 2020 2020 2020  he room.        
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002a40: 0a7c 2074 696b 746f 6b5f 7369 676e 5f75  .| tiktok_sign_u
+00002a50: 726c 2020 2020 207c 2060 7374 7260 2020  rl     | `str`  
+00002a60: 7c20 5468 6520 5b73 6967 6e61 7475 7265  | The [signature
+00002a70: 2073 6572 7665 725d 2868 7474 7073 3a2f   server](https:/
+00002a80: 2f67 6974 6875 622e 636f 6d2f 6973 6161  /github.com/isaa
+00002a90: 636b 6f67 616e 2f54 696b 546f 6b4c 6976  ckogan/TikTokLiv
+00002aa0: 652f 7769 6b69 2f41 6c6c 2d41 626f 7574  e/wiki/All-About
+00002ab0: 2d53 6967 6e61 7475 7265 7329 2075 7365  -Signatures) use
+00002ac0: 6420 746f 2067 656e 6572 6174 6520 746f  d to generate to
+00002ad0: 6b65 6e73 2074 6f20 636f 6e6e 6563 7420  kens to connect 
+00002ae0: 746f 2054 696b 546f 6b4c 6976 652e 207c  to TikTokLive. |
+00002af0: 0a7c 2074 696b 746f 6b5f 7765 6263 6173  .| tiktok_webcas
+00002b00: 745f 7572 6c20 207c 2060 7374 7260 2020  t_url  | `str`  
+00002b10: 7c20 5468 6520 5469 6b54 6f6b 206c 6976  | The TikTok liv
+00002b20: 6573 7472 6561 6d20 5552 4c20 2860 6874  estream URL (`ht
+00002b30: 7470 733a 2f2f 7765 6263 6173 742e 7469  tps://webcast.ti
+00002b40: 6b74 6f6b 2e63 6f6d 6029 2077 6865 7265  ktok.com`) where
+00002b50: 206c 6976 6573 7472 6561 6d73 2063 616e   livestreams can
+00002b60: 2062 6520 6163 6365 7373 6564 2066 726f   be accessed fro
+00002b70: 6d2e 2020 2020 2020 2020 2020 2020 2020  m.              
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002ba0: 0a7c 2063 6c69 656e 745f 7061 7261 6d73  .| client_params
+00002bb0: 2020 2020 2020 207c 2060 6469 6374 6020         | `dict` 
+00002bc0: 7c20 5468 6520 5552 4c20 7061 7261 6d65  | The URL parame
+00002bd0: 7465 7273 2061 6464 6564 206f 6e20 746f  ters added on to
+00002be0: 2054 696b 546f 6b20 7265 7175 6573 7473   TikTok requests
+00002bf0: 2066 726f 6d20 7468 6520 4854 5450 2063   from the HTTP c
+00002c00: 6c69 656e 742e 2020 2020 2020 2020 2020  lient.          
+00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c40: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002c50: 0a7c 2063 6c69 656e 745f 6865 6164 6572  .| client_header
+00002c60: 7320 2020 2020 207c 2060 6469 6374 6020  s      | `dict` 
+00002c70: 7c20 5468 6520 6865 6164 6572 7320 6164  | The headers ad
+00002c80: 6465 6420 6f6e 2074 6f20 5469 6b54 6f6b  ded on to TikTok
+00002c90: 2072 6571 7565 7374 7320 6672 6f6d 2074   requests from t
+00002ca0: 6865 2048 5454 5020 636c 6965 6e74 2e20  he HTTP client. 
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002d00: 0a7c 2074 696b 746f 6b5f 7369 676e 5f61  .| tiktok_sign_a
+00002d10: 7069 5f6b 6579 207c 2060 7374 7260 2020  pi_key | `str`  
+00002d20: 7c20 4120 676c 6f62 616c 2077 6179 206f  | A global way o
+00002d30: 6620 7365 7474 696e 6720 7468 6520 6073  f setting the `s
+00002d40: 6967 6e5f 6170 695f 6b65 7960 2070 6172  ign_api_key` par
+00002d50: 616d 6574 6572 2e20 2020 2020 2020 2020  ameter.         
+00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002da0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002db0: 0a0a 2323 2045 7665 6e74 730a 0a45 7665  ..## Events..Eve
+00002dc0: 6e74 7320 6361 6e20 6265 206c 6973 7465  nts can be liste
+00002dd0: 6e65 6420 746f 2075 7369 6e67 2061 2064  ned to using a d
+00002de0: 6563 6f72 6174 6f72 206f 7220 6e6f 6e2d  ecorator or non-
+00002df0: 6465 636f 7261 746f 7220 6d65 7468 6f64  decorator method
+00002e00: 2063 616c 6c2e 2054 6865 2066 6f6c 6c6f   call. The follo
+00002e10: 7769 6e67 2065 7861 6d70 6c65 7320 696c  wing examples il
+00002e20: 6c75 7374 7261 7465 2068 6f77 2079 6f75  lustrate how you
+00002e30: 2063 616e 206c 6973 7465 6e20 746f 2061   can listen to a
+00002e40: 6e20 6576 656e 743a 0a0a 6060 6070 7974  n event:..```pyt
+00002e50: 686f 6e0a 4063 6c69 656e 742e 6f6e 284c  hon.@client.on(L
+00002e60: 696b 6545 7665 6e74 290a 6173 796e 6320  ikeEvent).async 
+00002e70: 6465 6620 6f6e 5f6c 696b 6528 6576 656e  def on_like(even
+00002e80: 743a 204c 696b 6545 7665 6e74 2920 2d3e  t: LikeEvent) ->
+00002e90: 204e 6f6e 653a 0a20 2020 202e 2e2e 0a0a   None:.    .....
+00002ea0: 6173 796e 6320 6465 6620 6f6e 5f63 6f6d  async def on_com
+00002eb0: 6d65 6e74 2865 7665 6e74 3a20 436f 6d6d  ment(event: Comm
+00002ec0: 656e 7445 7665 6e74 2920 2d3e 204e 6f6e  entEvent) -> Non
+00002ed0: 653a 0a20 2020 202e 2e2e 0a0a 636c 6965  e:.    .....clie
+00002ee0: 6e74 2e61 6464 5f6c 6973 7465 6e65 7228  nt.add_listener(
+00002ef0: 436f 6d6d 656e 7445 7665 6e74 2c20 6f6e  CommentEvent, on
+00002f00: 5f63 6f6d 6d65 6e74 290a 6060 600a 0a54  _comment).```..T
+00002f10: 6865 7265 2061 7265 2074 776f 2074 7970  here are two typ
+00002f20: 6573 206f 6620 6576 656e 7473 2c20 5b60  es of events, [`
+00002f30: 4375 7374 6f6d 4576 656e 7460 5d28 6874  CustomEvent`](ht
+00002f40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002f50: 2f69 7361 6163 6b6f 6761 6e2f 5469 6b54  /isaackogan/TikT
+00002f60: 6f6b 4c69 7665 2f62 6c6f 622f 6d61 7374  okLive/blob/mast
+00002f70: 6572 2f54 696b 546f 6b4c 6976 652f 6576  er/TikTokLive/ev
+00002f80: 656e 7473 2f63 7573 746f 6d5f 6576 656e  ents/custom_even
+00002f90: 7473 2e70 7929 200a 6576 656e 7473 2061  ts.py) .events a
+00002fa0: 6e64 205b 6050 726f 746f 4576 656e 7460  nd [`ProtoEvent`
+00002fb0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002fc0: 2e63 6f6d 2f69 7361 6163 6b6f 6761 6e2f  .com/isaackogan/
+00002fd0: 5469 6b54 6f6b 4c69 7665 2f62 6c6f 622f  TikTokLive/blob/
+00002fe0: 6d61 7374 6572 2f54 696b 546f 6b4c 6976  master/TikTokLiv
+00002ff0: 652f 6576 656e 7473 2f70 726f 746f 5f65  e/events/proto_e
+00003000: 7665 6e74 732e 7079 2920 6576 656e 7473  vents.py) events
+00003010: 2e0a 426f 7468 2062 656c 6f6e 6720 746f  ..Both belong to
+00003020: 2074 6865 2054 696b 546f 6b4c 6976 6520   the TikTokLive 
+00003030: 6045 7665 6e74 6020 7479 7065 2061 6e64  `Event` type and
+00003040: 2063 616e 2062 6520 6c69 7374 656e 6564   can be listened
+00003050: 2074 6f2e 2054 6865 2066 6f6c 6c6f 7769   to. The followi
+00003060: 6e67 2065 7665 6e74 7320 6172 6520 6176  ng events are av
+00003070: 6169 6c61 626c 653a 0a0a 2323 2320 4375  ailable:..### Cu
+00003080: 7374 6f6d 2045 7665 6e74 730a 0a2d 2060  stom Events..- `
+00003090: 436f 6e6e 6563 7445 7665 6e74 6020 2d20  ConnectEvent` - 
+000030a0: 5472 6967 6765 7265 6420 7768 656e 2074  Triggered when t
+000030b0: 6865 2057 6562 6361 7374 2063 6f6e 6e65  he Webcast conne
+000030c0: 6374 696f 6e20 6973 2069 6e69 7469 6174  ction is initiat
+000030d0: 6564 0a2d 2060 4469 7363 6f6e 6e65 6374  ed.- `Disconnect
+000030e0: 4576 656e 7460 202d 2054 7269 6767 6572  Event` - Trigger
+000030f0: 6564 2077 6865 6e20 7468 6520 5765 6263  ed when the Webc
+00003100: 6173 7420 636f 6e6e 6563 7469 6f6e 2063  ast connection c
+00003110: 6c6f 7365 7320 2869 6e63 6c75 6469 6e67  loses (including
+00003120: 2074 6865 206c 6976 6573 7472 6561 6d20   the livestream 
+00003130: 656e 6469 6e67 290a 2d20 604c 6976 6545  ending).- `LiveE
+00003140: 6e64 4576 656e 7460 202d 2054 7269 6767  ndEvent` - Trigg
+00003150: 6572 6564 2077 6865 6e20 7468 6520 6c69  ered when the li
+00003160: 7665 7374 7265 616d 2065 6e64 730a 2d20  vestream ends.- 
+00003170: 604c 6976 6550 6175 7365 4576 656e 7460  `LivePauseEvent`
+00003180: 202d 2054 7269 6767 6572 6564 2077 6865   - Triggered whe
+00003190: 6e20 7468 6520 6c69 7665 7374 7265 616d  n the livestream
+000031a0: 2069 7320 7061 7573 6564 0a2d 2060 4c69   is paused.- `Li
+000031b0: 7665 556e 7061 7573 6545 7665 6e74 6020  veUnpauseEvent` 
+000031c0: 2d20 5472 6967 6765 7265 6420 7768 656e  - Triggered when
+000031d0: 2074 6865 206c 6976 6573 7472 6561 6d20   the livestream 
+000031e0: 6973 2075 6e70 6175 7365 640a 2d20 6046  is unpaused.- `F
+000031f0: 6f6c 6c6f 7745 7665 6e74 6020 2d20 5472  ollowEvent` - Tr
+00003200: 6967 6765 7265 6420 7768 656e 2061 2075  iggered when a u
+00003210: 7365 7220 696e 2074 6865 206c 6976 6573  ser in the lives
+00003220: 7472 6561 6d20 666f 6c6c 6f77 7320 7468  tream follows th
+00003230: 6520 7374 7265 616d 6572 0a2d 2060 5368  e streamer.- `Sh
+00003240: 6172 6545 7665 6e74 6020 2d20 5472 6967  areEvent` - Trig
+00003250: 6765 7265 6420 7768 656e 2061 2075 7365  gered when a use
+00003260: 7220 7368 6172 6573 2074 6865 206c 6976  r shares the liv
+00003270: 6573 7472 6561 6d0a 2d20 6057 6562 736f  estream.- `Webso
+00003280: 636b 6574 5265 7370 6f6e 7365 4576 656e  cketResponseEven
+00003290: 7460 202d 2054 7269 6767 6572 6564 2077  t` - Triggered w
+000032a0: 6865 6e20 616e 7920 6576 656e 7420 6973  hen any event is
+000032b0: 2072 6563 6569 7665 6420 2863 6f6e 7461   received (conta
+000032c0: 696e 7320 7468 6520 6576 656e 7429 0a2d  ins the event).-
+000032d0: 2060 556e 6b6e 6f77 6e45 7665 6e74 6020   `UnknownEvent` 
+000032e0: 2d20 416e 2069 6e73 7461 6e63 6520 6f66  - An instance of
+000032f0: 2060 5765 6273 6f63 6b65 7452 6573 706f   `WebsocketRespo
+00003300: 6e73 6545 7665 6e74 6020 7468 726f 776e  nseEvent` thrown
+00003310: 2077 6865 6e65 7665 7220 616e 2065 7665   whenever an eve
+00003320: 6e74 2064 6f65 7320 6e6f 7420 6861 7665  nt does not have
+00003330: 2061 6e20 6578 6973 7469 6e67 2064 6566   an existing def
+00003340: 696e 6974 696f 6e2c 2075 7365 6675 6c20  inition, useful 
+00003350: 666f 7220 6465 6275 6767 696e 670a 0a23  for debugging..#
+00003360: 2323 2050 726f 746f 2045 7665 6e74 730a  ## Proto Events.
+00003370: 0a49 6620 796f 7520 6b6e 6f77 2077 6861  .If you know wha
+00003380: 7420 616e 2065 7665 6e74 2064 6f65 732c  t an event does,
+00003390: 205b 6d61 6b65 2061 2070 756c 6c20 7265   [make a pull re
+000033a0: 7175 6573 745d 2868 7474 7073 3a2f 2f67  quest](https://g
+000033b0: 6974 6875 622e 636f 6d2f 6973 6161 636b  ithub.com/isaack
+000033c0: 6f67 616e 2f54 696b 546f 6b4c 6976 652f  ogan/TikTokLive/
+000033d0: 7075 6c6c 7329 2061 6e64 2061 6464 2074  pulls) and add t
+000033e0: 6865 2064 6573 6372 6970 7469 6f6e 2e20  he description. 
+000033f0: 0a0a 2d20 6047 6966 7445 7665 6e74 6020  ..- `GiftEvent` 
+00003400: 2d20 5472 6967 6765 7265 6420 7768 656e  - Triggered when
+00003410: 2061 2067 6966 7420 6973 2073 656e 7420   a gift is sent 
+00003420: 746f 2074 6865 2073 7472 6561 6d65 720a  to the streamer.
+00003430: 2d20 6047 6f61 6c55 7064 6174 6545 7665  - `GoalUpdateEve
+00003440: 6e74 6020 2d20 5472 6967 6765 7265 6420  nt` - Triggered 
+00003450: 7768 656e 2074 6865 2073 7562 7363 7269  when the subscri
+00003460: 6265 7220 676f 616c 2069 7320 7570 6461  ber goal is upda
+00003470: 7465 640a 2d20 6043 6f6e 7472 6f6c 4576  ted.- `ControlEv
+00003480: 656e 7460 202d 2054 7269 6767 6572 6564  ent` - Triggered
+00003490: 2077 6865 6e20 6120 7374 7265 616d 2061   when a stream a
+000034a0: 6374 696f 6e20 6f63 6375 7273 2028 652e  ction occurs (e.
+000034b0: 672e 204c 6976 6573 7472 6561 6d20 7374  g. Livestream st
+000034c0: 6172 742c 2065 6e64 290a 2d20 604c 696b  art, end).- `Lik
+000034d0: 6545 7665 6e74 6020 2d20 5472 6967 6765  eEvent` - Trigge
+000034e0: 7265 6420 7768 656e 2074 6865 2073 7472  red when the str
+000034f0: 6561 6d20 7265 6365 6976 6573 2061 206c  eam receives a l
+00003500: 696b 650a 2d20 6053 7562 7363 7269 6265  ike.- `Subscribe
+00003510: 4576 656e 7460 202d 2054 7269 6767 6572  Event` - Trigger
+00003520: 6564 2077 6865 6e20 736f 6d65 6f6e 6520  ed when someone 
+00003530: 7375 6273 6372 6962 6573 2074 6f20 7468  subscribes to th
+00003540: 6520 5469 6b54 6f6b 2063 7265 6174 6f72  e TikTok creator
+00003550: 0a2d 2060 506f 6c6c 4576 656e 7460 202d  .- `PollEvent` -
+00003560: 2054 7269 6767 6572 6564 2077 6865 6e20   Triggered when 
+00003570: 7468 6520 6372 6561 746f 7220 6c61 756e  the creator laun
+00003580: 6368 6573 2061 206e 6577 2070 6f6c 6c0a  ches a new poll.
+00003590: 2d20 6043 6f6d 6d65 6e74 4576 656e 7460  - `CommentEvent`
+000035a0: 202d 2054 7269 6767 6572 6564 2077 6865   - Triggered whe
+000035b0: 6e20 6120 636f 6d6d 656e 7420 6973 2073  n a comment is s
+000035c0: 656e 7420 696e 2074 6865 2073 7472 6561  ent in the strea
+000035d0: 6d0a 2d20 6052 6f6f 6d45 7665 6e74 6020  m.- `RoomEvent` 
+000035e0: 2d20 4d65 7373 6167 6573 2062 726f 6164  - Messages broad
+000035f0: 6361 7374 6564 2074 6f20 616c 6c20 7573  casted to all us
+00003600: 6572 7320 696e 2074 6865 2072 6f6f 6d20  ers in the room 
+00003610: 2865 2e67 2e20 2257 656c 636f 6d65 2074  (e.g. "Welcome t
+00003620: 6f20 5469 6b54 6f6b 204c 4956 4521 2229  o TikTok LIVE!")
+00003630: 0a2d 2060 456d 6f74 6543 6861 7445 7665  .- `EmoteChatEve
+00003640: 6e74 6020 2d20 5472 6967 6765 7265 6420  nt` - Triggered 
+00003650: 7768 656e 2061 2063 7573 746f 6d20 656d  when a custom em
+00003660: 6f74 6520 6973 2073 656e 7420 696e 2074  ote is sent in t
+00003670: 6865 2063 6861 740a 2d20 6045 6e76 656c  he chat.- `Envel
+00003680: 6f70 6545 7665 6e74 6020 2d20 5472 6967  opeEvent` - Trig
+00003690: 6765 7265 6420 6576 6572 7920 7469 6d65  gered every time
+000036a0: 2073 6f6d 656f 6e65 2073 656e 6473 2061   someone sends a
+000036b0: 2074 7265 6173 7572 6520 6368 6573 740a   treasure chest.
+000036c0: 2d20 6053 6f63 6961 6c45 7665 6e74 6020  - `SocialEvent` 
+000036d0: 2d20 5472 6967 6765 7265 6420 7768 656e  - Triggered when
+000036e0: 2061 2075 7365 7220 7368 6172 6573 2074   a user shares t
+000036f0: 6865 2073 7472 6561 6d20 6f72 2066 6f6c  he stream or fol
+00003700: 6c6f 7773 2074 6865 2068 6f73 740a 2d20  lows the host.- 
+00003710: 6051 7565 7374 696f 6e4e 6577 4576 656e  `QuestionNewEven
+00003720: 7460 202d 2054 7269 6767 6572 6564 2065  t` - Triggered e
+00003730: 7665 7279 2074 696d 6520 736f 6d65 6f6e  very time someon
+00003740: 6520 6173 6b73 2061 206e 6577 2071 7565  e asks a new que
+00003750: 7374 696f 6e20 7669 6120 7468 6520 7175  stion via the qu
+00003760: 6573 7469 6f6e 2066 6561 7475 7265 2e0a  estion feature..
+00003770: 2d20 604c 6976 6549 6e74 726f 4576 656e  - `LiveIntroEven
+00003780: 7460 202d 2054 7269 6767 6572 6564 2077  t` - Triggered w
+00003790: 6865 6e20 6120 6c69 7665 2069 6e74 726f  hen a live intro
+000037a0: 206d 6573 7361 6765 2061 7070 6561 7273   message appears
+000037b0: 0a2d 2060 4c69 6e6b 4d69 6341 726d 6965  .- `LinkMicArmie
+000037c0: 7345 7665 6e74 6020 2d20 5472 6967 6765  sEvent` - Trigge
+000037d0: 7265 6420 7768 656e 2061 2054 696b 546f  red when a TikTo
+000037e0: 6b20 6261 7474 6c65 2075 7365 7220 7265  k battle user re
+000037f0: 6365 6976 6573 2070 6f69 6e74 730a 2d20  ceives points.- 
+00003800: 604c 696e 6b4d 6963 4261 7474 6c65 4576  `LinkMicBattleEv
+00003810: 656e 7460 202d 2054 7269 6767 6572 6564  ent` - Triggered
+00003820: 2077 6865 6e20 6120 5469 6b54 6f6b 2062   when a TikTok b
+00003830: 6174 746c 6520 6973 2073 7461 7274 6564  attle is started
+00003840: 0a2d 2060 4a6f 696e 4576 656e 7460 202d  .- `JoinEvent` -
+00003850: 2054 7269 6767 6572 6564 2077 6865 6e20   Triggered when 
+00003860: 6120 7573 6572 206a 6f69 6e73 2074 6865  a user joins the
+00003870: 206c 6976 6573 7472 6561 6d0a 2d20 604c   livestream.- `L
+00003880: 696e 6b4d 6963 4661 6e54 6963 6b65 744d  inkMicFanTicketM
+00003890: 6574 686f 6445 7665 6e74 600a 2d20 604c  ethodEvent`.- `L
+000038a0: 696e 6b4d 6963 4d65 7468 6f64 4576 656e  inkMicMethodEven
+000038b0: 7460 0a2d 2060 4261 7272 6167 6545 7665  t`.- `BarrageEve
+000038c0: 6e74 600a 2d20 6043 6170 7469 6f6e 4576  nt`.- `CaptionEv
+000038d0: 656e 7460 0a2d 2060 496d 4465 6c65 7465  ent`.- `ImDelete
+000038e0: 4576 656e 7460 0a2d 2060 526f 6f6d 5573  Event`.- `RoomUs
+000038f0: 6572 5365 7145 7665 6e74 6020 2d20 4375  erSeqEvent` - Cu
+00003900: 7272 656e 7420 7669 6577 6572 2063 6f75  rrent viewer cou
+00003910: 6e74 2069 6e66 6f72 6d61 7469 6f6e 0a2d  nt information.-
+00003920: 2060 5261 6e6b 5570 6461 7465 4576 656e   `RankUpdateEven
+00003930: 7460 0a2d 2060 5261 6e6b 5465 7874 4576  t`.- `RankTextEv
+00003940: 656e 7460 0a2d 2060 486f 7572 6c79 5261  ent`.- `HourlyRa
+00003950: 6e6b 4576 656e 7460 0a2d 2060 556e 6175  nkEvent`.- `Unau
+00003960: 7468 6f72 697a 6564 4d65 6d62 6572 4576  thorizedMemberEv
+00003970: 656e 7460 0a2d 2060 4d65 7373 6167 6544  ent`.- `MessageD
+00003980: 6574 6563 7445 7665 6e74 600a 2d20 604f  etectEvent`.- `O
+00003990: 6563 4c69 7665 5368 6f70 7069 6e67 4576  ecLiveShoppingEv
+000039a0: 656e 7460 0a2d 2060 526f 6f6d 5069 6e45  ent`.- `RoomPinE
+000039b0: 7665 6e74 600a 2d20 6053 7973 7465 6d45  vent`.- `SystemE
+000039c0: 7665 6e74 600a 2d20 604c 696e 6b45 7665  vent`.- `LinkEve
+000039d0: 6e74 600a 2d20 604c 696e 6b4c 6179 6572  nt`.- `LinkLayer
+000039e0: 4576 656e 7460 0a0a 2323 2320 5370 6563  Event`..### Spec
+000039f0: 6961 6c20 4576 656e 7473 0a0a 2323 2320  ial Events..### 
+00003a00: 6047 6966 7445 7665 6e74 600a 0a54 7269  `GiftEvent`..Tri
+00003a10: 6767 6572 6564 2065 7665 7279 2074 696d  ggered every tim
+00003a20: 6520 6120 6769 6674 2061 7272 6976 6573  e a gift arrives
+00003a30: 2e20 4578 7472 6120 696e 666f 726d 6174  . Extra informat
+00003a40: 696f 6e20 6361 6e20 6265 2067 6c65 616d  ion can be gleam
+00003a50: 6564 2066 726f 6d20 7468 6520 6061 7661  ed from the `ava
+00003a60: 696c 6162 6c65 5f67 6966 7473 6020 636c  ilable_gifts` cl
+00003a70: 6965 6e74 2061 7474 7269 6275 7465 2e0a  ient attribute..
+00003a80: 3e20 2a2a 4e4f 5445 3a2a 2a20 5573 6572  > **NOTE:** User
+00003a90: 7320 6861 7665 2074 6865 2063 6170 6162  s have the capab
+00003aa0: 696c 6974 7920 746f 2073 656e 6420 6769  ility to send gi
+00003ab0: 6674 7320 696e 2061 2073 7472 6561 6b2e  fts in a streak.
+00003ac0: 2054 6869 7320 696e 6372 6561 7365 7320   This increases 
+00003ad0: 7468 6520 6065 7665 6e74 2e67 6966 742e  the `event.gift.
+00003ae0: 7265 7065 6174 5f63 6f75 6e74 6020 7661  repeat_count` va
+00003af0: 6c75 6520 756e 7469 6c20 7468 650a 3e20  lue until the.> 
+00003b00: 7573 6572 2074 6572 6d69 6e61 7465 7320  user terminates 
+00003b10: 7468 6520 7374 7265 616b 2e20 4475 7269  the streak. Duri
+00003b20: 6e67 2074 6869 7320 7469 6d65 206e 6577  ng this time new
+00003b30: 2067 6966 7420 6576 656e 7473 2061 7265   gift events are
+00003b40: 2074 7269 6767 6572 6564 2061 6761 696e   triggered again
+00003b50: 2061 6e64 2061 6761 696e 2077 6974 6820   and again with 
+00003b60: 616e 0a3e 2069 6e63 7265 6173 6564 2060  an.> increased `
+00003b70: 6576 656e 742e 6769 6674 2e72 6570 6561  event.gift.repea
+00003b80: 745f 636f 756e 7460 2076 616c 7565 2e20  t_count` value. 
+00003b90: 4974 2073 686f 756c 6420 6265 206e 6f74  It should be not
+00003ba0: 6564 2074 6861 7420 6166 7465 7220 7468  ed that after th
+00003bb0: 6520 656e 6420 6f66 2061 2073 7472 6561  e end of a strea
+00003bc0: 6b2c 2061 2066 696e 616c 2067 6966 7420  k, a final gift 
+00003bd0: 6576 656e 7420 6973 0a3e 2074 7269 6767  event is.> trigg
+00003be0: 6572 6564 2c20 7768 6963 6820 7369 676e  ered, which sign
+00003bf0: 616c 7320 7468 6520 656e 6420 6f66 2074  als the end of t
+00003c00: 6865 2073 7472 6561 6b20 7769 7468 2060  he streak with `
+00003c10: 6576 656e 742e 7265 7065 6174 5f65 6e64  event.repeat_end
+00003c20: 603a 6031 602e 2054 6865 2066 6f6c 6c6f  `:`1`. The follo
+00003c30: 7769 6e67 2068 616e 646c 6572 7320 7368  wing handlers sh
+00003c40: 6f77 2068 6f77 2079 6f75 2063 616e 2064  ow how you can d
+00003c50: 6561 6c20 7769 7468 2074 6869 7320 696e  eal with this in
+00003c60: 2079 6f75 7220 636f 6465 2e0a 0a55 7369   your code...Usi
+00003c70: 6e67 2074 6865 206c 6f77 2d6c 6576 656c  ng the low-level
+00003c80: 2064 6972 6563 7420 7072 6f74 6f3a 0a60   direct proto:.`
+00003c90: 6060 7079 7468 6f6e 0a40 636c 6965 6e74  ``python.@client
+00003ca0: 2e6f 6e28 4769 6674 4576 656e 7429 0a61  .on(GiftEvent).a
+00003cb0: 7379 6e63 2064 6566 206f 6e5f 6769 6674  sync def on_gift
+00003cc0: 2865 7665 6e74 3a20 4769 6674 4576 656e  (event: GiftEven
+00003cd0: 7429 3a0a 2020 2020 2320 4966 2069 7427  t):.    # If it'
+00003ce0: 7320 7479 7065 2031 2061 6e64 2074 6865  s type 1 and the
+00003cf0: 2073 7472 6561 6b20 6973 206f 7665 720a   streak is over.
+00003d00: 2020 2020 6966 2065 7665 6e74 2e67 6966      if event.gif
+00003d10: 742e 696e 666f 2e74 7970 6520 3d3d 2031  t.info.type == 1
+00003d20: 3a0a 2020 2020 2020 2020 6966 2065 7665  :.        if eve
+00003d30: 6e74 2e67 6966 742e 6973 5f72 6570 6561  nt.gift.is_repea
+00003d40: 7469 6e67 203d 3d20 313a 0a20 2020 2020  ting == 1:.     
+00003d50: 2020 2020 2020 2070 7269 6e74 2866 227b         print(f"{
+00003d60: 6576 656e 742e 7573 6572 2e75 6e69 7175  event.user.uniqu
+00003d70: 655f 6964 7d20 7365 6e74 207b 6576 656e  e_id} sent {even
+00003d80: 742e 6769 6674 2e63 6f75 6e74 7d78 205c  t.gift.count}x \
+00003d90: 227b 6576 656e 742e 6769 6674 2e69 6e66  "{event.gift.inf
+00003da0: 6f2e 6e61 6d65 7d5c 2222 290a 0a20 2020  o.name}\"")..   
+00003db0: 2023 2049 7427 7320 6e6f 7420 7479 7065   # It's not type
+00003dc0: 2031 2c20 7768 6963 6820 6d65 616e 7320   1, which means 
+00003dd0: 6974 2063 616e 2774 2068 6176 6520 6120  it can't have a 
+00003de0: 7374 7265 616b 2026 2069 7320 6175 746f  streak & is auto
+00003df0: 6d61 7469 6361 6c6c 7920 6f76 6572 0a20  matically over. 
+00003e00: 2020 2065 6c69 6620 6576 656e 742e 6769     elif event.gi
+00003e10: 6674 2e69 6e66 6f2e 7479 7065 2021 3d20  ft.info.type != 
+00003e20: 313a 0a20 2020 2020 2020 2070 7269 6e74  1:.        print
+00003e30: 2866 227b 6576 656e 742e 7573 6572 2e75  (f"{event.user.u
+00003e40: 6e69 7175 655f 6964 7d20 7365 6e74 205c  nique_id} sent \
+00003e50: 227b 6576 656e 742e 6769 6674 2e69 6e66  "{event.gift.inf
+00003e60: 6f2e 6e61 6d65 7d5c 2222 290a 6060 600a  o.name}\"").```.
+00003e70: 0a55 7369 6e67 2074 6865 2054 696b 546f  .Using the TikTo
+00003e80: 6b4c 6976 6520 6578 7465 6e64 6564 2070  kLive extended p
+00003e90: 726f 746f 3a0a 6060 6070 7974 686f 6e0a  roto:.```python.
+00003ea0: 4063 6c69 656e 742e 6f6e 2822 6769 6674  @client.on("gift
+00003eb0: 2229 0a61 7379 6e63 2064 6566 206f 6e5f  ").async def on_
+00003ec0: 6769 6674 2865 7665 6e74 3a20 4769 6674  gift(event: Gift
+00003ed0: 4576 656e 7429 3a0a 2020 2020 2320 5374  Event):.    # St
+00003ee0: 7265 616b 6162 6c65 2067 6966 7420 2620  reakable gift & 
+00003ef0: 7374 7265 616b 2069 7320 6f76 6572 0a20  streak is over. 
+00003f00: 2020 2069 6620 6576 656e 742e 6769 6674     if event.gift
+00003f10: 2e73 7472 6561 6b61 626c 6520 616e 6420  .streakable and 
+00003f20: 6e6f 7420 6576 656e 742e 7374 7265 616b  not event.streak
+00003f30: 696e 673a 0a20 2020 2020 2020 2070 7269  ing:.        pri
+00003f40: 6e74 2866 227b 6576 656e 742e 7573 6572  nt(f"{event.user
+00003f50: 2e75 6e69 7175 655f 6964 7d20 7365 6e74  .unique_id} sent
+00003f60: 207b 6576 656e 742e 6769 6674 2e63 6f75   {event.gift.cou
+00003f70: 6e74 7d78 205c 227b 6576 656e 742e 6769  nt}x \"{event.gi
+00003f80: 6674 2e69 6e66 6f2e 6e61 6d65 7d5c 2222  ft.info.name}\""
+00003f90: 290a 0a20 2020 2023 204e 6f6e 2d73 7472  )..    # Non-str
+00003fa0: 6561 6b61 626c 6520 6769 6674 0a20 2020  eakable gift.   
+00003fb0: 2065 6c69 6620 6e6f 7420 6576 656e 742e   elif not event.
+00003fc0: 6769 6674 2e73 7472 6561 6b61 626c 653a  gift.streakable:
+00003fd0: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
+00003fe0: 227b 6576 656e 742e 7573 6572 2e75 6e69  "{event.user.uni
+00003ff0: 7175 655f 6964 7d20 7365 6e74 205c 227b  que_id} sent \"{
+00004000: 6576 656e 742e 6769 6674 2e69 6e66 6f2e  event.gift.info.
+00004010: 6e61 6d65 7d5c 2222 290a 0a60 6060 0a0a  name}\"")..```..
+00004020: 2323 2320 6053 7562 7363 7269 6265 4576  ### `SubscribeEv
+00004030: 656e 7460 0a0a 5468 6973 2065 7665 6e74  ent`..This event
+00004040: 2077 696c 6c20 6f6e 6c79 2066 6972 6520   will only fire 
+00004050: 7768 656e 2061 2073 6573 7369 6f6e 2049  when a session I
+00004060: 4420 2861 6363 6f75 6e74 206c 6f67 696e  D (account login
+00004070: 2920 6973 2070 6173 7365 6420 746f 2074  ) is passed to t
+00004080: 6865 2048 5454 5020 636c 6965 6e74 202a  he HTTP client *
+00004090: 6265 666f 7265 2a20 636f 6e6e 6563 7469  before* connecti
+000040a0: 6e67 2074 6f20 5469 6b54 6f6b 204c 4956  ng to TikTok LIV
+000040b0: 452e 0a59 6f75 2063 616e 2073 6574 2074  E..You can set t
+000040c0: 6865 2073 6573 7369 6f6e 2049 4420 7769  he session ID wi
+000040d0: 7468 205b 6063 6c69 656e 742e 7765 622e  th [`client.web.
+000040e0: 7365 745f 7365 7373 696f 6e5f 6964 282e  set_session_id(.
+000040f0: 2e2e 2960 5d28 6874 7470 733a 2f2f 6769  ..)`](https://gi
+00004100: 7468 7562 2e63 6f6d 2f69 7361 6163 6b6f  thub.com/isaacko
+00004110: 6761 6e2f 5469 6b54 6f6b 4c69 7665 2f62  gan/TikTokLive/b
+00004120: 6c6f 622f 6d61 7374 6572 2f65 7861 6d70  lob/master/examp
+00004130: 6c65 732f 6c6f 6767 6564 5f69 6e2e 7079  les/logged_in.py
+00004140: 292e 0a0a 2323 2043 6865 636b 696e 6720  )...## Checking 
+00004150: 4966 2041 2055 7365 7220 4973 204c 6976  If A User Is Liv
+00004160: 650a 0a49 7420 6973 2063 6f6e 7369 6465  e..It is conside
+00004170: 7265 6420 696e 6566 6669 6369 656e 7420  red inefficient 
+00004180: 746f 2075 7365 2074 6865 2063 6f6e 6e65  to use the conne
+00004190: 6374 206d 6574 686f 6420 746f 2063 6865  ct method to che
+000041a0: 636b 2069 6620 6120 7573 6572 2069 7320  ck if a user is 
+000041b0: 6c69 7665 2e20 4974 2069 7320 6265 7474  live. It is bett
+000041c0: 6572 2074 6f20 7573 6520 7468 6520 6465  er to use the de
+000041d0: 6469 6361 7465 6420 6061 7761 6974 2063  dicated `await c
+000041e0: 6c69 656e 742e 6973 5f6c 6976 6528 2960  lient.is_live()`
+000041f0: 206d 6574 686f 642e 200a 0a54 6865 7265   method. ..There
+00004200: 2069 7320 6120 5b63 6f6d 706c 6574 6520   is a [complete 
+00004210: 6578 616d 706c 655d 2868 7474 7073 3a2f  example](https:/
+00004220: 2f67 6974 6875 622e 636f 6d2f 6973 6161  /github.com/isaa
+00004230: 636b 6f67 616e 2f54 696b 546f 6b4c 6976  ckogan/TikTokLiv
+00004240: 652f 626c 6f62 2f6d 6173 7465 722f 6578  e/blob/master/ex
+00004250: 616d 706c 6573 2f63 6865 636b 5f6c 6976  amples/check_liv
+00004260: 652e 7079 2920 6f66 2068 6f77 2074 6f20  e.py) of how to 
+00004270: 646f 2074 6869 7320 696e 2074 6865 205b  do this in the [
+00004280: 6578 616d 706c 6573 5d28 6874 7470 733a  examples](https:
+00004290: 2f2f 6769 7468 7562 2e63 6f6d 2f69 7361  //github.com/isa
+000042a0: 6163 6b6f 6761 6e2f 5469 6b54 6f6b 4c69  ackogan/TikTokLi
+000042b0: 7665 2f74 7265 652f 6d61 7374 6572 2f65  ve/tree/master/e
+000042c0: 7861 6d70 6c65 7329 2066 6f6c 6465 722e  xamples) folder.
+000042d0: 0a0a 2323 2043 6f6e 7472 6962 7574 6f72  ..## Contributor
+000042e0: 730a 0a2a 202a 2a49 7361 6163 204b 6f67  s..* **Isaac Kog
+000042f0: 616e 2a2a 202d 202a 4372 6561 746f 722c  an** - *Creator,
+00004300: 2050 7269 6d61 7279 204d 6169 6e74 6169   Primary Maintai
+00004310: 6e65 722c 2061 6e64 2052 6576 6572 7365  ner, and Reverse
+00004320: 2d45 6e67 696e 6565 7269 6e67 2a20 2d20  -Engineering* - 
+00004330: 5b69 7361 6163 6b6f 6761 6e5d 2868 7474  [isaackogan](htt
+00004340: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004350: 6973 6161 636b 6f67 616e 290a 2a20 2a2a  isaackogan).* **
+00004360: 5a65 726f 6479 2a2a 202d 202a 496e 6974  Zerody** - *Init
+00004370: 6961 6c20 5265 7665 7273 652d 456e 6769  ial Reverse-Engi
+00004380: 6e65 6572 696e 6720 5072 6f74 6f62 7566  neering Protobuf
+00004390: 2026 2053 7570 706f 7274 2a20 2d20 5b5a   & Support* - [Z
+000043a0: 6572 6f64 795d 2868 7474 7073 3a2f 2f67  erody](https://g
+000043b0: 6974 6875 622e 636f 6d2f 7a65 726f 6479  ithub.com/zerody
+000043c0: 7472 6173 682f 290a 2a20 2a2a 4461 7669  trash/).* **Davi
+000043d0: 6e63 6962 6c65 2a2a 202d 202a 5265 7665  ncible** - *Reve
+000043e0: 7273 652d 456e 6769 6e65 6572 696e 6720  rse-Engineering 
+000043f0: 5374 7265 616d 2044 6f77 6e6c 6f61 6473  Stream Downloads
+00004400: 2a20 202d 205b 6461 7669 6e63 6962 6c65  *  - [davincible
+00004410: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004420: 2e63 6f6d 2f64 6176 696e 6369 626c 6529  .com/davincible)
+00004430: 0a0a 5365 6520 616c 736f 2074 6865 2066  ..See also the f
+00004440: 756c 6c20 6c69 7374 206f 6620 5b63 6f6e  ull list of [con
+00004450: 7472 6962 7574 6f72 735d 2868 7474 7073  tributors](https
+00004460: 3a2f 2f67 6974 6875 622e 636f 6d2f 6973  ://github.com/is
+00004470: 6161 636b 6f67 616e 2f54 696b 546f 6b4c  aackogan/TikTokL
+00004480: 6976 652f 636f 6e74 7269 6275 746f 7273  ive/contributors
+00004490: 2920 7768 6f20 6861 7665 2070 6172 7469  ) who have parti
+000044a0: 6369 7061 7465 6420 696e 0a74 6869 7320  cipated in.this 
+000044b0: 7072 6f6a 6563 742e 0a0a 2323 204c 6963  project...## Lic
+000044c0: 656e 7365 0a0a 5468 6973 2070 726f 6a65  ense..This proje
+000044d0: 6374 2069 7320 6c69 6365 6e73 6564 2075  ct is licensed u
+000044e0: 6e64 6572 2074 6865 204d 4954 204c 6963  nder the MIT Lic
+000044f0: 656e 7365 202d 2073 6565 2074 6865 205b  ense - see the [
+00004500: 4c49 4345 4e53 455d 284c 4943 454e 5345  LICENSE](LICENSE
+00004510: 2920 6669 6c65 2066 6f72 2064 6574 6169  ) file for detai
+00004520: 6c73 2e0a                                ls..
```

### Comparing `TikTokLive-6.0.3/TikTokLive.egg-info/SOURCES.txt` & `TikTokLive-6.0.4/TikTokLive.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 TikTokLive/client/web/web_base.py
 TikTokLive/client/web/web_client.py
 TikTokLive/client/web/web_settings.py
 TikTokLive/client/web/routes/__init__.py
 TikTokLive/client/web/routes/fetch_gift_list.py
 TikTokLive/client/web/routes/fetch_image.py
 TikTokLive/client/web/routes/fetch_is_live.py
-TikTokLive/client/web/routes/fetch_room_id.py
+TikTokLive/client/web/routes/fetch_room_id_api.py
+TikTokLive/client/web/routes/fetch_room_id_html.py
 TikTokLive/client/web/routes/fetch_room_info.py
 TikTokLive/client/web/routes/fetch_sign.py
 TikTokLive/client/web/routes/fetch_video.py
 TikTokLive/client/ws/__init__.py
 TikTokLive/client/ws/ws_client.py
 TikTokLive/events/__init__.py
 TikTokLive/events/base_event.py
```

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/client/base.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/client/base.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/client/client.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/client/client.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/client/config.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/client/config.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/client/httpx.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/client/httpx.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/client/wsclient.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/client/wsclient.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/proto/tiktok_schema_pb2.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/proto/tiktok_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/proto/utilities.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/proto/utilities.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/types/errors.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/types/errors.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/types/events.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/types/events.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/types/objects.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/types/objects.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/types/utilities.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/types/utilities.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/TikTokLiveLegacy/utilities.py` & `TikTokLive-6.0.4/TikTokLiveLegacy/utilities.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.3/setup.py` & `TikTokLive-6.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # PyPi upload Command
 # rm -r dist ; python setup.py sdist ; python -m twine upload dist/*
 
 manifest: dict = {
     "name": "TikTokLive",
     "license": "MIT",
     "author": "Isaac Kogan",
-    "version": "6.0.3",
+    "version": "6.0.4",
     "email": "info@isaackogan.com"
 }
 
 if __name__ == '__main__':
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
```

