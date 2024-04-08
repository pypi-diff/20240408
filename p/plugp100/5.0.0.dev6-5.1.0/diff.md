# Comparing `tmp/plugp100-5.0.0.dev6.tar.gz` & `tmp/plugp100-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugp100-5.0.0.dev6.tar", last modified: Sat Apr  6 12:54:20 2024, max compression
+gzip compressed data, was "plugp100-5.1.0.tar", last modified: Mon Apr  8 05:56:11 2024, max compression
```

## Comparing `plugp100-5.0.0.dev6.tar` & `plugp100-5.1.0.tar`

### file list

```diff
@@ -1,162 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.698099 plugp100-5.0.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-06 12:54:20.698099 plugp100-5.0.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.682099 plugp100-5.0.0.dev6/plugp100/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-06 12:54:20.000000 plugp100-5.0.0.dev6/plugp100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.682099 plugp100-5.0.0.dev6/plugp100/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19612 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/light_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/light_effect_preset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.682099 plugp100-5.0.0.dev6/plugp100/api/requests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/handshake_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.682099 plugp100-5.0.0.dev6/plugp100/api/requests/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/internal/snowflake_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/login_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/secure_passthrough_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.682099 plugp100-5.0.0.dev6/plugp100/api/requests/set_device_info/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/set_device_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/set_device_info/play_alarm_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/set_device_info/set_light_color_info_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/set_device_info/set_light_info_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/set_device_info/set_plug_info_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/set_device_info/set_trv_info_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/tapo_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/requests/trigger_logs_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/api/tapo_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.686099 plugp100-5.0.0.dev6/plugp100/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/common/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.686099 plugp100-5.0.0.dev6/plugp100/common/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/common/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/common/functional/tri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.686099 plugp100-5.0.0.dev6/plugp100/common/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/common/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/common/utils/json_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.686099 plugp100-5.0.0.dev6/plugp100/discovery/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/discovery/cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/discovery/discovered_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/discovery/rsa_session.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3587 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/discovery/tapo_discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.686099 plugp100-5.0.0.dev6/plugp100/encryption/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/encryption/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/encryption/key_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/encryption/tp_link_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.686099 plugp100-5.0.0.dev6/plugp100/new/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.686099 plugp100-5.0.0.dev6/plugp100/new/child/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/child/tapohubchildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/child/tapostripsocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.690099 plugp100-5.0.0.dev6/plugp100/new/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/alarm_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/battery_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/device_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/energy_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/hub_children_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/humidity_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/light_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/light_effect_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/motion_sensor_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/on_off_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/overheat_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/report_mode_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/smart_door_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/socket_children_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/temperature_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/temperature_humidity_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/trigger_log_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/components/water_leak_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/device_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/device_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.690099 plugp100-5.0.0.dev6/plugp100/new/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/errors/invalid_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.690099 plugp100-5.0.0.dev6/plugp100/new/event_polling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/event_polling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/event_polling/event_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/event_polling/poll_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/event_polling/state_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/hub_device_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/tapobulb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/tapodevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/tapohub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/new/tapoplug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.694099 plugp100-5.0.0.dev6/plugp100/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/protocol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.694099 plugp100-5.0.0.dev6/plugp100/protocol/klap/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/protocol/klap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/protocol/klap/klap_handshake_revision.py
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/protocol/klap/klap_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/protocol/passthrough_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/protocol/securepassthrough_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/protocol/tapo_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.694099 plugp100-5.0.0.dev6/plugp100/responses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/alarm_type_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/child_device_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/device_usage_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/energy_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.694099 plugp100-5.0.0.dev6/plugp100/responses/hub_childs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/hub_childs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/hub_childs/hub_child_base_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/hub_childs/ke100_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/hub_childs/leak_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/hub_childs/s200b_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/hub_childs/switch_child_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/hub_childs/t100_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/hub_childs/t110_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/hub_childs/t31x_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/hub_childs/trigger_log_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/power_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/tapo_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/tapo_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/temperature_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/plugp100/responses/time_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.698099 plugp100-5.0.0.dev6/plugp100.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-06 12:54:20.000000 plugp100-5.0.0.dev6/plugp100.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-06 12:54:20.000000 plugp100-5.0.0.dev6/plugp100.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 12:54:20.000000 plugp100-5.0.0.dev6/plugp100.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-06 12:54:20.000000 plugp100-5.0.0.dev6/plugp100.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 12:54:20.000000 plugp100-5.0.0.dev6/plugp100.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-06 12:54:20.702099 plugp100-5.0.0.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.678099 plugp100-5.0.0.dev6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.698099 plugp100-5.0.0.dev6/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/integration/tapo_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/integration/test_button_t310.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/integration/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/integration/test_ledstrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/integration/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/integration/test_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/integration/test_power_strip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/integration/test_sensor_s200b.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3735 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/integration/test_tapo_discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.698099 plugp100-5.0.0.dev6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:54:20.698099 plugp100-5.0.0.dev6/tests/unit/hub_child/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/hub_child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/hub_child/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/hub_child/test_temp_hum_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/hub_child/test_trv_ke100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/test_bulb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/test_klap_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/test_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/test_plug_strip.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-06 12:53:47.000000 plugp100-5.0.0.dev6/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.083633 plugp100-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 05:55:44.000000 plugp100-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 05:55:44.000000 plugp100-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-08 05:56:11.083633 plugp100-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-08 05:55:44.000000 plugp100-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.063632 plugp100-5.1.0/plugp100/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 05:56:10.000000 plugp100-5.1.0/plugp100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.063632 plugp100-5.1.0/plugp100/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19612 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/light_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/light_effect_preset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.067632 plugp100-5.1.0/plugp100/api/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/handshake_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.067632 plugp100-5.1.0/plugp100/api/requests/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/internal/snowflake_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/login_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/secure_passthrough_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.067632 plugp100-5.1.0/plugp100/api/requests/set_device_info/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/set_device_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/set_device_info/play_alarm_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/set_device_info/set_light_color_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/set_device_info/set_light_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/set_device_info/set_plug_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/set_device_info/set_trv_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/tapo_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/requests/trigger_logs_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/api/tapo_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.067632 plugp100-5.1.0/plugp100/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/common/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.067632 plugp100-5.1.0/plugp100/common/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/common/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/common/functional/tri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.067632 plugp100-5.1.0/plugp100/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/common/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/common/utils/json_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.067632 plugp100-5.1.0/plugp100/discovery/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/discovery/cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/discovery/discovered_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/discovery/rsa_session.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3587 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/discovery/tapo_discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.071632 plugp100-5.1.0/plugp100/encryption/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/encryption/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/encryption/key_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/encryption/tp_link_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.071632 plugp100-5.1.0/plugp100/new/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.071632 plugp100-5.1.0/plugp100/new/child/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/child/tapohubchildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/child/tapostripsocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.075632 plugp100-5.1.0/plugp100/new/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/alarm_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/battery_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/countdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/device_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/energy_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/hub_children_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/humidity_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/light_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/light_effect_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/motion_sensor_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/on_off_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/overheat_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/report_mode_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/smart_door_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/socket_children_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/temperature_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/temperature_humidity_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/trigger_log_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/components/water_leak_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/device_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/device_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.075632 plugp100-5.1.0/plugp100/new/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/errors/invalid_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.075632 plugp100-5.1.0/plugp100/new/event_polling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/event_polling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/event_polling/event_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/event_polling/poll_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/event_polling/state_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/hub_device_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/tapobulb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/tapodevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/tapohub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/new/tapoplug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.075632 plugp100-5.1.0/plugp100/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/protocol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.075632 plugp100-5.1.0/plugp100/protocol/klap/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/protocol/klap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/protocol/klap/klap_handshake_revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/protocol/klap/klap_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/protocol/passthrough_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/protocol/securepassthrough_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/protocol/tapo_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.079632 plugp100-5.1.0/plugp100/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/alarm_type_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/child_device_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/device_usage_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/energy_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/firmware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.079632 plugp100-5.1.0/plugp100/responses/hub_childs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/hub_childs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/hub_childs/hub_child_base_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/hub_childs/ke100_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/hub_childs/leak_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/hub_childs/s200b_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/hub_childs/switch_child_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/hub_childs/t100_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/hub_childs/t110_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/hub_childs/t31x_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/hub_childs/trigger_log_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/power_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/tapo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/tapo_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/temperature_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-08 05:55:44.000000 plugp100-5.1.0/plugp100/responses/time_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.083633 plugp100-5.1.0/plugp100.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-08 05:56:11.000000 plugp100-5.1.0/plugp100.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-08 05:56:11.000000 plugp100-5.1.0/plugp100.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:56:11.000000 plugp100-5.1.0/plugp100.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-08 05:56:11.000000 plugp100-5.1.0/plugp100.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 05:56:11.000000 plugp100-5.1.0/plugp100.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-08 05:55:44.000000 plugp100-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 05:55:44.000000 plugp100-5.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 05:55:44.000000 plugp100-5.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-08 05:56:11.087633 plugp100-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-08 05:55:44.000000 plugp100-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.063632 plugp100-5.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.083633 plugp100-5.1.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/integration/tapo_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/integration/test_button_t310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/integration/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/integration/test_ledstrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/integration/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/integration/test_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/integration/test_power_strip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/integration/test_sensor_s200b.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3735 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/integration/test_tapo_discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.083633 plugp100-5.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:56:11.083633 plugp100-5.1.0/tests/unit/hub_child/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/hub_child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/hub_child/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/hub_child/test_temp_hum_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/hub_child/test_trv_ke100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/test_bulb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/test_klap_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/test_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/test_plug_strip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-08 05:55:44.000000 plugp100-5.1.0/tests/unit/test_utils.py
```

### Comparing `plugp100-5.0.0.dev6/LICENSE` & `plugp100-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/PKG-INFO` & `plugp100-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 5.0.0.dev6
+Version: 5.1.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-5.0.0.dev6/README.md` & `plugp100-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/__init__.py` & `plugp100-5.1.0/plugp100/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         sys.path.append(os.path.join(vendor_dir, vendor_path))
 
 from plugp100.responses import *
 from plugp100.api.requests import *
 from plugp100.api import *
 from plugp100.common import *
 
