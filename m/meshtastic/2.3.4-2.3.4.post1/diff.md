# Comparing `tmp/meshtastic-2.3.4.tar.gz` & `tmp/meshtastic-2.3.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic-2.3.4.tar", last modified: Mon Apr  8 17:14:13 2024, max compression
+gzip compressed data, was "meshtastic-2.3.4.post1.tar", last modified: Mon Apr  8 17:50:04 2024, max compression
```

## Comparing `meshtastic-2.3.4.tar` & `meshtastic-2.3.4.post1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:13.051780 meshtastic-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 17:14:00.000000 meshtastic-2.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 17:14:00.000000 meshtastic-2.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-08 17:14:13.051780 meshtastic-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-08 17:14:00.000000 meshtastic-2.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:13.051780 meshtastic-2.3.4/meshtastic/
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53538 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/admin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/apponly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/apponly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/atak_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/atak_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/ble_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/cannedmessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/cannedmessages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/channel_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/clientonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/clientonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    65909 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/connection_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/connection_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/deviceonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/deviceonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/localonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/localonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    41793 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/mesh_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15034 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    86471 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/mesh_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/module_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    48852 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/module_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/mqtt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/mqtt_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/nanopb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/nanopb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    30759 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/paxcount_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/paxcount_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/portnums_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/portnums_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/remote_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/remote_hardware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/remote_hardware_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/rtttl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/rtttl_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/serial_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/storeforward_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/storeforward_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/stream_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/supported_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/telemetry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/telemetry_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    20907 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/xmodem_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/xmodem_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:13.051780 meshtastic-2.3.4/meshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:14:13.051780 meshtastic-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-08 17:14:00.000000 meshtastic-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:04.482169 meshtastic-2.3.4.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-08 17:50:04.482169 meshtastic-2.3.4.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:04.478169 meshtastic-2.3.4.post1/meshtastic/
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53538 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/admin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/apponly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/apponly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/atak_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/atak_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/ble_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/cannedmessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/cannedmessages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/channel_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/clientonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/clientonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65909 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/connection_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/connection_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/deviceonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/deviceonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/localonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/localonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    41793 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/mesh_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15034 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86471 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/mesh_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/module_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48852 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/module_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/mqtt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/mqtt_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/nanopb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/nanopb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    30759 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/paxcount_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/paxcount_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/portnums_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/portnums_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/remote_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/remote_hardware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/remote_hardware_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/rtttl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/rtttl_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/serial_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/storeforward_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/storeforward_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/stream_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/supported_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/telemetry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/telemetry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20907 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/xmodem_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/xmodem_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:04.478169 meshtastic-2.3.4.post1/meshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:50:04.482169 meshtastic-2.3.4.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/setup.py
```

### Comparing `meshtastic-2.3.4/LICENSE.txt` & `meshtastic-2.3.4.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/PKG-INFO` & `meshtastic-2.3.4.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.4
+Version: 2.3.4.post1
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyserial>=3.4
-Requires-Dist: protobuf>=3.13.0
+Requires-Dist: protobuf>=5.26.0
 Requires-Dist: requests>=2.25.0
 Requires-Dist: pypubsub>=4.0.3
 Requires-Dist: dotmap>=1.3.14
 Requires-Dist: pexpect>=4.6.0
 Requires-Dist: pyqrcode>=1.2.1
 Requires-Dist: tabulate>=0.8.9
 Requires-Dist: timeago>=1.0.15
```

### Comparing `meshtastic-2.3.4/README.md` & `meshtastic-2.3.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/__init__.py` & `meshtastic-2.3.4.post1/meshtastic/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/__main__.py` & `meshtastic-2.3.4.post1/meshtastic/__main__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/admin_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/admin_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/apponly_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/apponly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/apponly_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/apponly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/atak_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/atak_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/atak_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/atak_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/ble_interface.py` & `meshtastic-2.3.4.post1/meshtastic/ble_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/cannedmessages_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/cannedmessages_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/cannedmessages_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/cannedmessages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/channel_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/channel_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/clientonly_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/clientonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/clientonly_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/clientonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/config_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/config_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/connection_status_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/connection_status_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/connection_status_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/connection_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/deviceonly_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/deviceonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/deviceonly_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/deviceonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/globals.py` & `meshtastic-2.3.4.post1/meshtastic/globals.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/localonly_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/localonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/localonly_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/localonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/mesh_interface.py` & `meshtastic-2.3.4.post1/meshtastic/mesh_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/mesh_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/mesh_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/mesh_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/module_config_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/module_config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/module_config_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/module_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/mqtt_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/mqtt_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/mqtt_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/nanopb_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/nanopb_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/nanopb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/node.py` & `meshtastic-2.3.4.post1/meshtastic/node.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/paxcount_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/paxcount_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/paxcount_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/paxcount_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/portnums_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/portnums_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/portnums_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/portnums_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/remote_hardware.py` & `meshtastic-2.3.4.post1/meshtastic/remote_hardware.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/remote_hardware_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/remote_hardware_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/remote_hardware_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/remote_hardware_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/rtttl_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/rtttl_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/rtttl_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/rtttl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/serial_interface.py` & `meshtastic-2.3.4.post1/meshtastic/serial_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/storeforward_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/storeforward_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/storeforward_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/storeforward_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/stream_interface.py` & `meshtastic-2.3.4.post1/meshtastic/stream_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/supported_device.py` & `meshtastic-2.3.4.post1/meshtastic/supported_device.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/tcp_interface.py` & `meshtastic-2.3.4.post1/meshtastic/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/telemetry_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/telemetry_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/telemetry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/test.py` & `meshtastic-2.3.4.post1/meshtastic/test.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/tunnel.py` & `meshtastic-2.3.4.post1/meshtastic/tunnel.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/util.py` & `meshtastic-2.3.4.post1/meshtastic/util.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/xmodem_pb2.py` & `meshtastic-2.3.4.post1/meshtastic/xmodem_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic/xmodem_pb2.pyi` & `meshtastic-2.3.4.post1/meshtastic/xmodem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/meshtastic.egg-info/PKG-INFO` & `meshtastic-2.3.4.post1/meshtastic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.4
+Version: 2.3.4.post1
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyserial>=3.4
-Requires-Dist: protobuf>=3.13.0
+Requires-Dist: protobuf>=5.26.0
 Requires-Dist: requests>=2.25.0
 Requires-Dist: pypubsub>=4.0.3
 Requires-Dist: dotmap>=1.3.14
 Requires-Dist: pexpect>=4.6.0
 Requires-Dist: pyqrcode>=1.2.1
 Requires-Dist: tabulate>=0.8.9
 Requires-Dist: timeago>=1.0.15
```

### Comparing `meshtastic-2.3.4/meshtastic.egg-info/SOURCES.txt` & `meshtastic-2.3.4.post1/meshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4/setup.py` & `meshtastic-2.3.4.post1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # This call to setup() does all the work
 setup(
     name="meshtastic",
-    version="2.3.4",
+    version="2.3.4.post1",
     description="Python API & client shell for talking to Meshtastic devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meshtastic/python",
     author="Meshtastic Developers",
     author_email="contact@meshtastic.org",
     license="GPL-3.0-only",
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     packages=["meshtastic"],
     include_package_data=True,
     install_requires=[
         "pyserial>=3.4",
-        "protobuf>=3.13.0",
+        "protobuf>=5.26.0",
         "requests>=2.25.0",
         "pypubsub>=4.0.3",
         "dotmap>=1.3.14",
         "pexpect>=4.6.0",
         "pyqrcode>=1.2.1",
         "tabulate>=0.8.9",
         "timeago>=1.0.15",
```

