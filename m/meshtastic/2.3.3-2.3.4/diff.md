# Comparing `tmp/meshtastic-2.3.3.tar.gz` & `tmp/meshtastic-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic-2.3.3.tar", last modified: Fri Mar 29 16:26:42 2024, max compression
+gzip compressed data, was "meshtastic-2.3.4.tar", last modified: Mon Apr  8 17:14:13 2024, max compression
```

## Comparing `meshtastic-2.3.3.tar` & `meshtastic-2.3.4.tar`

### file list

```diff
@@ -1,51 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:26:42.903577 meshtastic-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-29 16:26:33.000000 meshtastic-2.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-29 16:26:33.000000 meshtastic-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-29 16:26:42.903577 meshtastic-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-03-29 16:26:33.000000 meshtastic-2.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:26:42.903577 meshtastic-2.3.3/meshtastic/
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52289 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/apponly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/atak_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/ble_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/cannedmessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/clientonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/connection_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/deviceonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/localonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    41824 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/mesh_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    14587 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/module_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/mqtt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/nanopb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    30845 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/paxcount_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/portnums_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/remote_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/remote_hardware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/rtttl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/serial_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/storeforward_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/stream_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/supported_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/telemetry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    20642 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-29 16:26:33.000000 meshtastic-2.3.3/meshtastic/xmodem_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:26:42.903577 meshtastic-2.3.3/meshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-29 16:26:42.000000 meshtastic-2.3.3/meshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-29 16:26:42.000000 meshtastic-2.3.3/meshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:26:42.000000 meshtastic-2.3.3/meshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-29 16:26:42.000000 meshtastic-2.3.3/meshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-29 16:26:42.000000 meshtastic-2.3.3/meshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 16:26:42.000000 meshtastic-2.3.3/meshtastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 16:26:42.903577 meshtastic-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-29 16:26:33.000000 meshtastic-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:13.051780 meshtastic-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 17:14:00.000000 meshtastic-2.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 17:14:00.000000 meshtastic-2.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-08 17:14:13.051780 meshtastic-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-08 17:14:00.000000 meshtastic-2.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:13.051780 meshtastic-2.3.4/meshtastic/
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53538 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/admin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/apponly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/apponly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/atak_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/atak_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/ble_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/cannedmessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/cannedmessages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/channel_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/clientonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/clientonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65909 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/connection_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/connection_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/deviceonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/deviceonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/localonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/localonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    41793 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/mesh_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15034 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86471 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/mesh_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/module_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48852 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/module_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/mqtt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/mqtt_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/nanopb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/nanopb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    30759 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/paxcount_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/paxcount_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/portnums_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/portnums_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/remote_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/remote_hardware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/remote_hardware_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/rtttl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/rtttl_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/serial_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/storeforward_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/storeforward_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/stream_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/supported_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/telemetry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/telemetry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20907 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/xmodem_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-08 17:14:00.000000 meshtastic-2.3.4/meshtastic/xmodem_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:13.051780 meshtastic-2.3.4/meshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 17:14:13.000000 meshtastic-2.3.4/meshtastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:14:13.051780 meshtastic-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-08 17:14:00.000000 meshtastic-2.3.4/setup.py
```

### Comparing `meshtastic-2.3.3/LICENSE.txt` & `meshtastic-2.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.3/PKG-INFO` & `meshtastic-2.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.3
+Version: 2.3.4
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
@@ -29,30 +29,30 @@
 Requires-Dist: bleak>=0.21.1
 Requires-Dist: packaging
 Provides-Extra: tunnel
 Requires-Dist: pytap2>=2.0.0; extra == "tunnel"
 
 # Meshtastic Python
 