-__version__ = "5.0.0-dev.6"
+__version__ = "5.1.0"
```

### Comparing `plugp100-5.0.0.dev6/plugp100/api/light_effect.py` & `plugp100-5.1.0/plugp100/api/light_effect.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/api/light_effect_preset.py` & `plugp100-5.1.0/plugp100/api/light_effect_preset.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/api/requests/internal/snowflake_id.py` & `plugp100-5.1.0/plugp100/api/requests/internal/snowflake_id.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/api/requests/login_device.py` & `plugp100-5.1.0/plugp100/api/requests/login_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/api/requests/tapo_request.py` & `plugp100-5.1.0/plugp100/api/requests/tapo_request.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/api/tapo_client.py` & `plugp100-5.1.0/plugp100/api/tapo_client.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/common/functional/tri.py` & `plugp100-5.1.0/plugp100/common/functional/tri.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/common/utils/http_client.py` & `plugp100-5.1.0/plugp100/common/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/discovery/cloud_client.py` & `plugp100-5.1.0/plugp100/discovery/cloud_client.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/discovery/discovered_device.py` & `plugp100-5.1.0/plugp100/discovery/discovered_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/discovery/rsa_session.py` & `plugp100-5.1.0/plugp100/discovery/rsa_session.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/discovery/tapo_discovery.py` & `plugp100-5.1.0/plugp100/discovery/tapo_discovery.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/encryption/helpers.py` & `plugp100-5.1.0/plugp100/encryption/helpers.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/encryption/key_pair.py` & `plugp100-5.1.0/plugp100/encryption/key_pair.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/encryption/tp_link_cipher.py` & `plugp100-5.1.0/plugp100/encryption/tp_link_cipher.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/example.py` & `plugp100-5.1.0/plugp100/example.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/child/tapohubchildren.py` & `plugp100-5.1.0/plugp100/new/child/tapohubchildren.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/child/tapostripsocket.py` & `plugp100-5.1.0/plugp100/new/child/tapostripsocket.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/alarm_component.py` & `plugp100-5.1.0/plugp100/new/components/alarm_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/battery_component.py` & `plugp100-5.1.0/plugp100/new/components/battery_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/energy_component.py` & `plugp100-5.1.0/plugp100/new/components/energy_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/hub_children_component.py` & `plugp100-5.1.0/plugp100/new/components/hub_children_component.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from typing import Any, Optional
 
 from plugp100.api.tapo_client import TapoClient
 from plugp100.new.child.tapohubchildren import (
     SmartDoorSensor,
     TriggerButtonDevice,
     SwitchChildDevice,
@@ -10,14 +11,16 @@
     TemperatureHumiditySensor,
     KE100Device,
 )
 from plugp100.new.components.device_component import DeviceComponent
 from plugp100.new.tapodevice import TapoDevice
 from plugp100.responses.hub_childs.hub_child_base_info import HubChildBaseInfo
 
