# Comparing `tmp/hahomematic-2024.4.1.tar.gz` & `tmp/hahomematic-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.4.1.tar", last modified: Fri Apr  5 15:41:05 2024, max compression
+gzip compressed data, was "hahomematic-2024.4.2.tar", last modified: Mon Apr  8 11:38:21 2024, max compression
```

## Comparing `hahomematic-2024.4.1.tar` & `hahomematic-2024.4.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.056359 hahomematic-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-05 15:41:05.056359 hahomematic-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.044359 hahomematic-2024.4.1/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.048359 hahomematic-2024.4.1/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27481 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.048359 hahomematic-2024.4.1/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    56972 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.048359 hahomematic-2024.4.1/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14611 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.048359 hahomematic-2024.4.1/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.052359 hahomematic-2024.4.1/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44568 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33118 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    30209 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.052359 hahomematic-2024.4.1/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.052359 hahomematic-2024.4.1/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.052359 hahomematic-2024.4.1/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.056359 hahomematic-2024.4.1/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-05 15:41:05.000000 hahomematic-2024.4.1/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-05 15:41:05.000000 hahomematic-2024.4.1/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:41:05.000000 hahomematic-2024.4.1/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:41:04.000000 hahomematic-2024.4.1/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 15:41:05.000000 hahomematic-2024.4.1/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 15:41:05.000000 hahomematic-2024.4.1/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.056359 hahomematic-2024.4.1/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18422 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 15:41:05.060360 hahomematic-2024.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.056359 hahomematic-2024.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    26290 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26187 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    31933 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.978613 hahomematic-2024.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-08 11:38:21.978613 hahomematic-2024.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.966612 hahomematic-2024.4.2/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.966612 hahomematic-2024.4.2/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27513 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.966612 hahomematic-2024.4.2/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    57005 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.966612 hahomematic-2024.4.2/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14611 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.970613 hahomematic-2024.4.2/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.970613 hahomematic-2024.4.2/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33141 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30209 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.974613 hahomematic-2024.4.2/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.974613 hahomematic-2024.4.2/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.974613 hahomematic-2024.4.2/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.978613 hahomematic-2024.4.2/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.974613 hahomematic-2024.4.2/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 11:38:21.978613 hahomematic-2024.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.978613 hahomematic-2024.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26290 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26187 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31933 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_text.py
```

### Comparing `hahomematic-2024.4.1/LICENSE` & `hahomematic-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/PKG-INFO` & `hahomematic-2024.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.1/README.md` & `hahomematic-2024.4.2/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/__init__.py` & `hahomematic-2024.4.2/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/caches/dynamic.py` & `hahomematic-2024.4.2/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/caches/persistent.py` & `hahomematic-2024.4.2/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/caches/visibility.py` & `hahomematic-2024.4.2/hahomematic/caches/visibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,24 +309,24 @@
                         channel_no
                     ] = {ParamsetKey.MASTER: set()}
                 for parameter in parameters:
                     self._un_ignore_parameters_by_device_paramset_key[device_type_l][channel_no][
                         ParamsetKey.MASTER
                     ].add(parameter)
 
-    @lru_cache(maxsize=256)
+    @lru_cache(maxsize=128)
     def device_type_is_ignored(self, device_type: str) -> bool:
         """Check if a device type should be ignored for custom entities."""
         return element_matches_key(
             search_elements=self._ignore_custom_device_type,
             compare_with=device_type.lower(),
             do_wildcard_search=True,
         )
 
-    @lru_cache(maxsize=4096)
+    @lru_cache(maxsize=1024)
     def parameter_is_ignored(
         self,
         device_type: str,
         channel_no: int | None,
         paramset_key: str,
         parameter: str,
     ) -> bool:
@@ -429,22 +429,25 @@
                 and (channel_values := custom_un_ignore.get(dtl))
                 and (paramset_key_values := channel_values.get(cno))
                 and parameter in paramset_key_values.get(paramset_key, set())
             ):
                 return True  # pragma: no cover
 
         # check if parameter is in _UN_IGNORE_PARAMETERS_BY_DEVICE
