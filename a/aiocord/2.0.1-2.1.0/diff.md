# Comparing `tmp/aiocord-2.0.1.tar.gz` & `tmp/aiocord-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocord-2.0.1.tar", last modified: Mon Jun 26 20:47:03 2023, max compression
+gzip compressed data, was "aiocord-2.1.0.tar", last modified: Mon Apr  8 21:05:48 2024, max compression
```

## Comparing `aiocord-2.0.1.tar` & `aiocord-2.1.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.847487 aiocord-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.839486 aiocord-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.839486 aiocord-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 20:46:50.000000 aiocord-2.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-26 20:46:50.000000 aiocord-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-26 20:46:50.000000 aiocord-2.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-26 20:46:50.000000 aiocord-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-26 20:47:03.847487 aiocord-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-26 20:46:50.000000 aiocord-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.843487 aiocord-2.0.1/aiocord/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   264433 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    50483 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.843487 aiocord-2.0.1/aiocord/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/gateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/gateway/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/gateway/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/gateway/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/gateway/vital.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.843487 aiocord-2.0.1/aiocord/http/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/http/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/http/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    34793 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/http/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.843487 aiocord-2.0.1/aiocord/model/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29482 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/model/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/model/mentions.py
--rw-r--r--   0 runner    (1001) docker     (123)   208686 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/model/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    38076 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/model/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/model/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/model/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.843487 aiocord-2.0.1/aiocord/voice/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/voice/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/voice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/voice/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/voice/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/voice/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/voice/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/voice/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/voice/vital.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-06-26 20:46:50.000000 aiocord-2.0.1/aiocord/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.843487 aiocord-2.0.1/aiocord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-26 20:47:03.000000 aiocord-2.0.1/aiocord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-26 20:47:03.000000 aiocord-2.0.1/aiocord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:47:03.000000 aiocord-2.0.1/aiocord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 20:47:03.000000 aiocord-2.0.1/aiocord.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 20:47:03.000000 aiocord-2.0.1/aiocord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 20:47:03.000000 aiocord-2.0.1/aiocord.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.847487 aiocord-2.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.847487 aiocord-2.0.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.847487 aiocord-2.0.1/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/_static/images/github-mark-white.png
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/_static/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.847487 aiocord-2.0.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/_templates/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/_templates/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.847487 aiocord-2.0.1/docs/pages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:47:03.847487 aiocord-2.0.1/docs/pages/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/pages/examples/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/pages/examples/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/pages/examples/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/pages/examples/interact.naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/pages/examples/interact.smart.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/pages/examples/voice.data.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/pages/examples/voice.file.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/pages/examples/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/pages/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-26 20:46:50.000000 aiocord-2.0.1/docs/pages/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:47:03.847487 aiocord-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-26 20:46:50.000000 aiocord-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.937898 aiocord-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.917899 aiocord-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.921899 aiocord-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-08 21:05:36.000000 aiocord-2.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-08 21:05:36.000000 aiocord-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-08 21:05:36.000000 aiocord-2.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-08 21:05:36.000000 aiocord-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-08 21:05:48.933899 aiocord-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-08 21:05:36.000000 aiocord-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.925899 aiocord-2.1.0/aiocord/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   268310 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51561 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.925899 aiocord-2.1.0/aiocord/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/gateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/gateway/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/gateway/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/gateway/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/gateway/vital.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.925899 aiocord-2.1.0/aiocord/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/http/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/http/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35497 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/http/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.929899 aiocord-2.1.0/aiocord/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31456 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/model/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/model/mentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   219519 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/model/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40455 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/model/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/model/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.929899 aiocord-2.1.0/aiocord/voice/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/voice/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/voice/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/voice/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/voice/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/voice/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/voice/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/voice/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/voice/vital.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-04-08 21:05:36.000000 aiocord-2.1.0/aiocord/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.933899 aiocord-2.1.0/aiocord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-08 21:05:48.000000 aiocord-2.1.0/aiocord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-08 21:05:48.000000 aiocord-2.1.0/aiocord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:05:48.000000 aiocord-2.1.0/aiocord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 21:05:48.000000 aiocord-2.1.0/aiocord.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 21:05:48.000000 aiocord-2.1.0/aiocord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 21:05:48.000000 aiocord-2.1.0/aiocord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.933899 aiocord-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.933899 aiocord-2.1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.933899 aiocord-2.1.0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/_static/images/github-mark-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/_static/main.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.933899 aiocord-2.1.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/_templates/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/_templates/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.933899 aiocord-2.1.0/docs/pages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:05:48.933899 aiocord-2.1.0/docs/pages/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/pages/examples/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/pages/examples/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/pages/examples/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/pages/examples/interact.naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/pages/examples/interact.smart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/pages/examples/voice.data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/pages/examples/voice.file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/pages/examples/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/pages/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-08 21:05:36.000000 aiocord-2.1.0/docs/pages/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:05:48.937898 aiocord-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-08 21:05:36.000000 aiocord-2.1.0/setup.py
```

### Comparing `aiocord-2.0.1/.github/workflows/publish.yml` & `aiocord-2.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/.gitignore` & `aiocord-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/LICENSE` & `aiocord-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/PKG-INFO` & `aiocord-2.1.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: aiocord
-Version: 2.0.1
-Summary: A modern API wrapper for Discord.
-Home-page: https://github.com/Exahilosys/aiocord
-License: MIT
-Requires-Python: >=3.11
-Provides-Extra: docs
-License-File: LICENSE
-
 A modern API wrapper for Discord.
 
 Installation
 ------------
 
 .. code-block:: bash
```

### Comparing `aiocord-2.0.1/README.rst` & `aiocord-2.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: aiocord
+Version: 2.1.0
+Summary: A modern API wrapper for Discord.
+Home-page: https://github.com/Exahilosys/aiocord
+License: MIT
+Requires-Python: >=3.11
+License-File: LICENSE
+Requires-Dist: yarl<2.0.0,>=1.9.1
+Requires-Dist: aiohttp<4.0.0,>=3.8.4
+Requires-Dist: vessel<5.0.0,>=4.2.0
+Requires-Dist: pynacl<2.0.0,>=1.5.0
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-paramlinks; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+
 A modern API wrapper for Discord.
 
 Installation
 ------------
 
 .. code-block:: bash
```

### Comparing `aiocord-2.0.1/aiocord/client.py` & `aiocord-2.1.0/aiocord/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5283,14 +5283,114 @@
             data_user = data.get('user')
             core_user = None if data_user is None else _model.objects.User(data_user)
             core = _model.responses.get_self_authorization_information(core_application, core_scopes, core_expires, core_user)
             return core
 
         return self._request(_http.routes.get_self_authorization_information, _resolve, path)
     
+    class ___get_skus_hint(typing.TypedDict):
+
+        pass
+
+    def get_skus(self,
+                 application_id: _model.types.Snowflake,
+                 /,
+                 **fields: ___get_skus_hint):
+        
+        """
+        Use :data:`.http.routes.get_skus`.
+        """
+
+        path = [application_id]
+
+        def _resolve(data):
+            return list(map(_model.objects.SKU, data))
+        
+        return self._request(_http.routes.get_skus, _resolve, path)
+        
+    class ___get_entitlements_hint(typing.TypedDict):
+
+        user_id      : typing.Optional[_model.types.Snowflake]
+        sku_ids      : typing.Optional[list[_model.types.String]]
+        before       : typing.Optional[_model.types.Snowflake]
+        after        : typing.Optional[_model.types.Snowflake]
+        limit        : typing.Optional[_model.types.Integer]
+        guild_id     : typing.Optional[_model.types.Snowflake]
+        exclude_ended: typing.Optional[_model.types.Boolean]
+
+    def get_entitlements(self,
+                         application_id: _model.types.Snowflake,
+                         /,
+                         **fields: ___get_entitlements_hint):
+        
+        """
+        Use :data:`.http.routes.get_entitlements`.
+        """
+
+        path = [application_id]
+
+        try:
+            sku_ids = fields['sku_ids']
+        except KeyError:
+            pass
+        else:
+            fields['sku_ids'] = ','.join(sku_ids)
+
+        query = fields
+
+        def _resolve(data):
+            return list(map(_model.objects.Entitlement, data))
+
+        return self._request(_http.routes.get_entitlements, _resolve, path, query = query)
+    
+    class ___create_entitlement_hint(typing.TypedDict):
+
+        sku_id    : _model.types.String
+        owner_id  : _model.types.Snowflake
+        owner_type: _model.enums.EntitlementOwnerType
+
+    def create_entitlement(self,
+                           application_id: _model.types.Snowflake,
+                           /,
+                           **fields: ___create_entitlement_hint):
+        
+        """
+        Use :data:`.http.routes.create_entitlement`.
+        """
+
+        path = [application_id]
+
+        json = fields
+
+        def _resolve(data):
+            return _model.objects.Entitlement(data)
+
+        return self._request(_http.routes.create_entitlement, _resolve, path, json = json)
+
+    class ___delete_entitlement_hint(typing.TypedDict):
+
+        pass
+
+    def delete_entitlement(self,
+                           application_id: _model.types.Snowflake,
+                           entitlement_id: _model.types.Snowflake,
+                           /,
+                           **fields: ___delete_entitlement_hint):
+        
+        """
+        Use :data:`.http.routes.delete_entitlement`.
+        """
+
+        path = [application_id, entitlement_id]
+
+        def _resolve(data):
+            return None
+
+        return self._request(_http.routes.delete_entitlement, _resolve, path)
+
     def _create_sentinel(self, Event, check, timeout = None):
 
         event = asyncio.Event()
 
         value = NotImplemented
 
         async def callback(*args, **kwargs):