+_LOGGER = logging.getLogger("HubChildrenComponent")
+
 
 class HubChildrenComponent(DeviceComponent):
     def __init__(self, parent_device: TapoDevice, client: TapoClient):
         self._client = client
         self._children: [TapoDevice] = []
         self._parent_device = parent_device
 
@@ -29,36 +32,41 @@
         if len(self._children) == 0:
             children = (
                 await self._client.get_child_device_list(all_pages=True)
             ).get_or_raise()
             # _LOGGER.info("Initializing %s children", children.sum)
             for child in children.get_children_base_info():
                 child_device = _hub_child_create(self._parent_device, self._client, child)
-                self._children.append(child_device)
+                if child_device is not None:
+                    self._children.append(child_device)
+                else:
+                    _LOGGER.warning("Found child device not supported, model {}", child.model)
+                    _LOGGER.warning(
+                        "Please request support by opening an issue to https://github.com/petretiandrea/plugp100/issues/new")
 
             for child_device in self._children:
                 await child_device.update()
 
     def find_child_device_by_model(self, model_filter: str) -> Optional["TapoDevice"]:
         return next(
             (
                 child
                 for child in self.children
                 if child.device_id is not None
-                and model_filter.lower() in child.model.lower()
+                   and model_filter.lower() in child.model.lower()
             ),
             None,
         )
 
 
 # TODO: make based on device type
 def _hub_child_create(
-    parent_device: TapoDevice,
-    client: TapoClient,
-    child_info: HubChildBaseInfo,
+        parent_device: TapoDevice,
+        client: TapoClient,
+        child_info: HubChildBaseInfo,
 ) -> Optional[TapoDevice]:
     model = child_info.model.lower()
     if "t31" in model:
         return TemperatureHumiditySensor(
             host=parent_device.host,
             port=parent_device.port,
             client=client,
```

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/light_component.py` & `plugp100-5.1.0/plugp100/new/components/light_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/light_effect_component.py` & `plugp100-5.1.0/plugp100/new/components/light_effect_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/on_off_component.py` & `plugp100-5.1.0/plugp100/new/components/on_off_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/overheat_component.py` & `plugp100-5.1.0/plugp100/new/components/overheat_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/report_mode_component.py` & `plugp100-5.1.0/plugp100/new/components/report_mode_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/socket_children_component.py` & `plugp100-5.1.0/plugp100/new/components/socket_children_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/temperature_component.py` & `plugp100-5.1.0/plugp100/new/components/temperature_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/temperature_humidity_records.py` & `plugp100-5.1.0/plugp100/new/components/temperature_humidity_records.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/trigger_log_component.py` & `plugp100-5.1.0/plugp100/new/components/trigger_log_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/components/water_leak_component.py` & `plugp100-5.1.0/plugp100/new/components/water_leak_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/device_factory.py` & `plugp100-5.1.0/plugp100/new/device_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 async def connect(
     config: DeviceConnectConfiguration, session: Optional[aiohttp.ClientSession] = None
 ):
     if config.device_type is None:
         protocol = await _get_or_guess_protocol(config, session)
-        _LOGGER.info(
+        _LOGGER.debug(
             "Not enough information to detected device type and model, trying to fetching from device..."
         )
         device_info = DeviceInfo(
             **(await protocol.send_request(request=TapoRequest.get_device_info()))
             .get_or_raise()
             .result
         )
@@ -89,20 +89,20 @@
         KlapProtocol(config.credentials, config.url, klap_handshake_v1(), session),
         KlapProtocol(config.credentials, config.url, klap_handshake_v2(), session),
     ]
     device_info_request = TapoRequest.get_device_info()
     for protocol in protocols:
         info = await protocol.send_request(device_info_request)
         if info.is_success():
-            _LOGGER.info(f"Found working protocol {type(protocol)}")
+            _LOGGER.debug(f"Found working protocol {type(protocol)}")
             return protocol
         else:
-            _LOGGER.info(f"Protocol {type(protocol)} not working, trying next...")
+            _LOGGER.debug(f"Protocol {type(protocol)} not working, trying next...")
 
-    _LOGGER.info("None of available protocol is working, maybe invalid credentials")
+    _LOGGER.error("None of available protocol is working, maybe invalid credentials")
     raise InvalidAuthentication(config.host, config.device_type)
 
 
 def _get_device_class_from_model_type(device_type: str) -> Type[TapoDevice]:
     device_type = device_type.upper()
     if device_type == "SMART.TAPOPLUG":
         return TapoPlug
```

### Comparing `plugp100-5.0.0.dev6/plugp100/new/event_polling/event_subscription.py` & `plugp100-5.1.0/plugp100/new/event_polling/event_subscription.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/event_polling/poll_tracker.py` & `plugp100-5.1.0/plugp100/new/event_polling/poll_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/event_polling/state_tracker.py` & `plugp100-5.1.0/plugp100/new/event_polling/state_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/hub_device_tracker.py` & `plugp100-5.1.0/plugp100/new/hub_device_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/tapobulb.py` & `plugp100-5.1.0/plugp100/new/tapobulb.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/tapohub.py` & `plugp100-5.1.0/plugp100/new/tapohub.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/new/tapoplug.py` & `plugp100-5.1.0/plugp100/new/tapoplug.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,9 +36,8 @@
 
     def _get_components_to_activate(self, components: Components) -> list[C]:
         active_components = [OnOffComponent(self.client)]
         if components.has("energy_monitoring"):
             active_components.append(EnergyComponent(self.client))
         if components.has("control_child"):
             active_components.append(SocketChildrenComponent(self, self.client))
-
         return active_components
```

### Comparing `plugp100-5.0.0.dev6/plugp100/protocol/klap/klap_handshake_revision.py` & `plugp100-5.1.0/plugp100/protocol/klap/klap_handshake_revision.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/protocol/klap/klap_protocol.py` & `plugp100-5.1.0/plugp100/protocol/klap/klap_protocol.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/protocol/passthrough_protocol.py` & `plugp100-5.1.0/plugp100/protocol/passthrough_protocol.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/protocol/securepassthrough_transport.py` & `plugp100-5.1.0/plugp100/protocol/securepassthrough_transport.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/protocol/tapo_protocol.py` & `plugp100-5.1.0/plugp100/protocol/tapo_protocol.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/child_device_list.py` & `plugp100-5.1.0/plugp100/responses/child_device_list.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/components.py` & `plugp100-5.1.0/plugp100/responses/components.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/device_state.py` & `plugp100-5.1.0/plugp100/responses/device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/device_usage_info.py` & `plugp100-5.1.0/plugp100/responses/device_usage_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/energy_info.py` & `plugp100-5.1.0/plugp100/responses/energy_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/hub_childs/hub_child_base_info.py` & `plugp100-5.1.0/plugp100/responses/hub_childs/hub_child_base_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/hub_childs/ke100_device_state.py` & `plugp100-5.1.0/plugp100/responses/hub_childs/ke100_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/hub_childs/leak_device_state.py` & `plugp100-5.1.0/plugp100/responses/hub_childs/leak_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/hub_childs/s200b_device_state.py` & `plugp100-5.1.0/plugp100/responses/hub_childs/s200b_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/hub_childs/switch_child_device_state.py` & `plugp100-5.1.0/plugp100/responses/hub_childs/switch_child_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/hub_childs/t100_device_state.py` & `plugp100-5.1.0/plugp100/responses/hub_childs/t100_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/hub_childs/t110_device_state.py` & `plugp100-5.1.0/plugp100/responses/hub_childs/t110_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/hub_childs/t31x_device_state.py` & `plugp100-5.1.0/plugp100/responses/hub_childs/t31x_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/hub_childs/trigger_log_response.py` & `plugp100-5.1.0/plugp100/responses/hub_childs/trigger_log_response.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/tapo_exception.py` & `plugp100-5.1.0/plugp100/responses/tapo_exception.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/tapo_response.py` & `plugp100-5.1.0/plugp100/responses/tapo_response.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100/responses/time_info.py` & `plugp100-5.1.0/plugp100/responses/time_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/plugp100.egg-info/PKG-INFO` & `plugp100-5.1.0/plugp100.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 5.0.0.dev6
+Version: 5.1.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-5.0.0.dev6/plugp100.egg-info/SOURCES.txt` & `plugp100-5.1.0/plugp100.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 plugp100/new/tapoplug.py
 plugp100/new/child/__init__.py
 plugp100/new/child/tapohubchildren.py
 plugp100/new/child/tapostripsocket.py
 plugp100/new/components/__init__.py
 plugp100/new/components/alarm_component.py
 plugp100/new/components/battery_component.py
+plugp100/new/components/countdown.py
 plugp100/new/components/device_component.py
 plugp100/new/components/energy_component.py
 plugp100/new/components/hub_children_component.py
 plugp100/new/components/humidity_component.py
 plugp100/new/components/light_component.py
 plugp100/new/components/light_effect_component.py
 plugp100/new/components/motion_sensor_component.py
@@ -93,14 +94,15 @@
 plugp100/responses/__init__.py
 plugp100/responses/alarm_type_list.py
 plugp100/responses/child_device_list.py
 plugp100/responses/components.py
 plugp100/responses/device_state.py
 plugp100/responses/device_usage_info.py
 plugp100/responses/energy_info.py
+plugp100/responses/firmware.py
 plugp100/responses/power_info.py
 plugp100/responses/tapo_exception.py
 plugp100/responses/tapo_response.py
 plugp100/responses/temperature_unit.py
 plugp100/responses/time_info.py
 plugp100/responses/hub_childs/__init__.py
 plugp100/responses/hub_childs/hub_child_base_info.py
```

### Comparing `plugp100-5.0.0.dev6/setup.py` & `plugp100-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/integration/tapo_test_helper.py` & `plugp100-5.1.0/tests/integration/tapo_test_helper.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/integration/test_button_t310.py` & `plugp100-5.1.0/tests/integration/test_button_t310.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/integration/test_hub.py` & `plugp100-5.1.0/tests/integration/test_hub.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/integration/test_ledstrip.py` & `plugp100-5.1.0/tests/integration/test_ledstrip.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/integration/test_light.py` & `plugp100-5.1.0/tests/integration/test_light.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/integration/test_plug.py` & `plugp100-5.1.0/tests/integration/test_plug.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/integration/test_power_strip.py` & `plugp100-5.1.0/tests/integration/test_power_strip.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/integration/test_sensor_s200b.py` & `plugp100-5.1.0/tests/integration/test_sensor_s200b.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/integration/test_tapo_discovery.py` & `plugp100-5.1.0/tests/integration/test_tapo_discovery.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/unit/hub_child/test_button.py` & `plugp100-5.1.0/tests/unit/hub_child/test_button.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/unit/hub_child/test_temp_hum_sensor.py` & `plugp100-5.1.0/tests/unit/hub_child/test_temp_hum_sensor.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/unit/hub_child/test_trv_ke100.py` & `plugp100-5.1.0/tests/unit/hub_child/test_trv_ke100.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/unit/test_bulb.py` & `plugp100-5.1.0/tests/unit/test_bulb.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/unit/test_discovery.py` & `plugp100-5.1.0/tests/unit/test_discovery.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/unit/test_hub.py` & `plugp100-5.1.0/tests/unit/test_hub.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/unit/test_klap_protocol.py` & `plugp100-5.1.0/tests/unit/test_klap_protocol.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/unit/test_plug.py` & `plugp100-5.1.0/tests/unit/test_plug.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/unit/test_plug_strip.py` & `plugp100-5.1.0/tests/unit/test_plug_strip.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev6/tests/unit/test_utils.py` & `plugp100-5.1.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