-        if not custom_only:
-            if (
+        if (
+            not custom_only
+            and (
                 un_ignore_parameters := _get_value_from_dict_by_wildcard_key(
                     search_elements=self._un_ignore_parameters_by_device_lower,
                     compare_with=device_type_l,
                 )
-            ) and parameter in un_ignore_parameters:
-                return True
+            )
+            and parameter in un_ignore_parameters
+        ):
+            return True
 
         return False
 
     @lru_cache(maxsize=4096)
     def parameter_is_un_ignored(
         self,
         device_type: str,
```

### Comparing `hahomematic-2024.4.1/hahomematic/central/__init__.py` & `hahomematic-2024.4.2/hahomematic/central/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This is the python representation of a CCU.
 """
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Callable, Coroutine, Mapping, Set
+from collections.abc import Callable, Coroutine, Mapping, Set as AbstractSet
 from concurrent.futures._base import CancelledError
 from datetime import datetime
 import logging
 import socket
 import threading
 from typing import Any, Final, TypeVar, cast
 
@@ -827,21 +827,22 @@
             return
 
         self.last_events[interface_id] = datetime.now()
         # No need to check the response of a XmlRPC-PING
         if parameter == Parameter.PONG:
             if "#" in value:
                 v_interface_id, v_timestamp = value.split("#")
-                if v_interface_id == interface_id:
-                    if (
-                        client := self.get_client(interface_id=interface_id)
-                    ) and client.supports_ping_pong:
-                        client.ping_pong_cache.handle_received_pong(
-                            pong_ts=datetime.strptime(v_timestamp, DATETIME_FORMAT_MILLIS)
-                        )
+                if (
+                    v_interface_id == interface_id
+                    and (client := self.get_client(interface_id=interface_id))
+                    and client.supports_ping_pong
+                ):
+                    client.ping_pong_cache.handle_received_pong(
+                        pong_ts=datetime.strptime(v_timestamp, DATETIME_FORMAT_MILLIS)
+                    )
             return
         if (channel_address, parameter) in self._entity_event_subscriptions:
             try:
                 for callback in self._entity_event_subscriptions[(channel_address, parameter)]:
                     callback(value)
             except RuntimeError as rte:  # pragma: no cover
                 _LOGGER.debug(
@@ -1228,15 +1229,15 @@
         self,
         storage_folder: str,
         name: str,
         host: str,
         username: str,
         password: str,
         central_id: str,
-        interface_configs: Set[hmcl.InterfaceConfig],
+        interface_configs: AbstractSet[hmcl.InterfaceConfig],
         default_callback_port: int,
         client_session: ClientSession | None,
         tls: bool = DEFAULT_TLS,
         verify_tls: bool = DEFAULT_VERIFY_TLS,
         callback_host: str | None = None,
         callback_port: int | None = None,
         json_port: int | None = None,
@@ -1393,15 +1394,15 @@
                 reduce_args(args=exception.args),
                 extra_msg,
             )
 
 
 def _get_new_entities(
     new_devices: set[HmDevice],
-) -> Mapping[HmPlatform, Set[CallbackEntity]]:
+) -> Mapping[HmPlatform, AbstractSet[CallbackEntity]]:
     """Return new entities by platform."""
     entities_by_platform: dict[HmPlatform, set[CallbackEntity]] = {}
     for platform in HmPlatform:
         if platform == HmPlatform.EVENT:
             continue
         entities_by_platform[platform] = set()
```

### Comparing `hahomematic-2024.4.1/hahomematic/central/decorators.py` & `hahomematic-2024.4.2/hahomematic/central/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 from hahomematic import client as hmcl
 from hahomematic.const import SystemEvent
 from hahomematic.exceptions import HaHomematicException
 from hahomematic.support import reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
-_CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 
 _INTERFACE_ID: Final = "interface_id"
 
 
 def callback_system_event(system_event: SystemEvent) -> Callable:
```

### Comparing `hahomematic-2024.4.1/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.4.2/hahomematic/central/xml_rpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
             allow_none=True,
         )
         self._simple_xml_rpc_server.register_introspection_functions()
         self._simple_xml_rpc_server.register_multicall_functions()
         self._simple_xml_rpc_server.register_instance(RPCFunctions(self), allow_dotted_names=True)
         self._centrals: Final[dict[str, hmcu.CentralUnit]] = {}
 
-    def __new__(cls, local_port: int) -> XmlRpcServer:
+    def __new__(cls, local_port: int) -> XmlRpcServer:  # noqa: PYI034
         """Create new XmlRPC server."""
         if (xml_rpc := cls._instances.get(local_port)) is None:
             _LOGGER.debug("Creating XmlRpc server")
             return super().__new__(cls)
         return xml_rpc
 
     def run(self) -> None:
```

### Comparing `hahomematic-2024.4.1/hahomematic/client/__init__.py` & `hahomematic-2024.4.2/hahomematic/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/client/json_rpc.py` & `hahomematic-2024.4.2/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/client/xml_rpc.py` & `hahomematic-2024.4.2/hahomematic/client/xml_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/config.py` & `hahomematic-2024.4.2/hahomematic/config.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/const.py` & `hahomematic-2024.4.2/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/exceptions.py` & `hahomematic-2024.4.2/hahomematic/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from collections.abc import Awaitable, Callable
 from functools import wraps
 import logging
 from typing import Any, Final, ParamSpec, TypeVar, cast
 
 _LOGGER: Final = logging.getLogger(__name__)
 
-_CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 
 
 class BaseHomematicException(Exception):
     """hahomematic base exception."""
```

### Comparing `hahomematic-2024.4.1/hahomematic/hmcli.py` & `hahomematic-2024.4.2/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/performance.py` & `hahomematic-2024.4.2/hahomematic/performance.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/__init__.py` & `hahomematic-2024.4.2/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.4.2/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.4.2/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/custom/const.py` & `hahomematic-2024.4.2/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.4.2/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.4.2/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.4.2/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/custom/light.py` & `hahomematic-2024.4.2/hahomematic/platforms/custom/light.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,19 +386,22 @@
         """Turn the light on."""
         if not self.is_state_change(on=True, **kwargs):
             return
 
         if "effect" not in kwargs and self.supports_effects and self.effect != _EFFECT_OFF:
             await self._e_effect.send_value(value=0, collector=collector, collector_order=5)
 
-        if self.supports_effects and (effect := kwargs.get("effect")) is not None:
-            if (effect_idx := self._effects.index(effect)) is not None:
-                await self._e_effect.send_value(
-                    value=effect_idx, collector=collector, collector_order=95
-                )
+        if (
+            self.supports_effects
+            and (effect := kwargs.get("effect")) is not None
+            and (effect_idx := self._effects.index(effect)) is not None
+        ):
+            await self._e_effect.send_value(
+                value=effect_idx, collector=collector, collector_order=95
+            )
 
         await super().turn_on(collector=collector, **kwargs)
 
 
 class CeColorTempDimmer(CeDimmer):
     """Class for HomeMatic dimmer with color temperature entities."""
```

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.4.2/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.4.2/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/custom/support.py` & `hahomematic-2024.4.2/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.4.2/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/decorators.py` & `hahomematic-2024.4.2/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/device.py` & `hahomematic-2024.4.2/hahomematic/platforms/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module for the Device class."""
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Callable, Mapping, Set
+from collections.abc import Callable, Mapping, Set as AbstractSet
 from copy import copy
 from datetime import datetime
 import logging
 import os
 import random
 from typing import Any, Final
 
@@ -432,15 +432,15 @@
                 or exclude_no_create is False
             )
             and (registered is None or entity.is_registered == registered)
         )
 
     def get_entities_by_platform(
         self, exclude_no_create: bool = True, registered: bool | None = None
-    ) -> Mapping[HmPlatform, Set[CallbackEntity]]:
+    ) -> Mapping[HmPlatform, AbstractSet[CallbackEntity]]:
         """Return all externally registered entities."""
         entities_by_platform: dict[HmPlatform, set[CallbackEntity]] = {}
         for platform in PLATFORMS:
             if platform == HmPlatform.EVENT:
                 continue
             entities_by_platform[platform] = set()