@@ -7518,14 +7618,50 @@
         core_event = _events.DeleteStageInstance(
             guild          = core_guild,
             stage_instance = core_stage_instance
         )
 
         self._dispatch(core_event)
 
+    async def _handle_gateway_create_entitlement(self, shard, data):
+
+        # https://discord.com/developers/docs/monetization/entitlements#new-entitlement
+
+        core_entitlement = _model.objects.Entitlement(data)
+
+        core_event = _events.CreateEntitlement(
+            entitlement = core_entitlement
+        )
+
+        self._dispatch(core_event)
+
+    async def _handle_gateway_update_entitlement(self, shard, data):
+
+        # https://discord.com/developers/docs/monetization/entitlements#updated-entitlement
+
+        core_entitlement = _model.objects.Entitlement(data)
+
+        core_event = _events.UpdateEntitlement(
+            entitlement = core_entitlement
+        )
+
+        self._dispatch(core_event)
+
+    async def _handle_gateway_delete_entitlement(self, shard, data):
+
+        # https://discord.com/developers/docs/monetization/entitlements#deleted-entitlement
+
+        core_entitlement = _model.objects.Entitlement(data)
+
+        core_event = _events.DeleteEntitlement(
+            entitlement = core_entitlement
+        )
+
+        self._dispatch(core_event)
+
     async def _handle_voice_enter(self, voice, data):
 
         data_guild_id = voice.guild_id
 
         if data_guild_id is None:
             core_guild = _model.missing
         else:
@@ -7792,17 +7928,17 @@
                 shard_event_coros.append(shard_event_coro)
                 shard_start_coro = shard.start()
                 shard_start_task = asyncio.create_task(shard_start_coro)
                 shard_start_tasks.append(shard_start_task) 
             await asyncio.gather(*shard_event_coros)
 
     def start(self,
-              intents    : None | _enums.Intents                                     = None,
-              shard_ids  : None | list[int]                                          = None,
-              shard_count: None | int                                                = None,
+              intents    : None | _enums.Intents                                 = None,
+              shard_ids  : None | list[int]                                      = None,
+              shard_count: None | int                                            = None,
               present    : None | typing.Callable[[], _model.protocols.Presence] = None) -> typing.Awaitable[None]:
         
         """
         Start shard connections.
         
         :param intents:
             The intents to identify with.
@@ -7859,22 +7995,20 @@
         await self._handle('voice', event, *args)
     
     async def _start_voice(self, guild_id, channel_id):
 
         async def update_voice_state_check(core, copy):
             return core.voice_state.user_id == self._cache.user.id and core.voice_state.guild_id == guild_id and core.voice_state.channel_id == channel_id
 
-        update_voice_state_coro = self._create_sentinel(_events.UpdateVoiceState, update_voice_state_check)
-        update_voice_state_task = asyncio.create_task(update_voice_state_coro)
+        update_voice_state_task = self._create_sentinel(_events.UpdateVoiceState, update_voice_state_check)
 
         async def update_voice_server_check(core):
             return core.guild.id == guild_id
 
-        update_voice_server_coro = self._create_sentinel(_events.UpdateVoiceServer, update_voice_server_check)
-        update_voice_server_task = asyncio.create_task(update_voice_server_coro)
+        update_voice_server_task = self._create_sentinel(_events.UpdateVoiceServer, update_voice_server_check)
 
         await self._create_self_voice_state(
             guild_id = guild_id, 
             channel_id = channel_id, 
             self_mute = False, 
             self_deaf = False
         )
```

### Comparing `aiocord-2.0.1/aiocord/enums.py` & `aiocord-2.1.0/aiocord/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -359,14 +359,29 @@
     :ddoc:`Voice Server Update </topics/gateway-events#voice-server-update>` 
     """
     update_webhooks                        = 'WEBHOOKS_UPDATE'
     """
     |dsrc| 
     :ddoc:`Webhooks Update </topics/gateway-events#webhooks-update>` 
     """
+    create_entitlement                     = 'ENTITLEMENT_CREATE'
+    """
+    |dsrc|
+    :ddoc:`Entitlement Create` </monetization/entitlements#new-entitlement>
+    """
+    update_entitlement                     = 'ENTITLEMENT_UPDATE'
+    """
+    |dsrc|
+    :ddoc:`Entitlement Update` </monetization/entitlements#updated-entitlement>
+    """
+    delete_entitlement                     = 'ENTITLEMENT_DELETE'
+    """
+    |dsrc|
+    :ddoc:`Entitlement Delete` </monetization/entitlements#deleted-entitlement>
+    """
 
 
 class VoiceEvent(enum.StrEnum):
 
     speak = 'SPEAK'
     """
     A user has spoken.
```

### Comparing `aiocord-2.0.1/aiocord/events.py` & `aiocord-2.1.0/aiocord/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -2352,14 +2352,74 @@
         * - Source
           - Target
         * - body
           -
     """
 
 
+class CreateEntitlement(typing.NamedTuple):
+    
+    """
+    Dispatched on :attr:`.enums.GatewayEvent.create_entitlement`.
+    """
+
+    entitlement: _model.objects.Entitlement
+    """
+    .. list-table::
+        :width: 450px
+        :widths: 50 50
+        :header-rows: 1
+
+        * - Source
+          - Target
+        * - :attr: body
+          -
+    """
+
+
+class UpdateEntitlement(typing.NamedTuple):
+    
+    """
+    Dispatched on :attr:`.enums.GatewayEvent.delete_entitlement`.
+    """
+
+    entitlement: _model.objects.Entitlement
+    """
+    .. list-table::
+        :width: 450px
+        :widths: 50 50
+        :header-rows: 1
+
+        * - Source
+          - Target
+        * - :attr: body
+          -
+    """
+
+  
+class DeleteEntitlement(typing.NamedTuple):
+    
+    """
+    Dispatched on :attr:`.enums.GatewayEvent.delete_entitlement`.
+    """
+
+    entitlement: _model.objects.Entitlement
+    """
+    .. list-table::
+        :width: 450px
+        :widths: 50 50
+        :header-rows: 1
+
+        * - Source
+          - Target
+        * - :attr: body
+          -
+    """
+
+  
 class EnterVoice(typing.NamedTuple):
 
     """
     Dispatched on :attr:`.enums.VoiceEvent.enter`.
     """
 
     guild: _model.objects.Guild
```

### Comparing `aiocord-2.0.1/aiocord/gateway/client.py` & `aiocord-2.1.0/aiocord/gateway/client.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/gateway/errors.py` & `aiocord-2.1.0/aiocord/gateway/errors.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/gateway/vital.py` & `aiocord-2.1.0/aiocord/gateway/vital.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/helpers.py` & `aiocord-2.1.0/aiocord/helpers.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/http/client.py` & `aiocord-2.1.0/aiocord/http/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,7 +278,8 @@
             Used for handling rate limits.
         """
 
         data = await self._request(identity, verb, path, query, json, data, files, headers)
 
         return data
 
+ # type: ignore
```

### Comparing `aiocord-2.0.1/aiocord/http/errors.py` & `aiocord-2.1.0/aiocord/http/errors.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/http/helpers.py` & `aiocord-2.1.0/aiocord/http/helpers.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/http/routes.py` & `aiocord-2.1.0/aiocord/http/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,16 @@
     'create_webhook', 'get_channel_webhooks', 'get_guild_webhooks', 
     'get_webhook', 'get_webhook_via_token', 'update_webhook', 
     'update_webhook_via_token', 'delete_webhook', 'delete_webhook_via_token', 
     'create_webhook_message', 'create_webhook_message_slack_compatible', 
     'create_webhook_message_github_compatible', 'get_webhook_message', 
     'update_webhook_message', 'delete_webhook_message', 'get_gateway', 
     'get_gateway_bot', 'get_self_application_information',  
-    'get_self_authorization_information'
+    'get_self_authorization_information', 'get_skus', 'get_entitlements', 
+    'create_entitlement', 'delete_entitlement'
 )
 
 
 class Route:
     
     """
     Contains all necessary data to perform a targeted request.
@@ -1178,8 +1179,32 @@
 :ddoc:`Get Current Bot Application Information </topics/oauth2#get-current-bot-application-information>`
 """
 
 get_self_authorization_information = Route('GET', '/oauth2/@me')
 """
 |dsrc|
 :ddoc:`Get Current Authorization Information </topics/oauth2#get-current-authorization-information>`