-[![codecov](https://codecov.io/gh/meshtastic/Meshtastic-python/branch/master/graph/badge.svg?token=TIWPJL73KV)](https://codecov.io/gh/meshtastic/Meshtastic-python)
+[![codecov](https://codecov.io/gh/meshtastic/python/branch/master/graph/badge.svg?token=TIWPJL73KV)](https://codecov.io/gh/meshtastic/python)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/meshtastic)
 [![CI](https://img.shields.io/github/actions/workflow/status/meshtastic/python/ci.yml?branch=master&label=actions&logo=github&color=yellow)](https://github.com/meshtastic/python/actions/workflows/ci.yml)
 [![CLA assistant](https://cla-assistant.io/readme/badge/meshtastic/python)](https://cla-assistant.io/meshtastic/python)
 [![Fiscal Contributors](https://opencollective.com/meshtastic/tiers/badge.svg?label=Fiscal%20Contributors&color=deeppink)](https://opencollective.com/meshtastic/)
 
 ## Overview
 
 A Python client for use with Meshtastic devices.
 This small library (and example application) provides an easy API for sending and receiving messages over mesh radios.
 It also provides access to any of the operations/data available in the device user interface or the Android application.
 Events are delivered using a publish-subscribe model, and you can subscribe to only the message types you are interested in.
 
 **[Getting Started Guide](https://meshtastic.org/docs/software/python/cli/installation)**
 
-**[Documentation/API Reference](https://python.meshtastic.org/)**
+(Documentation/API Reference is currently offline)
 
 ## Call for Contributors
 
 This library and CLI has gone without a consistent maintainer for a while, and there's many improvements that could be made. We're all volunteers here and help is extremely appreciated, whether in implementing your own needs or helping maintain the library and CLI in general.
 
 If you're interested in contributing but don't have specific things you'd like to work on, look at the roadmap below!
```

### Comparing `meshtastic-2.3.3/README.md` & `meshtastic-2.3.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Meshtastic Python
 
-[![codecov](https://codecov.io/gh/meshtastic/Meshtastic-python/branch/master/graph/badge.svg?token=TIWPJL73KV)](https://codecov.io/gh/meshtastic/Meshtastic-python)
+[![codecov](https://codecov.io/gh/meshtastic/python/branch/master/graph/badge.svg?token=TIWPJL73KV)](https://codecov.io/gh/meshtastic/python)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/meshtastic)
 [![CI](https://img.shields.io/github/actions/workflow/status/meshtastic/python/ci.yml?branch=master&label=actions&logo=github&color=yellow)](https://github.com/meshtastic/python/actions/workflows/ci.yml)
 [![CLA assistant](https://cla-assistant.io/readme/badge/meshtastic/python)](https://cla-assistant.io/meshtastic/python)
 [![Fiscal Contributors](https://opencollective.com/meshtastic/tiers/badge.svg?label=Fiscal%20Contributors&color=deeppink)](https://opencollective.com/meshtastic/)
 
 ## Overview
 
 A Python client for use with Meshtastic devices.
 This small library (and example application) provides an easy API for sending and receiving messages over mesh radios.
 It also provides access to any of the operations/data available in the device user interface or the Android application.
 Events are delivered using a publish-subscribe model, and you can subscribe to only the message types you are interested in.
 
 **[Getting Started Guide](https://meshtastic.org/docs/software/python/cli/installation)**
 
-**[Documentation/API Reference](https://python.meshtastic.org/)**
+(Documentation/API Reference is currently offline)
 
 ## Call for Contributors
 
 This library and CLI has gone without a consistent maintainer for a while, and there's many improvements that could be made. We're all volunteers here and help is extremely appreciated, whether in implementing your own needs or helping maintain the library and CLI in general.
 
 If you're interested in contributing but don't have specific things you'd like to work on, look at the roadmap below!
```

### Comparing `meshtastic-2.3.3/meshtastic/__init__.py` & `meshtastic-2.3.4/meshtastic/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.3/meshtastic/__main__.py` & `meshtastic-2.3.4/meshtastic/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 import argparse
 import logging
 import os
 import platform
 import sys
 import time
 
-import pyqrcode
+import pyqrcode # type: ignore[import-untyped]
 import yaml
 from google.protobuf.json_format import MessageToDict
-from pubsub import pub
+from pubsub import pub # type: ignore[import-untyped]
 
 import meshtastic.test
 import meshtastic.util
-from meshtastic import channel_pb2, config_pb2, portnums_pb2, remote_hardware
+from meshtastic import channel_pb2, config_pb2, portnums_pb2, remote_hardware, BROADCAST_ADDR
 from meshtastic.version import get_active_version
-from meshtastic.__init__ import BROADCAST_ADDR
 from meshtastic.ble_interface import BLEInterface
 from meshtastic.globals import Globals
 
 
 def onReceive(packet, interface):
     """Callback invoked when a packet arrives"""
     our_globals = Globals.getInstance()
@@ -143,15 +142,15 @@
     snake_name = meshtastic.util.camel_to_snake(name[1])
     camel_name = meshtastic.util.snake_to_camel(name[1])
     logging.debug(f"snake_name:{snake_name}")
     logging.debug(f"camel_name:{camel_name}")
 
     objDesc = config.DESCRIPTOR
     config_type = objDesc.fields_by_name.get(name[0])
-    pref = False
+    pref = None
     if config_type and config_type.message_type is not None:
         pref = config_type.message_type.fields_by_name.get(snake_name)
     # Others like ChannelSettings are standalone
     elif config_type:
         pref = config_type
 
     if (not pref) or (not config_type):
@@ -848,15 +847,15 @@
     # We now call onConnected from main
     # pub.subscribe(onConnected, "meshtastic.connection.established")
 
     # pub.subscribe(onNode, "meshtastic.node")
 
 
 def export_config(interface):
-    """used in--export-config"""
+    """used in --export-config"""
     configObj = {}
 
     owner = interface.getLongName()
     owner_short = interface.getShortName()
     channel_url = interface.localNode.getURL()
     myinfo = interface.getMyNodeInfo()
     pos = myinfo.get("position")
@@ -915,15 +914,15 @@
 def common():
     """Shared code for all of our command line wrappers"""
     logfile = None
     our_globals = Globals.getInstance()
     args = our_globals.get_args()
     parser = our_globals.get_parser()
     logging.basicConfig(
-        level=logging.DEBUG if args.debug else logging.INFO,
+        level=logging.DEBUG if (args.debug or args.listen) else logging.INFO,
         format="%(levelname)s file:%(filename)s %(funcName)s line:%(lineno)s %(message)s",
     )
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         meshtastic.util.our_exit("", 1)
     else:
@@ -1027,402 +1026,429 @@
             ):  # loop until someone presses ctrlc
                 while True:
                     time.sleep(1000)
 
         # don't call exit, background threads might be running still
         # sys.exit(0)
 
+def addConnectionArgs(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
+    """Add connection specifiation arguments"""
+
+    outer = parser.add_argument_group('Connection', 'Optional arguments that specify how to connect to a Meshtastic device.')
+    group = outer.add_mutually_exclusive_group()
+    group.add_argument(
+        "--port",
+        help="The port of the device to connect to using serial, e.g. /dev/ttyUSB0.",
+        default=None,
+    )
+
+    group.add_argument(
+        "--host",
+        help="The hostname or IP address of the device to connect to using TCP",
+        default=None,
+    )
+
+    group.add_argument(
+        "--ble",
+        help="The BLE device address or name to connect to",
+        default=None,
+    )
+
+    return parser
+
 
 def initParser():
     """Initialize the command line argument parsing."""
     our_globals = Globals.getInstance()
     parser = our_globals.get_parser()
     args = our_globals.get_args()
 
-    parser.add_argument(
+    # The "Help" group includes the help option and other informational stuff about the CLI itself
+    outerHelpGroup = parser.add_argument_group('Help')
+    helpGroup = outerHelpGroup.add_mutually_exclusive_group()
+    helpGroup.add_argument("-h", "--help", action="help", help="show this help message and exit")
+
+    the_version = get_active_version()
+    helpGroup.add_argument("--version", action="version", version=f"{the_version}")
+
+    helpGroup.add_argument(
+        "--support",
+        action="store_true",
+        help="Show support info (useful when troubleshooting an issue)",
+    )
+
+    # Connection arguments to indicate a device to connect to
+    parser = addConnectionArgs(parser)
+
+    # Arguments concerning viewing and setting configuration
+
+    # Arguments for sending or requesting things from the local device
+
+    # Arguments for sending or requesting things from the mesh
+
+    # All the rest of the arguments
+    group = parser.add_argument_group("optional arguments")
+    group.add_argument(
         "--configure",
         help="Specify a path to a yaml(.yml) file containing the desired settings for the connected device.",
         action="append",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--export-config",
         help="Export the configuration in yaml(.yml) format.",
         action="store_true",
     )
 
-    parser.add_argument(
-        "--port",
-        help="The port the Meshtastic device is connected to, i.e. /dev/ttyUSB0.",
-        default=None,
-    )
-
-    parser.add_argument(
-        "--host",
-        help="The hostname/ipaddr of the device to connect to (over TCP)",
-        default=None,
-    )
-
-    parser.add_argument(
+    group.add_argument(
         "--seriallog",
         help="Log device serial output to either 'stdout', 'none' or a filename to append to.",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--info",
         help="Read and display the radio config information",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--get-canned-message",
         help="Show the canned message plugin message",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--get-ringtone", help="Show the stored ringtone", action="store_true"
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--nodes",
         help="Print Node List in a pretty formatted table",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--qr",
         help="Display the QR code that corresponds to the current channel",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--get",
         help=(
             "Get a preferences field. Use an invalid field such as '0' to get a list of all fields."
             " Can use either snake_case or camelCase format. (ex: 'ls_secs' or 'lsSecs')"
         ),
         nargs=1,
         action="append",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--set",
         help="Set a preferences field. Can use either snake_case or camelCase format. (ex: 'ls_secs' or 'lsSecs')",
         nargs=2,
         action="append",
     )
 
-    parser.add_argument("--seturl", help="Set a channel URL", action="store")
+    group.add_argument("--seturl", help="Set a channel URL", action="store")
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-index",
         help="Set the specified channel index. Channels start at 0 (0 is the PRIMARY channel).",
         action="store",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-add",
         help="Add a secondary channel, you must specify a channel name",
         default=None,
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-del", help="Delete the ch-index channel", action="store_true"
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-enable",
         help="Enable the specified channel",
         action="store_true",
         dest="ch_enable",
         default=False,
     )
 
     # Note: We are doing a double negative here (Do we want to disable? If ch_disable==True, then disable.)
-    parser.add_argument(
+    group.add_argument(
         "--ch-disable",
         help="Disable the specified channel",
         action="store_true",
         dest="ch_disable",
         default=False,
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-set",
         help=(
             "Set a channel parameter. To see channel settings available:'--ch-set all all --ch-index 0'. "
             "Can set the 'psk' using this command. To disable encryption on primary channel:'--ch-set psk none --ch-index 0'. "
             "To set encryption with a new random key on second channel:'--ch-set psk random --ch-index 1'. "
             "To set encryption back to the default:'--ch-set psk default --ch-index 0'. To set encryption with your "
             "own key: '--ch-set psk 0x1a1a1a1a2b2b2b2b1a1a1a1a2b2b2b2b1a1a1a1a2b2b2b2b1a1a1a1a2b2b2b2b --ch-index 0'."
         ),
         nargs=2,
         action="append",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-vlongslow",
         help="Change to the very long-range and slow channel",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-longslow",
         help="Change to the long-range and slow channel",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-longfast",
         help="Change to the long-range and fast channel",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-medslow",
         help="Change to the med-range and slow channel",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-medfast",
         help="Change to the med-range and fast channel",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-shortslow",
         help="Change to the short-range and slow channel",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ch-shortfast",
         help="Change to the short-range and fast channel",
         action="store_true",
     )
 
-    parser.add_argument("--set-owner", help="Set device owner name", action="store")
+    group.add_argument("--set-owner", help="Set device owner name", action="store")
 
-    parser.add_argument(
+    group.add_argument(
         "--set-canned-message",
         help="Set the canned messages plugin message (up to 200 characters).",
         action="store",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--set-ringtone",
         help="Set the Notification Ringtone (up to 230 characters).",
         action="store",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--set-owner-short", help="Set device owner short name", action="store"
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--set-ham", help="Set licensed Ham ID and turn off encryption", action="store"
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--dest",
         help="The destination node id for any sent commands, if not set '^all' or '^local' is assumed as appropriate",
         default=None,
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--sendtext",
         help="Send a text message. Can specify a destination '--dest' and/or channel index '--ch-index'.",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--traceroute",
         help="Traceroute from connected node to a destination. "
         "You need pass the destination ID as argument, like "
         "this: '--traceroute !ba4bf9d0' "
         "Only nodes that have the encryption key can be traced.",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--request-telemetry", 
         help="Request telemetry from a node. "
         "You need pass the destination ID as argument with '--dest'. "
         "For repeaters, the nodeNum is required.",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--ack",
         help="Use in combination with --sendtext to wait for an acknowledgment.",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--reboot", help="Tell the destination node to reboot", action="store_true"
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--reboot-ota",
         help="Tell the destination node to reboot into factory firmware",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--shutdown", help="Tell the destination node to shutdown", action="store_true"
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--device-metadata",
         help="Get the device metadata from the node",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--begin-edit",
         help="Tell the node to open a transaction to edit settings",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--commit-edit",
         help="Tell the node to commit open settings transaction",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--factory-reset",
         help="Tell the destination node to install the default config",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--reset-nodedb",
         help="Tell the destination node clear its list of nodes",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--reply", help="Reply to received messages", action="store_true"
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--gpio-wrb", nargs=2, help="Set a particular GPIO # to 1 or 0", action="append"
     )
 
-    parser.add_argument("--gpio-rd", help="Read from a GPIO mask (ex: '0x10')")
+    group.add_argument("--gpio-rd", help="Read from a GPIO mask (ex: '0x10')")
 
-    parser.add_argument(
+    group.add_argument(
         "--gpio-watch", help="Start watching a GPIO mask for changes (ex: '0x10')"
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--no-time",
         help="Suppress sending the current time to the mesh",
         action="store_true",
     )
 
-    parser.add_argument("--setalt", help="Set device altitude (allows use without GPS)")
+    group.add_argument("--setalt", help="Set device altitude in meters (allows use without GPS)")
 
-    parser.add_argument("--setlat", help="Set device latitude (allows use without GPS)")
+    group.add_argument("--setlat", help="Set device latitude (allows use without GPS)")
 
-    parser.add_argument(
+    group.add_argument(
         "--setlon", help="Set device longitude (allows use without GPS)"
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--pos-fields",
         help="Specify fields to send when sending a position. Use no argument for a list of valid values. "
         "Can pass multiple values as a space separated list like "
         "this: '--pos-fields POS_ALTITUDE POS_ALT_MSL'",
         nargs="*",
         action="store",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--debug", help="Show API library debug log messages", action="store_true"
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--test",
         help="Run stress test against all connected Meshtastic devices",
         action="store_true",
     )
 
-    parser.add_argument(
-        "--ble",
-        help="BLE device address or name to connect to",
-        default=None,
-    )
-    parser.add_argument(
+    group.add_argument(
         "--ble-scan",
         help="Scan for Meshtastic BLE devices",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--noproto",
         help="Don't start the API, just function as a dumb serial terminal.",
         action="store_true",
     )
 
-    parser.add_argument(
+    group.add_argument(
         "--listen",
-        help="Just stay open and listen to the protobuf stream.",
+        help="Just stay open and listen to the protobuf stream. Enables debug logging.",
         action="store_true",
     )
 
     have_tunnel = platform.system() == "Linux"
     if have_tunnel:
-        parser.add_argument(
+        tunnelArgs = parser.add_argument_group('Tunnel', 'Arguments related to establishing a tunnel device over the mesh.')
+        tunnelArgs.add_argument(
             "--tunnel",
             action="store_true",
             help="Create a TUN tunnel device for forwarding IP packets over the mesh",
         )
-        parser.add_argument(
+        tunnelArgs.add_argument(
             "--subnet",
             dest="tunnel_net",
             help="Sets the local-end subnet address for the TUN IP bridge. (ex: 10.115' which is the default)",
             default=None,
         )
 
     parser.set_defaults(deprecated=None)
 
-    the_version = get_active_version()
-    parser.add_argument("--version", action="version", version=f"{the_version}")
-
-    parser.add_argument(
-        "--support",
-        action="store_true",
-        help="Show support info (useful when troubleshooting an issue)",
-    )
 
     args = parser.parse_args()
     our_globals.set_args(args)
     our_globals.set_parser(parser)
 
 
 def main():
     """Perform command line meshtastic operations"""
     our_globals = Globals.getInstance()
     parser = argparse.ArgumentParser(
-        epilog="If neither --port nor --host are specified, we search for a compatible serial device, "
+        add_help=False,
+        epilog="If no connection arguments are specified, we search for a compatible serial device, "
                "and if none is found, then attempt a TCP connection to localhost.")
     our_globals.set_parser(parser)
     initParser()
     common()
     logfile = our_globals.get_logfile()
     if logfile:
         logfile.close()
 
 
 def tunnelMain():
     """Run a meshtastic IP tunnel"""
     our_globals = Globals.getInstance()
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(add_help=False)
     our_globals.set_parser(parser)
     initParser()
     args = our_globals.get_args()
     args.tunnel = True
     our_globals.set_args(args)
     common()
```

### Comparing `meshtastic-2.3.3/meshtastic/admin_pb2.py` & `meshtastic-2.3.4/meshtastic/admin_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 from meshtastic import channel_pb2 as meshtastic_dot_channel__pb2
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
 from meshtastic import connection_status_pb2 as meshtastic_dot_connection__status__pb2
 from meshtastic import mesh_pb2 as meshtastic_dot_mesh__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16meshtastic/admin.proto\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\"meshtastic/connection_status.proto\x1a\x15meshtastic/mesh.proto\x1a\x1emeshtastic/module_config.proto\"\xa9\x10\n\x0c\x41\x64minMessage\x12\x1d\n\x13get_channel_request\x18\x01 \x01(\rH\x00\x12(\n\x14get_channel_response\x18\x02 \x01(\x0b\x32\x08.ChannelH\x00\x12\x1b\n\x11get_owner_request\x18\x03 \x01(\x08H\x00\x12#\n\x12get_owner_response\x18\x04 \x01(\x0b\x32\x05.UserH\x00\x12\x36\n\x12get_config_request\x18\x05 \x01(\x0e\x32\x18.AdminMessage.ConfigTypeH\x00\x12&\n\x13get_config_response\x18\x06 \x01(\x0b\x32\x07.ConfigH\x00\x12\x43\n\x19get_module_config_request\x18\x07 \x01(\x0e\x32\x1e.AdminMessage.ModuleConfigTypeH\x00\x12\x33\n\x1aget_module_config_response\x18\x08 \x01(\x0b\x32\r.ModuleConfigH\x00\x12\x34\n*get_canned_message_module_messages_request\x18\n \x01(\x08H\x00\x12\x35\n+get_canned_message_module_messages_response\x18\x0b \x01(\tH\x00\x12%\n\x1bget_device_metadata_request\x18\x0c \x01(\x08H\x00\x12\x37\n\x1cget_device_metadata_response\x18\r \x01(\x0b\x32\x0f.DeviceMetadataH\x00\x12\x1e\n\x14get_ringtone_request\x18\x0e \x01(\x08H\x00\x12\x1f\n\x15get_ringtone_response\x18\x0f \x01(\tH\x00\x12.\n$get_device_connection_status_request\x18\x10 \x01(\x08H\x00\x12H\n%get_device_connection_status_response\x18\x11 \x01(\x0b\x32\x17.DeviceConnectionStatusH\x00\x12&\n\x0cset_ham_mode\x18\x12 \x01(\x0b\x32\x0e.HamParametersH\x00\x12/\n%get_node_remote_hardware_pins_request\x18\x13 \x01(\x08H\x00\x12Q\n&get_node_remote_hardware_pins_response\x18\x14 \x01(\x0b\x32\x1f.NodeRemoteHardwarePinsResponseH\x00\x12 \n\x16\x65nter_dfu_mode_request\x18\x15 \x01(\x08H\x00\x12\x1d\n\x13\x64\x65lete_file_request\x18\x16 \x01(\tH\x00\x12\x1a\n\tset_owner\x18  \x01(\x0b\x32\x05.UserH\x00\x12\x1f\n\x0bset_channel\x18! \x01(\x0b\x32\x08.ChannelH\x00\x12\x1d\n\nset_config\x18\" \x01(\x0b\x32\x07.ConfigH\x00\x12*\n\x11set_module_config\x18# \x01(\x0b\x32\r.ModuleConfigH\x00\x12,\n\"set_canned_message_module_messages\x18$ \x01(\tH\x00\x12\x1e\n\x14set_ringtone_message\x18% \x01(\tH\x00\x12\x1b\n\x11remove_by_nodenum\x18& \x01(\rH\x00\x12\x1b\n\x11set_favorite_node\x18\' \x01(\rH\x00\x12\x1e\n\x14remove_favorite_node\x18( \x01(\rH\x00\x12\'\n\x12set_fixed_position\x18) \x01(\x0b\x32\t.PositionH\x00\x12\x1f\n\x15remove_fixed_position\x18* \x01(\x08H\x00\x12\x1d\n\x13\x62\x65gin_edit_settings\x18@ \x01(\x08H\x00\x12\x1e\n\x14\x63ommit_edit_settings\x18\x41 \x01(\x08H\x00\x12\x1c\n\x12reboot_ota_seconds\x18_ \x01(\x05H\x00\x12\x18\n\x0e\x65xit_simulator\x18` \x01(\x08H\x00\x12\x18\n\x0ereboot_seconds\x18\x61 \x01(\x05H\x00\x12\x1a\n\x10shutdown_seconds\x18\x62 \x01(\x05H\x00\x12\x17\n\rfactory_reset\x18\x63 \x01(\x05H\x00\x12\x16\n\x0cnodedb_reset\x18\x64 \x01(\x05H\x00\"\x95\x01\n\nConfigType\x12\x11\n\rDEVICE_CONFIG\x10\x00\x12\x13\n\x0fPOSITION_CONFIG\x10\x01\x12\x10\n\x0cPOWER_CONFIG\x10\x02\x12\x12\n\x0eNETWORK_CONFIG\x10\x03\x12\x12\n\x0e\x44ISPLAY_CONFIG\x10\x04\x12\x0f\n\x0bLORA_CONFIG\x10\x05\x12\x14\n\x10\x42LUETOOTH_CONFIG\x10\x06\"\xbb\x02\n\x10ModuleConfigType\x12\x0f\n\x0bMQTT_CONFIG\x10\x00\x12\x11\n\rSERIAL_CONFIG\x10\x01\x12\x13\n\x0f\x45XTNOTIF_CONFIG\x10\x02\x12\x17\n\x13STOREFORWARD_CONFIG\x10\x03\x12\x14\n\x10RANGETEST_CONFIG\x10\x04\x12\x14\n\x10TELEMETRY_CONFIG\x10\x05\x12\x14\n\x10\x43\x41NNEDMSG_CONFIG\x10\x06\x12\x10\n\x0c\x41UDIO_CONFIG\x10\x07\x12\x19\n\x15REMOTEHARDWARE_CONFIG\x10\x08\x12\x17\n\x13NEIGHBORINFO_CONFIG\x10\t\x12\x1a\n\x16\x41MBIENTLIGHTING_CONFIG\x10\n\x12\x1a\n\x16\x44\x45TECTIONSENSOR_CONFIG\x10\x0b\x12\x15\n\x11PAXCOUNTER_CONFIG\x10\x0c\x42\x11\n\x0fpayload_variant\"[\n\rHamParameters\x12\x11\n\tcall_sign\x18\x01 \x01(\t\x12\x10\n\x08tx_power\x18\x02 \x01(\x05\x12\x11\n\tfrequency\x18\x03 \x01(\x02\x12\x12\n\nshort_name\x18\x04 \x01(\t\"[\n\x1eNodeRemoteHardwarePinsResponse\x12\x39\n\x19node_remote_hardware_pins\x18\x01 \x03(\x0b\x32\x16.NodeRemoteHardwarePinB`\n\x13\x63om.geeksville.meshB\x0b\x41\x64minProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16meshtastic/admin.proto\x12\nmeshtastic\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\"meshtastic/connection_status.proto\x1a\x15meshtastic/mesh.proto\x1a\x1emeshtastic/module_config.proto\"\xce\x11\n\x0c\x41\x64minMessage\x12\x1d\n\x13get_channel_request\x18\x01 \x01(\rH\x00\x12\x33\n\x14get_channel_response\x18\x02 \x01(\x0b\x32\x13.meshtastic.ChannelH\x00\x12\x1b\n\x11get_owner_request\x18\x03 \x01(\x08H\x00\x12.\n\x12get_owner_response\x18\x04 \x01(\x0b\x32\x10.meshtastic.UserH\x00\x12\x41\n\x12get_config_request\x18\x05 \x01(\x0e\x32#.meshtastic.AdminMessage.ConfigTypeH\x00\x12\x31\n\x13get_config_response\x18\x06 \x01(\x0b\x32\x12.meshtastic.ConfigH\x00\x12N\n\x19get_module_config_request\x18\x07 \x01(\x0e\x32).meshtastic.AdminMessage.ModuleConfigTypeH\x00\x12>\n\x1aget_module_config_response\x18\x08 \x01(\x0b\x32\x18.meshtastic.ModuleConfigH\x00\x12\x34\n*get_canned_message_module_messages_request\x18\n \x01(\x08H\x00\x12\x35\n+get_canned_message_module_messages_response\x18\x0b \x01(\tH\x00\x12%\n\x1bget_device_metadata_request\x18\x0c \x01(\x08H\x00\x12\x42\n\x1cget_device_metadata_response\x18\r \x01(\x0b\x32\x1a.meshtastic.DeviceMetadataH\x00\x12\x1e\n\x14get_ringtone_request\x18\x0e \x01(\x08H\x00\x12\x1f\n\x15get_ringtone_response\x18\x0f \x01(\tH\x00\x12.\n$get_device_connection_status_request\x18\x10 \x01(\x08H\x00\x12S\n%get_device_connection_status_response\x18\x11 \x01(\x0b\x32\".meshtastic.DeviceConnectionStatusH\x00\x12\x31\n\x0cset_ham_mode\x18\x12 \x01(\x0b\x32\x19.meshtastic.HamParametersH\x00\x12/\n%get_node_remote_hardware_pins_request\x18\x13 \x01(\x08H\x00\x12\\\n&get_node_remote_hardware_pins_response\x18\x14 \x01(\x0b\x32*.meshtastic.NodeRemoteHardwarePinsResponseH\x00\x12 \n\x16\x65nter_dfu_mode_request\x18\x15 \x01(\x08H\x00\x12\x1d\n\x13\x64\x65lete_file_request\x18\x16 \x01(\tH\x00\x12%\n\tset_owner\x18  \x01(\x0b\x32\x10.meshtastic.UserH\x00\x12*\n\x0bset_channel\x18! \x01(\x0b\x32\x13.meshtastic.ChannelH\x00\x12(\n\nset_config\x18\" \x01(\x0b\x32\x12.meshtastic.ConfigH\x00\x12\x35\n\x11set_module_config\x18# \x01(\x0b\x32\x18.meshtastic.ModuleConfigH\x00\x12,\n\"set_canned_message_module_messages\x18$ \x01(\tH\x00\x12\x1e\n\x14set_ringtone_message\x18% \x01(\tH\x00\x12\x1b\n\x11remove_by_nodenum\x18& \x01(\rH\x00\x12\x1b\n\x11set_favorite_node\x18\' \x01(\rH\x00\x12\x1e\n\x14remove_favorite_node\x18( \x01(\rH\x00\x12\x32\n\x12set_fixed_position\x18) \x01(\x0b\x32\x14.meshtastic.PositionH\x00\x12\x1f\n\x15remove_fixed_position\x18* \x01(\x08H\x00\x12\x1d\n\x13\x62\x65gin_edit_settings\x18@ \x01(\x08H\x00\x12\x1e\n\x14\x63ommit_edit_settings\x18\x41 \x01(\x08H\x00\x12\x1c\n\x12reboot_ota_seconds\x18_ \x01(\x05H\x00\x12\x18\n\x0e\x65xit_simulator\x18` \x01(\x08H\x00\x12\x18\n\x0ereboot_seconds\x18\x61 \x01(\x05H\x00\x12\x1a\n\x10shutdown_seconds\x18\x62 \x01(\x05H\x00\x12\x17\n\rfactory_reset\x18\x63 \x01(\x05H\x00\x12\x16\n\x0cnodedb_reset\x18\x64 \x01(\x05H\x00\"\x95\x01\n\nConfigType\x12\x11\n\rDEVICE_CONFIG\x10\x00\x12\x13\n\x0fPOSITION_CONFIG\x10\x01\x12\x10\n\x0cPOWER_CONFIG\x10\x02\x12\x12\n\x0eNETWORK_CONFIG\x10\x03\x12\x12\n\x0e\x44ISPLAY_CONFIG\x10\x04\x12\x0f\n\x0bLORA_CONFIG\x10\x05\x12\x14\n\x10\x42LUETOOTH_CONFIG\x10\x06\"\xbb\x02\n\x10ModuleConfigType\x12\x0f\n\x0bMQTT_CONFIG\x10\x00\x12\x11\n\rSERIAL_CONFIG\x10\x01\x12\x13\n\x0f\x45XTNOTIF_CONFIG\x10\x02\x12\x17\n\x13STOREFORWARD_CONFIG\x10\x03\x12\x14\n\x10RANGETEST_CONFIG\x10\x04\x12\x14\n\x10TELEMETRY_CONFIG\x10\x05\x12\x14\n\x10\x43\x41NNEDMSG_CONFIG\x10\x06\x12\x10\n\x0c\x41UDIO_CONFIG\x10\x07\x12\x19\n\x15REMOTEHARDWARE_CONFIG\x10\x08\x12\x17\n\x13NEIGHBORINFO_CONFIG\x10\t\x12\x1a\n\x16\x41MBIENTLIGHTING_CONFIG\x10\n\x12\x1a\n\x16\x44\x45TECTIONSENSOR_CONFIG\x10\x0b\x12\x15\n\x11PAXCOUNTER_CONFIG\x10\x0c\x42\x11\n\x0fpayload_variant\"[\n\rHamParameters\x12\x11\n\tcall_sign\x18\x01 \x01(\t\x12\x10\n\x08tx_power\x18\x02 \x01(\x05\x12\x11\n\tfrequency\x18\x03 \x01(\x02\x12\x12\n\nshort_name\x18\x04 \x01(\t\"f\n\x1eNodeRemoteHardwarePinsResponse\x12\x44\n\x19node_remote_hardware_pins\x18\x01 \x03(\x0b\x32!.meshtastic.NodeRemoteHardwarePinB`\n\x13\x63om.geeksville.meshB\x0b\x41\x64minProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.admin_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\013AdminProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _ADMINMESSAGE._serialized_start=169
-  _ADMINMESSAGE._serialized_end=2258
-  _ADMINMESSAGE_CONFIGTYPE._serialized_start=1772
-  _ADMINMESSAGE_CONFIGTYPE._serialized_end=1921
-  _ADMINMESSAGE_MODULECONFIGTYPE._serialized_start=1924
-  _ADMINMESSAGE_MODULECONFIGTYPE._serialized_end=2239
-  _HAMPARAMETERS._serialized_start=2260
-  _HAMPARAMETERS._serialized_end=2351
-  _NODEREMOTEHARDWAREPINSRESPONSE._serialized_start=2353
-  _NODEREMOTEHARDWAREPINSRESPONSE._serialized_end=2444
+  _ADMINMESSAGE._serialized_start=181
+  _ADMINMESSAGE._serialized_end=2435
+  _ADMINMESSAGE_CONFIGTYPE._serialized_start=1949
+  _ADMINMESSAGE_CONFIGTYPE._serialized_end=2098
+  _ADMINMESSAGE_MODULECONFIGTYPE._serialized_start=2101
+  _ADMINMESSAGE_MODULECONFIGTYPE._serialized_end=2416
+  _HAMPARAMETERS._serialized_start=2437
+  _HAMPARAMETERS._serialized_end=2528
+  _NODEREMOTEHARDWAREPINSRESPONSE._serialized_start=2530
+  _NODEREMOTEHARDWAREPINSRESPONSE._serialized_end=2632
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/apponly_pb2.py` & `meshtastic-2.3.4/meshtastic/apponly_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 _sym_db = _symbol_database.Default()
 
 
 from meshtastic import channel_pb2 as meshtastic_dot_channel__pb2
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18meshtastic/apponly.proto\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\"Y\n\nChannelSet\x12\"\n\x08settings\x18\x01 \x03(\x0b\x32\x10.ChannelSettings\x12\'\n\x0blora_config\x18\x02 \x01(\x0b\x32\x12.Config.LoRaConfigBb\n\x13\x63om.geeksville.meshB\rAppOnlyProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18meshtastic/apponly.proto\x12\nmeshtastic\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\"o\n\nChannelSet\x12-\n\x08settings\x18\x01 \x03(\x0b\x32\x1b.meshtastic.ChannelSettings\x12\x32\n\x0blora_config\x18\x02 \x01(\x0b\x32\x1d.meshtastic.Config.LoRaConfigBb\n\x13\x63om.geeksville.meshB\rAppOnlyProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.apponly_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\rAppOnlyProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _CHANNELSET._serialized_start=79
-  _CHANNELSET._serialized_end=168
+  _CHANNELSET._serialized_start=91
+  _CHANNELSET._serialized_end=202
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/atak_pb2.py` & `meshtastic-2.3.4/meshtastic/atak_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/atak.proto\"\xaf\x01\n\tTAKPacket\x12\x15\n\ris_compressed\x18\x01 \x01(\x08\x12\x19\n\x07\x63ontact\x18\x02 \x01(\x0b\x32\x08.Contact\x12\x15\n\x05group\x18\x03 \x01(\x0b\x32\x06.Group\x12\x17\n\x06status\x18\x04 \x01(\x0b\x32\x07.Status\x12\x13\n\x03pli\x18\x05 \x01(\x0b\x32\x04.PLIH\x00\x12\x18\n\x04\x63hat\x18\x06 \x01(\x0b\x32\x08.GeoChatH\x00\x42\x11\n\x0fpayload_variant\"2\n\x07GeoChat\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0f\n\x02to\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x05\n\x03_to\"7\n\x05Group\x12\x19\n\x04role\x18\x01 \x01(\x0e\x32\x0b.MemberRole\x12\x13\n\x04team\x18\x02 \x01(\x0e\x32\x05.Team\"\x19\n\x06Status\x12\x0f\n\x07\x62\x61ttery\x18\x01 \x01(\r\"4\n\x07\x43ontact\x12\x10\n\x08\x63\x61llsign\x18\x01 \x01(\t\x12\x17\n\x0f\x64\x65vice_callsign\x18\x02 \x01(\t\"_\n\x03PLI\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\r\n\x05speed\x18\x04 \x01(\r\x12\x0e\n\x06\x63ourse\x18\x05 \x01(\r*\xc0\x01\n\x04Team\x12\x14\n\x10Unspecifed_Color\x10\x00\x12\t\n\x05White\x10\x01\x12\n\n\x06Yellow\x10\x02\x12\n\n\x06Orange\x10\x03\x12\x0b\n\x07Magenta\x10\x04\x12\x07\n\x03Red\x10\x05\x12\n\n\x06Maroon\x10\x06\x12\n\n\x06Purple\x10\x07\x12\r\n\tDark_Blue\x10\x08\x12\x08\n\x04\x42lue\x10\t\x12\x08\n\x04\x43yan\x10\n\x12\x08\n\x04Teal\x10\x0b\x12\t\n\x05Green\x10\x0c\x12\x0e\n\nDark_Green\x10\r\x12\t\n\x05\x42rown\x10\x0e*\x7f\n\nMemberRole\x12\x0e\n\nUnspecifed\x10\x00\x12\x0e\n\nTeamMember\x10\x01\x12\x0c\n\x08TeamLead\x10\x02\x12\x06\n\x02HQ\x10\x03\x12\n\n\x06Sniper\x10\x04\x12\t\n\x05Medic\x10\x05\x12\x13\n\x0f\x46orwardObserver\x10\x06\x12\x07\n\x03RTO\x10\x07\x12\x06\n\x02K9\x10\x08\x42_\n\x13\x63om.geeksville.meshB\nATAKProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/atak.proto\x12\nmeshtastic\"\xe6\x01\n\tTAKPacket\x12\x15\n\ris_compressed\x18\x01 \x01(\x08\x12$\n\x07\x63ontact\x18\x02 \x01(\x0b\x32\x13.meshtastic.Contact\x12 \n\x05group\x18\x03 \x01(\x0b\x32\x11.meshtastic.Group\x12\"\n\x06status\x18\x04 \x01(\x0b\x32\x12.meshtastic.Status\x12\x1e\n\x03pli\x18\x05 \x01(\x0b\x32\x0f.meshtastic.PLIH\x00\x12#\n\x04\x63hat\x18\x06 \x01(\x0b\x32\x13.meshtastic.GeoChatH\x00\x42\x11\n\x0fpayload_variant\"2\n\x07GeoChat\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0f\n\x02to\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x05\n\x03_to\"M\n\x05Group\x12$\n\x04role\x18\x01 \x01(\x0e\x32\x16.meshtastic.MemberRole\x12\x1e\n\x04team\x18\x02 \x01(\x0e\x32\x10.meshtastic.Team\"\x19\n\x06Status\x12\x0f\n\x07\x62\x61ttery\x18\x01 \x01(\r\"4\n\x07\x43ontact\x12\x10\n\x08\x63\x61llsign\x18\x01 \x01(\t\x12\x17\n\x0f\x64\x65vice_callsign\x18\x02 \x01(\t\"_\n\x03PLI\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\r\n\x05speed\x18\x04 \x01(\r\x12\x0e\n\x06\x63ourse\x18\x05 \x01(\r*\xc0\x01\n\x04Team\x12\x14\n\x10Unspecifed_Color\x10\x00\x12\t\n\x05White\x10\x01\x12\n\n\x06Yellow\x10\x02\x12\n\n\x06Orange\x10\x03\x12\x0b\n\x07Magenta\x10\x04\x12\x07\n\x03Red\x10\x05\x12\n\n\x06Maroon\x10\x06\x12\n\n\x06Purple\x10\x07\x12\r\n\tDark_Blue\x10\x08\x12\x08\n\x04\x42lue\x10\t\x12\x08\n\x04\x43yan\x10\n\x12\x08\n\x04Teal\x10\x0b\x12\t\n\x05Green\x10\x0c\x12\x0e\n\nDark_Green\x10\r\x12\t\n\x05\x42rown\x10\x0e*\x7f\n\nMemberRole\x12\x0e\n\nUnspecifed\x10\x00\x12\x0e\n\nTeamMember\x10\x01\x12\x0c\n\x08TeamLead\x10\x02\x12\x06\n\x02HQ\x10\x03\x12\n\n\x06Sniper\x10\x04\x12\t\n\x05Medic\x10\x05\x12\x13\n\x0f\x46orwardObserver\x10\x06\x12\x07\n\x03RTO\x10\x07\x12\x06\n\x02K9\x10\x08\x42_\n\x13\x63om.geeksville.meshB\nATAKProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.atak_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\nATAKProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _TEAM._serialized_start=491
-  _TEAM._serialized_end=683
-  _MEMBERROLE._serialized_start=685
-  _MEMBERROLE._serialized_end=812
-  _TAKPACKET._serialized_start=26
-  _TAKPACKET._serialized_end=201
-  _GEOCHAT._serialized_start=203
-  _GEOCHAT._serialized_end=253
-  _GROUP._serialized_start=255
-  _GROUP._serialized_end=310
-  _STATUS._serialized_start=312
-  _STATUS._serialized_end=337
-  _CONTACT._serialized_start=339
-  _CONTACT._serialized_end=391
-  _PLI._serialized_start=393
-  _PLI._serialized_end=488
+  _TEAM._serialized_start=580
+  _TEAM._serialized_end=772
+  _MEMBERROLE._serialized_start=774
+  _MEMBERROLE._serialized_end=901
+  _TAKPACKET._serialized_start=38
+  _TAKPACKET._serialized_end=268
+  _GEOCHAT._serialized_start=270
+  _GEOCHAT._serialized_end=320
+  _GROUP._serialized_start=322
+  _GROUP._serialized_end=399
+  _STATUS._serialized_start=401
+  _STATUS._serialized_end=426
+  _CONTACT._serialized_start=428
+  _CONTACT._serialized_end=480
+  _PLI._serialized_start=482
+  _PLI._serialized_end=577
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/ble_interface.py` & `meshtastic-2.3.4/meshtastic/ble_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.3/meshtastic/cannedmessages_pb2.py` & `meshtastic-2.3.4/meshtastic/cannedmessages_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fmeshtastic/cannedmessages.proto\"-\n\x19\x43\x61nnedMessageModuleConfig\x12\x10\n\x08messages\x18\x01 \x01(\tBn\n\x13\x63om.geeksville.meshB\x19\x43\x61nnedMessageConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fmeshtastic/cannedmessages.proto\x12\nmeshtastic\"-\n\x19\x43\x61nnedMessageModuleConfig\x12\x10\n\x08messages\x18\x01 \x01(\tBn\n\x13\x63om.geeksville.meshB\x19\x43\x61nnedMessageConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.cannedmessages_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\031CannedMessageConfigProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _CANNEDMESSAGEMODULECONFIG._serialized_start=35
-  _CANNEDMESSAGEMODULECONFIG._serialized_end=80
+  _CANNEDMESSAGEMODULECONFIG._serialized_start=47
+  _CANNEDMESSAGEMODULECONFIG._serialized_end=92
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/channel_pb2.py` & `meshtastic-2.3.4/meshtastic/channel_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18meshtastic/channel.proto\"\xad\x01\n\x0f\x43hannelSettings\x12\x17\n\x0b\x63hannel_num\x18\x01 \x01(\rB\x02\x18\x01\x12\x0b\n\x03psk\x18\x02 \x01(\x0c\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\x07\x12\x16\n\x0euplink_enabled\x18\x05 \x01(\x08\x12\x18\n\x10\x64ownlink_enabled\x18\x06 \x01(\x08\x12(\n\x0fmodule_settings\x18\x07 \x01(\x0b\x32\x0f.ModuleSettings\",\n\x0eModuleSettings\x12\x1a\n\x12position_precision\x18\x01 \x01(\r\"\x8b\x01\n\x07\x43hannel\x12\r\n\x05index\x18\x01 \x01(\x05\x12\"\n\x08settings\x18\x02 \x01(\x0b\x32\x10.ChannelSettings\x12\x1b\n\x04role\x18\x03 \x01(\x0e\x32\r.Channel.Role\"0\n\x04Role\x12\x0c\n\x08\x44ISABLED\x10\x00\x12\x0b\n\x07PRIMARY\x10\x01\x12\r\n\tSECONDARY\x10\x02\x42\x62\n\x13\x63om.geeksville.meshB\rChannelProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18meshtastic/channel.proto\x12\nmeshtastic\"\xb8\x01\n\x0f\x43hannelSettings\x12\x17\n\x0b\x63hannel_num\x18\x01 \x01(\rB\x02\x18\x01\x12\x0b\n\x03psk\x18\x02 \x01(\x0c\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\x07\x12\x16\n\x0euplink_enabled\x18\x05 \x01(\x08\x12\x18\n\x10\x64ownlink_enabled\x18\x06 \x01(\x08\x12\x33\n\x0fmodule_settings\x18\x07 \x01(\x0b\x32\x1a.meshtastic.ModuleSettings\",\n\x0eModuleSettings\x12\x1a\n\x12position_precision\x18\x01 \x01(\r\"\xa1\x01\n\x07\x43hannel\x12\r\n\x05index\x18\x01 \x01(\x05\x12-\n\x08settings\x18\x02 \x01(\x0b\x32\x1b.meshtastic.ChannelSettings\x12&\n\x04role\x18\x03 \x01(\x0e\x32\x18.meshtastic.Channel.Role\"0\n\x04Role\x12\x0c\n\x08\x44ISABLED\x10\x00\x12\x0b\n\x07PRIMARY\x10\x01\x12\r\n\tSECONDARY\x10\x02\x42\x62\n\x13\x63om.geeksville.meshB\rChannelProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.channel_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\rChannelProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _CHANNELSETTINGS.fields_by_name['channel_num']._options = None
   _CHANNELSETTINGS.fields_by_name['channel_num']._serialized_options = b'\030\001'
-  _CHANNELSETTINGS._serialized_start=29
-  _CHANNELSETTINGS._serialized_end=202
-  _MODULESETTINGS._serialized_start=204
-  _MODULESETTINGS._serialized_end=248
-  _CHANNEL._serialized_start=251
-  _CHANNEL._serialized_end=390
-  _CHANNEL_ROLE._serialized_start=342
-  _CHANNEL_ROLE._serialized_end=390
+  _CHANNELSETTINGS._serialized_start=41
+  _CHANNELSETTINGS._serialized_end=225
+  _MODULESETTINGS._serialized_start=227
+  _MODULESETTINGS._serialized_end=271
+  _CHANNEL._serialized_start=274
+  _CHANNEL._serialized_end=435
+  _CHANNEL_ROLE._serialized_start=387
+  _CHANNEL_ROLE._serialized_end=435
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/clientonly_pb2.py` & `meshtastic-2.3.4/meshtastic/clientonly_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from meshtastic import localonly_pb2 as meshtastic_dot_localonly__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bmeshtastic/clientonly.proto\x1a\x1ameshtastic/localonly.proto\"\xf7\x01\n\rDeviceProfile\x12\x16\n\tlong_name\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x17\n\nshort_name\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x0b\x63hannel_url\x18\x03 \x01(\tH\x02\x88\x01\x01\x12!\n\x06\x63onfig\x18\x04 \x01(\x0b\x32\x0c.LocalConfigH\x03\x88\x01\x01\x12.\n\rmodule_config\x18\x05 \x01(\x0b\x32\x12.LocalModuleConfigH\x04\x88\x01\x01\x42\x0c\n\n_long_nameB\r\n\x0b_short_nameB\x0e\n\x0c_channel_urlB\t\n\x07_configB\x10\n\x0e_module_configBe\n\x13\x63om.geeksville.meshB\x10\x43lientOnlyProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bmeshtastic/clientonly.proto\x12\nmeshtastic\x1a\x1ameshtastic/localonly.proto\"\x8d\x02\n\rDeviceProfile\x12\x16\n\tlong_name\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x17\n\nshort_name\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x0b\x63hannel_url\x18\x03 \x01(\tH\x02\x88\x01\x01\x12,\n\x06\x63onfig\x18\x04 \x01(\x0b\x32\x17.meshtastic.LocalConfigH\x03\x88\x01\x01\x12\x39\n\rmodule_config\x18\x05 \x01(\x0b\x32\x1d.meshtastic.LocalModuleConfigH\x04\x88\x01\x01\x42\x0c\n\n_long_nameB\r\n\x0b_short_nameB\x0e\n\x0c_channel_urlB\t\n\x07_configB\x10\n\x0e_module_configBe\n\x13\x63om.geeksville.meshB\x10\x43lientOnlyProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.clientonly_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\020ClientOnlyProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _DEVICEPROFILE._serialized_start=60
-  _DEVICEPROFILE._serialized_end=307
+  _DEVICEPROFILE._serialized_start=72
+  _DEVICEPROFILE._serialized_end=341
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/config_pb2.py` & `meshtastic-2.3.4/meshtastic/config_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,62 +9,62 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17meshtastic/config.proto\"\xc2\x1d\n\x06\x43onfig\x12&\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x14.Config.DeviceConfigH\x00\x12*\n\x08position\x18\x02 \x01(\x0b\x32\x16.Config.PositionConfigH\x00\x12$\n\x05power\x18\x03 \x01(\x0b\x32\x13.Config.PowerConfigH\x00\x12(\n\x07network\x18\x04 \x01(\x0b\x32\x15.Config.NetworkConfigH\x00\x12(\n\x07\x64isplay\x18\x05 \x01(\x0b\x32\x15.Config.DisplayConfigH\x00\x12\"\n\x04lora\x18\x06 \x01(\x0b\x32\x12.Config.LoRaConfigH\x00\x12,\n\tbluetooth\x18\x07 \x01(\x0b\x32\x17.Config.BluetoothConfigH\x00\x1a\xcc\x04\n\x0c\x44\x65viceConfig\x12\'\n\x04role\x18\x01 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eserial_enabled\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x62ug_log_enabled\x18\x03 \x01(\x08\x12\x13\n\x0b\x62utton_gpio\x18\x04 \x01(\r\x12\x13\n\x0b\x62uzzer_gpio\x18\x05 \x01(\r\x12>\n\x10rebroadcast_mode\x18\x06 \x01(\x0e\x32$.Config.DeviceConfig.RebroadcastMode\x12 \n\x18node_info_broadcast_secs\x18\x07 \x01(\r\x12\"\n\x1a\x64ouble_tap_as_button_press\x18\x08 \x01(\x08\x12\x12\n\nis_managed\x18\t \x01(\x08\x12\x1c\n\x14\x64isable_triple_click\x18\n \x01(\x08\"\xaa\x01\n\x04Role\x12\n\n\x06\x43LIENT\x10\x00\x12\x0f\n\x0b\x43LIENT_MUTE\x10\x01\x12\n\n\x06ROUTER\x10\x02\x12\x11\n\rROUTER_CLIENT\x10\x03\x12\x0c\n\x08REPEATER\x10\x04\x12\x0b\n\x07TRACKER\x10\x05\x12\n\n\x06SENSOR\x10\x06\x12\x07\n\x03TAK\x10\x07\x12\x11\n\rCLIENT_HIDDEN\x10\x08\x12\x12\n\x0eLOST_AND_FOUND\x10\t\x12\x0f\n\x0bTAK_TRACKER\x10\n\"Q\n\x0fRebroadcastMode\x12\x07\n\x03\x41LL\x10\x00\x12\x15\n\x11\x41LL_SKIP_DECODING\x10\x01\x12\x0e\n\nLOCAL_ONLY\x10\x02\x12\x0e\n\nKNOWN_ONLY\x10\x03\x1a\x86\x05\n\x0ePositionConfig\x12\x1f\n\x17position_broadcast_secs\x18\x01 \x01(\r\x12(\n position_broadcast_smart_enabled\x18\x02 \x01(\x08\x12\x16\n\x0e\x66ixed_position\x18\x03 \x01(\x08\x12\x17\n\x0bgps_enabled\x18\x04 \x01(\x08\x42\x02\x18\x01\x12\x1b\n\x13gps_update_interval\x18\x05 \x01(\r\x12\x1c\n\x10gps_attempt_time\x18\x06 \x01(\rB\x02\x18\x01\x12\x16\n\x0eposition_flags\x18\x07 \x01(\r\x12\x0f\n\x07rx_gpio\x18\x08 \x01(\r\x12\x0f\n\x07tx_gpio\x18\t \x01(\r\x12(\n broadcast_smart_minimum_distance\x18\n \x01(\r\x12-\n%broadcast_smart_minimum_interval_secs\x18\x0b \x01(\r\x12\x13\n\x0bgps_en_gpio\x18\x0c \x01(\r\x12\x30\n\x08gps_mode\x18\r \x01(\x0e\x32\x1e.Config.PositionConfig.GpsMode\"\xab\x01\n\rPositionFlags\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x41LTITUDE\x10\x01\x12\x10\n\x0c\x41LTITUDE_MSL\x10\x02\x12\x16\n\x12GEOIDAL_SEPARATION\x10\x04\x12\x07\n\x03\x44OP\x10\x08\x12\t\n\x05HVDOP\x10\x10\x12\r\n\tSATINVIEW\x10 \x12\n\n\x06SEQ_NO\x10@\x12\x0e\n\tTIMESTAMP\x10\x80\x01\x12\x0c\n\x07HEADING\x10\x80\x02\x12\n\n\x05SPEED\x10\x80\x04\"5\n\x07GpsMode\x12\x0c\n\x08\x44ISABLED\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0f\n\x0bNOT_PRESENT\x10\x02\x1a\xea\x01\n\x0bPowerConfig\x12\x17\n\x0fis_power_saving\x18\x01 \x01(\x08\x12&\n\x1eon_battery_shutdown_after_secs\x18\x02 \x01(\r\x12\x1f\n\x17\x61\x64\x63_multiplier_override\x18\x03 \x01(\x02\x12\x1b\n\x13wait_bluetooth_secs\x18\x04 \x01(\r\x12\x10\n\x08sds_secs\x18\x06 \x01(\r\x12\x0f\n\x07ls_secs\x18\x07 \x01(\r\x12\x15\n\rmin_wake_secs\x18\x08 \x01(\r\x12\"\n\x1a\x64\x65vice_battery_ina_address\x18\t \x01(\r\x1a\xe8\x02\n\rNetworkConfig\x12\x14\n\x0cwifi_enabled\x18\x01 \x01(\x08\x12\x11\n\twifi_ssid\x18\x03 \x01(\t\x12\x10\n\x08wifi_psk\x18\x04 \x01(\t\x12\x12\n\nntp_server\x18\x05 \x01(\t\x12\x13\n\x0b\x65th_enabled\x18\x06 \x01(\x08\x12\x37\n\x0c\x61\x64\x64ress_mode\x18\x07 \x01(\x0e\x32!.Config.NetworkConfig.AddressMode\x12\x35\n\x0bipv4_config\x18\x08 \x01(\x0b\x32 .Config.NetworkConfig.IpV4Config\x12\x16\n\x0ersyslog_server\x18\t \x01(\t\x1a\x46\n\nIpV4Config\x12\n\n\x02ip\x18\x01 \x01(\x07\x12\x0f\n\x07gateway\x18\x02 \x01(\x07\x12\x0e\n\x06subnet\x18\x03 \x01(\x07\x12\x0b\n\x03\x64ns\x18\x04 \x01(\x07\"#\n\x0b\x41\x64\x64ressMode\x12\x08\n\x04\x44HCP\x10\x00\x12\n\n\x06STATIC\x10\x01\x1a\x92\x05\n\rDisplayConfig\x12\x16\n\x0escreen_on_secs\x18\x01 \x01(\r\x12=\n\ngps_format\x18\x02 \x01(\x0e\x32).Config.DisplayConfig.GpsCoordinateFormat\x12!\n\x19\x61uto_screen_carousel_secs\x18\x03 \x01(\r\x12\x19\n\x11\x63ompass_north_top\x18\x04 \x01(\x08\x12\x13\n\x0b\x66lip_screen\x18\x05 \x01(\x08\x12\x31\n\x05units\x18\x06 \x01(\x0e\x32\".Config.DisplayConfig.DisplayUnits\x12,\n\x04oled\x18\x07 \x01(\x0e\x32\x1e.Config.DisplayConfig.OledType\x12\x36\n\x0b\x64isplaymode\x18\x08 \x01(\x0e\x32!.Config.DisplayConfig.DisplayMode\x12\x14\n\x0cheading_bold\x18\t \x01(\x08\x12\x1d\n\x15wake_on_tap_or_motion\x18\n \x01(\x08\"M\n\x13GpsCoordinateFormat\x12\x07\n\x03\x44\x45\x43\x10\x00\x12\x07\n\x03\x44MS\x10\x01\x12\x07\n\x03UTM\x10\x02\x12\x08\n\x04MGRS\x10\x03\x12\x07\n\x03OLC\x10\x04\x12\x08\n\x04OSGR\x10\x05\"(\n\x0c\x44isplayUnits\x12\n\n\x06METRIC\x10\x00\x12\x0c\n\x08IMPERIAL\x10\x01\"M\n\x08OledType\x12\r\n\tOLED_AUTO\x10\x00\x12\x10\n\x0cOLED_SSD1306\x10\x01\x12\x0f\n\x0bOLED_SH1106\x10\x02\x12\x0f\n\x0bOLED_SH1107\x10\x03\"A\n\x0b\x44isplayMode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x0c\n\x08TWOCOLOR\x10\x01\x12\x0c\n\x08INVERTED\x10\x02\x12\t\n\x05\x43OLOR\x10\x03\x1a\x9a\x06\n\nLoRaConfig\x12\x12\n\nuse_preset\x18\x01 \x01(\x08\x12\x34\n\x0cmodem_preset\x18\x02 \x01(\x0e\x32\x1e.Config.LoRaConfig.ModemPreset\x12\x11\n\tbandwidth\x18\x03 \x01(\r\x12\x15\n\rspread_factor\x18\x04 \x01(\r\x12\x13\n\x0b\x63oding_rate\x18\x05 \x01(\r\x12\x18\n\x10\x66requency_offset\x18\x06 \x01(\x02\x12-\n\x06region\x18\x07 \x01(\x0e\x32\x1d.Config.LoRaConfig.RegionCode\x12\x11\n\thop_limit\x18\x08 \x01(\r\x12\x12\n\ntx_enabled\x18\t \x01(\x08\x12\x10\n\x08tx_power\x18\n \x01(\x05\x12\x13\n\x0b\x63hannel_num\x18\x0b \x01(\r\x12\x1b\n\x13override_duty_cycle\x18\x0c \x01(\x08\x12\x1e\n\x16sx126x_rx_boosted_gain\x18\r \x01(\x08\x12\x1a\n\x12override_frequency\x18\x0e \x01(\x02\x12\x17\n\x0fignore_incoming\x18g \x03(\r\x12\x13\n\x0bignore_mqtt\x18h \x01(\x08\"\xcd\x01\n\nRegionCode\x12\t\n\x05UNSET\x10\x00\x12\x06\n\x02US\x10\x01\x12\n\n\x06\x45U_433\x10\x02\x12\n\n\x06\x45U_868\x10\x03\x12\x06\n\x02\x43N\x10\x04\x12\x06\n\x02JP\x10\x05\x12\x07\n\x03\x41NZ\x10\x06\x12\x06\n\x02KR\x10\x07\x12\x06\n\x02TW\x10\x08\x12\x06\n\x02RU\x10\t\x12\x06\n\x02IN\x10\n\x12\n\n\x06NZ_865\x10\x0b\x12\x06\n\x02TH\x10\x0c\x12\x0b\n\x07LORA_24\x10\r\x12\n\n\x06UA_433\x10\x0e\x12\n\n\x06UA_868\x10\x0f\x12\n\n\x06MY_433\x10\x10\x12\n\n\x06MY_919\x10\x11\x12\n\n\x06SG_923\x10\x12\"\x94\x01\n\x0bModemPreset\x12\r\n\tLONG_FAST\x10\x00\x12\r\n\tLONG_SLOW\x10\x01\x12\x12\n\x0eVERY_LONG_SLOW\x10\x02\x12\x0f\n\x0bMEDIUM_SLOW\x10\x03\x12\x0f\n\x0bMEDIUM_FAST\x10\x04\x12\x0e\n\nSHORT_SLOW\x10\x05\x12\x0e\n\nSHORT_FAST\x10\x06\x12\x11\n\rLONG_MODERATE\x10\x07\x1a\xa2\x01\n\x0f\x42luetoothConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x31\n\x04mode\x18\x02 \x01(\x0e\x32#.Config.BluetoothConfig.PairingMode\x12\x11\n\tfixed_pin\x18\x03 \x01(\r\"8\n\x0bPairingMode\x12\x0e\n\nRANDOM_PIN\x10\x00\x12\r\n\tFIXED_PIN\x10\x01\x12\n\n\x06NO_PIN\x10\x02\x42\x11\n\x0fpayload_variantBa\n\x13\x63om.geeksville.meshB\x0c\x43onfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17meshtastic/config.proto\x12\nmeshtastic\"\xa2\x1f\n\x06\x43onfig\x12\x31\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x1f.meshtastic.Config.DeviceConfigH\x00\x12\x35\n\x08position\x18\x02 \x01(\x0b\x32!.meshtastic.Config.PositionConfigH\x00\x12/\n\x05power\x18\x03 \x01(\x0b\x32\x1e.meshtastic.Config.PowerConfigH\x00\x12\x33\n\x07network\x18\x04 \x01(\x0b\x32 .meshtastic.Config.NetworkConfigH\x00\x12\x33\n\x07\x64isplay\x18\x05 \x01(\x0b\x32 .meshtastic.Config.DisplayConfigH\x00\x12-\n\x04lora\x18\x06 \x01(\x0b\x32\x1d.meshtastic.Config.LoRaConfigH\x00\x12\x37\n\tbluetooth\x18\x07 \x01(\x0b\x32\".meshtastic.Config.BluetoothConfigH\x00\x1a\xf1\x04\n\x0c\x44\x65viceConfig\x12\x32\n\x04role\x18\x01 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\x12\x16\n\x0eserial_enabled\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x62ug_log_enabled\x18\x03 \x01(\x08\x12\x13\n\x0b\x62utton_gpio\x18\x04 \x01(\r\x12\x13\n\x0b\x62uzzer_gpio\x18\x05 \x01(\r\x12I\n\x10rebroadcast_mode\x18\x06 \x01(\x0e\x32/.meshtastic.Config.DeviceConfig.RebroadcastMode\x12 \n\x18node_info_broadcast_secs\x18\x07 \x01(\r\x12\"\n\x1a\x64ouble_tap_as_button_press\x18\x08 \x01(\x08\x12\x12\n\nis_managed\x18\t \x01(\x08\x12\x1c\n\x14\x64isable_triple_click\x18\n \x01(\x08\x12\r\n\x05tzdef\x18\x0b \x01(\t\"\xaa\x01\n\x04Role\x12\n\n\x06\x43LIENT\x10\x00\x12\x0f\n\x0b\x43LIENT_MUTE\x10\x01\x12\n\n\x06ROUTER\x10\x02\x12\x11\n\rROUTER_CLIENT\x10\x03\x12\x0c\n\x08REPEATER\x10\x04\x12\x0b\n\x07TRACKER\x10\x05\x12\n\n\x06SENSOR\x10\x06\x12\x07\n\x03TAK\x10\x07\x12\x11\n\rCLIENT_HIDDEN\x10\x08\x12\x12\n\x0eLOST_AND_FOUND\x10\t\x12\x0f\n\x0bTAK_TRACKER\x10\n\"Q\n\x0fRebroadcastMode\x12\x07\n\x03\x41LL\x10\x00\x12\x15\n\x11\x41LL_SKIP_DECODING\x10\x01\x12\x0e\n\nLOCAL_ONLY\x10\x02\x12\x0e\n\nKNOWN_ONLY\x10\x03\x1a\x91\x05\n\x0ePositionConfig\x12\x1f\n\x17position_broadcast_secs\x18\x01 \x01(\r\x12(\n position_broadcast_smart_enabled\x18\x02 \x01(\x08\x12\x16\n\x0e\x66ixed_position\x18\x03 \x01(\x08\x12\x17\n\x0bgps_enabled\x18\x04 \x01(\x08\x42\x02\x18\x01\x12\x1b\n\x13gps_update_interval\x18\x05 \x01(\r\x12\x1c\n\x10gps_attempt_time\x18\x06 \x01(\rB\x02\x18\x01\x12\x16\n\x0eposition_flags\x18\x07 \x01(\r\x12\x0f\n\x07rx_gpio\x18\x08 \x01(\r\x12\x0f\n\x07tx_gpio\x18\t \x01(\r\x12(\n broadcast_smart_minimum_distance\x18\n \x01(\r\x12-\n%broadcast_smart_minimum_interval_secs\x18\x0b \x01(\r\x12\x13\n\x0bgps_en_gpio\x18\x0c \x01(\r\x12;\n\x08gps_mode\x18\r \x01(\x0e\x32).meshtastic.Config.PositionConfig.GpsMode\"\xab\x01\n\rPositionFlags\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x41LTITUDE\x10\x01\x12\x10\n\x0c\x41LTITUDE_MSL\x10\x02\x12\x16\n\x12GEOIDAL_SEPARATION\x10\x04\x12\x07\n\x03\x44OP\x10\x08\x12\t\n\x05HVDOP\x10\x10\x12\r\n\tSATINVIEW\x10 \x12\n\n\x06SEQ_NO\x10@\x12\x0e\n\tTIMESTAMP\x10\x80\x01\x12\x0c\n\x07HEADING\x10\x80\x02\x12\n\n\x05SPEED\x10\x80\x04\"5\n\x07GpsMode\x12\x0c\n\x08\x44ISABLED\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0f\n\x0bNOT_PRESENT\x10\x02\x1a\xea\x01\n\x0bPowerConfig\x12\x17\n\x0fis_power_saving\x18\x01 \x01(\x08\x12&\n\x1eon_battery_shutdown_after_secs\x18\x02 \x01(\r\x12\x1f\n\x17\x61\x64\x63_multiplier_override\x18\x03 \x01(\x02\x12\x1b\n\x13wait_bluetooth_secs\x18\x04 \x01(\r\x12\x10\n\x08sds_secs\x18\x06 \x01(\r\x12\x0f\n\x07ls_secs\x18\x07 \x01(\r\x12\x15\n\rmin_wake_secs\x18\x08 \x01(\r\x12\"\n\x1a\x64\x65vice_battery_ina_address\x18\t \x01(\r\x1a\xfe\x02\n\rNetworkConfig\x12\x14\n\x0cwifi_enabled\x18\x01 \x01(\x08\x12\x11\n\twifi_ssid\x18\x03 \x01(\t\x12\x10\n\x08wifi_psk\x18\x04 \x01(\t\x12\x12\n\nntp_server\x18\x05 \x01(\t\x12\x13\n\x0b\x65th_enabled\x18\x06 \x01(\x08\x12\x42\n\x0c\x61\x64\x64ress_mode\x18\x07 \x01(\x0e\x32,.meshtastic.Config.NetworkConfig.AddressMode\x12@\n\x0bipv4_config\x18\x08 \x01(\x0b\x32+.meshtastic.Config.NetworkConfig.IpV4Config\x12\x16\n\x0ersyslog_server\x18\t \x01(\t\x1a\x46\n\nIpV4Config\x12\n\n\x02ip\x18\x01 \x01(\x07\x12\x0f\n\x07gateway\x18\x02 \x01(\x07\x12\x0e\n\x06subnet\x18\x03 \x01(\x07\x12\x0b\n\x03\x64ns\x18\x04 \x01(\x07\"#\n\x0b\x41\x64\x64ressMode\x12\x08\n\x04\x44HCP\x10\x00\x12\n\n\x06STATIC\x10\x01\x1a\xbe\x05\n\rDisplayConfig\x12\x16\n\x0escreen_on_secs\x18\x01 \x01(\r\x12H\n\ngps_format\x18\x02 \x01(\x0e\x32\x34.meshtastic.Config.DisplayConfig.GpsCoordinateFormat\x12!\n\x19\x61uto_screen_carousel_secs\x18\x03 \x01(\r\x12\x19\n\x11\x63ompass_north_top\x18\x04 \x01(\x08\x12\x13\n\x0b\x66lip_screen\x18\x05 \x01(\x08\x12<\n\x05units\x18\x06 \x01(\x0e\x32-.meshtastic.Config.DisplayConfig.DisplayUnits\x12\x37\n\x04oled\x18\x07 \x01(\x0e\x32).meshtastic.Config.DisplayConfig.OledType\x12\x41\n\x0b\x64isplaymode\x18\x08 \x01(\x0e\x32,.meshtastic.Config.DisplayConfig.DisplayMode\x12\x14\n\x0cheading_bold\x18\t \x01(\x08\x12\x1d\n\x15wake_on_tap_or_motion\x18\n \x01(\x08\"M\n\x13GpsCoordinateFormat\x12\x07\n\x03\x44\x45\x43\x10\x00\x12\x07\n\x03\x44MS\x10\x01\x12\x07\n\x03UTM\x10\x02\x12\x08\n\x04MGRS\x10\x03\x12\x07\n\x03OLC\x10\x04\x12\x08\n\x04OSGR\x10\x05\"(\n\x0c\x44isplayUnits\x12\n\n\x06METRIC\x10\x00\x12\x0c\n\x08IMPERIAL\x10\x01\"M\n\x08OledType\x12\r\n\tOLED_AUTO\x10\x00\x12\x10\n\x0cOLED_SSD1306\x10\x01\x12\x0f\n\x0bOLED_SH1106\x10\x02\x12\x0f\n\x0bOLED_SH1107\x10\x03\"A\n\x0b\x44isplayMode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x0c\n\x08TWOCOLOR\x10\x01\x12\x0c\n\x08INVERTED\x10\x02\x12\t\n\x05\x43OLOR\x10\x03\x1a\xb0\x06\n\nLoRaConfig\x12\x12\n\nuse_preset\x18\x01 \x01(\x08\x12?\n\x0cmodem_preset\x18\x02 \x01(\x0e\x32).meshtastic.Config.LoRaConfig.ModemPreset\x12\x11\n\tbandwidth\x18\x03 \x01(\r\x12\x15\n\rspread_factor\x18\x04 \x01(\r\x12\x13\n\x0b\x63oding_rate\x18\x05 \x01(\r\x12\x18\n\x10\x66requency_offset\x18\x06 \x01(\x02\x12\x38\n\x06region\x18\x07 \x01(\x0e\x32(.meshtastic.Config.LoRaConfig.RegionCode\x12\x11\n\thop_limit\x18\x08 \x01(\r\x12\x12\n\ntx_enabled\x18\t \x01(\x08\x12\x10\n\x08tx_power\x18\n \x01(\x05\x12\x13\n\x0b\x63hannel_num\x18\x0b \x01(\r\x12\x1b\n\x13override_duty_cycle\x18\x0c \x01(\x08\x12\x1e\n\x16sx126x_rx_boosted_gain\x18\r \x01(\x08\x12\x1a\n\x12override_frequency\x18\x0e \x01(\x02\x12\x17\n\x0fignore_incoming\x18g \x03(\r\x12\x13\n\x0bignore_mqtt\x18h \x01(\x08\"\xcd\x01\n\nRegionCode\x12\t\n\x05UNSET\x10\x00\x12\x06\n\x02US\x10\x01\x12\n\n\x06\x45U_433\x10\x02\x12\n\n\x06\x45U_868\x10\x03\x12\x06\n\x02\x43N\x10\x04\x12\x06\n\x02JP\x10\x05\x12\x07\n\x03\x41NZ\x10\x06\x12\x06\n\x02KR\x10\x07\x12\x06\n\x02TW\x10\x08\x12\x06\n\x02RU\x10\t\x12\x06\n\x02IN\x10\n\x12\n\n\x06NZ_865\x10\x0b\x12\x06\n\x02TH\x10\x0c\x12\x0b\n\x07LORA_24\x10\r\x12\n\n\x06UA_433\x10\x0e\x12\n\n\x06UA_868\x10\x0f\x12\n\n\x06MY_433\x10\x10\x12\n\n\x06MY_919\x10\x11\x12\n\n\x06SG_923\x10\x12\"\x94\x01\n\x0bModemPreset\x12\r\n\tLONG_FAST\x10\x00\x12\r\n\tLONG_SLOW\x10\x01\x12\x12\n\x0eVERY_LONG_SLOW\x10\x02\x12\x0f\n\x0bMEDIUM_SLOW\x10\x03\x12\x0f\n\x0bMEDIUM_FAST\x10\x04\x12\x0e\n\nSHORT_SLOW\x10\x05\x12\x0e\n\nSHORT_FAST\x10\x06\x12\x11\n\rLONG_MODERATE\x10\x07\x1a\xad\x01\n\x0f\x42luetoothConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12<\n\x04mode\x18\x02 \x01(\x0e\x32..meshtastic.Config.BluetoothConfig.PairingMode\x12\x11\n\tfixed_pin\x18\x03 \x01(\r\"8\n\x0bPairingMode\x12\x0e\n\nRANDOM_PIN\x10\x00\x12\r\n\tFIXED_PIN\x10\x01\x12\n\n\x06NO_PIN\x10\x02\x42\x11\n\x0fpayload_variantBa\n\x13\x63om.geeksville.meshB\x0c\x43onfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.config_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\014ConfigProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _CONFIG_POSITIONCONFIG.fields_by_name['gps_enabled']._options = None
   _CONFIG_POSITIONCONFIG.fields_by_name['gps_enabled']._serialized_options = b'\030\001'
   _CONFIG_POSITIONCONFIG.fields_by_name['gps_attempt_time']._options = None
   _CONFIG_POSITIONCONFIG.fields_by_name['gps_attempt_time']._serialized_options = b'\030\001'
-  _CONFIG._serialized_start=28
-  _CONFIG._serialized_end=3806
-  _CONFIG_DEVICECONFIG._serialized_start=327
-  _CONFIG_DEVICECONFIG._serialized_end=915
-  _CONFIG_DEVICECONFIG_ROLE._serialized_start=662
-  _CONFIG_DEVICECONFIG_ROLE._serialized_end=832
-  _CONFIG_DEVICECONFIG_REBROADCASTMODE._serialized_start=834
-  _CONFIG_DEVICECONFIG_REBROADCASTMODE._serialized_end=915
-  _CONFIG_POSITIONCONFIG._serialized_start=918
-  _CONFIG_POSITIONCONFIG._serialized_end=1564
-  _CONFIG_POSITIONCONFIG_POSITIONFLAGS._serialized_start=1338
-  _CONFIG_POSITIONCONFIG_POSITIONFLAGS._serialized_end=1509
-  _CONFIG_POSITIONCONFIG_GPSMODE._serialized_start=1511
-  _CONFIG_POSITIONCONFIG_GPSMODE._serialized_end=1564
-  _CONFIG_POWERCONFIG._serialized_start=1567
-  _CONFIG_POWERCONFIG._serialized_end=1801
-  _CONFIG_NETWORKCONFIG._serialized_start=1804
-  _CONFIG_NETWORKCONFIG._serialized_end=2164
-  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_start=2057
-  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_end=2127
-  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_start=2129
-  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_end=2164
-  _CONFIG_DISPLAYCONFIG._serialized_start=2167
-  _CONFIG_DISPLAYCONFIG._serialized_end=2825
-  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_start=2560
-  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_end=2637
-  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_start=2639
-  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_end=2679
-  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_start=2681
-  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_end=2758
-  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_start=2760
-  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_end=2825
-  _CONFIG_LORACONFIG._serialized_start=2828
-  _CONFIG_LORACONFIG._serialized_end=3622
-  _CONFIG_LORACONFIG_REGIONCODE._serialized_start=3266
-  _CONFIG_LORACONFIG_REGIONCODE._serialized_end=3471
-  _CONFIG_LORACONFIG_MODEMPRESET._serialized_start=3474
-  _CONFIG_LORACONFIG_MODEMPRESET._serialized_end=3622
-  _CONFIG_BLUETOOTHCONFIG._serialized_start=3625
-  _CONFIG_BLUETOOTHCONFIG._serialized_end=3787
-  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_start=3731
-  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_end=3787
+  _CONFIG._serialized_start=40
+  _CONFIG._serialized_end=4042
+  _CONFIG_DEVICECONFIG._serialized_start=416
+  _CONFIG_DEVICECONFIG._serialized_end=1041
+  _CONFIG_DEVICECONFIG_ROLE._serialized_start=788
+  _CONFIG_DEVICECONFIG_ROLE._serialized_end=958
+  _CONFIG_DEVICECONFIG_REBROADCASTMODE._serialized_start=960
+  _CONFIG_DEVICECONFIG_REBROADCASTMODE._serialized_end=1041
+  _CONFIG_POSITIONCONFIG._serialized_start=1044
+  _CONFIG_POSITIONCONFIG._serialized_end=1701
+  _CONFIG_POSITIONCONFIG_POSITIONFLAGS._serialized_start=1475
+  _CONFIG_POSITIONCONFIG_POSITIONFLAGS._serialized_end=1646
+  _CONFIG_POSITIONCONFIG_GPSMODE._serialized_start=1648
+  _CONFIG_POSITIONCONFIG_GPSMODE._serialized_end=1701
+  _CONFIG_POWERCONFIG._serialized_start=1704
+  _CONFIG_POWERCONFIG._serialized_end=1938
+  _CONFIG_NETWORKCONFIG._serialized_start=1941
+  _CONFIG_NETWORKCONFIG._serialized_end=2323
+  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_start=2216
+  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_end=2286
+  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_start=2288
+  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_end=2323
+  _CONFIG_DISPLAYCONFIG._serialized_start=2326
+  _CONFIG_DISPLAYCONFIG._serialized_end=3028
+  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_start=2763
+  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_end=2840
+  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_start=2842
+  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_end=2882
+  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_start=2884
+  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_end=2961
+  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_start=2963
+  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_end=3028
+  _CONFIG_LORACONFIG._serialized_start=3031
+  _CONFIG_LORACONFIG._serialized_end=3847
+  _CONFIG_LORACONFIG_REGIONCODE._serialized_start=3491
+  _CONFIG_LORACONFIG_REGIONCODE._serialized_end=3696
+  _CONFIG_LORACONFIG_MODEMPRESET._serialized_start=3699
+  _CONFIG_LORACONFIG_MODEMPRESET._serialized_end=3847
+  _CONFIG_BLUETOOTHCONFIG._serialized_start=3850
+  _CONFIG_BLUETOOTHCONFIG._serialized_end=4023
+  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_start=3967
+  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_end=4023
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/connection_status_pb2.py` & `meshtastic-2.3.4/meshtastic/connection_status_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"meshtastic/connection_status.proto\"\x85\x02\n\x16\x44\x65viceConnectionStatus\x12(\n\x04wifi\x18\x01 \x01(\x0b\x32\x15.WifiConnectionStatusH\x00\x88\x01\x01\x12\x30\n\x08\x65thernet\x18\x02 \x01(\x0b\x32\x19.EthernetConnectionStatusH\x01\x88\x01\x01\x12\x32\n\tbluetooth\x18\x03 \x01(\x0b\x32\x1a.BluetoothConnectionStatusH\x02\x88\x01\x01\x12,\n\x06serial\x18\x04 \x01(\x0b\x32\x17.SerialConnectionStatusH\x03\x88\x01\x01\x42\x07\n\x05_wifiB\x0b\n\t_ethernetB\x0c\n\n_bluetoothB\t\n\x07_serial\"\\\n\x14WifiConnectionStatus\x12(\n\x06status\x18\x01 \x01(\x0b\x32\x18.NetworkConnectionStatus\x12\x0c\n\x04ssid\x18\x02 \x01(\t\x12\x0c\n\x04rssi\x18\x03 \x01(\x05\"D\n\x18\x45thernetConnectionStatus\x12(\n\x06status\x18\x01 \x01(\x0b\x32\x18.NetworkConnectionStatus\"{\n\x17NetworkConnectionStatus\x12\x12\n\nip_address\x18\x01 \x01(\x07\x12\x14\n\x0cis_connected\x18\x02 \x01(\x08\x12\x19\n\x11is_mqtt_connected\x18\x03 \x01(\x08\x12\x1b\n\x13is_syslog_connected\x18\x04 \x01(\x08\"L\n\x19\x42luetoothConnectionStatus\x12\x0b\n\x03pin\x18\x01 \x01(\r\x12\x0c\n\x04rssi\x18\x02 \x01(\x05\x12\x14\n\x0cis_connected\x18\x03 \x01(\x08\"<\n\x16SerialConnectionStatus\x12\x0c\n\x04\x62\x61ud\x18\x01 \x01(\r\x12\x14\n\x0cis_connected\x18\x02 \x01(\x08\x42\x65\n\x13\x63om.geeksville.meshB\x10\x43onnStatusProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"meshtastic/connection_status.proto\x12\nmeshtastic\"\xb1\x02\n\x16\x44\x65viceConnectionStatus\x12\x33\n\x04wifi\x18\x01 \x01(\x0b\x32 .meshtastic.WifiConnectionStatusH\x00\x88\x01\x01\x12;\n\x08\x65thernet\x18\x02 \x01(\x0b\x32$.meshtastic.EthernetConnectionStatusH\x01\x88\x01\x01\x12=\n\tbluetooth\x18\x03 \x01(\x0b\x32%.meshtastic.BluetoothConnectionStatusH\x02\x88\x01\x01\x12\x37\n\x06serial\x18\x04 \x01(\x0b\x32\".meshtastic.SerialConnectionStatusH\x03\x88\x01\x01\x42\x07\n\x05_wifiB\x0b\n\t_ethernetB\x0c\n\n_bluetoothB\t\n\x07_serial\"g\n\x14WifiConnectionStatus\x12\x33\n\x06status\x18\x01 \x01(\x0b\x32#.meshtastic.NetworkConnectionStatus\x12\x0c\n\x04ssid\x18\x02 \x01(\t\x12\x0c\n\x04rssi\x18\x03 \x01(\x05\"O\n\x18\x45thernetConnectionStatus\x12\x33\n\x06status\x18\x01 \x01(\x0b\x32#.meshtastic.NetworkConnectionStatus\"{\n\x17NetworkConnectionStatus\x12\x12\n\nip_address\x18\x01 \x01(\x07\x12\x14\n\x0cis_connected\x18\x02 \x01(\x08\x12\x19\n\x11is_mqtt_connected\x18\x03 \x01(\x08\x12\x1b\n\x13is_syslog_connected\x18\x04 \x01(\x08\"L\n\x19\x42luetoothConnectionStatus\x12\x0b\n\x03pin\x18\x01 \x01(\r\x12\x0c\n\x04rssi\x18\x02 \x01(\x05\x12\x14\n\x0cis_connected\x18\x03 \x01(\x08\"<\n\x16SerialConnectionStatus\x12\x0c\n\x04\x62\x61ud\x18\x01 \x01(\r\x12\x14\n\x0cis_connected\x18\x02 \x01(\x08\x42\x65\n\x13\x63om.geeksville.meshB\x10\x43onnStatusProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.connection_status_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\020ConnStatusProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _DEVICECONNECTIONSTATUS._serialized_start=39
-  _DEVICECONNECTIONSTATUS._serialized_end=300
-  _WIFICONNECTIONSTATUS._serialized_start=302
-  _WIFICONNECTIONSTATUS._serialized_end=394
-  _ETHERNETCONNECTIONSTATUS._serialized_start=396
-  _ETHERNETCONNECTIONSTATUS._serialized_end=464
-  _NETWORKCONNECTIONSTATUS._serialized_start=466
-  _NETWORKCONNECTIONSTATUS._serialized_end=589
-  _BLUETOOTHCONNECTIONSTATUS._serialized_start=591
-  _BLUETOOTHCONNECTIONSTATUS._serialized_end=667
-  _SERIALCONNECTIONSTATUS._serialized_start=669
-  _SERIALCONNECTIONSTATUS._serialized_end=729
+  _DEVICECONNECTIONSTATUS._serialized_start=51
+  _DEVICECONNECTIONSTATUS._serialized_end=356
+  _WIFICONNECTIONSTATUS._serialized_start=358
+  _WIFICONNECTIONSTATUS._serialized_end=461
+  _ETHERNETCONNECTIONSTATUS._serialized_start=463
+  _ETHERNETCONNECTIONSTATUS._serialized_end=542
+  _NETWORKCONNECTIONSTATUS._serialized_start=544
+  _NETWORKCONNECTIONSTATUS._serialized_end=667
+  _BLUETOOTHCONNECTIONSTATUS._serialized_start=669
+  _BLUETOOTHCONNECTIONSTATUS._serialized_end=745
+  _SERIALCONNECTIONSTATUS._serialized_start=747
+  _SERIALCONNECTIONSTATUS._serialized_end=807
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/deviceonly_pb2.py` & `meshtastic-2.3.4/meshtastic/deviceonly_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,37 +10,37 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from meshtastic import channel_pb2 as meshtastic_dot_channel__pb2
 from meshtastic import localonly_pb2 as meshtastic_dot_localonly__pb2
 from meshtastic import mesh_pb2 as meshtastic_dot_mesh__pb2
-from meshtastic import telemetry_pb2 as meshtastic_dot_telemetry__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
+from meshtastic import telemetry_pb2 as meshtastic_dot_telemetry__pb2
 from . import nanopb_pb2 as nanopb__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bmeshtastic/deviceonly.proto\x1a\x18meshtastic/channel.proto\x1a\x1ameshtastic/localonly.proto\x1a\x15meshtastic/mesh.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x1emeshtastic/module_config.proto\x1a\x0cnanopb.proto\"\xf6\x02\n\x0b\x44\x65viceState\x12\x1c\n\x07my_node\x18\x02 \x01(\x0b\x32\x0b.MyNodeInfo\x12\x14\n\x05owner\x18\x03 \x01(\x0b\x32\x05.User\x12\"\n\rreceive_queue\x18\x05 \x03(\x0b\x32\x0b.MeshPacket\x12\x0f\n\x07version\x18\x08 \x01(\r\x12$\n\x0frx_text_message\x18\x07 \x01(\x0b\x32\x0b.MeshPacket\x12\x13\n\x07no_save\x18\t \x01(\x08\x42\x02\x18\x01\x12\x15\n\rdid_gps_reset\x18\x0b \x01(\x08\x12 \n\x0brx_waypoint\x18\x0c \x01(\x0b\x32\x0b.MeshPacket\x12\x39\n\x19node_remote_hardware_pins\x18\r \x03(\x0b\x32\x16.NodeRemoteHardwarePin\x12O\n\x0cnode_db_lite\x18\x0e \x03(\x0b\x32\r.NodeInfoLiteB*\x92?\'\x92\x01$std::vector<meshtastic_NodeInfoLite>\"\xe5\x01\n\x0cNodeInfoLite\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x13\n\x04user\x18\x02 \x01(\x0b\x32\x05.User\x12\x1f\n\x08position\x18\x03 \x01(\x0b\x32\r.PositionLite\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12&\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x0e.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\x12\x10\n\x08via_mqtt\x18\x08 \x01(\x08\x12\x11\n\thops_away\x18\t \x01(\r\x12\x13\n\x0bis_favorite\x18\n \x01(\x08\"\x85\x01\n\x0cPositionLite\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12,\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x13.Position.LocSource\":\n\x0b\x43hannelFile\x12\x1a\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x08.Channel\x12\x0f\n\x07version\x18\x02 \x01(\r\"\xf6\x01\n\x08OEMStore\x12\x16\n\x0eoem_icon_width\x18\x01 \x01(\r\x12\x17\n\x0foem_icon_height\x18\x02 \x01(\r\x12\x15\n\roem_icon_bits\x18\x03 \x01(\x0c\x12\x1e\n\x08oem_font\x18\x04 \x01(\x0e\x32\x0c.ScreenFonts\x12\x10\n\x08oem_text\x18\x05 \x01(\t\x12\x13\n\x0boem_aes_key\x18\x06 \x01(\x0c\x12&\n\x10oem_local_config\x18\x07 \x01(\x0b\x32\x0c.LocalConfig\x12\x33\n\x17oem_local_module_config\x18\x08 \x01(\x0b\x32\x12.LocalModuleConfig*>\n\x0bScreenFonts\x12\x0e\n\nFONT_SMALL\x10\x00\x12\x0f\n\x0b\x46ONT_MEDIUM\x10\x01\x12\x0e\n\nFONT_LARGE\x10\x02\x42m\n\x13\x63om.geeksville.meshB\nDeviceOnlyZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x92?\x0b\xc2\x01\x08<vector>b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bmeshtastic/deviceonly.proto\x12\nmeshtastic\x1a\x18meshtastic/channel.proto\x1a\x1ameshtastic/localonly.proto\x1a\x15meshtastic/mesh.proto\x1a\x1emeshtastic/module_config.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x0cnanopb.proto\"\x90\x01\n\x0cPositionLite\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12\x37\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x1e.meshtastic.Position.LocSource\"\x86\x02\n\x0cNodeInfoLite\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x1e\n\x04user\x18\x02 \x01(\x0b\x32\x10.meshtastic.User\x12*\n\x08position\x18\x03 \x01(\x0b\x32\x18.meshtastic.PositionLite\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12\x31\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x19.meshtastic.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\x12\x10\n\x08via_mqtt\x18\x08 \x01(\x08\x12\x11\n\thops_away\x18\t \x01(\r\x12\x13\n\x0bis_favorite\x18\n \x01(\x08\"\xc3\x03\n\x0b\x44\x65viceState\x12\'\n\x07my_node\x18\x02 \x01(\x0b\x32\x16.meshtastic.MyNodeInfo\x12\x1f\n\x05owner\x18\x03 \x01(\x0b\x32\x10.meshtastic.User\x12-\n\rreceive_queue\x18\x05 \x03(\x0b\x32\x16.meshtastic.MeshPacket\x12\x0f\n\x07version\x18\x08 \x01(\r\x12/\n\x0frx_text_message\x18\x07 \x01(\x0b\x32\x16.meshtastic.MeshPacket\x12\x13\n\x07no_save\x18\t \x01(\x08\x42\x02\x18\x01\x12\x15\n\rdid_gps_reset\x18\x0b \x01(\x08\x12+\n\x0brx_waypoint\x18\x0c \x01(\x0b\x32\x16.meshtastic.MeshPacket\x12\x44\n\x19node_remote_hardware_pins\x18\r \x03(\x0b\x32!.meshtastic.NodeRemoteHardwarePin\x12Z\n\x0cnode_db_lite\x18\x0e \x03(\x0b\x32\x18.meshtastic.NodeInfoLiteB*\x92?\'\x92\x01$std::vector<meshtastic_NodeInfoLite>\"E\n\x0b\x43hannelFile\x12%\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x13.meshtastic.Channel\x12\x0f\n\x07version\x18\x02 \x01(\r\"\x97\x02\n\x08OEMStore\x12\x16\n\x0eoem_icon_width\x18\x01 \x01(\r\x12\x17\n\x0foem_icon_height\x18\x02 \x01(\r\x12\x15\n\roem_icon_bits\x18\x03 \x01(\x0c\x12)\n\x08oem_font\x18\x04 \x01(\x0e\x32\x17.meshtastic.ScreenFonts\x12\x10\n\x08oem_text\x18\x05 \x01(\t\x12\x13\n\x0boem_aes_key\x18\x06 \x01(\x0c\x12\x31\n\x10oem_local_config\x18\x07 \x01(\x0b\x32\x17.meshtastic.LocalConfig\x12>\n\x17oem_local_module_config\x18\x08 \x01(\x0b\x32\x1d.meshtastic.LocalModuleConfig*>\n\x0bScreenFonts\x12\x0e\n\nFONT_SMALL\x10\x00\x12\x0f\n\x0b\x46ONT_MEDIUM\x10\x01\x12\x0e\n\nFONT_LARGE\x10\x02\x42m\n\x13\x63om.geeksville.meshB\nDeviceOnlyZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x92?\x0b\xc2\x01\x08<vector>b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.deviceonly_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\nDeviceOnlyZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000\222?\013\302\001\010<vector>'
   _DEVICESTATE.fields_by_name['no_save']._options = None
   _DEVICESTATE.fields_by_name['no_save']._serialized_options = b'\030\001'
   _DEVICESTATE.fields_by_name['node_db_lite']._options = None
   _DEVICESTATE.fields_by_name['node_db_lite']._serialized_options = b'\222?\'\222\001$std::vector<meshtastic_NodeInfoLite>'
-  _SCREENFONTS._serialized_start=1236
-  _SCREENFONTS._serialized_end=1298
-  _DEVICESTATE._serialized_start=183
-  _DEVICESTATE._serialized_end=557
-  _NODEINFOLITE._serialized_start=560
-  _NODEINFOLITE._serialized_end=789
-  _POSITIONLITE._serialized_start=792
-  _POSITIONLITE._serialized_end=925
-  _CHANNELFILE._serialized_start=927
-  _CHANNELFILE._serialized_end=985
-  _OEMSTORE._serialized_start=988
-  _OEMSTORE._serialized_end=1234
+  _SCREENFONTS._serialized_start=1413
+  _SCREENFONTS._serialized_end=1475
+  _POSITIONLITE._serialized_start=195
+  _POSITIONLITE._serialized_end=339
+  _NODEINFOLITE._serialized_start=342
+  _NODEINFOLITE._serialized_end=604
+  _DEVICESTATE._serialized_start=607
+  _DEVICESTATE._serialized_end=1058
+  _CHANNELFILE._serialized_start=1060
+  _CHANNELFILE._serialized_end=1129
+  _OEMSTORE._serialized_start=1132
+  _OEMSTORE._serialized_end=1411
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/globals.py` & `meshtastic-2.3.4/meshtastic/globals.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.3/meshtastic/localonly_pb2.py` & `meshtastic-2.3.4/meshtastic/localonly_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 _sym_db = _symbol_database.Default()
 
 
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ameshtastic/localonly.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\"\xb0\x02\n\x0bLocalConfig\x12$\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x14.Config.DeviceConfig\x12(\n\x08position\x18\x02 \x01(\x0b\x32\x16.Config.PositionConfig\x12\"\n\x05power\x18\x03 \x01(\x0b\x32\x13.Config.PowerConfig\x12&\n\x07network\x18\x04 \x01(\x0b\x32\x15.Config.NetworkConfig\x12&\n\x07\x64isplay\x18\x05 \x01(\x0b\x32\x15.Config.DisplayConfig\x12 \n\x04lora\x18\x06 \x01(\x0b\x32\x12.Config.LoRaConfig\x12*\n\tbluetooth\x18\x07 \x01(\x0b\x32\x17.Config.BluetoothConfig\x12\x0f\n\x07version\x18\x08 \x01(\r\"\xec\x05\n\x11LocalModuleConfig\x12&\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfig\x12*\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfig\x12G\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfig\x12\x37\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfig\x12\x31\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfig\x12\x30\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfig\x12\x39\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfig\x12(\n\x05\x61udio\x18\t \x01(\x0b\x32\x19.ModuleConfig.AudioConfig\x12;\n\x0fremote_hardware\x18\n \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfig\x12\x37\n\rneighbor_info\x18\x0b \x01(\x0b\x32 .ModuleConfig.NeighborInfoConfig\x12=\n\x10\x61mbient_lighting\x18\x0c \x01(\x0b\x32#.ModuleConfig.AmbientLightingConfig\x12=\n\x10\x64\x65tection_sensor\x18\r \x01(\x0b\x32#.ModuleConfig.DetectionSensorConfig\x12\x32\n\npaxcounter\x18\x0e \x01(\x0b\x32\x1e.ModuleConfig.PaxcounterConfig\x12\x0f\n\x07version\x18\x08 \x01(\rBd\n\x13\x63om.geeksville.meshB\x0fLocalOnlyProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ameshtastic/localonly.proto\x12\nmeshtastic\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\"\xfd\x02\n\x0bLocalConfig\x12/\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x1f.meshtastic.Config.DeviceConfig\x12\x33\n\x08position\x18\x02 \x01(\x0b\x32!.meshtastic.Config.PositionConfig\x12-\n\x05power\x18\x03 \x01(\x0b\x32\x1e.meshtastic.Config.PowerConfig\x12\x31\n\x07network\x18\x04 \x01(\x0b\x32 .meshtastic.Config.NetworkConfig\x12\x31\n\x07\x64isplay\x18\x05 \x01(\x0b\x32 .meshtastic.Config.DisplayConfig\x12+\n\x04lora\x18\x06 \x01(\x0b\x32\x1d.meshtastic.Config.LoRaConfig\x12\x35\n\tbluetooth\x18\x07 \x01(\x0b\x32\".meshtastic.Config.BluetoothConfig\x12\x0f\n\x07version\x18\x08 \x01(\r\"\xfb\x06\n\x11LocalModuleConfig\x12\x31\n\x04mqtt\x18\x01 \x01(\x0b\x32#.meshtastic.ModuleConfig.MQTTConfig\x12\x35\n\x06serial\x18\x02 \x01(\x0b\x32%.meshtastic.ModuleConfig.SerialConfig\x12R\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32\x33.meshtastic.ModuleConfig.ExternalNotificationConfig\x12\x42\n\rstore_forward\x18\x04 \x01(\x0b\x32+.meshtastic.ModuleConfig.StoreForwardConfig\x12<\n\nrange_test\x18\x05 \x01(\x0b\x32(.meshtastic.ModuleConfig.RangeTestConfig\x12;\n\ttelemetry\x18\x06 \x01(\x0b\x32(.meshtastic.ModuleConfig.TelemetryConfig\x12\x44\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32,.meshtastic.ModuleConfig.CannedMessageConfig\x12\x33\n\x05\x61udio\x18\t \x01(\x0b\x32$.meshtastic.ModuleConfig.AudioConfig\x12\x46\n\x0fremote_hardware\x18\n \x01(\x0b\x32-.meshtastic.ModuleConfig.RemoteHardwareConfig\x12\x42\n\rneighbor_info\x18\x0b \x01(\x0b\x32+.meshtastic.ModuleConfig.NeighborInfoConfig\x12H\n\x10\x61mbient_lighting\x18\x0c \x01(\x0b\x32..meshtastic.ModuleConfig.AmbientLightingConfig\x12H\n\x10\x64\x65tection_sensor\x18\r \x01(\x0b\x32..meshtastic.ModuleConfig.DetectionSensorConfig\x12=\n\npaxcounter\x18\x0e \x01(\x0b\x32).meshtastic.ModuleConfig.PaxcounterConfig\x12\x0f\n\x07version\x18\x08 \x01(\rBd\n\x13\x63om.geeksville.meshB\x0fLocalOnlyProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.localonly_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\017LocalOnlyProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _LOCALCONFIG._serialized_start=88
-  _LOCALCONFIG._serialized_end=392
-  _LOCALMODULECONFIG._serialized_start=395
-  _LOCALMODULECONFIG._serialized_end=1143
+  _LOCALCONFIG._serialized_start=100
+  _LOCALCONFIG._serialized_end=481
+  _LOCALMODULECONFIG._serialized_start=484
+  _LOCALMODULECONFIG._serialized_end=1375
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/mesh_interface.py` & `meshtastic-2.3.4/meshtastic/mesh_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,39 +5,40 @@
 import json
 import logging
 import random
 import sys
 import threading
 import time
 from datetime import datetime
-from typing import AnyStr
 
 import google.protobuf.json_format
-import timeago
-from google.protobuf.json_format import MessageToJson
-from pubsub import pub
+import timeago # type: ignore[import-untyped]
+from pubsub import pub # type: ignore[import-untyped]
 from tabulate import tabulate
 
 import meshtastic.node
-from meshtastic import mesh_pb2, portnums_pb2, telemetry_pb2
-from meshtastic.__init__ import (
+from meshtastic import (
+    mesh_pb2,
+    portnums_pb2,
+    telemetry_pb2,
     BROADCAST_ADDR,
     BROADCAST_NUM,
     LOCAL_ADDR,
     ResponseHandler,
     protocols,
     publishingThread,
 )
 from meshtastic.util import (
     Acknowledgment,
     Timeout,
     convert_mac_addr,
     our_exit,
     remove_keys_from_dict,
     stripnl,
+    message_to_json,
 )
 
 
 class MeshInterface:
     """Interface class for meshtastic devices
 
     Properties:
@@ -103,18 +104,18 @@
         self.close()
 
     def showInfo(self, file=sys.stdout):  # pylint: disable=W0613
         """Show human readable summary about this object"""
         owner = f"Owner: {self.getLongName()} ({self.getShortName()})"
         myinfo = ""
         if self.myInfo:
-            myinfo = f"\nMy info: {stripnl(MessageToJson(self.myInfo))}"
+            myinfo = f"\nMy info: {message_to_json(self.myInfo)}"
         metadata = ""
         if self.metadata:
-            metadata = f"\nMetadata: {stripnl(MessageToJson(self.metadata))}"
+            metadata = f"\nMetadata: {message_to_json(self.metadata)}"
         mesh = "\n\nNodes in mesh: "
         nodes = {}
         if self.nodes:
             for n in self.nodes.values():
                 # when the TBeam is first booted, it sometimes shows the raw data
                 # so, we will just remove any raw keys
                 keys_to_remove = ("raw", "decoded", "payload")
@@ -158,15 +159,15 @@
         rows = []
         if self.nodesByNum:
             logging.debug(f"self.nodes:{self.nodes}")
             for node in self.nodesByNum.values():
                 if not includeSelf and node["num"] == self.localNode.nodeNum:
                     continue
 
-                row = {"N": 0, "User": f"UNK: {node['num']}", "ID": f"!{node['num']:x}"}
+                row = {"N": 0, "User": f"UNK: {node['num']}", "ID": f"!{node['num']:08x}"}
 
                 user = node.get("user")
                 if user:
                     row.update(
                         {
                             "User": user.get("longName", "N/A"),
                             "AKA": user.get("shortName", "N/A"),
@@ -235,15 +236,15 @@
                 n.requestChannels()
                 if not n.waitForConfig():
                     our_exit("Error: Timed out waiting for channels")
             return n
 
     def sendText(
         self,
-        text: AnyStr,
+        text: str,
         destinationId=BROADCAST_ADDR,
         wantAck=False,
         wantResponse=False,
         onResponse=None,
         channelIndex=0,
     ):
         """Send a utf8 string to some other node, if the node has a display it
```

### Comparing `meshtastic-2.3.3/meshtastic/mesh_pb2.py` & `meshtastic-2.3.4/meshtastic/mesh_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,78 +15,78 @@
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
 from meshtastic import portnums_pb2 as meshtastic_dot_portnums__pb2
 from meshtastic import telemetry_pb2 as meshtastic_dot_telemetry__pb2
 from meshtastic import xmodem_pb2 as meshtastic_dot_xmodem__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xcf\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12,\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x13.Position.LocSource\x12,\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x13.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\x12\x16\n\x0eprecision_bits\x18\x17 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\xae\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x13\n\x07macaddr\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12 \n\x08hw_model\x18\x05 \x01(\x0e\x32\x0e.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\x12\'\n\x04role\x18\x07 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xdb\x02\n\x07Routing\x12(\n\rroute_request\x18\x01 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x0e.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\x9c\x01\n\x04\x44\x61ta\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"l\n\x16MqttClientProxyMessage\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x0e\n\x04\x64\x61ta\x18\x02 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x03 \x01(\tH\x00\x12\x10\n\x08retained\x18\x04 \x01(\x08\x42\x11\n\x0fpayload_variant\"\xf4\x03\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12\x18\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x05.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12&\n\x08priority\x18\x0b \x01(\x0e\x32\x14.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12(\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x13.MeshPacket.DelayedB\x02\x18\x01\x12\x10\n\x08via_mqtt\x18\x0e \x01(\x08\x12\x11\n\thop_start\x18\x0f \x01(\r\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xdd\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x13\n\x04user\x18\x02 \x01(\x0b\x32\x05.User\x12\x1b\n\x08position\x18\x03 \x01(\x0b\x32\t.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12&\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x0e.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\x12\x10\n\x08via_mqtt\x18\x08 \x01(\x08\x12\x11\n\thops_away\x18\t \x01(\r\x12\x13\n\x0bis_favorite\x18\n \x01(\x08\"P\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\"\xb5\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x1f\n\x05level\x18\x04 \x01(\x0e\x32\x10.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xe2\x03\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12\x1d\n\x06packet\x18\x02 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x1e\n\x07my_info\x18\x03 \x01(\x0b\x32\x0b.MyNodeInfoH\x00\x12\x1e\n\tnode_info\x18\x04 \x01(\x0b\x32\t.NodeInfoH\x00\x12\x19\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x07.ConfigH\x00\x12 \n\nlog_record\x18\x06 \x01(\x0b\x32\n.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12%\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\r.ModuleConfigH\x00\x12\x1b\n\x07\x63hannel\x18\n \x01(\x0b\x32\x08.ChannelH\x00\x12#\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x0c.QueueStatusH\x00\x12\x1f\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x07.XModemH\x00\x12#\n\x08metadata\x18\r \x01(\x0b\x32\x0f.DeviceMetadataH\x00\x12\x39\n\x16mqttClientProxyMessage\x18\x0e \x01(\x0b\x32\x17.MqttClientProxyMessageH\x00\x42\x11\n\x0fpayload_variant\"\xe8\x01\n\x07ToRadio\x12\x1d\n\x06packet\x18\x01 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12\x1f\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x07.XModemH\x00\x12\x39\n\x16mqttClientProxyMessage\x18\x06 \x01(\x0b\x32\x17.MqttClientProxyMessageH\x00\x12\x1f\n\theartbeat\x18\x07 \x01(\x0b\x32\n.HeartbeatH\x00\x42\x11\n\x0fpayload_variant\"5\n\nCompressed\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"|\n\x0cNeighborInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x17\n\x0flast_sent_by_id\x18\x02 \x01(\r\x12$\n\x1cnode_broadcast_interval_secs\x18\x03 \x01(\r\x12\x1c\n\tneighbors\x18\x04 \x03(\x0b\x32\t.Neighbor\"d\n\x08Neighbor\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x0b\n\x03snr\x18\x02 \x01(\x02\x12\x14\n\x0clast_rx_time\x18\x03 \x01(\x07\x12$\n\x1cnode_broadcast_interval_secs\x18\x04 \x01(\r\"\x97\x02\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\'\n\x04role\x18\x07 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12 \n\x08hw_model\x18\t \x01(\x0e\x32\x0e.HardwareModel\x12\x19\n\x11hasRemoteHardware\x18\n \x01(\x08\"\x0b\n\tHeartbeat\"J\n\x15NodeRemoteHardwarePin\x12\x10\n\x08node_num\x18\x01 \x01(\r\x12\x1f\n\x03pin\x18\x02 \x01(\x0b\x32\x12.RemoteHardwarePin*\xd4\x07\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x11\n\rNANO_G2_ULTRA\x10\x12\x12\r\n\tLORA_TYPE\x10\x13\x12\x0e\n\nSTATION_G1\x10\x19\x12\x0c\n\x08RAK11310\x10\x1a\x12\x14\n\x10SENSELORA_RP2040\x10\x1b\x12\x10\n\x0cSENSELORA_S3\x10\x1c\x12\r\n\tCANARYONE\x10\x1d\x12\x0f\n\x0bRP2040_LORA\x10\x1e\x12\x0e\n\nSTATION_G2\x10\x1f\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0c\n\x08RPI_PICO\x10/\x12\x1b\n\x17HELTEC_WIRELESS_TRACKER\x10\x30\x12\x19\n\x15HELTEC_WIRELESS_PAPER\x10\x31\x12\n\n\x06T_DECK\x10\x32\x12\x0e\n\nT_WATCH_S3\x10\x33\x12\x11\n\rPICOMPUTER_S3\x10\x34\x12\x0f\n\x0bHELTEC_HT62\x10\x35\x12\x12\n\x0e\x45\x42YTE_ESP32_S3\x10\x36\x12\x11\n\rESP32_S3_PICO\x10\x37\x12\r\n\tCHATTER_2\x10\x38\x12\x1e\n\x1aHELTEC_WIRELESS_PAPER_V1_0\x10\x39\x12 \n\x1cHELTEC_WIRELESS_TRACKER_V1_0\x10:\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x12\nmeshtastic\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xe5\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12\x37\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x1e.meshtastic.Position.LocSource\x12\x37\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x1e.meshtastic.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\x12\x16\n\x0eprecision_bits\x18\x17 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\xc4\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x13\n\x07macaddr\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12+\n\x08hw_model\x18\x05 \x01(\x0e\x32\x19.meshtastic.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\x12\x32\n\x04role\x18\x07 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xfc\x02\n\x07Routing\x12\x33\n\rroute_request\x18\x01 \x01(\x0b\x32\x1a.meshtastic.RouteDiscoveryH\x00\x12\x31\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x1a.meshtastic.RouteDiscoveryH\x00\x12\x31\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x19.meshtastic.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\xa7\x01\n\x04\x44\x61ta\x12$\n\x07portnum\x18\x01 \x01(\x0e\x32\x13.meshtastic.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"l\n\x16MqttClientProxyMessage\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x0e\n\x04\x64\x61ta\x18\x02 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x03 \x01(\tH\x00\x12\x10\n\x08retained\x18\x04 \x01(\x08\x42\x11\n\x0fpayload_variant\"\x95\x04\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12#\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x10.meshtastic.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12\x31\n\x08priority\x18\x0b \x01(\x0e\x32\x1f.meshtastic.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12\x33\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x1e.meshtastic.MeshPacket.DelayedB\x02\x18\x01\x12\x10\n\x08via_mqtt\x18\x0e \x01(\x08\x12\x11\n\thop_start\x18\x0f \x01(\r\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xfe\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x1e\n\x04user\x18\x02 \x01(\x0b\x32\x10.meshtastic.User\x12&\n\x08position\x18\x03 \x01(\x0b\x32\x14.meshtastic.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12\x31\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x19.meshtastic.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\x12\x10\n\x08via_mqtt\x18\x08 \x01(\x08\x12\x11\n\thops_away\x18\t \x01(\r\x12\x13\n\x0bis_favorite\x18\n \x01(\x08\"P\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\"\xc0\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12*\n\x05level\x18\x04 \x01(\x0e\x32\x1b.meshtastic.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xdb\x04\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12(\n\x06packet\x18\x02 \x01(\x0b\x32\x16.meshtastic.MeshPacketH\x00\x12)\n\x07my_info\x18\x03 \x01(\x0b\x32\x16.meshtastic.MyNodeInfoH\x00\x12)\n\tnode_info\x18\x04 \x01(\x0b\x32\x14.meshtastic.NodeInfoH\x00\x12$\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x12.meshtastic.ConfigH\x00\x12+\n\nlog_record\x18\x06 \x01(\x0b\x32\x15.meshtastic.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12\x30\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\x18.meshtastic.ModuleConfigH\x00\x12&\n\x07\x63hannel\x18\n \x01(\x0b\x32\x13.meshtastic.ChannelH\x00\x12.\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x17.meshtastic.QueueStatusH\x00\x12*\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x12.meshtastic.XModemH\x00\x12.\n\x08metadata\x18\r \x01(\x0b\x32\x1a.meshtastic.DeviceMetadataH\x00\x12\x44\n\x16mqttClientProxyMessage\x18\x0e \x01(\x0b\x32\".meshtastic.MqttClientProxyMessageH\x00\x42\x11\n\x0fpayload_variant\"\x94\x02\n\x07ToRadio\x12(\n\x06packet\x18\x01 \x01(\x0b\x32\x16.meshtastic.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12*\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x12.meshtastic.XModemH\x00\x12\x44\n\x16mqttClientProxyMessage\x18\x06 \x01(\x0b\x32\".meshtastic.MqttClientProxyMessageH\x00\x12*\n\theartbeat\x18\x07 \x01(\x0b\x32\x15.meshtastic.HeartbeatH\x00\x42\x11\n\x0fpayload_variant\"@\n\nCompressed\x12$\n\x07portnum\x18\x01 \x01(\x0e\x32\x13.meshtastic.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x87\x01\n\x0cNeighborInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x17\n\x0flast_sent_by_id\x18\x02 \x01(\r\x12$\n\x1cnode_broadcast_interval_secs\x18\x03 \x01(\r\x12\'\n\tneighbors\x18\x04 \x03(\x0b\x32\x14.meshtastic.Neighbor\"d\n\x08Neighbor\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x0b\n\x03snr\x18\x02 \x01(\x02\x12\x14\n\x0clast_rx_time\x18\x03 \x01(\x07\x12$\n\x1cnode_broadcast_interval_secs\x18\x04 \x01(\r\"\xad\x02\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\x32\n\x04role\x18\x07 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12+\n\x08hw_model\x18\t \x01(\x0e\x32\x19.meshtastic.HardwareModel\x12\x19\n\x11hasRemoteHardware\x18\n \x01(\x08\"\x0b\n\tHeartbeat\"U\n\x15NodeRemoteHardwarePin\x12\x10\n\x08node_num\x18\x01 \x01(\r\x12*\n\x03pin\x18\x02 \x01(\x0b\x32\x1d.meshtastic.RemoteHardwarePin*\xef\x07\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x11\n\rNANO_G2_ULTRA\x10\x12\x12\r\n\tLORA_TYPE\x10\x13\x12\x0e\n\nSTATION_G1\x10\x19\x12\x0c\n\x08RAK11310\x10\x1a\x12\x14\n\x10SENSELORA_RP2040\x10\x1b\x12\x10\n\x0cSENSELORA_S3\x10\x1c\x12\r\n\tCANARYONE\x10\x1d\x12\x0f\n\x0bRP2040_LORA\x10\x1e\x12\x0e\n\nSTATION_G2\x10\x1f\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0c\n\x08RPI_PICO\x10/\x12\x1b\n\x17HELTEC_WIRELESS_TRACKER\x10\x30\x12\x19\n\x15HELTEC_WIRELESS_PAPER\x10\x31\x12\n\n\x06T_DECK\x10\x32\x12\x0e\n\nT_WATCH_S3\x10\x33\x12\x11\n\rPICOMPUTER_S3\x10\x34\x12\x0f\n\x0bHELTEC_HT62\x10\x35\x12\x12\n\x0e\x45\x42YTE_ESP32_S3\x10\x36\x12\x11\n\rESP32_S3_PICO\x10\x37\x12\r\n\tCHATTER_2\x10\x38\x12\x1e\n\x1aHELTEC_WIRELESS_PAPER_V1_0\x10\x39\x12 \n\x1cHELTEC_WIRELESS_TRACKER_V1_0\x10:\x12\x0b\n\x07UNPHONE\x10;\x12\x0c\n\x08TD_LORAC\x10<\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.mesh_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _USER.fields_by_name['macaddr']._options = None
   _USER.fields_by_name['macaddr']._serialized_options = b'\030\001'
   _MESHPACKET.fields_by_name['delayed']._options = None
   _MESHPACKET.fields_by_name['delayed']._serialized_options = b'\030\001'
-  _HARDWAREMODEL._serialized_start=4339
-  _HARDWAREMODEL._serialized_end=5319
-  _CONSTANTS._serialized_start=5321
-  _CONSTANTS._serialized_end=5365
-  _CRITICALERRORCODE._serialized_start=5368
-  _CRITICALERRORCODE._serialized_end=5606
-  _POSITION._serialized_start=189
-  _POSITION._serialized_end=908
-  _POSITION_LOCSOURCE._serialized_start=730
-  _POSITION_LOCSOURCE._serialized_end=808
-  _POSITION_ALTSOURCE._serialized_start=810
-  _POSITION_ALTSOURCE._serialized_end=908
-  _USER._serialized_start=911
-  _USER._serialized_end=1085
-  _ROUTEDISCOVERY._serialized_start=1087
-  _ROUTEDISCOVERY._serialized_end=1118
-  _ROUTING._serialized_start=1121
-  _ROUTING._serialized_end=1468
-  _ROUTING_ERROR._serialized_start=1255
-  _ROUTING_ERROR._serialized_end=1457
-  _DATA._serialized_start=1471
-  _DATA._serialized_end=1627
-  _WAYPOINT._serialized_start=1630
-  _WAYPOINT._serialized_end=1777
-  _MQTTCLIENTPROXYMESSAGE._serialized_start=1779
-  _MQTTCLIENTPROXYMESSAGE._serialized_end=1887
-  _MESHPACKET._serialized_start=1890
-  _MESHPACKET._serialized_end=2390
-  _MESHPACKET_PRIORITY._serialized_start=2212
-  _MESHPACKET_PRIORITY._serialized_end=2303
-  _MESHPACKET_DELAYED._serialized_start=2305
-  _MESHPACKET_DELAYED._serialized_end=2371
-  _NODEINFO._serialized_start=2393
-  _NODEINFO._serialized_end=2614
-  _MYNODEINFO._serialized_start=2616
-  _MYNODEINFO._serialized_end=2696
-  _LOGRECORD._serialized_start=2699
-  _LOGRECORD._serialized_end=2880
-  _LOGRECORD_LEVEL._serialized_start=2792
-  _LOGRECORD_LEVEL._serialized_end=2880
-  _QUEUESTATUS._serialized_start=2882
-  _QUEUESTATUS._serialized_end=2962
-  _FROMRADIO._serialized_start=2965
-  _FROMRADIO._serialized_end=3447
-  _TORADIO._serialized_start=3450
-  _TORADIO._serialized_end=3682
-  _COMPRESSED._serialized_start=3684
-  _COMPRESSED._serialized_end=3737
-  _NEIGHBORINFO._serialized_start=3739
-  _NEIGHBORINFO._serialized_end=3863
-  _NEIGHBOR._serialized_start=3865
-  _NEIGHBOR._serialized_end=3965
-  _DEVICEMETADATA._serialized_start=3968
-  _DEVICEMETADATA._serialized_end=4247
-  _HEARTBEAT._serialized_start=4249
-  _HEARTBEAT._serialized_end=4260
-  _NODEREMOTEHARDWAREPIN._serialized_start=4262
-  _NODEREMOTEHARDWAREPIN._serialized_end=4336
+  _HARDWAREMODEL._serialized_start=4737
+  _HARDWAREMODEL._serialized_end=5744
+  _CONSTANTS._serialized_start=5746
+  _CONSTANTS._serialized_end=5790
+  _CRITICALERRORCODE._serialized_start=5793
+  _CRITICALERRORCODE._serialized_end=6031
+  _POSITION._serialized_start=201
+  _POSITION._serialized_end=942
+  _POSITION_LOCSOURCE._serialized_start=764
+  _POSITION_LOCSOURCE._serialized_end=842
+  _POSITION_ALTSOURCE._serialized_start=844
+  _POSITION_ALTSOURCE._serialized_end=942
+  _USER._serialized_start=945
+  _USER._serialized_end=1141
+  _ROUTEDISCOVERY._serialized_start=1143
+  _ROUTEDISCOVERY._serialized_end=1174
+  _ROUTING._serialized_start=1177
+  _ROUTING._serialized_end=1557
+  _ROUTING_ERROR._serialized_start=1344
+  _ROUTING_ERROR._serialized_end=1546
+  _DATA._serialized_start=1560
+  _DATA._serialized_end=1727
+  _WAYPOINT._serialized_start=1730
+  _WAYPOINT._serialized_end=1877
+  _MQTTCLIENTPROXYMESSAGE._serialized_start=1879
+  _MQTTCLIENTPROXYMESSAGE._serialized_end=1987
+  _MESHPACKET._serialized_start=1990
+  _MESHPACKET._serialized_end=2523
+  _MESHPACKET_PRIORITY._serialized_start=2345
+  _MESHPACKET_PRIORITY._serialized_end=2436
+  _MESHPACKET_DELAYED._serialized_start=2438
+  _MESHPACKET_DELAYED._serialized_end=2504
+  _NODEINFO._serialized_start=2526
+  _NODEINFO._serialized_end=2780
+  _MYNODEINFO._serialized_start=2782
+  _MYNODEINFO._serialized_end=2862
+  _LOGRECORD._serialized_start=2865
+  _LOGRECORD._serialized_end=3057
+  _LOGRECORD_LEVEL._serialized_start=2969
+  _LOGRECORD_LEVEL._serialized_end=3057
+  _QUEUESTATUS._serialized_start=3059
+  _QUEUESTATUS._serialized_end=3139
+  _FROMRADIO._serialized_start=3142
+  _FROMRADIO._serialized_end=3745
+  _TORADIO._serialized_start=3748
+  _TORADIO._serialized_end=4024
+  _COMPRESSED._serialized_start=4026
+  _COMPRESSED._serialized_end=4090
+  _NEIGHBORINFO._serialized_start=4093
+  _NEIGHBORINFO._serialized_end=4228
+  _NEIGHBOR._serialized_start=4230
+  _NEIGHBOR._serialized_end=4330
+  _DEVICEMETADATA._serialized_start=4333
+  _DEVICEMETADATA._serialized_end=4634
+  _HEARTBEAT._serialized_start=4636
+  _HEARTBEAT._serialized_end=4647
+  _NODEREMOTEHARDWAREPIN._serialized_start=4649
+  _NODEREMOTEHARDWAREPIN._serialized_end=4734
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/module_config_pb2.py` & `meshtastic-2.3.4/meshtastic/module_config_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,58 +9,58 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emeshtastic/module_config.proto\"\xbc \n\x0cModuleConfig\x12(\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfigH\x00\x12,\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfigH\x00\x12I\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfigH\x00\x12\x39\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfigH\x00\x12\x33\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfigH\x00\x12\x32\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfigH\x00\x12;\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfigH\x00\x12*\n\x05\x61udio\x18\x08 \x01(\x0b\x32\x19.ModuleConfig.AudioConfigH\x00\x12=\n\x0fremote_hardware\x18\t \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfigH\x00\x12\x39\n\rneighbor_info\x18\n \x01(\x0b\x32 .ModuleConfig.NeighborInfoConfigH\x00\x12?\n\x10\x61mbient_lighting\x18\x0b \x01(\x0b\x32#.ModuleConfig.AmbientLightingConfigH\x00\x12?\n\x10\x64\x65tection_sensor\x18\x0c \x01(\x0b\x32#.ModuleConfig.DetectionSensorConfigH\x00\x12\x34\n\npaxcounter\x18\r \x01(\x0b\x32\x1e.ModuleConfig.PaxcounterConfigH\x00\x1a\xa5\x02\n\nMQTTConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x1a\n\x12\x65ncryption_enabled\x18\x05 \x01(\x08\x12\x14\n\x0cjson_enabled\x18\x06 \x01(\x08\x12\x13\n\x0btls_enabled\x18\x07 \x01(\x08\x12\x0c\n\x04root\x18\x08 \x01(\t\x12\x1f\n\x17proxy_to_client_enabled\x18\t \x01(\x08\x12\x1d\n\x15map_reporting_enabled\x18\n \x01(\x08\x12<\n\x13map_report_settings\x18\x0b \x01(\x0b\x32\x1f.ModuleConfig.MapReportSettings\x1aN\n\x11MapReportSettings\x12\x1d\n\x15publish_interval_secs\x18\x01 \x01(\r\x12\x1a\n\x12position_precision\x18\x02 \x01(\r\x1aw\n\x14RemoteHardwareConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x1a\x61llow_undefined_pin_access\x18\x02 \x01(\x08\x12*\n\x0e\x61vailable_pins\x18\x03 \x03(\x0b\x32\x12.RemoteHardwarePin\x1a>\n\x12NeighborInfoConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\x0fupdate_interval\x18\x02 \x01(\r\x1a\xd2\x01\n\x15\x44\x65tectionSensorConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\x16minimum_broadcast_secs\x18\x02 \x01(\r\x12\x1c\n\x14state_broadcast_secs\x18\x03 \x01(\r\x12\x11\n\tsend_bell\x18\x04 \x01(\x08\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x13\n\x0bmonitor_pin\x18\x06 \x01(\r\x12 \n\x18\x64\x65tection_triggered_high\x18\x07 \x01(\x08\x12\x12\n\nuse_pullup\x18\x08 \x01(\x08\x1a\xd9\x02\n\x0b\x41udioConfig\x12\x16\n\x0e\x63odec2_enabled\x18\x01 \x01(\x08\x12\x0f\n\x07ptt_pin\x18\x02 \x01(\r\x12\x35\n\x07\x62itrate\x18\x03 \x01(\x0e\x32$.ModuleConfig.AudioConfig.Audio_Baud\x12\x0e\n\x06i2s_ws\x18\x04 \x01(\r\x12\x0e\n\x06i2s_sd\x18\x05 \x01(\r\x12\x0f\n\x07i2s_din\x18\x06 \x01(\r\x12\x0f\n\x07i2s_sck\x18\x07 \x01(\r\"\xa7\x01\n\nAudio_Baud\x12\x12\n\x0e\x43ODEC2_DEFAULT\x10\x00\x12\x0f\n\x0b\x43ODEC2_3200\x10\x01\x12\x0f\n\x0b\x43ODEC2_2400\x10\x02\x12\x0f\n\x0b\x43ODEC2_1600\x10\x03\x12\x0f\n\x0b\x43ODEC2_1400\x10\x04\x12\x0f\n\x0b\x43ODEC2_1300\x10\x05\x12\x0f\n\x0b\x43ODEC2_1200\x10\x06\x12\x0e\n\nCODEC2_700\x10\x07\x12\x0f\n\x0b\x43ODEC2_700B\x10\x08\x1aG\n\x10PaxcounterConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x1apaxcounter_update_interval\x18\x02 \x01(\r\x1a\xce\x04\n\x0cSerialConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x65\x63ho\x18\x02 \x01(\x08\x12\x0b\n\x03rxd\x18\x03 \x01(\r\x12\x0b\n\x03txd\x18\x04 \x01(\r\x12\x34\n\x04\x62\x61ud\x18\x05 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Baud\x12\x0f\n\x07timeout\x18\x06 \x01(\r\x12\x34\n\x04mode\x18\x07 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Mode\x12$\n\x1coverride_console_serial_port\x18\x08 \x01(\x08\"\x8a\x02\n\x0bSerial_Baud\x12\x10\n\x0c\x42\x41UD_DEFAULT\x10\x00\x12\x0c\n\x08\x42\x41UD_110\x10\x01\x12\x0c\n\x08\x42\x41UD_300\x10\x02\x12\x0c\n\x08\x42\x41UD_600\x10\x03\x12\r\n\tBAUD_1200\x10\x04\x12\r\n\tBAUD_2400\x10\x05\x12\r\n\tBAUD_4800\x10\x06\x12\r\n\tBAUD_9600\x10\x07\x12\x0e\n\nBAUD_19200\x10\x08\x12\x0e\n\nBAUD_38400\x10\t\x12\x0e\n\nBAUD_57600\x10\n\x12\x0f\n\x0b\x42\x41UD_115200\x10\x0b\x12\x0f\n\x0b\x42\x41UD_230400\x10\x0c\x12\x0f\n\x0b\x42\x41UD_460800\x10\r\x12\x0f\n\x0b\x42\x41UD_576000\x10\x0e\x12\x0f\n\x0b\x42\x41UD_921600\x10\x0f\"U\n\x0bSerial_Mode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06SIMPLE\x10\x01\x12\t\n\x05PROTO\x10\x02\x12\x0b\n\x07TEXTMSG\x10\x03\x12\x08\n\x04NMEA\x10\x04\x12\x0b\n\x07\x43\x41LTOPO\x10\x05\x1a\xe9\x02\n\x1a\x45xternalNotificationConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\toutput_ms\x18\x02 \x01(\r\x12\x0e\n\x06output\x18\x03 \x01(\r\x12\x14\n\x0coutput_vibra\x18\x08 \x01(\r\x12\x15\n\routput_buzzer\x18\t \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x15\n\ralert_message\x18\x05 \x01(\x08\x12\x1b\n\x13\x61lert_message_vibra\x18\n \x01(\x08\x12\x1c\n\x14\x61lert_message_buzzer\x18\x0b \x01(\x08\x12\x12\n\nalert_bell\x18\x06 \x01(\x08\x12\x18\n\x10\x61lert_bell_vibra\x18\x0c \x01(\x08\x12\x19\n\x11\x61lert_bell_buzzer\x18\r \x01(\x08\x12\x0f\n\x07use_pwm\x18\x07 \x01(\x08\x12\x13\n\x0bnag_timeout\x18\x0e \x01(\r\x12\x19\n\x11use_i2s_as_buzzer\x18\x0f \x01(\x08\x1a\x84\x01\n\x12StoreForwardConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\theartbeat\x18\x02 \x01(\x08\x12\x0f\n\x07records\x18\x03 \x01(\r\x12\x1a\n\x12history_return_max\x18\x04 \x01(\r\x12\x1d\n\x15history_return_window\x18\x05 \x01(\r\x1a@\n\x0fRangeTestConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06sender\x18\x02 \x01(\r\x12\x0c\n\x04save\x18\x03 \x01(\x08\x1a\xe6\x02\n\x0fTelemetryConfig\x12\x1e\n\x16\x64\x65vice_update_interval\x18\x01 \x01(\r\x12#\n\x1b\x65nvironment_update_interval\x18\x02 \x01(\r\x12\'\n\x1f\x65nvironment_measurement_enabled\x18\x03 \x01(\x08\x12\"\n\x1a\x65nvironment_screen_enabled\x18\x04 \x01(\x08\x12&\n\x1e\x65nvironment_display_fahrenheit\x18\x05 \x01(\x08\x12\x1b\n\x13\x61ir_quality_enabled\x18\x06 \x01(\x08\x12\x1c\n\x14\x61ir_quality_interval\x18\x07 \x01(\r\x12!\n\x19power_measurement_enabled\x18\x08 \x01(\x08\x12\x1d\n\x15power_update_interval\x18\t \x01(\r\x12\x1c\n\x14power_screen_enabled\x18\n \x01(\x08\x1a\xb5\x04\n\x13\x43\x61nnedMessageConfig\x12\x17\n\x0frotary1_enabled\x18\x01 \x01(\x08\x12\x19\n\x11inputbroker_pin_a\x18\x02 \x01(\r\x12\x19\n\x11inputbroker_pin_b\x18\x03 \x01(\r\x12\x1d\n\x15inputbroker_pin_press\x18\x04 \x01(\r\x12N\n\x14inputbroker_event_cw\x18\x05 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12O\n\x15inputbroker_event_ccw\x18\x06 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12Q\n\x17inputbroker_event_press\x18\x07 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12\x17\n\x0fupdown1_enabled\x18\x08 \x01(\x08\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x12\x1a\n\x12\x61llow_input_source\x18\n \x01(\t\x12\x11\n\tsend_bell\x18\x0b \x01(\x08\"c\n\x0eInputEventChar\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02UP\x10\x11\x12\x08\n\x04\x44OWN\x10\x12\x12\x08\n\x04LEFT\x10\x13\x12\t\n\x05RIGHT\x10\x14\x12\n\n\x06SELECT\x10\n\x12\x08\n\x04\x42\x41\x43K\x10\x1b\x12\n\n\x06\x43\x41NCEL\x10\x18\x1a\x65\n\x15\x41mbientLightingConfig\x12\x11\n\tled_state\x18\x01 \x01(\x08\x12\x0f\n\x07\x63urrent\x18\x02 \x01(\r\x12\x0b\n\x03red\x18\x03 \x01(\r\x12\r\n\x05green\x18\x04 \x01(\r\x12\x0c\n\x04\x62lue\x18\x05 \x01(\rB\x11\n\x0fpayload_variant\"Y\n\x11RemoteHardwarePin\x12\x10\n\x08gpio_pin\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12$\n\x04type\x18\x03 \x01(\x0e\x32\x16.RemoteHardwarePinType*I\n\x15RemoteHardwarePinType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0c\x44IGITAL_READ\x10\x01\x12\x11\n\rDIGITAL_WRITE\x10\x02\x42g\n\x13\x63om.geeksville.meshB\x12ModuleConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emeshtastic/module_config.proto\x12\nmeshtastic\"\xa4\"\n\x0cModuleConfig\x12\x33\n\x04mqtt\x18\x01 \x01(\x0b\x32#.meshtastic.ModuleConfig.MQTTConfigH\x00\x12\x37\n\x06serial\x18\x02 \x01(\x0b\x32%.meshtastic.ModuleConfig.SerialConfigH\x00\x12T\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32\x33.meshtastic.ModuleConfig.ExternalNotificationConfigH\x00\x12\x44\n\rstore_forward\x18\x04 \x01(\x0b\x32+.meshtastic.ModuleConfig.StoreForwardConfigH\x00\x12>\n\nrange_test\x18\x05 \x01(\x0b\x32(.meshtastic.ModuleConfig.RangeTestConfigH\x00\x12=\n\ttelemetry\x18\x06 \x01(\x0b\x32(.meshtastic.ModuleConfig.TelemetryConfigH\x00\x12\x46\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32,.meshtastic.ModuleConfig.CannedMessageConfigH\x00\x12\x35\n\x05\x61udio\x18\x08 \x01(\x0b\x32$.meshtastic.ModuleConfig.AudioConfigH\x00\x12H\n\x0fremote_hardware\x18\t \x01(\x0b\x32-.meshtastic.ModuleConfig.RemoteHardwareConfigH\x00\x12\x44\n\rneighbor_info\x18\n \x01(\x0b\x32+.meshtastic.ModuleConfig.NeighborInfoConfigH\x00\x12J\n\x10\x61mbient_lighting\x18\x0b \x01(\x0b\x32..meshtastic.ModuleConfig.AmbientLightingConfigH\x00\x12J\n\x10\x64\x65tection_sensor\x18\x0c \x01(\x0b\x32..meshtastic.ModuleConfig.DetectionSensorConfigH\x00\x12?\n\npaxcounter\x18\r \x01(\x0b\x32).meshtastic.ModuleConfig.PaxcounterConfigH\x00\x1a\xb0\x02\n\nMQTTConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x1a\n\x12\x65ncryption_enabled\x18\x05 \x01(\x08\x12\x14\n\x0cjson_enabled\x18\x06 \x01(\x08\x12\x13\n\x0btls_enabled\x18\x07 \x01(\x08\x12\x0c\n\x04root\x18\x08 \x01(\t\x12\x1f\n\x17proxy_to_client_enabled\x18\t \x01(\x08\x12\x1d\n\x15map_reporting_enabled\x18\n \x01(\x08\x12G\n\x13map_report_settings\x18\x0b \x01(\x0b\x32*.meshtastic.ModuleConfig.MapReportSettings\x1aN\n\x11MapReportSettings\x12\x1d\n\x15publish_interval_secs\x18\x01 \x01(\r\x12\x1a\n\x12position_precision\x18\x02 \x01(\r\x1a\x82\x01\n\x14RemoteHardwareConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x1a\x61llow_undefined_pin_access\x18\x02 \x01(\x08\x12\x35\n\x0e\x61vailable_pins\x18\x03 \x03(\x0b\x32\x1d.meshtastic.RemoteHardwarePin\x1a>\n\x12NeighborInfoConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\x0fupdate_interval\x18\x02 \x01(\r\x1a\xd2\x01\n\x15\x44\x65tectionSensorConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\x16minimum_broadcast_secs\x18\x02 \x01(\r\x12\x1c\n\x14state_broadcast_secs\x18\x03 \x01(\r\x12\x11\n\tsend_bell\x18\x04 \x01(\x08\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x13\n\x0bmonitor_pin\x18\x06 \x01(\r\x12 \n\x18\x64\x65tection_triggered_high\x18\x07 \x01(\x08\x12\x12\n\nuse_pullup\x18\x08 \x01(\x08\x1a\xe4\x02\n\x0b\x41udioConfig\x12\x16\n\x0e\x63odec2_enabled\x18\x01 \x01(\x08\x12\x0f\n\x07ptt_pin\x18\x02 \x01(\r\x12@\n\x07\x62itrate\x18\x03 \x01(\x0e\x32/.meshtastic.ModuleConfig.AudioConfig.Audio_Baud\x12\x0e\n\x06i2s_ws\x18\x04 \x01(\r\x12\x0e\n\x06i2s_sd\x18\x05 \x01(\r\x12\x0f\n\x07i2s_din\x18\x06 \x01(\r\x12\x0f\n\x07i2s_sck\x18\x07 \x01(\r\"\xa7\x01\n\nAudio_Baud\x12\x12\n\x0e\x43ODEC2_DEFAULT\x10\x00\x12\x0f\n\x0b\x43ODEC2_3200\x10\x01\x12\x0f\n\x0b\x43ODEC2_2400\x10\x02\x12\x0f\n\x0b\x43ODEC2_1600\x10\x03\x12\x0f\n\x0b\x43ODEC2_1400\x10\x04\x12\x0f\n\x0b\x43ODEC2_1300\x10\x05\x12\x0f\n\x0b\x43ODEC2_1200\x10\x06\x12\x0e\n\nCODEC2_700\x10\x07\x12\x0f\n\x0b\x43ODEC2_700B\x10\x08\x1aG\n\x10PaxcounterConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x1apaxcounter_update_interval\x18\x02 \x01(\r\x1a\xe4\x04\n\x0cSerialConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x65\x63ho\x18\x02 \x01(\x08\x12\x0b\n\x03rxd\x18\x03 \x01(\r\x12\x0b\n\x03txd\x18\x04 \x01(\r\x12?\n\x04\x62\x61ud\x18\x05 \x01(\x0e\x32\x31.meshtastic.ModuleConfig.SerialConfig.Serial_Baud\x12\x0f\n\x07timeout\x18\x06 \x01(\r\x12?\n\x04mode\x18\x07 \x01(\x0e\x32\x31.meshtastic.ModuleConfig.SerialConfig.Serial_Mode\x12$\n\x1coverride_console_serial_port\x18\x08 \x01(\x08\"\x8a\x02\n\x0bSerial_Baud\x12\x10\n\x0c\x42\x41UD_DEFAULT\x10\x00\x12\x0c\n\x08\x42\x41UD_110\x10\x01\x12\x0c\n\x08\x42\x41UD_300\x10\x02\x12\x0c\n\x08\x42\x41UD_600\x10\x03\x12\r\n\tBAUD_1200\x10\x04\x12\r\n\tBAUD_2400\x10\x05\x12\r\n\tBAUD_4800\x10\x06\x12\r\n\tBAUD_9600\x10\x07\x12\x0e\n\nBAUD_19200\x10\x08\x12\x0e\n\nBAUD_38400\x10\t\x12\x0e\n\nBAUD_57600\x10\n\x12\x0f\n\x0b\x42\x41UD_115200\x10\x0b\x12\x0f\n\x0b\x42\x41UD_230400\x10\x0c\x12\x0f\n\x0b\x42\x41UD_460800\x10\r\x12\x0f\n\x0b\x42\x41UD_576000\x10\x0e\x12\x0f\n\x0b\x42\x41UD_921600\x10\x0f\"U\n\x0bSerial_Mode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06SIMPLE\x10\x01\x12\t\n\x05PROTO\x10\x02\x12\x0b\n\x07TEXTMSG\x10\x03\x12\x08\n\x04NMEA\x10\x04\x12\x0b\n\x07\x43\x41LTOPO\x10\x05\x1a\xe9\x02\n\x1a\x45xternalNotificationConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\toutput_ms\x18\x02 \x01(\r\x12\x0e\n\x06output\x18\x03 \x01(\r\x12\x14\n\x0coutput_vibra\x18\x08 \x01(\r\x12\x15\n\routput_buzzer\x18\t \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x15\n\ralert_message\x18\x05 \x01(\x08\x12\x1b\n\x13\x61lert_message_vibra\x18\n \x01(\x08\x12\x1c\n\x14\x61lert_message_buzzer\x18\x0b \x01(\x08\x12\x12\n\nalert_bell\x18\x06 \x01(\x08\x12\x18\n\x10\x61lert_bell_vibra\x18\x0c \x01(\x08\x12\x19\n\x11\x61lert_bell_buzzer\x18\r \x01(\x08\x12\x0f\n\x07use_pwm\x18\x07 \x01(\x08\x12\x13\n\x0bnag_timeout\x18\x0e \x01(\r\x12\x19\n\x11use_i2s_as_buzzer\x18\x0f \x01(\x08\x1a\x84\x01\n\x12StoreForwardConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\theartbeat\x18\x02 \x01(\x08\x12\x0f\n\x07records\x18\x03 \x01(\r\x12\x1a\n\x12history_return_max\x18\x04 \x01(\r\x12\x1d\n\x15history_return_window\x18\x05 \x01(\r\x1a@\n\x0fRangeTestConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06sender\x18\x02 \x01(\r\x12\x0c\n\x04save\x18\x03 \x01(\x08\x1a\xe6\x02\n\x0fTelemetryConfig\x12\x1e\n\x16\x64\x65vice_update_interval\x18\x01 \x01(\r\x12#\n\x1b\x65nvironment_update_interval\x18\x02 \x01(\r\x12\'\n\x1f\x65nvironment_measurement_enabled\x18\x03 \x01(\x08\x12\"\n\x1a\x65nvironment_screen_enabled\x18\x04 \x01(\x08\x12&\n\x1e\x65nvironment_display_fahrenheit\x18\x05 \x01(\x08\x12\x1b\n\x13\x61ir_quality_enabled\x18\x06 \x01(\x08\x12\x1c\n\x14\x61ir_quality_interval\x18\x07 \x01(\r\x12!\n\x19power_measurement_enabled\x18\x08 \x01(\x08\x12\x1d\n\x15power_update_interval\x18\t \x01(\r\x12\x1c\n\x14power_screen_enabled\x18\n \x01(\x08\x1a\xd6\x04\n\x13\x43\x61nnedMessageConfig\x12\x17\n\x0frotary1_enabled\x18\x01 \x01(\x08\x12\x19\n\x11inputbroker_pin_a\x18\x02 \x01(\r\x12\x19\n\x11inputbroker_pin_b\x18\x03 \x01(\r\x12\x1d\n\x15inputbroker_pin_press\x18\x04 \x01(\r\x12Y\n\x14inputbroker_event_cw\x18\x05 \x01(\x0e\x32;.meshtastic.ModuleConfig.CannedMessageConfig.InputEventChar\x12Z\n\x15inputbroker_event_ccw\x18\x06 \x01(\x0e\x32;.meshtastic.ModuleConfig.CannedMessageConfig.InputEventChar\x12\\\n\x17inputbroker_event_press\x18\x07 \x01(\x0e\x32;.meshtastic.ModuleConfig.CannedMessageConfig.InputEventChar\x12\x17\n\x0fupdown1_enabled\x18\x08 \x01(\x08\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x12\x1a\n\x12\x61llow_input_source\x18\n \x01(\t\x12\x11\n\tsend_bell\x18\x0b \x01(\x08\"c\n\x0eInputEventChar\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02UP\x10\x11\x12\x08\n\x04\x44OWN\x10\x12\x12\x08\n\x04LEFT\x10\x13\x12\t\n\x05RIGHT\x10\x14\x12\n\n\x06SELECT\x10\n\x12\x08\n\x04\x42\x41\x43K\x10\x1b\x12\n\n\x06\x43\x41NCEL\x10\x18\x1a\x65\n\x15\x41mbientLightingConfig\x12\x11\n\tled_state\x18\x01 \x01(\x08\x12\x0f\n\x07\x63urrent\x18\x02 \x01(\r\x12\x0b\n\x03red\x18\x03 \x01(\r\x12\r\n\x05green\x18\x04 \x01(\r\x12\x0c\n\x04\x62lue\x18\x05 \x01(\rB\x11\n\x0fpayload_variant\"d\n\x11RemoteHardwarePin\x12\x10\n\x08gpio_pin\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12/\n\x04type\x18\x03 \x01(\x0e\x32!.meshtastic.RemoteHardwarePinType*I\n\x15RemoteHardwarePinType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0c\x44IGITAL_READ\x10\x01\x12\x11\n\rDIGITAL_WRITE\x10\x02\x42g\n\x13\x63om.geeksville.meshB\x12ModuleConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.module_config_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\022ModuleConfigProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _REMOTEHARDWAREPINTYPE._serialized_start=4284
-  _REMOTEHARDWAREPINTYPE._serialized_end=4357
-  _MODULECONFIG._serialized_start=35
-  _MODULECONFIG._serialized_end=4191
-  _MODULECONFIG_MQTTCONFIG._serialized_start=790
-  _MODULECONFIG_MQTTCONFIG._serialized_end=1083
-  _MODULECONFIG_MAPREPORTSETTINGS._serialized_start=1085
-  _MODULECONFIG_MAPREPORTSETTINGS._serialized_end=1163
-  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_start=1165
-  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_end=1284
-  _MODULECONFIG_NEIGHBORINFOCONFIG._serialized_start=1286
-  _MODULECONFIG_NEIGHBORINFOCONFIG._serialized_end=1348
-  _MODULECONFIG_DETECTIONSENSORCONFIG._serialized_start=1351
-  _MODULECONFIG_DETECTIONSENSORCONFIG._serialized_end=1561
-  _MODULECONFIG_AUDIOCONFIG._serialized_start=1564
-  _MODULECONFIG_AUDIOCONFIG._serialized_end=1909
-  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_start=1742
-  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_end=1909
-  _MODULECONFIG_PAXCOUNTERCONFIG._serialized_start=1911
-  _MODULECONFIG_PAXCOUNTERCONFIG._serialized_end=1982
-  _MODULECONFIG_SERIALCONFIG._serialized_start=1985
-  _MODULECONFIG_SERIALCONFIG._serialized_end=2575
-  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_start=2222
-  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_end=2488
-  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_start=2490
-  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_end=2575
-  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_start=2578
-  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_end=2939
-  _MODULECONFIG_STOREFORWARDCONFIG._serialized_start=2942
-  _MODULECONFIG_STOREFORWARDCONFIG._serialized_end=3074
-  _MODULECONFIG_RANGETESTCONFIG._serialized_start=3076
-  _MODULECONFIG_RANGETESTCONFIG._serialized_end=3140
-  _MODULECONFIG_TELEMETRYCONFIG._serialized_start=3143
-  _MODULECONFIG_TELEMETRYCONFIG._serialized_end=3501
-  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_start=3504
-  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_end=4069
-  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_start=3970
-  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_end=4069
-  _MODULECONFIG_AMBIENTLIGHTINGCONFIG._serialized_start=4071
-  _MODULECONFIG_AMBIENTLIGHTINGCONFIG._serialized_end=4172
-  _REMOTEHARDWAREPIN._serialized_start=4193
-  _REMOTEHARDWAREPIN._serialized_end=4282
+  _REMOTEHARDWAREPINTYPE._serialized_start=4539
+  _REMOTEHARDWAREPINTYPE._serialized_end=4612
+  _MODULECONFIG._serialized_start=47
+  _MODULECONFIG._serialized_end=4435
+  _MODULECONFIG_MQTTCONFIG._serialized_start=945
+  _MODULECONFIG_MQTTCONFIG._serialized_end=1249
+  _MODULECONFIG_MAPREPORTSETTINGS._serialized_start=1251
+  _MODULECONFIG_MAPREPORTSETTINGS._serialized_end=1329
+  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_start=1332
+  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_end=1462
+  _MODULECONFIG_NEIGHBORINFOCONFIG._serialized_start=1464
+  _MODULECONFIG_NEIGHBORINFOCONFIG._serialized_end=1526
+  _MODULECONFIG_DETECTIONSENSORCONFIG._serialized_start=1529
+  _MODULECONFIG_DETECTIONSENSORCONFIG._serialized_end=1739
+  _MODULECONFIG_AUDIOCONFIG._serialized_start=1742
+  _MODULECONFIG_AUDIOCONFIG._serialized_end=2098
+  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_start=1931
+  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_end=2098
+  _MODULECONFIG_PAXCOUNTERCONFIG._serialized_start=2100
+  _MODULECONFIG_PAXCOUNTERCONFIG._serialized_end=2171
+  _MODULECONFIG_SERIALCONFIG._serialized_start=2174
+  _MODULECONFIG_SERIALCONFIG._serialized_end=2786
+  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_start=2433
+  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_end=2699
+  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_start=2701
+  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_end=2786
+  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_start=2789
+  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_end=3150
+  _MODULECONFIG_STOREFORWARDCONFIG._serialized_start=3153
+  _MODULECONFIG_STOREFORWARDCONFIG._serialized_end=3285
+  _MODULECONFIG_RANGETESTCONFIG._serialized_start=3287
+  _MODULECONFIG_RANGETESTCONFIG._serialized_end=3351
+  _MODULECONFIG_TELEMETRYCONFIG._serialized_start=3354
+  _MODULECONFIG_TELEMETRYCONFIG._serialized_end=3712
+  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_start=3715
+  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_end=4313
+  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_start=4214
+  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_end=4313
+  _MODULECONFIG_AMBIENTLIGHTINGCONFIG._serialized_start=4315
+  _MODULECONFIG_AMBIENTLIGHTINGCONFIG._serialized_end=4416
+  _REMOTEHARDWAREPIN._serialized_start=4437
+  _REMOTEHARDWAREPIN._serialized_end=4537
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/mqtt_pb2.py` & `meshtastic-2.3.4/meshtastic/mqtt_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from meshtastic import mesh_pb2 as meshtastic_dot_mesh__pb2
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
+from meshtastic import mesh_pb2 as meshtastic_dot_mesh__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mqtt.proto\x1a\x15meshtastic/mesh.proto\x1a\x17meshtastic/config.proto\"V\n\x0fServiceEnvelope\x12\x1b\n\x06packet\x18\x01 \x01(\x0b\x32\x0b.MeshPacket\x12\x12\n\nchannel_id\x18\x02 \x01(\t\x12\x12\n\ngateway_id\x18\x03 \x01(\t\"\x90\x03\n\tMapReport\x12\x11\n\tlong_name\x18\x01 \x01(\t\x12\x12\n\nshort_name\x18\x02 \x01(\t\x12\'\n\x04role\x18\x03 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12 \n\x08hw_model\x18\x04 \x01(\x0e\x32\x0e.HardwareModel\x12\x18\n\x10\x66irmware_version\x18\x05 \x01(\t\x12-\n\x06region\x18\x06 \x01(\x0e\x32\x1d.Config.LoRaConfig.RegionCode\x12\x34\n\x0cmodem_preset\x18\x07 \x01(\x0e\x32\x1e.Config.LoRaConfig.ModemPreset\x12\x1b\n\x13has_default_channel\x18\x08 \x01(\x08\x12\x12\n\nlatitude_i\x18\t \x01(\x0f\x12\x13\n\x0blongitude_i\x18\n \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x0b \x01(\x05\x12\x1a\n\x12position_precision\x18\x0c \x01(\r\x12\x1e\n\x16num_online_local_nodes\x18\r \x01(\rB_\n\x13\x63om.geeksville.meshB\nMQTTProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mqtt.proto\x12\nmeshtastic\x1a\x17meshtastic/config.proto\x1a\x15meshtastic/mesh.proto\"a\n\x0fServiceEnvelope\x12&\n\x06packet\x18\x01 \x01(\x0b\x32\x16.meshtastic.MeshPacket\x12\x12\n\nchannel_id\x18\x02 \x01(\t\x12\x12\n\ngateway_id\x18\x03 \x01(\t\"\xbc\x03\n\tMapReport\x12\x11\n\tlong_name\x18\x01 \x01(\t\x12\x12\n\nshort_name\x18\x02 \x01(\t\x12\x32\n\x04role\x18\x03 \x01(\x0e\x32$.meshtastic.Config.DeviceConfig.Role\x12+\n\x08hw_model\x18\x04 \x01(\x0e\x32\x19.meshtastic.HardwareModel\x12\x18\n\x10\x66irmware_version\x18\x05 \x01(\t\x12\x38\n\x06region\x18\x06 \x01(\x0e\x32(.meshtastic.Config.LoRaConfig.RegionCode\x12?\n\x0cmodem_preset\x18\x07 \x01(\x0e\x32).meshtastic.Config.LoRaConfig.ModemPreset\x12\x1b\n\x13has_default_channel\x18\x08 \x01(\x08\x12\x12\n\nlatitude_i\x18\t \x01(\x0f\x12\x13\n\x0blongitude_i\x18\n \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x0b \x01(\x05\x12\x1a\n\x12position_precision\x18\x0c \x01(\r\x12\x1e\n\x16num_online_local_nodes\x18\r \x01(\rB_\n\x13\x63om.geeksville.meshB\nMQTTProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.mqtt_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\nMQTTProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _SERVICEENVELOPE._serialized_start=73
-  _SERVICEENVELOPE._serialized_end=159
-  _MAPREPORT._serialized_start=162
-  _MAPREPORT._serialized_end=562
+  _SERVICEENVELOPE._serialized_start=85
+  _SERVICEENVELOPE._serialized_end=182
+  _MAPREPORT._serialized_start=185
+  _MAPREPORT._serialized_end=629
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/nanopb_pb2.py` & `meshtastic-2.3.4/meshtastic/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.3/meshtastic/node.py` & `meshtastic-2.3.4/meshtastic/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Node class
 """
 
 import base64
 import logging
 import time
 
-from google.protobuf.json_format import MessageToJson
-
 from meshtastic import admin_pb2, apponly_pb2, channel_pb2, localonly_pb2, portnums_pb2
 from meshtastic.util import (
     Timeout,
     camel_to_snake,
     fromPSK,
     our_exit,
     pskToString,
     stripnl,
+    message_to_json,
 )
 
 
 class Node:
     """A model of a (local or remote) node in the mesh
 
     Includes methods for localConfig, moduleConfig and channels
@@ -43,16 +42,15 @@
 
     def showChannels(self):
         """Show human readable description of our channels."""
         print("Channels:")
         if self.channels:
             logging.debug(f"self.channels:{self.channels}")
             for c in self.channels:
-                # print('c.settings.psk:', c.settings.psk)
-                cStr = stripnl(MessageToJson(c.settings))
+                cStr = message_to_json(c.settings)
                 # don't show disabled channels
                 if channel_pb2.Channel.Role.Name(c.role) != "DISABLED":
                     print(
                         f"  Index {c.index}: {channel_pb2.Channel.Role.Name(c.role)} psk={pskToString(c.settings.psk)} {cStr}"
                     )
         publicURL = self.getURL(includeAll=False)
         adminURL = self.getURL(includeAll=True)
@@ -60,19 +58,19 @@
         if adminURL != publicURL:
             print(f"Complete URL (includes all channels): {adminURL}")
 
     def showInfo(self):
         """Show human readable description of our node"""
         prefs = ""
         if self.localConfig:
-            prefs = stripnl(MessageToJson(self.localConfig))
+            prefs = message_to_json(self.localConfig)
         print(f"Preferences: {prefs}\n")
         prefs = ""
         if self.moduleConfig:
-            prefs = stripnl(MessageToJson(self.moduleConfig))
+            prefs = message_to_json(self.moduleConfig)
         print(f"Module preferences: {prefs}\n")
         self.showChannels()
 
     def requestChannels(self):
         """Send regular MeshPackets to ask channels."""
         logging.debug(f"requestChannels for nodeNum:{self.nodeNum}")
         self.channels = None
@@ -119,15 +117,15 @@
         if self == self.iface.localNode:
             onResponse = None
         else:
             onResponse = self.onResponseRequestSettings
             print("Requesting current config from remote node (this can take a while).")
 
         msgIndex = configType.index
-        if configType.containing_type.full_name == "LocalConfig":
+        if configType.containing_type.full_name in ("meshtastic.LocalConfig", "LocalConfig"):
             p = admin_pb2.AdminMessage()
             p.get_config_request = msgIndex
             self._sendAdmin(p, wantResponse=True, onResponse=onResponse)
         else:
             p = admin_pb2.AdminMessage()
             p.get_module_config_request = msgIndex
             self._sendAdmin(p, wantResponse=True, onResponse=onResponse)
```

### Comparing `meshtastic-2.3.3/meshtastic/paxcount_pb2.py` & `meshtastic-2.3.4/meshtastic/paxcount_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19meshtastic/paxcount.proto\"5\n\x08Paxcount\x12\x0c\n\x04wifi\x18\x01 \x01(\r\x12\x0b\n\x03\x62le\x18\x02 \x01(\r\x12\x0e\n\x06uptime\x18\x03 \x01(\rBc\n\x13\x63om.geeksville.meshB\x0ePaxcountProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19meshtastic/paxcount.proto\x12\nmeshtastic\"5\n\x08Paxcount\x12\x0c\n\x04wifi\x18\x01 \x01(\r\x12\x0b\n\x03\x62le\x18\x02 \x01(\r\x12\x0e\n\x06uptime\x18\x03 \x01(\rBc\n\x13\x63om.geeksville.meshB\x0ePaxcountProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.paxcount_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\016PaxcountProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _PAXCOUNT._serialized_start=29
-  _PAXCOUNT._serialized_end=82
+  _PAXCOUNT._serialized_start=41
+  _PAXCOUNT._serialized_end=94
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/portnums_pb2.py` & `meshtastic-2.3.4/meshtastic/portnums_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19meshtastic/portnums.proto*\x8d\x04\n\x07PortNum\x12\x0f\n\x0bUNKNOWN_APP\x10\x00\x12\x14\n\x10TEXT_MESSAGE_APP\x10\x01\x12\x17\n\x13REMOTE_HARDWARE_APP\x10\x02\x12\x10\n\x0cPOSITION_APP\x10\x03\x12\x10\n\x0cNODEINFO_APP\x10\x04\x12\x0f\n\x0bROUTING_APP\x10\x05\x12\r\n\tADMIN_APP\x10\x06\x12\x1f\n\x1bTEXT_MESSAGE_COMPRESSED_APP\x10\x07\x12\x10\n\x0cWAYPOINT_APP\x10\x08\x12\r\n\tAUDIO_APP\x10\t\x12\x18\n\x14\x44\x45TECTION_SENSOR_APP\x10\n\x12\r\n\tREPLY_APP\x10 \x12\x11\n\rIP_TUNNEL_APP\x10!\x12\x12\n\x0ePAXCOUNTER_APP\x10\"\x12\x0e\n\nSERIAL_APP\x10@\x12\x15\n\x11STORE_FORWARD_APP\x10\x41\x12\x12\n\x0eRANGE_TEST_APP\x10\x42\x12\x11\n\rTELEMETRY_APP\x10\x43\x12\x0b\n\x07ZPS_APP\x10\x44\x12\x11\n\rSIMULATOR_APP\x10\x45\x12\x12\n\x0eTRACEROUTE_APP\x10\x46\x12\x14\n\x10NEIGHBORINFO_APP\x10G\x12\x0f\n\x0b\x41TAK_PLUGIN\x10H\x12\x12\n\x0eMAP_REPORT_APP\x10I\x12\x10\n\x0bPRIVATE_APP\x10\x80\x02\x12\x13\n\x0e\x41TAK_FORWARDER\x10\x81\x02\x12\x08\n\x03MAX\x10\xff\x03\x42]\n\x13\x63om.geeksville.meshB\x08PortnumsZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19meshtastic/portnums.proto\x12\nmeshtastic*\x8d\x04\n\x07PortNum\x12\x0f\n\x0bUNKNOWN_APP\x10\x00\x12\x14\n\x10TEXT_MESSAGE_APP\x10\x01\x12\x17\n\x13REMOTE_HARDWARE_APP\x10\x02\x12\x10\n\x0cPOSITION_APP\x10\x03\x12\x10\n\x0cNODEINFO_APP\x10\x04\x12\x0f\n\x0bROUTING_APP\x10\x05\x12\r\n\tADMIN_APP\x10\x06\x12\x1f\n\x1bTEXT_MESSAGE_COMPRESSED_APP\x10\x07\x12\x10\n\x0cWAYPOINT_APP\x10\x08\x12\r\n\tAUDIO_APP\x10\t\x12\x18\n\x14\x44\x45TECTION_SENSOR_APP\x10\n\x12\r\n\tREPLY_APP\x10 \x12\x11\n\rIP_TUNNEL_APP\x10!\x12\x12\n\x0ePAXCOUNTER_APP\x10\"\x12\x0e\n\nSERIAL_APP\x10@\x12\x15\n\x11STORE_FORWARD_APP\x10\x41\x12\x12\n\x0eRANGE_TEST_APP\x10\x42\x12\x11\n\rTELEMETRY_APP\x10\x43\x12\x0b\n\x07ZPS_APP\x10\x44\x12\x11\n\rSIMULATOR_APP\x10\x45\x12\x12\n\x0eTRACEROUTE_APP\x10\x46\x12\x14\n\x10NEIGHBORINFO_APP\x10G\x12\x0f\n\x0b\x41TAK_PLUGIN\x10H\x12\x12\n\x0eMAP_REPORT_APP\x10I\x12\x10\n\x0bPRIVATE_APP\x10\x80\x02\x12\x13\n\x0e\x41TAK_FORWARDER\x10\x81\x02\x12\x08\n\x03MAX\x10\xff\x03\x42]\n\x13\x63om.geeksville.meshB\x08PortnumsZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.portnums_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\010PortnumsZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _PORTNUM._serialized_start=30
-  _PORTNUM._serialized_end=555
+  _PORTNUM._serialized_start=42
+  _PORTNUM._serialized_end=567
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/remote_hardware.py` & `meshtastic-2.3.4/meshtastic/remote_hardware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Remote hardware
 """
 import logging
 
-from pubsub import pub
+from pubsub import pub # type: ignore[import-untyped]
 
 from meshtastic import portnums_pb2, remote_hardware_pb2
 from meshtastic.util import our_exit
 
 
 def onGPIOreceive(packet, interface):
     """Callback for received GPIO responses"""
```

### Comparing `meshtastic-2.3.3/meshtastic/remote_hardware_pb2.py` & `meshtastic-2.3.4/meshtastic/remote_hardware_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n meshtastic/remote_hardware.proto\"\xcb\x01\n\x0fHardwareMessage\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.HardwareMessage.Type\x12\x11\n\tgpio_mask\x18\x02 \x01(\x04\x12\x12\n\ngpio_value\x18\x03 \x01(\x04\"l\n\x04Type\x12\t\n\x05UNSET\x10\x00\x12\x0f\n\x0bWRITE_GPIOS\x10\x01\x12\x0f\n\x0bWATCH_GPIOS\x10\x02\x12\x11\n\rGPIOS_CHANGED\x10\x03\x12\x0e\n\nREAD_GPIOS\x10\x04\x12\x14\n\x10READ_GPIOS_REPLY\x10\x05\x42\x63\n\x13\x63om.geeksville.meshB\x0eRemoteHardwareZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n meshtastic/remote_hardware.proto\x12\nmeshtastic\"\xd6\x01\n\x0fHardwareMessage\x12.\n\x04type\x18\x01 \x01(\x0e\x32 .meshtastic.HardwareMessage.Type\x12\x11\n\tgpio_mask\x18\x02 \x01(\x04\x12\x12\n\ngpio_value\x18\x03 \x01(\x04\"l\n\x04Type\x12\t\n\x05UNSET\x10\x00\x12\x0f\n\x0bWRITE_GPIOS\x10\x01\x12\x0f\n\x0bWATCH_GPIOS\x10\x02\x12\x11\n\rGPIOS_CHANGED\x10\x03\x12\x0e\n\nREAD_GPIOS\x10\x04\x12\x14\n\x10READ_GPIOS_REPLY\x10\x05\x42\x63\n\x13\x63om.geeksville.meshB\x0eRemoteHardwareZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.remote_hardware_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\016RemoteHardwareZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _HARDWAREMESSAGE._serialized_start=37
-  _HARDWAREMESSAGE._serialized_end=240
-  _HARDWAREMESSAGE_TYPE._serialized_start=132
-  _HARDWAREMESSAGE_TYPE._serialized_end=240
+  _HARDWAREMESSAGE._serialized_start=49
+  _HARDWAREMESSAGE._serialized_end=263
+  _HARDWAREMESSAGE_TYPE._serialized_start=155
+  _HARDWAREMESSAGE_TYPE._serialized_end=263
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/rtttl_pb2.py` & `meshtastic-2.3.4/meshtastic/rtttl_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16meshtastic/rtttl.proto\"\x1f\n\x0bRTTTLConfig\x12\x10\n\x08ringtone\x18\x01 \x01(\tBf\n\x13\x63om.geeksville.meshB\x11RTTTLConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16meshtastic/rtttl.proto\x12\nmeshtastic\"\x1f\n\x0bRTTTLConfig\x12\x10\n\x08ringtone\x18\x01 \x01(\tBf\n\x13\x63om.geeksville.meshB\x11RTTTLConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.rtttl_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\021RTTTLConfigProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _RTTTLCONFIG._serialized_start=26
-  _RTTTLCONFIG._serialized_end=57
+  _RTTTLCONFIG._serialized_start=38
+  _RTTTLCONFIG._serialized_end=69
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/serial_interface.py` & `meshtastic-2.3.4/meshtastic/serial_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Serial interface class
 """
 import logging
 import platform
 import time
 
-import serial
+import serial # type: ignore[import-untyped]
 
 import meshtastic.util
 from meshtastic.stream_interface import StreamInterface
 
 if platform.system() != "Windows":
     import termios
```

### Comparing `meshtastic-2.3.3/meshtastic/storeforward_pb2.py` & `meshtastic-2.3.4/meshtastic/storeforward_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dmeshtastic/storeforward.proto\"\xf0\x06\n\x0fStoreAndForward\x12,\n\x02rr\x18\x01 \x01(\x0e\x32 .StoreAndForward.RequestResponse\x12,\n\x05stats\x18\x02 \x01(\x0b\x32\x1b.StoreAndForward.StatisticsH\x00\x12+\n\x07history\x18\x03 \x01(\x0b\x32\x18.StoreAndForward.HistoryH\x00\x12/\n\theartbeat\x18\x04 \x01(\x0b\x32\x1a.StoreAndForward.HeartbeatH\x00\x12\x0e\n\x04text\x18\x05 \x01(\x0cH\x00\x1a\xcd\x01\n\nStatistics\x12\x16\n\x0emessages_total\x18\x01 \x01(\r\x12\x16\n\x0emessages_saved\x18\x02 \x01(\r\x12\x14\n\x0cmessages_max\x18\x03 \x01(\r\x12\x0f\n\x07up_time\x18\x04 \x01(\r\x12\x10\n\x08requests\x18\x05 \x01(\r\x12\x18\n\x10requests_history\x18\x06 \x01(\r\x12\x11\n\theartbeat\x18\x07 \x01(\x08\x12\x12\n\nreturn_max\x18\x08 \x01(\r\x12\x15\n\rreturn_window\x18\t \x01(\r\x1aI\n\x07History\x12\x18\n\x10history_messages\x18\x01 \x01(\r\x12\x0e\n\x06window\x18\x02 \x01(\r\x12\x14\n\x0clast_request\x18\x03 \x01(\r\x1a.\n\tHeartbeat\x12\x0e\n\x06period\x18\x01 \x01(\r\x12\x11\n\tsecondary\x18\x02 \x01(\r\"\xbc\x02\n\x0fRequestResponse\x12\t\n\x05UNSET\x10\x00\x12\x10\n\x0cROUTER_ERROR\x10\x01\x12\x14\n\x10ROUTER_HEARTBEAT\x10\x02\x12\x0f\n\x0bROUTER_PING\x10\x03\x12\x0f\n\x0bROUTER_PONG\x10\x04\x12\x0f\n\x0bROUTER_BUSY\x10\x05\x12\x12\n\x0eROUTER_HISTORY\x10\x06\x12\x10\n\x0cROUTER_STATS\x10\x07\x12\x16\n\x12ROUTER_TEXT_DIRECT\x10\x08\x12\x19\n\x15ROUTER_TEXT_BROADCAST\x10\t\x12\x10\n\x0c\x43LIENT_ERROR\x10@\x12\x12\n\x0e\x43LIENT_HISTORY\x10\x41\x12\x10\n\x0c\x43LIENT_STATS\x10\x42\x12\x0f\n\x0b\x43LIENT_PING\x10\x43\x12\x0f\n\x0b\x43LIENT_PONG\x10\x44\x12\x10\n\x0c\x43LIENT_ABORT\x10jB\t\n\x07variantBj\n\x13\x63om.geeksville.meshB\x15StoreAndForwardProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dmeshtastic/storeforward.proto\x12\nmeshtastic\"\x9c\x07\n\x0fStoreAndForward\x12\x37\n\x02rr\x18\x01 \x01(\x0e\x32+.meshtastic.StoreAndForward.RequestResponse\x12\x37\n\x05stats\x18\x02 \x01(\x0b\x32&.meshtastic.StoreAndForward.StatisticsH\x00\x12\x36\n\x07history\x18\x03 \x01(\x0b\x32#.meshtastic.StoreAndForward.HistoryH\x00\x12:\n\theartbeat\x18\x04 \x01(\x0b\x32%.meshtastic.StoreAndForward.HeartbeatH\x00\x12\x0e\n\x04text\x18\x05 \x01(\x0cH\x00\x1a\xcd\x01\n\nStatistics\x12\x16\n\x0emessages_total\x18\x01 \x01(\r\x12\x16\n\x0emessages_saved\x18\x02 \x01(\r\x12\x14\n\x0cmessages_max\x18\x03 \x01(\r\x12\x0f\n\x07up_time\x18\x04 \x01(\r\x12\x10\n\x08requests\x18\x05 \x01(\r\x12\x18\n\x10requests_history\x18\x06 \x01(\r\x12\x11\n\theartbeat\x18\x07 \x01(\x08\x12\x12\n\nreturn_max\x18\x08 \x01(\r\x12\x15\n\rreturn_window\x18\t \x01(\r\x1aI\n\x07History\x12\x18\n\x10history_messages\x18\x01 \x01(\r\x12\x0e\n\x06window\x18\x02 \x01(\r\x12\x14\n\x0clast_request\x18\x03 \x01(\r\x1a.\n\tHeartbeat\x12\x0e\n\x06period\x18\x01 \x01(\r\x12\x11\n\tsecondary\x18\x02 \x01(\r\"\xbc\x02\n\x0fRequestResponse\x12\t\n\x05UNSET\x10\x00\x12\x10\n\x0cROUTER_ERROR\x10\x01\x12\x14\n\x10ROUTER_HEARTBEAT\x10\x02\x12\x0f\n\x0bROUTER_PING\x10\x03\x12\x0f\n\x0bROUTER_PONG\x10\x04\x12\x0f\n\x0bROUTER_BUSY\x10\x05\x12\x12\n\x0eROUTER_HISTORY\x10\x06\x12\x10\n\x0cROUTER_STATS\x10\x07\x12\x16\n\x12ROUTER_TEXT_DIRECT\x10\x08\x12\x19\n\x15ROUTER_TEXT_BROADCAST\x10\t\x12\x10\n\x0c\x43LIENT_ERROR\x10@\x12\x12\n\x0e\x43LIENT_HISTORY\x10\x41\x12\x10\n\x0c\x43LIENT_STATS\x10\x42\x12\x0f\n\x0b\x43LIENT_PING\x10\x43\x12\x0f\n\x0b\x43LIENT_PONG\x10\x44\x12\x10\n\x0c\x43LIENT_ABORT\x10jB\t\n\x07variantBj\n\x13\x63om.geeksville.meshB\x15StoreAndForwardProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.storeforward_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\025StoreAndForwardProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _STOREANDFORWARD._serialized_start=34
-  _STOREANDFORWARD._serialized_end=914
-  _STOREANDFORWARD_STATISTICS._serialized_start=256
-  _STOREANDFORWARD_STATISTICS._serialized_end=461
-  _STOREANDFORWARD_HISTORY._serialized_start=463
-  _STOREANDFORWARD_HISTORY._serialized_end=536
-  _STOREANDFORWARD_HEARTBEAT._serialized_start=538
-  _STOREANDFORWARD_HEARTBEAT._serialized_end=584
-  _STOREANDFORWARD_REQUESTRESPONSE._serialized_start=587
-  _STOREANDFORWARD_REQUESTRESPONSE._serialized_end=903
+  _STOREANDFORWARD._serialized_start=46
+  _STOREANDFORWARD._serialized_end=970
+  _STOREANDFORWARD_STATISTICS._serialized_start=312
+  _STOREANDFORWARD_STATISTICS._serialized_end=517
+  _STOREANDFORWARD_HISTORY._serialized_start=519
+  _STOREANDFORWARD_HISTORY._serialized_end=592
+  _STOREANDFORWARD_HEARTBEAT._serialized_start=594
+  _STOREANDFORWARD_HEARTBEAT._serialized_end=640
+  _STOREANDFORWARD_REQUESTRESPONSE._serialized_start=643
+  _STOREANDFORWARD_REQUESTRESPONSE._serialized_end=959
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/stream_interface.py` & `meshtastic-2.3.4/meshtastic/stream_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Stream Interface base class
 """
 import logging
 import threading
 import time
 import traceback
 
-import serial
+import serial # type: ignore[import-untyped]
 
 from meshtastic.mesh_interface import MeshInterface
 from meshtastic.util import is_windows11, stripnl
 
 START1 = 0x94
 START2 = 0xC3
 HEADER_LEN = 4
```

### Comparing `meshtastic-2.3.3/meshtastic/supported_device.py` & `meshtastic-2.3.4/meshtastic/supported_device.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.3/meshtastic/tcp_interface.py` & `meshtastic-2.3.4/meshtastic/tcp_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """TCPInterface class for interfacing with http endpoint
 """
 import logging
 import socket
-from typing import AnyStr
+from typing import Optional
 
 from meshtastic.stream_interface import StreamInterface
 
 
 class TCPInterface(StreamInterface):
     """Interface class for meshtastic devices over a TCP link"""
 
     def __init__(
         self,
-        hostname: AnyStr,
+        hostname: str,
         debugOut=None,
         noProto=False,
         connectNow=True,
         portNumber=4403,
     ):
         """Constructor, opens a connection to a specified IP address/hostname
 
@@ -26,18 +26,18 @@
 
         self.stream = None
 
         self.hostname = hostname
         self.portNumber = portNumber
 
         if connectNow:
-            logging.debug(f"Connecting to {hostname}")
+            logging.debug(f"Connecting to {hostname}") # type: ignore[str-bytes-safe]
             server_address = (hostname, portNumber)
             sock = socket.create_connection(server_address)
-            self.socket = sock
+            self.socket: Optional[socket.socket] = sock
         else:
             self.socket = None
 
         StreamInterface.__init__(
             self, debugOut=debugOut, noProto=noProto, connectNow=connectNow
         )
```

### Comparing `meshtastic-2.3.3/meshtastic/telemetry_pb2.py` & `meshtastic-2.3.4/meshtastic/telemetry_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ameshtastic/telemetry.proto\"i\n\rDeviceMetrics\x12\x15\n\rbattery_level\x18\x01 \x01(\r\x12\x0f\n\x07voltage\x18\x02 \x01(\x02\x12\x1b\n\x13\x63hannel_utilization\x18\x03 \x01(\x02\x12\x13\n\x0b\x61ir_util_tx\x18\x04 \x01(\x02\"\x9b\x01\n\x12\x45nvironmentMetrics\x12\x13\n\x0btemperature\x18\x01 \x01(\x02\x12\x19\n\x11relative_humidity\x18\x02 \x01(\x02\x12\x1b\n\x13\x62\x61rometric_pressure\x18\x03 \x01(\x02\x12\x16\n\x0egas_resistance\x18\x04 \x01(\x02\x12\x0f\n\x07voltage\x18\x05 \x01(\x02\x12\x0f\n\x07\x63urrent\x18\x06 \x01(\x02\"\x8c\x01\n\x0cPowerMetrics\x12\x13\n\x0b\x63h1_voltage\x18\x01 \x01(\x02\x12\x13\n\x0b\x63h1_current\x18\x02 \x01(\x02\x12\x13\n\x0b\x63h2_voltage\x18\x03 \x01(\x02\x12\x13\n\x0b\x63h2_current\x18\x04 \x01(\x02\x12\x13\n\x0b\x63h3_voltage\x18\x05 \x01(\x02\x12\x13\n\x0b\x63h3_current\x18\x06 \x01(\x02\"\xbf\x02\n\x11\x41irQualityMetrics\x12\x15\n\rpm10_standard\x18\x01 \x01(\r\x12\x15\n\rpm25_standard\x18\x02 \x01(\r\x12\x16\n\x0epm100_standard\x18\x03 \x01(\r\x12\x1a\n\x12pm10_environmental\x18\x04 \x01(\r\x12\x1a\n\x12pm25_environmental\x18\x05 \x01(\r\x12\x1b\n\x13pm100_environmental\x18\x06 \x01(\r\x12\x16\n\x0eparticles_03um\x18\x07 \x01(\r\x12\x16\n\x0eparticles_05um\x18\x08 \x01(\r\x12\x16\n\x0eparticles_10um\x18\t \x01(\r\x12\x16\n\x0eparticles_25um\x18\n \x01(\r\x12\x16\n\x0eparticles_50um\x18\x0b \x01(\r\x12\x17\n\x0fparticles_100um\x18\x0c \x01(\r\"\xdd\x01\n\tTelemetry\x12\x0c\n\x04time\x18\x01 \x01(\x07\x12(\n\x0e\x64\x65vice_metrics\x18\x02 \x01(\x0b\x32\x0e.DeviceMetricsH\x00\x12\x32\n\x13\x65nvironment_metrics\x18\x03 \x01(\x0b\x32\x13.EnvironmentMetricsH\x00\x12\x31\n\x13\x61ir_quality_metrics\x18\x04 \x01(\x0b\x32\x12.AirQualityMetricsH\x00\x12&\n\rpower_metrics\x18\x05 \x01(\x0b\x32\r.PowerMetricsH\x00\x42\t\n\x07variant*\xe0\x01\n\x13TelemetrySensorType\x12\x10\n\x0cSENSOR_UNSET\x10\x00\x12\n\n\x06\x42ME280\x10\x01\x12\n\n\x06\x42ME680\x10\x02\x12\x0b\n\x07MCP9808\x10\x03\x12\n\n\x06INA260\x10\x04\x12\n\n\x06INA219\x10\x05\x12\n\n\x06\x42MP280\x10\x06\x12\t\n\x05SHTC3\x10\x07\x12\t\n\x05LPS22\x10\x08\x12\x0b\n\x07QMC6310\x10\t\x12\x0b\n\x07QMI8658\x10\n\x12\x0c\n\x08QMC5883L\x10\x0b\x12\t\n\x05SHT31\x10\x0c\x12\x0c\n\x08PMSA003I\x10\r\x12\x0b\n\x07INA3221\x10\x0e\x12\n\n\x06\x42MP085\x10\x0f\x42\x64\n\x13\x63om.geeksville.meshB\x0fTelemetryProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ameshtastic/telemetry.proto\x12\nmeshtastic\"i\n\rDeviceMetrics\x12\x15\n\rbattery_level\x18\x01 \x01(\r\x12\x0f\n\x07voltage\x18\x02 \x01(\x02\x12\x1b\n\x13\x63hannel_utilization\x18\x03 \x01(\x02\x12\x13\n\x0b\x61ir_util_tx\x18\x04 \x01(\x02\"\x9b\x01\n\x12\x45nvironmentMetrics\x12\x13\n\x0btemperature\x18\x01 \x01(\x02\x12\x19\n\x11relative_humidity\x18\x02 \x01(\x02\x12\x1b\n\x13\x62\x61rometric_pressure\x18\x03 \x01(\x02\x12\x16\n\x0egas_resistance\x18\x04 \x01(\x02\x12\x0f\n\x07voltage\x18\x05 \x01(\x02\x12\x0f\n\x07\x63urrent\x18\x06 \x01(\x02\"\x8c\x01\n\x0cPowerMetrics\x12\x13\n\x0b\x63h1_voltage\x18\x01 \x01(\x02\x12\x13\n\x0b\x63h1_current\x18\x02 \x01(\x02\x12\x13\n\x0b\x63h2_voltage\x18\x03 \x01(\x02\x12\x13\n\x0b\x63h2_current\x18\x04 \x01(\x02\x12\x13\n\x0b\x63h3_voltage\x18\x05 \x01(\x02\x12\x13\n\x0b\x63h3_current\x18\x06 \x01(\x02\"\xbf\x02\n\x11\x41irQualityMetrics\x12\x15\n\rpm10_standard\x18\x01 \x01(\r\x12\x15\n\rpm25_standard\x18\x02 \x01(\r\x12\x16\n\x0epm100_standard\x18\x03 \x01(\r\x12\x1a\n\x12pm10_environmental\x18\x04 \x01(\r\x12\x1a\n\x12pm25_environmental\x18\x05 \x01(\r\x12\x1b\n\x13pm100_environmental\x18\x06 \x01(\r\x12\x16\n\x0eparticles_03um\x18\x07 \x01(\r\x12\x16\n\x0eparticles_05um\x18\x08 \x01(\r\x12\x16\n\x0eparticles_10um\x18\t \x01(\r\x12\x16\n\x0eparticles_25um\x18\n \x01(\r\x12\x16\n\x0eparticles_50um\x18\x0b \x01(\r\x12\x17\n\x0fparticles_100um\x18\x0c \x01(\r\"\x89\x02\n\tTelemetry\x12\x0c\n\x04time\x18\x01 \x01(\x07\x12\x33\n\x0e\x64\x65vice_metrics\x18\x02 \x01(\x0b\x32\x19.meshtastic.DeviceMetricsH\x00\x12=\n\x13\x65nvironment_metrics\x18\x03 \x01(\x0b\x32\x1e.meshtastic.EnvironmentMetricsH\x00\x12<\n\x13\x61ir_quality_metrics\x18\x04 \x01(\x0b\x32\x1d.meshtastic.AirQualityMetricsH\x00\x12\x31\n\rpower_metrics\x18\x05 \x01(\x0b\x32\x18.meshtastic.PowerMetricsH\x00\x42\t\n\x07variant*\xe0\x01\n\x13TelemetrySensorType\x12\x10\n\x0cSENSOR_UNSET\x10\x00\x12\n\n\x06\x42ME280\x10\x01\x12\n\n\x06\x42ME680\x10\x02\x12\x0b\n\x07MCP9808\x10\x03\x12\n\n\x06INA260\x10\x04\x12\n\n\x06INA219\x10\x05\x12\n\n\x06\x42MP280\x10\x06\x12\t\n\x05SHTC3\x10\x07\x12\t\n\x05LPS22\x10\x08\x12\x0b\n\x07QMC6310\x10\t\x12\x0b\n\x07QMI8658\x10\n\x12\x0c\n\x08QMC5883L\x10\x0b\x12\t\n\x05SHT31\x10\x0c\x12\x0c\n\x08PMSA003I\x10\r\x12\x0b\n\x07INA3221\x10\x0e\x12\n\n\x06\x42MP085\x10\x0f\x42\x64\n\x13\x63om.geeksville.meshB\x0fTelemetryProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.telemetry_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\017TelemetryProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _TELEMETRYSENSORTYPE._serialized_start=985
-  _TELEMETRYSENSORTYPE._serialized_end=1209
-  _DEVICEMETRICS._serialized_start=30
-  _DEVICEMETRICS._serialized_end=135
-  _ENVIRONMENTMETRICS._serialized_start=138
-  _ENVIRONMENTMETRICS._serialized_end=293
-  _POWERMETRICS._serialized_start=296
-  _POWERMETRICS._serialized_end=436
-  _AIRQUALITYMETRICS._serialized_start=439
-  _AIRQUALITYMETRICS._serialized_end=758
-  _TELEMETRY._serialized_start=761
-  _TELEMETRY._serialized_end=982
+  _TELEMETRYSENSORTYPE._serialized_start=1041
+  _TELEMETRYSENSORTYPE._serialized_end=1265
+  _DEVICEMETRICS._serialized_start=42
+  _DEVICEMETRICS._serialized_end=147
+  _ENVIRONMENTMETRICS._serialized_start=150
+  _ENVIRONMENTMETRICS._serialized_end=305
+  _POWERMETRICS._serialized_start=308
+  _POWERMETRICS._serialized_end=448
+  _AIRQUALITYMETRICS._serialized_start=451
+  _AIRQUALITYMETRICS._serialized_end=770
+  _TELEMETRY._serialized_start=773
+  _TELEMETRY._serialized_end=1038
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic/test.py` & `meshtastic-2.3.4/meshtastic/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
    messages and report back if successful.
 """
 import logging
 import sys
 import time
 import traceback
 
-from dotmap import DotMap
-from pubsub import pub
+from dotmap import DotMap # type: ignore[import-untyped]
+from pubsub import pub # type: ignore[import-untyped]
 
 import meshtastic.util
-from meshtastic.__init__ import BROADCAST_NUM
+from meshtastic import BROADCAST_NUM
 from meshtastic.serial_interface import SerialInterface
 from meshtastic.tcp_interface import TCPInterface
 
 """The interfaces we are using for our tests"""
 interfaces = None
 
 """A list of all packets we received while the current test was running"""
```

### Comparing `meshtastic-2.3.3/meshtastic/tunnel.py` & `meshtastic-2.3.4/meshtastic/tunnel.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # FIXME: use a more optimal MTU
 """
 
 import logging
 import platform
 import threading
 
-from pubsub import pub
+from pubsub import pub # type: ignore[import-untyped]
 from pytap2 import TapDevice
 
 from meshtastic import portnums_pb2
 from meshtastic.globals import Globals
 from meshtastic.util import ipstr, readnet_u16
```

### Comparing `meshtastic-2.3.3/meshtastic/util.py` & `meshtastic-2.3.4/meshtastic/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 import re
 import subprocess
 import sys
 import threading
 import time
 import traceback
 from queue import Queue
+from google.protobuf.json_format import MessageToJson
 
 import packaging.version as pkg_version
 import requests
 import serial # type: ignore[import-untyped]
 import serial.tools.list_ports # type: ignore[import-untyped]
 
 from meshtastic.supported_device import supported_devices
 from meshtastic.version import get_active_version
 
 """Some devices such as a seger jlink we never want to accidentally open"""
 blacklistVids = dict.fromkeys([0x1366])
 
-
 def quoteBooleans(a_string):
     """Quote booleans
     given a string that contains ": true", replace with ": 'true'" (or false)
     """
     tmp = a_string.replace(": true", ": 'true'")
     tmp = tmp.replace(": false", ": 'false'")
     return tmp
@@ -608,7 +608,11 @@
     except pkg_version.InvalidVersion:
         return pypi_version
 
     if parsed_pypi_version <= parsed_act_version:
         return None
 
     return pypi_version
+
+def message_to_json(message):
+    "Return protobuf message as JSON. Always print all fields, even when not present in data."
+    return stripnl(MessageToJson(message, always_print_fields_with_no_presence=True))
```

### Comparing `meshtastic-2.3.3/meshtastic/xmodem_pb2.py` & `meshtastic-2.3.4/meshtastic/xmodem_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17meshtastic/xmodem.proto\"\xab\x01\n\x06XModem\x12 \n\x07\x63ontrol\x18\x01 \x01(\x0e\x32\x0f.XModem.Control\x12\x0b\n\x03seq\x18\x02 \x01(\r\x12\r\n\x05\x63rc16\x18\x03 \x01(\r\x12\x0e\n\x06\x62uffer\x18\x04 \x01(\x0c\"S\n\x07\x43ontrol\x12\x07\n\x03NUL\x10\x00\x12\x07\n\x03SOH\x10\x01\x12\x07\n\x03STX\x10\x02\x12\x07\n\x03\x45OT\x10\x04\x12\x07\n\x03\x41\x43K\x10\x06\x12\x07\n\x03NAK\x10\x15\x12\x07\n\x03\x43\x41N\x10\x18\x12\t\n\x05\x43TRLZ\x10\x1a\x42\x61\n\x13\x63om.geeksville.meshB\x0cXmodemProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17meshtastic/xmodem.proto\x12\nmeshtastic\"\xb6\x01\n\x06XModem\x12+\n\x07\x63ontrol\x18\x01 \x01(\x0e\x32\x1a.meshtastic.XModem.Control\x12\x0b\n\x03seq\x18\x02 \x01(\r\x12\r\n\x05\x63rc16\x18\x03 \x01(\r\x12\x0e\n\x06\x62uffer\x18\x04 \x01(\x0c\"S\n\x07\x43ontrol\x12\x07\n\x03NUL\x10\x00\x12\x07\n\x03SOH\x10\x01\x12\x07\n\x03STX\x10\x02\x12\x07\n\x03\x45OT\x10\x04\x12\x07\n\x03\x41\x43K\x10\x06\x12\x07\n\x03NAK\x10\x15\x12\x07\n\x03\x43\x41N\x10\x18\x12\t\n\x05\x43TRLZ\x10\x1a\x42\x61\n\x13\x63om.geeksville.meshB\x0cXmodemProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.xmodem_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\014XmodemProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _XMODEM._serialized_start=28
-  _XMODEM._serialized_end=199
-  _XMODEM_CONTROL._serialized_start=116
-  _XMODEM_CONTROL._serialized_end=199
+  _XMODEM._serialized_start=40
+  _XMODEM._serialized_end=222
+  _XMODEM_CONTROL._serialized_start=139
+  _XMODEM_CONTROL._serialized_end=222
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.3/meshtastic.egg-info/PKG-INFO` & `meshtastic-2.3.4/meshtastic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.3
+Version: 2.3.4
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
@@ -29,30 +29,30 @@
 Requires-Dist: bleak>=0.21.1
 Requires-Dist: packaging
 Provides-Extra: tunnel
 Requires-Dist: pytap2>=2.0.0; extra == "tunnel"
 
 # Meshtastic Python
 
-[![codecov](https://codecov.io/gh/meshtastic/Meshtastic-python/branch/master/graph/badge.svg?token=TIWPJL73KV)](https://codecov.io/gh/meshtastic/Meshtastic-python)
+[![codecov](https://codecov.io/gh/meshtastic/python/branch/master/graph/badge.svg?token=TIWPJL73KV)](https://codecov.io/gh/meshtastic/python)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/meshtastic)
 [![CI](https://img.shields.io/github/actions/workflow/status/meshtastic/python/ci.yml?branch=master&label=actions&logo=github&color=yellow)](https://github.com/meshtastic/python/actions/workflows/ci.yml)
 [![CLA assistant](https://cla-assistant.io/readme/badge/meshtastic/python)](https://cla-assistant.io/meshtastic/python)
 [![Fiscal Contributors](https://opencollective.com/meshtastic/tiers/badge.svg?label=Fiscal%20Contributors&color=deeppink)](https://opencollective.com/meshtastic/)
 
 ## Overview
 
 A Python client for use with Meshtastic devices.
 This small library (and example application) provides an easy API for sending and receiving messages over mesh radios.
 It also provides access to any of the operations/data available in the device user interface or the Android application.
 Events are delivered using a publish-subscribe model, and you can subscribe to only the message types you are interested in.
 
 **[Getting Started Guide](https://meshtastic.org/docs/software/python/cli/installation)**
 
-**[Documentation/API Reference](https://python.meshtastic.org/)**
+(Documentation/API Reference is currently offline)
 
 ## Call for Contributors
 
 This library and CLI has gone without a consistent maintainer for a while, and there's many improvements that could be made. We're all volunteers here and help is extremely appreciated, whether in implementing your own needs or helping maintain the library and CLI in general.
 
 If you're interested in contributing but don't have specific things you'd like to work on, look at the roadmap below!
```

### Comparing `meshtastic-2.3.3/meshtastic.egg-info/SOURCES.txt` & `meshtastic-2.3.4/meshtastic.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,67 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
 meshtastic/__init__.py
 meshtastic/__main__.py
 meshtastic/admin_pb2.py
+meshtastic/admin_pb2.pyi
 meshtastic/apponly_pb2.py
+meshtastic/apponly_pb2.pyi
 meshtastic/atak_pb2.py
+meshtastic/atak_pb2.pyi
 meshtastic/ble_interface.py
 meshtastic/cannedmessages_pb2.py
+meshtastic/cannedmessages_pb2.pyi
 meshtastic/channel_pb2.py
+meshtastic/channel_pb2.pyi
 meshtastic/clientonly_pb2.py
+meshtastic/clientonly_pb2.pyi
 meshtastic/config_pb2.py
+meshtastic/config_pb2.pyi
 meshtastic/connection_status_pb2.py
+meshtastic/connection_status_pb2.pyi
 meshtastic/deviceonly_pb2.py
+meshtastic/deviceonly_pb2.pyi
 meshtastic/globals.py
 meshtastic/localonly_pb2.py
+meshtastic/localonly_pb2.pyi
 meshtastic/mesh_interface.py
 meshtastic/mesh_pb2.py
+meshtastic/mesh_pb2.pyi
 meshtastic/module_config_pb2.py
+meshtastic/module_config_pb2.pyi
 meshtastic/mqtt_pb2.py
+meshtastic/mqtt_pb2.pyi
 meshtastic/nanopb_pb2.py
+meshtastic/nanopb_pb2.pyi
 meshtastic/node.py
 meshtastic/paxcount_pb2.py
+meshtastic/paxcount_pb2.pyi
 meshtastic/portnums_pb2.py
+meshtastic/portnums_pb2.pyi
 meshtastic/remote_hardware.py
 meshtastic/remote_hardware_pb2.py
+meshtastic/remote_hardware_pb2.pyi
 meshtastic/rtttl_pb2.py
+meshtastic/rtttl_pb2.pyi
 meshtastic/serial_interface.py
 meshtastic/storeforward_pb2.py
+meshtastic/storeforward_pb2.pyi
 meshtastic/stream_interface.py
 meshtastic/supported_device.py
 meshtastic/tcp_interface.py
 meshtastic/telemetry_pb2.py
+meshtastic/telemetry_pb2.pyi
 meshtastic/test.py
 meshtastic/tunnel.py
 meshtastic/util.py
 meshtastic/version.py
 meshtastic/xmodem_pb2.py
+meshtastic/xmodem_pb2.pyi
 meshtastic.egg-info/PKG-INFO
 meshtastic.egg-info/SOURCES.txt
 meshtastic.egg-info/dependency_links.txt
 meshtastic.egg-info/entry_points.txt
 meshtastic.egg-info/requires.txt
 meshtastic.egg-info/top_level.txt
```

### Comparing `meshtastic-2.3.3/setup.py` & `meshtastic-2.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # This call to setup() does all the work
 setup(
     name="meshtastic",
-    version="2.3.3",
+    version="2.3.4",
     description="Python API & client shell for talking to Meshtastic devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meshtastic/python",
     author="Meshtastic Developers",
     author_email="contact@meshtastic.org",
     license="GPL-3.0-only",
```