```

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/entity.py` & `hahomematic-2024.4.2/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/event.py` & `hahomematic-2024.4.2/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.4.2/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/generic/action.py` & `hahomematic-2024.4.2/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.4.2/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/generic/button.py` & `hahomematic-2024.4.2/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.4.2/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/generic/number.py` & `hahomematic-2024.4.2/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/generic/select.py` & `hahomematic-2024.4.2/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.4.2/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.4.2/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.4.2/hahomematic/platforms/hub/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module for HaHomematic hub platforms."""
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Collection, Mapping, Set
+from collections.abc import Collection, Mapping, Set as AbstractSet
 import logging
 from typing import Final
 
 from hahomematic import central as hmcu
 from hahomematic.const import (
     HUB_PLATFORMS,
     Backend,
@@ -204,15 +204,15 @@
 def _clean_variables(variables: tuple[SystemVariableData, ...]) -> tuple[SystemVariableData, ...]:
     """Clean variables by removing excluded."""
     return tuple(sv for sv in variables if not _is_excluded(sv.name, _EXCLUDED))
 
 
 def _get_new_hub_entities(
     entities: Collection[GenericHubEntity],
-) -> Mapping[HmPlatform, Set[GenericHubEntity]]:
+) -> Mapping[HmPlatform, AbstractSet[GenericHubEntity]]:
     """Return entities as platform dict."""
     hm_hub_entities: dict[HmPlatform, set[GenericHubEntity]] = {}
     for hm_hub_platform in HUB_PLATFORMS:
         hm_hub_entities[hm_hub_platform] = set()
 
     for hub_entity in entities:
         if hub_entity.is_registered is False:
```

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.4.2/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/hub/button.py` & `hahomematic-2024.4.2/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.4.2/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/hub/number.py` & `hahomematic-2024.4.2/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/hub/select.py` & `hahomematic-2024.4.2/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.4.2/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/hub/text.py` & `hahomematic-2024.4.2/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/support.py` & `hahomematic-2024.4.2/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/platforms/update.py` & `hahomematic-2024.4.2/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.4.2/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.4.2/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.4.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic/support.py` & `hahomematic-2024.4.2/hahomematic/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Helper functions used within hahomematic."""
 
 from __future__ import annotations
 
 import base64
-from collections.abc import Callable, Collection
+from collections.abc import Collection
 import contextlib
 from dataclasses import dataclass
 from datetime import datetime
-from functools import cache
+from functools import lru_cache
 import logging
 import os
 import re
 import socket
 import ssl
-from typing import Any, Final, TypeVar
+from typing import Any, Final
 
 from hahomematic.const import (
     CCU_PASSWORD_PATTERN,
     FILE_DEVICES,
     FILE_PARAMSETS,
     IDENTIFIER_SEPARATOR,
     INIT_DATETIME,
@@ -25,16 +25,14 @@
     NO_CACHE_ENTRY,
     SysvarType,
 )
 from hahomematic.exceptions import BaseHomematicException, HaHomematicException
 
 _LOGGER: Final = logging.getLogger(__name__)
 
-_CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
-
 
 def reduce_args(args: tuple[Any, ...]) -> tuple[Any, ...] | Any:
     """Return the first arg, if there is only one arg."""
     return args[0] if len(args) == 1 else args
 
 
 def build_xml_rpc_uri(
@@ -167,15 +165,15 @@
 
 
 def get_channel_no(address: str) -> int | None:
     """Return the channel part of an address."""
     return get_split_channel_address(channel_address=address)[1]
 
 
-@cache
+@lru_cache(maxsize=2048)
 def get_split_channel_address(channel_address: str) -> tuple[str, int | None]:
     """Return the device part of an address."""
     if ":" in channel_address:
         device_address, channel_no = channel_address.split(":")
         if channel_no in (None, "None"):
             return device_address, None
         return device_address, int(channel_no)
@@ -218,25 +216,22 @@
     if isinstance(search_elements, str):
         if do_wildcard_search:
             return compare_with.lower().startswith(
                 search_elements.lower()
             )  # or search_elements.lower().startswith(compare_with.lower())
         return compare_with.lower() == search_elements.lower()
     if isinstance(search_elements, Collection):
-        if isinstance(search_elements, dict):
-            if (
-                match_key := _get_search_key(
-                    search_elements=search_elements, search_key=search_key
-                )
-                if search_key
-                else None
-            ):
-                if (elements := search_elements.get(match_key)) is None:
-                    return False
-                search_elements = elements
+        if isinstance(search_elements, dict) and (
+            match_key := _get_search_key(search_elements=search_elements, search_key=search_key)
+            if search_key
+            else None
+        ):
+            if (elements := search_elements.get(match_key)) is None:
+                return False
+            search_elements = elements
         for element in search_elements:
             if do_wildcard_search:
                 if compare_with.lower().startswith(element.lower()):
                     return True
             elif compare_with.lower() == element.lower():
                 return True
     return False
```

### Comparing `hahomematic-2024.4.1/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.4.2/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.1/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.4.2/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/hahomematic_support/client_local.py` & `hahomematic-2024.4.2/hahomematic_support/client_local.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/pyproject.toml` & `hahomematic-2024.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.4.1"
+version     = "2024.4.2"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
@@ -414,36 +414,40 @@
     "B014", # Exception handler with duplicate exception
     "B015", # Pointless comparison. Did you mean to assign a value? Otherwise, prepend assert or remove it.
     "B018", # Found useless attribute access. Either assign it to a variable or remove it.
     "B023", # Function definition does not bind loop variable {name}
     "B026", # Star-arg unpacking after a keyword argument is strongly discouraged
     "B032", # Possible unintentional type annotation (using :). Did you mean to assign (using =)?
     "B904", # Use raise from to specify exception cause
+    "B905", # zip() without an explicit strict= parameter
     "C",  # complexity
     "COM818", # Trailing comma on bare tuple prohibited
     "D",  # docstrings
     "DTZ003",  # Use datetime.now(tz=) instead of datetime.utcnow()
     "DTZ004",  # Use datetime.fromtimestamp(ts, tz=) instead of datetime.utcfromtimestamp(ts)
     "E",  # pycodestyle
     "F",  # pyflakes/autoflake
+    "FLY", # flynt
     "G", # flake8-logging-format
     "I",  # isort
+    "INP", # flake8-no-pep420
     "ICN001", # import concentions; {name} should be imported as {asname}
     "LOG", # flake8-logging
     "N804", # First argument of a class method should be named cls
     "N805", # First argument of a method should be named self
     "N815", # Variable {name} in class scope should not be mixedCase
     "PERF", # perflint
-    "PGH004",  # Use specific rule codes when using noqa
+    "PGH", # pygrep-hooks
     "PLC", # pylint
     "PLC0414", # Useless import alias. Import alias does not rename original package.
     "PLE", # pylint
     "PLR", # pylint
     "PLW", # pylint
     "PT", # flake8-pytest-style
+    "PYI", # flake8-pyi
     "Q000", # Double quotes found but single quotes preferred
     "RSE", # flake8-raise
     "RUF006", # Store a reference to the return value of asyncio.create_task
     "S102", # Use of exec detected
     "S103",  # bad-file-permissions
     "S108",  # hardcoded-temp-file
     "S306",  # suspicious-mktemp-usage
@@ -457,22 +461,16 @@
     "S319",  # suspicious-xml-pull-dom-usage
     "S320",  # suspicious-xmle-tree-usage
     "S601",  # paramiko-call
     "S602",  # subprocess-popen-with-shell-equals-true
     "S604",  # call-with-shell-equals-true
     "S608",  # hardcoded-sql-expression
     "S609",  # unix-command-wildcard-injection
-    "SIM105", # Use contextlib.suppress({exception}) instead of try-except-pass
-    "SIM117", # Merge with-statements that use the same scope
-    "SIM118", # Use {key} in {dict} instead of {key} in {dict}.keys()
-    "SIM201", # Use {left} != {right} instead of not {left} == {right}
-    "SIM208", # Use {expr} instead of not (not {expr})
-    "SIM212", # Use {a} if {a} else {b} instead of {b} if not {a} else {a}
-    "SIM300", # Yoda conditions. Use 'age == 42' instead of '42 == age'.
-    "SIM401", # Use get from dict with default instead of an if block
+    "SIM", # flake8-simplify
+    "SLOT", # flake8-slots
     "T100", # Trace found: {name} used
     "T20",  # flake8-print
     "TID251", # Banned imports
     "TRY004", # Prefer TypeError exception for invalid type
     "TRY302", # Remove exception handler; error is immediately re-raised
     "UP",  # pyupgrade
     "W",  # pycodestyle
@@ -492,14 +490,17 @@
     # False positives https://github.com/astral-sh/ruff/issues/5386
     "PLC0208", # Use a sequence type instead of a `set` when iterating over values
     "PLR0911", # Too many return statements ({returns} > {max_returns})
     "PLR0912", # Too many branches ({branches} > {max_branches})
     "PLR0913", # Too many arguments to function call ({c_args} > {max_args})
     "PT004", # Fixture {fixture} does not return anything, add leading underscore
     "PT011", # pytest.raises({exception}) is too broad, set the `match` parameter or use a more specific exception
+    "PYI024", # Use typing.NamedTuple instead of collections.namedtuple
+    "PYI036",
+    "PYI041",
     "PLR0915", # Too many statements ({statements} > {max_statements})
     "PLR2004",  # Magic value used in comparison, consider replacing {value} with a constant variable
     "PLW2901", # Outer {outer_kind} variable {name} overwritten by inner {inner_kind} target
     "UP006", # keep type annotation style as is
     "UP007", # keep type annotation style as is
     # Ignored due to performance: https://github.com/charliermarsh/ruff/issues/2923
     "UP038", # Use `X | Y` in `isinstance` call instead of `(X, Y)`
```

### Comparing `hahomematic-2024.4.1/tests/test_action.py` & `hahomematic-2024.4.2/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_binary_sensor.py` & `hahomematic-2024.4.2/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_button.py` & `hahomematic-2024.4.2/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_central.py` & `hahomematic-2024.4.2/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_central_pydevccu.py` & `hahomematic-2024.4.2/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_climate.py` & `hahomematic-2024.4.2/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_cover.py` & `hahomematic-2024.4.2/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_decorator.py` & `hahomematic-2024.4.2/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_device.py` & `hahomematic-2024.4.2/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_entity.py` & `hahomematic-2024.4.2/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_event.py` & `hahomematic-2024.4.2/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_json_rpc.py` & `hahomematic-2024.4.2/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_light.py` & `hahomematic-2024.4.2/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_lock.py` & `hahomematic-2024.4.2/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_number.py` & `hahomematic-2024.4.2/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_select.py` & `hahomematic-2024.4.2/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_sensor.py` & `hahomematic-2024.4.2/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_siren.py` & `hahomematic-2024.4.2/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_support.py` & `hahomematic-2024.4.2/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_switch.py` & `hahomematic-2024.4.2/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.1/tests/test_text.py` & `hahomematic-2024.4.2/tests/test_text.py`

 * *Files identical despite different names*