+"""
+
+get_skus = Route('GET', '/applications/{0}/skus')
+"""
+|dsrc|
+:ddoc:`List SKUs </monetization/skus#list-skus>`
+"""
+
+get_entitlements = Route('GET', '/applications/{0}/entitlements')
+"""
+|dsrc|
+:ddoc:`List Entitlements <//monetization/entitlements#create-test-entitlement>`
+"""
+
+create_entitlement = Route('POST', '/applications/{0}/entitlements')
+"""
+|dsrc|
+:ddoc:`Create Test Entitlement </monetization/entitlements#create-test-entitlement>`
+"""
+
+delete_entitlement = Route('DELETE', '/applications/{0}/entitlements/{1}')
+"""
+|dsrc|
+:ddoc:`Delete Test Entitlement </monetization/entitlements#delete-test-entitlement>`
 """
```

### Comparing `aiocord-2.0.1/aiocord/model/enums.py` & `aiocord-2.1.0/aiocord/model/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 
 __all__ = (
     'ApplicationCommandType', 'StatusType', 'Locale',
     'Permissions', 'ApplicationCommandOptionType', 'ChannelType', 
     'MessageComponentType', 'MessageButtonComponentStyle', 
     'MessageTextInputComponentStyle', 'InteractionType', 
-    'InteractionResponseType', 'ApplicationFlags', 
+    'InteractionContextType', 'InteractionResponseType', 
+    'ApplicationIntegrationType', 'ApplicationFlags', 
     'ApplicationRoleConnectionMetadataType', 'AuditLogEvent', 
     'OptionalAuditLogEntryInfoOverwrittenEntityType', 
     'AutoModerationTriggerType', 'AutoModerationRuleKeywordPresetType', 
     'AutoModerationRuleEventType', 'AutoModerationActionType', 
     'ChannelVideoQualityMode', 'ChannelFlags', 'ChannelSortOrderType', 
     'ForumLayoutType', 'MessageType', 'MessageActivityType', 'MessageFlags', 
     'OverwriteType', 'EmbedType', 'AllowedMentionsType', 
@@ -20,15 +21,16 @@
     'GuildMemberFlags', 'IntegrationExpireBehaviorType', 
     'GuildOnboardingPromptType', 'GuildScheduledEventPrivacyLevel', 
     'GuildScheduledEventEntityType', 'GuildScheduledEventStatus', 
     'InviteTargetType', 'StageInstancePrivacyLevel', 'StickerType', 
     'StickerFormatType', 'UserFlags', 'UserPremiumType', 
     'ConnectionVisibilityType', 'WebhookType', 'ActivityType', 
     'ActivityFlags', 'TeamMemberMembershipState', 'WidgetStyleOption',
-    'SpeechFlags', 'TimestampStyle'
+    'SpeechFlags', 'TimestampStyle', 'SKUType', 'SKUFlags', 'EntitlementType',
+    'EntitlementOwnerType'
 )
 
 
 class EnumMeta(enum.EnumType):
 
     def __call__(self, data, *args, **kwargs):
         try:
@@ -157,14 +159,16 @@
     create_private_threads              = 1 << 36
     use_external_stickers               = 1 << 37
     send_messages_in_threads            = 1 << 38
     use_embedded_activities             = 1 << 39
     moderate_members                    = 1 << 40
     view_creator_monetization_analytics = 1 << 41
     use_soundboard                      = 1 << 42
+    create_guild_expressions            = 1 << 43
+    create_events                       = 1 << 44
     send_voice_messages                 = 1 << 46
 
 
 class ApplicationCommandOptionType(enum.IntEnum, metaclass = EnumMeta):
 
     """
     |dsrc| 
@@ -199,14 +203,15 @@
     guild_announcement  = 5
     announcement_thread = 10
     public_thread       = 11
     private_thread      = 12
     guild_stage_voice   = 13
     guild_directory     = 14
     guild_forum         = 15
+    guild_media         = 16
 
 
 
 class ApplicationCommandPermissionType(enum.IntEnum, metaclass = EnumMeta):
 
     """
     |dsrc| 
@@ -244,20 +249,31 @@
 
     primary   = 1
     secondary = 2
     success   = 3
     danger    = 4
     link      = 5
 
+class MessageSelectMenuComponentDefaultValueType(enum.StrEnum, metaclass = EnumMeta):
+
+
+    """
+    |dsrc| 
+    :ddoc:`Select Meny Default Value Types </interactions/message-components#select-menu-object-select-default-value-structure>`
+    """
+
+    user = 'user'
+    role = 'role'
+    channel = 'channel'
 
 class MessageTextInputComponentStyle(enum.IntEnum, metaclass = EnumMeta):
 
     """
     |dsrc| 
-    :ddoc:`Text Inputs Text Input Styles </interactions/message-components#text-inputs-text-input-styles>`
+    :ddoc:`Text Input Styles </interactions/message-components#text-inputs-text-input-styles>`
     """
 
     short = 1
     paragraph = 2
 
 
 class InteractionType(enum.IntEnum, metaclass = EnumMeta):
@@ -270,28 +286,52 @@
     ping                             = 1
     application_command              = 2
     message_component                = 3
     application_command_autocomplete = 4
     modal_submit                     = 5
 
 
+class InteractionContextType(enum.IntEnum, metaclass = EnumMeta):
+
+    """
+    |dsrc| 
+    :ddoc:`Interaction Context Types </interactions/receiving-and-responding#interaction-object-interaction-context-types>`
+    """
+
+    guild           = 0
+    bot_dm          = 1
+    private_channel = 2
+    
+
 class InteractionResponseType(enum.IntEnum, metaclass = EnumMeta):
 
     """
     |dsrc| 
     :ddoc:`Interaction Callback Types </interactions/receiving-and-responding#interaction-response-object-interaction-callback-type>`
     """
 
     pong                                    = 1
     channel_message_with_source             = 4
     deferred_channel_message_with_source    = 5
     deferred_update_message                 = 6
     update_message                          = 7
     application_command_autocomplete_result = 8
     modal                                   = 9
+    premium_required                        = 10
+
+
+class ApplicationIntegrationType(enum.IntEnum, metaclass = EnumMeta):
+
+    """
+    |dsrc| 
+    :ddoc:`Application Integration Types </resources/application#application-object-application-integration-types>`
+    """
+
+    guild_install = 0
+    user_install  = 1
 
 
 class ApplicationFlags(enum.IntFlag, metaclass = EnumMeta):
 
     """
     |dsrc| 
     :ddoc:`Application Flags </resources/application#application-object-application-flags>`
@@ -986,8 +1026,52 @@
 
     short_time      = 't'
     long_time       = 'T'
     short_date      = 'd'
     long_date       = 'D'
     short_date_time = 'f'
     long_date_time  = 'F'
-    relative_time   = 'R'
+    relative_time   = 'R'
+
+
+class SKUType(enum.IntEnum):
+
+    """
+    |dsrc|
+    :ddoc:`SKU Types </monetization/skus#sku-object-sku-types>`
+    """
+
+    subscription       = 5
+    subscription_group = 6
+
+
+class SKUFlags(enum.IntFlag):
+
+    """
+    |dsrc|
+    :ddoc:`SKU Flags </monetization/skus#sku-object-sku-flags>`
+    """
+
+    available          = 1 << 2
+    guild_subscription = 1 << 7
+    user_subscription  = 1 << 8
+
+
+class EntitlementType(enum.IntEnum):
+
+    """
+    |dsrc|
+    :ddoc:`Entitlement Types </monetization/entitlements#entitlement-object-entitlement-types>`
+    """
+
+    application_subscription = 8
+
+
+class EntitlementOwnerType(enum.IntEnum):
+
+    """
+    |dsrc|
+    :ddoc:`Entitlement Owner Type </monetization/entitlements#create-test-entitlement>`
+    """
+
+    guild_subscription = 1
+    user_subscription  = 2
```

### Comparing `aiocord-2.0.1/aiocord/model/images.py` & `aiocord-2.1.0/aiocord/model/images.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/model/mentions.py` & `aiocord-2.1.0/aiocord/model/mentions.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/model/objects.py` & `aiocord-2.1.0/aiocord/model/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,25 +44,31 @@
     ),
     'options': vessel.SetField(
         create = lambda path, data: _types.Collection(ApplicationCommandOption, data)
     ),
     'default_member_permissions': vessel.SetField(
         create = lambda path, data: _enums.Permissions(data)
     ),
-    'dm_permission': vessel.SetField(
-        create = lambda path, data: _types.Boolean(data)
-    ),
+    # 'dm_permission': vessel.SetField(
+    #     create = lambda path, data: _types.Boolean(data)
+    # ),
     'default_permission': vessel.SetField(
         create = lambda path, data: _types.Boolean(data)
     ),
     'nsfw': vessel.SetField(
         create = lambda path, data: _types.Boolean(data)
     ),
     'version': vessel.SetField(
         create = lambda path, data: _types.Snowflake(data)
+    ),
+    'integration_types': vessel.SetField(
+        create = lambda path, data: _types.Collection(_enums.ApplicationIntegrationType, data)
+    ),
+    'contexts': vessel.SetField(
+        create = lambda path, data: _types.Collection(_enums.InteractionContextType, data)
     )
 }
 
 
 class ApplicationCommand(_types.Object[_protocols.ApplicationCommand], fields = _ApplicationCommand_fields):
 
     """
@@ -129,15 +135,15 @@
     """
     |dsrc| **default_member_permissions**
     """
     dm_permission: _types.Boolean = vessel.GetField(
         select = lambda root: root['dm_permission']
     )
     """
