# Comparing `tmp/deepgram-sdk-3.2.4.tar.gz` & `tmp/deepgram-sdk-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgram-sdk-3.2.4.tar", last modified: Fri Apr  5 22:31:44 2024, max compression
+gzip compressed data, was "deepgram-sdk-3.2.5.tar", last modified: Mon Apr  8 17:06:31 2024, max compression
```

## Comparing `deepgram-sdk-3.2.4.tar` & `deepgram-sdk-3.2.5.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.882693 deepgram-sdk-3.2.4/deepgram/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.882693 deepgram-sdk-3.2.4/deepgram/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.886693 deepgram-sdk-3.2.4/deepgram/audio/microphone/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/audio/microphone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/audio/microphone/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/audio/microphone/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/audio/microphone/microphone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.886693 deepgram-sdk-3.2.4/deepgram/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/abstract_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/abstract_sync_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.886693 deepgram-sdk-3.2.4/deepgram/clients/analyze/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.886693 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/listen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/live/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/live/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21558 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20861 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/manage/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33519 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33112 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/onprem/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/onprem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/onprem/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/deepgram/clients/speak/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-05 22:31:44.000000 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-05 22:31:44.000000 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 22:31:44.000000 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 22:31:44.000000 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 22:31:44.000000 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.466757 deepgram-sdk-3.2.5/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-08 17:06:22.000000 deepgram-sdk-3.2.5/deepgram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.466757 deepgram-sdk-3.2.5/deepgram/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.466757 deepgram-sdk-3.2.5/deepgram/audio/microphone/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/audio/microphone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/audio/microphone/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/audio/microphone/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/audio/microphone/microphone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.470757 deepgram-sdk-3.2.5/deepgram/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/abstract_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/abstract_sync_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.470757 deepgram-sdk-3.2.5/deepgram/clients/analyze/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.470757 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/listen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.470757 deepgram-sdk-3.2.5/deepgram/clients/live/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/live/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21558 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20861 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/manage/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33519 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33112 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/onprem/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/onprem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/onprem/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/deepgram/clients/speak/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-08 17:06:31.000000 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-08 17:06:31.000000 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:06:31.000000 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-08 17:06:31.000000 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 17:06:31.000000 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/setup.py
```

### Comparing `deepgram-sdk-3.2.4/LICENSE` & `deepgram-sdk-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/PKG-INFO` & `deepgram-sdk-3.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 3.2.4
+Version: 3.2.5
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Deepgram
 Author-email: devrel@deepgram.com
 License: MIT
 Keywords: deepgram,deepgram speech-to-text
 Classifier: Intended Audience :: Developers
```

### Comparing `deepgram-sdk-3.2.4/README.md` & `deepgram-sdk-3.2.5/README.md`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/__init__.py` & `deepgram-sdk-3.2.5/deepgram/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023-2024 Deepgram SDK contributors. All Rights Reserved.
 # Use of this source code is governed by a MIT license that can be found in the LICENSE file.
 # SPDX-License-Identifier: MIT
 
 # version
-__version__ = "v3.2.4"
+__version__ = "v3.2.5"
 
 # entry point for the deepgram python sdk
 from .client import Deepgram, DeepgramClient
 from .options import DeepgramClientOptions, ClientOptionsFromEnv
 import logging, verboselogs
 
 # listen client
```

### Comparing `deepgram-sdk-3.2.4/deepgram/audio/microphone/errors.py` & `deepgram-sdk-3.2.5/deepgram/audio/microphone/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/audio/microphone/microphone.py` & `deepgram-sdk-3.2.5/deepgram/audio/microphone/microphone.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/client.py` & `deepgram-sdk-3.2.5/deepgram/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/__init__.py` & `deepgram-sdk-3.2.5/deepgram/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/abstract_async_client.py` & `deepgram-sdk-3.2.5/deepgram/clients/abstract_async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/abstract_sync_client.py` & `deepgram-sdk-3.2.5/deepgram/clients/abstract_sync_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/analyze/__init__.py` & `deepgram-sdk-3.2.5/deepgram/clients/analyze/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/analyze/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/analyze/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/analyze/errors.py` & `deepgram-sdk-3.2.5/deepgram/clients/analyze/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/__init__.py` & `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/async_client.py` & `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/helpers.py` & `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/options.py` & `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Use of this source code is governed by a MIT license that can be found in the LICENSE file.
 # SPDX-License-Identifier: MIT
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 
 from io import BufferedReader
-from typing import Union, Optional
+from typing import List, Union, Optional
 from typing_extensions import TypedDict
 import logging, verboselogs
 
 
 @dataclass_json
 @dataclass
 class AnalyzeOptions:
@@ -23,21 +23,21 @@
 
     callback: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     callback_method: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    custom_intent: Optional[Union[list, str]] = field(
+    custom_intent: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     custom_intent_mode: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    custom_topic: Optional[Union[list, str]] = field(
+    custom_topic: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     custom_topic_mode: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     intents: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
```

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/response.py` & `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/errors.py` & `deepgram-sdk-3.2.5/deepgram/clients/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/helpers.py` & `deepgram-sdk-3.2.5/deepgram/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/listen.py` & `deepgram-sdk-3.2.5/deepgram/clients/listen.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/live/__init__.py` & `deepgram-sdk-3.2.5/deepgram/clients/live/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/live/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/live/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/live/enums.py` & `deepgram-sdk-3.2.5/deepgram/clients/live/enums.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/live/errors.py` & `deepgram-sdk-3.2.5/deepgram/clients/live/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/live/helpers.py` & `deepgram-sdk-3.2.5/deepgram/clients/live/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/live/v1/__init__.py` & `deepgram-sdk-3.2.5/deepgram/clients/live/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/live/v1/async_client.py` & `deepgram-sdk-3.2.5/deepgram/clients/live/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/live/v1/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/live/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/live/v1/options.py` & `deepgram-sdk-3.2.5/deepgram/clients/live/v1/options.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,24 +38,24 @@
     )
     encoding: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     endpointing: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    extra: Optional[Union[list, str]] = field(
+    extra: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     filler_words: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     interim_results: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    keywords: Optional[str] = field(
+    keywords: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     language: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     model: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
@@ -71,27 +71,27 @@
     )
     profanity_filter: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     redact: Optional[Union[List[str], bool, str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    replace: Optional[str] = field(
+    replace: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     sample_rate: Optional[int] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    search: Optional[str] = field(
+    search: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     smart_format: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    tag: Optional[list] = field(
+    tag: Optional[List[str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     tier: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     utterance_end_ms: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
```

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/live/v1/response.py` & `deepgram-sdk-3.2.5/deepgram/clients/live/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/manage/__init__.py` & `deepgram-sdk-3.2.5/deepgram/clients/manage/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/manage/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/manage/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/manage/v1/__init__.py` & `deepgram-sdk-3.2.5/deepgram/clients/manage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/manage/v1/async_client.py` & `deepgram-sdk-3.2.5/deepgram/clients/manage/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/manage/v1/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/manage/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/manage/v1/options.py` & `deepgram-sdk-3.2.5/deepgram/clients/manage/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/manage/v1/response.py` & `deepgram-sdk-3.2.5/deepgram/clients/manage/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/onprem/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/onprem/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/async_client.py` & `deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/__init__.py` & `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/errors.py` & `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/__init__.py` & `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/async_client.py` & `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/helpers.py` & `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/options.py` & `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     )
     callback: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     callback_method: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    custom_intent: Optional[Union[list, str]] = field(
+    custom_intent: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     custom_intent_mode: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    custom_topics: Optional[Union[list, str]] = field(
+    custom_topics: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     custom_topic_mode: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     detect_entities: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
@@ -62,24 +62,24 @@
     )
     dictation: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     encoding: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    extra: Optional[Union[list, str]] = field(
+    extra: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     filler_words: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     intents: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    keywords: Optional[Union[list, str]] = field(
+    keywords: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     language: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     measurements: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
@@ -101,33 +101,33 @@
     )
     punctuate: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     redact: Optional[Union[List[str], bool, str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    replace: Optional[Union[list, str]] = field(
+    replace: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     sample_rate: Optional[int] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    search: Optional[Union[list, str]] = field(
+    search: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     sentiment: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     smart_format: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     summarize: Optional[Union[bool, str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    tag: Optional[list] = field(
+    tag: Optional[List[str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     tier: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     topics: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
```

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/response.py` & `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/read.py` & `deepgram-sdk-3.2.5/deepgram/clients/read.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/speak/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/speak/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/speak/errors.py` & `deepgram-sdk-3.2.5/deepgram/clients/speak/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/speak/v1/async_client.py` & `deepgram-sdk-3.2.5/deepgram/clients/speak/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/speak/v1/client.py` & `deepgram-sdk-3.2.5/deepgram/clients/speak/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/speak/v1/options.py` & `deepgram-sdk-3.2.5/deepgram/clients/speak/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/clients/speak/v1/response.py` & `deepgram-sdk-3.2.5/deepgram/clients/speak/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/errors.py` & `deepgram-sdk-3.2.5/deepgram/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/deepgram/options.py` & `deepgram-sdk-3.2.5/deepgram/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright 2023-2024 Deepgram SDK contributors. All Rights Reserved.
 # Use of this source code is governed by a MIT license that can be found in the LICENSE file.
 # SPDX-License-Identifier: MIT
 
 import logging, verboselogs
 from typing import Dict, Optional
 from .errors import DeepgramApiKeyError
+from deepgram import __version__
+import sys
 import re
 import os
 
 
 class DeepgramClientOptions:
     """
     Represents options for configuring a Deepgram client.
@@ -60,14 +62,17 @@
         if not hasattr(self, "headers") or self.headers is None:
             self.headers = {}
         self.headers["Accept"] = "application/json"
         if self.api_key:
             self.headers["Authorization"] = f"Token {self.api_key}"
         elif "Authorization" in self.headers:
             del self.headers["Authorization"]
+        self.headers["User-Agent"] = (
+            f"@deepgram/sdk/{__version__} python/{sys.version_info[1]}.{sys.version_info[2]}"
+        )
         # Overwrite / add any headers that were passed in
         if headers:
             self.headers.update(headers)
 
 
 class ClientOptionsFromEnv(DeepgramClientOptions):
     def __init__(
```

### Comparing `deepgram-sdk-3.2.4/deepgram_sdk.egg-info/PKG-INFO` & `deepgram-sdk-3.2.5/deepgram_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 3.2.4
+Version: 3.2.5
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Deepgram
 Author-email: devrel@deepgram.com
 License: MIT
 Keywords: deepgram,deepgram speech-to-text
 Classifier: Intended Audience :: Developers
```

### Comparing `deepgram-sdk-3.2.4/deepgram_sdk.egg-info/SOURCES.txt` & `deepgram-sdk-3.2.5/deepgram_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/pyproject.toml` & `deepgram-sdk-3.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.4/setup.py` & `deepgram-sdk-3.2.5/setup.py`

 * *Files identical despite different names*

