# Comparing `tmp/gp2040ce-binary-tools-0.6.0.tar.gz` & `tmp/gp2040ce-binary-tools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp2040ce-binary-tools-0.6.0.tar", last modified: Tue Jan  9 17:02:37 2024, max compression
+gzip compressed data, was "gp2040ce-binary-tools-0.7.0.tar", last modified: Mon Apr  8 15:50:28 2024, max compression
```

## Comparing `gp2040ce-binary-tools-0.6.0.tar` & `gp2040ce-binary-tools-0.7.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-01-09 17:02:37.314597 gp2040ce-binary-tools-0.6.0/
--rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce-binary-tools-0.6.0/.gitattributes
--rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce-binary-tools-0.6.0/.gitignore
--rw-r--r--   0 bss       (1026) bss       (1000)     4294 2024-01-09 15:49:59.000000 gp2040ce-binary-tools-0.6.0/CHANGELOG.md
--rw-r--r--   0 bss       (1026) bss       (1000)     1394 2024-01-02 21:16:25.000000 gp2040ce-binary-tools-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 bss       (1026) bss       (1000)     1366 2024-01-02 21:16:25.000000 gp2040ce-binary-tools-0.6.0/DCO.txt
--rw-r--r--   0 bss       (1026) bss       (1000)     1073 2024-01-02 21:16:25.000000 gp2040ce-binary-tools-0.6.0/LICENSE
--rw-r--r--   0 bss       (1026) bss       (1000)      428 2024-01-02 21:16:25.000000 gp2040ce-binary-tools-0.6.0/MAINTAINERS.md
--rw-r--r--   0 bss       (1026) bss       (1000)     9543 2024-01-09 17:02:37.313597 gp2040ce-binary-tools-0.6.0/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     7789 2024-01-09 15:59:55.000000 gp2040ce-binary-tools-0.6.0/README.md
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-01-09 17:02:37.312597 gp2040ce-binary-tools-0.6.0/gp2040ce_binary_tools.egg-info/
--rw-r--r--   0 bss       (1026) bss       (1000)     9543 2024-01-09 17:02:37.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_binary_tools.egg-info/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     1664 2024-01-09 17:02:37.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_binary_tools.egg-info/SOURCES.txt
--rw-r--r--   0 bss       (1026) bss       (1000)        1 2024-01-09 17:02:37.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_binary_tools.egg-info/dependency_links.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      282 2024-01-09 17:02:37.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_binary_tools.egg-info/entry_points.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      289 2024-01-09 17:02:37.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_binary_tools.egg-info/requires.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       18 2024-01-09 17:02:37.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_binary_tools.egg-info/top_level.txt
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-01-09 17:02:37.295597 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/
--rw-r--r--   0 bss       (1026) bss       (1000)     2848 2024-01-09 06:46:23.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)      411 2024-01-09 17:02:37.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/_version.py
--rw-r--r--   0 bss       (1026) bss       (1000)    16336 2024-01-07 03:00:31.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)      712 2023-06-30 07:04:59.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/config_tree.css
--rw-r--r--   0 bss       (1026) bss       (1000)    19398 2024-01-04 00:27:04.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/gui.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-01-09 17:02:37.296597 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/
--rw-r--r--   0 bss       (1026) bss       (1000)      407 2024-01-09 14:29:46.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)    21293 2024-01-09 14:31:34.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)    40233 2024-01-09 14:25:54.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     7063 2024-01-09 14:31:34.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)    11078 2024-01-09 14:25:44.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-01-09 14:31:58.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-01-09 14:32:05.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9199 2024-01-08 20:26:07.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/rp2040.py
--rw-r--r--   0 bss       (1026) bss       (1000)    12500 2024-01-06 22:40:58.000000 gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     2647 2024-01-09 16:58:02.000000 gp2040ce-binary-tools-0.6.0/pyproject.toml
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-01-09 17:02:37.296597 gp2040ce-binary-tools-0.6.0/requirements/
--rw-r--r--   0 bss       (1026) bss       (1000)     4534 2024-01-09 16:58:02.000000 gp2040ce-binary-tools-0.6.0/requirements/requirements-dev.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      991 2024-01-09 16:58:02.000000 gp2040ce-binary-tools-0.6.0/requirements/requirements.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       38 2024-01-09 17:02:37.314597 gp2040ce-binary-tools-0.6.0/setup.cfg
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-01-09 17:02:37.296597 gp2040ce-binary-tools-0.6.0/tests/
--rw-r--r--   0 bss       (1026) bss       (1000)     2016 2024-01-07 02:40:50.000000 gp2040ce-binary-tools-0.6.0/tests/conftest.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-01-09 17:02:37.299597 gp2040ce-binary-tools-0.6.0/tests/test-files/
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-01-09 17:02:37.312597 gp2040ce-binary-tools-0.6.0/tests/test-files/pb2-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    40233 2024-01-03 17:46:11.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/pb2-files/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)    11078 2024-01-03 17:46:13.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/pb2-files/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-01-03 17:46:15.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/pb2-files/nanopb_pb2.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-01-09 17:02:37.312597 gp2040ce-binary-tools-0.6.0/tests/test-files/proto-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    21293 2024-01-03 17:46:02.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/proto-files/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     7063 2024-01-03 17:46:02.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/proto-files/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2023-11-07 05:46:20.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/proto-files/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     3770 2024-01-03 19:02:39.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/test-binary-source-of-json-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)     3321 2023-11-06 22:22:53.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/test-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    27799 2024-01-03 17:34:09.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/test-config.json
--rw-r--r--   0 bss       (1026) bss       (1000)   816968 2023-11-06 22:20:55.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/test-firmware.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    16384 2023-11-06 22:20:55.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/test-storage-area.bin
--rw-r--r--   0 bss       (1026) bss       (1000)  2097152 2024-01-06 22:53:09.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/test-whole-board-with-board-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-11-06 22:20:55.000000 gp2040ce-binary-tools-0.6.0/tests/test-files/test-whole-board.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    14252 2024-01-07 02:51:19.000000 gp2040ce-binary-tools-0.6.0/tests/test_builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)     3671 2024-01-03 19:34:33.000000 gp2040ce-binary-tools-0.6.0/tests/test_commands.py
--rw-r--r--   0 bss       (1026) bss       (1000)     8892 2024-01-03 18:15:42.000000 gp2040ce-binary-tools-0.6.0/tests/test_gui.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1495 2024-01-09 14:38:17.000000 gp2040ce-binary-tools-0.6.0/tests/test_package.py
--rw-r--r--   0 bss       (1026) bss       (1000)    11075 2024-01-02 21:16:25.000000 gp2040ce-binary-tools-0.6.0/tests/test_rp2040.py
--rw-r--r--   0 bss       (1026) bss       (1000)     8289 2024-01-09 14:21:09.000000 gp2040ce-binary-tools-0.6.0/tests/test_storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1628 2024-01-09 16:29:24.000000 gp2040ce-binary-tools-0.6.0/tox.ini
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.882169 gp2040ce-binary-tools-0.7.0/
+-rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce-binary-tools-0.7.0/.gitattributes
+-rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce-binary-tools-0.7.0/.gitignore
+-rw-r--r--   0 bss       (1026) bss       (1000)     4294 2024-01-09 15:49:59.000000 gp2040ce-binary-tools-0.7.0/CHANGELOG.md
+-rw-r--r--   0 bss       (1026) bss       (1000)     1392 2024-03-07 15:19:40.000000 gp2040ce-binary-tools-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 bss       (1026) bss       (1000)     1366 2024-01-02 21:16:25.000000 gp2040ce-binary-tools-0.7.0/DCO.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)    35149 2024-03-07 15:11:36.000000 gp2040ce-binary-tools-0.7.0/LICENSE
+-rw-r--r--   0 bss       (1026) bss       (1000)      428 2024-01-02 21:16:25.000000 gp2040ce-binary-tools-0.7.0/MAINTAINERS.md
+-rw-r--r--   0 bss       (1026) bss       (1000)    51143 2024-04-08 15:50:28.882169 gp2040ce-binary-tools-0.7.0/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     8815 2024-04-08 13:57:12.000000 gp2040ce-binary-tools-0.7.0/README.md
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.881168 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/
+-rw-r--r--   0 bss       (1026) bss       (1000)    51143 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     1664 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)        1 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      282 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/entry_points.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      289 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/requires.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       18 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/top_level.txt
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.868168 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2861 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)      411 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/_version.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    14971 2024-03-25 16:36:51.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)      968 2024-03-26 17:28:23.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/config_tree.css
+-rw-r--r--   0 bss       (1026) bss       (1000)    22958 2024-03-26 17:49:27.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/gui.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.869169 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/
+-rw-r--r--   0 bss       (1026) bss       (1000)      407 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 13:57:12.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 13:57:12.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 13:57:12.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 13:57:12.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 13:35:15.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 13:35:48.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9212 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/rp2040.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    14826 2024-03-25 15:03:42.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     2687 2024-03-07 15:17:10.000000 gp2040ce-binary-tools-0.7.0/pyproject.toml
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.869169 gp2040ce-binary-tools-0.7.0/requirements/
+-rw-r--r--   0 bss       (1026) bss       (1000)     4047 2024-04-08 14:07:50.000000 gp2040ce-binary-tools-0.7.0/requirements/requirements-dev.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      906 2024-04-08 14:07:50.000000 gp2040ce-binary-tools-0.7.0/requirements/requirements.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       38 2024-04-08 15:50:28.882169 gp2040ce-binary-tools-0.7.0/setup.cfg
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.869169 gp2040ce-binary-tools-0.7.0/tests/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2029 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/tests/conftest.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.871168 gp2040ce-binary-tools-0.7.0/tests/test-files/
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.881168 gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 14:01:25.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 14:01:25.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 14:00:25.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/nanopb_pb2.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.881168 gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 14:01:25.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 14:01:25.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 14:00:09.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     3770 2024-01-03 19:02:39.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-binary-source-of-json-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)     3321 2023-11-06 22:22:53.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    27879 2024-04-08 14:07:47.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-config.json
+-rw-r--r--   0 bss       (1026) bss       (1000)   816968 2023-11-06 22:20:55.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-firmware.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    16384 2023-11-06 22:20:55.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-storage-area.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)  2097152 2024-01-06 22:53:09.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-whole-board-with-board-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-11-06 22:20:55.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-whole-board.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    14262 2024-03-25 16:41:58.000000 gp2040ce-binary-tools-0.7.0/tests/test_builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     3684 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/tests/test_commands.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9870 2024-03-26 18:47:23.000000 gp2040ce-binary-tools-0.7.0/tests/test_gui.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1508 2024-04-08 13:56:04.000000 gp2040ce-binary-tools-0.7.0/tests/test_package.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11088 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/tests/test_rp2040.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9532 2024-03-25 14:19:49.000000 gp2040ce-binary-tools-0.7.0/tests/test_storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1628 2024-01-09 16:29:24.000000 gp2040ce-binary-tools-0.7.0/tox.ini
```

### Comparing `gp2040ce-binary-tools-0.6.0/.gitignore` & `gp2040ce-binary-tools-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/CHANGELOG.md` & `gp2040ce-binary-tools-0.7.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/CONTRIBUTING.md` & `gp2040ce-binary-tools-0.7.0/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Contributing Guidelines
 
-gp2040ce-binary-tools is made available under the MIT (Expat) license. Contributions are welcome via pull requests. This
+gp2040ce-binary-tools is made available under the GPLv3 (or later). Contributions are welcome via pull requests.  This
 document outlines the process to get your contribution accepted.
 
 ## Sign Offs/Custody of Contributions
 
 The Developer Certificate of Origin (DCO) is a way for contributors to certify that they wrote or otherwise have the
 right to license their code contributions to the project. The full text of the DCO can be found
 [here](https://developercertificate.org/) or in `DCO.txt`. Contributors must sign-off that they adhere to these
```

### Comparing `gp2040ce-binary-tools-0.6.0/DCO.txt` & `gp2040ce-binary-tools-0.7.0/DCO.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/PKG-INFO` & `gp2040ce-binary-tools-0.7.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,7 @@
-Metadata-Version: 2.1
-Name: gp2040ce-binary-tools
-Version: 0.6.0
-Summary: Tools for working with GP2040-CE firmware and storage binaries.
-Author-email: "Brian S. Stephan" <bss@incorporeal.org>
-License: MIT
-Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
-Project-URL: Changelog, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md
-Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: grpcio-tools
-Requires-Dist: pyusb
-Requires-Dist: textual
-Provides-Extra: dev
-Requires-Dist: bandit; extra == "dev"
-Requires-Dist: decorator; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: flake8-blind-except; extra == "dev"
-Requires-Dist: flake8-builtins; extra == "dev"
-Requires-Dist: flake8-docstrings; extra == "dev"
-Requires-Dist: flake8-executable; extra == "dev"
-Requires-Dist: flake8-fixme; extra == "dev"
-Requires-Dist: flake8-isort; extra == "dev"
-Requires-Dist: flake8-logging-format; extra == "dev"
-Requires-Dist: flake8-mutable; extra == "dev"
-Requires-Dist: flake8-pyproject; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pip-tools; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: setuptools-scm; extra == "dev"
-Requires-Dist: textual-dev; extra == "dev"
-Requires-Dist: tox; extra == "dev"
-
 # GP2040-CE Binary Tools
 
 Tools for working with GP2040-CE binary dumps.
 
 ## Dependencies
 
 While not necessary for most tools, you may want [picotool](https://github.com/raspberrypi/picotool) as an alternative
@@ -239,16 +197,23 @@
 ## Miscellaneous
 
 ### Version information
 
 The GP2040-CE configuration is still changing, so the tools are changing accordingly. This project doesn't currently make
 a huge effort to be backwards compatible, so instead, refer to this:
 
-* `gp2040ce-binary-tools >=v0.5.1` supports `GP2040-CE >=v0.7.5`.
-* `gp2040ce-binary-tools <=v0.5.0` supported `GP2040-CE <v0.7.5`.
+#### Flash Layouts
+
+* `gp2040ce-binary-tools >=v0.6.0` supports both board and user configs still being developed in `GP2040-CE`.
+* `gp2040ce-binary-tools >=v0.5.1` supported the increased user config size in `GP2040-CE >=v0.7.5`.
+* `gp2040ce-binary-tools <=v0.5.0` supported the smaller user config size in `GP2040-CE <v0.7.5`.
+
+#### Config Structures
+
+The latest update of the configuration snapshot is from **v0.7.8-RC2**.
 
 ### Dumping the GP2040-CE board with picotool
 
 Some of these tools require a dump of your GP2040-CE board, either the storage section or the whole board, depending on
 the context. The storage section of a GP2040-CE board is a reserved 16 KB starting at `0x101FC000`. To dump your board's
 storage with picotool:
 
@@ -257,7 +222,22 @@
 ```
 
 And to dump your whole board:
 
 ```
 % picotool save -a whole-board.bin
 ```
+
+## Author and Licensing
+
+Written by and copyright Brian S. Stephan (<bss@incorporeal.org>).
+
+gp2040ce-binary-tools is free software: you can redistribute it and/or modify it under the terms of the GNU General
+Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any
+later version.
+
+gp2040ce-binary-tools is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the
+implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
+details.
+
+You should have received a copy of the GNU General Public License along with gp2040ce-binary-tools. If not, see
+<https://www.gnu.org/licenses/>.
```

### Comparing `gp2040ce-binary-tools-0.6.0/gp2040ce_binary_tools.egg-info/SOURCES.txt` & `gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/__init__.py` & `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Initialize the package and get dependencies.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import argparse
 import importlib
 import logging
 import os
 import pathlib
 import sys
```

### Comparing `gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/builder.py` & `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 """Build binary files for a GP2040-CE board.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import argparse
 import copy
 import logging
-import struct
 from typing import Optional
 
 from google.protobuf.message import Message
 
 from gp2040ce_bintools import core_parser
 from gp2040ce_bintools.rp2040 import get_bootsel_endpoints, read, write
 from gp2040ce_bintools.storage import (BOARD_CONFIG_BINARY_LOCATION, STORAGE_SIZE, USER_CONFIG_BINARY_LOCATION,
-                                       USER_CONFIG_BOOTSEL_ADDRESS, get_config_from_json, pad_config_to_storage_size,
-                                       serialize_config_with_footer)
+                                       USER_CONFIG_BOOTSEL_ADDRESS, convert_binary_to_uf2, get_config_from_json,
+                                       pad_config_to_storage_size, serialize_config_with_footer)
 
 logger = logging.getLogger(__name__)
 
 GP2040CE_START_ADDRESS = 0x10000000
 GP2040CE_SIZE = 2 * 1024 * 1024
 
-UF2_FAMILY_ID = 0xE48BFF56
-UF2_MAGIC_FIRST = 0x0A324655
-UF2_MAGIC_SECOND = 0x9E5D5157
-UF2_MAGIC_FINAL = 0x0AB16F30
-
 
 #################
 # LIBRARY ITEMS #
 #################
 
 
 class FirmwareLengthError(ValueError):
@@ -111,46 +105,14 @@
             else:
                 combined.write(new_binary)
     if usb:
         endpoint_out, endpoint_in = get_bootsel_endpoints()
         write(endpoint_out, endpoint_in, GP2040CE_START_ADDRESS, bytes(new_binary))
 
 
-def convert_binary_to_uf2(binary: bytearray) -> bytearray:
-    """Convert a GP2040-CE binary payload to Microsoft's UF2 format.
-
-    https://github.com/microsoft/uf2/tree/master#overview
-
-    Args:
-        binary: bytearray content to convert to a UF2 payload
-    Returns:
-        the content in UF2 format
-    """
-    size = len(binary)
-    blocks = (len(binary) // 256) + 1 if len(binary) % 256 else len(binary) // 256
-    uf2 = bytearray()
-
-    index = 0
-    while index < size:
-        pad_count = 476 - len(binary[index:index+256])
-        uf2 += struct.pack('<LLLLLLLL',
-                           UF2_MAGIC_FIRST,                                 # first magic number
-                           UF2_MAGIC_SECOND,                                # second magic number
-                           0x00002000,                                      # familyID present
-                           0x10000000 + index,                              # address to write to
-                           256,                                             # bytes to write in this block
-                           index // 256,                                    # sequential block number
-                           blocks,                                          # total number of blocks
-                           UF2_FAMILY_ID)                                   # family ID
-        uf2 += binary[index:index+256] + bytearray(b'\x00' * pad_count)     # content
-        uf2 += struct.pack('<L', UF2_MAGIC_FINAL)                           # final magic number
-        index += 256
-    return uf2
-
-
 def get_gp2040ce_from_usb() -> tuple[bytes, object, object]:
     """Read the firmware + config sections from a USB device.
 
     Returns:
         the bytes from the board, along with the USB out and in endpoints for reference
     """
     # open the USB device and get the config
@@ -248,19 +210,24 @@
                 the whole file is replaced
     """
     if inject:
         config_binary = serialize_config_with_footer(config)
         with open(filename, 'rb') as file:
             existing_binary = file.read()
         binary = replace_config_in_binary(bytearray(existing_binary), config_binary)
+        with open(filename, 'wb') as file:
+            file.write(binary)
     else:
         binary = serialize_config_with_footer(config)
-
-    with open(filename, 'wb') as file:
-        file.write(binary)
+        with open(filename, 'wb') as file:
+            if filename[-4:] == '.uf2':
+                file.write(convert_binary_to_uf2(pad_config_to_storage_size(binary),
+                                                 start=USER_CONFIG_BINARY_LOCATION))
+            else:
+                file.write(binary)
 
 
 def write_new_config_to_usb(config: Message, endpoint_out: object, endpoint_in: object):
     """Serialize the provided config to a device over USB, in the proper location for a GP2040-CE board.
 
     Args:
         config: the Protobuf configuration to write to a RP2040 board in BOOTSEL mode
```

### Comparing `gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/gui.py` & `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/gui.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """GUI applications for working with binary files.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import argparse
 import logging
+from textwrap import dedent
 
 from google.protobuf import descriptor
 from google.protobuf.message import Message
 from rich.highlighter import ReprHighlighter
 from rich.text import Text
 from textual import on
 from textual.app import App, ComposeResult
-from textual.containers import Grid
+from textual.containers import Container, Grid, Horizontal
 from textual.logging import TextualHandler
 from textual.screen import ModalScreen
-from textual.validation import Number
-from textual.widgets import Button, Footer, Header, Input, Label, Pretty, Select, Tree
+from textual.validation import Length, Number
+from textual.widgets import Button, Footer, Header, Input, Label, Pretty, Select, TextArea, Tree
 from textual.widgets.tree import TreeNode
 
-from gp2040ce_bintools import core_parser, handler
+from gp2040ce_bintools import _version, core_parser, handler
 from gp2040ce_bintools.builder import write_new_config_to_filename, write_new_config_to_usb
 from gp2040ce_bintools.rp2040 import get_bootsel_endpoints, read
 from gp2040ce_bintools.storage import (STORAGE_SIZE, USER_CONFIG_BOOTSEL_ADDRESS, ConfigReadError, get_config,
                                        get_config_from_file, get_new_config)
 
 logger = logging.getLogger(__name__)
 
@@ -53,40 +54,41 @@
             self.input_field = Input(value=repr(self.field_value), validators=[Number()], id='field-input')
         elif self.field_descriptor.type == descriptor.FieldDescriptor.TYPE_STRING:
             self.input_field = Input(value=self.field_value, id='field-input')
         else:
             # we don't handle whatever these are yet
             self.input_field = Label(repr(self.field_value), id='field-input')
         yield Grid(
-            Label(self.field_descriptor.full_name, id="field-name"),
-            self.input_field,
-            Pretty('', id='input-errors', classes='hidden'),
-            Button("Save", id='save-button'),
-            Button("Cancel", id='cancel-button'),
+            Container(Label(self.field_descriptor.full_name, id='field-name'), id='field-name-container'),
+            Container(self.input_field, id='input-field-container'),
+            Container(Pretty('', id='input-errors', classes='hidden'), id='error-container'),
+            Horizontal(Container(Button("Cancel", id='cancel-button'), id='cancel-button-container'),
+                       Container(Button("Confirm", id='confirm-button'), id='confirm-button-container'),
+                       id='button-container'),
             id='edit-dialog',
         )
 
     @on(Input.Changed)
     def show_invalid_reasons(self, event: Input.Changed) -> None:
         """Update the UI to show why validation failed."""
         if event.validation_result:
             error_field = self.query_one(Pretty)
-            save_button = self.query_one('#save-button', Button)
+            save_button = self.query_one('#confirm-button', Button)
             if not event.validation_result.is_valid:
                 error_field.update(event.validation_result.failure_descriptions)
                 error_field.classes = ''
                 save_button.disabled = True
             else:
                 error_field.update('')
                 error_field.classes = 'hidden'
                 save_button.disabled = False
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         """Process the button actions."""
-        if event.button.id == 'save-button':
+        if event.button.id == 'confirm-button':
             logger.debug("calling _save")
             self._save()
         self.app.pop_screen()
 
     def _save(self):
         """Save the field value to the retained config item."""
         if not isinstance(self.input_field, Label):
@@ -109,34 +111,85 @@
         """Store the message for later display."""
         self.text = text
         super().__init__(*args, **kwargs)
 
     def compose(self) -> ComposeResult:
         """Build the pop-up window with the desired message displayed."""
         yield Grid(
-            Label(self.text, id="message-text"),
-            Button("OK", id='ok-button'),
+            Container(TextArea(self.text, id='message-text', read_only=True), id='text-container'),
+            Container(Button("OK", id='ok-button'), id='button-container'),
             id='message-dialog',
         )
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         """Process the button action (close the window)."""
         self.app.pop_screen()
 
 
+class SaveAsScreen(ModalScreen):
+    """Present the option of saving the configuration as a new file."""
+
+    def __init__(self, config, *args, **kwargs):
+        """Initialize a filename argument to be populated."""
+        self.config = config
+        super().__init__(*args, **kwargs)
+
+    def compose(self) -> ComposeResult:
+        """Build the pop-up window prompting for the new filename to save the configuration as."""
+        self.filename_field = Input(value=None, id='field-input', validators=[Length(minimum=1)])
+        yield Grid(
+            Container(Label("Filename (.uf2 or .bin) to write to:", id='field-name'), id='field-name-container'),
+            Container(self.filename_field, id='input-field-container'),
+            Container(Pretty('', id='input-errors', classes='hidden'), id='error-container'),
+            Horizontal(Container(Button("Cancel", id='cancel-button'), id='cancel-button-container'),
+                       Container(Button("Confirm", id='confirm-button'), id='confirm-button-container'),
+                       id='button-container'),
+            id='save-as-dialog',
+        )
+
+    @on(Input.Changed)
+    def show_invalid_reasons(self, event: Input.Changed) -> None:
+        """Update the UI to show why validation failed."""
+        if event.validation_result:
+            error_field = self.query_one(Pretty)
+            save_button = self.query_one('#confirm-button', Button)
+            if not event.validation_result.is_valid:
+                error_field.update(event.validation_result.failure_descriptions)
+                error_field.classes = ''
+                save_button.disabled = True
+            else:
+                error_field.update('')
+                error_field.classes = 'hidden'
+                save_button.disabled = False
+
+    def on_button_pressed(self, event: Button.Pressed) -> None:
+        """Process the button actions."""
+        if event.button.id == 'confirm-button':
+            logger.debug("calling _save")
+            self._save()
+        self.app.pop_screen()
+
+    def _save(self):
+        """Save the configuration to the specified file."""
+        write_new_config_to_filename(self.config, self.filename_field.value, inject=False)
+        self.notify(f"Saved to {self.filename_field.value}.", title="Configuration Saved")
+
+
 class ConfigEditor(App):
     """Display the GP2040-CE configuration as a tree."""
 
     BINDINGS = [
-        ('a', 'add_node', "Add Node"),
+        ('a', 'save_as', "Save As..."),
+        ('n', 'add_node', "Add Node"),
         ('s', 'save', "Save Config"),
         ('q', 'quit', "Quit"),
+        ('?', 'about', "About"),
     ]
     CSS_PATH = "config_tree.css"
-    TITLE = "GP2040-CE Configuration Editor"
+    TITLE = F"GP2040-CE Configuration Editor - {_version.version}"
 
     def __init__(self, *args, **kwargs):
         """Initialize config."""
         # disable normal logging and enable console logging
         logger.debug("reconfiguring logging...")
         root = logging.getLogger()
         root.setLevel(logging.DEBUG)
@@ -158,15 +211,15 @@
         else:
             self.source_name = self.config_filename
 
     def compose(self) -> ComposeResult:
         """Compose the UI."""
         yield Header()
         yield Footer()
-        yield Tree("Root")
+        yield Tree("Root", id='config_tree')
 
     def on_mount(self) -> None:
         """Load the configuration object into the tree view."""
         tree = self.query_one(Tree)
 
         tree.root.data = (None, self.config.DESCRIPTOR, self.config)
         tree.root.set_label(self.source_name)
@@ -183,14 +236,23 @@
                                    value_is_config=child_is_message)
         tree.root.expand()
 
     def on_tree_node_selected(self, node_event: Tree.NodeSelected) -> None:
         """Take the appropriate action for this type of node."""
         self._modify_node(node_event.node)
 
+    def action_about(self) -> None:
+        """Display a help/about popup."""
+        self.push_screen(MessageScreen(dedent("""
+            gp2040ce-binary-tools - Tools for working with GP2040-CE firmware and storage binaries
+
+            Copyright © 2023 Brian S. Stephan <bss@incorporeal.org>
+            Made available WITHOUT ANY WARRANTY under the GNU General Public License, version 3 or later.
+        """)))
+
     def action_add_node(self) -> None:
         """Add a node to the tree item, if allowed by the tree and config section."""
         tree = self.query_one(Tree)
         current_node = tree.cursor_node
 
         if not current_node or not current_node.allow_expand:
             logger.debug("no node selected, or it does not allow expansion")
@@ -214,20 +276,25 @@
                                    value_is_config=True)
             current_node.expand()
 
     def action_save(self) -> None:
         """Save the configuration."""
         if self.usb:
             write_new_config_to_usb(self.config, self.endpoint_out, self.endpoint_in)
-            self.push_screen(MessageScreen(f"Configuration saved to "
-                                           f"{hex(self.endpoint_out.device.idVendor)}:"
-                                           f"{hex(self.endpoint_out.device.idProduct)}."))
+            self.notify(f"Saved to {hex(self.endpoint_out.device.idVendor)}:"
+                        f"{hex(self.endpoint_out.device.idProduct)}.",
+                        title="Configuration Saved")
         elif self.config_filename:
             write_new_config_to_filename(self.config, self.config_filename, inject=self.whole_board)
-            self.push_screen(MessageScreen(f"Configuration saved to {self.config_filename}."))
+            self.notify(f"Saved to {self.config_filename}.",
+                        title="Configuration Saved")
+
+    def action_save_as(self) -> None:
+        """Present a new dialog to save the configuration as a new standalone file."""
+        self.push_screen(SaveAsScreen(self.config))
 
     def action_quit(self) -> None:
         """Quit the application."""
         self.exit()
 
     @staticmethod
     def _add_node(parent_node: TreeNode, parent_config: Message,
@@ -392,16 +459,17 @@
     )
     parser.add_argument('--whole-board', action='store_true', help="indicate the binary file is a whole board dump")
     parser.add_argument('--new-if-not-found', action='store_true', default=True,
                         help="if the file/USB device doesn't have a config section, start a new one (default: enabled)")
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument('--usb', action='store_true', help="retrieve the config from a RP2040 board connected over USB "
                                                           "and in BOOTSEL mode")
-    group.add_argument('--filename', help=".bin file of a GP2040-CE board's config + footer or entire storage section, "
-                                          "or of a GP2040-CE's whole board dump if --whole-board is specified")
+    group.add_argument('--filename', help=".bin of a GP2040-CE's whole board dump if --whole-board is specified, or a"
+                                          ".bin file of a GP2040-CE board's config + footer or entire storage section; "
+                                          "if creating a new config, it can also be written in .uf2 format")
     args, _ = parser.parse_known_args()
 
     if args.usb:
         app = ConfigEditor(usb=True, create_new=args.new_if_not_found)
     else:
         app = ConfigEditor(config_filename=args.filename, whole_board=args.whole_board,
                            create_new=args.new_if_not_found)
```

### Comparing `gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/config_pb2.py` & `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,35 +11,39 @@
 _sym_db = _symbol_database.Default()
 
 
 import nanopb_pb2 as nanopb__pb2
 import enums_pb2 as enums__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63onfig.proto\x1a\x0cnanopb.proto\x1a\x0b\x65nums.proto\"\xf6\x03\n\x0eGamepadOptions\x12\x1d\n\tinputMode\x18\x01 \x01(\x0e\x32\n.InputMode\x12\x1b\n\x08\x64padMode\x18\x02 \x01(\x0e\x32\t.DpadMode\x12\x1b\n\x08socdMode\x18\x03 \x01(\x0e\x32\t.SOCDMode\x12\x13\n\x0binvertXAxis\x18\x04 \x01(\x08\x12\x13\n\x0binvertYAxis\x18\x05 \x01(\x08\x12\x1b\n\x13switchTpShareForDs4\x18\x06 \x01(\x08\x12\x13\n\x0blockHotkeys\x18\x07 \x01(\x08\x12\x13\n\x0b\x66ourWayMode\x18\x08 \x01(\x08\x12\x15\n\rprofileNumber\x18\t \x01(\r\x12-\n\x11ps4ControllerType\x18\n \x01(\x0e\x32\x12.PS4ControllerType\x12\x15\n\rdebounceDelay\x18\x0b \x01(\r\x12\x13\n\x0binputModeB1\x18\x0c \x01(\x05\x12\x13\n\x0binputModeB2\x18\r \x01(\x05\x12\x13\n\x0binputModeB3\x18\x0e \x01(\x05\x12\x13\n\x0binputModeB4\x18\x0f \x01(\x05\x12\x13\n\x0binputModeL1\x18\x10 \x01(\x05\x12\x13\n\x0binputModeL2\x18\x11 \x01(\x05\x12\x13\n\x0binputModeR1\x18\x12 \x01(\x05\x12\x13\n\x0binputModeR2\x18\x13 \x01(\x05\x12\x15\n\rps4ReportHack\x18\x14 \x01(\x08\"\x8a\x03\n\x0fKeyboardMapping\x12\x11\n\tkeyDpadUp\x18\x01 \x01(\r\x12\x13\n\x0bkeyDpadDown\x18\x02 \x01(\r\x12\x13\n\x0bkeyDpadLeft\x18\x03 \x01(\r\x12\x14\n\x0ckeyDpadRight\x18\x04 \x01(\r\x12\x13\n\x0bkeyButtonB1\x18\x05 \x01(\r\x12\x13\n\x0bkeyButtonB2\x18\x06 \x01(\r\x12\x13\n\x0bkeyButtonB3\x18\x07 \x01(\r\x12\x13\n\x0bkeyButtonB4\x18\x08 \x01(\r\x12\x13\n\x0bkeyButtonL1\x18\t \x01(\r\x12\x13\n\x0bkeyButtonR1\x18\n \x01(\r\x12\x13\n\x0bkeyButtonL2\x18\x0b \x01(\r\x12\x13\n\x0bkeyButtonR2\x18\x0c \x01(\r\x12\x13\n\x0bkeyButtonS1\x18\r \x01(\r\x12\x13\n\x0bkeyButtonS2\x18\x0e \x01(\r\x12\x13\n\x0bkeyButtonL3\x18\x0f \x01(\r\x12\x13\n\x0bkeyButtonR3\x18\x10 \x01(\r\x12\x13\n\x0bkeyButtonA1\x18\x11 \x01(\r\x12\x13\n\x0bkeyButtonA2\x18\x12 \x01(\r\"e\n\x0bHotkeyEntry\x12\x10\n\x08\x64padMask\x18\x01 \x01(\r\x12\x1e\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x0e.GamepadHotkey\x12\x13\n\x0b\x62uttonsMask\x18\x03 \x01(\r\x12\x0f\n\x07\x61uxMask\x18\x04 \x01(\r\"\x8f\x04\n\rHotkeyOptions\x12\x1e\n\x08hotkey01\x18\x01 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey02\x18\x02 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey03\x18\x03 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey04\x18\x04 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey05\x18\x05 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey06\x18\x06 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey07\x18\x07 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey08\x18\x08 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey09\x18\t \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey10\x18\n \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey11\x18\x0b \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey12\x18\x0c \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey13\x18\r \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey14\x18\x0e \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey15\x18\x0f \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey16\x18\x10 \x01(\x0b\x32\x0c.HotkeyEntry\"\xf1\x03\n\x11PeripheralOptions\x12\x30\n\tblockI2C0\x18\x01 \x01(\x0b\x32\x1d.PeripheralOptions.I2COptions\x12\x30\n\tblockI2C1\x18\x02 \x01(\x0b\x32\x1d.PeripheralOptions.I2COptions\x12\x30\n\tblockSPI0\x18\x03 \x01(\x0b\x32\x1d.PeripheralOptions.SPIOptions\x12\x30\n\tblockSPI1\x18\x04 \x01(\x0b\x32\x1d.PeripheralOptions.SPIOptions\x12\x30\n\tblockUSB0\x18\x05 \x01(\x0b\x32\x1d.PeripheralOptions.USBOptions\x1a\x46\n\nI2COptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03sda\x18\x02 \x01(\x05\x12\x0b\n\x03scl\x18\x03 \x01(\x05\x12\r\n\x05speed\x18\x04 \x01(\r\x1aN\n\nSPIOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02rx\x18\x02 \x01(\x05\x12\n\n\x02\x63s\x18\x03 \x01(\x05\x12\x0b\n\x03sck\x18\x04 \x01(\x05\x12\n\n\x02tx\x18\x05 \x01(\x05\x1aJ\n\nUSBOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02\x64p\x18\x02 \x01(\x05\x12\x10\n\x08\x65nable5v\x18\x03 \x01(\x05\x12\r\n\x05order\x18\x04 \x01(\r\"4\n\x12\x46orcedSetupOptions\x12\x1e\n\x04mode\x18\x01 \x01(\x0e\x32\x10.ForcedSetupMode\"g\n\x18\x42uttonLayoutParamsCommon\x12\x0e\n\x06startX\x18\x01 \x01(\x05\x12\x0e\n\x06startY\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonRadius\x18\x03 \x01(\x05\x12\x15\n\rbuttonPadding\x18\x04 \x01(\x05\"b\n\x16\x42uttonLayoutParamsLeft\x12\x1d\n\x06layout\x18\x01 \x01(\x0e\x32\r.ButtonLayout\x12)\n\x06\x63ommon\x18\x02 \x01(\x0b\x32\x19.ButtonLayoutParamsCommon\"h\n\x17\x42uttonLayoutParamsRight\x12\"\n\x06layout\x18\x01 \x01(\x0e\x32\x12.ButtonLayoutRight\x12)\n\x06\x63ommon\x18\x02 \x01(\x0b\x32\x19.ButtonLayoutParamsCommon\"w\n\x19\x42uttonLayoutCustomOptions\x12+\n\nparamsLeft\x18\x01 \x01(\x0b\x32\x17.ButtonLayoutParamsLeft\x12-\n\x0bparamsRight\x18\x02 \x01(\x0b\x32\x18.ButtonLayoutParamsRight\"\x9b\x03\n\x0bPinMappings\x12\x11\n\tpinDpadUp\x18\x01 \x01(\x05\x12\x13\n\x0bpinDpadDown\x18\x02 \x01(\x05\x12\x13\n\x0bpinDpadLeft\x18\x03 \x01(\x05\x12\x14\n\x0cpinDpadRight\x18\x04 \x01(\x05\x12\x13\n\x0bpinButtonB1\x18\x05 \x01(\x05\x12\x13\n\x0bpinButtonB2\x18\x06 \x01(\x05\x12\x13\n\x0bpinButtonB3\x18\x07 \x01(\x05\x12\x13\n\x0bpinButtonB4\x18\x08 \x01(\x05\x12\x13\n\x0bpinButtonL1\x18\t \x01(\x05\x12\x13\n\x0bpinButtonR1\x18\n \x01(\x05\x12\x13\n\x0bpinButtonL2\x18\x0b \x01(\x05\x12\x13\n\x0bpinButtonR2\x18\x0c \x01(\x05\x12\x13\n\x0bpinButtonS1\x18\r \x01(\x05\x12\x13\n\x0bpinButtonS2\x18\x0e \x01(\x05\x12\x13\n\x0bpinButtonL3\x18\x0f \x01(\x05\x12\x13\n\x0bpinButtonR3\x18\x10 \x01(\x05\x12\x13\n\x0bpinButtonA1\x18\x11 \x01(\x05\x12\x13\n\x0bpinButtonA2\x18\x12 \x01(\x05\x12\x13\n\x0bpinButtonFn\x18\x13 \x01(\x05\".\n\x0fGpioMappingInfo\x12\x1b\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\x0b.GpioAction\"5\n\x0cGpioMappings\x12%\n\x04pins\x18\x01 \x03(\x0b\x32\x10.GpioMappingInfoB\x05\x92?\x02\x10\x1e\"\x93\x02\n\x16\x41lternativePinMappings\x12\x13\n\x0bpinButtonB1\x18\x01 \x01(\x05\x12\x13\n\x0bpinButtonB2\x18\x02 \x01(\x05\x12\x13\n\x0bpinButtonB3\x18\x03 \x01(\x05\x12\x13\n\x0bpinButtonB4\x18\x04 \x01(\x05\x12\x13\n\x0bpinButtonL1\x18\x05 \x01(\x05\x12\x13\n\x0bpinButtonR1\x18\x06 \x01(\x05\x12\x13\n\x0bpinButtonL2\x18\x07 \x01(\x05\x12\x13\n\x0bpinButtonR2\x18\x08 \x01(\x05\x12\x11\n\tpinDpadUp\x18\t \x01(\x05\x12\x13\n\x0bpinDpadDown\x18\n \x01(\x05\x12\x13\n\x0bpinDpadLeft\x18\x0b \x01(\x05\x12\x14\n\x0cpinDpadRight\x18\x0c \x01(\x05\"\x8c\x01\n\x0eProfileOptions\x12J\n deprecatedAlternativePinMappings\x18\x01 \x03(\x0b\x32\x17.AlternativePinMappingsB\x07\x18\x01\x92?\x02\x10\x03\x12.\n\x10gpioMappingsSets\x18\x02 \x03(\x0b\x32\r.GpioMappingsB\x05\x92?\x02\x10\x03\"\x9e\x04\n\x0e\x44isplayOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x12\n\ni2cAddress\x18\x05 \x01(\x05\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x06 \x01(\x05\x42\x02\x18\x01\x12#\n\x0c\x62uttonLayout\x18\x07 \x01(\x0e\x32\r.ButtonLayout\x12-\n\x11\x62uttonLayoutRight\x18\x08 \x01(\x0e\x32\x12.ButtonLayoutRight\x12=\n\x19\x62uttonLayoutCustomOptions\x18\t \x01(\x0b\x32\x1a.ButtonLayoutCustomOptions\x12\x1f\n\nsplashMode\x18\n \x01(\x0e\x32\x0b.SplashMode\x12#\n\x0csplashChoice\x18\x0b \x01(\x0e\x32\r.SplashChoice\x12\x16\n\x0esplashDuration\x18\x0c \x01(\x05\x12\x1b\n\x0bsplashImage\x18\r \x01(\x0c\x42\x06\x92?\x03\x08\x80\x08\x12\x0c\n\x04size\x18\x0e \x01(\x05\x12\x0c\n\x04\x66lip\x18\x0f \x01(\x05\x12\x0e\n\x06invert\x18\x10 \x01(\x08\x12\x1b\n\x13\x64isplaySaverTimeout\x18\x11 \x01(\x05\x12\x1c\n\x14turnOffWhenSuspended\x18\x12 \x01(\x08\"\xce\x05\n\nLEDOptions\x12\x0f\n\x07\x64\x61taPin\x18\x01 \x01(\x05\x12#\n\tledFormat\x18\x02 \x01(\x0e\x32\x10.LEDFormat_Proto\x12 \n\tledLayout\x18\x03 \x01(\x0e\x32\r.ButtonLayout\x12\x15\n\rledsPerButton\x18\x04 \x01(\r\x12\x19\n\x11\x62rightnessMaximum\x18\x05 \x01(\r\x12\x17\n\x0f\x62rightnessSteps\x18\x06 \x01(\r\x12\x0f\n\x07indexUp\x18\x07 \x01(\x05\x12\x11\n\tindexDown\x18\x08 \x01(\x05\x12\x11\n\tindexLeft\x18\t \x01(\x05\x12\x12\n\nindexRight\x18\n \x01(\x05\x12\x0f\n\x07indexB1\x18\x0b \x01(\x05\x12\x0f\n\x07indexB2\x18\x0c \x01(\x05\x12\x0f\n\x07indexB3\x18\r \x01(\x05\x12\x0f\n\x07indexB4\x18\x0e \x01(\x05\x12\x0f\n\x07indexL1\x18\x0f \x01(\x05\x12\x0f\n\x07indexR1\x18\x10 \x01(\x05\x12\x0f\n\x07indexL2\x18\x11 \x01(\x05\x12\x0f\n\x07indexR2\x18\x12 \x01(\x05\x12\x0f\n\x07indexS1\x18\x13 \x01(\x05\x12\x0f\n\x07indexS2\x18\x14 \x01(\x05\x12\x0f\n\x07indexL3\x18\x15 \x01(\x05\x12\x0f\n\x07indexR3\x18\x16 \x01(\x05\x12\x0f\n\x07indexA1\x18\x17 \x01(\x05\x12\x0f\n\x07indexA2\x18\x18 \x01(\x05\x12\x1b\n\x08pledType\x18\x19 \x01(\x0e\x32\t.PLEDType\x12\x10\n\x08pledPin1\x18\x1a \x01(\x05\x12\x10\n\x08pledPin2\x18\x1b \x01(\x05\x12\x10\n\x08pledPin3\x18\x1c \x01(\x05\x12\x10\n\x08pledPin4\x18\x1d \x01(\x05\x12\x11\n\tpledColor\x18\x1e \x01(\r\x12\x1c\n\x14turnOffWhenSuspended\x18\x1f \x01(\x08\x12\x12\n\npledIndex1\x18  \x01(\x05\x12\x12\n\npledIndex2\x18! \x01(\x05\x12\x12\n\npledIndex3\x18\" \x01(\x05\x12\x12\n\npledIndex4\x18# \x01(\x05\"\xa2\t\n\x16\x41nimationOptions_Proto\x12\x1a\n\x12\x62\x61seAnimationIndex\x18\x01 \x01(\r\x12\x12\n\nbrightness\x18\x02 \x01(\r\x12\x18\n\x10staticColorIndex\x18\x03 \x01(\r\x12\x18\n\x10\x62uttonColorIndex\x18\x04 \x01(\r\x12\x16\n\x0e\x63haseCycleTime\x18\x05 \x01(\x05\x12\x18\n\x10rainbowCycleTime\x18\x06 \x01(\x05\x12\x12\n\nthemeIndex\x18\x07 \x01(\r\x12\x16\n\x0ehasCustomTheme\x18\x08 \x01(\x08\x12\x15\n\rcustomThemeUp\x18\t \x01(\r\x12\x17\n\x0f\x63ustomThemeDown\x18\n \x01(\r\x12\x17\n\x0f\x63ustomThemeLeft\x18\x0b \x01(\r\x12\x18\n\x10\x63ustomThemeRight\x18\x0c \x01(\r\x12\x15\n\rcustomThemeB1\x18\r \x01(\r\x12\x15\n\rcustomThemeB2\x18\x0e \x01(\r\x12\x15\n\rcustomThemeB3\x18\x0f \x01(\r\x12\x15\n\rcustomThemeB4\x18\x10 \x01(\r\x12\x15\n\rcustomThemeL1\x18\x11 \x01(\r\x12\x15\n\rcustomThemeR1\x18\x12 \x01(\r\x12\x15\n\rcustomThemeL2\x18\x13 \x01(\r\x12\x15\n\rcustomThemeR2\x18\x14 \x01(\r\x12\x15\n\rcustomThemeS1\x18\x15 \x01(\r\x12\x15\n\rcustomThemeS2\x18\x16 \x01(\r\x12\x15\n\rcustomThemeL3\x18\x17 \x01(\r\x12\x15\n\rcustomThemeR3\x18\x18 \x01(\r\x12\x15\n\rcustomThemeA1\x18\x19 \x01(\r\x12\x15\n\rcustomThemeA2\x18\x1a \x01(\r\x12\x1c\n\x14\x63ustomThemeUpPressed\x18\x1b \x01(\r\x12\x1e\n\x16\x63ustomThemeDownPressed\x18\x1c \x01(\r\x12\x1e\n\x16\x63ustomThemeLeftPressed\x18\x1d \x01(\r\x12\x1f\n\x17\x63ustomThemeRightPressed\x18\x1e \x01(\r\x12\x1c\n\x14\x63ustomThemeB1Pressed\x18\x1f \x01(\r\x12\x1c\n\x14\x63ustomThemeB2Pressed\x18  \x01(\r\x12\x1c\n\x14\x63ustomThemeB3Pressed\x18! \x01(\r\x12\x1c\n\x14\x63ustomThemeB4Pressed\x18\" \x01(\r\x12\x1c\n\x14\x63ustomThemeL1Pressed\x18# \x01(\r\x12\x1c\n\x14\x63ustomThemeR1Pressed\x18$ \x01(\r\x12\x1c\n\x14\x63ustomThemeL2Pressed\x18% \x01(\r\x12\x1c\n\x14\x63ustomThemeR2Pressed\x18& \x01(\r\x12\x1c\n\x14\x63ustomThemeS1Pressed\x18\' \x01(\r\x12\x1c\n\x14\x63ustomThemeS2Pressed\x18( \x01(\r\x12\x1c\n\x14\x63ustomThemeL3Pressed\x18) \x01(\r\x12\x1c\n\x14\x63ustomThemeR3Pressed\x18* \x01(\r\x12\x1c\n\x14\x63ustomThemeA1Pressed\x18+ \x01(\r\x12\x1c\n\x14\x63ustomThemeA2Pressed\x18, \x01(\r\":\n\x14\x42ootselButtonOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbuttonMap\x18\x02 \x01(\r\"C\n\x11OnBoardLedOptions\x12\x1d\n\x04mode\x18\x01 \x01(\x0e\x32\x0f.OnBoardLedMode\x12\x0f\n\x07\x65nabled\x18\x02 \x01(\x08\"\xe1\x02\n\rAnalogOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0e\x61nalogAdc1PinX\x18\x02 \x01(\x05\x12\x16\n\x0e\x61nalogAdc1PinY\x18\x03 \x01(\x05\x12\x1a\n\x12\x66orced_circularity\x18\x04 \x01(\x08\x12\x17\n\x0f\x61nalog_deadzone\x18\x05 \x01(\r\x12\x16\n\x0e\x61nalogAdc2PinX\x18\x06 \x01(\x05\x12\x16\n\x0e\x61nalogAdc2PinY\x18\x07 \x01(\x05\x12!\n\x0e\x61nalogAdc1Mode\x18\x08 \x01(\x0e\x32\t.DpadMode\x12!\n\x0e\x61nalogAdc2Mode\x18\t \x01(\x0e\x32\t.DpadMode\x12%\n\x10\x61nalogAdc1Invert\x18\n \x01(\x0e\x32\x0b.InvertMode\x12%\n\x10\x61nalogAdc2Invert\x18\x0b \x01(\x0e\x32\x0b.InvertMode\x12\x16\n\x0e\x61uto_calibrate\x18\x0c \x01(\x08\"\xbe\x03\n\x0cTurboOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbuttonPin\x18\x02 \x01(\x05\x12\x0e\n\x06ledPin\x18\x03 \x01(\x05\x12\x11\n\tshotCount\x18\x04 \x01(\r\x12\x14\n\x0cshmupDialPin\x18\x05 \x01(\x05\x12\x18\n\x10shmupModeEnabled\x18\x06 \x01(\x08\x12\x16\n\x0eshmupAlwaysOn1\x18\x07 \x01(\r\x12\x16\n\x0eshmupAlwaysOn2\x18\x08 \x01(\r\x12\x16\n\x0eshmupAlwaysOn3\x18\t \x01(\r\x12\x16\n\x0eshmupAlwaysOn4\x18\n \x01(\r\x12\x14\n\x0cshmupBtn1Pin\x18\x0b \x01(\x05\x12\x14\n\x0cshmupBtn2Pin\x18\x0c \x01(\x05\x12\x14\n\x0cshmupBtn3Pin\x18\r \x01(\x05\x12\x14\n\x0cshmupBtn4Pin\x18\x0e \x01(\x05\x12\x15\n\rshmupBtnMask1\x18\x0f \x01(\r\x12\x15\n\rshmupBtnMask2\x18\x10 \x01(\r\x12\x15\n\rshmupBtnMask3\x18\x11 \x01(\r\x12\x15\n\rshmupBtnMask4\x18\x12 \x01(\r\x12#\n\x0cshmupMixMode\x18\x13 \x01(\x0e\x32\r.ShmupMixMode\"\xdc\x01\n\rSliderOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x16\x64\x65precatedPinSliderOne\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\"\n\x16\x64\x65precatedPinSliderTwo\x18\x03 \x01(\x05\x42\x02\x18\x01\x12(\n\x11\x64\x65precatedModeOne\x18\x04 \x01(\x0e\x32\t.DpadModeB\x02\x18\x01\x12(\n\x11\x64\x65precatedModeTwo\x18\x05 \x01(\x0e\x32\t.DpadModeB\x02\x18\x01\x12\x1e\n\x0bmodeDefault\x18\x06 \x01(\x0e\x32\t.DpadMode\"\xd4\x01\n\x11SOCDSliderOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1c\n\x10\x64\x65precatedPinOne\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1c\n\x10\x64\x65precatedPinTwo\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x0bmodeDefault\x18\x04 \x01(\x0e\x32\t.SOCDMode\x12(\n\x11\x64\x65precatedModeOne\x18\x05 \x01(\x0e\x32\t.SOCDModeB\x02\x18\x01\x12(\n\x11\x64\x65precatedModeTwo\x18\x06 \x01(\x0e\x32\t.SOCDModeB\x02\x18\x01\"\x93\x01\n\x0eReverseOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbuttonPin\x18\x02 \x01(\x05\x12\x0e\n\x06ledPin\x18\x03 \x01(\x05\x12\x10\n\x08\x61\x63tionUp\x18\x04 \x01(\r\x12\x12\n\nactionDown\x18\x05 \x01(\r\x12\x12\n\nactionLeft\x18\x06 \x01(\r\x12\x13\n\x0b\x61\x63tionRight\x18\x07 \x01(\r\"\xaf\x01\n\x14\x41nalogADS1219Options\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x12\n\ni2cAddress\x18\x05 \x01(\x05\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x06 \x01(\x05\x42\x02\x18\x01\"\xeb\x01\n\x16\x44ualDirectionalOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1b\n\x0f\x64\x65precatedUpPin\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1d\n\x11\x64\x65precatedDownPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1d\n\x11\x64\x65precatedLeftPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x12\x64\x65precatedRightPin\x18\x05 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x08\x64padMode\x18\x06 \x01(\x0e\x32\t.DpadMode\x12\x13\n\x0b\x63ombineMode\x18\x07 \x01(\r\x12\x13\n\x0b\x66ourWayMode\x18\x08 \x01(\x08\"\xd8\x04\n\x0bTiltOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08tilt1Pin\x18\x02 \x01(\x05\x12\x10\n\x08tilt2Pin\x18\x03 \x01(\x05\x12%\n\x19\x64\x65precatedTiltFunctionPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13tiltLeftAnalogUpPin\x18\x05 \x01(\x05\x12\x1d\n\x15tiltLeftAnalogDownPin\x18\x06 \x01(\x05\x12\x1d\n\x15tiltLeftAnalogLeftPin\x18\x07 \x01(\x05\x12\x1e\n\x16tiltLeftAnalogRightPin\x18\x08 \x01(\x05\x12\x1c\n\x14tiltRightAnalogUpPin\x18\t \x01(\x05\x12\x1e\n\x16tiltRightAnalogDownPin\x18\n \x01(\x05\x12\x1e\n\x16tiltRightAnalogLeftPin\x18\x0b \x01(\x05\x12\x1f\n\x17tiltRightAnalogRightPin\x18\x0c \x01(\x05\x12\x1f\n\x0ctiltSOCDMode\x18\r \x01(\x0e\x32\t.SOCDMode\x12\x18\n\x10\x66\x61\x63torTilt1LeftX\x18\x0e \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt1LeftY\x18\x0f \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt1RightX\x18\x10 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt1RightY\x18\x11 \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt2LeftX\x18\x12 \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt2LeftY\x18\x13 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt2RightX\x18\x14 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt2RightY\x18\x15 \x01(\x05\"=\n\rBuzzerOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x0e\n\x06volume\x18\x03 \x01(\r\"E\n\x12\x45xtraButtonOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x11\n\tbuttonMap\x18\x03 \x01(\r\"6\n\x13PlayerNumberOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06number\x18\x02 \x01(\r\"\x98\x02\n\nPS4Options\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\x06serial\x18\x02 \x01(\x0c\x42\x05\x92?\x02\x08\x10\x12\x19\n\tsignature\x18\x03 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x14\n\x04rsaN\x18\x04 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x13\n\x04rsaE\x18\x05 \x01(\x0c\x42\x05\x92?\x02\x08\x04\x12\x14\n\x04rsaD\x18\x06 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x14\n\x04rsaP\x18\x07 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x14\n\x04rsaQ\x18\x08 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaDP\x18\t \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaDQ\x18\n \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaQP\x18\x0b \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaRN\x18\x0c \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\"d\n\x14PSPassthroughOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\x12\x64\x65precatedPinDplus\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x0f\x64\x65precatedPin5V\x18\x03 \x01(\x05\x42\x02\x18\x01\"*\n\x17XBOnePassthroughOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\"\xf5\x11\n\nWiiOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x05 \x01(\x05\x42\x02\x18\x01\x12\x32\n\x0b\x63ontrollers\x18\x06 \x01(\x0b\x32\x1d.WiiOptions.ControllerOptions\x1a\x42\n\nAnalogAxis\x12\x10\n\x08\x61xisType\x18\x01 \x01(\x05\x12\x10\n\x08minRange\x18\x02 \x01(\x05\x12\x10\n\x08maxRange\x18\x03 \x01(\x05\x1aT\n\x0cStickOptions\x12!\n\x01x\x18\x01 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12!\n\x01y\x18\x02 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a[\n\x0eNunchukOptions\x12\x0f\n\x07\x62uttonC\x18\x01 \x01(\x05\x12\x0f\n\x07\x62uttonZ\x18\x02 \x01(\x05\x12\'\n\x05stick\x18\x03 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x1a\xdc\x03\n\x0e\x43lassicOptions\x12\x0f\n\x07\x62uttonA\x18\x01 \x01(\x05\x12\x0f\n\x07\x62uttonB\x18\x02 \x01(\x05\x12\x0f\n\x07\x62uttonX\x18\x03 \x01(\x05\x12\x0f\n\x07\x62uttonY\x18\x04 \x01(\x05\x12\x0f\n\x07\x62uttonL\x18\x05 \x01(\x05\x12\x10\n\x08\x62uttonZL\x18\x06 \x01(\x05\x12\x0f\n\x07\x62uttonR\x18\x07 \x01(\x05\x12\x10\n\x08\x62uttonZR\x18\x08 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\t \x01(\x05\x12\x12\n\nbuttonPlus\x18\n \x01(\x05\x12\x12\n\nbuttonHome\x18\x0b \x01(\x05\x12\x10\n\x08\x62uttonUp\x18\x0c \x01(\x05\x12\x12\n\nbuttonDown\x18\r \x01(\x05\x12\x12\n\nbuttonLeft\x18\x0e \x01(\x05\x12\x13\n\x0b\x62uttonRight\x18\x0f \x01(\x05\x12,\n\nrightStick\x18\x11 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12+\n\tleftStick\x18\x10 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12+\n\x0bleftTrigger\x18\x12 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12,\n\x0crightTrigger\x18\x13 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1al\n\x0cTaikoOptions\x12\x15\n\rbuttonKatLeft\x18\x01 \x01(\x05\x12\x16\n\x0e\x62uttonKatRight\x18\x02 \x01(\x05\x12\x15\n\rbuttonDonLeft\x18\x03 \x01(\x05\x12\x16\n\x0e\x62uttonDonRight\x18\x04 \x01(\x05\x1a\xad\x02\n\rGuitarOptions\x12\x11\n\tbuttonRed\x18\x01 \x01(\x05\x12\x13\n\x0b\x62uttonGreen\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonYellow\x18\x03 \x01(\x05\x12\x12\n\nbuttonBlue\x18\x04 \x01(\x05\x12\x14\n\x0c\x62uttonOrange\x18\x05 \x01(\x05\x12\x13\n\x0b\x62uttonPedal\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\x0f\n\x07strumUp\x18\t \x01(\x05\x12\x11\n\tstrumDown\x18\n \x01(\x05\x12\'\n\x05stick\x18\x0b \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12)\n\twhammyBar\x18\x0c \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a\xdc\x01\n\x0b\x44rumOptions\x12\x11\n\tbuttonRed\x18\x01 \x01(\x05\x12\x13\n\x0b\x62uttonGreen\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonYellow\x18\x03 \x01(\x05\x12\x12\n\nbuttonBlue\x18\x04 \x01(\x05\x12\x14\n\x0c\x62uttonOrange\x18\x05 \x01(\x05\x12\x13\n\x0b\x62uttonPedal\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\'\n\x05stick\x18\t \x01(\x0b\x32\x18.WiiOptions.StickOptions\x1a\xbe\x03\n\x10TurntableOptions\x12\x15\n\rbuttonLeftRed\x18\x01 \x01(\x05\x12\x17\n\x0f\x62uttonLeftGreen\x18\x02 \x01(\x05\x12\x16\n\x0e\x62uttonLeftBlue\x18\x03 \x01(\x05\x12\x16\n\x0e\x62uttonRightRed\x18\x04 \x01(\x05\x12\x18\n\x10\x62uttonRightGreen\x18\x05 \x01(\x05\x12\x17\n\x0f\x62uttonRightBlue\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\x16\n\x0e\x62uttonEuphoria\x18\t \x01(\x05\x12\'\n\x05stick\x18\n \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12-\n\rleftTurntable\x18\x0b \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12.\n\x0erightTurntable\x18\x0c \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12\'\n\x07\x65\x66\x66\x65\x63ts\x18\r \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12%\n\x05\x66\x61\x64\x65r\x18\x0e \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a\x99\x02\n\x11\x43ontrollerOptions\x12+\n\x07nunchuk\x18\x01 \x01(\x0b\x32\x1a.WiiOptions.NunchukOptions\x12+\n\x07\x63lassic\x18\x02 \x01(\x0b\x32\x1a.WiiOptions.ClassicOptions\x12\'\n\x05taiko\x18\x03 \x01(\x0b\x32\x18.WiiOptions.TaikoOptions\x12)\n\x06guitar\x18\x04 \x01(\x0b\x32\x19.WiiOptions.GuitarOptions\x12%\n\x04\x64rum\x18\x05 \x01(\x0b\x32\x17.WiiOptions.DrumOptions\x12/\n\tturntable\x18\x06 \x01(\x0b\x32\x1c.WiiOptions.TurntableOptions\"S\n\x0bSNESOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08\x63lockPin\x18\x02 \x01(\x05\x12\x10\n\x08latchPin\x18\x03 \x01(\x05\x12\x0f\n\x07\x64\x61taPin\x18\x04 \x01(\x05\"\x86\x01\n\x13KeyboardHostOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\x12\x64\x65precatedPinDplus\x18\x02 \x01(\x05\x42\x02\x18\x01\x12!\n\x07mapping\x18\x03 \x01(\x0b\x32\x10.KeyboardMapping\x12\x1b\n\x0f\x64\x65precatedPin5V\x18\x04 \x01(\x05\x42\x02\x18\x01\"\xae\x01\n\x10\x46ocusModeOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x16\n\x0e\x62uttonLockMask\x18\x03 \x01(\x05\x12\x17\n\x0foledLockEnabled\x18\x04 \x01(\x08\x12\x16\n\x0ergbLockEnabled\x18\x05 \x01(\x08\x12\x19\n\x11\x62uttonLockEnabled\x18\x06 \x01(\x08\x12\x18\n\x10macroLockEnabled\x18\x07 \x01(\x08\"K\n\nMacroInput\x12\x12\n\nbuttonMask\x18\x01 \x01(\r\x12\x10\n\x08\x64uration\x18\x02 \x01(\r\x12\x17\n\x0cwaitDuration\x18\x03 \x01(\r:\x01\x30\"\xa4\x02\n\x05Macro\x12\x1d\n\tmacroType\x18\x01 \x01(\x0e\x32\n.MacroType\x12\x19\n\nmacroLabel\x18\x02 \x01(\tB\x05\x92?\x02p@\x12\'\n\x0bmacroInputs\x18\x03 \x03(\x0b\x32\x0b.MacroInputB\x05\x92?\x02\x10\x1e\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\x12\x1d\n\x15useMacroTriggerButton\x18\x05 \x01(\x08\x12\x1b\n\x0fmacroTriggerPin\x18\x06 \x01(\x05:\x02-1\x12\x1a\n\x12macroTriggerButton\x18\x07 \x01(\r\x12\x17\n\texclusive\x18\x08 \x01(\x08:\x04true\x12\x1b\n\rinterruptible\x18\t \x01(\x08:\x04true\x12\x19\n\nshowFrames\x18\n \x01(\x08:\x05\x66\x61lse\"l\n\x0cMacroOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x1c\n\x14macroBoardLedEnabled\x18\x04 \x01(\x08\x12 \n\tmacroList\x18\x03 \x03(\x0b\x32\x06.MacroB\x05\x92?\x02\x10\x06\"P\n\x13InputHistoryOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06length\x18\x02 \x01(\r\x12\x0b\n\x03\x63ol\x18\x03 \x01(\r\x12\x0b\n\x03row\x18\x04 \x01(\r\"\xfc\x07\n\x0c\x41\x64\x64onOptions\x12\x33\n\x14\x62ootselButtonOptions\x18\x01 \x01(\x0b\x32\x15.BootselButtonOptions\x12-\n\x11onBoardLedOptions\x18\x02 \x01(\x0b\x32\x12.OnBoardLedOptions\x12%\n\ranalogOptions\x18\x03 \x01(\x0b\x32\x0e.AnalogOptions\x12#\n\x0cturboOptions\x18\x04 \x01(\x0b\x32\r.TurboOptions\x12%\n\rsliderOptions\x18\x05 \x01(\x0b\x32\x0e.SliderOptions\x12\'\n\x0ereverseOptions\x18\x06 \x01(\x0b\x32\x0f.ReverseOptions\x12\x33\n\x14\x61nalogADS1219Options\x18\x07 \x01(\x0b\x32\x15.AnalogADS1219Options\x12\x37\n\x16\x64ualDirectionalOptions\x18\x08 \x01(\x0b\x32\x17.DualDirectionalOptions\x12%\n\rbuzzerOptions\x18\t \x01(\x0b\x32\x0e.BuzzerOptions\x12=\n\x1c\x64\x65precatedExtraButtonOptions\x18\n \x01(\x0b\x32\x13.ExtraButtonOptionsB\x02\x18\x01\x12\x31\n\x13playerNumberOptions\x18\x0b \x01(\x0b\x32\x14.PlayerNumberOptions\x12\'\n\nps4Options\x18\x0c \x01(\x0b\x32\x0b.PS4OptionsB\x06\x92?\x03\xf0\x01\x01\x12\x1f\n\nwiiOptions\x18\r \x01(\x0b\x32\x0b.WiiOptions\x12-\n\x11socdSliderOptions\x18\x0e \x01(\x0b\x32\x12.SOCDSliderOptions\x12!\n\x0bsnesOptions\x18\x0f \x01(\x0b\x32\x0c.SNESOptions\x12+\n\x10\x66ocusModeOptions\x18\x10 \x01(\x0b\x32\x11.FocusModeOptions\x12\x31\n\x13keyboardHostOptions\x18\x11 \x01(\x0b\x32\x14.KeyboardHostOptions\x12!\n\x0btiltOptions\x18\x12 \x01(\x0b\x32\x0c.TiltOptions\x12\x33\n\x14psPassthroughOptions\x18\x13 \x01(\x0b\x32\x15.PSPassthroughOptions\x12#\n\x0cmacroOptions\x18\x14 \x01(\x0b\x32\r.MacroOptions\x12\x31\n\x13inputHistoryOptions\x18\x15 \x01(\x0b\x32\x14.InputHistoryOptions\x12\x39\n\x17xbonePassthroughOptions\x18\x16 \x01(\x0b\x32\x18.XBOnePassthroughOptions\"~\n\x10MigrationHistory\x12\x1e\n\x0fhotkeysMigrated\x18\x01 \x01(\x08:\x05\x66\x61lse\x12#\n\x14gpioMappingsMigrated\x18\x02 \x01(\x08:\x05\x66\x61lse\x12%\n\x16\x62uttonProfilesMigrated\x18\x03 \x01(\x08:\x05\x66\x61lse\"\xe4\x04\n\x06\x43onfig\x12\x1b\n\x0c\x62oardVersion\x18\x01 \x01(\tB\x05\x92?\x02p\x1f\x12\'\n\x0egamepadOptions\x18\x02 \x01(\x0b\x32\x0f.GamepadOptions\x12%\n\rhotkeyOptions\x18\x03 \x01(\x0b\x32\x0e.HotkeyOptions\x12/\n\x15\x64\x65precatedPinMappings\x18\x04 \x01(\x0b\x32\x0c.PinMappingsB\x02\x18\x01\x12)\n\x0fkeyboardMapping\x18\x05 \x01(\x0b\x32\x10.KeyboardMapping\x12\'\n\x0e\x64isplayOptions\x18\x06 \x01(\x0b\x32\x0f.DisplayOptions\x12\x1f\n\nledOptions\x18\x07 \x01(\x0b\x32\x0b.LEDOptions\x12\x31\n\x10\x61nimationOptions\x18\x08 \x01(\x0b\x32\x17.AnimationOptions_Proto\x12#\n\x0c\x61\x64\x64onOptions\x18\t \x01(\x0b\x32\r.AddonOptions\x12/\n\x12\x66orcedSetupOptions\x18\n \x01(\x0b\x32\x13.ForcedSetupOptions\x12\'\n\x0eprofileOptions\x18\x0b \x01(\x0b\x32\x0f.ProfileOptions\x12\x1a\n\x0b\x62oardConfig\x18\x0c \x01(\tB\x05\x92?\x02p?\x12#\n\x0cgpioMappings\x18\r \x01(\x0b\x32\r.GpioMappings\x12%\n\nmigrations\x18\x0e \x01(\x0b\x32\x11.MigrationHistory\x12-\n\x11peripheralOptions\x18\x0f \x01(\x0b\x32\x12.PeripheralOptions')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63onfig.proto\x1a\x0cnanopb.proto\x1a\x0b\x65nums.proto\"\xf8\x04\n\x0eGamepadOptions\x12\x1d\n\tinputMode\x18\x01 \x01(\x0e\x32\n.InputMode\x12\x1b\n\x08\x64padMode\x18\x02 \x01(\x0e\x32\t.DpadMode\x12\x1b\n\x08socdMode\x18\x03 \x01(\x0e\x32\t.SOCDMode\x12\x13\n\x0binvertXAxis\x18\x04 \x01(\x08\x12\x13\n\x0binvertYAxis\x18\x05 \x01(\x08\x12\x1b\n\x13switchTpShareForDs4\x18\x06 \x01(\x08\x12\x13\n\x0blockHotkeys\x18\x07 \x01(\x08\x12\x13\n\x0b\x66ourWayMode\x18\x08 \x01(\x08\x12\x15\n\rprofileNumber\x18\t \x01(\r\x12-\n\x11ps4ControllerType\x18\n \x01(\x0e\x32\x12.PS4ControllerType\x12\x15\n\rdebounceDelay\x18\x0b \x01(\r\x12\x13\n\x0binputModeB1\x18\x0c \x01(\x05\x12\x13\n\x0binputModeB2\x18\r \x01(\x05\x12\x13\n\x0binputModeB3\x18\x0e \x01(\x05\x12\x13\n\x0binputModeB4\x18\x0f \x01(\x05\x12\x13\n\x0binputModeL1\x18\x10 \x01(\x05\x12\x13\n\x0binputModeL2\x18\x11 \x01(\x05\x12\x13\n\x0binputModeR1\x18\x12 \x01(\x05\x12\x13\n\x0binputModeR2\x18\x13 \x01(\x05\x12\x19\n\rps4ReportHack\x18\x14 \x01(\x08\x42\x02\x18\x01\x12\'\n\x0bps4AuthType\x18\x15 \x01(\x0e\x32\x12.InputModeAuthType\x12\'\n\x0bps5AuthType\x18\x16 \x01(\x0e\x32\x12.InputModeAuthType\x12*\n\x0exinputAuthType\x18\x17 \x01(\x0e\x32\x12.InputModeAuthType\"\x8a\x03\n\x0fKeyboardMapping\x12\x11\n\tkeyDpadUp\x18\x01 \x01(\r\x12\x13\n\x0bkeyDpadDown\x18\x02 \x01(\r\x12\x13\n\x0bkeyDpadLeft\x18\x03 \x01(\r\x12\x14\n\x0ckeyDpadRight\x18\x04 \x01(\r\x12\x13\n\x0bkeyButtonB1\x18\x05 \x01(\r\x12\x13\n\x0bkeyButtonB2\x18\x06 \x01(\r\x12\x13\n\x0bkeyButtonB3\x18\x07 \x01(\r\x12\x13\n\x0bkeyButtonB4\x18\x08 \x01(\r\x12\x13\n\x0bkeyButtonL1\x18\t \x01(\r\x12\x13\n\x0bkeyButtonR1\x18\n \x01(\r\x12\x13\n\x0bkeyButtonL2\x18\x0b \x01(\r\x12\x13\n\x0bkeyButtonR2\x18\x0c \x01(\r\x12\x13\n\x0bkeyButtonS1\x18\r \x01(\r\x12\x13\n\x0bkeyButtonS2\x18\x0e \x01(\r\x12\x13\n\x0bkeyButtonL3\x18\x0f \x01(\r\x12\x13\n\x0bkeyButtonR3\x18\x10 \x01(\r\x12\x13\n\x0bkeyButtonA1\x18\x11 \x01(\r\x12\x13\n\x0bkeyButtonA2\x18\x12 \x01(\r\"e\n\x0bHotkeyEntry\x12\x10\n\x08\x64padMask\x18\x01 \x01(\r\x12\x1e\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x0e.GamepadHotkey\x12\x13\n\x0b\x62uttonsMask\x18\x03 \x01(\r\x12\x0f\n\x07\x61uxMask\x18\x04 \x01(\r\"\x8f\x04\n\rHotkeyOptions\x12\x1e\n\x08hotkey01\x18\x01 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey02\x18\x02 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey03\x18\x03 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey04\x18\x04 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey05\x18\x05 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey06\x18\x06 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey07\x18\x07 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey08\x18\x08 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey09\x18\t \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey10\x18\n \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey11\x18\x0b \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey12\x18\x0c \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey13\x18\r \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey14\x18\x0e \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey15\x18\x0f \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey16\x18\x10 \x01(\x0b\x32\x0c.HotkeyEntry\"\xf1\x03\n\x11PeripheralOptions\x12\x30\n\tblockI2C0\x18\x01 \x01(\x0b\x32\x1d.PeripheralOptions.I2COptions\x12\x30\n\tblockI2C1\x18\x02 \x01(\x0b\x32\x1d.PeripheralOptions.I2COptions\x12\x30\n\tblockSPI0\x18\x03 \x01(\x0b\x32\x1d.PeripheralOptions.SPIOptions\x12\x30\n\tblockSPI1\x18\x04 \x01(\x0b\x32\x1d.PeripheralOptions.SPIOptions\x12\x30\n\tblockUSB0\x18\x05 \x01(\x0b\x32\x1d.PeripheralOptions.USBOptions\x1a\x46\n\nI2COptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03sda\x18\x02 \x01(\x05\x12\x0b\n\x03scl\x18\x03 \x01(\x05\x12\r\n\x05speed\x18\x04 \x01(\r\x1aN\n\nSPIOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02rx\x18\x02 \x01(\x05\x12\n\n\x02\x63s\x18\x03 \x01(\x05\x12\x0b\n\x03sck\x18\x04 \x01(\x05\x12\n\n\x02tx\x18\x05 \x01(\x05\x1aJ\n\nUSBOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02\x64p\x18\x02 \x01(\x05\x12\x10\n\x08\x65nable5v\x18\x03 \x01(\x05\x12\r\n\x05order\x18\x04 \x01(\r\"4\n\x12\x46orcedSetupOptions\x12\x1e\n\x04mode\x18\x01 \x01(\x0e\x32\x10.ForcedSetupMode\"g\n\x18\x42uttonLayoutParamsCommon\x12\x0e\n\x06startX\x18\x01 \x01(\x05\x12\x0e\n\x06startY\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonRadius\x18\x03 \x01(\x05\x12\x15\n\rbuttonPadding\x18\x04 \x01(\x05\"b\n\x16\x42uttonLayoutParamsLeft\x12\x1d\n\x06layout\x18\x01 \x01(\x0e\x32\r.ButtonLayout\x12)\n\x06\x63ommon\x18\x02 \x01(\x0b\x32\x19.ButtonLayoutParamsCommon\"h\n\x17\x42uttonLayoutParamsRight\x12\"\n\x06layout\x18\x01 \x01(\x0e\x32\x12.ButtonLayoutRight\x12)\n\x06\x63ommon\x18\x02 \x01(\x0b\x32\x19.ButtonLayoutParamsCommon\"w\n\x19\x42uttonLayoutCustomOptions\x12+\n\nparamsLeft\x18\x01 \x01(\x0b\x32\x17.ButtonLayoutParamsLeft\x12-\n\x0bparamsRight\x18\x02 \x01(\x0b\x32\x18.ButtonLayoutParamsRight\"\x9b\x03\n\x0bPinMappings\x12\x11\n\tpinDpadUp\x18\x01 \x01(\x05\x12\x13\n\x0bpinDpadDown\x18\x02 \x01(\x05\x12\x13\n\x0bpinDpadLeft\x18\x03 \x01(\x05\x12\x14\n\x0cpinDpadRight\x18\x04 \x01(\x05\x12\x13\n\x0bpinButtonB1\x18\x05 \x01(\x05\x12\x13\n\x0bpinButtonB2\x18\x06 \x01(\x05\x12\x13\n\x0bpinButtonB3\x18\x07 \x01(\x05\x12\x13\n\x0bpinButtonB4\x18\x08 \x01(\x05\x12\x13\n\x0bpinButtonL1\x18\t \x01(\x05\x12\x13\n\x0bpinButtonR1\x18\n \x01(\x05\x12\x13\n\x0bpinButtonL2\x18\x0b \x01(\x05\x12\x13\n\x0bpinButtonR2\x18\x0c \x01(\x05\x12\x13\n\x0bpinButtonS1\x18\r \x01(\x05\x12\x13\n\x0bpinButtonS2\x18\x0e \x01(\x05\x12\x13\n\x0bpinButtonL3\x18\x0f \x01(\x05\x12\x13\n\x0bpinButtonR3\x18\x10 \x01(\x05\x12\x13\n\x0bpinButtonA1\x18\x11 \x01(\x05\x12\x13\n\x0bpinButtonA2\x18\x12 \x01(\x05\x12\x13\n\x0bpinButtonFn\x18\x13 \x01(\x05\".\n\x0fGpioMappingInfo\x12\x1b\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\x0b.GpioAction\"5\n\x0cGpioMappings\x12%\n\x04pins\x18\x01 \x03(\x0b\x32\x10.GpioMappingInfoB\x05\x92?\x02\x10\x1e\"\x93\x02\n\x16\x41lternativePinMappings\x12\x13\n\x0bpinButtonB1\x18\x01 \x01(\x05\x12\x13\n\x0bpinButtonB2\x18\x02 \x01(\x05\x12\x13\n\x0bpinButtonB3\x18\x03 \x01(\x05\x12\x13\n\x0bpinButtonB4\x18\x04 \x01(\x05\x12\x13\n\x0bpinButtonL1\x18\x05 \x01(\x05\x12\x13\n\x0bpinButtonR1\x18\x06 \x01(\x05\x12\x13\n\x0bpinButtonL2\x18\x07 \x01(\x05\x12\x13\n\x0bpinButtonR2\x18\x08 \x01(\x05\x12\x11\n\tpinDpadUp\x18\t \x01(\x05\x12\x13\n\x0bpinDpadDown\x18\n \x01(\x05\x12\x13\n\x0bpinDpadLeft\x18\x0b \x01(\x05\x12\x14\n\x0cpinDpadRight\x18\x0c \x01(\x05\"\x8c\x01\n\x0eProfileOptions\x12J\n deprecatedAlternativePinMappings\x18\x01 \x03(\x0b\x32\x17.AlternativePinMappingsB\x07\x18\x01\x92?\x02\x10\x03\x12.\n\x10gpioMappingsSets\x18\x02 \x03(\x0b\x32\r.GpioMappingsB\x05\x92?\x02\x10\x03\"\x9e\x04\n\x0e\x44isplayOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x12\n\ni2cAddress\x18\x05 \x01(\x05\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x06 \x01(\x05\x42\x02\x18\x01\x12#\n\x0c\x62uttonLayout\x18\x07 \x01(\x0e\x32\r.ButtonLayout\x12-\n\x11\x62uttonLayoutRight\x18\x08 \x01(\x0e\x32\x12.ButtonLayoutRight\x12=\n\x19\x62uttonLayoutCustomOptions\x18\t \x01(\x0b\x32\x1a.ButtonLayoutCustomOptions\x12\x1f\n\nsplashMode\x18\n \x01(\x0e\x32\x0b.SplashMode\x12#\n\x0csplashChoice\x18\x0b \x01(\x0e\x32\r.SplashChoice\x12\x16\n\x0esplashDuration\x18\x0c \x01(\x05\x12\x1b\n\x0bsplashImage\x18\r \x01(\x0c\x42\x06\x92?\x03\x08\x80\x08\x12\x0c\n\x04size\x18\x0e \x01(\x05\x12\x0c\n\x04\x66lip\x18\x0f \x01(\x05\x12\x0e\n\x06invert\x18\x10 \x01(\x08\x12\x1b\n\x13\x64isplaySaverTimeout\x18\x11 \x01(\x05\x12\x1c\n\x14turnOffWhenSuspended\x18\x12 \x01(\x08\"\xce\x05\n\nLEDOptions\x12\x0f\n\x07\x64\x61taPin\x18\x01 \x01(\x05\x12#\n\tledFormat\x18\x02 \x01(\x0e\x32\x10.LEDFormat_Proto\x12 \n\tledLayout\x18\x03 \x01(\x0e\x32\r.ButtonLayout\x12\x15\n\rledsPerButton\x18\x04 \x01(\r\x12\x19\n\x11\x62rightnessMaximum\x18\x05 \x01(\r\x12\x17\n\x0f\x62rightnessSteps\x18\x06 \x01(\r\x12\x0f\n\x07indexUp\x18\x07 \x01(\x05\x12\x11\n\tindexDown\x18\x08 \x01(\x05\x12\x11\n\tindexLeft\x18\t \x01(\x05\x12\x12\n\nindexRight\x18\n \x01(\x05\x12\x0f\n\x07indexB1\x18\x0b \x01(\x05\x12\x0f\n\x07indexB2\x18\x0c \x01(\x05\x12\x0f\n\x07indexB3\x18\r \x01(\x05\x12\x0f\n\x07indexB4\x18\x0e \x01(\x05\x12\x0f\n\x07indexL1\x18\x0f \x01(\x05\x12\x0f\n\x07indexR1\x18\x10 \x01(\x05\x12\x0f\n\x07indexL2\x18\x11 \x01(\x05\x12\x0f\n\x07indexR2\x18\x12 \x01(\x05\x12\x0f\n\x07indexS1\x18\x13 \x01(\x05\x12\x0f\n\x07indexS2\x18\x14 \x01(\x05\x12\x0f\n\x07indexL3\x18\x15 \x01(\x05\x12\x0f\n\x07indexR3\x18\x16 \x01(\x05\x12\x0f\n\x07indexA1\x18\x17 \x01(\x05\x12\x0f\n\x07indexA2\x18\x18 \x01(\x05\x12\x1b\n\x08pledType\x18\x19 \x01(\x0e\x32\t.PLEDType\x12\x10\n\x08pledPin1\x18\x1a \x01(\x05\x12\x10\n\x08pledPin2\x18\x1b \x01(\x05\x12\x10\n\x08pledPin3\x18\x1c \x01(\x05\x12\x10\n\x08pledPin4\x18\x1d \x01(\x05\x12\x11\n\tpledColor\x18\x1e \x01(\r\x12\x1c\n\x14turnOffWhenSuspended\x18\x1f \x01(\x08\x12\x12\n\npledIndex1\x18  \x01(\x05\x12\x12\n\npledIndex2\x18! \x01(\x05\x12\x12\n\npledIndex3\x18\" \x01(\x05\x12\x12\n\npledIndex4\x18# \x01(\x05\"\xcc\t\n\x16\x41nimationOptions_Proto\x12\x1a\n\x12\x62\x61seAnimationIndex\x18\x01 \x01(\r\x12\x12\n\nbrightness\x18\x02 \x01(\r\x12\x18\n\x10staticColorIndex\x18\x03 \x01(\r\x12\x18\n\x10\x62uttonColorIndex\x18\x04 \x01(\r\x12\x16\n\x0e\x63haseCycleTime\x18\x05 \x01(\x05\x12\x18\n\x10rainbowCycleTime\x18\x06 \x01(\x05\x12\x12\n\nthemeIndex\x18\x07 \x01(\r\x12\x16\n\x0ehasCustomTheme\x18\x08 \x01(\x08\x12\x15\n\rcustomThemeUp\x18\t \x01(\r\x12\x17\n\x0f\x63ustomThemeDown\x18\n \x01(\r\x12\x17\n\x0f\x63ustomThemeLeft\x18\x0b \x01(\r\x12\x18\n\x10\x63ustomThemeRight\x18\x0c \x01(\r\x12\x15\n\rcustomThemeB1\x18\r \x01(\r\x12\x15\n\rcustomThemeB2\x18\x0e \x01(\r\x12\x15\n\rcustomThemeB3\x18\x0f \x01(\r\x12\x15\n\rcustomThemeB4\x18\x10 \x01(\r\x12\x15\n\rcustomThemeL1\x18\x11 \x01(\r\x12\x15\n\rcustomThemeR1\x18\x12 \x01(\r\x12\x15\n\rcustomThemeL2\x18\x13 \x01(\r\x12\x15\n\rcustomThemeR2\x18\x14 \x01(\r\x12\x15\n\rcustomThemeS1\x18\x15 \x01(\r\x12\x15\n\rcustomThemeS2\x18\x16 \x01(\r\x12\x15\n\rcustomThemeL3\x18\x17 \x01(\r\x12\x15\n\rcustomThemeR3\x18\x18 \x01(\r\x12\x15\n\rcustomThemeA1\x18\x19 \x01(\r\x12\x15\n\rcustomThemeA2\x18\x1a \x01(\r\x12\x1c\n\x14\x63ustomThemeUpPressed\x18\x1b \x01(\r\x12\x1e\n\x16\x63ustomThemeDownPressed\x18\x1c \x01(\r\x12\x1e\n\x16\x63ustomThemeLeftPressed\x18\x1d \x01(\r\x12\x1f\n\x17\x63ustomThemeRightPressed\x18\x1e \x01(\r\x12\x1c\n\x14\x63ustomThemeB1Pressed\x18\x1f \x01(\r\x12\x1c\n\x14\x63ustomThemeB2Pressed\x18  \x01(\r\x12\x1c\n\x14\x63ustomThemeB3Pressed\x18! \x01(\r\x12\x1c\n\x14\x63ustomThemeB4Pressed\x18\" \x01(\r\x12\x1c\n\x14\x63ustomThemeL1Pressed\x18# \x01(\r\x12\x1c\n\x14\x63ustomThemeR1Pressed\x18$ \x01(\r\x12\x1c\n\x14\x63ustomThemeL2Pressed\x18% \x01(\r\x12\x1c\n\x14\x63ustomThemeR2Pressed\x18& \x01(\r\x12\x1c\n\x14\x63ustomThemeS1Pressed\x18\' \x01(\r\x12\x1c\n\x14\x63ustomThemeS2Pressed\x18( \x01(\r\x12\x1c\n\x14\x63ustomThemeL3Pressed\x18) \x01(\r\x12\x1c\n\x14\x63ustomThemeR3Pressed\x18* \x01(\r\x12\x1c\n\x14\x63ustomThemeA1Pressed\x18+ \x01(\r\x12\x1c\n\x14\x63ustomThemeA2Pressed\x18, \x01(\r\x12(\n buttonPressColorCooldownTimeInMs\x18- \x01(\r\":\n\x14\x42ootselButtonOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbuttonMap\x18\x02 \x01(\r\"C\n\x11OnBoardLedOptions\x12\x1d\n\x04mode\x18\x01 \x01(\x0e\x32\x0f.OnBoardLedMode\x12\x0f\n\x07\x65nabled\x18\x02 \x01(\x08\"\xe1\x02\n\rAnalogOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0e\x61nalogAdc1PinX\x18\x02 \x01(\x05\x12\x16\n\x0e\x61nalogAdc1PinY\x18\x03 \x01(\x05\x12\x1a\n\x12\x66orced_circularity\x18\x04 \x01(\x08\x12\x17\n\x0f\x61nalog_deadzone\x18\x05 \x01(\r\x12\x16\n\x0e\x61nalogAdc2PinX\x18\x06 \x01(\x05\x12\x16\n\x0e\x61nalogAdc2PinY\x18\x07 \x01(\x05\x12!\n\x0e\x61nalogAdc1Mode\x18\x08 \x01(\x0e\x32\t.DpadMode\x12!\n\x0e\x61nalogAdc2Mode\x18\t \x01(\x0e\x32\t.DpadMode\x12%\n\x10\x61nalogAdc1Invert\x18\n \x01(\x0e\x32\x0b.InvertMode\x12%\n\x10\x61nalogAdc2Invert\x18\x0b \x01(\x0e\x32\x0b.InvertMode\x12\x16\n\x0e\x61uto_calibrate\x18\x0c \x01(\x08\"\xcc\x03\n\x0cTurboOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1f\n\x13\x64\x65precatedButtonPin\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x0e\n\x06ledPin\x18\x03 \x01(\x05\x12\x11\n\tshotCount\x18\x04 \x01(\r\x12\x14\n\x0cshmupDialPin\x18\x05 \x01(\x05\x12\x18\n\x10shmupModeEnabled\x18\x06 \x01(\x08\x12\x16\n\x0eshmupAlwaysOn1\x18\x07 \x01(\r\x12\x16\n\x0eshmupAlwaysOn2\x18\x08 \x01(\r\x12\x16\n\x0eshmupAlwaysOn3\x18\t \x01(\r\x12\x16\n\x0eshmupAlwaysOn4\x18\n \x01(\r\x12\x14\n\x0cshmupBtn1Pin\x18\x0b \x01(\x05\x12\x14\n\x0cshmupBtn2Pin\x18\x0c \x01(\x05\x12\x14\n\x0cshmupBtn3Pin\x18\r \x01(\x05\x12\x14\n\x0cshmupBtn4Pin\x18\x0e \x01(\x05\x12\x15\n\rshmupBtnMask1\x18\x0f \x01(\r\x12\x15\n\rshmupBtnMask2\x18\x10 \x01(\r\x12\x15\n\rshmupBtnMask3\x18\x11 \x01(\r\x12\x15\n\rshmupBtnMask4\x18\x12 \x01(\r\x12#\n\x0cshmupMixMode\x18\x13 \x01(\x0e\x32\r.ShmupMixMode\"\xdc\x01\n\rSliderOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x16\x64\x65precatedPinSliderOne\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\"\n\x16\x64\x65precatedPinSliderTwo\x18\x03 \x01(\x05\x42\x02\x18\x01\x12(\n\x11\x64\x65precatedModeOne\x18\x04 \x01(\x0e\x32\t.DpadModeB\x02\x18\x01\x12(\n\x11\x64\x65precatedModeTwo\x18\x05 \x01(\x0e\x32\t.DpadModeB\x02\x18\x01\x12\x1e\n\x0bmodeDefault\x18\x06 \x01(\x0e\x32\t.DpadMode\"\xd4\x01\n\x11SOCDSliderOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1c\n\x10\x64\x65precatedPinOne\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1c\n\x10\x64\x65precatedPinTwo\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x0bmodeDefault\x18\x04 \x01(\x0e\x32\t.SOCDMode\x12(\n\x11\x64\x65precatedModeOne\x18\x05 \x01(\x0e\x32\t.SOCDModeB\x02\x18\x01\x12(\n\x11\x64\x65precatedModeTwo\x18\x06 \x01(\x0e\x32\t.SOCDModeB\x02\x18\x01\"\x93\x01\n\x0eReverseOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbuttonPin\x18\x02 \x01(\x05\x12\x0e\n\x06ledPin\x18\x03 \x01(\x05\x12\x10\n\x08\x61\x63tionUp\x18\x04 \x01(\r\x12\x12\n\nactionDown\x18\x05 \x01(\r\x12\x12\n\nactionLeft\x18\x06 \x01(\r\x12\x13\n\x0b\x61\x63tionRight\x18\x07 \x01(\r\"\xaf\x01\n\x14\x41nalogADS1219Options\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x12\n\ni2cAddress\x18\x05 \x01(\x05\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x06 \x01(\x05\x42\x02\x18\x01\"\x7f\n\x14\x41nalogADS1256Options\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08spiBlock\x18\x02 \x01(\x05\x12\r\n\x05\x63sPin\x18\x03 \x01(\x05\x12\x0f\n\x07\x64rdyPin\x18\x04 \x01(\x05\x12\x0c\n\x04\x61vdd\x18\x05 \x01(\x02\x12\x16\n\x0e\x65nableTriggers\x18\x06 \x01(\x08\"\x8c\x02\n\x16\x44ualDirectionalOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1b\n\x0f\x64\x65precatedUpPin\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1d\n\x11\x64\x65precatedDownPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1d\n\x11\x64\x65precatedLeftPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x12\x64\x65precatedRightPin\x18\x05 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x08\x64padMode\x18\x06 \x01(\x0e\x32\t.DpadMode\x12\x34\n\x0b\x63ombineMode\x18\x07 \x01(\x0e\x32\x1f.DualDirectionalCombinationMode\x12\x13\n\x0b\x66ourWayMode\x18\x08 \x01(\x08\"\xd8\x04\n\x0bTiltOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08tilt1Pin\x18\x02 \x01(\x05\x12\x10\n\x08tilt2Pin\x18\x03 \x01(\x05\x12%\n\x19\x64\x65precatedTiltFunctionPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13tiltLeftAnalogUpPin\x18\x05 \x01(\x05\x12\x1d\n\x15tiltLeftAnalogDownPin\x18\x06 \x01(\x05\x12\x1d\n\x15tiltLeftAnalogLeftPin\x18\x07 \x01(\x05\x12\x1e\n\x16tiltLeftAnalogRightPin\x18\x08 \x01(\x05\x12\x1c\n\x14tiltRightAnalogUpPin\x18\t \x01(\x05\x12\x1e\n\x16tiltRightAnalogDownPin\x18\n \x01(\x05\x12\x1e\n\x16tiltRightAnalogLeftPin\x18\x0b \x01(\x05\x12\x1f\n\x17tiltRightAnalogRightPin\x18\x0c \x01(\x05\x12\x1f\n\x0ctiltSOCDMode\x18\r \x01(\x0e\x32\t.SOCDMode\x12\x18\n\x10\x66\x61\x63torTilt1LeftX\x18\x0e \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt1LeftY\x18\x0f \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt1RightX\x18\x10 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt1RightY\x18\x11 \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt2LeftX\x18\x12 \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt2LeftY\x18\x13 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt2RightX\x18\x14 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt2RightY\x18\x15 \x01(\x05\"P\n\rBuzzerOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x0e\n\x06volume\x18\x03 \x01(\r\x12\x11\n\tenablePin\x18\x04 \x01(\x05\"E\n\x12\x45xtraButtonOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x11\n\tbuttonMap\x18\x03 \x01(\r\"6\n\x13PlayerNumberOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06number\x18\x02 \x01(\r\"\x98\x02\n\nPS4Options\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\x06serial\x18\x02 \x01(\x0c\x42\x05\x92?\x02\x08\x10\x12\x19\n\tsignature\x18\x03 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x14\n\x04rsaN\x18\x04 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x13\n\x04rsaE\x18\x05 \x01(\x0c\x42\x05\x92?\x02\x08\x04\x12\x14\n\x04rsaD\x18\x06 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x14\n\x04rsaP\x18\x07 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x14\n\x04rsaQ\x18\x08 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaDP\x18\t \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaDQ\x18\n \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaQP\x18\x0b \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaRN\x18\x0c \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\"h\n\x14PSPassthroughOptions\x12\x13\n\x07\x65nabled\x18\x01 \x01(\x08\x42\x02\x18\x01\x12\x1e\n\x12\x64\x65precatedPinDplus\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x0f\x64\x65precatedPin5V\x18\x03 \x01(\x05\x42\x02\x18\x01\".\n\x17XBOnePassthroughOptions\x12\x13\n\x07\x65nabled\x18\x01 \x01(\x08\x42\x02\x18\x01\"\xf5\x11\n\nWiiOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x05 \x01(\x05\x42\x02\x18\x01\x12\x32\n\x0b\x63ontrollers\x18\x06 \x01(\x0b\x32\x1d.WiiOptions.ControllerOptions\x1a\x42\n\nAnalogAxis\x12\x10\n\x08\x61xisType\x18\x01 \x01(\x05\x12\x10\n\x08minRange\x18\x02 \x01(\x05\x12\x10\n\x08maxRange\x18\x03 \x01(\x05\x1aT\n\x0cStickOptions\x12!\n\x01x\x18\x01 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12!\n\x01y\x18\x02 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a[\n\x0eNunchukOptions\x12\x0f\n\x07\x62uttonC\x18\x01 \x01(\x05\x12\x0f\n\x07\x62uttonZ\x18\x02 \x01(\x05\x12\'\n\x05stick\x18\x03 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x1a\xdc\x03\n\x0e\x43lassicOptions\x12\x0f\n\x07\x62uttonA\x18\x01 \x01(\x05\x12\x0f\n\x07\x62uttonB\x18\x02 \x01(\x05\x12\x0f\n\x07\x62uttonX\x18\x03 \x01(\x05\x12\x0f\n\x07\x62uttonY\x18\x04 \x01(\x05\x12\x0f\n\x07\x62uttonL\x18\x05 \x01(\x05\x12\x10\n\x08\x62uttonZL\x18\x06 \x01(\x05\x12\x0f\n\x07\x62uttonR\x18\x07 \x01(\x05\x12\x10\n\x08\x62uttonZR\x18\x08 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\t \x01(\x05\x12\x12\n\nbuttonPlus\x18\n \x01(\x05\x12\x12\n\nbuttonHome\x18\x0b \x01(\x05\x12\x10\n\x08\x62uttonUp\x18\x0c \x01(\x05\x12\x12\n\nbuttonDown\x18\r \x01(\x05\x12\x12\n\nbuttonLeft\x18\x0e \x01(\x05\x12\x13\n\x0b\x62uttonRight\x18\x0f \x01(\x05\x12,\n\nrightStick\x18\x11 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12+\n\tleftStick\x18\x10 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12+\n\x0bleftTrigger\x18\x12 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12,\n\x0crightTrigger\x18\x13 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1al\n\x0cTaikoOptions\x12\x15\n\rbuttonKatLeft\x18\x01 \x01(\x05\x12\x16\n\x0e\x62uttonKatRight\x18\x02 \x01(\x05\x12\x15\n\rbuttonDonLeft\x18\x03 \x01(\x05\x12\x16\n\x0e\x62uttonDonRight\x18\x04 \x01(\x05\x1a\xad\x02\n\rGuitarOptions\x12\x11\n\tbuttonRed\x18\x01 \x01(\x05\x12\x13\n\x0b\x62uttonGreen\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonYellow\x18\x03 \x01(\x05\x12\x12\n\nbuttonBlue\x18\x04 \x01(\x05\x12\x14\n\x0c\x62uttonOrange\x18\x05 \x01(\x05\x12\x13\n\x0b\x62uttonPedal\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\x0f\n\x07strumUp\x18\t \x01(\x05\x12\x11\n\tstrumDown\x18\n \x01(\x05\x12\'\n\x05stick\x18\x0b \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12)\n\twhammyBar\x18\x0c \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a\xdc\x01\n\x0b\x44rumOptions\x12\x11\n\tbuttonRed\x18\x01 \x01(\x05\x12\x13\n\x0b\x62uttonGreen\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonYellow\x18\x03 \x01(\x05\x12\x12\n\nbuttonBlue\x18\x04 \x01(\x05\x12\x14\n\x0c\x62uttonOrange\x18\x05 \x01(\x05\x12\x13\n\x0b\x62uttonPedal\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\'\n\x05stick\x18\t \x01(\x0b\x32\x18.WiiOptions.StickOptions\x1a\xbe\x03\n\x10TurntableOptions\x12\x15\n\rbuttonLeftRed\x18\x01 \x01(\x05\x12\x17\n\x0f\x62uttonLeftGreen\x18\x02 \x01(\x05\x12\x16\n\x0e\x62uttonLeftBlue\x18\x03 \x01(\x05\x12\x16\n\x0e\x62uttonRightRed\x18\x04 \x01(\x05\x12\x18\n\x10\x62uttonRightGreen\x18\x05 \x01(\x05\x12\x17\n\x0f\x62uttonRightBlue\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\x16\n\x0e\x62uttonEuphoria\x18\t \x01(\x05\x12\'\n\x05stick\x18\n \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12-\n\rleftTurntable\x18\x0b \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12.\n\x0erightTurntable\x18\x0c \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12\'\n\x07\x65\x66\x66\x65\x63ts\x18\r \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12%\n\x05\x66\x61\x64\x65r\x18\x0e \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a\x99\x02\n\x11\x43ontrollerOptions\x12+\n\x07nunchuk\x18\x01 \x01(\x0b\x32\x1a.WiiOptions.NunchukOptions\x12+\n\x07\x63lassic\x18\x02 \x01(\x0b\x32\x1a.WiiOptions.ClassicOptions\x12\'\n\x05taiko\x18\x03 \x01(\x0b\x32\x18.WiiOptions.TaikoOptions\x12)\n\x06guitar\x18\x04 \x01(\x0b\x32\x19.WiiOptions.GuitarOptions\x12%\n\x04\x64rum\x18\x05 \x01(\x0b\x32\x17.WiiOptions.DrumOptions\x12/\n\tturntable\x18\x06 \x01(\x0b\x32\x1c.WiiOptions.TurntableOptions\"S\n\x0bSNESOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08\x63lockPin\x18\x02 \x01(\x05\x12\x10\n\x08latchPin\x18\x03 \x01(\x05\x12\x0f\n\x07\x64\x61taPin\x18\x04 \x01(\x05\"\x86\x01\n\x13KeyboardHostOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\x12\x64\x65precatedPinDplus\x18\x02 \x01(\x05\x42\x02\x18\x01\x12!\n\x07mapping\x18\x03 \x01(\x0b\x32\x10.KeyboardMapping\x12\x1b\n\x0f\x64\x65precatedPin5V\x18\x04 \x01(\x05\x42\x02\x18\x01\"\xae\x01\n\x10\x46ocusModeOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x16\n\x0e\x62uttonLockMask\x18\x03 \x01(\x05\x12\x17\n\x0foledLockEnabled\x18\x04 \x01(\x08\x12\x16\n\x0ergbLockEnabled\x18\x05 \x01(\x08\x12\x19\n\x11\x62uttonLockEnabled\x18\x06 \x01(\x08\x12\x18\n\x10macroLockEnabled\x18\x07 \x01(\x08\"K\n\nMacroInput\x12\x12\n\nbuttonMask\x18\x01 \x01(\r\x12\x10\n\x08\x64uration\x18\x02 \x01(\r\x12\x17\n\x0cwaitDuration\x18\x03 \x01(\r:\x01\x30\"\xae\x02\n\x05Macro\x12\x1d\n\tmacroType\x18\x01 \x01(\x0e\x32\n.MacroType\x12\x19\n\nmacroLabel\x18\x02 \x01(\tB\x05\x92?\x02p@\x12\'\n\x0bmacroInputs\x18\x03 \x03(\x0b\x32\x0b.MacroInputB\x05\x92?\x02\x10\x1e\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\x12\x1d\n\x15useMacroTriggerButton\x18\x05 \x01(\x08\x12%\n\x19\x64\x65precatedMacroTriggerPin\x18\x06 \x01(\x05\x42\x02\x18\x01\x12\x1a\n\x12macroTriggerButton\x18\x07 \x01(\r\x12\x17\n\texclusive\x18\x08 \x01(\x08:\x04true\x12\x1b\n\rinterruptible\x18\t \x01(\x08:\x04true\x12\x19\n\nshowFrames\x18\n \x01(\x08:\x05\x66\x61lse\"z\n\x0cMacroOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x19\n\rdeprecatedPin\x18\x02 \x01(\x05\x42\x02\x18\x01\x12 \n\tmacroList\x18\x03 \x03(\x0b\x32\x06.MacroB\x05\x92?\x02\x10\x06\x12\x1c\n\x14macroBoardLedEnabled\x18\x04 \x01(\x08\"P\n\x13InputHistoryOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06length\x18\x02 \x01(\r\x12\x0b\n\x03\x63ol\x18\x03 \x01(\r\x12\x0b\n\x03row\x18\x04 \x01(\r\"\xc2\x01\n\x10RotaryPinOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04pinA\x18\x02 \x01(\x05\x12\x0c\n\x04pinB\x18\x03 \x01(\x05\x12#\n\x04mode\x18\x04 \x01(\x0e\x32\x15.RotaryEncoderPinMode\x12\x1b\n\x13pulsesPerRevolution\x18\x05 \x01(\r\x12\x12\n\nresetAfter\x18\x06 \x01(\r\x12\x17\n\x0f\x61llowWrapAround\x18\x07 \x01(\x08\x12\x12\n\nmultiplier\x18\x08 \x01(\x02\"n\n\rRotaryOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12%\n\nencoderOne\x18\x02 \x01(\x0b\x32\x11.RotaryPinOptions\x12%\n\nencoderTwo\x18\x03 \x01(\x0b\x32\x11.RotaryPinOptions\"\xe0\x08\n\x0c\x41\x64\x64onOptions\x12\x33\n\x14\x62ootselButtonOptions\x18\x01 \x01(\x0b\x32\x15.BootselButtonOptions\x12-\n\x11onBoardLedOptions\x18\x02 \x01(\x0b\x32\x12.OnBoardLedOptions\x12%\n\ranalogOptions\x18\x03 \x01(\x0b\x32\x0e.AnalogOptions\x12#\n\x0cturboOptions\x18\x04 \x01(\x0b\x32\r.TurboOptions\x12%\n\rsliderOptions\x18\x05 \x01(\x0b\x32\x0e.SliderOptions\x12\'\n\x0ereverseOptions\x18\x06 \x01(\x0b\x32\x0f.ReverseOptions\x12\x33\n\x14\x61nalogADS1219Options\x18\x07 \x01(\x0b\x32\x15.AnalogADS1219Options\x12\x37\n\x16\x64ualDirectionalOptions\x18\x08 \x01(\x0b\x32\x17.DualDirectionalOptions\x12%\n\rbuzzerOptions\x18\t \x01(\x0b\x32\x0e.BuzzerOptions\x12=\n\x1c\x64\x65precatedExtraButtonOptions\x18\n \x01(\x0b\x32\x13.ExtraButtonOptionsB\x02\x18\x01\x12\x31\n\x13playerNumberOptions\x18\x0b \x01(\x0b\x32\x14.PlayerNumberOptions\x12\'\n\nps4Options\x18\x0c \x01(\x0b\x32\x0b.PS4OptionsB\x06\x92?\x03\xf0\x01\x01\x12\x1f\n\nwiiOptions\x18\r \x01(\x0b\x32\x0b.WiiOptions\x12-\n\x11socdSliderOptions\x18\x0e \x01(\x0b\x32\x12.SOCDSliderOptions\x12!\n\x0bsnesOptions\x18\x0f \x01(\x0b\x32\x0c.SNESOptions\x12+\n\x10\x66ocusModeOptions\x18\x10 \x01(\x0b\x32\x11.FocusModeOptions\x12\x31\n\x13keyboardHostOptions\x18\x11 \x01(\x0b\x32\x14.KeyboardHostOptions\x12!\n\x0btiltOptions\x18\x12 \x01(\x0b\x32\x0c.TiltOptions\x12\x37\n\x14psPassthroughOptions\x18\x13 \x01(\x0b\x32\x15.PSPassthroughOptionsB\x02\x18\x01\x12#\n\x0cmacroOptions\x18\x14 \x01(\x0b\x32\r.MacroOptions\x12\x31\n\x13inputHistoryOptions\x18\x15 \x01(\x0b\x32\x14.InputHistoryOptions\x12=\n\x17xbonePassthroughOptions\x18\x16 \x01(\x0b\x32\x18.XBOnePassthroughOptionsB\x02\x18\x01\x12\x33\n\x14\x61nalogADS1256Options\x18\x17 \x01(\x0b\x32\x15.AnalogADS1256Options\x12%\n\rrotaryOptions\x18\x18 \x01(\x0b\x32\x0e.RotaryOptions\"~\n\x10MigrationHistory\x12\x1e\n\x0fhotkeysMigrated\x18\x01 \x01(\x08:\x05\x66\x61lse\x12#\n\x14gpioMappingsMigrated\x18\x02 \x01(\x08:\x05\x66\x61lse\x12%\n\x16\x62uttonProfilesMigrated\x18\x03 \x01(\x08:\x05\x66\x61lse\"\xe4\x04\n\x06\x43onfig\x12\x1b\n\x0c\x62oardVersion\x18\x01 \x01(\tB\x05\x92?\x02p\x1f\x12\'\n\x0egamepadOptions\x18\x02 \x01(\x0b\x32\x0f.GamepadOptions\x12%\n\rhotkeyOptions\x18\x03 \x01(\x0b\x32\x0e.HotkeyOptions\x12/\n\x15\x64\x65precatedPinMappings\x18\x04 \x01(\x0b\x32\x0c.PinMappingsB\x02\x18\x01\x12)\n\x0fkeyboardMapping\x18\x05 \x01(\x0b\x32\x10.KeyboardMapping\x12\'\n\x0e\x64isplayOptions\x18\x06 \x01(\x0b\x32\x0f.DisplayOptions\x12\x1f\n\nledOptions\x18\x07 \x01(\x0b\x32\x0b.LEDOptions\x12\x31\n\x10\x61nimationOptions\x18\x08 \x01(\x0b\x32\x17.AnimationOptions_Proto\x12#\n\x0c\x61\x64\x64onOptions\x18\t \x01(\x0b\x32\r.AddonOptions\x12/\n\x12\x66orcedSetupOptions\x18\n \x01(\x0b\x32\x13.ForcedSetupOptions\x12\'\n\x0eprofileOptions\x18\x0b \x01(\x0b\x32\x0f.ProfileOptions\x12\x1a\n\x0b\x62oardConfig\x18\x0c \x01(\tB\x05\x92?\x02p?\x12#\n\x0cgpioMappings\x18\r \x01(\x0b\x32\r.GpioMappings\x12%\n\nmigrations\x18\x0e \x01(\x0b\x32\x11.MigrationHistory\x12-\n\x11peripheralOptions\x18\x0f \x01(\x0b\x32\x12.PeripheralOptions')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
+  _GAMEPADOPTIONS.fields_by_name['ps4ReportHack']._options = None
+  _GAMEPADOPTIONS.fields_by_name['ps4ReportHack']._serialized_options = b'\030\001'
   _GPIOMAPPINGS.fields_by_name['pins']._options = None
   _GPIOMAPPINGS.fields_by_name['pins']._serialized_options = b'\222?\002\020\036'
   _PROFILEOPTIONS.fields_by_name['deprecatedAlternativePinMappings']._options = None
   _PROFILEOPTIONS.fields_by_name['deprecatedAlternativePinMappings']._serialized_options = b'\030\001\222?\002\020\003'
   _PROFILEOPTIONS.fields_by_name['gpioMappingsSets']._options = None
   _PROFILEOPTIONS.fields_by_name['gpioMappingsSets']._serialized_options = b'\222?\002\020\003'
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSDAPin']._options = None
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSDAPin']._serialized_options = b'\030\001'
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSCLPin']._options = None
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSCLPin']._serialized_options = b'\030\001'
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSpeed']._options = None
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSpeed']._serialized_options = b'\030\001'
   _DISPLAYOPTIONS.fields_by_name['splashImage']._options = None
   _DISPLAYOPTIONS.fields_by_name['splashImage']._serialized_options = b'\222?\003\010\200\010'
+  _TURBOOPTIONS.fields_by_name['deprecatedButtonPin']._options = None
+  _TURBOOPTIONS.fields_by_name['deprecatedButtonPin']._serialized_options = b'\030\001'
   _SLIDEROPTIONS.fields_by_name['deprecatedPinSliderOne']._options = None
   _SLIDEROPTIONS.fields_by_name['deprecatedPinSliderOne']._serialized_options = b'\030\001'
   _SLIDEROPTIONS.fields_by_name['deprecatedPinSliderTwo']._options = None
   _SLIDEROPTIONS.fields_by_name['deprecatedPinSliderTwo']._serialized_options = b'\030\001'
   _SLIDEROPTIONS.fields_by_name['deprecatedModeOne']._options = None
   _SLIDEROPTIONS.fields_by_name['deprecatedModeOne']._serialized_options = b'\030\001'
   _SLIDEROPTIONS.fields_by_name['deprecatedModeTwo']._options = None
@@ -86,152 +90,170 @@
   _PS4OPTIONS.fields_by_name['rsaDP']._serialized_options = b'\222?\003\010\200\001'
   _PS4OPTIONS.fields_by_name['rsaDQ']._options = None
   _PS4OPTIONS.fields_by_name['rsaDQ']._serialized_options = b'\222?\003\010\200\001'
   _PS4OPTIONS.fields_by_name['rsaQP']._options = None
   _PS4OPTIONS.fields_by_name['rsaQP']._serialized_options = b'\222?\003\010\200\001'
   _PS4OPTIONS.fields_by_name['rsaRN']._options = None
   _PS4OPTIONS.fields_by_name['rsaRN']._serialized_options = b'\222?\003\010\200\002'
+  _PSPASSTHROUGHOPTIONS.fields_by_name['enabled']._options = None
+  _PSPASSTHROUGHOPTIONS.fields_by_name['enabled']._serialized_options = b'\030\001'
   _PSPASSTHROUGHOPTIONS.fields_by_name['deprecatedPinDplus']._options = None
   _PSPASSTHROUGHOPTIONS.fields_by_name['deprecatedPinDplus']._serialized_options = b'\030\001'
   _PSPASSTHROUGHOPTIONS.fields_by_name['deprecatedPin5V']._options = None
   _PSPASSTHROUGHOPTIONS.fields_by_name['deprecatedPin5V']._serialized_options = b'\030\001'
+  _XBONEPASSTHROUGHOPTIONS.fields_by_name['enabled']._options = None
+  _XBONEPASSTHROUGHOPTIONS.fields_by_name['enabled']._serialized_options = b'\030\001'
   _WIIOPTIONS.fields_by_name['deprecatedI2cSDAPin']._options = None
   _WIIOPTIONS.fields_by_name['deprecatedI2cSDAPin']._serialized_options = b'\030\001'
   _WIIOPTIONS.fields_by_name['deprecatedI2cSCLPin']._options = None
   _WIIOPTIONS.fields_by_name['deprecatedI2cSCLPin']._serialized_options = b'\030\001'
   _WIIOPTIONS.fields_by_name['deprecatedI2cSpeed']._options = None
   _WIIOPTIONS.fields_by_name['deprecatedI2cSpeed']._serialized_options = b'\030\001'
   _KEYBOARDHOSTOPTIONS.fields_by_name['deprecatedPinDplus']._options = None
   _KEYBOARDHOSTOPTIONS.fields_by_name['deprecatedPinDplus']._serialized_options = b'\030\001'
   _KEYBOARDHOSTOPTIONS.fields_by_name['deprecatedPin5V']._options = None
   _KEYBOARDHOSTOPTIONS.fields_by_name['deprecatedPin5V']._serialized_options = b'\030\001'
   _MACRO.fields_by_name['macroLabel']._options = None
   _MACRO.fields_by_name['macroLabel']._serialized_options = b'\222?\002p@'
   _MACRO.fields_by_name['macroInputs']._options = None
   _MACRO.fields_by_name['macroInputs']._serialized_options = b'\222?\002\020\036'
+  _MACRO.fields_by_name['deprecatedMacroTriggerPin']._options = None
+  _MACRO.fields_by_name['deprecatedMacroTriggerPin']._serialized_options = b'\030\001'
+  _MACROOPTIONS.fields_by_name['deprecatedPin']._options = None
+  _MACROOPTIONS.fields_by_name['deprecatedPin']._serialized_options = b'\030\001'
   _MACROOPTIONS.fields_by_name['macroList']._options = None
   _MACROOPTIONS.fields_by_name['macroList']._serialized_options = b'\222?\002\020\006'
   _ADDONOPTIONS.fields_by_name['deprecatedExtraButtonOptions']._options = None
   _ADDONOPTIONS.fields_by_name['deprecatedExtraButtonOptions']._serialized_options = b'\030\001'
   _ADDONOPTIONS.fields_by_name['ps4Options']._options = None
   _ADDONOPTIONS.fields_by_name['ps4Options']._serialized_options = b'\222?\003\360\001\001'
+  _ADDONOPTIONS.fields_by_name['psPassthroughOptions']._options = None
+  _ADDONOPTIONS.fields_by_name['psPassthroughOptions']._serialized_options = b'\030\001'
+  _ADDONOPTIONS.fields_by_name['xbonePassthroughOptions']._options = None
+  _ADDONOPTIONS.fields_by_name['xbonePassthroughOptions']._serialized_options = b'\030\001'
   _CONFIG.fields_by_name['boardVersion']._options = None
   _CONFIG.fields_by_name['boardVersion']._serialized_options = b'\222?\002p\037'
   _CONFIG.fields_by_name['deprecatedPinMappings']._options = None
   _CONFIG.fields_by_name['deprecatedPinMappings']._serialized_options = b'\030\001'
   _CONFIG.fields_by_name['boardConfig']._options = None
   _CONFIG.fields_by_name['boardConfig']._serialized_options = b'\222?\002p?'
   _GAMEPADOPTIONS._serialized_start=44
-  _GAMEPADOPTIONS._serialized_end=546
-  _KEYBOARDMAPPING._serialized_start=549
-  _KEYBOARDMAPPING._serialized_end=943
-  _HOTKEYENTRY._serialized_start=945
-  _HOTKEYENTRY._serialized_end=1046
-  _HOTKEYOPTIONS._serialized_start=1049
-  _HOTKEYOPTIONS._serialized_end=1576
-  _PERIPHERALOPTIONS._serialized_start=1579
-  _PERIPHERALOPTIONS._serialized_end=2076
-  _PERIPHERALOPTIONS_I2COPTIONS._serialized_start=1850
-  _PERIPHERALOPTIONS_I2COPTIONS._serialized_end=1920
-  _PERIPHERALOPTIONS_SPIOPTIONS._serialized_start=1922
-  _PERIPHERALOPTIONS_SPIOPTIONS._serialized_end=2000
-  _PERIPHERALOPTIONS_USBOPTIONS._serialized_start=2002
-  _PERIPHERALOPTIONS_USBOPTIONS._serialized_end=2076
-  _FORCEDSETUPOPTIONS._serialized_start=2078
-  _FORCEDSETUPOPTIONS._serialized_end=2130
-  _BUTTONLAYOUTPARAMSCOMMON._serialized_start=2132
-  _BUTTONLAYOUTPARAMSCOMMON._serialized_end=2235
-  _BUTTONLAYOUTPARAMSLEFT._serialized_start=2237
-  _BUTTONLAYOUTPARAMSLEFT._serialized_end=2335
-  _BUTTONLAYOUTPARAMSRIGHT._serialized_start=2337
-  _BUTTONLAYOUTPARAMSRIGHT._serialized_end=2441
-  _BUTTONLAYOUTCUSTOMOPTIONS._serialized_start=2443
-  _BUTTONLAYOUTCUSTOMOPTIONS._serialized_end=2562
-  _PINMAPPINGS._serialized_start=2565
-  _PINMAPPINGS._serialized_end=2976
-  _GPIOMAPPINGINFO._serialized_start=2978
-  _GPIOMAPPINGINFO._serialized_end=3024
-  _GPIOMAPPINGS._serialized_start=3026
-  _GPIOMAPPINGS._serialized_end=3079
-  _ALTERNATIVEPINMAPPINGS._serialized_start=3082
-  _ALTERNATIVEPINMAPPINGS._serialized_end=3357
-  _PROFILEOPTIONS._serialized_start=3360
-  _PROFILEOPTIONS._serialized_end=3500
-  _DISPLAYOPTIONS._serialized_start=3503
-  _DISPLAYOPTIONS._serialized_end=4045
-  _LEDOPTIONS._serialized_start=4048
-  _LEDOPTIONS._serialized_end=4766
-  _ANIMATIONOPTIONS_PROTO._serialized_start=4769
-  _ANIMATIONOPTIONS_PROTO._serialized_end=5955
-  _BOOTSELBUTTONOPTIONS._serialized_start=5957
-  _BOOTSELBUTTONOPTIONS._serialized_end=6015
-  _ONBOARDLEDOPTIONS._serialized_start=6017
-  _ONBOARDLEDOPTIONS._serialized_end=6084
-  _ANALOGOPTIONS._serialized_start=6087
-  _ANALOGOPTIONS._serialized_end=6440
-  _TURBOOPTIONS._serialized_start=6443
-  _TURBOOPTIONS._serialized_end=6889
-  _SLIDEROPTIONS._serialized_start=6892
-  _SLIDEROPTIONS._serialized_end=7112
-  _SOCDSLIDEROPTIONS._serialized_start=7115
-  _SOCDSLIDEROPTIONS._serialized_end=7327
-  _REVERSEOPTIONS._serialized_start=7330
-  _REVERSEOPTIONS._serialized_end=7477
-  _ANALOGADS1219OPTIONS._serialized_start=7480
-  _ANALOGADS1219OPTIONS._serialized_end=7655
-  _DUALDIRECTIONALOPTIONS._serialized_start=7658
-  _DUALDIRECTIONALOPTIONS._serialized_end=7893
-  _TILTOPTIONS._serialized_start=7896
-  _TILTOPTIONS._serialized_end=8496
-  _BUZZEROPTIONS._serialized_start=8498
-  _BUZZEROPTIONS._serialized_end=8559
-  _EXTRABUTTONOPTIONS._serialized_start=8561
-  _EXTRABUTTONOPTIONS._serialized_end=8630
-  _PLAYERNUMBEROPTIONS._serialized_start=8632
-  _PLAYERNUMBEROPTIONS._serialized_end=8686
-  _PS4OPTIONS._serialized_start=8689
-  _PS4OPTIONS._serialized_end=8969
-  _PSPASSTHROUGHOPTIONS._serialized_start=8971
-  _PSPASSTHROUGHOPTIONS._serialized_end=9071
-  _XBONEPASSTHROUGHOPTIONS._serialized_start=9073
-  _XBONEPASSTHROUGHOPTIONS._serialized_end=9115
-  _WIIOPTIONS._serialized_start=9118
-  _WIIOPTIONS._serialized_end=11411
-  _WIIOPTIONS_ANALOGAXIS._serialized_start=9317
-  _WIIOPTIONS_ANALOGAXIS._serialized_end=9383
-  _WIIOPTIONS_STICKOPTIONS._serialized_start=9385
-  _WIIOPTIONS_STICKOPTIONS._serialized_end=9469
-  _WIIOPTIONS_NUNCHUKOPTIONS._serialized_start=9471
-  _WIIOPTIONS_NUNCHUKOPTIONS._serialized_end=9562
-  _WIIOPTIONS_CLASSICOPTIONS._serialized_start=9565
-  _WIIOPTIONS_CLASSICOPTIONS._serialized_end=10041
-  _WIIOPTIONS_TAIKOOPTIONS._serialized_start=10043
-  _WIIOPTIONS_TAIKOOPTIONS._serialized_end=10151
-  _WIIOPTIONS_GUITAROPTIONS._serialized_start=10154
-  _WIIOPTIONS_GUITAROPTIONS._serialized_end=10455
-  _WIIOPTIONS_DRUMOPTIONS._serialized_start=10458
-  _WIIOPTIONS_DRUMOPTIONS._serialized_end=10678
-  _WIIOPTIONS_TURNTABLEOPTIONS._serialized_start=10681
-  _WIIOPTIONS_TURNTABLEOPTIONS._serialized_end=11127
-  _WIIOPTIONS_CONTROLLEROPTIONS._serialized_start=11130
-  _WIIOPTIONS_CONTROLLEROPTIONS._serialized_end=11411
-  _SNESOPTIONS._serialized_start=11413
-  _SNESOPTIONS._serialized_end=11496
-  _KEYBOARDHOSTOPTIONS._serialized_start=11499
-  _KEYBOARDHOSTOPTIONS._serialized_end=11633
-  _FOCUSMODEOPTIONS._serialized_start=11636
-  _FOCUSMODEOPTIONS._serialized_end=11810
-  _MACROINPUT._serialized_start=11812
-  _MACROINPUT._serialized_end=11887
-  _MACRO._serialized_start=11890
-  _MACRO._serialized_end=12182
-  _MACROOPTIONS._serialized_start=12184
-  _MACROOPTIONS._serialized_end=12292
-  _INPUTHISTORYOPTIONS._serialized_start=12294
-  _INPUTHISTORYOPTIONS._serialized_end=12374
-  _ADDONOPTIONS._serialized_start=12377
-  _ADDONOPTIONS._serialized_end=13397
-  _MIGRATIONHISTORY._serialized_start=13399
-  _MIGRATIONHISTORY._serialized_end=13525
-  _CONFIG._serialized_start=13528
-  _CONFIG._serialized_end=14140
+  _GAMEPADOPTIONS._serialized_end=676
+  _KEYBOARDMAPPING._serialized_start=679
+  _KEYBOARDMAPPING._serialized_end=1073
+  _HOTKEYENTRY._serialized_start=1075
+  _HOTKEYENTRY._serialized_end=1176
+  _HOTKEYOPTIONS._serialized_start=1179
+  _HOTKEYOPTIONS._serialized_end=1706
+  _PERIPHERALOPTIONS._serialized_start=1709
+  _PERIPHERALOPTIONS._serialized_end=2206
+  _PERIPHERALOPTIONS_I2COPTIONS._serialized_start=1980
+  _PERIPHERALOPTIONS_I2COPTIONS._serialized_end=2050
+  _PERIPHERALOPTIONS_SPIOPTIONS._serialized_start=2052
+  _PERIPHERALOPTIONS_SPIOPTIONS._serialized_end=2130
+  _PERIPHERALOPTIONS_USBOPTIONS._serialized_start=2132
+  _PERIPHERALOPTIONS_USBOPTIONS._serialized_end=2206
+  _FORCEDSETUPOPTIONS._serialized_start=2208
+  _FORCEDSETUPOPTIONS._serialized_end=2260
+  _BUTTONLAYOUTPARAMSCOMMON._serialized_start=2262
+  _BUTTONLAYOUTPARAMSCOMMON._serialized_end=2365
+  _BUTTONLAYOUTPARAMSLEFT._serialized_start=2367
+  _BUTTONLAYOUTPARAMSLEFT._serialized_end=2465
+  _BUTTONLAYOUTPARAMSRIGHT._serialized_start=2467
+  _BUTTONLAYOUTPARAMSRIGHT._serialized_end=2571
+  _BUTTONLAYOUTCUSTOMOPTIONS._serialized_start=2573
+  _BUTTONLAYOUTCUSTOMOPTIONS._serialized_end=2692
+  _PINMAPPINGS._serialized_start=2695
+  _PINMAPPINGS._serialized_end=3106
+  _GPIOMAPPINGINFO._serialized_start=3108
+  _GPIOMAPPINGINFO._serialized_end=3154
+  _GPIOMAPPINGS._serialized_start=3156
+  _GPIOMAPPINGS._serialized_end=3209
+  _ALTERNATIVEPINMAPPINGS._serialized_start=3212
+  _ALTERNATIVEPINMAPPINGS._serialized_end=3487
+  _PROFILEOPTIONS._serialized_start=3490
+  _PROFILEOPTIONS._serialized_end=3630
+  _DISPLAYOPTIONS._serialized_start=3633
+  _DISPLAYOPTIONS._serialized_end=4175
+  _LEDOPTIONS._serialized_start=4178
+  _LEDOPTIONS._serialized_end=4896
+  _ANIMATIONOPTIONS_PROTO._serialized_start=4899
+  _ANIMATIONOPTIONS_PROTO._serialized_end=6127
+  _BOOTSELBUTTONOPTIONS._serialized_start=6129
+  _BOOTSELBUTTONOPTIONS._serialized_end=6187
+  _ONBOARDLEDOPTIONS._serialized_start=6189
+  _ONBOARDLEDOPTIONS._serialized_end=6256
+  _ANALOGOPTIONS._serialized_start=6259
+  _ANALOGOPTIONS._serialized_end=6612
+  _TURBOOPTIONS._serialized_start=6615
+  _TURBOOPTIONS._serialized_end=7075
+  _SLIDEROPTIONS._serialized_start=7078
+  _SLIDEROPTIONS._serialized_end=7298
+  _SOCDSLIDEROPTIONS._serialized_start=7301
+  _SOCDSLIDEROPTIONS._serialized_end=7513
+  _REVERSEOPTIONS._serialized_start=7516
+  _REVERSEOPTIONS._serialized_end=7663
+  _ANALOGADS1219OPTIONS._serialized_start=7666
+  _ANALOGADS1219OPTIONS._serialized_end=7841
+  _ANALOGADS1256OPTIONS._serialized_start=7843
+  _ANALOGADS1256OPTIONS._serialized_end=7970
+  _DUALDIRECTIONALOPTIONS._serialized_start=7973
+  _DUALDIRECTIONALOPTIONS._serialized_end=8241
+  _TILTOPTIONS._serialized_start=8244
+  _TILTOPTIONS._serialized_end=8844
+  _BUZZEROPTIONS._serialized_start=8846
+  _BUZZEROPTIONS._serialized_end=8926
+  _EXTRABUTTONOPTIONS._serialized_start=8928
+  _EXTRABUTTONOPTIONS._serialized_end=8997
+  _PLAYERNUMBEROPTIONS._serialized_start=8999
+  _PLAYERNUMBEROPTIONS._serialized_end=9053
+  _PS4OPTIONS._serialized_start=9056
+  _PS4OPTIONS._serialized_end=9336
+  _PSPASSTHROUGHOPTIONS._serialized_start=9338
+  _PSPASSTHROUGHOPTIONS._serialized_end=9442
+  _XBONEPASSTHROUGHOPTIONS._serialized_start=9444
+  _XBONEPASSTHROUGHOPTIONS._serialized_end=9490
+  _WIIOPTIONS._serialized_start=9493
+  _WIIOPTIONS._serialized_end=11786
+  _WIIOPTIONS_ANALOGAXIS._serialized_start=9692
+  _WIIOPTIONS_ANALOGAXIS._serialized_end=9758
+  _WIIOPTIONS_STICKOPTIONS._serialized_start=9760
+  _WIIOPTIONS_STICKOPTIONS._serialized_end=9844
+  _WIIOPTIONS_NUNCHUKOPTIONS._serialized_start=9846
+  _WIIOPTIONS_NUNCHUKOPTIONS._serialized_end=9937
+  _WIIOPTIONS_CLASSICOPTIONS._serialized_start=9940
+  _WIIOPTIONS_CLASSICOPTIONS._serialized_end=10416
+  _WIIOPTIONS_TAIKOOPTIONS._serialized_start=10418
+  _WIIOPTIONS_TAIKOOPTIONS._serialized_end=10526
+  _WIIOPTIONS_GUITAROPTIONS._serialized_start=10529
+  _WIIOPTIONS_GUITAROPTIONS._serialized_end=10830
+  _WIIOPTIONS_DRUMOPTIONS._serialized_start=10833
+  _WIIOPTIONS_DRUMOPTIONS._serialized_end=11053
+  _WIIOPTIONS_TURNTABLEOPTIONS._serialized_start=11056
+  _WIIOPTIONS_TURNTABLEOPTIONS._serialized_end=11502
+  _WIIOPTIONS_CONTROLLEROPTIONS._serialized_start=11505
+  _WIIOPTIONS_CONTROLLEROPTIONS._serialized_end=11786
+  _SNESOPTIONS._serialized_start=11788
+  _SNESOPTIONS._serialized_end=11871
+  _KEYBOARDHOSTOPTIONS._serialized_start=11874
+  _KEYBOARDHOSTOPTIONS._serialized_end=12008
+  _FOCUSMODEOPTIONS._serialized_start=12011
+  _FOCUSMODEOPTIONS._serialized_end=12185
+  _MACROINPUT._serialized_start=12187
+  _MACROINPUT._serialized_end=12262
+  _MACRO._serialized_start=12265
+  _MACRO._serialized_end=12567
+  _MACROOPTIONS._serialized_start=12569
+  _MACROOPTIONS._serialized_end=12691
+  _INPUTHISTORYOPTIONS._serialized_start=12693
+  _INPUTHISTORYOPTIONS._serialized_end=12773
+  _ROTARYPINOPTIONS._serialized_start=12776
+  _ROTARYPINOPTIONS._serialized_end=12970
+  _ROTARYOPTIONS._serialized_start=12972
+  _ROTARYOPTIONS._serialized_end=13082
+  _ADDONOPTIONS._serialized_start=13085
+  _ADDONOPTIONS._serialized_end=14205
+  _MIGRATIONHISTORY._serialized_start=14207
+  _MIGRATIONHISTORY._serialized_end=14333
+  _CONFIG._serialized_start=14336
+  _CONFIG._serialized_end=14948
 # @@protoc_insertion_point(module_scope)
```

### Comparing `gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/enums.proto` & `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/enums.proto`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,28 @@
     BUTTON_LAYOUT_TWINSTICKA = 7;
     BUTTON_LAYOUT_BLANKA = 8;
     BUTTON_LAYOUT_VLXA = 9;
     BUTTON_LAYOUT_FIGHTBOARD_STICK = 10;
     BUTTON_LAYOUT_FIGHTBOARD_MIRRORED = 11;
     BUTTON_LAYOUT_CUSTOMA = 12;
     BUTTON_LAYOUT_OPENCORE0WASDA = 13;
+    BUTTON_LAYOUT_STICKLESS_13 = 14;
+    BUTTON_LAYOUT_STICKLESS_16 = 15;
+    BUTTON_LAYOUT_STICKLESS_14 = 16;
+    BUTTON_LAYOUT_DANCEPAD_DDR_LEFT = 17;
+    BUTTON_LAYOUT_DANCEPAD_DDR_SOLO = 18;
+    BUTTON_LAYOUT_DANCEPAD_PIU_LEFT = 19;
+    BUTTON_LAYOUT_POPN_A = 20;
+    BUTTON_LAYOUT_TAIKO_A = 21;
+    BUTTON_LAYOUT_BM_TURNTABLE_A = 22;
+    BUTTON_LAYOUT_BM_5KEY_A = 23;
+    BUTTON_LAYOUT_BM_7KEY_A = 24;
+    BUTTON_LAYOUT_GITADORA_FRET_A = 25;
+    BUTTON_LAYOUT_GITADORA_STRUM_A = 26;
+    BUTTON_LAYOUT_BOARD_DEFINED_A = 27;
 }
 
 enum ButtonLayoutRight
 {
     option (nanopb_enumopt).long_names = false;
 
     BUTTON_LAYOUT_ARCADE = 0;
@@ -41,14 +55,27 @@
     BUTTON_LAYOUT_BLANKB = 12;
     BUTTON_LAYOUT_VLXB = 13;
     BUTTON_LAYOUT_FIGHTBOARD = 14;
     BUTTON_LAYOUT_FIGHTBOARD_STICK_MIRRORED = 15;
     BUTTON_LAYOUT_CUSTOMB = 16;
     BUTTON_LAYOUT_KEYBOARD8B = 17;
     BUTTON_LAYOUT_OPENCORE0WASDB = 18;
+    BUTTON_LAYOUT_STICKLESS_13B = 19;
+    BUTTON_LAYOUT_STICKLESS_16B = 20;
+    BUTTON_LAYOUT_STICKLESS_14B = 21;
+    BUTTON_LAYOUT_DANCEPAD_DDR_RIGHT = 22;
+    BUTTON_LAYOUT_DANCEPAD_PIU_RIGHT = 23;
+    BUTTON_LAYOUT_POPN_B = 24;
+    BUTTON_LAYOUT_TAIKO_B = 25;
+    BUTTON_LAYOUT_BM_TURNTABLE_B = 26;
+    BUTTON_LAYOUT_BM_5KEY_B = 27;
+    BUTTON_LAYOUT_BM_7KEY_B = 28;
+    BUTTON_LAYOUT_GITADORA_FRET_B = 29;
+    BUTTON_LAYOUT_GITADORA_STRUM_B = 30;
+    BUTTON_LAYOUT_BOARD_DEFINED_B = 31;
 }
 
 enum SplashMode
 {
     option (nanopb_enumopt).long_names = false;
 
     SPLASH_MODE_STATIC = 0;
@@ -92,17 +119,28 @@
     INPUT_MODE_MDMINI = 6;
     INPUT_MODE_NEOGEO = 7;
     INPUT_MODE_PCEMINI = 8;
     INPUT_MODE_EGRET = 9;
     INPUT_MODE_ASTRO = 10;
     INPUT_MODE_PSCLASSIC = 11;
     INPUT_MODE_XBOXORIGINAL = 12;
+    INPUT_MODE_PS5 = 13;
     INPUT_MODE_CONFIG = 255;
 }
 
+enum InputModeAuthType
+{
+    option (nanopb_enumopt).long_names = false;
+
+    INPUT_MODE_AUTH_TYPE_NONE = 0;
+    INPUT_MODE_AUTH_TYPE_KEYS = 1;
+    INPUT_MODE_AUTH_TYPE_USB = 2;
+    INPUT_MODE_AUTH_TYPE_I2C = 3;
+}
+
 enum DpadMode
 {
     option (nanopb_enumopt).long_names = false;
 
     DPAD_MODE_DIGITAL = 0;
     DPAD_MODE_LEFT_ANALOG = 1;
     DPAD_MODE_RIGHT_ANALOG = 2;
@@ -165,14 +203,22 @@
     SUSTAIN_DP_MODE_LS           = 25;
     SUSTAIN_DP_MODE_RS           = 26;
     SUSTAIN_SOCD_MODE_UP_PRIO    = 27;
     SUSTAIN_SOCD_MODE_NEUTRAL    = 28;
     SUSTAIN_SOCD_MODE_SECOND_WIN = 29;
     SUSTAIN_SOCD_MODE_FIRST_WIN  = 30;
     SUSTAIN_SOCD_MODE_BYPASS     = 31;
+    BUTTON_PRESS_TURBO           = 32;
+    BUTTON_PRESS_MACRO           = 33;
+    BUTTON_PRESS_MACRO_1         = 34;
+    BUTTON_PRESS_MACRO_2         = 35;
+    BUTTON_PRESS_MACRO_3         = 36;
+    BUTTON_PRESS_MACRO_4         = 37;
+    BUTTON_PRESS_MACRO_5         = 38;
+    BUTTON_PRESS_MACRO_6         = 39;
 }
 
 enum GamepadHotkey
 {
     option (nanopb_enumopt).long_names = false;
 
     HOTKEY_NONE                  = 0;
@@ -244,14 +290,24 @@
     
 	FORCED_SETUP_MODE_OFF = 0;
 	FORCED_SETUP_MODE_LOCK_MODE_SWITCH = 1;
 	FORCED_SETUP_MODE_LOCK_WEB_CONFIG = 2;
 	FORCED_SETUP_MODE_LOCK_BOTH = 3;
 };
 
+enum DualDirectionalCombinationMode
+{
+	option (nanopb_enumopt).long_names = false;
+
+	MIXED_MODE = 0;
+	GAMEPAD_MODE = 1;
+	DUAL_MODE = 2;
+	NONE_MODE = 3;
+}
+
 enum PS4ControllerType
 {
     option (nanopb_enumopt).long_names = false;
     
     PS4_CONTROLLER = 0;
     PS4_ARCADESTICK = 7;
 }
@@ -260,7 +316,48 @@
 {
     option (nanopb_enumopt).long_names = false;
 
     ON_PRESS = 1;
     ON_HOLD_REPEAT = 2;
     ON_TOGGLE = 3;
 };
+
+enum GPElement
+{
+    option (nanopb_enumopt).long_names = false;
+
+    GP_ELEMENT_WIDGET = 0;
+    GP_ELEMENT_SCREEN = 1;
+    GP_ELEMENT_BTN_BUTTON = 2;
+    GP_ELEMENT_DIR_BUTTON = 3;
+    GP_ELEMENT_PIN_BUTTON = 4;
+    GP_ELEMENT_LEVER = 5;
+    GP_ELEMENT_LABEL = 6;
+    GP_ELEMENT_SPRITE = 7;
+    GP_ELEMENT_SHAPE = 8;
+};
+
+enum GPShape_Type
+{
+    option (nanopb_enumopt).long_names = false;
+    
+    GP_SHAPE_ELLIPSE = 0;
+    GP_SHAPE_SQUARE = 1;
+    GP_SHAPE_DIAMOND = 2;
+    GP_SHAPE_POLYGON = 3;
+    GP_SHAPE_ARC = 4;
+};
+
+enum RotaryEncoderPinMode
+{
+    option (nanopb_enumopt).long_names = false;
+
+    ENCODER_MODE_NONE = 0;
+    ENCODER_MODE_LEFT_ANALOG_X = 1;
+    ENCODER_MODE_LEFT_ANALOG_Y = 2;
+    ENCODER_MODE_RIGHT_ANALOG_X = 3;
+    ENCODER_MODE_RIGHT_ANALOG_Y = 4;
+    ENCODER_MODE_LEFT_TRIGGER = 5;
+    ENCODER_MODE_RIGHT_TRIGGER = 6;
+    ENCODER_MODE_DPAD_X = 7;
+    ENCODER_MODE_DPAD_Y = 8;
+};
```

### Comparing `gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py` & `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import nanopb_pb2 as nanopb__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x65nums.proto\x1a\x0cnanopb.proto*\xc3\x03\n\x0c\x42uttonLayout\x12\x17\n\x13\x42UTTON_LAYOUT_STICK\x10\x00\x12\x1b\n\x17\x42UTTON_LAYOUT_STICKLESS\x10\x01\x12 \n\x1c\x42UTTON_LAYOUT_BUTTONS_ANGLED\x10\x02\x12\x1f\n\x1b\x42UTTON_LAYOUT_BUTTONS_BASIC\x10\x03\x12!\n\x1d\x42UTTON_LAYOUT_KEYBOARD_ANGLED\x10\x04\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDA\x10\x05\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADA\x10\x06\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKA\x10\x07\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKA\x10\x08\x12\x16\n\x12\x42UTTON_LAYOUT_VLXA\x10\t\x12\"\n\x1e\x42UTTON_LAYOUT_FIGHTBOARD_STICK\x10\n\x12%\n!BUTTON_LAYOUT_FIGHTBOARD_MIRRORED\x10\x0b\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMA\x10\x0c\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDA\x10\r\x1a\x05\x92?\x02 \x00*\xc2\x04\n\x11\x42uttonLayoutRight\x12\x18\n\x14\x42UTTON_LAYOUT_ARCADE\x10\x00\x12\x1c\n\x18\x42UTTON_LAYOUT_STICKLESSB\x10\x01\x12!\n\x1d\x42UTTON_LAYOUT_BUTTONS_ANGLEDB\x10\x02\x12\x18\n\x14\x42UTTON_LAYOUT_VEWLIX\x10\x03\x12\x19\n\x15\x42UTTON_LAYOUT_VEWLIX7\x10\x04\x12\x18\n\x14\x42UTTON_LAYOUT_CAPCOM\x10\x05\x12\x19\n\x15\x42UTTON_LAYOUT_CAPCOM6\x10\x06\x12\x18\n\x14\x42UTTON_LAYOUT_SEGA2P\x10\x07\x12\x17\n\x13\x42UTTON_LAYOUT_NOIR8\x10\x08\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDB\x10\t\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADB\x10\n\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKB\x10\x0b\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKB\x10\x0c\x12\x16\n\x12\x42UTTON_LAYOUT_VLXB\x10\r\x12\x1c\n\x18\x42UTTON_LAYOUT_FIGHTBOARD\x10\x0e\x12+\n\'BUTTON_LAYOUT_FIGHTBOARD_STICK_MIRRORED\x10\x0f\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMB\x10\x10\x12\x1c\n\x18\x42UTTON_LAYOUT_KEYBOARD8B\x10\x11\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDB\x10\x12\x1a\x05\x92?\x02 \x00*y\n\nSplashMode\x12\x16\n\x12SPLASH_MODE_STATIC\x10\x00\x12\x17\n\x13SPLASH_MODE_CLOSEIN\x10\x01\x12\x1d\n\x19SPLASH_MODE_CLOSEINCUSTOM\x10\x02\x12\x14\n\x10SPLASH_MODE_NONE\x10\x03\x1a\x05\x92?\x02 \x00*\xa0\x01\n\x0cSplashChoice\x12\x16\n\x12SPLASH_CHOICE_MAIN\x10\x00\x12\x13\n\x0fSPLASH_CHOICE_X\x10\x01\x12\x13\n\x0fSPLASH_CHOICE_Y\x10\x02\x12\x13\n\x0fSPLASH_CHOICE_Z\x10\x03\x12\x18\n\x14SPLASH_CHOICE_CUSTOM\x10\x04\x12\x18\n\x14SPLASH_CHOICE_LEGACY\x10\x05\x1a\x05\x92?\x02 \x00*\x99\x01\n\x0eOnBoardLedMode\x12\x19\n\x15ON_BOARD_LED_MODE_OFF\x10\x00\x12$\n ON_BOARD_LED_MODE_MODE_INDICATOR\x10\x01\x12 \n\x1cON_BOARD_LED_MODE_INPUT_TEST\x10\x02\x12\x1d\n\x19ON_BOARD_LED_MODE_PS_AUTH\x10\x03\x1a\x05\x92?\x02 \x00*\xd8\x02\n\tInputMode\x12\x15\n\x11INPUT_MODE_XINPUT\x10\x00\x12\x15\n\x11INPUT_MODE_SWITCH\x10\x01\x12\x12\n\x0eINPUT_MODE_HID\x10\x02\x12\x17\n\x13INPUT_MODE_KEYBOARD\x10\x03\x12\x12\n\x0eINPUT_MODE_PS4\x10\x04\x12\x14\n\x10INPUT_MODE_XBONE\x10\x05\x12\x15\n\x11INPUT_MODE_MDMINI\x10\x06\x12\x15\n\x11INPUT_MODE_NEOGEO\x10\x07\x12\x16\n\x12INPUT_MODE_PCEMINI\x10\x08\x12\x14\n\x10INPUT_MODE_EGRET\x10\t\x12\x14\n\x10INPUT_MODE_ASTRO\x10\n\x12\x18\n\x14INPUT_MODE_PSCLASSIC\x10\x0b\x12\x1b\n\x17INPUT_MODE_XBOXORIGINAL\x10\x0c\x12\x16\n\x11INPUT_MODE_CONFIG\x10\xff\x01\x1a\x05\x92?\x02 \x00*_\n\x08\x44padMode\x12\x15\n\x11\x44PAD_MODE_DIGITAL\x10\x00\x12\x19\n\x15\x44PAD_MODE_LEFT_ANALOG\x10\x01\x12\x1a\n\x16\x44PAD_MODE_RIGHT_ANALOG\x10\x02\x1a\x05\x92?\x02 \x00*O\n\nInvertMode\x12\x0f\n\x0bINVERT_NONE\x10\x00\x12\x0c\n\x08INVERT_X\x10\x01\x12\x0c\n\x08INVERT_Y\x10\x02\x12\r\n\tINVERT_XY\x10\x03\x1a\x05\x92?\x02 \x00*\xa2\x01\n\x08SOCDMode\x12\x19\n\x15SOCD_MODE_UP_PRIORITY\x10\x00\x12\x15\n\x11SOCD_MODE_NEUTRAL\x10\x01\x12#\n\x1fSOCD_MODE_SECOND_INPUT_PRIORITY\x10\x02\x12\"\n\x1eSOCD_MODE_FIRST_INPUT_PRIORITY\x10\x03\x12\x14\n\x10SOCD_MODE_BYPASS\x10\x04\x1a\x05\x92?\x02 \x00*\xbc\x06\n\nGpioAction\x12\x11\n\x04NONE\x10\xf6\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x08RESERVED\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x41SSIGNED_TO_ADDON\x10\x00\x12\x13\n\x0f\x42UTTON_PRESS_UP\x10\x01\x12\x15\n\x11\x42UTTON_PRESS_DOWN\x10\x02\x12\x15\n\x11\x42UTTON_PRESS_LEFT\x10\x03\x12\x16\n\x12\x42UTTON_PRESS_RIGHT\x10\x04\x12\x13\n\x0f\x42UTTON_PRESS_B1\x10\x05\x12\x13\n\x0f\x42UTTON_PRESS_B2\x10\x06\x12\x13\n\x0f\x42UTTON_PRESS_B3\x10\x07\x12\x13\n\x0f\x42UTTON_PRESS_B4\x10\x08\x12\x13\n\x0f\x42UTTON_PRESS_L1\x10\t\x12\x13\n\x0f\x42UTTON_PRESS_R1\x10\n\x12\x13\n\x0f\x42UTTON_PRESS_L2\x10\x0b\x12\x13\n\x0f\x42UTTON_PRESS_R2\x10\x0c\x12\x13\n\x0f\x42UTTON_PRESS_S1\x10\r\x12\x13\n\x0f\x42UTTON_PRESS_S2\x10\x0e\x12\x13\n\x0f\x42UTTON_PRESS_A1\x10\x0f\x12\x13\n\x0f\x42UTTON_PRESS_A2\x10\x10\x12\x13\n\x0f\x42UTTON_PRESS_L3\x10\x11\x12\x13\n\x0f\x42UTTON_PRESS_R3\x10\x12\x12\x13\n\x0f\x42UTTON_PRESS_FN\x10\x13\x12\x17\n\x13\x42UTTON_PRESS_DDI_UP\x10\x14\x12\x19\n\x15\x42UTTON_PRESS_DDI_DOWN\x10\x15\x12\x19\n\x15\x42UTTON_PRESS_DDI_LEFT\x10\x16\x12\x1a\n\x16\x42UTTON_PRESS_DDI_RIGHT\x10\x17\x12\x16\n\x12SUSTAIN_DP_MODE_DP\x10\x18\x12\x16\n\x12SUSTAIN_DP_MODE_LS\x10\x19\x12\x16\n\x12SUSTAIN_DP_MODE_RS\x10\x1a\x12\x1d\n\x19SUSTAIN_SOCD_MODE_UP_PRIO\x10\x1b\x12\x1d\n\x19SUSTAIN_SOCD_MODE_NEUTRAL\x10\x1c\x12 \n\x1cSUSTAIN_SOCD_MODE_SECOND_WIN\x10\x1d\x12\x1f\n\x1bSUSTAIN_SOCD_MODE_FIRST_WIN\x10\x1e\x12\x1c\n\x18SUSTAIN_SOCD_MODE_BYPASS\x10\x1f\x1a\x05\x92?\x02 \x00*\x80\x07\n\rGamepadHotkey\x12\x0f\n\x0bHOTKEY_NONE\x10\x00\x12\x17\n\x13HOTKEY_DPAD_DIGITAL\x10\x01\x12\x1b\n\x17HOTKEY_DPAD_LEFT_ANALOG\x10\x02\x12\x1c\n\x18HOTKEY_DPAD_RIGHT_ANALOG\x10\x03\x12\x16\n\x12HOTKEY_HOME_BUTTON\x10\x04\x12\x19\n\x15HOTKEY_CAPTURE_BUTTON\x10\x05\x12\x1b\n\x17HOTKEY_SOCD_UP_PRIORITY\x10\x06\x12\x17\n\x13HOTKEY_SOCD_NEUTRAL\x10\x07\x12\x1a\n\x16HOTKEY_SOCD_LAST_INPUT\x10\x08\x12\x18\n\x14HOTKEY_INVERT_X_AXIS\x10\t\x12\x18\n\x14HOTKEY_INVERT_Y_AXIS\x10\n\x12\x1b\n\x17HOTKEY_SOCD_FIRST_INPUT\x10\x0b\x12\x16\n\x12HOTKEY_SOCD_BYPASS\x10\x0c\x12\x1c\n\x18HOTKEY_TOGGLE_4_WAY_MODE\x10\r\x12 \n\x1cHOTKEY_TOGGLE_DDI_4_WAY_MODE\x10\x0e\x12\x19\n\x15HOTKEY_LOAD_PROFILE_1\x10\x0f\x12\x19\n\x15HOTKEY_LOAD_PROFILE_2\x10\x10\x12\x19\n\x15HOTKEY_LOAD_PROFILE_3\x10\x11\x12\x19\n\x15HOTKEY_LOAD_PROFILE_4\x10\x12\x12\x14\n\x10HOTKEY_L3_BUTTON\x10\x13\x12\x14\n\x10HOTKEY_R3_BUTTON\x10\x14\x12\x1a\n\x16HOTKEY_TOUCHPAD_BUTTON\x10\x15\x12\x19\n\x15HOTKEY_REBOOT_DEFAULT\x10\x16\x12\x14\n\x10HOTKEY_B1_BUTTON\x10\x17\x12\x14\n\x10HOTKEY_B2_BUTTON\x10\x18\x12\x14\n\x10HOTKEY_B3_BUTTON\x10\x19\x12\x14\n\x10HOTKEY_B4_BUTTON\x10\x1a\x12\x14\n\x10HOTKEY_L1_BUTTON\x10\x1b\x12\x14\n\x10HOTKEY_R1_BUTTON\x10\x1c\x12\x14\n\x10HOTKEY_L2_BUTTON\x10\x1d\x12\x14\n\x10HOTKEY_R2_BUTTON\x10\x1e\x12\x14\n\x10HOTKEY_S1_BUTTON\x10\x1f\x12\x14\n\x10HOTKEY_S2_BUTTON\x10 \x12\x14\n\x10HOTKEY_A1_BUTTON\x10!\x12\x14\n\x10HOTKEY_A2_BUTTON\x10\"\x1a\x05\x92?\x02 \x00*c\n\x0fLEDFormat_Proto\x12\x12\n\x0eLED_FORMAT_GRB\x10\x00\x12\x12\n\x0eLED_FORMAT_RGB\x10\x01\x12\x13\n\x0fLED_FORMAT_GRBW\x10\x02\x12\x13\n\x0fLED_FORMAT_RGBW\x10\x03*\\\n\x0cShmupMixMode\x12!\n\x1dSHMUP_MIX_MODE_TURBO_PRIORITY\x10\x00\x12\"\n\x1eSHMUP_MIX_MODE_CHARGE_PRIORITY\x10\x01\x1a\x05\x92?\x02 \x00*T\n\x08PLEDType\x12\x1b\n\x0ePLED_TYPE_NONE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x11\n\rPLED_TYPE_PWM\x10\x00\x12\x11\n\rPLED_TYPE_RGB\x10\x01\x1a\x05\x92?\x02 \x00*\xa3\x01\n\x0f\x46orcedSetupMode\x12\x19\n\x15\x46ORCED_SETUP_MODE_OFF\x10\x00\x12&\n\"FORCED_SETUP_MODE_LOCK_MODE_SWITCH\x10\x01\x12%\n!FORCED_SETUP_MODE_LOCK_WEB_CONFIG\x10\x02\x12\x1f\n\x1b\x46ORCED_SETUP_MODE_LOCK_BOTH\x10\x03\x1a\x05\x92?\x02 \x00*C\n\x11PS4ControllerType\x12\x12\n\x0ePS4_CONTROLLER\x10\x00\x12\x13\n\x0fPS4_ARCADESTICK\x10\x07\x1a\x05\x92?\x02 \x00*C\n\tMacroType\x12\x0c\n\x08ON_PRESS\x10\x01\x12\x12\n\x0eON_HOLD_REPEAT\x10\x02\x12\r\n\tON_TOGGLE\x10\x03\x1a\x05\x92?\x02 \x00')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x65nums.proto\x1a\x0cnanopb.proto*\x8d\x07\n\x0c\x42uttonLayout\x12\x17\n\x13\x42UTTON_LAYOUT_STICK\x10\x00\x12\x1b\n\x17\x42UTTON_LAYOUT_STICKLESS\x10\x01\x12 \n\x1c\x42UTTON_LAYOUT_BUTTONS_ANGLED\x10\x02\x12\x1f\n\x1b\x42UTTON_LAYOUT_BUTTONS_BASIC\x10\x03\x12!\n\x1d\x42UTTON_LAYOUT_KEYBOARD_ANGLED\x10\x04\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDA\x10\x05\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADA\x10\x06\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKA\x10\x07\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKA\x10\x08\x12\x16\n\x12\x42UTTON_LAYOUT_VLXA\x10\t\x12\"\n\x1e\x42UTTON_LAYOUT_FIGHTBOARD_STICK\x10\n\x12%\n!BUTTON_LAYOUT_FIGHTBOARD_MIRRORED\x10\x0b\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMA\x10\x0c\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDA\x10\r\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_13\x10\x0e\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_16\x10\x0f\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_14\x10\x10\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_LEFT\x10\x11\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_SOLO\x10\x12\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_PIU_LEFT\x10\x13\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_A\x10\x14\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_A\x10\x15\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_A\x10\x16\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_A\x10\x17\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_A\x10\x18\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_A\x10\x19\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_A\x10\x1a\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_A\x10\x1b\x1a\x05\x92?\x02 \x00*\xec\x07\n\x11\x42uttonLayoutRight\x12\x18\n\x14\x42UTTON_LAYOUT_ARCADE\x10\x00\x12\x1c\n\x18\x42UTTON_LAYOUT_STICKLESSB\x10\x01\x12!\n\x1d\x42UTTON_LAYOUT_BUTTONS_ANGLEDB\x10\x02\x12\x18\n\x14\x42UTTON_LAYOUT_VEWLIX\x10\x03\x12\x19\n\x15\x42UTTON_LAYOUT_VEWLIX7\x10\x04\x12\x18\n\x14\x42UTTON_LAYOUT_CAPCOM\x10\x05\x12\x19\n\x15\x42UTTON_LAYOUT_CAPCOM6\x10\x06\x12\x18\n\x14\x42UTTON_LAYOUT_SEGA2P\x10\x07\x12\x17\n\x13\x42UTTON_LAYOUT_NOIR8\x10\x08\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDB\x10\t\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADB\x10\n\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKB\x10\x0b\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKB\x10\x0c\x12\x16\n\x12\x42UTTON_LAYOUT_VLXB\x10\r\x12\x1c\n\x18\x42UTTON_LAYOUT_FIGHTBOARD\x10\x0e\x12+\n\'BUTTON_LAYOUT_FIGHTBOARD_STICK_MIRRORED\x10\x0f\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMB\x10\x10\x12\x1c\n\x18\x42UTTON_LAYOUT_KEYBOARD8B\x10\x11\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDB\x10\x12\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_13B\x10\x13\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_16B\x10\x14\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_14B\x10\x15\x12$\n BUTTON_LAYOUT_DANCEPAD_DDR_RIGHT\x10\x16\x12$\n BUTTON_LAYOUT_DANCEPAD_PIU_RIGHT\x10\x17\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_B\x10\x18\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_B\x10\x19\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_B\x10\x1a\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_B\x10\x1b\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_B\x10\x1c\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_B\x10\x1d\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_B\x10\x1e\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_B\x10\x1f\x1a\x05\x92?\x02 \x00*y\n\nSplashMode\x12\x16\n\x12SPLASH_MODE_STATIC\x10\x00\x12\x17\n\x13SPLASH_MODE_CLOSEIN\x10\x01\x12\x1d\n\x19SPLASH_MODE_CLOSEINCUSTOM\x10\x02\x12\x14\n\x10SPLASH_MODE_NONE\x10\x03\x1a\x05\x92?\x02 \x00*\xa0\x01\n\x0cSplashChoice\x12\x16\n\x12SPLASH_CHOICE_MAIN\x10\x00\x12\x13\n\x0fSPLASH_CHOICE_X\x10\x01\x12\x13\n\x0fSPLASH_CHOICE_Y\x10\x02\x12\x13\n\x0fSPLASH_CHOICE_Z\x10\x03\x12\x18\n\x14SPLASH_CHOICE_CUSTOM\x10\x04\x12\x18\n\x14SPLASH_CHOICE_LEGACY\x10\x05\x1a\x05\x92?\x02 \x00*\x99\x01\n\x0eOnBoardLedMode\x12\x19\n\x15ON_BOARD_LED_MODE_OFF\x10\x00\x12$\n ON_BOARD_LED_MODE_MODE_INDICATOR\x10\x01\x12 \n\x1cON_BOARD_LED_MODE_INPUT_TEST\x10\x02\x12\x1d\n\x19ON_BOARD_LED_MODE_PS_AUTH\x10\x03\x1a\x05\x92?\x02 \x00*\xec\x02\n\tInputMode\x12\x15\n\x11INPUT_MODE_XINPUT\x10\x00\x12\x15\n\x11INPUT_MODE_SWITCH\x10\x01\x12\x12\n\x0eINPUT_MODE_HID\x10\x02\x12\x17\n\x13INPUT_MODE_KEYBOARD\x10\x03\x12\x12\n\x0eINPUT_MODE_PS4\x10\x04\x12\x14\n\x10INPUT_MODE_XBONE\x10\x05\x12\x15\n\x11INPUT_MODE_MDMINI\x10\x06\x12\x15\n\x11INPUT_MODE_NEOGEO\x10\x07\x12\x16\n\x12INPUT_MODE_PCEMINI\x10\x08\x12\x14\n\x10INPUT_MODE_EGRET\x10\t\x12\x14\n\x10INPUT_MODE_ASTRO\x10\n\x12\x18\n\x14INPUT_MODE_PSCLASSIC\x10\x0b\x12\x1b\n\x17INPUT_MODE_XBOXORIGINAL\x10\x0c\x12\x12\n\x0eINPUT_MODE_PS5\x10\r\x12\x16\n\x11INPUT_MODE_CONFIG\x10\xff\x01\x1a\x05\x92?\x02 \x00*\x94\x01\n\x11InputModeAuthType\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_NONE\x10\x00\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_KEYS\x10\x01\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_USB\x10\x02\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_I2C\x10\x03\x1a\x05\x92?\x02 \x00*_\n\x08\x44padMode\x12\x15\n\x11\x44PAD_MODE_DIGITAL\x10\x00\x12\x19\n\x15\x44PAD_MODE_LEFT_ANALOG\x10\x01\x12\x1a\n\x16\x44PAD_MODE_RIGHT_ANALOG\x10\x02\x1a\x05\x92?\x02 \x00*O\n\nInvertMode\x12\x0f\n\x0bINVERT_NONE\x10\x00\x12\x0c\n\x08INVERT_X\x10\x01\x12\x0c\n\x08INVERT_Y\x10\x02\x12\r\n\tINVERT_XY\x10\x03\x1a\x05\x92?\x02 \x00*\xa2\x01\n\x08SOCDMode\x12\x19\n\x15SOCD_MODE_UP_PRIORITY\x10\x00\x12\x15\n\x11SOCD_MODE_NEUTRAL\x10\x01\x12#\n\x1fSOCD_MODE_SECOND_INPUT_PRIORITY\x10\x02\x12\"\n\x1eSOCD_MODE_FIRST_INPUT_PRIORITY\x10\x03\x12\x14\n\x10SOCD_MODE_BYPASS\x10\x04\x1a\x05\x92?\x02 \x00*\x88\x08\n\nGpioAction\x12\x11\n\x04NONE\x10\xf6\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x08RESERVED\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x41SSIGNED_TO_ADDON\x10\x00\x12\x13\n\x0f\x42UTTON_PRESS_UP\x10\x01\x12\x15\n\x11\x42UTTON_PRESS_DOWN\x10\x02\x12\x15\n\x11\x42UTTON_PRESS_LEFT\x10\x03\x12\x16\n\x12\x42UTTON_PRESS_RIGHT\x10\x04\x12\x13\n\x0f\x42UTTON_PRESS_B1\x10\x05\x12\x13\n\x0f\x42UTTON_PRESS_B2\x10\x06\x12\x13\n\x0f\x42UTTON_PRESS_B3\x10\x07\x12\x13\n\x0f\x42UTTON_PRESS_B4\x10\x08\x12\x13\n\x0f\x42UTTON_PRESS_L1\x10\t\x12\x13\n\x0f\x42UTTON_PRESS_R1\x10\n\x12\x13\n\x0f\x42UTTON_PRESS_L2\x10\x0b\x12\x13\n\x0f\x42UTTON_PRESS_R2\x10\x0c\x12\x13\n\x0f\x42UTTON_PRESS_S1\x10\r\x12\x13\n\x0f\x42UTTON_PRESS_S2\x10\x0e\x12\x13\n\x0f\x42UTTON_PRESS_A1\x10\x0f\x12\x13\n\x0f\x42UTTON_PRESS_A2\x10\x10\x12\x13\n\x0f\x42UTTON_PRESS_L3\x10\x11\x12\x13\n\x0f\x42UTTON_PRESS_R3\x10\x12\x12\x13\n\x0f\x42UTTON_PRESS_FN\x10\x13\x12\x17\n\x13\x42UTTON_PRESS_DDI_UP\x10\x14\x12\x19\n\x15\x42UTTON_PRESS_DDI_DOWN\x10\x15\x12\x19\n\x15\x42UTTON_PRESS_DDI_LEFT\x10\x16\x12\x1a\n\x16\x42UTTON_PRESS_DDI_RIGHT\x10\x17\x12\x16\n\x12SUSTAIN_DP_MODE_DP\x10\x18\x12\x16\n\x12SUSTAIN_DP_MODE_LS\x10\x19\x12\x16\n\x12SUSTAIN_DP_MODE_RS\x10\x1a\x12\x1d\n\x19SUSTAIN_SOCD_MODE_UP_PRIO\x10\x1b\x12\x1d\n\x19SUSTAIN_SOCD_MODE_NEUTRAL\x10\x1c\x12 \n\x1cSUSTAIN_SOCD_MODE_SECOND_WIN\x10\x1d\x12\x1f\n\x1bSUSTAIN_SOCD_MODE_FIRST_WIN\x10\x1e\x12\x1c\n\x18SUSTAIN_SOCD_MODE_BYPASS\x10\x1f\x12\x16\n\x12\x42UTTON_PRESS_TURBO\x10 \x12\x16\n\x12\x42UTTON_PRESS_MACRO\x10!\x12\x18\n\x14\x42UTTON_PRESS_MACRO_1\x10\"\x12\x18\n\x14\x42UTTON_PRESS_MACRO_2\x10#\x12\x18\n\x14\x42UTTON_PRESS_MACRO_3\x10$\x12\x18\n\x14\x42UTTON_PRESS_MACRO_4\x10%\x12\x18\n\x14\x42UTTON_PRESS_MACRO_5\x10&\x12\x18\n\x14\x42UTTON_PRESS_MACRO_6\x10\'\x1a\x05\x92?\x02 \x00*\x80\x07\n\rGamepadHotkey\x12\x0f\n\x0bHOTKEY_NONE\x10\x00\x12\x17\n\x13HOTKEY_DPAD_DIGITAL\x10\x01\x12\x1b\n\x17HOTKEY_DPAD_LEFT_ANALOG\x10\x02\x12\x1c\n\x18HOTKEY_DPAD_RIGHT_ANALOG\x10\x03\x12\x16\n\x12HOTKEY_HOME_BUTTON\x10\x04\x12\x19\n\x15HOTKEY_CAPTURE_BUTTON\x10\x05\x12\x1b\n\x17HOTKEY_SOCD_UP_PRIORITY\x10\x06\x12\x17\n\x13HOTKEY_SOCD_NEUTRAL\x10\x07\x12\x1a\n\x16HOTKEY_SOCD_LAST_INPUT\x10\x08\x12\x18\n\x14HOTKEY_INVERT_X_AXIS\x10\t\x12\x18\n\x14HOTKEY_INVERT_Y_AXIS\x10\n\x12\x1b\n\x17HOTKEY_SOCD_FIRST_INPUT\x10\x0b\x12\x16\n\x12HOTKEY_SOCD_BYPASS\x10\x0c\x12\x1c\n\x18HOTKEY_TOGGLE_4_WAY_MODE\x10\r\x12 \n\x1cHOTKEY_TOGGLE_DDI_4_WAY_MODE\x10\x0e\x12\x19\n\x15HOTKEY_LOAD_PROFILE_1\x10\x0f\x12\x19\n\x15HOTKEY_LOAD_PROFILE_2\x10\x10\x12\x19\n\x15HOTKEY_LOAD_PROFILE_3\x10\x11\x12\x19\n\x15HOTKEY_LOAD_PROFILE_4\x10\x12\x12\x14\n\x10HOTKEY_L3_BUTTON\x10\x13\x12\x14\n\x10HOTKEY_R3_BUTTON\x10\x14\x12\x1a\n\x16HOTKEY_TOUCHPAD_BUTTON\x10\x15\x12\x19\n\x15HOTKEY_REBOOT_DEFAULT\x10\x16\x12\x14\n\x10HOTKEY_B1_BUTTON\x10\x17\x12\x14\n\x10HOTKEY_B2_BUTTON\x10\x18\x12\x14\n\x10HOTKEY_B3_BUTTON\x10\x19\x12\x14\n\x10HOTKEY_B4_BUTTON\x10\x1a\x12\x14\n\x10HOTKEY_L1_BUTTON\x10\x1b\x12\x14\n\x10HOTKEY_R1_BUTTON\x10\x1c\x12\x14\n\x10HOTKEY_L2_BUTTON\x10\x1d\x12\x14\n\x10HOTKEY_R2_BUTTON\x10\x1e\x12\x14\n\x10HOTKEY_S1_BUTTON\x10\x1f\x12\x14\n\x10HOTKEY_S2_BUTTON\x10 \x12\x14\n\x10HOTKEY_A1_BUTTON\x10!\x12\x14\n\x10HOTKEY_A2_BUTTON\x10\"\x1a\x05\x92?\x02 \x00*c\n\x0fLEDFormat_Proto\x12\x12\n\x0eLED_FORMAT_GRB\x10\x00\x12\x12\n\x0eLED_FORMAT_RGB\x10\x01\x12\x13\n\x0fLED_FORMAT_GRBW\x10\x02\x12\x13\n\x0fLED_FORMAT_RGBW\x10\x03*\\\n\x0cShmupMixMode\x12!\n\x1dSHMUP_MIX_MODE_TURBO_PRIORITY\x10\x00\x12\"\n\x1eSHMUP_MIX_MODE_CHARGE_PRIORITY\x10\x01\x1a\x05\x92?\x02 \x00*T\n\x08PLEDType\x12\x1b\n\x0ePLED_TYPE_NONE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x11\n\rPLED_TYPE_PWM\x10\x00\x12\x11\n\rPLED_TYPE_RGB\x10\x01\x1a\x05\x92?\x02 \x00*\xa3\x01\n\x0f\x46orcedSetupMode\x12\x19\n\x15\x46ORCED_SETUP_MODE_OFF\x10\x00\x12&\n\"FORCED_SETUP_MODE_LOCK_MODE_SWITCH\x10\x01\x12%\n!FORCED_SETUP_MODE_LOCK_WEB_CONFIG\x10\x02\x12\x1f\n\x1b\x46ORCED_SETUP_MODE_LOCK_BOTH\x10\x03\x1a\x05\x92?\x02 \x00*g\n\x1e\x44ualDirectionalCombinationMode\x12\x0e\n\nMIXED_MODE\x10\x00\x12\x10\n\x0cGAMEPAD_MODE\x10\x01\x12\r\n\tDUAL_MODE\x10\x02\x12\r\n\tNONE_MODE\x10\x03\x1a\x05\x92?\x02 \x00*C\n\x11PS4ControllerType\x12\x12\n\x0ePS4_CONTROLLER\x10\x00\x12\x13\n\x0fPS4_ARCADESTICK\x10\x07\x1a\x05\x92?\x02 \x00*C\n\tMacroType\x12\x0c\n\x08ON_PRESS\x10\x01\x12\x12\n\x0eON_HOLD_REPEAT\x10\x02\x12\r\n\tON_TOGGLE\x10\x03\x1a\x05\x92?\x02 \x00*\xea\x01\n\tGPElement\x12\x15\n\x11GP_ELEMENT_WIDGET\x10\x00\x12\x15\n\x11GP_ELEMENT_SCREEN\x10\x01\x12\x19\n\x15GP_ELEMENT_BTN_BUTTON\x10\x02\x12\x19\n\x15GP_ELEMENT_DIR_BUTTON\x10\x03\x12\x19\n\x15GP_ELEMENT_PIN_BUTTON\x10\x04\x12\x14\n\x10GP_ELEMENT_LEVER\x10\x05\x12\x14\n\x10GP_ELEMENT_LABEL\x10\x06\x12\x15\n\x11GP_ELEMENT_SPRITE\x10\x07\x12\x14\n\x10GP_ELEMENT_SHAPE\x10\x08\x1a\x05\x92?\x02 \x00*~\n\x0cGPShape_Type\x12\x14\n\x10GP_SHAPE_ELLIPSE\x10\x00\x12\x13\n\x0fGP_SHAPE_SQUARE\x10\x01\x12\x14\n\x10GP_SHAPE_DIAMOND\x10\x02\x12\x14\n\x10GP_SHAPE_POLYGON\x10\x03\x12\x10\n\x0cGP_SHAPE_ARC\x10\x04\x1a\x05\x92?\x02 \x00*\xa7\x02\n\x14RotaryEncoderPinMode\x12\x15\n\x11\x45NCODER_MODE_NONE\x10\x00\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_X\x10\x01\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_Y\x10\x02\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_X\x10\x03\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_Y\x10\x04\x12\x1d\n\x19\x45NCODER_MODE_LEFT_TRIGGER\x10\x05\x12\x1e\n\x1a\x45NCODER_MODE_RIGHT_TRIGGER\x10\x06\x12\x17\n\x13\x45NCODER_MODE_DPAD_X\x10\x07\x12\x17\n\x13\x45NCODER_MODE_DPAD_Y\x10\x08\x1a\x05\x92?\x02 \x00')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'enums_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _BUTTONLAYOUT._options = None
@@ -29,14 +29,16 @@
   _SPLASHMODE._serialized_options = b'\222?\002 \000'
   _SPLASHCHOICE._options = None
   _SPLASHCHOICE._serialized_options = b'\222?\002 \000'
   _ONBOARDLEDMODE._options = None
   _ONBOARDLEDMODE._serialized_options = b'\222?\002 \000'
   _INPUTMODE._options = None
   _INPUTMODE._serialized_options = b'\222?\002 \000'
+  _INPUTMODEAUTHTYPE._options = None
+  _INPUTMODEAUTHTYPE._serialized_options = b'\222?\002 \000'
   _DPADMODE._options = None
   _DPADMODE._serialized_options = b'\222?\002 \000'
   _INVERTMODE._options = None
   _INVERTMODE._serialized_options = b'\222?\002 \000'
   _SOCDMODE._options = None
   _SOCDMODE._serialized_options = b'\222?\002 \000'
   _GPIOACTION._options = None
@@ -45,46 +47,64 @@
   _GAMEPADHOTKEY._serialized_options = b'\222?\002 \000'
   _SHMUPMIXMODE._options = None
   _SHMUPMIXMODE._serialized_options = b'\222?\002 \000'
   _PLEDTYPE._options = None
   _PLEDTYPE._serialized_options = b'\222?\002 \000'
   _FORCEDSETUPMODE._options = None
   _FORCEDSETUPMODE._serialized_options = b'\222?\002 \000'
+  _DUALDIRECTIONALCOMBINATIONMODE._options = None
+  _DUALDIRECTIONALCOMBINATIONMODE._serialized_options = b'\222?\002 \000'
   _PS4CONTROLLERTYPE._options = None
   _PS4CONTROLLERTYPE._serialized_options = b'\222?\002 \000'
   _MACROTYPE._options = None
   _MACROTYPE._serialized_options = b'\222?\002 \000'
+  _GPELEMENT._options = None
+  _GPELEMENT._serialized_options = b'\222?\002 \000'
+  _GPSHAPE_TYPE._options = None
+  _GPSHAPE_TYPE._serialized_options = b'\222?\002 \000'
+  _ROTARYENCODERPINMODE._options = None
+  _ROTARYENCODERPINMODE._serialized_options = b'\222?\002 \000'
   _BUTTONLAYOUT._serialized_start=30
-  _BUTTONLAYOUT._serialized_end=481
-  _BUTTONLAYOUTRIGHT._serialized_start=484
-  _BUTTONLAYOUTRIGHT._serialized_end=1062
-  _SPLASHMODE._serialized_start=1064
-  _SPLASHMODE._serialized_end=1185
-  _SPLASHCHOICE._serialized_start=1188
-  _SPLASHCHOICE._serialized_end=1348
-  _ONBOARDLEDMODE._serialized_start=1351
-  _ONBOARDLEDMODE._serialized_end=1504
-  _INPUTMODE._serialized_start=1507
-  _INPUTMODE._serialized_end=1851
-  _DPADMODE._serialized_start=1853
-  _DPADMODE._serialized_end=1948
-  _INVERTMODE._serialized_start=1950
-  _INVERTMODE._serialized_end=2029
-  _SOCDMODE._serialized_start=2032
-  _SOCDMODE._serialized_end=2194
-  _GPIOACTION._serialized_start=2197
-  _GPIOACTION._serialized_end=3025
-  _GAMEPADHOTKEY._serialized_start=3028
-  _GAMEPADHOTKEY._serialized_end=3924
-  _LEDFORMAT_PROTO._serialized_start=3926
-  _LEDFORMAT_PROTO._serialized_end=4025
-  _SHMUPMIXMODE._serialized_start=4027
-  _SHMUPMIXMODE._serialized_end=4119
-  _PLEDTYPE._serialized_start=4121
-  _PLEDTYPE._serialized_end=4205
-  _FORCEDSETUPMODE._serialized_start=4208
-  _FORCEDSETUPMODE._serialized_end=4371
-  _PS4CONTROLLERTYPE._serialized_start=4373
-  _PS4CONTROLLERTYPE._serialized_end=4440
-  _MACROTYPE._serialized_start=4442
-  _MACROTYPE._serialized_end=4509
+  _BUTTONLAYOUT._serialized_end=939
+  _BUTTONLAYOUTRIGHT._serialized_start=942
+  _BUTTONLAYOUTRIGHT._serialized_end=1946
+  _SPLASHMODE._serialized_start=1948
+  _SPLASHMODE._serialized_end=2069
+  _SPLASHCHOICE._serialized_start=2072
+  _SPLASHCHOICE._serialized_end=2232
+  _ONBOARDLEDMODE._serialized_start=2235
+  _ONBOARDLEDMODE._serialized_end=2388
+  _INPUTMODE._serialized_start=2391
+  _INPUTMODE._serialized_end=2755
+  _INPUTMODEAUTHTYPE._serialized_start=2758
+  _INPUTMODEAUTHTYPE._serialized_end=2906
+  _DPADMODE._serialized_start=2908
+  _DPADMODE._serialized_end=3003
+  _INVERTMODE._serialized_start=3005
+  _INVERTMODE._serialized_end=3084
+  _SOCDMODE._serialized_start=3087
+  _SOCDMODE._serialized_end=3249
+  _GPIOACTION._serialized_start=3252
+  _GPIOACTION._serialized_end=4284
+  _GAMEPADHOTKEY._serialized_start=4287
+  _GAMEPADHOTKEY._serialized_end=5183
+  _LEDFORMAT_PROTO._serialized_start=5185
+  _LEDFORMAT_PROTO._serialized_end=5284
+  _SHMUPMIXMODE._serialized_start=5286
+  _SHMUPMIXMODE._serialized_end=5378
+  _PLEDTYPE._serialized_start=5380
+  _PLEDTYPE._serialized_end=5464
+  _FORCEDSETUPMODE._serialized_start=5467
+  _FORCEDSETUPMODE._serialized_end=5630
+  _DUALDIRECTIONALCOMBINATIONMODE._serialized_start=5632
+  _DUALDIRECTIONALCOMBINATIONMODE._serialized_end=5735
+  _PS4CONTROLLERTYPE._serialized_start=5737
+  _PS4CONTROLLERTYPE._serialized_end=5804
+  _MACROTYPE._serialized_start=5806
+  _MACROTYPE._serialized_end=5873
+  _GPELEMENT._serialized_start=5876
+  _GPELEMENT._serialized_end=6110
+  _GPSHAPE_TYPE._serialized_start=6112
+  _GPSHAPE_TYPE._serialized_end=6238
+  _ROTARYENCODERPINMODE._serialized_start=6241
+  _ROTARYENCODERPINMODE._serialized_end=6536
 # @@protoc_insertion_point(module_scope)
```

### Comparing `gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/nanopb.proto` & `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py` & `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/rp2040.py` & `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/rp2040.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Methods to interact with the Raspberry Pi RP2040 directly.
 
 Much of this code is a partial Python implementation of picotool.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import logging
 import struct
 
 import usb.core
 
 logger = logging.getLogger(__name__)
```

### Comparing `gp2040ce-binary-tools-0.6.0/gp2040ce_bintools/storage.py` & `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/storage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Interact with the protobuf config from a picotool flash dump of a GP2040-CE board.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import argparse
 import binascii
 import logging
+import struct
 
 from google.protobuf.json_format import MessageToJson
 from google.protobuf.json_format import Parse as JsonParse
 from google.protobuf.message import Message
 
 from gp2040ce_bintools import core_parser, get_config_pb2
 from gp2040ce_bintools.rp2040 import get_bootsel_endpoints, read
@@ -21,14 +22,19 @@
 STORAGE_SIZE = 16384
 USER_CONFIG_BINARY_LOCATION = 0x1FC000
 USER_CONFIG_BOOTSEL_ADDRESS = 0x10000000 + USER_CONFIG_BINARY_LOCATION
 
 FOOTER_SIZE = 12
 FOOTER_MAGIC = b'\x65\xe3\xf1\xd2'
 
+UF2_FAMILY_ID = 0xE48BFF56
+UF2_MAGIC_FIRST = 0x0A324655
+UF2_MAGIC_SECOND = 0x9E5D5157
+UF2_MAGIC_FINAL = 0x0AB16F30
+
 
 #################
 # LIBRARY ITEMS #
 #################
 
 
 class ConfigReadError(ValueError):
@@ -43,14 +49,47 @@
     """Exception raised when a length sanity check fails."""
 
 
 class ConfigMagicError(ConfigReadError):
     """Exception raised when the config section does not have the magic value in its footer."""
 
 
+def convert_binary_to_uf2(binary: bytearray, start: int = 0) -> bytearray:
+    """Convert a GP2040-CE binary payload to Microsoft's UF2 format.
+
+    https://github.com/microsoft/uf2/tree/master#overview
+
+    Args:
+        binary: bytearray content to convert to a UF2 payload
+        start: position offset to start at rather than flash start (for creating e.g. user config UF2s)
+    Returns:
+        the content in UF2 format
+    """
+    size = len(binary)
+    blocks = (len(binary) // 256) + 1 if len(binary) % 256 else len(binary) // 256
+    uf2 = bytearray()
+
+    index = 0
+    while index < size:
+        pad_count = 476 - len(binary[index:index+256])
+        uf2 += struct.pack('<LLLLLLLL',
+                           UF2_MAGIC_FIRST,                                 # first magic number
+                           UF2_MAGIC_SECOND,                                # second magic number
+                           0x00002000,                                      # familyID present
+                           0x10000000 + start + index,                      # address to write to
+                           256,                                             # bytes to write in this block
+                           index // 256,                                    # sequential block number
+                           blocks,                                          # total number of blocks
+                           UF2_FAMILY_ID)                                   # family ID
+        uf2 += binary[index:index+256] + bytearray(b'\x00' * pad_count)     # content
+        uf2 += struct.pack('<L', UF2_MAGIC_FINAL)                           # final magic number
+        index += 256
+    return uf2
+
+
 def get_config(content: bytes) -> Message:
     """Read the config from a GP2040-CE storage section.
 
     Args:
         content: bytes from a GP2040-CE board's storage section
     Returns:
         the parsed configuration
@@ -276,24 +315,31 @@
 
 ############
 # COMMANDS #
 ############
 
 
 def dump_config():
-    """Save the GP2040-CE's configuration to a binary file."""
+    """Save the GP2040-CE's user configuration to a binary or UF2 file."""
     parser = argparse.ArgumentParser(
         description="Read the configuration section from a USB device and save it to a binary file.",
         parents=[core_parser],
     )
-    parser.add_argument('binary_filename', help=".bin file to save the GP2040-CE board's config section to")
+    parser.add_argument('filename', help="file to save the GP2040-CE board's config section to --- if the "
+                                         "suffix is .uf2, it is saved in UF2 format, else it is a raw binary")
     args, _ = parser.parse_known_args()
     config, _, _ = get_user_config_from_usb()
-    with open(args.binary_filename, 'wb') as out_file:
-        out_file.write(serialize_config_with_footer(config))
+    binary_config = serialize_config_with_footer(config)
+    with open(args.filename, 'wb') as out_file:
+        if args.filename[-4:] == '.uf2':
+            # we must pad to storage start in order for the UF2 write addresses to make sense
+            out_file.write(convert_binary_to_uf2(pad_config_to_storage_size(binary_config),
+                                                 start=USER_CONFIG_BINARY_LOCATION))
+        else:
+            out_file.write(binary_config)
 
 
 def visualize():
     """Print the contents of GP2040-CE's storage."""
     parser = argparse.ArgumentParser(
         description="Read the configuration section from a dump of a GP2040-CE board's storage section and print out "
                     "its contents.",
```

### Comparing `gp2040ce-binary-tools-0.6.0/pyproject.toml` & `gp2040ce-binary-tools-0.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gp2040ce-binary-tools"
 description = "Tools for working with GP2040-CE firmware and storage binaries."
 readme = "README.md"
-license = {text = "MIT"}
+license = {file = "LICENSE"}
 authors = [
     {name = "Brian S. Stephan", email = "bss@incorporeal.org"},
 ]
 requires-python = ">=3.9"
 dependencies = ["grpcio-tools", "pyusb", "textual"]
 dynamic = ["version"]
 classifiers = [
     "Environment :: Console",
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/OpenStickCommunity/gp2040ce-binary-tools"
 "Changelog" = "https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md"
```

### Comparing `gp2040ce-binary-tools-0.6.0/requirements/requirements-dev.txt` & `gp2040ce-binary-tools-0.7.0/requirements/requirements-dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,55 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --extra=dev --output-file=requirements/requirements-dev.txt
 #
-aiohttp==3.8.6
+aiohttp==3.9.3
     # via textual-dev
 aiosignal==1.3.1
     # via aiohttp
-async-timeout==4.0.3
+attrs==23.2.0
     # via aiohttp
-attrs==23.1.0
-    # via aiohttp
-bandit==1.7.5
+bandit==1.7.8
     # via gp2040ce-binary-tools (pyproject.toml)
-build==1.0.3
+build==1.2.1
     # via pip-tools
-cachetools==5.3.2
+cachetools==5.3.3
     # via tox
 chardet==5.2.0
     # via tox
-charset-normalizer==3.3.2
-    # via aiohttp
 click==8.1.7
     # via
     #   pip-tools
     #   textual-dev
 colorama==0.4.6
     # via tox
-coverage[toml]==7.3.2
+coverage[toml]==7.4.4
     # via pytest-cov
 decorator==5.1.1
     # via gp2040ce-binary-tools (pyproject.toml)
-distlib==0.3.7
+distlib==0.3.8
     # via virtualenv
-exceptiongroup==1.1.3
-    # via pytest
-filelock==3.13.1
+filelock==3.13.3
     # via
     #   tox
     #   virtualenv
-flake8==6.1.0
+flake8==7.0.0
     # via
     #   flake8-builtins
     #   flake8-docstrings
     #   flake8-executable
     #   flake8-isort
     #   flake8-mutable
     #   flake8-pyproject
     #   gp2040ce-binary-tools (pyproject.toml)
 flake8-blind-except==0.2.1
     # via gp2040ce-binary-tools (pyproject.toml)
-flake8-builtins==2.2.0
+flake8-builtins==2.4.0
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-docstrings==1.7.0
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-executable==2.1.3
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-fixme==1.1.1
     # via gp2040ce-binary-tools (pyproject.toml)
@@ -63,148 +57,128 @@
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-logging-format==0.9.0
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-mutable==1.2.0
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-pyproject==1.2.3
     # via gp2040ce-binary-tools (pyproject.toml)
-frozenlist==1.4.0
+frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-gitdb==4.0.11
-    # via gitpython
-gitpython==3.1.40
-    # via bandit
-grpcio==1.59.2
+grpcio==1.62.1
     # via grpcio-tools
-grpcio-tools==1.59.2
+grpcio-tools==1.62.1
     # via gp2040ce-binary-tools (pyproject.toml)
-idna==3.4
+idna==3.6
     # via yarl
-importlib-metadata==6.8.0
-    # via textual
 iniconfig==2.0.0
     # via pytest
-isort==5.12.0
+isort==5.13.2
     # via flake8-isort
-linkify-it-py==2.0.2
+linkify-it-py==2.0.3
     # via markdown-it-py
 markdown-it-py[linkify,plugins]==3.0.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
 mccabe==0.7.0
     # via flake8
 mdit-py-plugins==0.4.0
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
-msgpack==1.0.7
+msgpack==1.0.8
     # via textual-dev
-multidict==6.0.4
+multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
-mypy==1.6.1
+mypy==1.9.0
     # via gp2040ce-binary-tools (pyproject.toml)
 mypy-extensions==1.0.0
     # via mypy
-packaging==23.2
+packaging==24.0
     # via
     #   build
     #   pyproject-api
     #   pytest
     #   setuptools-scm
     #   tox
-pbr==5.11.1
+pbr==6.0.0
     # via stevedore
-pip-tools==7.3.0
+pip-tools==7.4.1
     # via gp2040ce-binary-tools (pyproject.toml)
-platformdirs==3.11.0
+platformdirs==4.2.0
     # via
     #   tox
     #   virtualenv
-pluggy==1.3.0
+pluggy==1.4.0
     # via
     #   pytest
     #   tox
-protobuf==4.25.0
+protobuf==4.25.3
     # via grpcio-tools
 pycodestyle==2.11.1
     # via flake8
 pydocstyle==6.3.0
     # via flake8-docstrings
-pyflakes==3.1.0
+pyflakes==3.2.0
     # via flake8
-pygments==2.16.1
+pygments==2.17.2
     # via rich
 pyproject-api==1.6.1
     # via tox
 pyproject-hooks==1.0.0
-    # via build
-pytest==7.4.3
+    # via
+    #   build
+    #   pip-tools
+pytest==8.1.1
     # via
     #   gp2040ce-binary-tools (pyproject.toml)
     #   pytest-asyncio
     #   pytest-cov
-pytest-asyncio==0.21.1
+pytest-asyncio==0.23.6
     # via gp2040ce-binary-tools (pyproject.toml)
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via gp2040ce-binary-tools (pyproject.toml)
 pyusb==1.2.1
     # via gp2040ce-binary-tools (pyproject.toml)
 pyyaml==6.0.1
     # via bandit
-rich==13.6.0
+rich==13.7.1
     # via
     #   bandit
     #   textual
 setuptools-scm==8.0.4
     # via gp2040ce-binary-tools (pyproject.toml)
-smmap==5.0.1
-    # via gitdb
 snowballstemmer==2.2.0
     # via pydocstyle
-stevedore==5.1.0
+stevedore==5.2.0
     # via bandit
-textual==0.41.0
+textual==0.56.2
     # via
     #   gp2040ce-binary-tools (pyproject.toml)
     #   textual-dev
-textual-dev==1.2.1
+textual-dev==1.5.1
     # via gp2040ce-binary-tools (pyproject.toml)
-tomli==2.0.1
-    # via
-    #   build
-    #   coverage
-    #   flake8-pyproject
-    #   mypy
-    #   pip-tools
-    #   pyproject-api
-    #   pyproject-hooks
-    #   pytest
-    #   setuptools-scm
-    #   tox
-tox==4.11.3
+tox==4.14.2
     # via gp2040ce-binary-tools (pyproject.toml)
-typing-extensions==4.8.0
+typing-extensions==4.11.0
     # via
     #   mypy
     #   setuptools-scm
     #   textual
     #   textual-dev
-uc-micro-py==1.0.2
+uc-micro-py==1.0.3
     # via linkify-it-py
-virtualenv==20.24.6
+virtualenv==20.25.1
     # via tox
-wheel==0.41.3
+wheel==0.43.0
     # via pip-tools
-yarl==1.9.2
+yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `gp2040ce-binary-tools-0.6.0/requirements/requirements.txt` & `gp2040ce-binary-tools-0.7.0/requirements/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --output-file=requirements/requirements.txt
 #
-grpcio==1.59.2
+grpcio==1.62.1
     # via grpcio-tools
-grpcio-tools==1.59.2
+grpcio-tools==1.62.1
     # via gp2040ce-binary-tools (pyproject.toml)
-importlib-metadata==6.8.0
-    # via textual
-linkify-it-py==2.0.2
+linkify-it-py==2.0.3
     # via markdown-it-py
 markdown-it-py[linkify,plugins]==3.0.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
 mdit-py-plugins==0.4.0
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
-protobuf==4.25.0
+protobuf==4.25.3
     # via grpcio-tools
-pygments==2.16.1
+pygments==2.17.2
     # via rich
 pyusb==1.2.1
     # via gp2040ce-binary-tools (pyproject.toml)
-rich==13.6.0
+rich==13.7.1
     # via textual
-textual==0.41.0
+textual==0.56.2
     # via gp2040ce-binary-tools (pyproject.toml)
-typing-extensions==4.8.0
+typing-extensions==4.11.0
     # via textual
-uc-micro-py==1.0.2
+uc-micro-py==1.0.3
     # via linkify-it-py
-zipp==3.17.0
-    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `gp2040ce-binary-tools-0.6.0/tests/conftest.py` & `gp2040ce-binary-tools-0.7.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Create the test fixtures and other data.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import os
 
 import pytest
 
 HERE = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/pb2-files/config_pb2.py` & `gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,35 +11,39 @@
 _sym_db = _symbol_database.Default()
 
 
 import nanopb_pb2 as nanopb__pb2
 import enums_pb2 as enums__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63onfig.proto\x1a\x0cnanopb.proto\x1a\x0b\x65nums.proto\"\xf6\x03\n\x0eGamepadOptions\x12\x1d\n\tinputMode\x18\x01 \x01(\x0e\x32\n.InputMode\x12\x1b\n\x08\x64padMode\x18\x02 \x01(\x0e\x32\t.DpadMode\x12\x1b\n\x08socdMode\x18\x03 \x01(\x0e\x32\t.SOCDMode\x12\x13\n\x0binvertXAxis\x18\x04 \x01(\x08\x12\x13\n\x0binvertYAxis\x18\x05 \x01(\x08\x12\x1b\n\x13switchTpShareForDs4\x18\x06 \x01(\x08\x12\x13\n\x0blockHotkeys\x18\x07 \x01(\x08\x12\x13\n\x0b\x66ourWayMode\x18\x08 \x01(\x08\x12\x15\n\rprofileNumber\x18\t \x01(\r\x12-\n\x11ps4ControllerType\x18\n \x01(\x0e\x32\x12.PS4ControllerType\x12\x15\n\rdebounceDelay\x18\x0b \x01(\r\x12\x13\n\x0binputModeB1\x18\x0c \x01(\x05\x12\x13\n\x0binputModeB2\x18\r \x01(\x05\x12\x13\n\x0binputModeB3\x18\x0e \x01(\x05\x12\x13\n\x0binputModeB4\x18\x0f \x01(\x05\x12\x13\n\x0binputModeL1\x18\x10 \x01(\x05\x12\x13\n\x0binputModeL2\x18\x11 \x01(\x05\x12\x13\n\x0binputModeR1\x18\x12 \x01(\x05\x12\x13\n\x0binputModeR2\x18\x13 \x01(\x05\x12\x15\n\rps4ReportHack\x18\x14 \x01(\x08\"\x8a\x03\n\x0fKeyboardMapping\x12\x11\n\tkeyDpadUp\x18\x01 \x01(\r\x12\x13\n\x0bkeyDpadDown\x18\x02 \x01(\r\x12\x13\n\x0bkeyDpadLeft\x18\x03 \x01(\r\x12\x14\n\x0ckeyDpadRight\x18\x04 \x01(\r\x12\x13\n\x0bkeyButtonB1\x18\x05 \x01(\r\x12\x13\n\x0bkeyButtonB2\x18\x06 \x01(\r\x12\x13\n\x0bkeyButtonB3\x18\x07 \x01(\r\x12\x13\n\x0bkeyButtonB4\x18\x08 \x01(\r\x12\x13\n\x0bkeyButtonL1\x18\t \x01(\r\x12\x13\n\x0bkeyButtonR1\x18\n \x01(\r\x12\x13\n\x0bkeyButtonL2\x18\x0b \x01(\r\x12\x13\n\x0bkeyButtonR2\x18\x0c \x01(\r\x12\x13\n\x0bkeyButtonS1\x18\r \x01(\r\x12\x13\n\x0bkeyButtonS2\x18\x0e \x01(\r\x12\x13\n\x0bkeyButtonL3\x18\x0f \x01(\r\x12\x13\n\x0bkeyButtonR3\x18\x10 \x01(\r\x12\x13\n\x0bkeyButtonA1\x18\x11 \x01(\r\x12\x13\n\x0bkeyButtonA2\x18\x12 \x01(\r\"e\n\x0bHotkeyEntry\x12\x10\n\x08\x64padMask\x18\x01 \x01(\r\x12\x1e\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x0e.GamepadHotkey\x12\x13\n\x0b\x62uttonsMask\x18\x03 \x01(\r\x12\x0f\n\x07\x61uxMask\x18\x04 \x01(\r\"\x8f\x04\n\rHotkeyOptions\x12\x1e\n\x08hotkey01\x18\x01 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey02\x18\x02 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey03\x18\x03 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey04\x18\x04 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey05\x18\x05 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey06\x18\x06 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey07\x18\x07 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey08\x18\x08 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey09\x18\t \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey10\x18\n \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey11\x18\x0b \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey12\x18\x0c \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey13\x18\r \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey14\x18\x0e \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey15\x18\x0f \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey16\x18\x10 \x01(\x0b\x32\x0c.HotkeyEntry\"\xf1\x03\n\x11PeripheralOptions\x12\x30\n\tblockI2C0\x18\x01 \x01(\x0b\x32\x1d.PeripheralOptions.I2COptions\x12\x30\n\tblockI2C1\x18\x02 \x01(\x0b\x32\x1d.PeripheralOptions.I2COptions\x12\x30\n\tblockSPI0\x18\x03 \x01(\x0b\x32\x1d.PeripheralOptions.SPIOptions\x12\x30\n\tblockSPI1\x18\x04 \x01(\x0b\x32\x1d.PeripheralOptions.SPIOptions\x12\x30\n\tblockUSB0\x18\x05 \x01(\x0b\x32\x1d.PeripheralOptions.USBOptions\x1a\x46\n\nI2COptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03sda\x18\x02 \x01(\x05\x12\x0b\n\x03scl\x18\x03 \x01(\x05\x12\r\n\x05speed\x18\x04 \x01(\r\x1aN\n\nSPIOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02rx\x18\x02 \x01(\x05\x12\n\n\x02\x63s\x18\x03 \x01(\x05\x12\x0b\n\x03sck\x18\x04 \x01(\x05\x12\n\n\x02tx\x18\x05 \x01(\x05\x1aJ\n\nUSBOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02\x64p\x18\x02 \x01(\x05\x12\x10\n\x08\x65nable5v\x18\x03 \x01(\x05\x12\r\n\x05order\x18\x04 \x01(\r\"4\n\x12\x46orcedSetupOptions\x12\x1e\n\x04mode\x18\x01 \x01(\x0e\x32\x10.ForcedSetupMode\"g\n\x18\x42uttonLayoutParamsCommon\x12\x0e\n\x06startX\x18\x01 \x01(\x05\x12\x0e\n\x06startY\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonRadius\x18\x03 \x01(\x05\x12\x15\n\rbuttonPadding\x18\x04 \x01(\x05\"b\n\x16\x42uttonLayoutParamsLeft\x12\x1d\n\x06layout\x18\x01 \x01(\x0e\x32\r.ButtonLayout\x12)\n\x06\x63ommon\x18\x02 \x01(\x0b\x32\x19.ButtonLayoutParamsCommon\"h\n\x17\x42uttonLayoutParamsRight\x12\"\n\x06layout\x18\x01 \x01(\x0e\x32\x12.ButtonLayoutRight\x12)\n\x06\x63ommon\x18\x02 \x01(\x0b\x32\x19.ButtonLayoutParamsCommon\"w\n\x19\x42uttonLayoutCustomOptions\x12+\n\nparamsLeft\x18\x01 \x01(\x0b\x32\x17.ButtonLayoutParamsLeft\x12-\n\x0bparamsRight\x18\x02 \x01(\x0b\x32\x18.ButtonLayoutParamsRight\"\x9b\x03\n\x0bPinMappings\x12\x11\n\tpinDpadUp\x18\x01 \x01(\x05\x12\x13\n\x0bpinDpadDown\x18\x02 \x01(\x05\x12\x13\n\x0bpinDpadLeft\x18\x03 \x01(\x05\x12\x14\n\x0cpinDpadRight\x18\x04 \x01(\x05\x12\x13\n\x0bpinButtonB1\x18\x05 \x01(\x05\x12\x13\n\x0bpinButtonB2\x18\x06 \x01(\x05\x12\x13\n\x0bpinButtonB3\x18\x07 \x01(\x05\x12\x13\n\x0bpinButtonB4\x18\x08 \x01(\x05\x12\x13\n\x0bpinButtonL1\x18\t \x01(\x05\x12\x13\n\x0bpinButtonR1\x18\n \x01(\x05\x12\x13\n\x0bpinButtonL2\x18\x0b \x01(\x05\x12\x13\n\x0bpinButtonR2\x18\x0c \x01(\x05\x12\x13\n\x0bpinButtonS1\x18\r \x01(\x05\x12\x13\n\x0bpinButtonS2\x18\x0e \x01(\x05\x12\x13\n\x0bpinButtonL3\x18\x0f \x01(\x05\x12\x13\n\x0bpinButtonR3\x18\x10 \x01(\x05\x12\x13\n\x0bpinButtonA1\x18\x11 \x01(\x05\x12\x13\n\x0bpinButtonA2\x18\x12 \x01(\x05\x12\x13\n\x0bpinButtonFn\x18\x13 \x01(\x05\".\n\x0fGpioMappingInfo\x12\x1b\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\x0b.GpioAction\"5\n\x0cGpioMappings\x12%\n\x04pins\x18\x01 \x03(\x0b\x32\x10.GpioMappingInfoB\x05\x92?\x02\x10\x1e\"\x93\x02\n\x16\x41lternativePinMappings\x12\x13\n\x0bpinButtonB1\x18\x01 \x01(\x05\x12\x13\n\x0bpinButtonB2\x18\x02 \x01(\x05\x12\x13\n\x0bpinButtonB3\x18\x03 \x01(\x05\x12\x13\n\x0bpinButtonB4\x18\x04 \x01(\x05\x12\x13\n\x0bpinButtonL1\x18\x05 \x01(\x05\x12\x13\n\x0bpinButtonR1\x18\x06 \x01(\x05\x12\x13\n\x0bpinButtonL2\x18\x07 \x01(\x05\x12\x13\n\x0bpinButtonR2\x18\x08 \x01(\x05\x12\x11\n\tpinDpadUp\x18\t \x01(\x05\x12\x13\n\x0bpinDpadDown\x18\n \x01(\x05\x12\x13\n\x0bpinDpadLeft\x18\x0b \x01(\x05\x12\x14\n\x0cpinDpadRight\x18\x0c \x01(\x05\"\x8c\x01\n\x0eProfileOptions\x12J\n deprecatedAlternativePinMappings\x18\x01 \x03(\x0b\x32\x17.AlternativePinMappingsB\x07\x18\x01\x92?\x02\x10\x03\x12.\n\x10gpioMappingsSets\x18\x02 \x03(\x0b\x32\r.GpioMappingsB\x05\x92?\x02\x10\x03\"\x9e\x04\n\x0e\x44isplayOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x12\n\ni2cAddress\x18\x05 \x01(\x05\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x06 \x01(\x05\x42\x02\x18\x01\x12#\n\x0c\x62uttonLayout\x18\x07 \x01(\x0e\x32\r.ButtonLayout\x12-\n\x11\x62uttonLayoutRight\x18\x08 \x01(\x0e\x32\x12.ButtonLayoutRight\x12=\n\x19\x62uttonLayoutCustomOptions\x18\t \x01(\x0b\x32\x1a.ButtonLayoutCustomOptions\x12\x1f\n\nsplashMode\x18\n \x01(\x0e\x32\x0b.SplashMode\x12#\n\x0csplashChoice\x18\x0b \x01(\x0e\x32\r.SplashChoice\x12\x16\n\x0esplashDuration\x18\x0c \x01(\x05\x12\x1b\n\x0bsplashImage\x18\r \x01(\x0c\x42\x06\x92?\x03\x08\x80\x08\x12\x0c\n\x04size\x18\x0e \x01(\x05\x12\x0c\n\x04\x66lip\x18\x0f \x01(\x05\x12\x0e\n\x06invert\x18\x10 \x01(\x08\x12\x1b\n\x13\x64isplaySaverTimeout\x18\x11 \x01(\x05\x12\x1c\n\x14turnOffWhenSuspended\x18\x12 \x01(\x08\"\xce\x05\n\nLEDOptions\x12\x0f\n\x07\x64\x61taPin\x18\x01 \x01(\x05\x12#\n\tledFormat\x18\x02 \x01(\x0e\x32\x10.LEDFormat_Proto\x12 \n\tledLayout\x18\x03 \x01(\x0e\x32\r.ButtonLayout\x12\x15\n\rledsPerButton\x18\x04 \x01(\r\x12\x19\n\x11\x62rightnessMaximum\x18\x05 \x01(\r\x12\x17\n\x0f\x62rightnessSteps\x18\x06 \x01(\r\x12\x0f\n\x07indexUp\x18\x07 \x01(\x05\x12\x11\n\tindexDown\x18\x08 \x01(\x05\x12\x11\n\tindexLeft\x18\t \x01(\x05\x12\x12\n\nindexRight\x18\n \x01(\x05\x12\x0f\n\x07indexB1\x18\x0b \x01(\x05\x12\x0f\n\x07indexB2\x18\x0c \x01(\x05\x12\x0f\n\x07indexB3\x18\r \x01(\x05\x12\x0f\n\x07indexB4\x18\x0e \x01(\x05\x12\x0f\n\x07indexL1\x18\x0f \x01(\x05\x12\x0f\n\x07indexR1\x18\x10 \x01(\x05\x12\x0f\n\x07indexL2\x18\x11 \x01(\x05\x12\x0f\n\x07indexR2\x18\x12 \x01(\x05\x12\x0f\n\x07indexS1\x18\x13 \x01(\x05\x12\x0f\n\x07indexS2\x18\x14 \x01(\x05\x12\x0f\n\x07indexL3\x18\x15 \x01(\x05\x12\x0f\n\x07indexR3\x18\x16 \x01(\x05\x12\x0f\n\x07indexA1\x18\x17 \x01(\x05\x12\x0f\n\x07indexA2\x18\x18 \x01(\x05\x12\x1b\n\x08pledType\x18\x19 \x01(\x0e\x32\t.PLEDType\x12\x10\n\x08pledPin1\x18\x1a \x01(\x05\x12\x10\n\x08pledPin2\x18\x1b \x01(\x05\x12\x10\n\x08pledPin3\x18\x1c \x01(\x05\x12\x10\n\x08pledPin4\x18\x1d \x01(\x05\x12\x11\n\tpledColor\x18\x1e \x01(\r\x12\x1c\n\x14turnOffWhenSuspended\x18\x1f \x01(\x08\x12\x12\n\npledIndex1\x18  \x01(\x05\x12\x12\n\npledIndex2\x18! \x01(\x05\x12\x12\n\npledIndex3\x18\" \x01(\x05\x12\x12\n\npledIndex4\x18# \x01(\x05\"\xa2\t\n\x16\x41nimationOptions_Proto\x12\x1a\n\x12\x62\x61seAnimationIndex\x18\x01 \x01(\r\x12\x12\n\nbrightness\x18\x02 \x01(\r\x12\x18\n\x10staticColorIndex\x18\x03 \x01(\r\x12\x18\n\x10\x62uttonColorIndex\x18\x04 \x01(\r\x12\x16\n\x0e\x63haseCycleTime\x18\x05 \x01(\x05\x12\x18\n\x10rainbowCycleTime\x18\x06 \x01(\x05\x12\x12\n\nthemeIndex\x18\x07 \x01(\r\x12\x16\n\x0ehasCustomTheme\x18\x08 \x01(\x08\x12\x15\n\rcustomThemeUp\x18\t \x01(\r\x12\x17\n\x0f\x63ustomThemeDown\x18\n \x01(\r\x12\x17\n\x0f\x63ustomThemeLeft\x18\x0b \x01(\r\x12\x18\n\x10\x63ustomThemeRight\x18\x0c \x01(\r\x12\x15\n\rcustomThemeB1\x18\r \x01(\r\x12\x15\n\rcustomThemeB2\x18\x0e \x01(\r\x12\x15\n\rcustomThemeB3\x18\x0f \x01(\r\x12\x15\n\rcustomThemeB4\x18\x10 \x01(\r\x12\x15\n\rcustomThemeL1\x18\x11 \x01(\r\x12\x15\n\rcustomThemeR1\x18\x12 \x01(\r\x12\x15\n\rcustomThemeL2\x18\x13 \x01(\r\x12\x15\n\rcustomThemeR2\x18\x14 \x01(\r\x12\x15\n\rcustomThemeS1\x18\x15 \x01(\r\x12\x15\n\rcustomThemeS2\x18\x16 \x01(\r\x12\x15\n\rcustomThemeL3\x18\x17 \x01(\r\x12\x15\n\rcustomThemeR3\x18\x18 \x01(\r\x12\x15\n\rcustomThemeA1\x18\x19 \x01(\r\x12\x15\n\rcustomThemeA2\x18\x1a \x01(\r\x12\x1c\n\x14\x63ustomThemeUpPressed\x18\x1b \x01(\r\x12\x1e\n\x16\x63ustomThemeDownPressed\x18\x1c \x01(\r\x12\x1e\n\x16\x63ustomThemeLeftPressed\x18\x1d \x01(\r\x12\x1f\n\x17\x63ustomThemeRightPressed\x18\x1e \x01(\r\x12\x1c\n\x14\x63ustomThemeB1Pressed\x18\x1f \x01(\r\x12\x1c\n\x14\x63ustomThemeB2Pressed\x18  \x01(\r\x12\x1c\n\x14\x63ustomThemeB3Pressed\x18! \x01(\r\x12\x1c\n\x14\x63ustomThemeB4Pressed\x18\" \x01(\r\x12\x1c\n\x14\x63ustomThemeL1Pressed\x18# \x01(\r\x12\x1c\n\x14\x63ustomThemeR1Pressed\x18$ \x01(\r\x12\x1c\n\x14\x63ustomThemeL2Pressed\x18% \x01(\r\x12\x1c\n\x14\x63ustomThemeR2Pressed\x18& \x01(\r\x12\x1c\n\x14\x63ustomThemeS1Pressed\x18\' \x01(\r\x12\x1c\n\x14\x63ustomThemeS2Pressed\x18( \x01(\r\x12\x1c\n\x14\x63ustomThemeL3Pressed\x18) \x01(\r\x12\x1c\n\x14\x63ustomThemeR3Pressed\x18* \x01(\r\x12\x1c\n\x14\x63ustomThemeA1Pressed\x18+ \x01(\r\x12\x1c\n\x14\x63ustomThemeA2Pressed\x18, \x01(\r\":\n\x14\x42ootselButtonOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbuttonMap\x18\x02 \x01(\r\"C\n\x11OnBoardLedOptions\x12\x1d\n\x04mode\x18\x01 \x01(\x0e\x32\x0f.OnBoardLedMode\x12\x0f\n\x07\x65nabled\x18\x02 \x01(\x08\"\xe1\x02\n\rAnalogOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0e\x61nalogAdc1PinX\x18\x02 \x01(\x05\x12\x16\n\x0e\x61nalogAdc1PinY\x18\x03 \x01(\x05\x12\x1a\n\x12\x66orced_circularity\x18\x04 \x01(\x08\x12\x17\n\x0f\x61nalog_deadzone\x18\x05 \x01(\r\x12\x16\n\x0e\x61nalogAdc2PinX\x18\x06 \x01(\x05\x12\x16\n\x0e\x61nalogAdc2PinY\x18\x07 \x01(\x05\x12!\n\x0e\x61nalogAdc1Mode\x18\x08 \x01(\x0e\x32\t.DpadMode\x12!\n\x0e\x61nalogAdc2Mode\x18\t \x01(\x0e\x32\t.DpadMode\x12%\n\x10\x61nalogAdc1Invert\x18\n \x01(\x0e\x32\x0b.InvertMode\x12%\n\x10\x61nalogAdc2Invert\x18\x0b \x01(\x0e\x32\x0b.InvertMode\x12\x16\n\x0e\x61uto_calibrate\x18\x0c \x01(\x08\"\xbe\x03\n\x0cTurboOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbuttonPin\x18\x02 \x01(\x05\x12\x0e\n\x06ledPin\x18\x03 \x01(\x05\x12\x11\n\tshotCount\x18\x04 \x01(\r\x12\x14\n\x0cshmupDialPin\x18\x05 \x01(\x05\x12\x18\n\x10shmupModeEnabled\x18\x06 \x01(\x08\x12\x16\n\x0eshmupAlwaysOn1\x18\x07 \x01(\r\x12\x16\n\x0eshmupAlwaysOn2\x18\x08 \x01(\r\x12\x16\n\x0eshmupAlwaysOn3\x18\t \x01(\r\x12\x16\n\x0eshmupAlwaysOn4\x18\n \x01(\r\x12\x14\n\x0cshmupBtn1Pin\x18\x0b \x01(\x05\x12\x14\n\x0cshmupBtn2Pin\x18\x0c \x01(\x05\x12\x14\n\x0cshmupBtn3Pin\x18\r \x01(\x05\x12\x14\n\x0cshmupBtn4Pin\x18\x0e \x01(\x05\x12\x15\n\rshmupBtnMask1\x18\x0f \x01(\r\x12\x15\n\rshmupBtnMask2\x18\x10 \x01(\r\x12\x15\n\rshmupBtnMask3\x18\x11 \x01(\r\x12\x15\n\rshmupBtnMask4\x18\x12 \x01(\r\x12#\n\x0cshmupMixMode\x18\x13 \x01(\x0e\x32\r.ShmupMixMode\"\xdc\x01\n\rSliderOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x16\x64\x65precatedPinSliderOne\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\"\n\x16\x64\x65precatedPinSliderTwo\x18\x03 \x01(\x05\x42\x02\x18\x01\x12(\n\x11\x64\x65precatedModeOne\x18\x04 \x01(\x0e\x32\t.DpadModeB\x02\x18\x01\x12(\n\x11\x64\x65precatedModeTwo\x18\x05 \x01(\x0e\x32\t.DpadModeB\x02\x18\x01\x12\x1e\n\x0bmodeDefault\x18\x06 \x01(\x0e\x32\t.DpadMode\"\xd4\x01\n\x11SOCDSliderOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1c\n\x10\x64\x65precatedPinOne\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1c\n\x10\x64\x65precatedPinTwo\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x0bmodeDefault\x18\x04 \x01(\x0e\x32\t.SOCDMode\x12(\n\x11\x64\x65precatedModeOne\x18\x05 \x01(\x0e\x32\t.SOCDModeB\x02\x18\x01\x12(\n\x11\x64\x65precatedModeTwo\x18\x06 \x01(\x0e\x32\t.SOCDModeB\x02\x18\x01\"\x93\x01\n\x0eReverseOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbuttonPin\x18\x02 \x01(\x05\x12\x0e\n\x06ledPin\x18\x03 \x01(\x05\x12\x10\n\x08\x61\x63tionUp\x18\x04 \x01(\r\x12\x12\n\nactionDown\x18\x05 \x01(\r\x12\x12\n\nactionLeft\x18\x06 \x01(\r\x12\x13\n\x0b\x61\x63tionRight\x18\x07 \x01(\r\"\xaf\x01\n\x14\x41nalogADS1219Options\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x12\n\ni2cAddress\x18\x05 \x01(\x05\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x06 \x01(\x05\x42\x02\x18\x01\"\xeb\x01\n\x16\x44ualDirectionalOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1b\n\x0f\x64\x65precatedUpPin\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1d\n\x11\x64\x65precatedDownPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1d\n\x11\x64\x65precatedLeftPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x12\x64\x65precatedRightPin\x18\x05 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x08\x64padMode\x18\x06 \x01(\x0e\x32\t.DpadMode\x12\x13\n\x0b\x63ombineMode\x18\x07 \x01(\r\x12\x13\n\x0b\x66ourWayMode\x18\x08 \x01(\x08\"\xd8\x04\n\x0bTiltOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08tilt1Pin\x18\x02 \x01(\x05\x12\x10\n\x08tilt2Pin\x18\x03 \x01(\x05\x12%\n\x19\x64\x65precatedTiltFunctionPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13tiltLeftAnalogUpPin\x18\x05 \x01(\x05\x12\x1d\n\x15tiltLeftAnalogDownPin\x18\x06 \x01(\x05\x12\x1d\n\x15tiltLeftAnalogLeftPin\x18\x07 \x01(\x05\x12\x1e\n\x16tiltLeftAnalogRightPin\x18\x08 \x01(\x05\x12\x1c\n\x14tiltRightAnalogUpPin\x18\t \x01(\x05\x12\x1e\n\x16tiltRightAnalogDownPin\x18\n \x01(\x05\x12\x1e\n\x16tiltRightAnalogLeftPin\x18\x0b \x01(\x05\x12\x1f\n\x17tiltRightAnalogRightPin\x18\x0c \x01(\x05\x12\x1f\n\x0ctiltSOCDMode\x18\r \x01(\x0e\x32\t.SOCDMode\x12\x18\n\x10\x66\x61\x63torTilt1LeftX\x18\x0e \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt1LeftY\x18\x0f \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt1RightX\x18\x10 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt1RightY\x18\x11 \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt2LeftX\x18\x12 \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt2LeftY\x18\x13 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt2RightX\x18\x14 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt2RightY\x18\x15 \x01(\x05\"=\n\rBuzzerOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x0e\n\x06volume\x18\x03 \x01(\r\"E\n\x12\x45xtraButtonOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x11\n\tbuttonMap\x18\x03 \x01(\r\"6\n\x13PlayerNumberOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06number\x18\x02 \x01(\r\"\x98\x02\n\nPS4Options\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\x06serial\x18\x02 \x01(\x0c\x42\x05\x92?\x02\x08\x10\x12\x19\n\tsignature\x18\x03 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x14\n\x04rsaN\x18\x04 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x13\n\x04rsaE\x18\x05 \x01(\x0c\x42\x05\x92?\x02\x08\x04\x12\x14\n\x04rsaD\x18\x06 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x14\n\x04rsaP\x18\x07 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x14\n\x04rsaQ\x18\x08 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaDP\x18\t \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaDQ\x18\n \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaQP\x18\x0b \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaRN\x18\x0c \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\"d\n\x14PSPassthroughOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\x12\x64\x65precatedPinDplus\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x0f\x64\x65precatedPin5V\x18\x03 \x01(\x05\x42\x02\x18\x01\"*\n\x17XBOnePassthroughOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\"\xf5\x11\n\nWiiOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x05 \x01(\x05\x42\x02\x18\x01\x12\x32\n\x0b\x63ontrollers\x18\x06 \x01(\x0b\x32\x1d.WiiOptions.ControllerOptions\x1a\x42\n\nAnalogAxis\x12\x10\n\x08\x61xisType\x18\x01 \x01(\x05\x12\x10\n\x08minRange\x18\x02 \x01(\x05\x12\x10\n\x08maxRange\x18\x03 \x01(\x05\x1aT\n\x0cStickOptions\x12!\n\x01x\x18\x01 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12!\n\x01y\x18\x02 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a[\n\x0eNunchukOptions\x12\x0f\n\x07\x62uttonC\x18\x01 \x01(\x05\x12\x0f\n\x07\x62uttonZ\x18\x02 \x01(\x05\x12\'\n\x05stick\x18\x03 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x1a\xdc\x03\n\x0e\x43lassicOptions\x12\x0f\n\x07\x62uttonA\x18\x01 \x01(\x05\x12\x0f\n\x07\x62uttonB\x18\x02 \x01(\x05\x12\x0f\n\x07\x62uttonX\x18\x03 \x01(\x05\x12\x0f\n\x07\x62uttonY\x18\x04 \x01(\x05\x12\x0f\n\x07\x62uttonL\x18\x05 \x01(\x05\x12\x10\n\x08\x62uttonZL\x18\x06 \x01(\x05\x12\x0f\n\x07\x62uttonR\x18\x07 \x01(\x05\x12\x10\n\x08\x62uttonZR\x18\x08 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\t \x01(\x05\x12\x12\n\nbuttonPlus\x18\n \x01(\x05\x12\x12\n\nbuttonHome\x18\x0b \x01(\x05\x12\x10\n\x08\x62uttonUp\x18\x0c \x01(\x05\x12\x12\n\nbuttonDown\x18\r \x01(\x05\x12\x12\n\nbuttonLeft\x18\x0e \x01(\x05\x12\x13\n\x0b\x62uttonRight\x18\x0f \x01(\x05\x12,\n\nrightStick\x18\x11 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12+\n\tleftStick\x18\x10 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12+\n\x0bleftTrigger\x18\x12 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12,\n\x0crightTrigger\x18\x13 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1al\n\x0cTaikoOptions\x12\x15\n\rbuttonKatLeft\x18\x01 \x01(\x05\x12\x16\n\x0e\x62uttonKatRight\x18\x02 \x01(\x05\x12\x15\n\rbuttonDonLeft\x18\x03 \x01(\x05\x12\x16\n\x0e\x62uttonDonRight\x18\x04 \x01(\x05\x1a\xad\x02\n\rGuitarOptions\x12\x11\n\tbuttonRed\x18\x01 \x01(\x05\x12\x13\n\x0b\x62uttonGreen\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonYellow\x18\x03 \x01(\x05\x12\x12\n\nbuttonBlue\x18\x04 \x01(\x05\x12\x14\n\x0c\x62uttonOrange\x18\x05 \x01(\x05\x12\x13\n\x0b\x62uttonPedal\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\x0f\n\x07strumUp\x18\t \x01(\x05\x12\x11\n\tstrumDown\x18\n \x01(\x05\x12\'\n\x05stick\x18\x0b \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12)\n\twhammyBar\x18\x0c \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a\xdc\x01\n\x0b\x44rumOptions\x12\x11\n\tbuttonRed\x18\x01 \x01(\x05\x12\x13\n\x0b\x62uttonGreen\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonYellow\x18\x03 \x01(\x05\x12\x12\n\nbuttonBlue\x18\x04 \x01(\x05\x12\x14\n\x0c\x62uttonOrange\x18\x05 \x01(\x05\x12\x13\n\x0b\x62uttonPedal\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\'\n\x05stick\x18\t \x01(\x0b\x32\x18.WiiOptions.StickOptions\x1a\xbe\x03\n\x10TurntableOptions\x12\x15\n\rbuttonLeftRed\x18\x01 \x01(\x05\x12\x17\n\x0f\x62uttonLeftGreen\x18\x02 \x01(\x05\x12\x16\n\x0e\x62uttonLeftBlue\x18\x03 \x01(\x05\x12\x16\n\x0e\x62uttonRightRed\x18\x04 \x01(\x05\x12\x18\n\x10\x62uttonRightGreen\x18\x05 \x01(\x05\x12\x17\n\x0f\x62uttonRightBlue\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\x16\n\x0e\x62uttonEuphoria\x18\t \x01(\x05\x12\'\n\x05stick\x18\n \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12-\n\rleftTurntable\x18\x0b \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12.\n\x0erightTurntable\x18\x0c \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12\'\n\x07\x65\x66\x66\x65\x63ts\x18\r \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12%\n\x05\x66\x61\x64\x65r\x18\x0e \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a\x99\x02\n\x11\x43ontrollerOptions\x12+\n\x07nunchuk\x18\x01 \x01(\x0b\x32\x1a.WiiOptions.NunchukOptions\x12+\n\x07\x63lassic\x18\x02 \x01(\x0b\x32\x1a.WiiOptions.ClassicOptions\x12\'\n\x05taiko\x18\x03 \x01(\x0b\x32\x18.WiiOptions.TaikoOptions\x12)\n\x06guitar\x18\x04 \x01(\x0b\x32\x19.WiiOptions.GuitarOptions\x12%\n\x04\x64rum\x18\x05 \x01(\x0b\x32\x17.WiiOptions.DrumOptions\x12/\n\tturntable\x18\x06 \x01(\x0b\x32\x1c.WiiOptions.TurntableOptions\"S\n\x0bSNESOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08\x63lockPin\x18\x02 \x01(\x05\x12\x10\n\x08latchPin\x18\x03 \x01(\x05\x12\x0f\n\x07\x64\x61taPin\x18\x04 \x01(\x05\"\x86\x01\n\x13KeyboardHostOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\x12\x64\x65precatedPinDplus\x18\x02 \x01(\x05\x42\x02\x18\x01\x12!\n\x07mapping\x18\x03 \x01(\x0b\x32\x10.KeyboardMapping\x12\x1b\n\x0f\x64\x65precatedPin5V\x18\x04 \x01(\x05\x42\x02\x18\x01\"\xae\x01\n\x10\x46ocusModeOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x16\n\x0e\x62uttonLockMask\x18\x03 \x01(\x05\x12\x17\n\x0foledLockEnabled\x18\x04 \x01(\x08\x12\x16\n\x0ergbLockEnabled\x18\x05 \x01(\x08\x12\x19\n\x11\x62uttonLockEnabled\x18\x06 \x01(\x08\x12\x18\n\x10macroLockEnabled\x18\x07 \x01(\x08\"K\n\nMacroInput\x12\x12\n\nbuttonMask\x18\x01 \x01(\r\x12\x10\n\x08\x64uration\x18\x02 \x01(\r\x12\x17\n\x0cwaitDuration\x18\x03 \x01(\r:\x01\x30\"\xa4\x02\n\x05Macro\x12\x1d\n\tmacroType\x18\x01 \x01(\x0e\x32\n.MacroType\x12\x19\n\nmacroLabel\x18\x02 \x01(\tB\x05\x92?\x02p@\x12\'\n\x0bmacroInputs\x18\x03 \x03(\x0b\x32\x0b.MacroInputB\x05\x92?\x02\x10\x1e\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\x12\x1d\n\x15useMacroTriggerButton\x18\x05 \x01(\x08\x12\x1b\n\x0fmacroTriggerPin\x18\x06 \x01(\x05:\x02-1\x12\x1a\n\x12macroTriggerButton\x18\x07 \x01(\r\x12\x17\n\texclusive\x18\x08 \x01(\x08:\x04true\x12\x1b\n\rinterruptible\x18\t \x01(\x08:\x04true\x12\x19\n\nshowFrames\x18\n \x01(\x08:\x05\x66\x61lse\"l\n\x0cMacroOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x1c\n\x14macroBoardLedEnabled\x18\x04 \x01(\x08\x12 \n\tmacroList\x18\x03 \x03(\x0b\x32\x06.MacroB\x05\x92?\x02\x10\x06\"P\n\x13InputHistoryOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06length\x18\x02 \x01(\r\x12\x0b\n\x03\x63ol\x18\x03 \x01(\r\x12\x0b\n\x03row\x18\x04 \x01(\r\"\xfc\x07\n\x0c\x41\x64\x64onOptions\x12\x33\n\x14\x62ootselButtonOptions\x18\x01 \x01(\x0b\x32\x15.BootselButtonOptions\x12-\n\x11onBoardLedOptions\x18\x02 \x01(\x0b\x32\x12.OnBoardLedOptions\x12%\n\ranalogOptions\x18\x03 \x01(\x0b\x32\x0e.AnalogOptions\x12#\n\x0cturboOptions\x18\x04 \x01(\x0b\x32\r.TurboOptions\x12%\n\rsliderOptions\x18\x05 \x01(\x0b\x32\x0e.SliderOptions\x12\'\n\x0ereverseOptions\x18\x06 \x01(\x0b\x32\x0f.ReverseOptions\x12\x33\n\x14\x61nalogADS1219Options\x18\x07 \x01(\x0b\x32\x15.AnalogADS1219Options\x12\x37\n\x16\x64ualDirectionalOptions\x18\x08 \x01(\x0b\x32\x17.DualDirectionalOptions\x12%\n\rbuzzerOptions\x18\t \x01(\x0b\x32\x0e.BuzzerOptions\x12=\n\x1c\x64\x65precatedExtraButtonOptions\x18\n \x01(\x0b\x32\x13.ExtraButtonOptionsB\x02\x18\x01\x12\x31\n\x13playerNumberOptions\x18\x0b \x01(\x0b\x32\x14.PlayerNumberOptions\x12\'\n\nps4Options\x18\x0c \x01(\x0b\x32\x0b.PS4OptionsB\x06\x92?\x03\xf0\x01\x01\x12\x1f\n\nwiiOptions\x18\r \x01(\x0b\x32\x0b.WiiOptions\x12-\n\x11socdSliderOptions\x18\x0e \x01(\x0b\x32\x12.SOCDSliderOptions\x12!\n\x0bsnesOptions\x18\x0f \x01(\x0b\x32\x0c.SNESOptions\x12+\n\x10\x66ocusModeOptions\x18\x10 \x01(\x0b\x32\x11.FocusModeOptions\x12\x31\n\x13keyboardHostOptions\x18\x11 \x01(\x0b\x32\x14.KeyboardHostOptions\x12!\n\x0btiltOptions\x18\x12 \x01(\x0b\x32\x0c.TiltOptions\x12\x33\n\x14psPassthroughOptions\x18\x13 \x01(\x0b\x32\x15.PSPassthroughOptions\x12#\n\x0cmacroOptions\x18\x14 \x01(\x0b\x32\r.MacroOptions\x12\x31\n\x13inputHistoryOptions\x18\x15 \x01(\x0b\x32\x14.InputHistoryOptions\x12\x39\n\x17xbonePassthroughOptions\x18\x16 \x01(\x0b\x32\x18.XBOnePassthroughOptions\"~\n\x10MigrationHistory\x12\x1e\n\x0fhotkeysMigrated\x18\x01 \x01(\x08:\x05\x66\x61lse\x12#\n\x14gpioMappingsMigrated\x18\x02 \x01(\x08:\x05\x66\x61lse\x12%\n\x16\x62uttonProfilesMigrated\x18\x03 \x01(\x08:\x05\x66\x61lse\"\xe4\x04\n\x06\x43onfig\x12\x1b\n\x0c\x62oardVersion\x18\x01 \x01(\tB\x05\x92?\x02p\x1f\x12\'\n\x0egamepadOptions\x18\x02 \x01(\x0b\x32\x0f.GamepadOptions\x12%\n\rhotkeyOptions\x18\x03 \x01(\x0b\x32\x0e.HotkeyOptions\x12/\n\x15\x64\x65precatedPinMappings\x18\x04 \x01(\x0b\x32\x0c.PinMappingsB\x02\x18\x01\x12)\n\x0fkeyboardMapping\x18\x05 \x01(\x0b\x32\x10.KeyboardMapping\x12\'\n\x0e\x64isplayOptions\x18\x06 \x01(\x0b\x32\x0f.DisplayOptions\x12\x1f\n\nledOptions\x18\x07 \x01(\x0b\x32\x0b.LEDOptions\x12\x31\n\x10\x61nimationOptions\x18\x08 \x01(\x0b\x32\x17.AnimationOptions_Proto\x12#\n\x0c\x61\x64\x64onOptions\x18\t \x01(\x0b\x32\r.AddonOptions\x12/\n\x12\x66orcedSetupOptions\x18\n \x01(\x0b\x32\x13.ForcedSetupOptions\x12\'\n\x0eprofileOptions\x18\x0b \x01(\x0b\x32\x0f.ProfileOptions\x12\x1a\n\x0b\x62oardConfig\x18\x0c \x01(\tB\x05\x92?\x02p?\x12#\n\x0cgpioMappings\x18\r \x01(\x0b\x32\r.GpioMappings\x12%\n\nmigrations\x18\x0e \x01(\x0b\x32\x11.MigrationHistory\x12-\n\x11peripheralOptions\x18\x0f \x01(\x0b\x32\x12.PeripheralOptions')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63onfig.proto\x1a\x0cnanopb.proto\x1a\x0b\x65nums.proto\"\xf8\x04\n\x0eGamepadOptions\x12\x1d\n\tinputMode\x18\x01 \x01(\x0e\x32\n.InputMode\x12\x1b\n\x08\x64padMode\x18\x02 \x01(\x0e\x32\t.DpadMode\x12\x1b\n\x08socdMode\x18\x03 \x01(\x0e\x32\t.SOCDMode\x12\x13\n\x0binvertXAxis\x18\x04 \x01(\x08\x12\x13\n\x0binvertYAxis\x18\x05 \x01(\x08\x12\x1b\n\x13switchTpShareForDs4\x18\x06 \x01(\x08\x12\x13\n\x0blockHotkeys\x18\x07 \x01(\x08\x12\x13\n\x0b\x66ourWayMode\x18\x08 \x01(\x08\x12\x15\n\rprofileNumber\x18\t \x01(\r\x12-\n\x11ps4ControllerType\x18\n \x01(\x0e\x32\x12.PS4ControllerType\x12\x15\n\rdebounceDelay\x18\x0b \x01(\r\x12\x13\n\x0binputModeB1\x18\x0c \x01(\x05\x12\x13\n\x0binputModeB2\x18\r \x01(\x05\x12\x13\n\x0binputModeB3\x18\x0e \x01(\x05\x12\x13\n\x0binputModeB4\x18\x0f \x01(\x05\x12\x13\n\x0binputModeL1\x18\x10 \x01(\x05\x12\x13\n\x0binputModeL2\x18\x11 \x01(\x05\x12\x13\n\x0binputModeR1\x18\x12 \x01(\x05\x12\x13\n\x0binputModeR2\x18\x13 \x01(\x05\x12\x19\n\rps4ReportHack\x18\x14 \x01(\x08\x42\x02\x18\x01\x12\'\n\x0bps4AuthType\x18\x15 \x01(\x0e\x32\x12.InputModeAuthType\x12\'\n\x0bps5AuthType\x18\x16 \x01(\x0e\x32\x12.InputModeAuthType\x12*\n\x0exinputAuthType\x18\x17 \x01(\x0e\x32\x12.InputModeAuthType\"\x8a\x03\n\x0fKeyboardMapping\x12\x11\n\tkeyDpadUp\x18\x01 \x01(\r\x12\x13\n\x0bkeyDpadDown\x18\x02 \x01(\r\x12\x13\n\x0bkeyDpadLeft\x18\x03 \x01(\r\x12\x14\n\x0ckeyDpadRight\x18\x04 \x01(\r\x12\x13\n\x0bkeyButtonB1\x18\x05 \x01(\r\x12\x13\n\x0bkeyButtonB2\x18\x06 \x01(\r\x12\x13\n\x0bkeyButtonB3\x18\x07 \x01(\r\x12\x13\n\x0bkeyButtonB4\x18\x08 \x01(\r\x12\x13\n\x0bkeyButtonL1\x18\t \x01(\r\x12\x13\n\x0bkeyButtonR1\x18\n \x01(\r\x12\x13\n\x0bkeyButtonL2\x18\x0b \x01(\r\x12\x13\n\x0bkeyButtonR2\x18\x0c \x01(\r\x12\x13\n\x0bkeyButtonS1\x18\r \x01(\r\x12\x13\n\x0bkeyButtonS2\x18\x0e \x01(\r\x12\x13\n\x0bkeyButtonL3\x18\x0f \x01(\r\x12\x13\n\x0bkeyButtonR3\x18\x10 \x01(\r\x12\x13\n\x0bkeyButtonA1\x18\x11 \x01(\r\x12\x13\n\x0bkeyButtonA2\x18\x12 \x01(\r\"e\n\x0bHotkeyEntry\x12\x10\n\x08\x64padMask\x18\x01 \x01(\r\x12\x1e\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x0e.GamepadHotkey\x12\x13\n\x0b\x62uttonsMask\x18\x03 \x01(\r\x12\x0f\n\x07\x61uxMask\x18\x04 \x01(\r\"\x8f\x04\n\rHotkeyOptions\x12\x1e\n\x08hotkey01\x18\x01 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey02\x18\x02 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey03\x18\x03 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey04\x18\x04 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey05\x18\x05 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey06\x18\x06 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey07\x18\x07 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey08\x18\x08 \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey09\x18\t \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey10\x18\n \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey11\x18\x0b \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey12\x18\x0c \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey13\x18\r \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey14\x18\x0e \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey15\x18\x0f \x01(\x0b\x32\x0c.HotkeyEntry\x12\x1e\n\x08hotkey16\x18\x10 \x01(\x0b\x32\x0c.HotkeyEntry\"\xf1\x03\n\x11PeripheralOptions\x12\x30\n\tblockI2C0\x18\x01 \x01(\x0b\x32\x1d.PeripheralOptions.I2COptions\x12\x30\n\tblockI2C1\x18\x02 \x01(\x0b\x32\x1d.PeripheralOptions.I2COptions\x12\x30\n\tblockSPI0\x18\x03 \x01(\x0b\x32\x1d.PeripheralOptions.SPIOptions\x12\x30\n\tblockSPI1\x18\x04 \x01(\x0b\x32\x1d.PeripheralOptions.SPIOptions\x12\x30\n\tblockUSB0\x18\x05 \x01(\x0b\x32\x1d.PeripheralOptions.USBOptions\x1a\x46\n\nI2COptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03sda\x18\x02 \x01(\x05\x12\x0b\n\x03scl\x18\x03 \x01(\x05\x12\r\n\x05speed\x18\x04 \x01(\r\x1aN\n\nSPIOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02rx\x18\x02 \x01(\x05\x12\n\n\x02\x63s\x18\x03 \x01(\x05\x12\x0b\n\x03sck\x18\x04 \x01(\x05\x12\n\n\x02tx\x18\x05 \x01(\x05\x1aJ\n\nUSBOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02\x64p\x18\x02 \x01(\x05\x12\x10\n\x08\x65nable5v\x18\x03 \x01(\x05\x12\r\n\x05order\x18\x04 \x01(\r\"4\n\x12\x46orcedSetupOptions\x12\x1e\n\x04mode\x18\x01 \x01(\x0e\x32\x10.ForcedSetupMode\"g\n\x18\x42uttonLayoutParamsCommon\x12\x0e\n\x06startX\x18\x01 \x01(\x05\x12\x0e\n\x06startY\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonRadius\x18\x03 \x01(\x05\x12\x15\n\rbuttonPadding\x18\x04 \x01(\x05\"b\n\x16\x42uttonLayoutParamsLeft\x12\x1d\n\x06layout\x18\x01 \x01(\x0e\x32\r.ButtonLayout\x12)\n\x06\x63ommon\x18\x02 \x01(\x0b\x32\x19.ButtonLayoutParamsCommon\"h\n\x17\x42uttonLayoutParamsRight\x12\"\n\x06layout\x18\x01 \x01(\x0e\x32\x12.ButtonLayoutRight\x12)\n\x06\x63ommon\x18\x02 \x01(\x0b\x32\x19.ButtonLayoutParamsCommon\"w\n\x19\x42uttonLayoutCustomOptions\x12+\n\nparamsLeft\x18\x01 \x01(\x0b\x32\x17.ButtonLayoutParamsLeft\x12-\n\x0bparamsRight\x18\x02 \x01(\x0b\x32\x18.ButtonLayoutParamsRight\"\x9b\x03\n\x0bPinMappings\x12\x11\n\tpinDpadUp\x18\x01 \x01(\x05\x12\x13\n\x0bpinDpadDown\x18\x02 \x01(\x05\x12\x13\n\x0bpinDpadLeft\x18\x03 \x01(\x05\x12\x14\n\x0cpinDpadRight\x18\x04 \x01(\x05\x12\x13\n\x0bpinButtonB1\x18\x05 \x01(\x05\x12\x13\n\x0bpinButtonB2\x18\x06 \x01(\x05\x12\x13\n\x0bpinButtonB3\x18\x07 \x01(\x05\x12\x13\n\x0bpinButtonB4\x18\x08 \x01(\x05\x12\x13\n\x0bpinButtonL1\x18\t \x01(\x05\x12\x13\n\x0bpinButtonR1\x18\n \x01(\x05\x12\x13\n\x0bpinButtonL2\x18\x0b \x01(\x05\x12\x13\n\x0bpinButtonR2\x18\x0c \x01(\x05\x12\x13\n\x0bpinButtonS1\x18\r \x01(\x05\x12\x13\n\x0bpinButtonS2\x18\x0e \x01(\x05\x12\x13\n\x0bpinButtonL3\x18\x0f \x01(\x05\x12\x13\n\x0bpinButtonR3\x18\x10 \x01(\x05\x12\x13\n\x0bpinButtonA1\x18\x11 \x01(\x05\x12\x13\n\x0bpinButtonA2\x18\x12 \x01(\x05\x12\x13\n\x0bpinButtonFn\x18\x13 \x01(\x05\".\n\x0fGpioMappingInfo\x12\x1b\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\x0b.GpioAction\"5\n\x0cGpioMappings\x12%\n\x04pins\x18\x01 \x03(\x0b\x32\x10.GpioMappingInfoB\x05\x92?\x02\x10\x1e\"\x93\x02\n\x16\x41lternativePinMappings\x12\x13\n\x0bpinButtonB1\x18\x01 \x01(\x05\x12\x13\n\x0bpinButtonB2\x18\x02 \x01(\x05\x12\x13\n\x0bpinButtonB3\x18\x03 \x01(\x05\x12\x13\n\x0bpinButtonB4\x18\x04 \x01(\x05\x12\x13\n\x0bpinButtonL1\x18\x05 \x01(\x05\x12\x13\n\x0bpinButtonR1\x18\x06 \x01(\x05\x12\x13\n\x0bpinButtonL2\x18\x07 \x01(\x05\x12\x13\n\x0bpinButtonR2\x18\x08 \x01(\x05\x12\x11\n\tpinDpadUp\x18\t \x01(\x05\x12\x13\n\x0bpinDpadDown\x18\n \x01(\x05\x12\x13\n\x0bpinDpadLeft\x18\x0b \x01(\x05\x12\x14\n\x0cpinDpadRight\x18\x0c \x01(\x05\"\x8c\x01\n\x0eProfileOptions\x12J\n deprecatedAlternativePinMappings\x18\x01 \x03(\x0b\x32\x17.AlternativePinMappingsB\x07\x18\x01\x92?\x02\x10\x03\x12.\n\x10gpioMappingsSets\x18\x02 \x03(\x0b\x32\r.GpioMappingsB\x05\x92?\x02\x10\x03\"\x9e\x04\n\x0e\x44isplayOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x12\n\ni2cAddress\x18\x05 \x01(\x05\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x06 \x01(\x05\x42\x02\x18\x01\x12#\n\x0c\x62uttonLayout\x18\x07 \x01(\x0e\x32\r.ButtonLayout\x12-\n\x11\x62uttonLayoutRight\x18\x08 \x01(\x0e\x32\x12.ButtonLayoutRight\x12=\n\x19\x62uttonLayoutCustomOptions\x18\t \x01(\x0b\x32\x1a.ButtonLayoutCustomOptions\x12\x1f\n\nsplashMode\x18\n \x01(\x0e\x32\x0b.SplashMode\x12#\n\x0csplashChoice\x18\x0b \x01(\x0e\x32\r.SplashChoice\x12\x16\n\x0esplashDuration\x18\x0c \x01(\x05\x12\x1b\n\x0bsplashImage\x18\r \x01(\x0c\x42\x06\x92?\x03\x08\x80\x08\x12\x0c\n\x04size\x18\x0e \x01(\x05\x12\x0c\n\x04\x66lip\x18\x0f \x01(\x05\x12\x0e\n\x06invert\x18\x10 \x01(\x08\x12\x1b\n\x13\x64isplaySaverTimeout\x18\x11 \x01(\x05\x12\x1c\n\x14turnOffWhenSuspended\x18\x12 \x01(\x08\"\xce\x05\n\nLEDOptions\x12\x0f\n\x07\x64\x61taPin\x18\x01 \x01(\x05\x12#\n\tledFormat\x18\x02 \x01(\x0e\x32\x10.LEDFormat_Proto\x12 \n\tledLayout\x18\x03 \x01(\x0e\x32\r.ButtonLayout\x12\x15\n\rledsPerButton\x18\x04 \x01(\r\x12\x19\n\x11\x62rightnessMaximum\x18\x05 \x01(\r\x12\x17\n\x0f\x62rightnessSteps\x18\x06 \x01(\r\x12\x0f\n\x07indexUp\x18\x07 \x01(\x05\x12\x11\n\tindexDown\x18\x08 \x01(\x05\x12\x11\n\tindexLeft\x18\t \x01(\x05\x12\x12\n\nindexRight\x18\n \x01(\x05\x12\x0f\n\x07indexB1\x18\x0b \x01(\x05\x12\x0f\n\x07indexB2\x18\x0c \x01(\x05\x12\x0f\n\x07indexB3\x18\r \x01(\x05\x12\x0f\n\x07indexB4\x18\x0e \x01(\x05\x12\x0f\n\x07indexL1\x18\x0f \x01(\x05\x12\x0f\n\x07indexR1\x18\x10 \x01(\x05\x12\x0f\n\x07indexL2\x18\x11 \x01(\x05\x12\x0f\n\x07indexR2\x18\x12 \x01(\x05\x12\x0f\n\x07indexS1\x18\x13 \x01(\x05\x12\x0f\n\x07indexS2\x18\x14 \x01(\x05\x12\x0f\n\x07indexL3\x18\x15 \x01(\x05\x12\x0f\n\x07indexR3\x18\x16 \x01(\x05\x12\x0f\n\x07indexA1\x18\x17 \x01(\x05\x12\x0f\n\x07indexA2\x18\x18 \x01(\x05\x12\x1b\n\x08pledType\x18\x19 \x01(\x0e\x32\t.PLEDType\x12\x10\n\x08pledPin1\x18\x1a \x01(\x05\x12\x10\n\x08pledPin2\x18\x1b \x01(\x05\x12\x10\n\x08pledPin3\x18\x1c \x01(\x05\x12\x10\n\x08pledPin4\x18\x1d \x01(\x05\x12\x11\n\tpledColor\x18\x1e \x01(\r\x12\x1c\n\x14turnOffWhenSuspended\x18\x1f \x01(\x08\x12\x12\n\npledIndex1\x18  \x01(\x05\x12\x12\n\npledIndex2\x18! \x01(\x05\x12\x12\n\npledIndex3\x18\" \x01(\x05\x12\x12\n\npledIndex4\x18# \x01(\x05\"\xcc\t\n\x16\x41nimationOptions_Proto\x12\x1a\n\x12\x62\x61seAnimationIndex\x18\x01 \x01(\r\x12\x12\n\nbrightness\x18\x02 \x01(\r\x12\x18\n\x10staticColorIndex\x18\x03 \x01(\r\x12\x18\n\x10\x62uttonColorIndex\x18\x04 \x01(\r\x12\x16\n\x0e\x63haseCycleTime\x18\x05 \x01(\x05\x12\x18\n\x10rainbowCycleTime\x18\x06 \x01(\x05\x12\x12\n\nthemeIndex\x18\x07 \x01(\r\x12\x16\n\x0ehasCustomTheme\x18\x08 \x01(\x08\x12\x15\n\rcustomThemeUp\x18\t \x01(\r\x12\x17\n\x0f\x63ustomThemeDown\x18\n \x01(\r\x12\x17\n\x0f\x63ustomThemeLeft\x18\x0b \x01(\r\x12\x18\n\x10\x63ustomThemeRight\x18\x0c \x01(\r\x12\x15\n\rcustomThemeB1\x18\r \x01(\r\x12\x15\n\rcustomThemeB2\x18\x0e \x01(\r\x12\x15\n\rcustomThemeB3\x18\x0f \x01(\r\x12\x15\n\rcustomThemeB4\x18\x10 \x01(\r\x12\x15\n\rcustomThemeL1\x18\x11 \x01(\r\x12\x15\n\rcustomThemeR1\x18\x12 \x01(\r\x12\x15\n\rcustomThemeL2\x18\x13 \x01(\r\x12\x15\n\rcustomThemeR2\x18\x14 \x01(\r\x12\x15\n\rcustomThemeS1\x18\x15 \x01(\r\x12\x15\n\rcustomThemeS2\x18\x16 \x01(\r\x12\x15\n\rcustomThemeL3\x18\x17 \x01(\r\x12\x15\n\rcustomThemeR3\x18\x18 \x01(\r\x12\x15\n\rcustomThemeA1\x18\x19 \x01(\r\x12\x15\n\rcustomThemeA2\x18\x1a \x01(\r\x12\x1c\n\x14\x63ustomThemeUpPressed\x18\x1b \x01(\r\x12\x1e\n\x16\x63ustomThemeDownPressed\x18\x1c \x01(\r\x12\x1e\n\x16\x63ustomThemeLeftPressed\x18\x1d \x01(\r\x12\x1f\n\x17\x63ustomThemeRightPressed\x18\x1e \x01(\r\x12\x1c\n\x14\x63ustomThemeB1Pressed\x18\x1f \x01(\r\x12\x1c\n\x14\x63ustomThemeB2Pressed\x18  \x01(\r\x12\x1c\n\x14\x63ustomThemeB3Pressed\x18! \x01(\r\x12\x1c\n\x14\x63ustomThemeB4Pressed\x18\" \x01(\r\x12\x1c\n\x14\x63ustomThemeL1Pressed\x18# \x01(\r\x12\x1c\n\x14\x63ustomThemeR1Pressed\x18$ \x01(\r\x12\x1c\n\x14\x63ustomThemeL2Pressed\x18% \x01(\r\x12\x1c\n\x14\x63ustomThemeR2Pressed\x18& \x01(\r\x12\x1c\n\x14\x63ustomThemeS1Pressed\x18\' \x01(\r\x12\x1c\n\x14\x63ustomThemeS2Pressed\x18( \x01(\r\x12\x1c\n\x14\x63ustomThemeL3Pressed\x18) \x01(\r\x12\x1c\n\x14\x63ustomThemeR3Pressed\x18* \x01(\r\x12\x1c\n\x14\x63ustomThemeA1Pressed\x18+ \x01(\r\x12\x1c\n\x14\x63ustomThemeA2Pressed\x18, \x01(\r\x12(\n buttonPressColorCooldownTimeInMs\x18- \x01(\r\":\n\x14\x42ootselButtonOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbuttonMap\x18\x02 \x01(\r\"C\n\x11OnBoardLedOptions\x12\x1d\n\x04mode\x18\x01 \x01(\x0e\x32\x0f.OnBoardLedMode\x12\x0f\n\x07\x65nabled\x18\x02 \x01(\x08\"\xe1\x02\n\rAnalogOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0e\x61nalogAdc1PinX\x18\x02 \x01(\x05\x12\x16\n\x0e\x61nalogAdc1PinY\x18\x03 \x01(\x05\x12\x1a\n\x12\x66orced_circularity\x18\x04 \x01(\x08\x12\x17\n\x0f\x61nalog_deadzone\x18\x05 \x01(\r\x12\x16\n\x0e\x61nalogAdc2PinX\x18\x06 \x01(\x05\x12\x16\n\x0e\x61nalogAdc2PinY\x18\x07 \x01(\x05\x12!\n\x0e\x61nalogAdc1Mode\x18\x08 \x01(\x0e\x32\t.DpadMode\x12!\n\x0e\x61nalogAdc2Mode\x18\t \x01(\x0e\x32\t.DpadMode\x12%\n\x10\x61nalogAdc1Invert\x18\n \x01(\x0e\x32\x0b.InvertMode\x12%\n\x10\x61nalogAdc2Invert\x18\x0b \x01(\x0e\x32\x0b.InvertMode\x12\x16\n\x0e\x61uto_calibrate\x18\x0c \x01(\x08\"\xcc\x03\n\x0cTurboOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1f\n\x13\x64\x65precatedButtonPin\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x0e\n\x06ledPin\x18\x03 \x01(\x05\x12\x11\n\tshotCount\x18\x04 \x01(\r\x12\x14\n\x0cshmupDialPin\x18\x05 \x01(\x05\x12\x18\n\x10shmupModeEnabled\x18\x06 \x01(\x08\x12\x16\n\x0eshmupAlwaysOn1\x18\x07 \x01(\r\x12\x16\n\x0eshmupAlwaysOn2\x18\x08 \x01(\r\x12\x16\n\x0eshmupAlwaysOn3\x18\t \x01(\r\x12\x16\n\x0eshmupAlwaysOn4\x18\n \x01(\r\x12\x14\n\x0cshmupBtn1Pin\x18\x0b \x01(\x05\x12\x14\n\x0cshmupBtn2Pin\x18\x0c \x01(\x05\x12\x14\n\x0cshmupBtn3Pin\x18\r \x01(\x05\x12\x14\n\x0cshmupBtn4Pin\x18\x0e \x01(\x05\x12\x15\n\rshmupBtnMask1\x18\x0f \x01(\r\x12\x15\n\rshmupBtnMask2\x18\x10 \x01(\r\x12\x15\n\rshmupBtnMask3\x18\x11 \x01(\r\x12\x15\n\rshmupBtnMask4\x18\x12 \x01(\r\x12#\n\x0cshmupMixMode\x18\x13 \x01(\x0e\x32\r.ShmupMixMode\"\xdc\x01\n\rSliderOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x16\x64\x65precatedPinSliderOne\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\"\n\x16\x64\x65precatedPinSliderTwo\x18\x03 \x01(\x05\x42\x02\x18\x01\x12(\n\x11\x64\x65precatedModeOne\x18\x04 \x01(\x0e\x32\t.DpadModeB\x02\x18\x01\x12(\n\x11\x64\x65precatedModeTwo\x18\x05 \x01(\x0e\x32\t.DpadModeB\x02\x18\x01\x12\x1e\n\x0bmodeDefault\x18\x06 \x01(\x0e\x32\t.DpadMode\"\xd4\x01\n\x11SOCDSliderOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1c\n\x10\x64\x65precatedPinOne\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1c\n\x10\x64\x65precatedPinTwo\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x0bmodeDefault\x18\x04 \x01(\x0e\x32\t.SOCDMode\x12(\n\x11\x64\x65precatedModeOne\x18\x05 \x01(\x0e\x32\t.SOCDModeB\x02\x18\x01\x12(\n\x11\x64\x65precatedModeTwo\x18\x06 \x01(\x0e\x32\t.SOCDModeB\x02\x18\x01\"\x93\x01\n\x0eReverseOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbuttonPin\x18\x02 \x01(\x05\x12\x0e\n\x06ledPin\x18\x03 \x01(\x05\x12\x10\n\x08\x61\x63tionUp\x18\x04 \x01(\r\x12\x12\n\nactionDown\x18\x05 \x01(\r\x12\x12\n\nactionLeft\x18\x06 \x01(\r\x12\x13\n\x0b\x61\x63tionRight\x18\x07 \x01(\r\"\xaf\x01\n\x14\x41nalogADS1219Options\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x12\n\ni2cAddress\x18\x05 \x01(\x05\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x06 \x01(\x05\x42\x02\x18\x01\"\x7f\n\x14\x41nalogADS1256Options\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08spiBlock\x18\x02 \x01(\x05\x12\r\n\x05\x63sPin\x18\x03 \x01(\x05\x12\x0f\n\x07\x64rdyPin\x18\x04 \x01(\x05\x12\x0c\n\x04\x61vdd\x18\x05 \x01(\x02\x12\x16\n\x0e\x65nableTriggers\x18\x06 \x01(\x08\"\x8c\x02\n\x16\x44ualDirectionalOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1b\n\x0f\x64\x65precatedUpPin\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1d\n\x11\x64\x65precatedDownPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1d\n\x11\x64\x65precatedLeftPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x12\x64\x65precatedRightPin\x18\x05 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x08\x64padMode\x18\x06 \x01(\x0e\x32\t.DpadMode\x12\x34\n\x0b\x63ombineMode\x18\x07 \x01(\x0e\x32\x1f.DualDirectionalCombinationMode\x12\x13\n\x0b\x66ourWayMode\x18\x08 \x01(\x08\"\xd8\x04\n\x0bTiltOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08tilt1Pin\x18\x02 \x01(\x05\x12\x10\n\x08tilt2Pin\x18\x03 \x01(\x05\x12%\n\x19\x64\x65precatedTiltFunctionPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13tiltLeftAnalogUpPin\x18\x05 \x01(\x05\x12\x1d\n\x15tiltLeftAnalogDownPin\x18\x06 \x01(\x05\x12\x1d\n\x15tiltLeftAnalogLeftPin\x18\x07 \x01(\x05\x12\x1e\n\x16tiltLeftAnalogRightPin\x18\x08 \x01(\x05\x12\x1c\n\x14tiltRightAnalogUpPin\x18\t \x01(\x05\x12\x1e\n\x16tiltRightAnalogDownPin\x18\n \x01(\x05\x12\x1e\n\x16tiltRightAnalogLeftPin\x18\x0b \x01(\x05\x12\x1f\n\x17tiltRightAnalogRightPin\x18\x0c \x01(\x05\x12\x1f\n\x0ctiltSOCDMode\x18\r \x01(\x0e\x32\t.SOCDMode\x12\x18\n\x10\x66\x61\x63torTilt1LeftX\x18\x0e \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt1LeftY\x18\x0f \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt1RightX\x18\x10 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt1RightY\x18\x11 \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt2LeftX\x18\x12 \x01(\x05\x12\x18\n\x10\x66\x61\x63torTilt2LeftY\x18\x13 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt2RightX\x18\x14 \x01(\x05\x12\x19\n\x11\x66\x61\x63torTilt2RightY\x18\x15 \x01(\x05\"P\n\rBuzzerOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x0e\n\x06volume\x18\x03 \x01(\r\x12\x11\n\tenablePin\x18\x04 \x01(\x05\"E\n\x12\x45xtraButtonOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x11\n\tbuttonMap\x18\x03 \x01(\r\"6\n\x13PlayerNumberOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06number\x18\x02 \x01(\r\"\x98\x02\n\nPS4Options\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\x06serial\x18\x02 \x01(\x0c\x42\x05\x92?\x02\x08\x10\x12\x19\n\tsignature\x18\x03 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x14\n\x04rsaN\x18\x04 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x13\n\x04rsaE\x18\x05 \x01(\x0c\x42\x05\x92?\x02\x08\x04\x12\x14\n\x04rsaD\x18\x06 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\x12\x14\n\x04rsaP\x18\x07 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x14\n\x04rsaQ\x18\x08 \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaDP\x18\t \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaDQ\x18\n \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaQP\x18\x0b \x01(\x0c\x42\x06\x92?\x03\x08\x80\x01\x12\x15\n\x05rsaRN\x18\x0c \x01(\x0c\x42\x06\x92?\x03\x08\x80\x02\"h\n\x14PSPassthroughOptions\x12\x13\n\x07\x65nabled\x18\x01 \x01(\x08\x42\x02\x18\x01\x12\x1e\n\x12\x64\x65precatedPinDplus\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x0f\x64\x65precatedPin5V\x18\x03 \x01(\x05\x42\x02\x18\x01\".\n\x17XBOnePassthroughOptions\x12\x13\n\x07\x65nabled\x18\x01 \x01(\x08\x42\x02\x18\x01\"\xf5\x11\n\nWiiOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08i2cBlock\x18\x02 \x01(\x05\x12\x1f\n\x13\x64\x65precatedI2cSDAPin\x18\x03 \x01(\x05\x42\x02\x18\x01\x12\x1f\n\x13\x64\x65precatedI2cSCLPin\x18\x04 \x01(\x05\x42\x02\x18\x01\x12\x1e\n\x12\x64\x65precatedI2cSpeed\x18\x05 \x01(\x05\x42\x02\x18\x01\x12\x32\n\x0b\x63ontrollers\x18\x06 \x01(\x0b\x32\x1d.WiiOptions.ControllerOptions\x1a\x42\n\nAnalogAxis\x12\x10\n\x08\x61xisType\x18\x01 \x01(\x05\x12\x10\n\x08minRange\x18\x02 \x01(\x05\x12\x10\n\x08maxRange\x18\x03 \x01(\x05\x1aT\n\x0cStickOptions\x12!\n\x01x\x18\x01 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12!\n\x01y\x18\x02 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a[\n\x0eNunchukOptions\x12\x0f\n\x07\x62uttonC\x18\x01 \x01(\x05\x12\x0f\n\x07\x62uttonZ\x18\x02 \x01(\x05\x12\'\n\x05stick\x18\x03 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x1a\xdc\x03\n\x0e\x43lassicOptions\x12\x0f\n\x07\x62uttonA\x18\x01 \x01(\x05\x12\x0f\n\x07\x62uttonB\x18\x02 \x01(\x05\x12\x0f\n\x07\x62uttonX\x18\x03 \x01(\x05\x12\x0f\n\x07\x62uttonY\x18\x04 \x01(\x05\x12\x0f\n\x07\x62uttonL\x18\x05 \x01(\x05\x12\x10\n\x08\x62uttonZL\x18\x06 \x01(\x05\x12\x0f\n\x07\x62uttonR\x18\x07 \x01(\x05\x12\x10\n\x08\x62uttonZR\x18\x08 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\t \x01(\x05\x12\x12\n\nbuttonPlus\x18\n \x01(\x05\x12\x12\n\nbuttonHome\x18\x0b \x01(\x05\x12\x10\n\x08\x62uttonUp\x18\x0c \x01(\x05\x12\x12\n\nbuttonDown\x18\r \x01(\x05\x12\x12\n\nbuttonLeft\x18\x0e \x01(\x05\x12\x13\n\x0b\x62uttonRight\x18\x0f \x01(\x05\x12,\n\nrightStick\x18\x11 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12+\n\tleftStick\x18\x10 \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12+\n\x0bleftTrigger\x18\x12 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12,\n\x0crightTrigger\x18\x13 \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1al\n\x0cTaikoOptions\x12\x15\n\rbuttonKatLeft\x18\x01 \x01(\x05\x12\x16\n\x0e\x62uttonKatRight\x18\x02 \x01(\x05\x12\x15\n\rbuttonDonLeft\x18\x03 \x01(\x05\x12\x16\n\x0e\x62uttonDonRight\x18\x04 \x01(\x05\x1a\xad\x02\n\rGuitarOptions\x12\x11\n\tbuttonRed\x18\x01 \x01(\x05\x12\x13\n\x0b\x62uttonGreen\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonYellow\x18\x03 \x01(\x05\x12\x12\n\nbuttonBlue\x18\x04 \x01(\x05\x12\x14\n\x0c\x62uttonOrange\x18\x05 \x01(\x05\x12\x13\n\x0b\x62uttonPedal\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\x0f\n\x07strumUp\x18\t \x01(\x05\x12\x11\n\tstrumDown\x18\n \x01(\x05\x12\'\n\x05stick\x18\x0b \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12)\n\twhammyBar\x18\x0c \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a\xdc\x01\n\x0b\x44rumOptions\x12\x11\n\tbuttonRed\x18\x01 \x01(\x05\x12\x13\n\x0b\x62uttonGreen\x18\x02 \x01(\x05\x12\x14\n\x0c\x62uttonYellow\x18\x03 \x01(\x05\x12\x12\n\nbuttonBlue\x18\x04 \x01(\x05\x12\x14\n\x0c\x62uttonOrange\x18\x05 \x01(\x05\x12\x13\n\x0b\x62uttonPedal\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\'\n\x05stick\x18\t \x01(\x0b\x32\x18.WiiOptions.StickOptions\x1a\xbe\x03\n\x10TurntableOptions\x12\x15\n\rbuttonLeftRed\x18\x01 \x01(\x05\x12\x17\n\x0f\x62uttonLeftGreen\x18\x02 \x01(\x05\x12\x16\n\x0e\x62uttonLeftBlue\x18\x03 \x01(\x05\x12\x16\n\x0e\x62uttonRightRed\x18\x04 \x01(\x05\x12\x18\n\x10\x62uttonRightGreen\x18\x05 \x01(\x05\x12\x17\n\x0f\x62uttonRightBlue\x18\x06 \x01(\x05\x12\x13\n\x0b\x62uttonMinus\x18\x07 \x01(\x05\x12\x12\n\nbuttonPlus\x18\x08 \x01(\x05\x12\x16\n\x0e\x62uttonEuphoria\x18\t \x01(\x05\x12\'\n\x05stick\x18\n \x01(\x0b\x32\x18.WiiOptions.StickOptions\x12-\n\rleftTurntable\x18\x0b \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12.\n\x0erightTurntable\x18\x0c \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12\'\n\x07\x65\x66\x66\x65\x63ts\x18\r \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x12%\n\x05\x66\x61\x64\x65r\x18\x0e \x01(\x0b\x32\x16.WiiOptions.AnalogAxis\x1a\x99\x02\n\x11\x43ontrollerOptions\x12+\n\x07nunchuk\x18\x01 \x01(\x0b\x32\x1a.WiiOptions.NunchukOptions\x12+\n\x07\x63lassic\x18\x02 \x01(\x0b\x32\x1a.WiiOptions.ClassicOptions\x12\'\n\x05taiko\x18\x03 \x01(\x0b\x32\x18.WiiOptions.TaikoOptions\x12)\n\x06guitar\x18\x04 \x01(\x0b\x32\x19.WiiOptions.GuitarOptions\x12%\n\x04\x64rum\x18\x05 \x01(\x0b\x32\x17.WiiOptions.DrumOptions\x12/\n\tturntable\x18\x06 \x01(\x0b\x32\x1c.WiiOptions.TurntableOptions\"S\n\x0bSNESOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08\x63lockPin\x18\x02 \x01(\x05\x12\x10\n\x08latchPin\x18\x03 \x01(\x05\x12\x0f\n\x07\x64\x61taPin\x18\x04 \x01(\x05\"\x86\x01\n\x13KeyboardHostOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\x12\x64\x65precatedPinDplus\x18\x02 \x01(\x05\x42\x02\x18\x01\x12!\n\x07mapping\x18\x03 \x01(\x0b\x32\x10.KeyboardMapping\x12\x1b\n\x0f\x64\x65precatedPin5V\x18\x04 \x01(\x05\x42\x02\x18\x01\"\xae\x01\n\x10\x46ocusModeOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03pin\x18\x02 \x01(\x05\x12\x16\n\x0e\x62uttonLockMask\x18\x03 \x01(\x05\x12\x17\n\x0foledLockEnabled\x18\x04 \x01(\x08\x12\x16\n\x0ergbLockEnabled\x18\x05 \x01(\x08\x12\x19\n\x11\x62uttonLockEnabled\x18\x06 \x01(\x08\x12\x18\n\x10macroLockEnabled\x18\x07 \x01(\x08\"K\n\nMacroInput\x12\x12\n\nbuttonMask\x18\x01 \x01(\r\x12\x10\n\x08\x64uration\x18\x02 \x01(\r\x12\x17\n\x0cwaitDuration\x18\x03 \x01(\r:\x01\x30\"\xae\x02\n\x05Macro\x12\x1d\n\tmacroType\x18\x01 \x01(\x0e\x32\n.MacroType\x12\x19\n\nmacroLabel\x18\x02 \x01(\tB\x05\x92?\x02p@\x12\'\n\x0bmacroInputs\x18\x03 \x03(\x0b\x32\x0b.MacroInputB\x05\x92?\x02\x10\x1e\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\x12\x1d\n\x15useMacroTriggerButton\x18\x05 \x01(\x08\x12%\n\x19\x64\x65precatedMacroTriggerPin\x18\x06 \x01(\x05\x42\x02\x18\x01\x12\x1a\n\x12macroTriggerButton\x18\x07 \x01(\r\x12\x17\n\texclusive\x18\x08 \x01(\x08:\x04true\x12\x1b\n\rinterruptible\x18\t \x01(\x08:\x04true\x12\x19\n\nshowFrames\x18\n \x01(\x08:\x05\x66\x61lse\"z\n\x0cMacroOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x19\n\rdeprecatedPin\x18\x02 \x01(\x05\x42\x02\x18\x01\x12 \n\tmacroList\x18\x03 \x03(\x0b\x32\x06.MacroB\x05\x92?\x02\x10\x06\x12\x1c\n\x14macroBoardLedEnabled\x18\x04 \x01(\x08\"P\n\x13InputHistoryOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06length\x18\x02 \x01(\r\x12\x0b\n\x03\x63ol\x18\x03 \x01(\r\x12\x0b\n\x03row\x18\x04 \x01(\r\"\xc2\x01\n\x10RotaryPinOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04pinA\x18\x02 \x01(\x05\x12\x0c\n\x04pinB\x18\x03 \x01(\x05\x12#\n\x04mode\x18\x04 \x01(\x0e\x32\x15.RotaryEncoderPinMode\x12\x1b\n\x13pulsesPerRevolution\x18\x05 \x01(\r\x12\x12\n\nresetAfter\x18\x06 \x01(\r\x12\x17\n\x0f\x61llowWrapAround\x18\x07 \x01(\x08\x12\x12\n\nmultiplier\x18\x08 \x01(\x02\"n\n\rRotaryOptions\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12%\n\nencoderOne\x18\x02 \x01(\x0b\x32\x11.RotaryPinOptions\x12%\n\nencoderTwo\x18\x03 \x01(\x0b\x32\x11.RotaryPinOptions\"\xe0\x08\n\x0c\x41\x64\x64onOptions\x12\x33\n\x14\x62ootselButtonOptions\x18\x01 \x01(\x0b\x32\x15.BootselButtonOptions\x12-\n\x11onBoardLedOptions\x18\x02 \x01(\x0b\x32\x12.OnBoardLedOptions\x12%\n\ranalogOptions\x18\x03 \x01(\x0b\x32\x0e.AnalogOptions\x12#\n\x0cturboOptions\x18\x04 \x01(\x0b\x32\r.TurboOptions\x12%\n\rsliderOptions\x18\x05 \x01(\x0b\x32\x0e.SliderOptions\x12\'\n\x0ereverseOptions\x18\x06 \x01(\x0b\x32\x0f.ReverseOptions\x12\x33\n\x14\x61nalogADS1219Options\x18\x07 \x01(\x0b\x32\x15.AnalogADS1219Options\x12\x37\n\x16\x64ualDirectionalOptions\x18\x08 \x01(\x0b\x32\x17.DualDirectionalOptions\x12%\n\rbuzzerOptions\x18\t \x01(\x0b\x32\x0e.BuzzerOptions\x12=\n\x1c\x64\x65precatedExtraButtonOptions\x18\n \x01(\x0b\x32\x13.ExtraButtonOptionsB\x02\x18\x01\x12\x31\n\x13playerNumberOptions\x18\x0b \x01(\x0b\x32\x14.PlayerNumberOptions\x12\'\n\nps4Options\x18\x0c \x01(\x0b\x32\x0b.PS4OptionsB\x06\x92?\x03\xf0\x01\x01\x12\x1f\n\nwiiOptions\x18\r \x01(\x0b\x32\x0b.WiiOptions\x12-\n\x11socdSliderOptions\x18\x0e \x01(\x0b\x32\x12.SOCDSliderOptions\x12!\n\x0bsnesOptions\x18\x0f \x01(\x0b\x32\x0c.SNESOptions\x12+\n\x10\x66ocusModeOptions\x18\x10 \x01(\x0b\x32\x11.FocusModeOptions\x12\x31\n\x13keyboardHostOptions\x18\x11 \x01(\x0b\x32\x14.KeyboardHostOptions\x12!\n\x0btiltOptions\x18\x12 \x01(\x0b\x32\x0c.TiltOptions\x12\x37\n\x14psPassthroughOptions\x18\x13 \x01(\x0b\x32\x15.PSPassthroughOptionsB\x02\x18\x01\x12#\n\x0cmacroOptions\x18\x14 \x01(\x0b\x32\r.MacroOptions\x12\x31\n\x13inputHistoryOptions\x18\x15 \x01(\x0b\x32\x14.InputHistoryOptions\x12=\n\x17xbonePassthroughOptions\x18\x16 \x01(\x0b\x32\x18.XBOnePassthroughOptionsB\x02\x18\x01\x12\x33\n\x14\x61nalogADS1256Options\x18\x17 \x01(\x0b\x32\x15.AnalogADS1256Options\x12%\n\rrotaryOptions\x18\x18 \x01(\x0b\x32\x0e.RotaryOptions\"~\n\x10MigrationHistory\x12\x1e\n\x0fhotkeysMigrated\x18\x01 \x01(\x08:\x05\x66\x61lse\x12#\n\x14gpioMappingsMigrated\x18\x02 \x01(\x08:\x05\x66\x61lse\x12%\n\x16\x62uttonProfilesMigrated\x18\x03 \x01(\x08:\x05\x66\x61lse\"\xe4\x04\n\x06\x43onfig\x12\x1b\n\x0c\x62oardVersion\x18\x01 \x01(\tB\x05\x92?\x02p\x1f\x12\'\n\x0egamepadOptions\x18\x02 \x01(\x0b\x32\x0f.GamepadOptions\x12%\n\rhotkeyOptions\x18\x03 \x01(\x0b\x32\x0e.HotkeyOptions\x12/\n\x15\x64\x65precatedPinMappings\x18\x04 \x01(\x0b\x32\x0c.PinMappingsB\x02\x18\x01\x12)\n\x0fkeyboardMapping\x18\x05 \x01(\x0b\x32\x10.KeyboardMapping\x12\'\n\x0e\x64isplayOptions\x18\x06 \x01(\x0b\x32\x0f.DisplayOptions\x12\x1f\n\nledOptions\x18\x07 \x01(\x0b\x32\x0b.LEDOptions\x12\x31\n\x10\x61nimationOptions\x18\x08 \x01(\x0b\x32\x17.AnimationOptions_Proto\x12#\n\x0c\x61\x64\x64onOptions\x18\t \x01(\x0b\x32\r.AddonOptions\x12/\n\x12\x66orcedSetupOptions\x18\n \x01(\x0b\x32\x13.ForcedSetupOptions\x12\'\n\x0eprofileOptions\x18\x0b \x01(\x0b\x32\x0f.ProfileOptions\x12\x1a\n\x0b\x62oardConfig\x18\x0c \x01(\tB\x05\x92?\x02p?\x12#\n\x0cgpioMappings\x18\r \x01(\x0b\x32\r.GpioMappings\x12%\n\nmigrations\x18\x0e \x01(\x0b\x32\x11.MigrationHistory\x12-\n\x11peripheralOptions\x18\x0f \x01(\x0b\x32\x12.PeripheralOptions')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
+  _GAMEPADOPTIONS.fields_by_name['ps4ReportHack']._options = None
+  _GAMEPADOPTIONS.fields_by_name['ps4ReportHack']._serialized_options = b'\030\001'
   _GPIOMAPPINGS.fields_by_name['pins']._options = None
   _GPIOMAPPINGS.fields_by_name['pins']._serialized_options = b'\222?\002\020\036'
   _PROFILEOPTIONS.fields_by_name['deprecatedAlternativePinMappings']._options = None
   _PROFILEOPTIONS.fields_by_name['deprecatedAlternativePinMappings']._serialized_options = b'\030\001\222?\002\020\003'
   _PROFILEOPTIONS.fields_by_name['gpioMappingsSets']._options = None
   _PROFILEOPTIONS.fields_by_name['gpioMappingsSets']._serialized_options = b'\222?\002\020\003'
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSDAPin']._options = None
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSDAPin']._serialized_options = b'\030\001'
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSCLPin']._options = None
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSCLPin']._serialized_options = b'\030\001'
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSpeed']._options = None
   _DISPLAYOPTIONS.fields_by_name['deprecatedI2cSpeed']._serialized_options = b'\030\001'
   _DISPLAYOPTIONS.fields_by_name['splashImage']._options = None
   _DISPLAYOPTIONS.fields_by_name['splashImage']._serialized_options = b'\222?\003\010\200\010'
+  _TURBOOPTIONS.fields_by_name['deprecatedButtonPin']._options = None
+  _TURBOOPTIONS.fields_by_name['deprecatedButtonPin']._serialized_options = b'\030\001'
   _SLIDEROPTIONS.fields_by_name['deprecatedPinSliderOne']._options = None
   _SLIDEROPTIONS.fields_by_name['deprecatedPinSliderOne']._serialized_options = b'\030\001'
   _SLIDEROPTIONS.fields_by_name['deprecatedPinSliderTwo']._options = None
   _SLIDEROPTIONS.fields_by_name['deprecatedPinSliderTwo']._serialized_options = b'\030\001'
   _SLIDEROPTIONS.fields_by_name['deprecatedModeOne']._options = None
   _SLIDEROPTIONS.fields_by_name['deprecatedModeOne']._serialized_options = b'\030\001'
   _SLIDEROPTIONS.fields_by_name['deprecatedModeTwo']._options = None
@@ -86,152 +90,170 @@
   _PS4OPTIONS.fields_by_name['rsaDP']._serialized_options = b'\222?\003\010\200\001'
   _PS4OPTIONS.fields_by_name['rsaDQ']._options = None
   _PS4OPTIONS.fields_by_name['rsaDQ']._serialized_options = b'\222?\003\010\200\001'
   _PS4OPTIONS.fields_by_name['rsaQP']._options = None
   _PS4OPTIONS.fields_by_name['rsaQP']._serialized_options = b'\222?\003\010\200\001'
   _PS4OPTIONS.fields_by_name['rsaRN']._options = None
   _PS4OPTIONS.fields_by_name['rsaRN']._serialized_options = b'\222?\003\010\200\002'
+  _PSPASSTHROUGHOPTIONS.fields_by_name['enabled']._options = None
+  _PSPASSTHROUGHOPTIONS.fields_by_name['enabled']._serialized_options = b'\030\001'
   _PSPASSTHROUGHOPTIONS.fields_by_name['deprecatedPinDplus']._options = None
   _PSPASSTHROUGHOPTIONS.fields_by_name['deprecatedPinDplus']._serialized_options = b'\030\001'
   _PSPASSTHROUGHOPTIONS.fields_by_name['deprecatedPin5V']._options = None
   _PSPASSTHROUGHOPTIONS.fields_by_name['deprecatedPin5V']._serialized_options = b'\030\001'
+  _XBONEPASSTHROUGHOPTIONS.fields_by_name['enabled']._options = None
+  _XBONEPASSTHROUGHOPTIONS.fields_by_name['enabled']._serialized_options = b'\030\001'
   _WIIOPTIONS.fields_by_name['deprecatedI2cSDAPin']._options = None
   _WIIOPTIONS.fields_by_name['deprecatedI2cSDAPin']._serialized_options = b'\030\001'
   _WIIOPTIONS.fields_by_name['deprecatedI2cSCLPin']._options = None
   _WIIOPTIONS.fields_by_name['deprecatedI2cSCLPin']._serialized_options = b'\030\001'
   _WIIOPTIONS.fields_by_name['deprecatedI2cSpeed']._options = None
   _WIIOPTIONS.fields_by_name['deprecatedI2cSpeed']._serialized_options = b'\030\001'
   _KEYBOARDHOSTOPTIONS.fields_by_name['deprecatedPinDplus']._options = None
   _KEYBOARDHOSTOPTIONS.fields_by_name['deprecatedPinDplus']._serialized_options = b'\030\001'
   _KEYBOARDHOSTOPTIONS.fields_by_name['deprecatedPin5V']._options = None
   _KEYBOARDHOSTOPTIONS.fields_by_name['deprecatedPin5V']._serialized_options = b'\030\001'
   _MACRO.fields_by_name['macroLabel']._options = None
   _MACRO.fields_by_name['macroLabel']._serialized_options = b'\222?\002p@'
   _MACRO.fields_by_name['macroInputs']._options = None
   _MACRO.fields_by_name['macroInputs']._serialized_options = b'\222?\002\020\036'
+  _MACRO.fields_by_name['deprecatedMacroTriggerPin']._options = None
+  _MACRO.fields_by_name['deprecatedMacroTriggerPin']._serialized_options = b'\030\001'
+  _MACROOPTIONS.fields_by_name['deprecatedPin']._options = None
+  _MACROOPTIONS.fields_by_name['deprecatedPin']._serialized_options = b'\030\001'
   _MACROOPTIONS.fields_by_name['macroList']._options = None
   _MACROOPTIONS.fields_by_name['macroList']._serialized_options = b'\222?\002\020\006'
   _ADDONOPTIONS.fields_by_name['deprecatedExtraButtonOptions']._options = None
   _ADDONOPTIONS.fields_by_name['deprecatedExtraButtonOptions']._serialized_options = b'\030\001'
   _ADDONOPTIONS.fields_by_name['ps4Options']._options = None
   _ADDONOPTIONS.fields_by_name['ps4Options']._serialized_options = b'\222?\003\360\001\001'
+  _ADDONOPTIONS.fields_by_name['psPassthroughOptions']._options = None
+  _ADDONOPTIONS.fields_by_name['psPassthroughOptions']._serialized_options = b'\030\001'
+  _ADDONOPTIONS.fields_by_name['xbonePassthroughOptions']._options = None
+  _ADDONOPTIONS.fields_by_name['xbonePassthroughOptions']._serialized_options = b'\030\001'
   _CONFIG.fields_by_name['boardVersion']._options = None
   _CONFIG.fields_by_name['boardVersion']._serialized_options = b'\222?\002p\037'
   _CONFIG.fields_by_name['deprecatedPinMappings']._options = None
   _CONFIG.fields_by_name['deprecatedPinMappings']._serialized_options = b'\030\001'
   _CONFIG.fields_by_name['boardConfig']._options = None
   _CONFIG.fields_by_name['boardConfig']._serialized_options = b'\222?\002p?'
   _GAMEPADOPTIONS._serialized_start=44
-  _GAMEPADOPTIONS._serialized_end=546
-  _KEYBOARDMAPPING._serialized_start=549
-  _KEYBOARDMAPPING._serialized_end=943
-  _HOTKEYENTRY._serialized_start=945
-  _HOTKEYENTRY._serialized_end=1046
-  _HOTKEYOPTIONS._serialized_start=1049
-  _HOTKEYOPTIONS._serialized_end=1576
-  _PERIPHERALOPTIONS._serialized_start=1579
-  _PERIPHERALOPTIONS._serialized_end=2076
-  _PERIPHERALOPTIONS_I2COPTIONS._serialized_start=1850
-  _PERIPHERALOPTIONS_I2COPTIONS._serialized_end=1920
-  _PERIPHERALOPTIONS_SPIOPTIONS._serialized_start=1922
-  _PERIPHERALOPTIONS_SPIOPTIONS._serialized_end=2000
-  _PERIPHERALOPTIONS_USBOPTIONS._serialized_start=2002
-  _PERIPHERALOPTIONS_USBOPTIONS._serialized_end=2076
-  _FORCEDSETUPOPTIONS._serialized_start=2078
-  _FORCEDSETUPOPTIONS._serialized_end=2130
-  _BUTTONLAYOUTPARAMSCOMMON._serialized_start=2132
-  _BUTTONLAYOUTPARAMSCOMMON._serialized_end=2235
-  _BUTTONLAYOUTPARAMSLEFT._serialized_start=2237
-  _BUTTONLAYOUTPARAMSLEFT._serialized_end=2335
-  _BUTTONLAYOUTPARAMSRIGHT._serialized_start=2337
-  _BUTTONLAYOUTPARAMSRIGHT._serialized_end=2441
-  _BUTTONLAYOUTCUSTOMOPTIONS._serialized_start=2443
-  _BUTTONLAYOUTCUSTOMOPTIONS._serialized_end=2562
-  _PINMAPPINGS._serialized_start=2565
-  _PINMAPPINGS._serialized_end=2976
-  _GPIOMAPPINGINFO._serialized_start=2978
-  _GPIOMAPPINGINFO._serialized_end=3024
-  _GPIOMAPPINGS._serialized_start=3026
-  _GPIOMAPPINGS._serialized_end=3079
-  _ALTERNATIVEPINMAPPINGS._serialized_start=3082
-  _ALTERNATIVEPINMAPPINGS._serialized_end=3357
-  _PROFILEOPTIONS._serialized_start=3360
-  _PROFILEOPTIONS._serialized_end=3500
-  _DISPLAYOPTIONS._serialized_start=3503
-  _DISPLAYOPTIONS._serialized_end=4045
-  _LEDOPTIONS._serialized_start=4048
-  _LEDOPTIONS._serialized_end=4766
-  _ANIMATIONOPTIONS_PROTO._serialized_start=4769
-  _ANIMATIONOPTIONS_PROTO._serialized_end=5955
-  _BOOTSELBUTTONOPTIONS._serialized_start=5957
-  _BOOTSELBUTTONOPTIONS._serialized_end=6015
-  _ONBOARDLEDOPTIONS._serialized_start=6017
-  _ONBOARDLEDOPTIONS._serialized_end=6084
-  _ANALOGOPTIONS._serialized_start=6087
-  _ANALOGOPTIONS._serialized_end=6440
-  _TURBOOPTIONS._serialized_start=6443
-  _TURBOOPTIONS._serialized_end=6889
-  _SLIDEROPTIONS._serialized_start=6892
-  _SLIDEROPTIONS._serialized_end=7112
-  _SOCDSLIDEROPTIONS._serialized_start=7115
-  _SOCDSLIDEROPTIONS._serialized_end=7327
-  _REVERSEOPTIONS._serialized_start=7330
-  _REVERSEOPTIONS._serialized_end=7477
-  _ANALOGADS1219OPTIONS._serialized_start=7480
-  _ANALOGADS1219OPTIONS._serialized_end=7655
-  _DUALDIRECTIONALOPTIONS._serialized_start=7658
-  _DUALDIRECTIONALOPTIONS._serialized_end=7893
-  _TILTOPTIONS._serialized_start=7896
-  _TILTOPTIONS._serialized_end=8496
-  _BUZZEROPTIONS._serialized_start=8498
-  _BUZZEROPTIONS._serialized_end=8559
-  _EXTRABUTTONOPTIONS._serialized_start=8561
-  _EXTRABUTTONOPTIONS._serialized_end=8630
-  _PLAYERNUMBEROPTIONS._serialized_start=8632
-  _PLAYERNUMBEROPTIONS._serialized_end=8686
-  _PS4OPTIONS._serialized_start=8689
-  _PS4OPTIONS._serialized_end=8969
-  _PSPASSTHROUGHOPTIONS._serialized_start=8971
-  _PSPASSTHROUGHOPTIONS._serialized_end=9071
-  _XBONEPASSTHROUGHOPTIONS._serialized_start=9073
-  _XBONEPASSTHROUGHOPTIONS._serialized_end=9115
-  _WIIOPTIONS._serialized_start=9118
-  _WIIOPTIONS._serialized_end=11411
-  _WIIOPTIONS_ANALOGAXIS._serialized_start=9317
-  _WIIOPTIONS_ANALOGAXIS._serialized_end=9383
-  _WIIOPTIONS_STICKOPTIONS._serialized_start=9385
-  _WIIOPTIONS_STICKOPTIONS._serialized_end=9469
-  _WIIOPTIONS_NUNCHUKOPTIONS._serialized_start=9471
-  _WIIOPTIONS_NUNCHUKOPTIONS._serialized_end=9562
-  _WIIOPTIONS_CLASSICOPTIONS._serialized_start=9565
-  _WIIOPTIONS_CLASSICOPTIONS._serialized_end=10041
-  _WIIOPTIONS_TAIKOOPTIONS._serialized_start=10043
-  _WIIOPTIONS_TAIKOOPTIONS._serialized_end=10151
-  _WIIOPTIONS_GUITAROPTIONS._serialized_start=10154
-  _WIIOPTIONS_GUITAROPTIONS._serialized_end=10455
-  _WIIOPTIONS_DRUMOPTIONS._serialized_start=10458
-  _WIIOPTIONS_DRUMOPTIONS._serialized_end=10678
-  _WIIOPTIONS_TURNTABLEOPTIONS._serialized_start=10681
-  _WIIOPTIONS_TURNTABLEOPTIONS._serialized_end=11127
-  _WIIOPTIONS_CONTROLLEROPTIONS._serialized_start=11130
-  _WIIOPTIONS_CONTROLLEROPTIONS._serialized_end=11411
-  _SNESOPTIONS._serialized_start=11413
-  _SNESOPTIONS._serialized_end=11496
-  _KEYBOARDHOSTOPTIONS._serialized_start=11499
-  _KEYBOARDHOSTOPTIONS._serialized_end=11633
-  _FOCUSMODEOPTIONS._serialized_start=11636
-  _FOCUSMODEOPTIONS._serialized_end=11810
-  _MACROINPUT._serialized_start=11812
-  _MACROINPUT._serialized_end=11887
-  _MACRO._serialized_start=11890
-  _MACRO._serialized_end=12182
-  _MACROOPTIONS._serialized_start=12184
-  _MACROOPTIONS._serialized_end=12292
-  _INPUTHISTORYOPTIONS._serialized_start=12294
-  _INPUTHISTORYOPTIONS._serialized_end=12374
-  _ADDONOPTIONS._serialized_start=12377
-  _ADDONOPTIONS._serialized_end=13397
-  _MIGRATIONHISTORY._serialized_start=13399
-  _MIGRATIONHISTORY._serialized_end=13525
-  _CONFIG._serialized_start=13528
-  _CONFIG._serialized_end=14140
+  _GAMEPADOPTIONS._serialized_end=676
+  _KEYBOARDMAPPING._serialized_start=679
+  _KEYBOARDMAPPING._serialized_end=1073
+  _HOTKEYENTRY._serialized_start=1075
+  _HOTKEYENTRY._serialized_end=1176
+  _HOTKEYOPTIONS._serialized_start=1179
+  _HOTKEYOPTIONS._serialized_end=1706
+  _PERIPHERALOPTIONS._serialized_start=1709
+  _PERIPHERALOPTIONS._serialized_end=2206
+  _PERIPHERALOPTIONS_I2COPTIONS._serialized_start=1980
+  _PERIPHERALOPTIONS_I2COPTIONS._serialized_end=2050
+  _PERIPHERALOPTIONS_SPIOPTIONS._serialized_start=2052
+  _PERIPHERALOPTIONS_SPIOPTIONS._serialized_end=2130
+  _PERIPHERALOPTIONS_USBOPTIONS._serialized_start=2132
+  _PERIPHERALOPTIONS_USBOPTIONS._serialized_end=2206
+  _FORCEDSETUPOPTIONS._serialized_start=2208
+  _FORCEDSETUPOPTIONS._serialized_end=2260
+  _BUTTONLAYOUTPARAMSCOMMON._serialized_start=2262
+  _BUTTONLAYOUTPARAMSCOMMON._serialized_end=2365
+  _BUTTONLAYOUTPARAMSLEFT._serialized_start=2367
+  _BUTTONLAYOUTPARAMSLEFT._serialized_end=2465
+  _BUTTONLAYOUTPARAMSRIGHT._serialized_start=2467
+  _BUTTONLAYOUTPARAMSRIGHT._serialized_end=2571
+  _BUTTONLAYOUTCUSTOMOPTIONS._serialized_start=2573
+  _BUTTONLAYOUTCUSTOMOPTIONS._serialized_end=2692
+  _PINMAPPINGS._serialized_start=2695
+  _PINMAPPINGS._serialized_end=3106
+  _GPIOMAPPINGINFO._serialized_start=3108
+  _GPIOMAPPINGINFO._serialized_end=3154
+  _GPIOMAPPINGS._serialized_start=3156
+  _GPIOMAPPINGS._serialized_end=3209
+  _ALTERNATIVEPINMAPPINGS._serialized_start=3212
+  _ALTERNATIVEPINMAPPINGS._serialized_end=3487
+  _PROFILEOPTIONS._serialized_start=3490
+  _PROFILEOPTIONS._serialized_end=3630
+  _DISPLAYOPTIONS._serialized_start=3633
+  _DISPLAYOPTIONS._serialized_end=4175
+  _LEDOPTIONS._serialized_start=4178
+  _LEDOPTIONS._serialized_end=4896
+  _ANIMATIONOPTIONS_PROTO._serialized_start=4899
+  _ANIMATIONOPTIONS_PROTO._serialized_end=6127
+  _BOOTSELBUTTONOPTIONS._serialized_start=6129
+  _BOOTSELBUTTONOPTIONS._serialized_end=6187
+  _ONBOARDLEDOPTIONS._serialized_start=6189
+  _ONBOARDLEDOPTIONS._serialized_end=6256
+  _ANALOGOPTIONS._serialized_start=6259
+  _ANALOGOPTIONS._serialized_end=6612
+  _TURBOOPTIONS._serialized_start=6615
+  _TURBOOPTIONS._serialized_end=7075
+  _SLIDEROPTIONS._serialized_start=7078
+  _SLIDEROPTIONS._serialized_end=7298
+  _SOCDSLIDEROPTIONS._serialized_start=7301
+  _SOCDSLIDEROPTIONS._serialized_end=7513
+  _REVERSEOPTIONS._serialized_start=7516
+  _REVERSEOPTIONS._serialized_end=7663
+  _ANALOGADS1219OPTIONS._serialized_start=7666
+  _ANALOGADS1219OPTIONS._serialized_end=7841
+  _ANALOGADS1256OPTIONS._serialized_start=7843
+  _ANALOGADS1256OPTIONS._serialized_end=7970
+  _DUALDIRECTIONALOPTIONS._serialized_start=7973
+  _DUALDIRECTIONALOPTIONS._serialized_end=8241
+  _TILTOPTIONS._serialized_start=8244
+  _TILTOPTIONS._serialized_end=8844
+  _BUZZEROPTIONS._serialized_start=8846
+  _BUZZEROPTIONS._serialized_end=8926
+  _EXTRABUTTONOPTIONS._serialized_start=8928
+  _EXTRABUTTONOPTIONS._serialized_end=8997
+  _PLAYERNUMBEROPTIONS._serialized_start=8999
+  _PLAYERNUMBEROPTIONS._serialized_end=9053
+  _PS4OPTIONS._serialized_start=9056
+  _PS4OPTIONS._serialized_end=9336
+  _PSPASSTHROUGHOPTIONS._serialized_start=9338
+  _PSPASSTHROUGHOPTIONS._serialized_end=9442
+  _XBONEPASSTHROUGHOPTIONS._serialized_start=9444
+  _XBONEPASSTHROUGHOPTIONS._serialized_end=9490
+  _WIIOPTIONS._serialized_start=9493
+  _WIIOPTIONS._serialized_end=11786
+  _WIIOPTIONS_ANALOGAXIS._serialized_start=9692
+  _WIIOPTIONS_ANALOGAXIS._serialized_end=9758
+  _WIIOPTIONS_STICKOPTIONS._serialized_start=9760
+  _WIIOPTIONS_STICKOPTIONS._serialized_end=9844
+  _WIIOPTIONS_NUNCHUKOPTIONS._serialized_start=9846
+  _WIIOPTIONS_NUNCHUKOPTIONS._serialized_end=9937
+  _WIIOPTIONS_CLASSICOPTIONS._serialized_start=9940
+  _WIIOPTIONS_CLASSICOPTIONS._serialized_end=10416
+  _WIIOPTIONS_TAIKOOPTIONS._serialized_start=10418
+  _WIIOPTIONS_TAIKOOPTIONS._serialized_end=10526
+  _WIIOPTIONS_GUITAROPTIONS._serialized_start=10529
+  _WIIOPTIONS_GUITAROPTIONS._serialized_end=10830
+  _WIIOPTIONS_DRUMOPTIONS._serialized_start=10833
+  _WIIOPTIONS_DRUMOPTIONS._serialized_end=11053
+  _WIIOPTIONS_TURNTABLEOPTIONS._serialized_start=11056
+  _WIIOPTIONS_TURNTABLEOPTIONS._serialized_end=11502
+  _WIIOPTIONS_CONTROLLEROPTIONS._serialized_start=11505
+  _WIIOPTIONS_CONTROLLEROPTIONS._serialized_end=11786
+  _SNESOPTIONS._serialized_start=11788
+  _SNESOPTIONS._serialized_end=11871
+  _KEYBOARDHOSTOPTIONS._serialized_start=11874
+  _KEYBOARDHOSTOPTIONS._serialized_end=12008
+  _FOCUSMODEOPTIONS._serialized_start=12011
+  _FOCUSMODEOPTIONS._serialized_end=12185
+  _MACROINPUT._serialized_start=12187
+  _MACROINPUT._serialized_end=12262
+  _MACRO._serialized_start=12265
+  _MACRO._serialized_end=12567
+  _MACROOPTIONS._serialized_start=12569
+  _MACROOPTIONS._serialized_end=12691
+  _INPUTHISTORYOPTIONS._serialized_start=12693
+  _INPUTHISTORYOPTIONS._serialized_end=12773
+  _ROTARYPINOPTIONS._serialized_start=12776
+  _ROTARYPINOPTIONS._serialized_end=12970
+  _ROTARYOPTIONS._serialized_start=12972
+  _ROTARYOPTIONS._serialized_end=13082
+  _ADDONOPTIONS._serialized_start=13085
+  _ADDONOPTIONS._serialized_end=14205
+  _MIGRATIONHISTORY._serialized_start=14207
+  _MIGRATIONHISTORY._serialized_end=14333
+  _CONFIG._serialized_start=14336
+  _CONFIG._serialized_end=14948
 # @@protoc_insertion_point(module_scope)
```

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/pb2-files/enums_pb2.py` & `gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/enums_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import nanopb_pb2 as nanopb__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x65nums.proto\x1a\x0cnanopb.proto*\xc3\x03\n\x0c\x42uttonLayout\x12\x17\n\x13\x42UTTON_LAYOUT_STICK\x10\x00\x12\x1b\n\x17\x42UTTON_LAYOUT_STICKLESS\x10\x01\x12 \n\x1c\x42UTTON_LAYOUT_BUTTONS_ANGLED\x10\x02\x12\x1f\n\x1b\x42UTTON_LAYOUT_BUTTONS_BASIC\x10\x03\x12!\n\x1d\x42UTTON_LAYOUT_KEYBOARD_ANGLED\x10\x04\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDA\x10\x05\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADA\x10\x06\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKA\x10\x07\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKA\x10\x08\x12\x16\n\x12\x42UTTON_LAYOUT_VLXA\x10\t\x12\"\n\x1e\x42UTTON_LAYOUT_FIGHTBOARD_STICK\x10\n\x12%\n!BUTTON_LAYOUT_FIGHTBOARD_MIRRORED\x10\x0b\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMA\x10\x0c\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDA\x10\r\x1a\x05\x92?\x02 \x00*\xc2\x04\n\x11\x42uttonLayoutRight\x12\x18\n\x14\x42UTTON_LAYOUT_ARCADE\x10\x00\x12\x1c\n\x18\x42UTTON_LAYOUT_STICKLESSB\x10\x01\x12!\n\x1d\x42UTTON_LAYOUT_BUTTONS_ANGLEDB\x10\x02\x12\x18\n\x14\x42UTTON_LAYOUT_VEWLIX\x10\x03\x12\x19\n\x15\x42UTTON_LAYOUT_VEWLIX7\x10\x04\x12\x18\n\x14\x42UTTON_LAYOUT_CAPCOM\x10\x05\x12\x19\n\x15\x42UTTON_LAYOUT_CAPCOM6\x10\x06\x12\x18\n\x14\x42UTTON_LAYOUT_SEGA2P\x10\x07\x12\x17\n\x13\x42UTTON_LAYOUT_NOIR8\x10\x08\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDB\x10\t\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADB\x10\n\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKB\x10\x0b\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKB\x10\x0c\x12\x16\n\x12\x42UTTON_LAYOUT_VLXB\x10\r\x12\x1c\n\x18\x42UTTON_LAYOUT_FIGHTBOARD\x10\x0e\x12+\n\'BUTTON_LAYOUT_FIGHTBOARD_STICK_MIRRORED\x10\x0f\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMB\x10\x10\x12\x1c\n\x18\x42UTTON_LAYOUT_KEYBOARD8B\x10\x11\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDB\x10\x12\x1a\x05\x92?\x02 \x00*y\n\nSplashMode\x12\x16\n\x12SPLASH_MODE_STATIC\x10\x00\x12\x17\n\x13SPLASH_MODE_CLOSEIN\x10\x01\x12\x1d\n\x19SPLASH_MODE_CLOSEINCUSTOM\x10\x02\x12\x14\n\x10SPLASH_MODE_NONE\x10\x03\x1a\x05\x92?\x02 \x00*\xa0\x01\n\x0cSplashChoice\x12\x16\n\x12SPLASH_CHOICE_MAIN\x10\x00\x12\x13\n\x0fSPLASH_CHOICE_X\x10\x01\x12\x13\n\x0fSPLASH_CHOICE_Y\x10\x02\x12\x13\n\x0fSPLASH_CHOICE_Z\x10\x03\x12\x18\n\x14SPLASH_CHOICE_CUSTOM\x10\x04\x12\x18\n\x14SPLASH_CHOICE_LEGACY\x10\x05\x1a\x05\x92?\x02 \x00*\x99\x01\n\x0eOnBoardLedMode\x12\x19\n\x15ON_BOARD_LED_MODE_OFF\x10\x00\x12$\n ON_BOARD_LED_MODE_MODE_INDICATOR\x10\x01\x12 \n\x1cON_BOARD_LED_MODE_INPUT_TEST\x10\x02\x12\x1d\n\x19ON_BOARD_LED_MODE_PS_AUTH\x10\x03\x1a\x05\x92?\x02 \x00*\xd8\x02\n\tInputMode\x12\x15\n\x11INPUT_MODE_XINPUT\x10\x00\x12\x15\n\x11INPUT_MODE_SWITCH\x10\x01\x12\x12\n\x0eINPUT_MODE_HID\x10\x02\x12\x17\n\x13INPUT_MODE_KEYBOARD\x10\x03\x12\x12\n\x0eINPUT_MODE_PS4\x10\x04\x12\x14\n\x10INPUT_MODE_XBONE\x10\x05\x12\x15\n\x11INPUT_MODE_MDMINI\x10\x06\x12\x15\n\x11INPUT_MODE_NEOGEO\x10\x07\x12\x16\n\x12INPUT_MODE_PCEMINI\x10\x08\x12\x14\n\x10INPUT_MODE_EGRET\x10\t\x12\x14\n\x10INPUT_MODE_ASTRO\x10\n\x12\x18\n\x14INPUT_MODE_PSCLASSIC\x10\x0b\x12\x1b\n\x17INPUT_MODE_XBOXORIGINAL\x10\x0c\x12\x16\n\x11INPUT_MODE_CONFIG\x10\xff\x01\x1a\x05\x92?\x02 \x00*_\n\x08\x44padMode\x12\x15\n\x11\x44PAD_MODE_DIGITAL\x10\x00\x12\x19\n\x15\x44PAD_MODE_LEFT_ANALOG\x10\x01\x12\x1a\n\x16\x44PAD_MODE_RIGHT_ANALOG\x10\x02\x1a\x05\x92?\x02 \x00*O\n\nInvertMode\x12\x0f\n\x0bINVERT_NONE\x10\x00\x12\x0c\n\x08INVERT_X\x10\x01\x12\x0c\n\x08INVERT_Y\x10\x02\x12\r\n\tINVERT_XY\x10\x03\x1a\x05\x92?\x02 \x00*\xa2\x01\n\x08SOCDMode\x12\x19\n\x15SOCD_MODE_UP_PRIORITY\x10\x00\x12\x15\n\x11SOCD_MODE_NEUTRAL\x10\x01\x12#\n\x1fSOCD_MODE_SECOND_INPUT_PRIORITY\x10\x02\x12\"\n\x1eSOCD_MODE_FIRST_INPUT_PRIORITY\x10\x03\x12\x14\n\x10SOCD_MODE_BYPASS\x10\x04\x1a\x05\x92?\x02 \x00*\xbc\x06\n\nGpioAction\x12\x11\n\x04NONE\x10\xf6\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x08RESERVED\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x41SSIGNED_TO_ADDON\x10\x00\x12\x13\n\x0f\x42UTTON_PRESS_UP\x10\x01\x12\x15\n\x11\x42UTTON_PRESS_DOWN\x10\x02\x12\x15\n\x11\x42UTTON_PRESS_LEFT\x10\x03\x12\x16\n\x12\x42UTTON_PRESS_RIGHT\x10\x04\x12\x13\n\x0f\x42UTTON_PRESS_B1\x10\x05\x12\x13\n\x0f\x42UTTON_PRESS_B2\x10\x06\x12\x13\n\x0f\x42UTTON_PRESS_B3\x10\x07\x12\x13\n\x0f\x42UTTON_PRESS_B4\x10\x08\x12\x13\n\x0f\x42UTTON_PRESS_L1\x10\t\x12\x13\n\x0f\x42UTTON_PRESS_R1\x10\n\x12\x13\n\x0f\x42UTTON_PRESS_L2\x10\x0b\x12\x13\n\x0f\x42UTTON_PRESS_R2\x10\x0c\x12\x13\n\x0f\x42UTTON_PRESS_S1\x10\r\x12\x13\n\x0f\x42UTTON_PRESS_S2\x10\x0e\x12\x13\n\x0f\x42UTTON_PRESS_A1\x10\x0f\x12\x13\n\x0f\x42UTTON_PRESS_A2\x10\x10\x12\x13\n\x0f\x42UTTON_PRESS_L3\x10\x11\x12\x13\n\x0f\x42UTTON_PRESS_R3\x10\x12\x12\x13\n\x0f\x42UTTON_PRESS_FN\x10\x13\x12\x17\n\x13\x42UTTON_PRESS_DDI_UP\x10\x14\x12\x19\n\x15\x42UTTON_PRESS_DDI_DOWN\x10\x15\x12\x19\n\x15\x42UTTON_PRESS_DDI_LEFT\x10\x16\x12\x1a\n\x16\x42UTTON_PRESS_DDI_RIGHT\x10\x17\x12\x16\n\x12SUSTAIN_DP_MODE_DP\x10\x18\x12\x16\n\x12SUSTAIN_DP_MODE_LS\x10\x19\x12\x16\n\x12SUSTAIN_DP_MODE_RS\x10\x1a\x12\x1d\n\x19SUSTAIN_SOCD_MODE_UP_PRIO\x10\x1b\x12\x1d\n\x19SUSTAIN_SOCD_MODE_NEUTRAL\x10\x1c\x12 \n\x1cSUSTAIN_SOCD_MODE_SECOND_WIN\x10\x1d\x12\x1f\n\x1bSUSTAIN_SOCD_MODE_FIRST_WIN\x10\x1e\x12\x1c\n\x18SUSTAIN_SOCD_MODE_BYPASS\x10\x1f\x1a\x05\x92?\x02 \x00*\x80\x07\n\rGamepadHotkey\x12\x0f\n\x0bHOTKEY_NONE\x10\x00\x12\x17\n\x13HOTKEY_DPAD_DIGITAL\x10\x01\x12\x1b\n\x17HOTKEY_DPAD_LEFT_ANALOG\x10\x02\x12\x1c\n\x18HOTKEY_DPAD_RIGHT_ANALOG\x10\x03\x12\x16\n\x12HOTKEY_HOME_BUTTON\x10\x04\x12\x19\n\x15HOTKEY_CAPTURE_BUTTON\x10\x05\x12\x1b\n\x17HOTKEY_SOCD_UP_PRIORITY\x10\x06\x12\x17\n\x13HOTKEY_SOCD_NEUTRAL\x10\x07\x12\x1a\n\x16HOTKEY_SOCD_LAST_INPUT\x10\x08\x12\x18\n\x14HOTKEY_INVERT_X_AXIS\x10\t\x12\x18\n\x14HOTKEY_INVERT_Y_AXIS\x10\n\x12\x1b\n\x17HOTKEY_SOCD_FIRST_INPUT\x10\x0b\x12\x16\n\x12HOTKEY_SOCD_BYPASS\x10\x0c\x12\x1c\n\x18HOTKEY_TOGGLE_4_WAY_MODE\x10\r\x12 \n\x1cHOTKEY_TOGGLE_DDI_4_WAY_MODE\x10\x0e\x12\x19\n\x15HOTKEY_LOAD_PROFILE_1\x10\x0f\x12\x19\n\x15HOTKEY_LOAD_PROFILE_2\x10\x10\x12\x19\n\x15HOTKEY_LOAD_PROFILE_3\x10\x11\x12\x19\n\x15HOTKEY_LOAD_PROFILE_4\x10\x12\x12\x14\n\x10HOTKEY_L3_BUTTON\x10\x13\x12\x14\n\x10HOTKEY_R3_BUTTON\x10\x14\x12\x1a\n\x16HOTKEY_TOUCHPAD_BUTTON\x10\x15\x12\x19\n\x15HOTKEY_REBOOT_DEFAULT\x10\x16\x12\x14\n\x10HOTKEY_B1_BUTTON\x10\x17\x12\x14\n\x10HOTKEY_B2_BUTTON\x10\x18\x12\x14\n\x10HOTKEY_B3_BUTTON\x10\x19\x12\x14\n\x10HOTKEY_B4_BUTTON\x10\x1a\x12\x14\n\x10HOTKEY_L1_BUTTON\x10\x1b\x12\x14\n\x10HOTKEY_R1_BUTTON\x10\x1c\x12\x14\n\x10HOTKEY_L2_BUTTON\x10\x1d\x12\x14\n\x10HOTKEY_R2_BUTTON\x10\x1e\x12\x14\n\x10HOTKEY_S1_BUTTON\x10\x1f\x12\x14\n\x10HOTKEY_S2_BUTTON\x10 \x12\x14\n\x10HOTKEY_A1_BUTTON\x10!\x12\x14\n\x10HOTKEY_A2_BUTTON\x10\"\x1a\x05\x92?\x02 \x00*c\n\x0fLEDFormat_Proto\x12\x12\n\x0eLED_FORMAT_GRB\x10\x00\x12\x12\n\x0eLED_FORMAT_RGB\x10\x01\x12\x13\n\x0fLED_FORMAT_GRBW\x10\x02\x12\x13\n\x0fLED_FORMAT_RGBW\x10\x03*\\\n\x0cShmupMixMode\x12!\n\x1dSHMUP_MIX_MODE_TURBO_PRIORITY\x10\x00\x12\"\n\x1eSHMUP_MIX_MODE_CHARGE_PRIORITY\x10\x01\x1a\x05\x92?\x02 \x00*T\n\x08PLEDType\x12\x1b\n\x0ePLED_TYPE_NONE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x11\n\rPLED_TYPE_PWM\x10\x00\x12\x11\n\rPLED_TYPE_RGB\x10\x01\x1a\x05\x92?\x02 \x00*\xa3\x01\n\x0f\x46orcedSetupMode\x12\x19\n\x15\x46ORCED_SETUP_MODE_OFF\x10\x00\x12&\n\"FORCED_SETUP_MODE_LOCK_MODE_SWITCH\x10\x01\x12%\n!FORCED_SETUP_MODE_LOCK_WEB_CONFIG\x10\x02\x12\x1f\n\x1b\x46ORCED_SETUP_MODE_LOCK_BOTH\x10\x03\x1a\x05\x92?\x02 \x00*C\n\x11PS4ControllerType\x12\x12\n\x0ePS4_CONTROLLER\x10\x00\x12\x13\n\x0fPS4_ARCADESTICK\x10\x07\x1a\x05\x92?\x02 \x00*C\n\tMacroType\x12\x0c\n\x08ON_PRESS\x10\x01\x12\x12\n\x0eON_HOLD_REPEAT\x10\x02\x12\r\n\tON_TOGGLE\x10\x03\x1a\x05\x92?\x02 \x00')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x65nums.proto\x1a\x0cnanopb.proto*\x8d\x07\n\x0c\x42uttonLayout\x12\x17\n\x13\x42UTTON_LAYOUT_STICK\x10\x00\x12\x1b\n\x17\x42UTTON_LAYOUT_STICKLESS\x10\x01\x12 \n\x1c\x42UTTON_LAYOUT_BUTTONS_ANGLED\x10\x02\x12\x1f\n\x1b\x42UTTON_LAYOUT_BUTTONS_BASIC\x10\x03\x12!\n\x1d\x42UTTON_LAYOUT_KEYBOARD_ANGLED\x10\x04\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDA\x10\x05\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADA\x10\x06\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKA\x10\x07\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKA\x10\x08\x12\x16\n\x12\x42UTTON_LAYOUT_VLXA\x10\t\x12\"\n\x1e\x42UTTON_LAYOUT_FIGHTBOARD_STICK\x10\n\x12%\n!BUTTON_LAYOUT_FIGHTBOARD_MIRRORED\x10\x0b\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMA\x10\x0c\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDA\x10\r\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_13\x10\x0e\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_16\x10\x0f\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_14\x10\x10\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_LEFT\x10\x11\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_SOLO\x10\x12\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_PIU_LEFT\x10\x13\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_A\x10\x14\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_A\x10\x15\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_A\x10\x16\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_A\x10\x17\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_A\x10\x18\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_A\x10\x19\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_A\x10\x1a\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_A\x10\x1b\x1a\x05\x92?\x02 \x00*\xec\x07\n\x11\x42uttonLayoutRight\x12\x18\n\x14\x42UTTON_LAYOUT_ARCADE\x10\x00\x12\x1c\n\x18\x42UTTON_LAYOUT_STICKLESSB\x10\x01\x12!\n\x1d\x42UTTON_LAYOUT_BUTTONS_ANGLEDB\x10\x02\x12\x18\n\x14\x42UTTON_LAYOUT_VEWLIX\x10\x03\x12\x19\n\x15\x42UTTON_LAYOUT_VEWLIX7\x10\x04\x12\x18\n\x14\x42UTTON_LAYOUT_CAPCOM\x10\x05\x12\x19\n\x15\x42UTTON_LAYOUT_CAPCOM6\x10\x06\x12\x18\n\x14\x42UTTON_LAYOUT_SEGA2P\x10\x07\x12\x17\n\x13\x42UTTON_LAYOUT_NOIR8\x10\x08\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDB\x10\t\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADB\x10\n\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKB\x10\x0b\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKB\x10\x0c\x12\x16\n\x12\x42UTTON_LAYOUT_VLXB\x10\r\x12\x1c\n\x18\x42UTTON_LAYOUT_FIGHTBOARD\x10\x0e\x12+\n\'BUTTON_LAYOUT_FIGHTBOARD_STICK_MIRRORED\x10\x0f\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMB\x10\x10\x12\x1c\n\x18\x42UTTON_LAYOUT_KEYBOARD8B\x10\x11\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDB\x10\x12\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_13B\x10\x13\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_16B\x10\x14\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_14B\x10\x15\x12$\n BUTTON_LAYOUT_DANCEPAD_DDR_RIGHT\x10\x16\x12$\n BUTTON_LAYOUT_DANCEPAD_PIU_RIGHT\x10\x17\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_B\x10\x18\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_B\x10\x19\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_B\x10\x1a\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_B\x10\x1b\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_B\x10\x1c\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_B\x10\x1d\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_B\x10\x1e\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_B\x10\x1f\x1a\x05\x92?\x02 \x00*y\n\nSplashMode\x12\x16\n\x12SPLASH_MODE_STATIC\x10\x00\x12\x17\n\x13SPLASH_MODE_CLOSEIN\x10\x01\x12\x1d\n\x19SPLASH_MODE_CLOSEINCUSTOM\x10\x02\x12\x14\n\x10SPLASH_MODE_NONE\x10\x03\x1a\x05\x92?\x02 \x00*\xa0\x01\n\x0cSplashChoice\x12\x16\n\x12SPLASH_CHOICE_MAIN\x10\x00\x12\x13\n\x0fSPLASH_CHOICE_X\x10\x01\x12\x13\n\x0fSPLASH_CHOICE_Y\x10\x02\x12\x13\n\x0fSPLASH_CHOICE_Z\x10\x03\x12\x18\n\x14SPLASH_CHOICE_CUSTOM\x10\x04\x12\x18\n\x14SPLASH_CHOICE_LEGACY\x10\x05\x1a\x05\x92?\x02 \x00*\x99\x01\n\x0eOnBoardLedMode\x12\x19\n\x15ON_BOARD_LED_MODE_OFF\x10\x00\x12$\n ON_BOARD_LED_MODE_MODE_INDICATOR\x10\x01\x12 \n\x1cON_BOARD_LED_MODE_INPUT_TEST\x10\x02\x12\x1d\n\x19ON_BOARD_LED_MODE_PS_AUTH\x10\x03\x1a\x05\x92?\x02 \x00*\xec\x02\n\tInputMode\x12\x15\n\x11INPUT_MODE_XINPUT\x10\x00\x12\x15\n\x11INPUT_MODE_SWITCH\x10\x01\x12\x12\n\x0eINPUT_MODE_HID\x10\x02\x12\x17\n\x13INPUT_MODE_KEYBOARD\x10\x03\x12\x12\n\x0eINPUT_MODE_PS4\x10\x04\x12\x14\n\x10INPUT_MODE_XBONE\x10\x05\x12\x15\n\x11INPUT_MODE_MDMINI\x10\x06\x12\x15\n\x11INPUT_MODE_NEOGEO\x10\x07\x12\x16\n\x12INPUT_MODE_PCEMINI\x10\x08\x12\x14\n\x10INPUT_MODE_EGRET\x10\t\x12\x14\n\x10INPUT_MODE_ASTRO\x10\n\x12\x18\n\x14INPUT_MODE_PSCLASSIC\x10\x0b\x12\x1b\n\x17INPUT_MODE_XBOXORIGINAL\x10\x0c\x12\x12\n\x0eINPUT_MODE_PS5\x10\r\x12\x16\n\x11INPUT_MODE_CONFIG\x10\xff\x01\x1a\x05\x92?\x02 \x00*\x94\x01\n\x11InputModeAuthType\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_NONE\x10\x00\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_KEYS\x10\x01\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_USB\x10\x02\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_I2C\x10\x03\x1a\x05\x92?\x02 \x00*_\n\x08\x44padMode\x12\x15\n\x11\x44PAD_MODE_DIGITAL\x10\x00\x12\x19\n\x15\x44PAD_MODE_LEFT_ANALOG\x10\x01\x12\x1a\n\x16\x44PAD_MODE_RIGHT_ANALOG\x10\x02\x1a\x05\x92?\x02 \x00*O\n\nInvertMode\x12\x0f\n\x0bINVERT_NONE\x10\x00\x12\x0c\n\x08INVERT_X\x10\x01\x12\x0c\n\x08INVERT_Y\x10\x02\x12\r\n\tINVERT_XY\x10\x03\x1a\x05\x92?\x02 \x00*\xa2\x01\n\x08SOCDMode\x12\x19\n\x15SOCD_MODE_UP_PRIORITY\x10\x00\x12\x15\n\x11SOCD_MODE_NEUTRAL\x10\x01\x12#\n\x1fSOCD_MODE_SECOND_INPUT_PRIORITY\x10\x02\x12\"\n\x1eSOCD_MODE_FIRST_INPUT_PRIORITY\x10\x03\x12\x14\n\x10SOCD_MODE_BYPASS\x10\x04\x1a\x05\x92?\x02 \x00*\x88\x08\n\nGpioAction\x12\x11\n\x04NONE\x10\xf6\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x08RESERVED\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x41SSIGNED_TO_ADDON\x10\x00\x12\x13\n\x0f\x42UTTON_PRESS_UP\x10\x01\x12\x15\n\x11\x42UTTON_PRESS_DOWN\x10\x02\x12\x15\n\x11\x42UTTON_PRESS_LEFT\x10\x03\x12\x16\n\x12\x42UTTON_PRESS_RIGHT\x10\x04\x12\x13\n\x0f\x42UTTON_PRESS_B1\x10\x05\x12\x13\n\x0f\x42UTTON_PRESS_B2\x10\x06\x12\x13\n\x0f\x42UTTON_PRESS_B3\x10\x07\x12\x13\n\x0f\x42UTTON_PRESS_B4\x10\x08\x12\x13\n\x0f\x42UTTON_PRESS_L1\x10\t\x12\x13\n\x0f\x42UTTON_PRESS_R1\x10\n\x12\x13\n\x0f\x42UTTON_PRESS_L2\x10\x0b\x12\x13\n\x0f\x42UTTON_PRESS_R2\x10\x0c\x12\x13\n\x0f\x42UTTON_PRESS_S1\x10\r\x12\x13\n\x0f\x42UTTON_PRESS_S2\x10\x0e\x12\x13\n\x0f\x42UTTON_PRESS_A1\x10\x0f\x12\x13\n\x0f\x42UTTON_PRESS_A2\x10\x10\x12\x13\n\x0f\x42UTTON_PRESS_L3\x10\x11\x12\x13\n\x0f\x42UTTON_PRESS_R3\x10\x12\x12\x13\n\x0f\x42UTTON_PRESS_FN\x10\x13\x12\x17\n\x13\x42UTTON_PRESS_DDI_UP\x10\x14\x12\x19\n\x15\x42UTTON_PRESS_DDI_DOWN\x10\x15\x12\x19\n\x15\x42UTTON_PRESS_DDI_LEFT\x10\x16\x12\x1a\n\x16\x42UTTON_PRESS_DDI_RIGHT\x10\x17\x12\x16\n\x12SUSTAIN_DP_MODE_DP\x10\x18\x12\x16\n\x12SUSTAIN_DP_MODE_LS\x10\x19\x12\x16\n\x12SUSTAIN_DP_MODE_RS\x10\x1a\x12\x1d\n\x19SUSTAIN_SOCD_MODE_UP_PRIO\x10\x1b\x12\x1d\n\x19SUSTAIN_SOCD_MODE_NEUTRAL\x10\x1c\x12 \n\x1cSUSTAIN_SOCD_MODE_SECOND_WIN\x10\x1d\x12\x1f\n\x1bSUSTAIN_SOCD_MODE_FIRST_WIN\x10\x1e\x12\x1c\n\x18SUSTAIN_SOCD_MODE_BYPASS\x10\x1f\x12\x16\n\x12\x42UTTON_PRESS_TURBO\x10 \x12\x16\n\x12\x42UTTON_PRESS_MACRO\x10!\x12\x18\n\x14\x42UTTON_PRESS_MACRO_1\x10\"\x12\x18\n\x14\x42UTTON_PRESS_MACRO_2\x10#\x12\x18\n\x14\x42UTTON_PRESS_MACRO_3\x10$\x12\x18\n\x14\x42UTTON_PRESS_MACRO_4\x10%\x12\x18\n\x14\x42UTTON_PRESS_MACRO_5\x10&\x12\x18\n\x14\x42UTTON_PRESS_MACRO_6\x10\'\x1a\x05\x92?\x02 \x00*\x80\x07\n\rGamepadHotkey\x12\x0f\n\x0bHOTKEY_NONE\x10\x00\x12\x17\n\x13HOTKEY_DPAD_DIGITAL\x10\x01\x12\x1b\n\x17HOTKEY_DPAD_LEFT_ANALOG\x10\x02\x12\x1c\n\x18HOTKEY_DPAD_RIGHT_ANALOG\x10\x03\x12\x16\n\x12HOTKEY_HOME_BUTTON\x10\x04\x12\x19\n\x15HOTKEY_CAPTURE_BUTTON\x10\x05\x12\x1b\n\x17HOTKEY_SOCD_UP_PRIORITY\x10\x06\x12\x17\n\x13HOTKEY_SOCD_NEUTRAL\x10\x07\x12\x1a\n\x16HOTKEY_SOCD_LAST_INPUT\x10\x08\x12\x18\n\x14HOTKEY_INVERT_X_AXIS\x10\t\x12\x18\n\x14HOTKEY_INVERT_Y_AXIS\x10\n\x12\x1b\n\x17HOTKEY_SOCD_FIRST_INPUT\x10\x0b\x12\x16\n\x12HOTKEY_SOCD_BYPASS\x10\x0c\x12\x1c\n\x18HOTKEY_TOGGLE_4_WAY_MODE\x10\r\x12 \n\x1cHOTKEY_TOGGLE_DDI_4_WAY_MODE\x10\x0e\x12\x19\n\x15HOTKEY_LOAD_PROFILE_1\x10\x0f\x12\x19\n\x15HOTKEY_LOAD_PROFILE_2\x10\x10\x12\x19\n\x15HOTKEY_LOAD_PROFILE_3\x10\x11\x12\x19\n\x15HOTKEY_LOAD_PROFILE_4\x10\x12\x12\x14\n\x10HOTKEY_L3_BUTTON\x10\x13\x12\x14\n\x10HOTKEY_R3_BUTTON\x10\x14\x12\x1a\n\x16HOTKEY_TOUCHPAD_BUTTON\x10\x15\x12\x19\n\x15HOTKEY_REBOOT_DEFAULT\x10\x16\x12\x14\n\x10HOTKEY_B1_BUTTON\x10\x17\x12\x14\n\x10HOTKEY_B2_BUTTON\x10\x18\x12\x14\n\x10HOTKEY_B3_BUTTON\x10\x19\x12\x14\n\x10HOTKEY_B4_BUTTON\x10\x1a\x12\x14\n\x10HOTKEY_L1_BUTTON\x10\x1b\x12\x14\n\x10HOTKEY_R1_BUTTON\x10\x1c\x12\x14\n\x10HOTKEY_L2_BUTTON\x10\x1d\x12\x14\n\x10HOTKEY_R2_BUTTON\x10\x1e\x12\x14\n\x10HOTKEY_S1_BUTTON\x10\x1f\x12\x14\n\x10HOTKEY_S2_BUTTON\x10 \x12\x14\n\x10HOTKEY_A1_BUTTON\x10!\x12\x14\n\x10HOTKEY_A2_BUTTON\x10\"\x1a\x05\x92?\x02 \x00*c\n\x0fLEDFormat_Proto\x12\x12\n\x0eLED_FORMAT_GRB\x10\x00\x12\x12\n\x0eLED_FORMAT_RGB\x10\x01\x12\x13\n\x0fLED_FORMAT_GRBW\x10\x02\x12\x13\n\x0fLED_FORMAT_RGBW\x10\x03*\\\n\x0cShmupMixMode\x12!\n\x1dSHMUP_MIX_MODE_TURBO_PRIORITY\x10\x00\x12\"\n\x1eSHMUP_MIX_MODE_CHARGE_PRIORITY\x10\x01\x1a\x05\x92?\x02 \x00*T\n\x08PLEDType\x12\x1b\n\x0ePLED_TYPE_NONE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x11\n\rPLED_TYPE_PWM\x10\x00\x12\x11\n\rPLED_TYPE_RGB\x10\x01\x1a\x05\x92?\x02 \x00*\xa3\x01\n\x0f\x46orcedSetupMode\x12\x19\n\x15\x46ORCED_SETUP_MODE_OFF\x10\x00\x12&\n\"FORCED_SETUP_MODE_LOCK_MODE_SWITCH\x10\x01\x12%\n!FORCED_SETUP_MODE_LOCK_WEB_CONFIG\x10\x02\x12\x1f\n\x1b\x46ORCED_SETUP_MODE_LOCK_BOTH\x10\x03\x1a\x05\x92?\x02 \x00*g\n\x1e\x44ualDirectionalCombinationMode\x12\x0e\n\nMIXED_MODE\x10\x00\x12\x10\n\x0cGAMEPAD_MODE\x10\x01\x12\r\n\tDUAL_MODE\x10\x02\x12\r\n\tNONE_MODE\x10\x03\x1a\x05\x92?\x02 \x00*C\n\x11PS4ControllerType\x12\x12\n\x0ePS4_CONTROLLER\x10\x00\x12\x13\n\x0fPS4_ARCADESTICK\x10\x07\x1a\x05\x92?\x02 \x00*C\n\tMacroType\x12\x0c\n\x08ON_PRESS\x10\x01\x12\x12\n\x0eON_HOLD_REPEAT\x10\x02\x12\r\n\tON_TOGGLE\x10\x03\x1a\x05\x92?\x02 \x00*\xea\x01\n\tGPElement\x12\x15\n\x11GP_ELEMENT_WIDGET\x10\x00\x12\x15\n\x11GP_ELEMENT_SCREEN\x10\x01\x12\x19\n\x15GP_ELEMENT_BTN_BUTTON\x10\x02\x12\x19\n\x15GP_ELEMENT_DIR_BUTTON\x10\x03\x12\x19\n\x15GP_ELEMENT_PIN_BUTTON\x10\x04\x12\x14\n\x10GP_ELEMENT_LEVER\x10\x05\x12\x14\n\x10GP_ELEMENT_LABEL\x10\x06\x12\x15\n\x11GP_ELEMENT_SPRITE\x10\x07\x12\x14\n\x10GP_ELEMENT_SHAPE\x10\x08\x1a\x05\x92?\x02 \x00*~\n\x0cGPShape_Type\x12\x14\n\x10GP_SHAPE_ELLIPSE\x10\x00\x12\x13\n\x0fGP_SHAPE_SQUARE\x10\x01\x12\x14\n\x10GP_SHAPE_DIAMOND\x10\x02\x12\x14\n\x10GP_SHAPE_POLYGON\x10\x03\x12\x10\n\x0cGP_SHAPE_ARC\x10\x04\x1a\x05\x92?\x02 \x00*\xa7\x02\n\x14RotaryEncoderPinMode\x12\x15\n\x11\x45NCODER_MODE_NONE\x10\x00\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_X\x10\x01\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_Y\x10\x02\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_X\x10\x03\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_Y\x10\x04\x12\x1d\n\x19\x45NCODER_MODE_LEFT_TRIGGER\x10\x05\x12\x1e\n\x1a\x45NCODER_MODE_RIGHT_TRIGGER\x10\x06\x12\x17\n\x13\x45NCODER_MODE_DPAD_X\x10\x07\x12\x17\n\x13\x45NCODER_MODE_DPAD_Y\x10\x08\x1a\x05\x92?\x02 \x00')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'enums_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _BUTTONLAYOUT._options = None
@@ -29,14 +29,16 @@
   _SPLASHMODE._serialized_options = b'\222?\002 \000'
   _SPLASHCHOICE._options = None
   _SPLASHCHOICE._serialized_options = b'\222?\002 \000'
   _ONBOARDLEDMODE._options = None
   _ONBOARDLEDMODE._serialized_options = b'\222?\002 \000'
   _INPUTMODE._options = None
   _INPUTMODE._serialized_options = b'\222?\002 \000'
+  _INPUTMODEAUTHTYPE._options = None
+  _INPUTMODEAUTHTYPE._serialized_options = b'\222?\002 \000'
   _DPADMODE._options = None
   _DPADMODE._serialized_options = b'\222?\002 \000'
   _INVERTMODE._options = None
   _INVERTMODE._serialized_options = b'\222?\002 \000'
   _SOCDMODE._options = None
   _SOCDMODE._serialized_options = b'\222?\002 \000'
   _GPIOACTION._options = None
@@ -45,46 +47,64 @@
   _GAMEPADHOTKEY._serialized_options = b'\222?\002 \000'
   _SHMUPMIXMODE._options = None
   _SHMUPMIXMODE._serialized_options = b'\222?\002 \000'
   _PLEDTYPE._options = None
   _PLEDTYPE._serialized_options = b'\222?\002 \000'
   _FORCEDSETUPMODE._options = None
   _FORCEDSETUPMODE._serialized_options = b'\222?\002 \000'
+  _DUALDIRECTIONALCOMBINATIONMODE._options = None
+  _DUALDIRECTIONALCOMBINATIONMODE._serialized_options = b'\222?\002 \000'
   _PS4CONTROLLERTYPE._options = None
   _PS4CONTROLLERTYPE._serialized_options = b'\222?\002 \000'
   _MACROTYPE._options = None
   _MACROTYPE._serialized_options = b'\222?\002 \000'
+  _GPELEMENT._options = None
+  _GPELEMENT._serialized_options = b'\222?\002 \000'
+  _GPSHAPE_TYPE._options = None
+  _GPSHAPE_TYPE._serialized_options = b'\222?\002 \000'
+  _ROTARYENCODERPINMODE._options = None
+  _ROTARYENCODERPINMODE._serialized_options = b'\222?\002 \000'
   _BUTTONLAYOUT._serialized_start=30
-  _BUTTONLAYOUT._serialized_end=481
-  _BUTTONLAYOUTRIGHT._serialized_start=484
-  _BUTTONLAYOUTRIGHT._serialized_end=1062
-  _SPLASHMODE._serialized_start=1064
-  _SPLASHMODE._serialized_end=1185
-  _SPLASHCHOICE._serialized_start=1188
-  _SPLASHCHOICE._serialized_end=1348
-  _ONBOARDLEDMODE._serialized_start=1351
-  _ONBOARDLEDMODE._serialized_end=1504
-  _INPUTMODE._serialized_start=1507
-  _INPUTMODE._serialized_end=1851
-  _DPADMODE._serialized_start=1853
-  _DPADMODE._serialized_end=1948
-  _INVERTMODE._serialized_start=1950
-  _INVERTMODE._serialized_end=2029
-  _SOCDMODE._serialized_start=2032
-  _SOCDMODE._serialized_end=2194
-  _GPIOACTION._serialized_start=2197
-  _GPIOACTION._serialized_end=3025
-  _GAMEPADHOTKEY._serialized_start=3028
-  _GAMEPADHOTKEY._serialized_end=3924
-  _LEDFORMAT_PROTO._serialized_start=3926
-  _LEDFORMAT_PROTO._serialized_end=4025
-  _SHMUPMIXMODE._serialized_start=4027
-  _SHMUPMIXMODE._serialized_end=4119
-  _PLEDTYPE._serialized_start=4121
-  _PLEDTYPE._serialized_end=4205
-  _FORCEDSETUPMODE._serialized_start=4208
-  _FORCEDSETUPMODE._serialized_end=4371
-  _PS4CONTROLLERTYPE._serialized_start=4373
-  _PS4CONTROLLERTYPE._serialized_end=4440
-  _MACROTYPE._serialized_start=4442
-  _MACROTYPE._serialized_end=4509
+  _BUTTONLAYOUT._serialized_end=939
+  _BUTTONLAYOUTRIGHT._serialized_start=942
+  _BUTTONLAYOUTRIGHT._serialized_end=1946
+  _SPLASHMODE._serialized_start=1948
+  _SPLASHMODE._serialized_end=2069
+  _SPLASHCHOICE._serialized_start=2072
+  _SPLASHCHOICE._serialized_end=2232
+  _ONBOARDLEDMODE._serialized_start=2235
+  _ONBOARDLEDMODE._serialized_end=2388
+  _INPUTMODE._serialized_start=2391
+  _INPUTMODE._serialized_end=2755
+  _INPUTMODEAUTHTYPE._serialized_start=2758
+  _INPUTMODEAUTHTYPE._serialized_end=2906
+  _DPADMODE._serialized_start=2908
+  _DPADMODE._serialized_end=3003
+  _INVERTMODE._serialized_start=3005
+  _INVERTMODE._serialized_end=3084
+  _SOCDMODE._serialized_start=3087
+  _SOCDMODE._serialized_end=3249
+  _GPIOACTION._serialized_start=3252
+  _GPIOACTION._serialized_end=4284
+  _GAMEPADHOTKEY._serialized_start=4287
+  _GAMEPADHOTKEY._serialized_end=5183
+  _LEDFORMAT_PROTO._serialized_start=5185
+  _LEDFORMAT_PROTO._serialized_end=5284
+  _SHMUPMIXMODE._serialized_start=5286
+  _SHMUPMIXMODE._serialized_end=5378
+  _PLEDTYPE._serialized_start=5380
+  _PLEDTYPE._serialized_end=5464
+  _FORCEDSETUPMODE._serialized_start=5467
+  _FORCEDSETUPMODE._serialized_end=5630
+  _DUALDIRECTIONALCOMBINATIONMODE._serialized_start=5632
+  _DUALDIRECTIONALCOMBINATIONMODE._serialized_end=5735
+  _PS4CONTROLLERTYPE._serialized_start=5737
+  _PS4CONTROLLERTYPE._serialized_end=5804
+  _MACROTYPE._serialized_start=5806
+  _MACROTYPE._serialized_end=5873
+  _GPELEMENT._serialized_start=5876
+  _GPELEMENT._serialized_end=6110
+  _GPSHAPE_TYPE._serialized_start=6112
+  _GPSHAPE_TYPE._serialized_end=6238
+  _ROTARYENCODERPINMODE._serialized_start=6241
+  _ROTARYENCODERPINMODE._serialized_end=6536
 # @@protoc_insertion_point(module_scope)
```

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/pb2-files/nanopb_pb2.py` & `gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/proto-files/enums.proto` & `gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/enums.proto`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,28 @@
     BUTTON_LAYOUT_TWINSTICKA = 7;
     BUTTON_LAYOUT_BLANKA = 8;
     BUTTON_LAYOUT_VLXA = 9;
     BUTTON_LAYOUT_FIGHTBOARD_STICK = 10;
     BUTTON_LAYOUT_FIGHTBOARD_MIRRORED = 11;
     BUTTON_LAYOUT_CUSTOMA = 12;
     BUTTON_LAYOUT_OPENCORE0WASDA = 13;
+    BUTTON_LAYOUT_STICKLESS_13 = 14;
+    BUTTON_LAYOUT_STICKLESS_16 = 15;
+    BUTTON_LAYOUT_STICKLESS_14 = 16;
+    BUTTON_LAYOUT_DANCEPAD_DDR_LEFT = 17;
+    BUTTON_LAYOUT_DANCEPAD_DDR_SOLO = 18;
+    BUTTON_LAYOUT_DANCEPAD_PIU_LEFT = 19;
+    BUTTON_LAYOUT_POPN_A = 20;
+    BUTTON_LAYOUT_TAIKO_A = 21;
+    BUTTON_LAYOUT_BM_TURNTABLE_A = 22;
+    BUTTON_LAYOUT_BM_5KEY_A = 23;
+    BUTTON_LAYOUT_BM_7KEY_A = 24;
+    BUTTON_LAYOUT_GITADORA_FRET_A = 25;
+    BUTTON_LAYOUT_GITADORA_STRUM_A = 26;
+    BUTTON_LAYOUT_BOARD_DEFINED_A = 27;
 }
 
 enum ButtonLayoutRight
 {
     option (nanopb_enumopt).long_names = false;
 
     BUTTON_LAYOUT_ARCADE = 0;
@@ -41,14 +55,27 @@
     BUTTON_LAYOUT_BLANKB = 12;
     BUTTON_LAYOUT_VLXB = 13;
     BUTTON_LAYOUT_FIGHTBOARD = 14;
     BUTTON_LAYOUT_FIGHTBOARD_STICK_MIRRORED = 15;
     BUTTON_LAYOUT_CUSTOMB = 16;
     BUTTON_LAYOUT_KEYBOARD8B = 17;
     BUTTON_LAYOUT_OPENCORE0WASDB = 18;
+    BUTTON_LAYOUT_STICKLESS_13B = 19;
+    BUTTON_LAYOUT_STICKLESS_16B = 20;
+    BUTTON_LAYOUT_STICKLESS_14B = 21;
+    BUTTON_LAYOUT_DANCEPAD_DDR_RIGHT = 22;
+    BUTTON_LAYOUT_DANCEPAD_PIU_RIGHT = 23;
+    BUTTON_LAYOUT_POPN_B = 24;
+    BUTTON_LAYOUT_TAIKO_B = 25;
+    BUTTON_LAYOUT_BM_TURNTABLE_B = 26;
+    BUTTON_LAYOUT_BM_5KEY_B = 27;
+    BUTTON_LAYOUT_BM_7KEY_B = 28;
+    BUTTON_LAYOUT_GITADORA_FRET_B = 29;
+    BUTTON_LAYOUT_GITADORA_STRUM_B = 30;
+    BUTTON_LAYOUT_BOARD_DEFINED_B = 31;
 }
 
 enum SplashMode
 {
     option (nanopb_enumopt).long_names = false;
 
     SPLASH_MODE_STATIC = 0;
@@ -92,17 +119,28 @@
     INPUT_MODE_MDMINI = 6;
     INPUT_MODE_NEOGEO = 7;
     INPUT_MODE_PCEMINI = 8;
     INPUT_MODE_EGRET = 9;
     INPUT_MODE_ASTRO = 10;
     INPUT_MODE_PSCLASSIC = 11;
     INPUT_MODE_XBOXORIGINAL = 12;
+    INPUT_MODE_PS5 = 13;
     INPUT_MODE_CONFIG = 255;
 }
 
+enum InputModeAuthType
+{
+    option (nanopb_enumopt).long_names = false;
+
+    INPUT_MODE_AUTH_TYPE_NONE = 0;
+    INPUT_MODE_AUTH_TYPE_KEYS = 1;
+    INPUT_MODE_AUTH_TYPE_USB = 2;
+    INPUT_MODE_AUTH_TYPE_I2C = 3;
+}
+
 enum DpadMode
 {
     option (nanopb_enumopt).long_names = false;
 
     DPAD_MODE_DIGITAL = 0;
     DPAD_MODE_LEFT_ANALOG = 1;
     DPAD_MODE_RIGHT_ANALOG = 2;
@@ -165,14 +203,22 @@
     SUSTAIN_DP_MODE_LS           = 25;
     SUSTAIN_DP_MODE_RS           = 26;
     SUSTAIN_SOCD_MODE_UP_PRIO    = 27;
     SUSTAIN_SOCD_MODE_NEUTRAL    = 28;
     SUSTAIN_SOCD_MODE_SECOND_WIN = 29;
     SUSTAIN_SOCD_MODE_FIRST_WIN  = 30;
     SUSTAIN_SOCD_MODE_BYPASS     = 31;
+    BUTTON_PRESS_TURBO           = 32;
+    BUTTON_PRESS_MACRO           = 33;
+    BUTTON_PRESS_MACRO_1         = 34;
+    BUTTON_PRESS_MACRO_2         = 35;
+    BUTTON_PRESS_MACRO_3         = 36;
+    BUTTON_PRESS_MACRO_4         = 37;
+    BUTTON_PRESS_MACRO_5         = 38;
+    BUTTON_PRESS_MACRO_6         = 39;
 }
 
 enum GamepadHotkey
 {
     option (nanopb_enumopt).long_names = false;
 
     HOTKEY_NONE                  = 0;
@@ -244,14 +290,24 @@
     
 	FORCED_SETUP_MODE_OFF = 0;
 	FORCED_SETUP_MODE_LOCK_MODE_SWITCH = 1;
 	FORCED_SETUP_MODE_LOCK_WEB_CONFIG = 2;
 	FORCED_SETUP_MODE_LOCK_BOTH = 3;
 };
 
+enum DualDirectionalCombinationMode
+{
+	option (nanopb_enumopt).long_names = false;
+
+	MIXED_MODE = 0;
+	GAMEPAD_MODE = 1;
+	DUAL_MODE = 2;
+	NONE_MODE = 3;
+}
+
 enum PS4ControllerType
 {
     option (nanopb_enumopt).long_names = false;
     
     PS4_CONTROLLER = 0;
     PS4_ARCADESTICK = 7;
 }
@@ -260,7 +316,48 @@
 {
     option (nanopb_enumopt).long_names = false;
 
     ON_PRESS = 1;
     ON_HOLD_REPEAT = 2;
     ON_TOGGLE = 3;
 };
+
+enum GPElement
+{
+    option (nanopb_enumopt).long_names = false;
+
+    GP_ELEMENT_WIDGET = 0;
+    GP_ELEMENT_SCREEN = 1;
+    GP_ELEMENT_BTN_BUTTON = 2;
+    GP_ELEMENT_DIR_BUTTON = 3;
+    GP_ELEMENT_PIN_BUTTON = 4;
+    GP_ELEMENT_LEVER = 5;
+    GP_ELEMENT_LABEL = 6;
+    GP_ELEMENT_SPRITE = 7;
+    GP_ELEMENT_SHAPE = 8;
+};
+
+enum GPShape_Type
+{
+    option (nanopb_enumopt).long_names = false;
+    
+    GP_SHAPE_ELLIPSE = 0;
+    GP_SHAPE_SQUARE = 1;
+    GP_SHAPE_DIAMOND = 2;
+    GP_SHAPE_POLYGON = 3;
+    GP_SHAPE_ARC = 4;
+};
+
+enum RotaryEncoderPinMode
+{
+    option (nanopb_enumopt).long_names = false;
+
+    ENCODER_MODE_NONE = 0;
+    ENCODER_MODE_LEFT_ANALOG_X = 1;
+    ENCODER_MODE_LEFT_ANALOG_Y = 2;
+    ENCODER_MODE_RIGHT_ANALOG_X = 3;
+    ENCODER_MODE_RIGHT_ANALOG_Y = 4;
+    ENCODER_MODE_LEFT_TRIGGER = 5;
+    ENCODER_MODE_RIGHT_TRIGGER = 6;
+    ENCODER_MODE_DPAD_X = 7;
+    ENCODER_MODE_DPAD_Y = 8;
+};
```

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/proto-files/nanopb.proto` & `gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/test-binary-source-of-json-config.bin` & `gp2040ce-binary-tools-0.7.0/tests/test-files/test-binary-source-of-json-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/test-config.bin` & `gp2040ce-binary-tools-0.7.0/tests/test-files/test-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/test-config.json` & `gp2040ce-binary-tools-0.7.0/tests/test-files/test-config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996060606060606%*

 * *Differences: {"'addonOptions'": "{'turboOptions': {'deprecatedButtonPin': -1, delete: ['buttonPin']}, "*

 * *                   "'macroOptions': {'macroList': {0: {'deprecatedMacroTriggerPin': -1, delete: "*

 * *                   "['macroTriggerPin']}, 1: {'deprecatedMacroTriggerPin': -1, delete: "*

 * *                   "['macroTriggerPin']}, 2: {'deprecatedMacroTriggerPin': -1, delete: "*

 * *                   "['macroTriggerPin']}, 3: {'deprecatedMacroTriggerPin': -1, delete: "*

 * *                   "['macroTriggerPin']}, 4: {'deprecate […]*

```diff
@@ -83,85 +83,85 @@
                 "keyDpadDown": 81,
                 "keyDpadLeft": 80,
                 "keyDpadRight": 79,
                 "keyDpadUp": 82
             }
         },
         "macroOptions": {
+            "deprecatedPin": -1,
             "enabled": false,
             "macroBoardLedEnabled": true,
             "macroList": [
                 {
+                    "deprecatedMacroTriggerPin": -1,
                     "enabled": false,
                     "exclusive": true,
                     "interruptible": true,
                     "macroLabel": "",
                     "macroTriggerButton": 0,
-                    "macroTriggerPin": -1,
                     "macroType": "ON_PRESS",
                     "showFrames": false,
                     "useMacroTriggerButton": false
                 },
                 {
+                    "deprecatedMacroTriggerPin": -1,
                     "enabled": false,
                     "exclusive": true,
                     "interruptible": true,
                     "macroLabel": "",
                     "macroTriggerButton": 0,
-                    "macroTriggerPin": -1,
                     "macroType": "ON_PRESS",
                     "showFrames": false,
                     "useMacroTriggerButton": false
                 },
                 {
+                    "deprecatedMacroTriggerPin": -1,
                     "enabled": false,
                     "exclusive": true,
                     "interruptible": true,
                     "macroLabel": "",
                     "macroTriggerButton": 0,
-                    "macroTriggerPin": -1,
                     "macroType": "ON_PRESS",
                     "showFrames": false,
                     "useMacroTriggerButton": false
                 },
                 {
+                    "deprecatedMacroTriggerPin": -1,
                     "enabled": false,
                     "exclusive": true,
                     "interruptible": true,
                     "macroLabel": "",
                     "macroTriggerButton": 0,
-                    "macroTriggerPin": -1,
                     "macroType": "ON_PRESS",
                     "showFrames": false,
                     "useMacroTriggerButton": false
                 },
                 {
+                    "deprecatedMacroTriggerPin": -1,
                     "enabled": false,
                     "exclusive": true,
                     "interruptible": true,
                     "macroLabel": "",
                     "macroTriggerButton": 0,
-                    "macroTriggerPin": -1,
                     "macroType": "ON_PRESS",
                     "showFrames": false,
                     "useMacroTriggerButton": false
                 },
                 {
+                    "deprecatedMacroTriggerPin": -1,
                     "enabled": false,
                     "exclusive": true,
                     "interruptible": true,
                     "macroLabel": "",
                     "macroTriggerButton": 0,
-                    "macroTriggerPin": -1,
                     "macroType": "ON_PRESS",
                     "showFrames": false,
                     "useMacroTriggerButton": false
                 }
-            ],
-            "pin": -1
+            ]
         },
         "onBoardLedOptions": {
             "enabled": false,
             "mode": "ON_BOARD_LED_MODE_MODE_INDICATOR"
         },
         "playerNumberOptions": {
             "enabled": false,
@@ -237,15 +237,15 @@
             "tiltRightAnalogDownPin": -1,
             "tiltRightAnalogLeftPin": -1,
             "tiltRightAnalogRightPin": -1,
             "tiltRightAnalogUpPin": -1,
             "tiltSOCDMode": "SOCD_MODE_NEUTRAL"
         },
         "turboOptions": {
-            "buttonPin": -1,
+            "deprecatedButtonPin": -1,
             "enabled": false,
             "ledPin": -1,
             "shmupAlwaysOn1": 0,
             "shmupAlwaysOn2": 0,
             "shmupAlwaysOn3": 0,
             "shmupAlwaysOn4": 0,
             "shmupBtn1Pin": -1,
```

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/test-firmware.bin` & `gp2040ce-binary-tools-0.7.0/tests/test-files/test-firmware.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/test-storage-area.bin` & `gp2040ce-binary-tools-0.7.0/tests/test-files/test-storage-area.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/test-whole-board-with-board-config.bin` & `gp2040ce-binary-tools-0.7.0/tests/test-files/test-whole-board-with-board-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test-files/test-whole-board.bin` & `gp2040ce-binary-tools-0.7.0/tests/test-files/test-whole-board.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test_builder.py` & `gp2040ce-binary-tools-0.7.0/tests/test_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Tests for the image builder module.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import os
 import sys
 import unittest.mock as mock
 
 import pytest
 from decorator import decorator
 
 from gp2040ce_bintools import get_config_pb2
 from gp2040ce_bintools.builder import (FirmwareLengthError, combine_firmware_and_config,
-                                       concatenate_firmware_and_storage_files, convert_binary_to_uf2,
-                                       get_gp2040ce_from_usb, pad_binary_up_to_board_config,
-                                       pad_binary_up_to_user_config, replace_config_in_binary,
-                                       write_new_config_to_filename, write_new_config_to_usb)
-from gp2040ce_bintools.storage import (get_board_storage_section, get_config, get_config_footer,
+                                       concatenate_firmware_and_storage_files, get_gp2040ce_from_usb,
+                                       pad_binary_up_to_board_config, pad_binary_up_to_user_config,
+                                       replace_config_in_binary, write_new_config_to_filename, write_new_config_to_usb)
+from gp2040ce_bintools.storage import (STORAGE_SIZE, get_board_storage_section, get_config, get_config_footer,
                                        get_user_storage_section, serialize_config_with_footer)
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 
 @decorator
 def with_pb2s(test, *args, **kwargs):
@@ -72,23 +71,14 @@
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 3309
     storage = get_user_storage_section(content)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 3309
 
 
-def test_convert_binary_to_uf2(whole_board_with_board_config_dump):
-    """Do some sanity checks in the attempt to convert a binary to a UF2."""
-    uf2 = convert_binary_to_uf2(whole_board_with_board_config_dump)
-    assert len(uf2) == 4194304                              # binary is 8192 256 byte chunks, UF2 is 512 b per chunk
-    assert uf2[0:4] == b'\x55\x46\x32\x0a' == b'UF2\n'      # proper magic
-    assert uf2[8:12] == bytearray(b'\x00\x20\x00\x00')      # family ID set
-    assert uf2[524:528] == bytearray(b'\x00\x01\x00\x10')   # address to write the second chunk
-
-
 @with_pb2s
 def test_concatenate_user_json_to_file(tmp_path):
     """Test that we write a file with firmware + JSON user config as expected."""
     tmp_file = os.path.join(tmp_path, 'concat.bin')
     firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
     config_file = os.path.join(HERE, 'test-files', 'test-config.json')
     concatenate_firmware_and_storage_files(firmware_file, json_user_config_filename=config_file,
@@ -279,14 +269,31 @@
     config = get_config(config_dump)
     config_size, _, _ = get_config_footer(config_dump)
     assert config.boardVersion == 'v0.7.5-COOL'
     assert len(config_dump) == config_size + 12
 
 
 @with_pb2s
+def test_write_new_config_to_config_uf2(firmware_binary, tmp_path):
+    """Test that the config can be written to a file."""
+    tmp_file = os.path.join(tmp_path, 'config.uf2')
+    config_pb2 = get_config_pb2()
+    config = config_pb2.Config()
+    config.boardVersion = 'v0.7.5-COOL'
+    write_new_config_to_filename(config, tmp_file)
+
+    # read new file
+    with open(tmp_file, 'rb') as file:
+        config_dump = file.read()
+    # the current implementation of UF2 writing does it in 256 blocks, so each 256 byte block of
+    # binary is 512 bytes in the UF2
+    assert len(config_dump) == STORAGE_SIZE * 2
+
+
+@with_pb2s
 def test_write_new_config_to_usb(config_binary):
     """Test that the config can be written to USB at the proper alignment."""
     config = get_config(config_binary)
     serialized = serialize_config_with_footer(config)
     end_out, end_in = mock.MagicMock(), mock.MagicMock()
     with mock.patch('gp2040ce_bintools.builder.write') as mock_write:
         write_new_config_to_usb(config, end_out, end_in)
```

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test_commands.py` & `gp2040ce-binary-tools-0.7.0/tests/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test our tools themselves to make sure they adhere to certain flags.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import json
 import os
 import sys
 from subprocess import run
 
 from decorator import decorator
```

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test_gui.py` & `gp2040ce-binary-tools-0.7.0/tests/test_gui.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test the Textual GUI.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import os
 import sys
 import unittest.mock as mock
 
 import pytest
 from decorator import decorator
@@ -117,15 +117,15 @@
         tree.select_node(i2cspeed_node)
         tree.action_select_cursor()
         await pilot.wait_for_scheduled_animations()
         await pilot.click('Input#field-input')
         await pilot.wait_for_scheduled_animations()
         await pilot.press('backspace', 'backspace', 'backspace', 'backspace', 'backspace', 'backspace', '5')
         await pilot.wait_for_scheduled_animations()
-        await pilot.click('Button#save-button')
+        await pilot.click('Button#confirm-button')
         assert pilot.app.config.displayOptions.deprecatedI2cSpeed == 5
 
 
 @pytest.mark.asyncio
 @with_pb2s
 async def test_simple_edit_via_input_field_enum():
     """Test that we can change an enum via the UI and see it reflected in the config."""
@@ -141,15 +141,15 @@
         tree.select_node(dpadmode_node)
         tree.action_select_cursor()
         await pilot.wait_for_scheduled_animations()
         await pilot.click('Select#field-input')
         await pilot.wait_for_scheduled_animations()
         await pilot.press('down', 'down', 'enter')
         await pilot.wait_for_scheduled_animations()
-        await pilot.click('Button#save-button')
+        await pilot.click('Button#confirm-button')
         assert pilot.app.config.gamepadOptions.dpadMode == 1
 
 
 @pytest.mark.asyncio
 @with_pb2s
 async def test_simple_edit_via_input_field_string():
     """Test that we can change a string via the UI and see it reflected in the config."""
@@ -162,15 +162,15 @@
         tree.select_node(version_node)
         tree.action_select_cursor()
         await pilot.wait_for_scheduled_animations()
         await pilot.click('Input#field-input')
         await pilot.wait_for_scheduled_animations()
         await pilot.press('backspace', '-', 'h', 'i')
         await pilot.wait_for_scheduled_animations()
-        await pilot.click('Button#save-button')
+        await pilot.click('Button#confirm-button')
         assert pilot.app.config.boardVersion == 'v0.7.-hi'
 
 
 @pytest.mark.asyncio
 @with_pb2s
 async def test_add_node_to_repeated():
     """Test that we can navigate to an empty repeated and add a node."""
@@ -179,28 +179,28 @@
         tree = pilot.app.query_one(Tree)
         profile_node = tree.root.children[13]
         altpinmappings_node = profile_node.children[0]
 
         tree.root.expand_all()
         await pilot.wait_for_scheduled_animations()
         tree.select_node(altpinmappings_node)
-        await pilot.press('a')
+        await pilot.press('n')
         newpinmappings_node = altpinmappings_node.children[0]
         newpinmappings_node.expand()
         await pilot.wait_for_scheduled_animations()
         tree.select_node(newpinmappings_node)
         b4_node = newpinmappings_node.children[3]
         tree.select_node(b4_node)
         tree.action_select_cursor()
         await pilot.wait_for_scheduled_animations()
         await pilot.click('Input#field-input')
         await pilot.wait_for_scheduled_animations()
         await pilot.press('backspace', 'backspace', 'backspace', 'backspace', 'backspace', 'backspace', '5')
         await pilot.wait_for_scheduled_animations()
-        await pilot.click('Button#save-button')
+        await pilot.click('Button#confirm-button')
 
         assert pilot.app.config.profileOptions.deprecatedAlternativePinMappings[0].pinButtonB4 == 5
 
 
 @pytest.mark.asyncio
 @with_pb2s
 async def test_save(config_binary, tmp_path):
@@ -212,7 +212,32 @@
     app = ConfigEditor(config_filename=new_filename)
     async with app.run_test() as pilot:
         pilot.app.config.boardVersion = 'v0.7.5-bss-wuz-here'
         await pilot.press('s')
 
     config = get_config_from_file(new_filename)
     assert config.boardVersion == 'v0.7.5-bss-wuz-here'
+
+
+@pytest.mark.asyncio
+@with_pb2s
+async def test_save_as(config_binary, tmp_path):
+    """Test that we can save to a new file."""
+    filename = os.path.join(tmp_path, 'config-original.bin')
+    with open(filename, 'wb') as file:
+        file.write(config_binary)
+    original_config = get_config(config_binary)
+
+    app = ConfigEditor(config_filename=filename)
+    async with app.run_test() as pilot:
+        await pilot.press('a')
+        await pilot.wait_for_scheduled_animations()
+        await pilot.click('Input#field-input')
+        await pilot.wait_for_scheduled_animations()
+        await pilot.press('/', 't', 'm', 'p', '/', 'g', 'p', 't', 'e', 's', 't')
+        await pilot.wait_for_scheduled_animations()
+        await pilot.click('Button#confirm-button')
+
+    with open('/tmp/gptest', 'rb') as new_file:
+        test_config_binary = new_file.read()
+    test_config = get_config(test_config_binary)
+    assert original_config == test_config
```

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test_package.py` & `gp2040ce-binary-tools-0.7.0/tests/test_package.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test high level package capabilities.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import os
 import sys
 
 from gp2040ce_bintools import get_config_pb2
 
 HERE = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test_rp2040.py` & `gp2040ce-binary-tools-0.7.0/tests/test_rp2040.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test operations for interfacing directly with a Pico.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import os
 import struct
 import sys
 import unittest.mock as mock
 from array import array
```

### Comparing `gp2040ce-binary-tools-0.6.0/tests/test_storage.py` & `gp2040ce-binary-tools-0.7.0/tests/test_storage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for the storage module.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
-SPDX-License-Identifier: MIT
+SPDX-License-Identifier: GPL-3.0-or-later
 """
 import os
 import sys
 import unittest.mock as mock
 
 import pytest
 from decorator import decorator
@@ -126,14 +126,32 @@
     """Test that we can read in a whole board and still find the config section."""
     config = storage.get_config(storage.get_user_storage_section(whole_board_dump))
     assert config.boardVersion == 'v0.7.5'
     assert config.hotkeyOptions.hotkey01.dpadMask == 0
     assert config.hotkeyOptions.hotkey02.dpadMask == 1
 
 
+def test_convert_binary_to_uf2(whole_board_with_board_config_dump):
+    """Do some sanity checks in the attempt to convert a binary to a UF2."""
+    uf2 = storage.convert_binary_to_uf2(whole_board_with_board_config_dump)
+    assert len(uf2) == 4194304                              # binary is 8192 256 byte chunks, UF2 is 512 b per chunk
+    assert uf2[0:4] == b'\x55\x46\x32\x0a' == b'UF2\n'      # proper magic
+    assert uf2[8:12] == bytearray(b'\x00\x20\x00\x00')      # family ID set
+    assert uf2[524:528] == bytearray(b'\x00\x01\x00\x10')   # address to write the second chunk
+
+
+def test_convert_binary_to_uf2_with_offsets(whole_board_with_board_config_dump):
+    """Do some sanity checks in the attempt to convert a binary to a UF2."""
+    uf2 = storage.convert_binary_to_uf2(whole_board_with_board_config_dump, start=storage.USER_CONFIG_BINARY_LOCATION)
+    assert len(uf2) == 4194304                              # binary is 8192 256 byte chunks, UF2 is 512 b per chunk
+    assert uf2[0:4] == b'\x55\x46\x32\x0a' == b'UF2\n'      # proper magic
+    assert uf2[8:12] == bytearray(b'\x00\x20\x00\x00')      # family ID set
+    assert uf2[524:528] == bytearray(b'\x00\xc1\x1f\x10')   # address to write the second chunk
+
+
 @with_pb2s
 def test_serialize_config_with_footer(storage_dump, config_binary):
     """Test that reserializing a read in config matches the original.
 
     Note that this isn't going to produce an *identical* result, because new message fields
     may have default values that get saved in the reserialized binary, so we can still only test
     some particular parts. But it should work.
```

### Comparing `gp2040ce-binary-tools-0.6.0/tox.ini` & `gp2040ce-binary-tools-0.7.0/tox.ini`

 * *Files identical despite different names*