-    |dsrc| **dm_permission**
+    |dsrc| **dm_permission** (deprecated)
     """
     default_permission: _types.Boolean = vessel.GetField(
         select = lambda root: root['default_permission']
     )
     """
     |dsrc| **default_permission**
     """
@@ -149,14 +155,26 @@
     """
     version: _types.Snowflake = vessel.GetField(
         select = lambda root: root['version']
     )
     """
     |dsrc| **version**
     """
+    integration_types: _types.Collection[_enums.ApplicationIntegrationType] = vessel.GetField(
+        select = lambda root: root['integration_types']
+    )
+    """
+    |dsrc| **integration_types**
+    """
+    context_types: _types.Collection[_enums.InteractionContextType] = vessel.GetField(
+        select = lambda root: root['contexts']
+    )
+    """
+    |dsrc| **contexts**
+    """
 
     def mention(self):
 
         """
         Get the mention.
         """
 
@@ -585,14 +603,17 @@
     ),
     'channel_types': vessel.SetField(
         create = lambda path, data: _types.Collection(_enums.ChannelType, data)
     ),
     'placeholder': vessel.SetField(
         create = lambda path, data: _types.String(data)
     ),
+    'default_values': vessel.SetField(
+        create = lambda path, data: _types.Collection(MessageSelectMenuComponentDefaultValue, data)
+    ),
     'min_values': vessel.SetField(
         create = lambda path, data: _types.Integer(data)
     ),
     'max_values': vessel.SetField(
         create = lambda path, data: _types.Integer(data)
     ),
     'disabled': vessel.SetField(
@@ -633,14 +654,20 @@
     """
     placeholder: _types.String = vessel.GetField(
         select = lambda root: root['placeholder']
     )
     """
     |dsrc| **placeholder**
     """
+    default_values: _types.Collection['MessageSelectMenuComponentDefaultValue'] = vessel.GetField(
+        select = lambda root: root['default_values']
+    )
+    """
+    |dsrc| **default_values**
+    """
     min_values: _types.Integer = vessel.GetField(
         select = lambda root: root['min_values']
     )
     """
     |dsrc| **min_values**
     """
     max_values: _types.Integer = vessel.GetField(
@@ -709,14 +736,41 @@
     default: _types.Boolean = vessel.GetField(
         select = lambda root: root['default']
     )
     """
     |dsrc| **default**
     """
 
+_MessageSelectMenuComponentDefaultValue_fields = {
+    'id': vessel.SetField(
+        create = lambda path, data: _types.Snowflake(data)
+    ),
+    'type': vessel.SetField(
+        create = lambda path, data: _enums.MessageSelectMenuComponentDefaultValueType(data)
+    )
+}
+
+class MessageSelectMenuComponentDefaultValue(_types.Object[_protocols.MessageSelectMenuComponentDefaultValue], fields = _MessageSelectMenuComponentDefaultValue_fields):
+
+    """
+    |dsrc| :ddoc:`Select Default Value Structure </interactions/message-components#select-menu-object-select-default-value-structure>`
+    """
+
+    id: _types.Snowflake = vessel.GetField(
+        select = lambda root: root['id']
+    )
+    """
+    |dsrc| **id**
+    """
+    type: _enums.MessageSelectMenuComponentDefaultValueType = vessel.GetField(
+        select = lambda root: root['type']
+    )
+    """
+    |dsrc| **type**
+    """
 
 _MessageTextInputComponent_fields = {
     'type': vessel.SetField(
         create = lambda path, data: _enums.MessageComponentType(data)
     ),
     'custom_id': vessel.SetField(
         create = lambda path, data: _types.String(data)
@@ -863,14 +917,31 @@
         create = lambda path, data: _types.String(data)
     ),
     'locale': vessel.SetField(
         create = lambda path, data: _types.String(data)
     ),
     'guild_locale': vessel.SetField(
         create = lambda path, data: _types.String(data)
+    ),
+    'entitlements': vessel.SetField(
+        create = lambda path, data: _types.Collection(Entitlement, data)
+    ),
+    'authorizing_integration_owners': vessel.SetField(
+        create = lambda path, data: dict(
+            map(
+                lambda item: (
+                    _enums.ApplicationIntegrationType(item[0]),
+                    _types.Snowflake(item[1])
+                ),
+                data.items()
+            )
+        )
+    ),
+    'context': vessel.SetField(
+        create = lambda path, data: _enums.InteractionContextType(data)
     )
 }
 
 
 class Interaction(_types.Object[_protocols.Interaction], fields = _Interaction_fields):
 
     """
@@ -963,14 +1034,32 @@
     """
     guild_locale: _types.String = vessel.GetField(
         select = lambda root: root['guild_locale']
     )
     """
     |dsrc| **guild_locale**
     """
+    entitlements: _types.Collection['Entitlement'] = vessel.GetField(
+        select = lambda root: root['entitlements']
+    )
+    """
+    |dsrc| **entitlements**
+    """
+    authorizing_integration_owners: dict[_enums.ApplicationIntegrationType, _types.Snowflake] = vessel.GetField(
+        select = lambda root: root['authorizing_integration_owners']
+    )
+    """
+    |dsrc| **authorizing_integration_owners**
+    """
+    context: _enums.InteractionContextType = vessel.GetField(
+        select = lambda root: root['context']
+    )
+    """
+    |dsrc| **context**
+    """
 
 
 _ApplicationCommandInteractionData_fields = {
     'id': vessel.SetField(
         create = lambda path, data: _types.Snowflake(data),
         unique = True
     ),
@@ -994,15 +1083,15 @@
     )
 }
 
 
 def _ApplicationCommandInteractionData_keyify(path, data):
 
     data_id = data['id']
-    core_id = _types.Snowflake(data_id)
+    core_id: _types.Snowflake(data_id)
 
     return core_id
 
 
 class ApplicationCommandInteractionData(_types.Object[_protocols.ApplicationCommandInteractionData], fields = _ApplicationCommandInteractionData_fields, keyify = _ApplicationCommandInteractionData_keyify):
 
     """
@@ -1424,22 +1513,33 @@
         create = lambda path, data: ApplicationInstallParams(data)
     ),
     'custom_install_url': vessel.SetField(
         create = lambda path, data: _types.String(data)
     ),
     'role_connections_verification_url': vessel.SetField(
         create = lambda path, data: _types.String(data)
+    ),
+    'integration_types_config': vessel.SetField(
+        create  = lambda path, data: dict(
+            map(
+                lambda item: (
+                    _enums.ApplicationIntegrationType(item[0]),
+                    ApplicationIntegrationTypeConfiguration(item[1])
+                ),
+                data.items()
+            )
+        )
     )
 }
 
 
 def _Application_identify(path, data):
 
     data_id = data['id']
-    core_id = _types.Snowflake(data_id)
+    core_id: _types.Snowflake(data_id)
 
     return core_id
 
 
 class Application(_types.Object[_protocols.Application], fields = _Application_fields):
 
     """
@@ -1568,14 +1668,20 @@
     """
     role_connections_verification_url: _types.String = vessel.GetField(
         select = lambda root: root['role_connections_verification_url']
     )
     """
     |dsrc| **role_connections_verification_url**
     """
+    integration_type_configs: dict[_enums.ApplicationIntegrationType, 'ApplicationIntegrationTypeConfiguration'] = vessel.GetField(
+        select = lambda root: root['role_connections_verification_url']
+    )
+    """
+    |dsrc| **integration_types_config**
+    """
 
     def icon_url(self, **kwargs: typing.Unpack[_images._make_hint]):
 
         """
         Get the icon url.
         """
 
@@ -1594,14 +1700,35 @@
         """
         Get the asset url.
         """
 
         return _images.application_asset(self.id, asset_id, **kwargs)
 
 
+_ApplicationIntegrationTypeConfiguration_fields = {
+    'oauth2_install_params': vessel.SetField(
+        create = lambda path, data: ApplicationInstallParams(data)
+    )
+}
+
+
+class ApplicationIntegrationTypeConfiguration(_types.Object[_protocols.ApplicationIntegrationTypeConfiguration], fields = _ApplicationIntegrationTypeConfiguration_fields):
+
+    """
+    |dsrc| :ddoc:`Application Integration Type Configuration Object </resources/application#application-object-application-integration-type-configuration-object>`
+    """
+
+    oauth2_install_params: 'ApplicationInstallParams' = vessel.GetField(
+        select = lambda root: root['oauth2_install_params']
+    )
+    """
+    |dsrc| **oauth2_install_params**
+    """
+
+
 _ApplicationInstallParams_fields = {
     'scopes': vessel.SetField(
         create = lambda path, data: _types.Collection(_types.String, data)
     ),
     'permissions': vessel.SetField(
         create = lambda path, data: _enums.Permissions(data)
     )
@@ -2058,15 +2185,15 @@
     )
 }
 
 
 def _AutoModerationRule_identify(path, data):
 
     data_id = data['id']
-    core_id = _types.Snowflake(data_id)
+    core_id: _types.Snowflake(data_id)
 
     return core_id
 
 
 class AutoModerationRule(_types.Object[_protocols.AutoModerationRule], fields = _AutoModerationRule_fields):
 
     """
@@ -2388,15 +2515,15 @@
     )
 }
 
 
 def _Channel_identify(path, data):
 
     data_id = data['id']
-    core_id = _types.Snowflake(data_id)
+    core_id: _types.Snowflake(data_id)
 
     return core_id
 
 
 class Channel(_types.Object[_protocols.Channel], fields = _Channel_fields):
 
     """
@@ -2704,17 +2831,17 @@
     ),
     'flags': vessel.SetField(
         create = lambda path, data: _enums.MessageFlags(data)
     ),
     'referenced_message': vessel.SetField(
         create = lambda path, data: Message(data)
     ),
-    'interaction': vessel.SetField(
-        create = lambda path, data: MessageInteraction(data)
-    ),
+    # 'interaction': vessel.SetField(
+    #     create = lambda path, data: MessageInteraction(data)
+    # ),
     'thread': vessel.SetField(
         create = lambda path, data: Channel(data)
     ),
     'components': vessel.SetField(
         create = lambda path, data: _types.Collection(lambda data: _Message_fields_get_components_subtype(data)(data), data)
     ),
     'sticker_items': vessel.SetField(
@@ -2724,14 +2851,17 @@
     #     create = lambda path, data: _types.Collection(Sticker, data)
     # ),
     'position': vessel.SetField(
         create = lambda path, data: _types.Integer(data)
     ),
     'role_subscription_data': vessel.SetField(
         create = lambda path, data: RoleSubscriptionData(data)
+    ),
+    'interaction_metadata': vessel.SetField(
+        create = lambda path, data: MessageInteractionMetadata(data)
     )
 }
 
 
 class Message(_types.Object[_protocols.Message], fields = _Message_fields):
 
     """
@@ -2882,15 +3012,15 @@
     """
     |dsrc| **referenced_message**
     """
     interaction: 'MessageInteraction' = vessel.GetField(
         select = lambda root: root['interaction']
     )
     """
-    |dsrc| **interaction**
+    |dsrc| **interaction** (deprecated)
     """
     thread: 'Channel' = vessel.GetField(
         select = lambda root: root['thread']
     )
     """
     |dsrc| **thread**
     """
@@ -2914,14 +3044,99 @@
     """
     role_subscription_data: 'RoleSubscriptionData' = vessel.GetField(
         select = lambda root: root['role_subscription_data']
     )
     """
     |dsrc| **role_subscription_data**
     """
+    interaction_metadata: 'MessageInteractionMetadata' = vessel.GetField(
+        select = lambda root: root['interaction_metadata']
+    )
+    """
+    |dsrc| **interaction_metadata**
+    """
+
+
+_MessageInteractionMetadata_fields = {
+    'id': vessel.SetField(
+        create = lambda path, data: _types.Snowflake(data['id'])
+    ),
+    'type': vessel.SetField(
+        create = lambda path, data: _enums.InteractionType(data['type'])
+    ),
+    'user_id': vessel.SetField(
+        create = lambda path, data: _types.Snowflake(data['user_id'])
+    ),
+    'authorizing_integration_owners': vessel.SetField(
+        create = lambda path, data: dict(
+            map(
+                lambda item: (
+                    _enums.ApplicationIntegrationType(item[0]),
+                    item[1]
+                ),
+                data.items()
+            )
+        )
+    ),
+    'original_response_message_id': vessel.SetField(
+        create = lambda path, data: _types.Snowflake(data['original_response_message_id'])
+    ),
+    'triggering_interaction_metadata': vessel.SetField(
+        create = lambda path, data: MessageInteractionMetadata(data['triggering_interaction_metadata'])
+    )
+}
+
+class MessageInteractionMetadata(_types.Object[_protocols.MessageInteractionMetadata], fields = _MessageInteractionMetadata_fields):
+
+    """
+    |dsrc| :ddoc:`Message Interaction Metadata Structure </resources/channel#message-interaction-metadata-object-message-interaction-metadata-structure`
+    """
+
+    id: _types.Snowflake = vessel.GetField(
+        select = lambda root: root['id']
+    )
+    """
+    |dsrc| **id**
+    """
+    type: _enums.InteractionType = vessel.GetField(
+        select = lambda root: root['type']
+    )
+    """
+    |dsrc| **type**
+    """
+    user_id: _types.Snowflake = vessel.GetField(
+        select = lambda root: root['user_id']
+    )
+    """
+    |dsrc| **user_id**
+    """
+    authorizing_integration_owners: dict[_enums.ApplicationIntegrationType, _enums.InteractionContextType] = vessel.GetField(
+        select = lambda root: root['authorizing_integration_owners']
+    )
+    """
+    |dsrc| **authorizing_integration_owners**
+    """
+    original_response_message_id: _types.Snowflake = vessel.GetField(
+        select = lambda root: root['original_response_message_id']
+    )
+    """
+    |dsrc| **original_response_message_id**
+    """
+    interacted_message_id: _types.Snowflake = vessel.GetField(
+        select = lambda root: root['interacted_message_id']
+    )
+    """
+    |dsrc| **interacted_message_id**
+    """
+    triggering_interaction_metadata: 'MessageInteractionMetadata' = vessel.GetField(
+        select = lambda root: root['triggering_interaction_metadata']
+    )
+    """
+    |dsrc| **triggering_interaction_metadata**
+    """
     
 
 _MessageActivity_fields = {
     'type': vessel.SetField(
         create = lambda path, data: _enums.MessageActivityType(data)
     ),
     'party_id': vessel.SetField(
@@ -7619,8 +7834,122 @@
     |dsrc| **team_id**
     """
     user: 'User' = vessel.GetField(
         select = lambda root: root['user']
     )
     """
     |dsrc| **user**
-    """
+    """
+
+
+_SKU_fields = {
+    'id': vessel.SetField(
+        create = lambda path, data: _types.Snowflake(data)
+    ),
+    'type': vessel.SetField(
+        create = lambda path, data: _enums.SKUType(data)
+    ),
+    'application_id': vessel.SetField(
+        create = lambda path, data: _types.Snowflake(data)
+    ),
+    'name': vessel.SetField(
+        create = lambda path, data: _types.String(data)
+    ),
+    'slug': vessel.SetField(
+        create = lambda path, data: _types.String(data)
+    ),
+    'flags': vessel.SetField(
+        create = lambda path, data: _enums.SKUFlags(data)
+    )
+}
+
+
+class SKU(_types.Object[_protocols.SKU], fields = _SKU_fields):
+
+    """
+    |dsrc| :ddoc:`SKU Structure </monetization/skus#sku-object-sku-structure>`
+    """
+
+    id: _types.Snowflake = vessel.GetField(
+        select = lambda root: ['id']
+    )
+    type: _enums.SKUType = vessel.GetField(
+        select = lambda root: ['type']
+    )
+    application_id: _types.Snowflake = vessel.GetField(
+        select = lambda root: ['application_id']
+    )
+    name: _types.String = vessel.GetField(
+        select = lambda root: ['name']
+    )
+    slug: _types.String = vessel.GetField(
+        select = lambda root: ['slug']
+    )
+    flags: _enums.SKUFlags = vessel.GetField(
+        select = lambda root: ['flags']
+    )
+
+
+_Entitlement_fields = {
+    'id': vessel.SetField(
+        create = lambda path, data: _types.Snowflake(data)
+    ),
+    'sku_id': vessel.SetField(
+        create = lambda path, data: _types.Snowflake(data)
+    ),
+    'application_id': vessel.SetField(
+        create = lambda path, data: _types.Snowflake(data)
+    ),
+    'user_id': vessel.SetField(
+        create = lambda path, data: _types.Snowflake(data)
+    ),
+    'type': vessel.SetField(
+        create = lambda path, data: _enums.EntitlementType(data)
+    ),
+    'deleted': vessel.SetField(
+        create = lambda path, data: data
+    ),
+    'starts_at': vessel.SetField(
+        create = lambda path, data: _types.ISO8601Timestamp(data)
+    ),
+    'ends_at': vessel.SetField(
+        create = lambda path, data: _types.ISO8601Timestamp(data)
+    ),
+    'guild_id': vessel.SetField(
+        create = lambda path, data: _types.Snowflake(data)
+    )
+}
+
+
+class Entitlement(_types.Object[_protocols.Entitlement], fields = _Entitlement_fields):
+
+    """
+    |dsrc| :ddoc:`Entitlement Structure </monetization/entitlements#entitlement-object-entitlement-structure>`
+    """
+
+    id: _types.Snowflake = vessel.GetField(
+        select = lambda root: _types.Snowflake(root['id'])
+    )
+    sku_id: _types.Snowflake = vessel.GetField(
+        select = lambda root: _types.Snowflake(root['sku_id'])
+    )
+    application_id: _types.Snowflake = vessel.GetField(
+        select = lambda root: _types.Snowflake(root['application_id'])
+    )
+    user_id: _types.Snowflake = vessel.GetField(
+        select = lambda root: _types.Snowflake(root['user_id'])
+    )
+    type = _enums.EntitlementType = vessel.GetField(
+        select = lambda root: _enums.EntitlementType(root['type'])
+    )
+    deleted: _types.Boolean = vessel.GetField(
+        select = lambda path, data: _types.Boolean(data)
+    )
+    starts_at: _types.ISO8601Timestamp = vessel.GetField(
+        select = lambda root: _types.ISO8601Timestamp(root['starts_at'])
+    )
+    ends_at: _types.ISO8601Timestamp = vessel.GetField(
+        select = lambda root: _types.ISO8601Timestamp(root['ends_at'])
+    )
+    guild_id: _types.Snowflake = vessel.GetField(
+        select = lambda root: _types.Snowflake(root['guild_id'])
+    )
```

### Comparing `aiocord-2.0.1/aiocord/model/protocols.py` & `aiocord-2.1.0/aiocord/model/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,41 +5,43 @@
 
 
 __all__ = (
     'ApplicationCommand', 'ApplicationCommandOption', 
     'ApplicationCommandOptionChoice', 'GuildApplicationCommandPermissions',
     'ApplicationCommandPermission', 'MessageActionRowComponent',
     'MessageButtonComponent', 'MessageSelectMenuComponent', 
+    'MessageSelectMenuComponentDefaultValue', 
     'MessageSelectMenuComponentOption', 'MessageTextInputComponent', 
     'Interaction', 'ApplicationCommandInteractionData', 
     'ApplicationCommandInteractionDataOption', 
     'MessageComponentInteractionData', 'ModalSubmitInteractionData', 
     'ResolvedInteractionData', 'MessageInteraction', 'InteractionResponse', 
     'MessageInteractionResponse', 'AutocompleteInteractionResponse',
-    'ModalInteractionResponse', 'Application', 'ApplicationInstallParams', 
+    'ModalInteractionResponse', 'Application', 
+    'ApplicationIntegrationTypeConfiguration','ApplicationInstallParams', 
     'ApplicationRoleConnectionMetadata', 'AuditLog', 'AuditLogEntry', 
     'OptionalAuditLogEntryInfo', 'AuditLogChange', 'AutoModerationRule', 
     'AutoModerationTriggerMetadata', 'AutoModerationAction', 
     'AutoModerationActionMetadata', 'Channel', 'Message', 'MessageActivity', 
-    'MessageReference', 'Reaction', 'FollowedChannel', 'Overwrite', 
-    'ThreadMetadata', 'ThreadMember', 'DefaultReaction', 'ForumTag', 'Embed', 
-    'EmbedThumbnail', 'EmbedVideo', 'EmbedImage', 'EmbedProvider', 
-    'EmbedAuthor', 'EmbedFooter', 'EmbedField', 'Attachment', 
-    'AllowedMentions', 'RoleSubscriptionData', 'Emoji', 'Guild', 
+    'MessageInteractionMetadata', 'MessageReference', 'Reaction', 
+    'FollowedChannel', 'Overwrite', 'ThreadMetadata', 'ThreadMember', 
+    'DefaultReaction', 'ForumTag', 'Embed', 'EmbedThumbnail', 'EmbedVideo', 
+    'EmbedImage', 'EmbedProvider', 'EmbedAuthor', 'EmbedFooter', 'EmbedField', 
+    'Attachment', 'AllowedMentions', 'RoleSubscriptionData', 'Emoji', 'Guild', 
     'GuildWidgetSettings', 'GuildWidget', 'GuildMember', 'Integration', 
     'IntegrationAccount', 'IntegrationApplication', 'Ban', 'WelcomeScreen', 
     'WelcomeScreenChannel', 'GuildOnboarding', 'GuildOnboardingPrompt', 
     'GuildOnboardingPromptOption', 'GuildScheduledEvent', 
     'GuildScheduledEventEntityMetadata', 'GuildScheduledEventUser', 
     'GuildTemplate', 'Invite', 'InviteStageInstance', 'StageInstance', 
     'Sticker', 'StickerPack', 'User', 'Connection', 
     'ApplicationRoleConnection', 'VoiceState', 'VoiceRegion', 
     'Webhook', 'Presence', 'ClientStatus', 'Activity', 'ActivityTimestamps', 
     'ActivityParty', 'ActivityAssets', 'ActivitySecrets', 'ActivityButton', 
-    'Role', 'RoleTags', 'Team', 'TeamMember'
+    'Role', 'RoleTags', 'Team', 'TeamMember', 'SKU', 'Entitlement'
 )
 
 
 class ApplicationCommand(typing.TypedDict):
     
     id                        : _types.Snowflake
     type                      : _enums.ApplicationCommandType
@@ -47,18 +49,20 @@
     guild_id                  : _types.Snowflake
     name                      : _types.String
     name_localizations        : dict[_enums.Locale, _types.String]
     description               : _types.String
     description_localizations : dict[_enums.Locale, _types.String]
     options                   : list['ApplicationCommandOption']
     default_member_permissions: _enums.Permissions
-    dm_permission             : _types.Boolean
+    # dm_permission             : _types.Boolean
     default_permission        : _types.Boolean
     nsfw                      : _types.Boolean
     version                   : _types.Snowflake
+    integration_types         : list[_enums.ApplicationIntegrationType]
+    contexts                  : list[_enums.InteractionContextType]
 
 
 class ApplicationCommandOption(typing.TypedDict):
     
     type                     : _enums.ApplicationCommandOptionType
     name                     : _types.String
     name_localizations       : dict[_enums.Locale, _types.String]
@@ -112,33 +116,40 @@
     custom_id: _types.String
     url      : _types.String
     disabled : _types.Boolean
 
 
 class MessageSelectMenuComponent(typing.TypedDict):
     
-    type         : _enums.MessageComponentType
-    custom_id    : _types.String
-    options      : list['MessageSelectMenuComponentOption']
-    channel_types: list[_enums.ChannelType]
-    placeholder  : _types.String
-    min_values   : _types.Integer
-    max_values   : _types.Integer
-    disabled     : _types.Boolean
+    type          : _enums.MessageComponentType
+    custom_id     : _types.String
+    options       : list['MessageSelectMenuComponentOption']
+    channel_types : list[_enums.ChannelType]
+    placeholder   : _types.String
+    default_values: list['MessageSelectMenuComponentDefaultValue']
+    min_values    : _types.Integer
+    max_values    : _types.Integer
+    disabled      : _types.Boolean
 
 
 class MessageSelectMenuComponentOption(typing.TypedDict):
     
     label      : _types.String
     value      : _types.String
     description: _types.String
     emoji      : 'Emoji'
     default    : _types.Boolean
 
 
+class MessageSelectMenuComponentDefaultValue(typing.TypedDict):
+
+    id: _types.Snowflake
+    type: _enums.MessageSelectMenuComponentDefaultValueType
+
+
 class MessageTextInputComponent(typing.TypedDict):
     
     type       : _types.Integer
     custom_id  : _types.String
     style      : _enums.MessageTextInputComponentStyle
     label      : _types.String
     min_length : _types.Integer
@@ -146,29 +157,32 @@
     required   : _types.Boolean
     value      : _types.String
     placeholder: _types.String
 
 
 class Interaction(typing.TypedDict):
     
-    id             : _types.Snowflake
-    application_id : _types.Snowflake
-    type           : _enums.InteractionType
-    data           : typing.Union['ApplicationCommandInteractionData', 'MessageComponentInteractionData', 'ModalSubmitInteractionData', 'ResolvedInteractionData']
-    guild_id       : _types.Snowflake
-    channel        : 'Channel'
-    channel_id     : _types.Snowflake
-    member         : 'GuildMember'
-    user           : 'User'
-    token          : _types.String
-    version        : _types.Integer
-    message        : 'Message'
-    app_permissions: _types.String
-    locale         : _types.String
-    guild_locale   : _types.String
+    id                            : _types.Snowflake
+    application_id                : _types.Snowflake
+    type                          : _enums.InteractionType
+    data                          : typing.Union['ApplicationCommandInteractionData', 'MessageComponentInteractionData', 'ModalSubmitInteractionData', 'ResolvedInteractionData']
+    guild_id                      : _types.Snowflake
+    channel                       : 'Channel'
+    channel_id                    : _types.Snowflake
+    member                        : 'GuildMember'
+    user                          : 'User'
+    token                         : _types.String
+    version                       : _types.Integer
+    message                       : 'Message'
+    app_permissions               : _types.String
+    locale                        : _types.String
+    guild_locale                  : _types.String
+    entitlements                  : list['Entitlement']
+    authorizing_integration_owners: dict[_enums.ApplicationIntegrationType, _types.Snowflake]
+    context                       : _enums.InteractionContextType
 
 
 class ApplicationCommandInteractionData(typing.TypedDict):
     
     id       : _types.Snowflake
     name     : _types.String
     type     : _types.Integer
@@ -266,14 +280,20 @@
     slug                             : _types.String
     cover_image                      : _types.String
     flags                            : _types.Integer
     tags                             : list[_types.String]
     install_params                   : 'ApplicationInstallParams'
     custom_install_url               : _types.String
     role_connections_verification_url: _types.String
+    integration_types_config         : dict[_enums.ApplicationIntegrationType, 'ApplicationIntegrationTypeConfiguration']
+
+
+class ApplicationIntegrationTypeConfiguration(typing.TypedDict):
+
+    oauth2_install_params: 'ApplicationInstallParams'
 
 
 class ApplicationInstallParams(typing.TypedDict):
     
     scopes     : list[_types.String]
     permissions: _enums.Permissions
 
@@ -438,22 +458,34 @@
     referenced_message    : typing.Optional['Message']
     interaction           : 'MessageInteraction'
     thread                : 'Channel'
     components            : list['MessageActionRowComponent']
     stickers              : list['Sticker']
     position              : _types.Integer
     role_subscription_data: 'RoleSubscriptionData'
+    interaction_metadata  : 'MessageInteractionMetadata'
 
 
 class MessageActivity(typing.TypedDict):
     
     type    : _enums.MessageActivityType
     party_id: _types.String
 
 
+class MessageInteractionMetadata(typing.TypedDict):
+
+    id                             : _types.Snowflake
+    type                           : _enums.InteractionType
+    user_id                        : _types.Snowflake
+    authorizing_integration_owners : dict[_enums.ApplicationIntegrationType, typing.Any]
+    original_response_message_id   : _types.Snowflake
+    interacted_message_id          : _types.Snowflake
+    triggering_interaction_metadata: 'MessageInteractionMetadata'
+
+
 class MessageReference(typing.TypedDict):
     
     message_id        : _types.Snowflake
     channel_id        : _types.Snowflake
     guild_id          : _types.Snowflake
     fail_if_not_exists: _types.Boolean
 
@@ -1098,8 +1130,31 @@
 
 
 class TeamMember(typing.TypedDict):
     
     membership_state: _enums.TeamMemberMembershipState
     permissions     : list[_types.String]
     team_id         : _types.Snowflake
-    user            : 'User'
+    user            : 'User'
+
+
+class SKU(typing.TypedDict):
+
+    id            : _types.Snowflake
+    type          : _enums.SKUType
+    application_id: _types.Snowflake
+    name          : _types.String
+    slug          : _types.String
+    flags         : _enums.SKUFlags
+
+
+class Entitlement(typing.TypedDict):
+
+    id            : _types.Snowflake
+    sku_id        : _types.Snowflake
+    application_id: _types.Snowflake
+    user_id       : _types.Snowflake
+    type          : _enums.EntitlementType
+    deleted       : _types.Boolean
+    starts_at     : _types.ISO8601Timestamp
+    ends_at       : _types.ISO8601Timestamp
+    guild_id      : _types.Snowflake
```

### Comparing `aiocord-2.0.1/aiocord/model/responses.py` & `aiocord-2.1.0/aiocord/model/responses.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/model/types.py` & `aiocord-2.1.0/aiocord/model/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     @property
     def datetime(self) -> datetime.datetime:
 
         """
         The datetime object representation.
         """
 
-        return datetime.datetime.fromtimestamp(self)
+        return datetime.datetime.fromtimestamp(self, tz = datetime.timezone.utc)
     
     def mention(self, style: _enums.TimestampStyle = None):
 
         """
         Get the mention.
 
         :param style:
@@ -97,8 +97,8 @@
     @property
     def timestamp(self, epoch = 1420070400000) -> Timestamp:
 
         """
         The internal timestamp.
         """
 
-        return Timestamp((int(self) >> 22) + epoch)
+        return Timestamp(((int(self) >> 22) + epoch) / 1000)
```

### Comparing `aiocord-2.0.1/aiocord/utils.py` & `aiocord-2.1.0/aiocord/utils.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/vendor.py` & `aiocord-2.1.0/aiocord/vendor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,55 @@
 import os
+import sys
 import asyncio
 import argparse
 import json
 import functools
 import operator
+import contextlib
+import queue
+import logging
+import logging.handlers
 
 from . import helpers as _helpers
 from . import enums   as _enums
 from . import events  as _events
 from . import client  as _client
 from . import utils   as _utils
 from . import widget  as _widget
 
 
 __all__ = ('main',)
 
 
+@contextlib.contextmanager
+def _maintain_logging():
+
+    store = queue.Queue()
+    queue_handler = logging.handlers.QueueHandler(store)
+    basic_handler = logging.StreamHandler()
+    listener = logging.handlers.QueueListener(store, basic_handler)
+
+    LoggerBase = logging.getLoggerClass()
+
+    class Logger(LoggerBase):
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.handlers.append(queue_handler)
+
+    logging.setLoggerClass(Logger)
+
+    listener.start()
+
+    yield
+
+    listener.stop()
+
+    logging.setLoggerClass(LoggerBase)
+
 _parser = argparse.ArgumentParser(
     description = 'manage a discord client'
 )
 
 _parser.add_argument(
     '--token',
     help = 'the client\'s type-less authentication token (if missing, sought as DISCORD_TOKEN env-var)',
@@ -29,15 +59,15 @@
 
 def _get_client(info):
 
     if (token := info.token) is None:
         try:
             token = os.environ['DISCORD_TOKEN']
         except KeyError:
-            print('token not specified or set in environment')
+            print('token not specified or set in environment', file = sys.stderr)
             exit()
 
     token = 'Bot ' + token
 
     client = _client.Client(token = token)
 
     return client
@@ -52,15 +82,16 @@
 
     info = _parser.parse_args(args)
 
     space = globals()
 
     function = space[f'_main_{info.action}']
     
-    function(info)
+    with _maintain_logging():
+        function(info)
   
 
 _manage_start_parser = _manage_parsers.add_parser(
     'start',
     description = 'start the client'
 )
 
@@ -89,52 +120,58 @@
     '--shard-count',
     help = 'the shard count',
     type = lambda data: int(data),
     default = None,
     required = False
 )
 
+_manage_start_parser.add_argument(
+    '--vendor',
+    help = 'the vendor from which to load the widget (supported: github)',
+    default = None,
+    required = False
+)
+
 _main_start_enter_default_Events = {
     # required for voice
     _events.UpdateVoiceState
 }
 
-async def _main_start_enter(client, path, intents, shard_ids, shard_count):
+async def _main_start_enter(client, vendor, path, intents, shard_ids, shard_count):
 
-    path, name = os.path.split(path)
+    name = object()
 
-    await _widget.load(client, name, path)
+    await _widget.load(client, name, path, vendor = vendor)
 
     Events = set(_main_start_enter_default_Events)
 
     for asset in _widget._assets.values():
         Events.update(asset.Events)
 
     intents |= _utils.get_eventful_intents(Events)
 
-    await client.start(intents, shard_ids, shard_count)
+    await client.start(intents = intents, shard_ids = shard_ids, shard_count = shard_count)
 
     await client.ready()
 
     return name
 
 async def _main_start_leave(client, name):
 
     await client.stop()
 
     await _widget.drop(client, name)
 
-
 def _main_start(info):
 
     loop = asyncio.get_event_loop()
 
     client = _get_client(info)
 
-    coro = _main_start_enter(client, info.path, info.intents, info.shard_ids, info.shard_count)
+    coro = _main_start_enter(client, info.vendor, info.path, info.intents, info.shard_ids, info.shard_count)
     name = loop.run_until_complete(coro)
 
     try:
         loop.run_forever()
     except KeyboardInterrupt:
         pass
     finally:
```

### Comparing `aiocord-2.0.1/aiocord/voice/audio.py` & `aiocord-2.1.0/aiocord/voice/audio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import typing
-import sys
-import os
 import asyncio
 import subprocess
 
 from . import stream as _stream
 
 
 __all__ = ('Audio',)
```

### Comparing `aiocord-2.0.1/aiocord/voice/client.py` & `aiocord-2.1.0/aiocord/voice/client.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/voice/errors.py` & `aiocord-2.1.0/aiocord/voice/errors.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/voice/player.py` & `aiocord-2.1.0/aiocord/voice/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from . import errors as _errors
 from . import audio  as _audio
 
 
 __all__ = ('Player',)
 
 
-
 class Player:
 
     """
     Manages timely sending voice packets.
 
     :param send:
         Used with ``(samples, data)`` for sending.
```

### Comparing `aiocord-2.0.1/aiocord/voice/stream.py` & `aiocord-2.1.0/aiocord/voice/stream.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/voice/vital.py` & `aiocord-2.1.0/aiocord/voice/vital.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/aiocord/widget.py` & `aiocord-2.1.0/aiocord/widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import typing
 import os
 import asyncio
 import functools
 import types
 import weakref
 import inspect
+import itertools
+import aiohttp
+import re
+import io
+import zipfile
+import tempfile
 
 from . import helpers as _helpers
 from . import model   as _model
 from . import client  as _client
 from . import events  as _events
 
 
@@ -31,15 +37,19 @@
     """
     widgets: dict[str, types.ModuleType]
     """
     All currently loaded widgets.
     """
 
 
-def _load_module(name, path, intermediary = '_m_'):
+def _load_module(path, *, ids = itertools.count(0)):
+
+    intermediary = next(ids)
+
+    name = os.path.basename(path)
 
     module_name = f'{__name__}.{intermediary}.{name}'
 
     module = _helpers.load_module_via_path(module_name, path)
 
     return module
 
@@ -104,50 +114,40 @@
         if index < 2:
             continue
         module = inspect.getmodule(frame)
         try:
             asset = _assets[module]
         except KeyError:
             continue
-        return asset
+        break
+    else:
+        asset = None
     
-    return None
-
+    return module, asset
 
-async def _load(client, name, path):
 
-    if path is None:
-        asset = _find_caller_widget_asset()
-        path = '.' if asset is None else os.path.dirname(asset.path)
+async def _load_internal_widget(client, name, module):
 
-    loop = asyncio.get_event_loop()
+    try:
+        await _drop(client, name, pop = False)
+    except KeyError:
+        pass
 
     try:
         modules = _modules_group[client]
     except KeyError:
         modules = _modules_group[client] = weakref.WeakValueDictionary()
 
-    try:
-        await _drop(client, name, pop = False)
-    except KeyError:
-        pass
+    modules[name] = module
 
     if not (application := client.cache.application):
         application = await client.get_self_application_information()
 
     commands = await client.get_global_application_commands(application.id)
 
-    module_path = os.path.join(path, name)
-    
-    load_module = functools.partial(_load_module, name, module_path, intermediary = id(client))
-
-    module = modules[name] = await loop.run_in_executor(None, load_module)
-
-    # module.__name__, name = name, module.__name__
-
     info = Info(client, types.MappingProxyType(modules))
 
     callbacks = []
 
     Events = set()
 
     def load_callback(Event, function):
@@ -198,43 +198,140 @@
     except AttributeError:
         pass
     else:
         await load(info)
 
     client.callbacks.extend(callbacks)
 
-    _assets[module] = types.SimpleNamespace(
-        name = name, 
-        path = path, 
+    asset = _assets[module] = types.SimpleNamespace(
+        name = name,
         info = info, 
         Events = Events,
         callbacks = callbacks
     )
 
+    return asset
+
+
+async def _load_internal(client, name, path):
+
+    loop = asyncio.get_event_loop()
+
+    if path is None:
+        module, asset = _find_caller_widget_asset()
+        if asset is None:
+            raise ModuleNotFoundError('implicit path used with unknown calling widget')
+        path = os.path.dirname(module.__path__[0])
+
+    load_module = functools.partial(_load_module, path)
+
+    module = await loop.run_in_executor(None, load_module)
+    
+    asset = await _load_internal_widget(client, name, module)
+
+    return module
+
+
+async def _load_external_github(session, client, name, author, project, version):
+
+    response = await session.request('GET', f'https://api.github.com/repos/{author}/{project}/tags')
+    tags = await response.json()
+
+    if version is None:
+        tag = max(tags, key = lambda tag: tag['name'])
+    else:
+        version_pattern = re.compile(version)
+        try:
+            tag = next(filter(lambda tag: version_pattern.match(tag['name']), tags))
+        except StopIteration:
+            raise ModuleNotFoundError(f'unknown tag {version} for {author}/{project}')
+    
+    response = await session.request('GET', tag['zipball_url'])
+    data = await response.read()
+    archive = zipfile.ZipFile(io.BytesIO(data))
+
+    loop = asyncio.get_event_loop()
+
+    def load_module():
+        with tempfile.TemporaryDirectory(prefix = __name__ + '_') as project_path_base:
+            archive.extractall(project_path_base)
+            for project_path_name in os.listdir(project_path_base):
+                if any(map(project_path_name.startswith, ('.', '_'))):
+                    continue
+                project_path = os.path.join(project_path_base, project_path_name)
+                if not os.path.isdir(project_path):
+                    continue
+                break
+            else:
+                raise ModuleNotFoundError(f'could not find project directory')
+            module_path = os.path.join(project_path, 'widget')
+            module = _load_module(module_path)
+        return module
+    
+    module = await loop.run_in_executor(None, load_module)
+    
+    asset = await _load_internal_widget(client, name, module)
+
+    return module
+
+
+_load_external_functions = {
+    'github': _load_external_github
+} 
+
+
+async def _load_external(vendor, client, name, path, version):
+
+    function = _load_external_functions[vendor]
+
+    author, project = path.split('/')
+
+    async with aiohttp.ClientSession() as session:
+        module = await function(session, client, name, author, project, version)
+
+    return module
+
+
+async def _load(client, name, path, vendor, *, version = None):
+
+    if vendor is None:
+        function = lambda: _load_internal(client, name, path)
+    else:
+        function = lambda: _load_external(vendor, client, name, path, version)
+
+    module = await function()
+
     return module
 
 
-def load(client: _client.Client, 
-         name  : str, 
-         path  : str = None) -> typing.Awaitable[types.ModuleType]:
+def load(client : _client.Client, 
+         name   : str, 
+         path   : str                      = None,
+         vendor : typing.Literal['github'] = None,
+         *,
+         version: str                      = None) -> typing.Awaitable[types.ModuleType]:
     
     """
     Load a widget by creating and attaching events to the client.
     
     :param client:
         The client to load the widget for.
     :param name:
         The name of the widget, used for identifying in :attr:`.Info.widgets` and :func:`.drop`\ing.
     :param path:
-        The location of the module's parent directory. If not specified, the caller widget's parent directory is used.
+        The location of the package. If not specified, the calling widget's parent directory is used.
+    :param vendor:
+        The vendor from which to download the widget, given that :paramref:`.path` is an the form of ``author/project/version``.
+    :param version:
+        The project version to fetch. The latest is used if not specified. Only valid when :paramref:`.vendor` is used. 
 
     The widget may define a ``__load__(info)`` function, which will be called before callbacks are attached.
     """
 
-    return _load(client, name, path)
+    return _load(client, name, path, vendor, version = version)
 
 
 def _drop_module(name):
 
     _helpers.drop_module(name)
 
 
@@ -259,15 +356,15 @@
     try:
         drop = getattr(module, '__drop__')
     except AttributeError:
         pass
     else:
         await drop(asset.info)
 
-    drop_module = functools.partial(_drop_module, asset.name)
+    drop_module = functools.partial(_drop_module, module.__name__)
 
     await loop.run_in_executor(None, drop_module)
 
 
 def drop(client: _client.Client, 
          name: str) -> typing.Awaitable[None]:
```

### Comparing `aiocord-2.0.1/aiocord.egg-info/PKG-INFO` & `aiocord-2.1.0/aiocord.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 Metadata-Version: 2.1
 Name: aiocord
-Version: 2.0.1
+Version: 2.1.0
 Summary: A modern API wrapper for Discord.
 Home-page: https://github.com/Exahilosys/aiocord
 License: MIT
 Requires-Python: >=3.11
-Provides-Extra: docs
 License-File: LICENSE
+Requires-Dist: yarl<2.0.0,>=1.9.1
+Requires-Dist: aiohttp<4.0.0,>=3.8.4
+Requires-Dist: vessel<5.0.0,>=4.2.0
+Requires-Dist: pynacl<2.0.0,>=1.5.0
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-paramlinks; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 
 A modern API wrapper for Discord.
 
 Installation
 ------------
 
 .. code-block:: bash
```

### Comparing `aiocord-2.0.1/aiocord.egg-info/SOURCES.txt` & `aiocord-2.1.0/aiocord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/Makefile` & `aiocord-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/_static/images/github-mark-white.png` & `aiocord-2.1.0/docs/_static/images/github-mark-white.png`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/_static/main.css` & `aiocord-2.1.0/docs/_static/main.css`

 * *Files 0% similar despite different names*

```diff
@@ -296,8 +296,9 @@
     background-color: var(--color-block-norm);
 }
 
 .document .documentwrapper .bodywrapper .py.class,
 .document .documentwrapper .bodywrapper .py.function,
 .document .documentwrapper .bodywrapper .py.data {
     border-left: 4px solid #ffffff0e;
+    border-bottom-width: 32px;
 }
```

### Comparing `aiocord-2.0.1/docs/_templates/layout.html` & `aiocord-2.1.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/conf.py` & `aiocord-2.1.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 html_static_path = ['_static']
 
 html_css_files = [
     'main.css'
 ]
 
-pygments_style = 'stata-dark'
+pygments_style = 'github-dark'
 
 html_sidebars = {
    '**': ['searchbox.html', 'globaltoc.html']
 }
 
 html_show_copyright = False
```

### Comparing `aiocord-2.0.1/docs/index.rst` & `aiocord-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/make.bat` & `aiocord-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/pages/examples/interact.naive.py` & `aiocord-2.1.0/docs/pages/examples/interact.naive.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/pages/examples/interact.smart.py` & `aiocord-2.1.0/docs/pages/examples/interact.smart.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/pages/examples/voice.data.py` & `aiocord-2.1.0/docs/pages/examples/voice.data.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/pages/examples/voice.file.py` & `aiocord-2.1.0/docs/pages/examples/voice.file.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/pages/examples/widget.py` & `aiocord-2.1.0/docs/pages/examples/widget.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/pages/examples.rst` & `aiocord-2.1.0/docs/pages/examples.rst`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/docs/pages/reference.rst` & `aiocord-2.1.0/docs/pages/reference.rst`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.1/setup.py` & `aiocord-2.1.0/setup.py`

 * *Files identical despite different names*

