# Comparing `tmp/catalystwan-0.31.2.dev2.tar.gz` & `tmp/catalystwan-0.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystwan-0.31.2.dev2.tar", max compression
+gzip compressed data, was "catalystwan-0.32.0.tar", max compression
```

## Comparing `catalystwan-0.31.2.dev2.tar` & `catalystwan-0.32.0.tar`

### file list

```diff
@@ -1,419 +1,334 @@
--rw-r--r--   0        0        0    11375 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/LICENSE
--rw-r--r--   0        0        0    12364 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/README.md
--rw-r--r--   0        0        0     2524 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/__init__.py
--rw-r--r--   0        0        0     1432 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/abstractions.py
--rw-r--r--   0        0        0        0 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/__init__.py
--rw-r--r--   0        0        0     6369 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/admin_tech_api.py
--rw-r--r--   0        0        0    14935 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/administration.py
--rw-r--r--   0        0        0     6314 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/alarms_api.py
--rw-r--r--   0        0        0     3201 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/api_container.py
--rw-r--r--   0        0        0    11636 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/basic_api.py
--rw-r--r--   0        0        0     2053 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/config_device_inventory_api.py
--rw-r--r--   0        0        0     4625 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/config_group_api.py
--rw-r--r--   0        0        0     5557 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/configuration_groups/parcel.py
--rw-r--r--   0        0        0     1290 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/configuration_groups/parcels/cellular_controller.py
--rw-r--r--   0        0        0     7315 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/dashboard_api.py
--rw-r--r--   0        0        0     7360 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/device_action_api.py
--rw-r--r--   0        0        0    28761 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/feature_profile_api.py
--rw-r--r--   0        0        0     1919 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/logs_api.py
--rw-r--r--   0        0        0     2449 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/monitoring_status_api.py
--rw-r--r--   0        0        0     6036 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4394 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/omp_api.py
--rw-r--r--   0        0        0     5691 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/packet_capture_api.py
--rw-r--r--   0        0        0     1654 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/parcel_api.py
--rw-r--r--   0        0        0     5600 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/partition_manager_api.py
--rw-r--r--   0        0        0    29839 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/policy_api.py
--rw-r--r--   0        0        0     2284 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/resource_pool_api.py
--rw-r--r--   0        0        0    11320 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/software_action_api.py
--rw-r--r--   0        0        0     5473 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/speedtest_api.py
--rw-r--r--   0        0        0     7149 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/task_status_api.py
--rw-r--r--   0        0        0    32389 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/template_api.py
--rw-r--r--   0        0        0     3540 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/templates/README.md
--rw-r--r--   0        0        0      251 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/templates/bool_str.py
--rw-r--r--   0        0        0     7481 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/templates/cli_template.py
--rw-r--r--   0        0        0     4213 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      571 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0      137 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/templates/device_variable.py
--rw-r--r--   0        0        0     5235 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/templates/feature_template.py
--rw-r--r--   0        0        0     6678 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      661 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     3244 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0      667 2024-03-27 20:14:32.944515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_banner_model.py
--rw-r--r--   0        0        0     2180 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_bfd_model.py
--rw-r--r--   0        0        0    12522 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_bgp_model.py
--rw-r--r--   0        0        0     3436 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_logging_model.py
--rw-r--r--   0        0        0     1584 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_ntp_model.py
--rw-r--r--   0        0        0     3835 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_omp_model.py
--rw-r--r--   0        0        0     6749 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_ospf.py
--rw-r--r--   0        0        0    13901 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_ospfv3.py
--rw-r--r--   0        0        0     9589 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
--rw-r--r--   0        0        0     2581 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_snmp_model.py
--rw-r--r--   0        0        0     8986 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_system.py
--rw-r--r--   0        0        0    21665 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_vpn_interface_model.py
--rw-r--r--   0        0        0    15328 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_vpn_model.py
--rw-r--r--   0        0        0      472 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cli_template.py
--rw-r--r--   0        0        0     1835 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/omp_vsmart_model.py
--rw-r--r--   0        0        0      806 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/security_vsmart_model.py
--rw-r--r--   0        0        0     1882 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/supported.py
--rw-r--r--   0        0        0     2624 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/models/system_vsmart_model.py
--rw-r--r--   0        0        0     2261 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0     2558 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4547 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2247 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      683 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     7113 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1446 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     5013 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0     4400 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/tenant_management_api.py
--rw-r--r--   0        0        0     5089 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/tenant_migration_api.py
--rw-r--r--   0        0        0    13671 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/api/versions_utils.py
--rw-r--r--   0        0        0    21558 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/dataclasses.py
--rw-r--r--   0        0        0    27675 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/__init__.py
--rw-r--r--   0        0        0    11938 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/administration_user_and_group.py
--rw-r--r--   0        0        0     6731 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/certificate_management_device.py
--rw-r--r--   0        0        0     1274 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/certificate_management_vmanage.py
--rw-r--r--   0        0        0     2554 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/client.py
--rw-r--r--   0        0        0     2770 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/cluster_management.py
--rw-r--r--   0        0        0      983 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/device/software_update.py
--rw-r--r--   0        0        0     9447 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/disaster_recovery.py
--rw-r--r--   0        0        0     2553 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py
--rw-r--r--   0        0        0     4037 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
--rw-r--r--   0        0        0     1249 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py
--rw-r--r--   0        0        0     3662 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
--rw-r--r--   0        0        0     4828 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
--rw-r--r--   0        0        0     1361 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/abstractions.py
--rw-r--r--   0        0        0     1969 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     2024 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2025 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/control.py
--rw-r--r--   0        0        0     2170 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/device_access.py
--rw-r--r--   0        0        0     2239 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     2099 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     1954 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/mesh.py
--rw-r--r--   0        0        0     1991 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/qos_map.py
--rw-r--r--   0        0        0     2065 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/rewrite.py
--rw-r--r--   0        0        0     1967 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/rule_set.py
--rw-r--r--   0        0        0     2092 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/security_group.py
--rw-r--r--   0        0        0     2029 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     2184 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0     2111 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1740 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/app.py
--rw-r--r--   0        0        0     1900 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/app_probe.py
--rw-r--r--   0        0        0     1793 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/as_path.py
--rw-r--r--   0        0        0     1813 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/class_map.py
--rw-r--r--   0        0        0     1772 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/color.py
--rw-r--r--   0        0        0     1854 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/community.py
--rw-r--r--   0        0        0     1971 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0     1873 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/data_prefix.py
--rw-r--r--   0        0        0     2023 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/expanded_community.py
--rw-r--r--   0        0        0     1752 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/fqdn.py
--rw-r--r--   0        0        0     1893 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/geo_location.py
--rw-r--r--   0        0        0     1930 2024-03-27 20:14:32.948515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1873 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0     1833 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/local_app.py
--rw-r--r--   0        0        0     1893 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/local_domain.py
--rw-r--r--   0        0        0     1792 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/mirror.py
--rw-r--r--   0        0        0     1817 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/policer.py
--rw-r--r--   0        0        0     1752 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/port.py
--rw-r--r--   0        0        0     2065 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1852 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/prefix.py
--rw-r--r--   0        0        0     1930 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1683 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/region.py
--rw-r--r--   0        0        0     1892 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/site.py
--rw-r--r--   0        0        0     1782 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/sla.py
--rw-r--r--   0        0        0     1752 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/tloc.py
--rw-r--r--   0        0        0     1863 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
--rw-r--r--   0        0        0     1863 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/url_block_list.py
--rw-r--r--   0        0        0     1734 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/vpn.py
--rw-r--r--   0        0        0     1752 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/zone.py
--rw-r--r--   0        0        0     1782 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/security_template.py
--rw-r--r--   0        0        0     1738 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/vedge_template.py
--rw-r--r--   0        0        0     2672 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/vsmart_template.py
--rw-r--r--   0        0        0     8865 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/software_actions.py
--rw-r--r--   0        0        0     3711 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_dashboard_status.py
--rw-r--r--   0        0        0    10675 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_device_actions.py
--rw-r--r--   0        0        0    13948 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_device_inventory.py
--rw-r--r--   0        0        0      819 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_device_template.py
--rw-r--r--   0        0        0     5277 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_feature_profile.py
--rw-r--r--   0        0        0     5365 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_group.py
--rw-r--r--   0        0        0    22618 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_settings.py
--rw-r--r--   0        0        0    14040 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/endpoints_container.py
--rw-r--r--   0        0        0      760 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/misc.py
--rw-r--r--   0        0        0     6311 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/monitoring_device_details.py
--rw-r--r--   0        0        0     1929 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/monitoring_status.py
--rw-r--r--   0        0        0     1446 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/real_time_monitoring/reboot_history.py
--rw-r--r--   0        0        0     1085 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/sdavc_cloud_connector.py
--rw-r--r--   0        0        0     1050 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/tenant_backup_restore.py
--rw-r--r--   0        0        0     5929 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/tenant_management.py
--rw-r--r--   0        0        0     2792 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/tenant_migration.py
--rw-r--r--   0        0        0     3661 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
--rw-r--r--   0        0        0     5747 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/exceptions.py
--rw-r--r--   0        0        0     2198 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/integration_tests/feature_profile/sdwan/other/test_models.py
--rw-r--r--   0        0        0     1916 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/integration_tests/feature_profile/sdwan/service/test_models.py
--rw-r--r--   0        0        0     7786 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/integration_tests/feature_profile/sdwan/system/test_models.py
--rw-r--r--   0        0        0     1078 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/integration_tests/test_config_migration.py
--rw-r--r--   0        0        0     1845 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/integration_tests/test_find_template_values.py
--rw-r--r--   0        0        0      676 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/logging.conf
--rw-r--r--   0        0        0     5058 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/common.py
--rw-r--r--   0        0        0      171 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/common.py
--rw-r--r--   0        0        0     6573 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/config_migration.py
--rw-r--r--   0        0        0       89 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/docs/README.md
--rw-r--r--   0        0        0   142336 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/docs/diagram.png
--rw-r--r--   0        0        0    10033 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/README.md
--rw-r--r--   0        0        0      663 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/builder.py
--rw-r--r--   0        0        0     9130 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/common.py
--rw-r--r--   0        0        0     1086 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py
--rw-r--r--   0        0        0      420 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/__init__.py
--rw-r--r--   0        0        0     5373 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py
--rw-r--r--   0        0        0     3875 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py
--rw-r--r--   0        0        0     4423 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
--rw-r--r--   0        0        0     1426 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
--rw-r--r--   0        0        0     1203 2024-03-27 20:14:32.952515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
--rw-r--r--   0        0        0      653 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
--rw-r--r--   0        0        0     1244 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
--rw-r--r--   0        0        0     1016 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
--rw-r--r--   0        0        0      807 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
--rw-r--r--   0        0        0     1152 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
--rw-r--r--   0        0        0     1706 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
--rw-r--r--   0        0        0     1332 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py
--rw-r--r--   0        0        0     2995 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
--rw-r--r--   0        0        0     1106 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
--rw-r--r--   0        0        0     5272 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
--rw-r--r--   0        0        0     1215 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
--rw-r--r--   0        0        0     1641 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
--rw-r--r--   0        0        0     1277 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
--rw-r--r--   0        0        0      871 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
--rw-r--r--   0        0        0      830 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
--rw-r--r--   0        0        0     1288 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
--rw-r--r--   0        0        0     1604 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
--rw-r--r--   0        0        0      907 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
--rw-r--r--   0        0        0      799 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
--rw-r--r--   0        0        0     1408 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
--rw-r--r--   0        0        0     1079 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
--rw-r--r--   0        0        0     1461 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
--rw-r--r--   0        0        0      391 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py
--rw-r--r--   0        0        0    14665 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
--rw-r--r--   0        0        0     9779 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
--rw-r--r--   0        0        0    14020 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
--rw-r--r--   0        0        0     5933 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
--rw-r--r--   0        0        0     3835 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
--rw-r--r--   0        0        0     2777 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
--rw-r--r--   0        0        0    14424 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
--rw-r--r--   0        0        0     9128 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
--rw-r--r--   0        0        0     6575 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
--rw-r--r--   0        0        0     7971 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
--rw-r--r--   0        0        0    24489 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
--rw-r--r--   0        0        0    10081 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
--rw-r--r--   0        0        0     3294 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
--rw-r--r--   0        0        0     6725 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
--rw-r--r--   0        0        0    11900 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
--rw-r--r--   0        0        0     6391 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
--rw-r--r--   0        0        0     6993 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
--rw-r--r--   0        0        0     5179 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
--rw-r--r--   0        0        0     3790 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
--rw-r--r--   0        0        0     5294 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
--rw-r--r--   0        0        0     1058 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py
--rw-r--r--   0        0        0    14039 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
--rw-r--r--   0        0        0      977 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py
--rw-r--r--   0        0        0    10457 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py
--rw-r--r--   0        0        0     2427 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py
--rw-r--r--   0        0        0     6396 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py
--rw-r--r--   0        0        0     6355 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py
--rw-r--r--   0        0        0     2935 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py
--rw-r--r--   0        0        0     3841 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py
--rw-r--r--   0        0        0     5186 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py
--rw-r--r--   0        0        0     6653 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/security.py
--rw-r--r--   0        0        0     6841 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py
--rw-r--r--   0        0        0      503 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py
--rw-r--r--   0        0        0    26780 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/bgp.py
--rw-r--r--   0        0        0     2280 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
--rw-r--r--   0        0        0      157 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/profile_type.py
--rw-r--r--   0        0        0      378 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/configuration/topology_group.py
--rw-r--r--   0        0        0     1041 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/device_inventory.py
--rw-r--r--   0        0        0      342 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/feature_profile_parcel.py
--rw-r--r--   0        0        0      785 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/misc/application_protocols.py
--rw-r--r--   0        0        0     8027 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/__init__.py
--rw-r--r--   0        0        0     8308 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/centralized.py
--rw-r--r--   0        0        0     5748 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     5948 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0    12022 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/control.py
--rw-r--r--   0        0        0     4105 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/device_access.py
--rw-r--r--   0        0        0     4219 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     3251 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     1403 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/mesh.py
--rw-r--r--   0        0        0     3520 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/qos_map.py
--rw-r--r--   0        0        0     1415 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/rewrite.py
--rw-r--r--   0        0        0    12467 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/rule_set.py
--rw-r--r--   0        0        0     3187 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/security_group.py
--rw-r--r--   0        0        0    13783 2024-03-27 20:14:32.956515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     1329 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0     9908 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1094 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/app.py
--rw-r--r--   0        0        0     1295 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/app_probe.py
--rw-r--r--   0        0        0      651 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/as_path.py
--rw-r--r--   0        0        0      789 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/class_map.py
--rw-r--r--   0        0        0      661 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/color.py
--rw-r--r--   0        0        0     1378 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/communities.py
--rw-r--r--   0        0        0      918 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0      860 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/data_prefix.py
--rw-r--r--   0        0        0      495 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/fqdn.py
--rw-r--r--   0        0        0     1055 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/geo_location.py
--rw-r--r--   0        0        0      817 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1111 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0      990 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/local_app.py
--rw-r--r--   0        0        0      923 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/local_domain.py
--rw-r--r--   0        0        0      714 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/mirror.py
--rw-r--r--   0        0        0     1127 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/policer.py
--rw-r--r--   0        0        0      771 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/port.py
--rw-r--r--   0        0        0     3196 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1055 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/prefix.py
--rw-r--r--   0        0        0      723 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1325 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/region.py
--rw-r--r--   0        0        0      942 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/site.py
--rw-r--r--   0        0        0     6864 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/sla.py
--rw-r--r--   0        0        0      960 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/tloc.py
--rw-r--r--   0        0        0      856 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/url.py
--rw-r--r--   0        0        0     1071 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/vpn.py
--rw-r--r--   0        0        0     1405 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/list/zone.py
--rw-r--r--   0        0        0     5558 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/localized.py
--rw-r--r--   0        0        0     3686 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/policy.py
--rw-r--r--   0        0        0    32212 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/policy_definition.py
--rw-r--r--   0        0        0     1557 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/policy_list.py
--rw-r--r--   0        0        0     8877 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/policy/security.py
--rw-r--r--   0        0        0     2908 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/models/tenant.py
--rw-r--r--   0        0        0     9590 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/response.py
--rw-r--r--   0        0        0    18707 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/session.py
--rw-r--r--   0        0        0     1236 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/config_migration/test_converter_chooser.py
--rw-r--r--   0        0        0     1731 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/config_migration/test_flatten_general_templates.py
--rw-r--r--   0        0        0     4288 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/config_migration/test_normalizer.py
--rw-r--r--   0        0        0      401 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
--rw-r--r--   0        0        0      513 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/banner_1.json
--rw-r--r--   0        0        0      116 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/basic/alias.json
--rw-r--r--   0        0        0      114 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/basic/basic.json
--rw-r--r--   0        0        0      109 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/basic/basic_no_value.json
--rw-r--r--   0        0        0      848 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/basic/children.json
--rw-r--r--   0        0        0     2348 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/basic/children_nested.json
--rw-r--r--   0        0        0     2348 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      274 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/basic/data_path.json
--rw-r--r--   0        0        0     2973 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/cisco_bfd.json
--rw-r--r--   0        0        0    11100 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/complex_aaa.json
--rw-r--r--   0        0        0    41165 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
--rw-r--r--   0        0        0     5219 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/default_cisco_system.json
--rw-r--r--   0        0        0     5505 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/iuo.json
--rw-r--r--   0        0        0      249 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/omp_1.json
--rw-r--r--   0        0        0      875 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/omp_2.json
--rw-r--r--   0        0        0     1682 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/omp_3.json
--rw-r--r--   0        0        0      662 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/__init__.py
--rw-r--r--   0        0        0     2828 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/cisco_aaa.py
--rw-r--r--   0        0        0      303 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/cisco_banner.py
--rw-r--r--   0        0        0      587 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/cisco_bfd.py
--rw-r--r--   0        0        0      344 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/cisco_system.py
--rw-r--r--   0        0        0     8078 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/cisco_vpn.py
--rw-r--r--   0        0        0     1091 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/omp_vsmart.py
--rw-r--r--   0        0        0      605 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/alias.json
--rw-r--r--   0        0        0      574 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/basic.json
--rw-r--r--   0        0        0     1810 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/children.json
--rw-r--r--   0        0        0     4005 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/children_nested.json
--rw-r--r--   0        0        0     4005 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      731 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/data_path.json
--rw-r--r--   0        0        0    43436 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/cedge_aaa.json
--rw-r--r--   0        0        0     1200 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/cisco_banner.json
--rw-r--r--   0        0        0     9495 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/cisco_bfd.json
--rw-r--r--   0        0        0    99045 2024-03-27 20:14:32.960515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/cisco_system.json
--rw-r--r--   0        0        0    87854 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/cisco_vpn.json
--rw-r--r--   0        0        0     5939 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/omp-vsmart.json
--rw-r--r--   0        0        0     1381 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/test_chose_model.py
--rw-r--r--   0        0        0     2598 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/test_deserialize_model.py
--rw-r--r--   0        0        0     1621 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/test_device_template.py
--rw-r--r--   0        0        0     4598 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/test_generate_payload.py
--rw-r--r--   0        0        0     1756 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/templates/test_serialize_model.py
--rw-r--r--   0        0        0     7945 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    17792 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_administration.py
--rw-r--r--   0        0        0    11116 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8322 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_cli_template.py
--rw-r--r--   0        0        0     5494 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3981 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_device_action_api.py
--rw-r--r--   0        0        0    28154 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_devices_api.py
--rw-r--r--   0        0        0    34937 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_endpoints.py
--rw-r--r--   0        0        0     4045 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_feature_profile_api.py
--rw-r--r--   0        0        0      894 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1545 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_logs_api.py
--rw-r--r--   0        0        0     5489 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_monitoring_status_api.py
--rw-r--r--   0        0        0    11026 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    16472 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_omp_api.py
--rw-r--r--   0        0        0     5223 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_packet_capture.py
--rw-r--r--   0        0        0     5727 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     7335 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_response.py
--rw-r--r--   0        0        0     6724 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_session.py
--rw-r--r--   0        0        0     7117 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6071 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_speed_test_api.py
--rw-r--r--   0        0        0    14851 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_task_status_api.py
--rw-r--r--   0        0        0    15050 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_templates.py
--rw-r--r--   0        0        0     3705 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     6063 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_tenant_management_api.py
--rw-r--r--   0        0        0     4721 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_tenant_migration_api.py
--rw-r--r--   0        0        0    11346 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_typed_list.py
--rw-r--r--   0        0        0     2968 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_version.py
--rw-r--r--   0        0        0    10377 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_version_utils.py
--rw-r--r--   0        0        0     3343 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     8719 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/typed_list.py
--rw-r--r--   0        0        0        0 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/__init__.py
--rw-r--r--   0        0        0      266 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/alarm_status.py
--rw-r--r--   0        0        0      253 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/certificate_status.py
--rw-r--r--   0        0        0      279 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/colors.py
--rw-r--r--   0        0        0      328 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/__init__.py
--rw-r--r--   0        0        0     3445 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/aaa.py
--rw-r--r--   0        0        0     3165 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/appqoe.py
--rw-r--r--   0        0        0      796 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/banner.py
--rw-r--r--   0        0        0      298 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/base.py
--rw-r--r--   0        0        0     3003 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/basic.py
--rw-r--r--   0        0        0      910 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/bfd.py
--rw-r--r--   0        0        0     4366 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/bgp.py
--rw-r--r--   0        0        0     4402 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/dhcp.py
--rw-r--r--   0        0        0     3589 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/factory_method.py
--rw-r--r--   0        0        0      590 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/global_.py
--rw-r--r--   0        0        0     1975 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/logging_.py
--rw-r--r--   0        0        0     2722 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/normalizer.py
--rw-r--r--   0        0        0      928 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/ntp.py
--rw-r--r--   0        0        0     1439 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/omp.py
--rw-r--r--   0        0        0     1568 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/security.py
--rw-r--r--   0        0        0     2062 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/snmp.py
--rw-r--r--   0        0        0     2471 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py
--rw-r--r--   0        0        0     1871 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/feature_template/ucse.py
--rw-r--r--   0        0        0     9236 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/converters/policy/policy_lists.py
--rw-r--r--   0        0        0     3878 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/creators/config_pusher.py
--rw-r--r--   0        0        0     1450 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/creators/strategy/parcels.py
--rw-r--r--   0        0        0      195 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/device_templates/__init__.py
--rw-r--r--   0        0        0      715 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/device_templates/flatten_general_templates.py
--rw-r--r--   0        0        0     1592 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/factories/feature_profile_api.py
--rw-r--r--   0        0        0     1179 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/factories/parcel_pusher.py
--rw-r--r--   0        0        0     1427 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_migration/reverters/config_reverter.py
--rw-r--r--   0        0        0      154 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/config_status.py
--rw-r--r--   0        0        0     4778 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/creation_tools.py
--rw-r--r--   0        0        0     7281 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/dashboard.py
--rw-r--r--   0        0        0     2863 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/device_model.py
--rw-r--r--   0        0        0     2110 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/dict.py
--rw-r--r--   0        0        0      896 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/feature_template/choose_model.py
--rw-r--r--   0        0        0     5009 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/feature_template/find_template_values.py
--rw-r--r--   0        0        0      584 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/operation_status.py
--rw-r--r--   0        0        0      196 2024-03-27 20:14:32.964515 catalystwan-0.31.2.dev2/catalystwan/utils/personality.py
--rw-r--r--   0        0        0      360 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/catalystwan/utils/pydantic_field.py
--rw-r--r--   0        0        0      172 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/catalystwan/utils/reachability.py
--rw-r--r--   0        0        0      407 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/catalystwan/utils/session_type.py
--rw-r--r--   0        0        0      149 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/catalystwan/utils/template_type.py
--rw-r--r--   0        0        0     9825 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/catalystwan/utils/timezone.py
--rw-r--r--   0        0        0     3930 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/catalystwan/utils/upgrades_helper.py
--rw-r--r--   0        0        0      159 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/catalystwan/utils/validate_status.py
--rw-r--r--   0        0        0     3032 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/catalystwan/version.py
--rw-r--r--   0        0        0     5415 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/catalystwan/vmanage_auth.py
--rw-r--r--   0        0        0     8486 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/catalystwan/workflows/config_migration.py
--rw-r--r--   0        0        0     9946 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/catalystwan/workflows/tenant_migration.py
--rw-r--r--   0        0        0      856 2024-03-27 20:14:32.968515 catalystwan-0.31.2.dev2/pyproject.toml
--rw-r--r--   0        0        0    16644 1970-01-01 00:00:00.000000 catalystwan-0.31.2.dev2/setup.py
--rw-r--r--   0        0        0    13476 1970-01-01 00:00:00.000000 catalystwan-0.31.2.dev2/PKG-INFO
+-rw-r--r--   0        0        0    11375 2024-04-08 14:34:01.363267 catalystwan-0.32.0/LICENSE
+-rw-r--r--   0        0        0    12394 2024-04-08 14:34:01.363267 catalystwan-0.32.0/README.md
+-rw-r--r--   0        0        0     2524 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/__init__.py
+-rw-r--r--   0        0        0     1432 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/abstractions.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/__init__.py
+-rw-r--r--   0        0        0     6369 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/admin_tech_api.py
+-rw-r--r--   0        0        0    14935 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/administration.py
+-rw-r--r--   0        0        0     6314 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/alarms_api.py
+-rw-r--r--   0        0        0     3105 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/api_container.py
+-rw-r--r--   0        0        0    11636 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/basic_api.py
+-rw-r--r--   0        0        0     2053 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/config_device_inventory_api.py
+-rw-r--r--   0        0        0     4301 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/config_group_api.py
+-rw-r--r--   0        0        0     4645 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/configuration_groups/parcel.py
+-rw-r--r--   0        0        0     1290 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/configuration_groups/parcels/cellular_controller.py
+-rw-r--r--   0        0        0     7315 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/dashboard_api.py
+-rw-r--r--   0        0        0     7360 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/device_action_api.py
+-rw-r--r--   0        0        0    15767 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/feature_profile_api.py
+-rw-r--r--   0        0        0     1919 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/logs_api.py
+-rw-r--r--   0        0        0     2449 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/monitoring_status_api.py
+-rw-r--r--   0        0        0     6036 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4394 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/omp_api.py
+-rw-r--r--   0        0        0     5691 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/packet_capture_api.py
+-rw-r--r--   0        0        0     1654 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/parcel_api.py
+-rw-r--r--   0        0        0     5600 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/partition_manager_api.py
+-rw-r--r--   0        0        0    28976 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/policy_api.py
+-rw-r--r--   0        0        0     2284 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/resource_pool_api.py
+-rw-r--r--   0        0        0    11320 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/software_action_api.py
+-rw-r--r--   0        0        0     5473 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/speedtest_api.py
+-rw-r--r--   0        0        0     7149 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/task_status_api.py
+-rw-r--r--   0        0        0    29260 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/template_api.py
+-rw-r--r--   0        0        0     3540 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/templates/README.md
+-rw-r--r--   0        0        0      251 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/templates/bool_str.py
+-rw-r--r--   0        0        0     7481 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/templates/cli_template.py
+-rw-r--r--   0        0        0     3107 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      571 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0      137 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/device_variable.py
+-rw-r--r--   0        0        0     5235 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/feature_template.py
+-rw-r--r--   0        0        0     6576 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      661 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     3244 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0      667 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_banner_model.py
+-rw-r--r--   0        0        0     2180 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_bfd_model.py
+-rw-r--r--   0        0        0    12522 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_bgp_model.py
+-rw-r--r--   0        0        0     3436 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_logging_model.py
+-rw-r--r--   0        0        0     1584 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ntp_model.py
+-rw-r--r--   0        0        0     3835 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_omp_model.py
+-rw-r--r--   0        0        0     6749 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ospf.py
+-rw-r--r--   0        0        0    13901 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ospfv3.py
+-rw-r--r--   0        0        0     9589 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
+-rw-r--r--   0        0        0     2581 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_snmp_model.py
+-rw-r--r--   0        0        0     8986 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_system.py
+-rw-r--r--   0        0        0    21665 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_vpn_interface_model.py
+-rw-r--r--   0        0        0    15836 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_vpn_model.py
+-rw-r--r--   0        0        0      472 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cli_template.py
+-rw-r--r--   0        0        0     1835 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      806 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     1882 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/supported.py
+-rw-r--r--   0        0        0     2624 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/system_vsmart_model.py
+-rw-r--r--   0        0        0     2261 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0     2558 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4547 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2247 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      683 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     7113 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1446 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     5013 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     4400 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/tenant_management_api.py
+-rw-r--r--   0        0        0     5089 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/tenant_migration_api.py
+-rw-r--r--   0        0        0    13671 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/versions_utils.py
+-rw-r--r--   0        0        0    21558 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/dataclasses.py
+-rw-r--r--   0        0        0    26501 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/__init__.py
+-rw-r--r--   0        0        0    11938 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/administration_user_and_group.py
+-rw-r--r--   0        0        0     6731 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/certificate_management_device.py
+-rw-r--r--   0        0        0     1274 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/certificate_management_vmanage.py
+-rw-r--r--   0        0        0     2554 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/client.py
+-rw-r--r--   0        0        0     2770 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/cluster_management.py
+-rw-r--r--   0        0        0      983 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/device/software_update.py
+-rw-r--r--   0        0        0     9447 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/disaster_recovery.py
+-rw-r--r--   0        0        0     4037 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
+-rw-r--r--   0        0        0     2064 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
+-rw-r--r--   0        0        0     4836 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
+-rw-r--r--   0        0        0     2028 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     2091 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2092 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/control.py
+-rw-r--r--   0        0        0     2247 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/device_access.py
+-rw-r--r--   0        0        0     2324 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     2174 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     2032 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/mesh.py
+-rw-r--r--   0        0        0     2073 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     2132 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     2039 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     2159 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/security_group.py
+-rw-r--r--   0        0        0     2104 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     2263 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0     2186 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1793 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/app.py
+-rw-r--r--   0        0        0     1950 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/app_probe.py
+-rw-r--r--   0        0        0     1848 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/as_path.py
+-rw-r--r--   0        0        0     1870 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/class_map.py
+-rw-r--r--   0        0        0     1827 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/color.py
+-rw-r--r--   0        0        0     1911 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/community.py
+-rw-r--r--   0        0        0     2016 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0     1932 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/data_prefix.py
+-rw-r--r--   0        0        0     2079 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/expanded_community.py
+-rw-r--r--   0        0        0     1806 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1953 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/geo_location.py
+-rw-r--r--   0        0        0     1974 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1932 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0     1890 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/local_app.py
+-rw-r--r--   0        0        0     1953 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/local_domain.py
+-rw-r--r--   0        0        0     1848 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/mirror.py
+-rw-r--r--   0        0        0     1874 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/policer.py
+-rw-r--r--   0        0        0     1806 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/port.py
+-rw-r--r--   0        0        0     2115 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1848 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/prefix.py
+-rw-r--r--   0        0        0     1974 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1781 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/region.py
+-rw-r--r--   0        0        0     1946 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/site.py
+-rw-r--r--   0        0        0     1845 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/sla.py
+-rw-r--r--   0        0        0     1806 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/tloc.py
+-rw-r--r--   0        0        0     1926 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
+-rw-r--r--   0        0        0     1926 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/url_block_list.py
+-rw-r--r--   0        0        0     1787 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/vpn.py
+-rw-r--r--   0        0        0     1806 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/zone.py
+-rw-r--r--   0        0        0     1782 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/security_template.py
+-rw-r--r--   0        0        0     1738 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/vedge_template.py
+-rw-r--r--   0        0        0     2672 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/vsmart_template.py
+-rw-r--r--   0        0        0     8865 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/software_actions.py
+-rw-r--r--   0        0        0     3711 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_dashboard_status.py
+-rw-r--r--   0        0        0    10675 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_device_actions.py
+-rw-r--r--   0        0        0    13948 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_device_inventory.py
+-rw-r--r--   0        0        0      819 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_device_template.py
+-rw-r--r--   0        0        0     5277 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_feature_profile.py
+-rw-r--r--   0        0        0     4698 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_group.py
+-rw-r--r--   0        0        0    22618 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_settings.py
+-rw-r--r--   0        0        0    14040 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/endpoints_container.py
+-rw-r--r--   0        0        0      760 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/misc.py
+-rw-r--r--   0        0        0     6311 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/monitoring_device_details.py
+-rw-r--r--   0        0        0     1929 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/monitoring_status.py
+-rw-r--r--   0        0        0     1446 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/real_time_monitoring/reboot_history.py
+-rw-r--r--   0        0        0     1085 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/sdavc_cloud_connector.py
+-rw-r--r--   0        0        0     1050 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/tenant_backup_restore.py
+-rw-r--r--   0        0        0     5929 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/tenant_management.py
+-rw-r--r--   0        0        0     2792 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/tenant_migration.py
+-rw-r--r--   0        0        0     3661 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
+-rw-r--r--   0        0        0     5747 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/exceptions.py
+-rw-r--r--   0        0        0     1902 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/integration_tests/test_find_template_values.py
+-rw-r--r--   0        0        0      676 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/logging.conf
+-rw-r--r--   0        0        0     3079 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/common.py
+-rw-r--r--   0        0        0      171 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/common.py
+-rw-r--r--   0        0        0     1090 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/config_migration.py
+-rw-r--r--   0        0        0    10043 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/README.md
+-rw-r--r--   0        0        0      663 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/builder.py
+-rw-r--r--   0        0        0     9117 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/common.py
+-rw-r--r--   0        0        0     1086 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py
+-rw-r--r--   0        0        0     5553 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
+-rw-r--r--   0        0        0     1342 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
+-rw-r--r--   0        0        0     1121 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
+-rw-r--r--   0        0        0      577 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
+-rw-r--r--   0        0        0     1033 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
+-rw-r--r--   0        0        0      885 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
+-rw-r--r--   0        0        0      731 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
+-rw-r--r--   0        0        0     1034 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
+-rw-r--r--   0        0        0     1034 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
+-rw-r--r--   0        0        0     1268 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py
+-rw-r--r--   0        0        0     2867 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
+-rw-r--r--   0        0        0     1028 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
+-rw-r--r--   0        0        0     5197 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
+-rw-r--r--   0        0        0      925 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
+-rw-r--r--   0        0        0     1581 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
+-rw-r--r--   0        0        0     1177 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
+-rw-r--r--   0        0        0      759 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
+-rw-r--r--   0        0        0      738 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
+-rw-r--r--   0        0        0     1182 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
+-rw-r--r--   0        0        0     1496 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
+-rw-r--r--   0        0        0      801 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
+-rw-r--r--   0        0        0      691 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
+-rw-r--r--   0        0        0     1131 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
+-rw-r--r--   0        0        0      883 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
+-rw-r--r--   0        0        0     1384 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
+-rw-r--r--   0        0        0    14665 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
+-rw-r--r--   0        0        0     8961 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
+-rw-r--r--   0        0        0    14020 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
+-rw-r--r--   0        0        0     3448 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
+-rw-r--r--   0        0        0     3835 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
+-rw-r--r--   0        0        0     2777 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
+-rw-r--r--   0        0        0    14424 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
+-rw-r--r--   0        0        0     9128 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
+-rw-r--r--   0        0        0     6575 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
+-rw-r--r--   0        0        0     7971 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
+-rw-r--r--   0        0        0    24489 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
+-rw-r--r--   0        0        0    10081 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
+-rw-r--r--   0        0        0     3294 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
+-rw-r--r--   0        0        0     6725 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
+-rw-r--r--   0        0        0    11900 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
+-rw-r--r--   0        0        0     6391 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
+-rw-r--r--   0        0        0     6993 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
+-rw-r--r--   0        0        0     5179 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
+-rw-r--r--   0        0        0     3790 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
+-rw-r--r--   0        0        0     5294 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
+-rw-r--r--   0        0        0    13826 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
+-rw-r--r--   0        0        0     2179 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
+-rw-r--r--   0        0        0      167 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/profile_type.py
+-rw-r--r--   0        0        0     1041 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/device_inventory.py
+-rw-r--r--   0        0        0      342 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/feature_profile_parcel.py
+-rw-r--r--   0        0        0      785 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/misc/application_protocols.py
+-rw-r--r--   0        0        0     4567 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/__init__.py
+-rw-r--r--   0        0        0     7598 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/centralized.py
+-rw-r--r--   0        0        0     5540 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/access_control_list.py
+-rw-r--r--   0        0        0     5726 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/access_control_list_ipv6.py
+-rw-r--r--   0        0        0    11851 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/control.py
+-rw-r--r--   0        0        0     3861 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/device_access.py
+-rw-r--r--   0        0        0     3961 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/device_access_ipv6.py
+-rw-r--r--   0        0        0     3004 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/hub_and_spoke.py
+-rw-r--r--   0        0        0     1184 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/mesh.py
+-rw-r--r--   0        0        0     3454 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/qos_map.py
+-rw-r--r--   0        0        0     1193 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/rewrite.py
+-rw-r--r--   0        0        0    12252 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/rule_set.py
+-rw-r--r--   0        0        0     2948 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/security_group.py
+-rw-r--r--   0        0        0    13309 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/traffic_data.py
+-rw-r--r--   0        0        0     1074 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/vpn_membership.py
+-rw-r--r--   0        0        0     9345 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/zone_based_firewall.py
+-rw-r--r--   0        0        0    10893 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/lists.py
+-rw-r--r--   0        0        0    14613 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/lists_entries.py
+-rw-r--r--   0        0        0     5558 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/localized.py
+-rw-r--r--   0        0        0     3525 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/policy.py
+-rw-r--r--   0        0        0    31904 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/policy_definition.py
+-rw-r--r--   0        0        0     1274 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/policy_list.py
+-rw-r--r--   0        0        0     7100 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/security.py
+-rw-r--r--   0        0        0     2908 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/tenant.py
+-rw-r--r--   0        0        0     9590 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/response.py
+-rw-r--r--   0        0        0    19161 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/session.py
+-rw-r--r--   0        0        0      401 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
+-rw-r--r--   0        0        0      513 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/banner_1.json
+-rw-r--r--   0        0        0      116 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/alias.json
+-rw-r--r--   0        0        0      114 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/basic.json
+-rw-r--r--   0        0        0      109 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/basic_no_value.json
+-rw-r--r--   0        0        0      848 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children.json
+-rw-r--r--   0        0        0     2348 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children_nested.json
+-rw-r--r--   0        0        0     2348 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      274 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/data_path.json
+-rw-r--r--   0        0        0     2973 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/cisco_bfd.json
+-rw-r--r--   0        0        0    11100 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/complex_aaa.json
+-rw-r--r--   0        0        0    41165 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
+-rw-r--r--   0        0        0     5219 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/default_cisco_system.json
+-rw-r--r--   0        0        0     5505 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/iuo.json
+-rw-r--r--   0        0        0      249 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/omp_1.json
+-rw-r--r--   0        0        0      875 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/omp_2.json
+-rw-r--r--   0        0        0     1682 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/omp_3.json
+-rw-r--r--   0        0        0      662 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/__init__.py
+-rw-r--r--   0        0        0     2828 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_aaa.py
+-rw-r--r--   0        0        0      303 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_banner.py
+-rw-r--r--   0        0        0      587 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_bfd.py
+-rw-r--r--   0        0        0      344 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_system.py
+-rw-r--r--   0        0        0     8078 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_vpn.py
+-rw-r--r--   0        0        0     1091 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/omp_vsmart.py
+-rw-r--r--   0        0        0      605 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/alias.json
+-rw-r--r--   0        0        0      574 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/basic.json
+-rw-r--r--   0        0        0     1810 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children.json
+-rw-r--r--   0        0        0     4005 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children_nested.json
+-rw-r--r--   0        0        0     4005 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      731 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/data_path.json
+-rw-r--r--   0        0        0    43436 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/cedge_aaa.json
+-rw-r--r--   0        0        0     1200 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_banner.json
+-rw-r--r--   0        0        0     9495 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_bfd.json
+-rw-r--r--   0        0        0    99045 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_system.json
+-rw-r--r--   0        0        0    87854 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_vpn.json
+-rw-r--r--   0        0        0     5939 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/omp-vsmart.json
+-rw-r--r--   0        0        0     1381 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/test_chose_model.py
+-rw-r--r--   0        0        0     2598 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/test_deserialize_model.py
+-rw-r--r--   0        0        0     4598 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/test_generate_payload.py
+-rw-r--r--   0        0        0     1756 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/test_serialize_model.py
+-rw-r--r--   0        0        0     7945 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    17792 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_administration.py
+-rw-r--r--   0        0        0    11116 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8322 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_cli_template.py
+-rw-r--r--   0        0        0     5494 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3981 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    28154 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_devices_api.py
+-rw-r--r--   0        0        0    34937 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_endpoints.py
+-rw-r--r--   0        0        0      894 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1545 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_logs_api.py
+-rw-r--r--   0        0        0     5489 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_monitoring_status_api.py
+-rw-r--r--   0        0        0    11026 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    16472 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5223 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     5727 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     7335 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_response.py
+-rw-r--r--   0        0        0     6724 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_session.py
+-rw-r--r--   0        0        0     7117 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6071 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0    14851 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_task_status_api.py
+-rw-r--r--   0        0        0    15050 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_templates.py
+-rw-r--r--   0        0        0     3705 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     6063 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_tenant_management_api.py
+-rw-r--r--   0        0        0     4721 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_tenant_migration_api.py
+-rw-r--r--   0        0        0    11346 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_typed_list.py
+-rw-r--r--   0        0        0     2968 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_version.py
+-rw-r--r--   0        0        0    10377 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3343 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     8719 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/typed_list.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/__init__.py
+-rw-r--r--   0        0        0      266 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/alarm_status.py
+-rw-r--r--   0        0        0      253 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/certificate_status.py
+-rw-r--r--   0        0        0      279 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/colors.py
+-rw-r--r--   0        0        0      154 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/config_status.py
+-rw-r--r--   0        0        0     4778 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/creation_tools.py
+-rw-r--r--   0        0        0     7281 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/dashboard.py
+-rw-r--r--   0        0        0     2863 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/device_model.py
+-rw-r--r--   0        0        0     2110 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/dict.py
+-rw-r--r--   0        0        0      953 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/feature_template/choose_model.py
+-rw-r--r--   0        0        0     5066 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/feature_template/find_template_values.py
+-rw-r--r--   0        0        0      584 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/operation_status.py
+-rw-r--r--   0        0        0      196 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/personality.py
+-rw-r--r--   0        0        0      360 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/pydantic_field.py
+-rw-r--r--   0        0        0      172 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/reachability.py
+-rw-r--r--   0        0        0      407 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/session_type.py
+-rw-r--r--   0        0        0      149 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/template_type.py
+-rw-r--r--   0        0        0    17168 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/timezone.py
+-rw-r--r--   0        0        0     3930 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      159 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/validate_status.py
+-rw-r--r--   0        0        0     3032 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/version.py
+-rw-r--r--   0        0        0     5415 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/vmanage_auth.py
+-rw-r--r--   0        0        0     9946 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/workflows/tenant_migration.py
+-rw-r--r--   0        0        0      862 2024-04-08 14:34:01.387267 catalystwan-0.32.0/pyproject.toml
+-rw-r--r--   0        0        0    15920 1970-01-01 00:00:00.000000 catalystwan-0.32.0/setup.py
+-rw-r--r--   0        0        0    13521 1970-01-01 00:00:00.000000 catalystwan-0.32.0/PKG-INFO
```

### Comparing `catalystwan-0.31.2.dev2/LICENSE` & `catalystwan-0.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/README.md` & `catalystwan-0.32.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -393,15 +393,15 @@
     print(error.response.status_code)
     print(error.info.code)
     print(error.info.message)
     print(error.info.details)
 
 ```
 
-## [Supported API endpoints](https://github.com/CiscoDevNet/catalystwan/blob/main/ENDPOINTS.md)
+## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)
 
 
-## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/catalystwan/blob/main/CONTRIBUTING.md)
+## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)
 
 ## Seeking support
 
-You can contact us by submitting [issues](https://github.com/CiscoDevNet/catalystwan/issues), or directly via mail on vmngclient@cisco.com.
+You can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on vmngclient@cisco.com.
```

#### html2text {}

```diff
@@ -142,12 +142,12 @@
 (warning is suppressed when `catalystwan_devel` environment variable is set):
 ```Python import urllib3 urllib3.disable_warnings
 (urllib3.exceptions.InsecureRequestWarning) ``` ## Catching Exceptions
 ```python try: session.api.users.delete("bogus-user-name") except
 ManagerHTTPError as error: # Process an error. print
 (error.response.status_code) print(error.info.code) print(error.info.message)
 print(error.info.details) ``` ## [Supported API endpoints](https://github.com/
-CiscoDevNet/catalystwan/blob/main/ENDPOINTS.md) ## [Contributing, bug reporting
-and feature requests](https://github.com/CiscoDevNet/catalystwan/blob/main/
-CONTRIBUTING.md) ## Seeking support You can contact us by submitting [issues]
-(https://github.com/CiscoDevNet/catalystwan/issues), or directly via mail on
-vmngclient@cisco.com.
+cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md) ## [Contributing, bug
+reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-
+wan-sdk/blob/main/CONTRIBUTING.md) ## Seeking support You can contact us by
+submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/
+issues), or directly via mail on vmngclient@cisco.com.
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/__init__.py` & `catalystwan-0.32.0/catalystwan/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/abstractions.py` & `catalystwan-0.32.0/catalystwan/abstractions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/admin_tech_api.py` & `catalystwan-0.32.0/catalystwan/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/administration.py` & `catalystwan-0.32.0/catalystwan/api/administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/alarms_api.py` & `catalystwan-0.32.0/catalystwan/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/api_container.py` & `catalystwan-0.32.0/catalystwan/api/api_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     UsersAPI,
 )
 from catalystwan.api.alarms_api import AlarmsAPI
 from catalystwan.api.basic_api import DevicesAPI, DeviceStateAPI
 from catalystwan.api.config_device_inventory_api import ConfigurationDeviceInventoryAPI
 from catalystwan.api.config_group_api import ConfigGroupAPI
 from catalystwan.api.dashboard_api import DashboardAPI
-from catalystwan.api.feature_profile_api import SDRoutingFeatureProfilesAPI, SDWANFeatureProfilesAPI
+from catalystwan.api.feature_profile_api import SDRoutingFeatureProfilesAPI
 from catalystwan.api.logs_api import LogsAPI
 from catalystwan.api.omp_api import OmpAPI
 from catalystwan.api.packet_capture_api import PacketCaptureAPI
 from catalystwan.api.partition_manager_api import PartitionManagerAPI
 from catalystwan.api.policy_api import PolicyAPI
 from catalystwan.api.resource_pool_api import ResourcePoolAPI
 from catalystwan.api.software_action_api import SoftwareActionAPI
@@ -62,8 +62,7 @@
         self.users = UsersAPI(session)
         self.cluster_management = ClusterManagementAPI(session)
         self.user_groups = UserGroupsAPI(session)
         self.resource_groups = ResourceGroupsAPI(session)
         self.sessions = SessionsAPI(session)
         self.policy = PolicyAPI(session)
         self.sd_routing_feature_profiles = SDRoutingFeatureProfilesAPI(session)
-        self.sdwan_feature_profiles = SDWANFeatureProfilesAPI(session)
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/basic_api.py` & `catalystwan-0.32.0/catalystwan/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/config_device_inventory_api.py` & `catalystwan-0.32.0/catalystwan/api/config_device_inventory_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/config_group_api.py` & `catalystwan-0.32.0/catalystwan/api/config_group_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional, Union
-from uuid import UUID
-
-from catalystwan.typed_list import DataSequence
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 from catalystwan.endpoints.configuration_group import (
-    ConfigGroup,
     ConfigGroupAssociatePayload,
     ConfigGroupCreationPayload,
     ConfigGroupCreationResponse,
     ConfigGroupDeployPayload,
     ConfigGroupDeployResponse,
     ConfigGroupDisassociateResponse,
     ConfigGroupEditPayload,
     ConfigGroupEditResponse,
+    ConfigGroupResponsePayload,
     ConfigGroupVariablesCreatePayload,
     ConfigGroupVariablesCreateResponse,
     ConfigGroupVariablesEditPayload,
     ConfigurationGroup,
     DeviceId,
     ProfileId,
     Solution,
@@ -109,22 +106,19 @@
 
         for profile_id in profile_ids:
             profiles.append(ProfileId(id=profile_id))
         payload = ConfigGroupEditPayload(name=name, description=description, solution=solution, profiles=profiles)
 
         return self.endpoint.edit_config_group(config_group_id=cg_id, payload=payload)
 
-    def get(self, group_id: Optional[UUID] = None) -> Union[DataSequence[ConfigGroup], ConfigGroup, None]:
+    def get(self) -> ConfigGroupResponsePayload:
         """
-        Gets list of existing config-groups or single config-group with given ID
-         If given ID is not correct return None
+        Gets list of existing config-groups
         """
-        if group_id is None:
-            return self.endpoint.get()
-        return self.endpoint.get().filter(id=group_id).single_or_default()
+        return self.endpoint.get()
 
     def update_variables(self, cg_id: str, solution: Solution, device_variables: list) -> None:
         """
         Updates device specific variable data in given config-group
         """
         payload = ConfigGroupVariablesEditPayload(solution=solution, devices=device_variables)
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/configuration_groups/parcel.py` & `catalystwan-0.32.0/catalystwan/api/configuration_groups/parcel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,37 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from enum import Enum
 from typing import Any, Dict, Generic, Literal, Optional, TypeVar, get_origin
 
-from pydantic import (
-    AliasPath,
-    BaseModel,
-    ConfigDict,
-    Field,
-    PrivateAttr,
-    SerializerFunctionWrapHandler,
-    model_serializer,
-)
-
-from catalystwan.exceptions import CatalystwanException
+from pydantic import AliasPath, BaseModel, ConfigDict, Field, PrivateAttr, model_serializer
 
 T = TypeVar("T")
 
 
 class _ParcelBase(BaseModel):
-    model_config = ConfigDict(
-        extra="allow", arbitrary_types_allowed=True, populate_by_name=True, json_schema_mode_override="validation"
-    )
+    model_config = ConfigDict(extra="forbid", arbitrary_types_allowed=True, populate_by_name=True)
     parcel_name: str = Field(
         min_length=1,
         max_length=128,
         pattern=r'^[^&<>! "]+$',
         serialization_alias="name",
         validation_alias="name",
     )
     parcel_description: Optional[str] = Field(
         default=None,
         serialization_alias="description",
         validation_alias="description",
         description="Set the parcel description",
     )
+    data: Optional[Any] = None
     _parcel_data_key: str = PrivateAttr(default="data")
 
     @model_serializer(mode="wrap")
-    def envelope_parcel_data(self, handler: SerializerFunctionWrapHandler) -> Dict[str, Any]:
-        """
-        serializes model fields with respect to field validation_alias,
-        sub-classing parcel fields can be defined like following:
-        >>> entries: List[SecurityZoneListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
-
-        "data" is default _parcel_data_key which must match validation_alias prefix,
-        this attribute can be overriden in sub-class when needed
-        """
+    def envelope_parcel_data(self, handler) -> Dict[str, Any]:
         model_dict = handler(self)
         model_dict[self._parcel_data_key] = {}
         remove_keys = []
 
         for key in model_dict.keys():
             field_info = self.model_fields.get(key)
             if field_info and isinstance(field_info.validation_alias, AliasPath):
@@ -58,30 +39,23 @@
                 if aliases and aliases[0] == self._parcel_data_key and len(aliases) == 2:
                     model_dict[self._parcel_data_key][aliases[1]] = model_dict[key]
                     remove_keys.append(key)
         for key in remove_keys:
             del model_dict[key]
         return model_dict
 
-    @classmethod
-    def _get_parcel_type(cls) -> str:
-        field_info = cls.model_fields.get("type_")
-        if field_info is not None:
-            return str(field_info.default)
-        raise CatalystwanException(f"{cls.__name__} field parcel type is not set.")
-
 
 class OptionType(str, Enum):
     GLOBAL = "global"
     DEFAULT = "default"
     VARIABLE = "variable"
 
 
 class ParcelAttribute(BaseModel):
-    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    model_config = ConfigDict(extra="forbid")
     option_type: OptionType = Field(serialization_alias="optionType", validation_alias="optionType")
 
 
 # https://github.com/pydantic/pydantic/discussions/6090
 # Usage: Global[str](value="test")
 class Global(ParcelAttribute, Generic[T]):
     option_type: OptionType = Field(
@@ -112,15 +86,15 @@
     value: str = Field(pattern=r"^\{\{[.\/\[\]a-zA-Z0-9_-]+\}\}$", min_length=1, max_length=64)
 
 
 class Default(ParcelAttribute, Generic[T]):
     option_type: OptionType = Field(
         default=OptionType.DEFAULT, serialization_alias="optionType", validation_alias="optionType"
     )
-    value: Optional[Any] = None
+    value: Any
 
 
 def as_global(value: Any, generic_alias: Any = None):
     """Produces Global object given only value (type is induced from value)
 
     Args:
         value (Any): value of Global object to be produced
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/configuration_groups/parcels/cellular_controller.py` & `catalystwan-0.32.0/catalystwan/api/configuration_groups/parcels/cellular_controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/dashboard_api.py` & `catalystwan-0.32.0/catalystwan/api/dashboard_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/device_action_api.py` & `catalystwan-0.32.0/catalystwan/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/feature_profile_api.py` & `catalystwan-0.32.0/catalystwan/api/feature_profile_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,62 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Optional, Protocol, Type, Union, overload
+from typing import TYPE_CHECKING, Any, Protocol, Type, Union, overload
 from uuid import UUID
 
-from pydantic import Json
-
-from catalystwan.endpoints.configuration.feature_profile.sdwan.other import OtherFeatureProfile
-from catalystwan.endpoints.configuration.feature_profile.sdwan.service import ServiceFeatureProfile
-from catalystwan.endpoints.configuration.feature_profile.sdwan.system import SystemFeatureProfile
-from catalystwan.models.configuration.feature_profile.sdwan.other import AnyOtherParcel
-from catalystwan.models.configuration.feature_profile.sdwan.policy_object.security.url import URLParcel
 from catalystwan.typed_list import DataSequence
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 from catalystwan.api.parcel_api import SDRoutingFullConfigParcelAPI
 from catalystwan.endpoints.configuration.feature_profile.sdwan.policy_object import PolicyObjectFeatureProfile
 from catalystwan.endpoints.configuration_feature_profile import SDRoutingConfigurationFeatureProfile
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
-    FeatureProfileInfo,
-    GetFeatureProfilesPayload,
     Parcel,
     ParcelCreationResponse,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.policy_object import (
+    POLICY_OBJECT_PAYLOAD_ENDPOINT_MAPPING,
     AnyPolicyObjectParcel,
     ApplicationListParcel,
     AppProbeParcel,
     ColorParcel,
     DataPrefixParcel,
     ExpandedCommunityParcel,
     FowardingClassParcel,
     FQDNDomainParcel,
     GeoLocationListParcel,
     IPSSignatureParcel,
     IPv6DataPrefixParcel,
     IPv6PrefixListParcel,
     LocalDomainParcel,
-    PolicerParcel,
+    PolicierParcel,
     PreferredColorGroupParcel,
     PrefixListParcel,
     ProtocolListParcel,
     SecurityApplicationListParcel,
     SecurityDataPrefixParcel,
     SecurityPortParcel,
     SecurityZoneListParcel,
     StandardCommunityParcel,
     TlocParcel,
-)
-from catalystwan.models.configuration.feature_profile.sdwan.system import (
-    AAAParcel,
-    AnySystemParcel,
-    BannerParcel,
-    BasicParcel,
-    BFDParcel,
-    GlobalParcel,
-    LoggingParcel,
-    MRFParcel,
-    NTPParcel,
-    OMPParcel,
-    SecurityParcel,
-    SNMPParcel,
+    URLAllowParcel,
+    URLBlockParcel,
 )
 
 
 class SDRoutingFeatureProfilesAPI:
     def __init__(self, session: ManagerSession):
         self.cli = SDRoutingCLIFeatureProfileAPI(session=session)
-
-
-class SDWANFeatureProfilesAPI:
-    def __init__(self, session: ManagerSession):
         self.policy_object = PolicyObjectFeatureProfileAPI(session=session)
-        self.system = SystemFeatureProfileAPI(session=session)
-        self.other = OtherFeatureProfileAPI(session=session)
-        self.service = ServiceFeatureProfileAPI(session=session)
 
 
 class FeatureProfileAPI(Protocol):
     def init_parcels(self, fp_id: str) -> None:
         """
         Initialized parcel(s) associated with this feature profile
         """
@@ -128,480 +101,14 @@
     def delete(self, fp_id: str) -> None:
         """
         Deletes CLI feature-profile
         """
         self.endpoint.delete_cli_feature_profile(cli_fp_id=fp_id)
 
 
-class OtherFeatureProfileAPI:
-    """
-    SDWAN Feature Profile System APIs
-    """
-
-    def __init__(self, session: ManagerSession):
-        self.session = session
-        self.endpoint = OtherFeatureProfile(session)
-
-    def get_profiles(
-        self, limit: Optional[int] = None, offset: Optional[int] = None
-    ) -> DataSequence[FeatureProfileInfo]:
-        """
-        Get all Other Feature Profiles
-        """
-        payload = GetFeatureProfilesPayload(limit=limit if limit else None, offset=offset if offset else None)
-
-        return self.endpoint.get_sdwan_other_feature_profiles(payload)
-
-    def create_profile(self, name: str, description: str) -> FeatureProfileCreationResponse:
-        """
-        Create Other Feature Profile
-        """
-        payload = FeatureProfileCreationPayload(name=name, description=description)
-        return self.endpoint.create_sdwan_other_feature_profile(payload)
-
-    def delete_profile(self, profile_id: UUID) -> None:
-        """
-        Delete Other Feature Profile
-        """
-        self.endpoint.delete_sdwan_other_feature_profile(profile_id)
-
-    def get(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[AnyOtherParcel],  # UCSE, 1000-eyes, cybervision
-        parcel_id: Union[UUID, None] = None,
-    ) -> DataSequence[Parcel[Any]]:
-        """
-        Get all Other Parcels for selected profile_id and selected type or get one Other Parcel given parcel id
-        """
-
-        if not parcel_id:
-            return self.endpoint.get_all(profile_id, parcel_type._get_parcel_type())
-        return self.endpoint.get_by_id(profile_id, parcel_type._get_parcel_type(), parcel_id)
-
-    def create_parcel(self, profile_id: UUID, payload: AnyOtherParcel) -> ParcelCreationResponse:
-        """
-        Create Other Parcel for selected profile_id based on payload type
-        """
-
-        return self.endpoint.create(profile_id, payload._get_parcel_type(), payload)
-
-    def update_parcel(self, profile_id: UUID, payload: AnyOtherParcel, parcel_id: UUID) -> ParcelCreationResponse:
-        """
-        Update Other Parcel for selected profile_id based on payload type
-        """
-
-        return self.endpoint.update(profile_id, payload._get_parcel_type(), parcel_id, payload)
-
-    def delete_parcel(self, profile_id: UUID, parcel_type: Type[AnyOtherParcel], parcel_id: UUID) -> None:
-        """
-        Delete Other Parcel for selected profile_id based on payload type
-        """
-        return self.endpoint.delete(profile_id, parcel_type._get_parcel_type(), parcel_id)
-
-
-class ServiceFeatureProfileAPI:
-    """
-    SDWAN Feature Profile Service APIs
-    """
-
-    def __init__(self, session: ManagerSession):
-        self.session = session
-        self.endpoint = ServiceFeatureProfile(session)
-
-    def get_profiles(
-        self, limit: Optional[int] = None, offset: Optional[int] = None
-    ) -> DataSequence[FeatureProfileInfo]:
-        """
-        Get all Service Feature Profiles
-        """
-        payload = GetFeatureProfilesPayload(limit=limit if limit else None, offset=offset if offset else None)
-
-        return self.endpoint.get_sdwan_service_feature_profiles(payload)
-
-    def create_profile(self, name: str, description: str) -> FeatureProfileCreationResponse:
-        """
-        Create Service Feature Profile
-        """
-        payload = FeatureProfileCreationPayload(name=name, description=description)
-        return self.endpoint.create_sdwan_service_feature_profile(payload)
-
-    def delete_profile(self, profile_id: UUID) -> None:
-        """
-        Delete Service Feature Profile
-        """
-        self.endpoint.delete_sdwan_service_feature_profile(profile_id)
-
-
-class SystemFeatureProfileAPI:
-    """
-    SDWAN Feature Profile System APIs
-    """
-
-    def __init__(self, session: ManagerSession):
-        self.session = session
-        self.endpoint = SystemFeatureProfile(session)
-
-    def get_profiles(
-        self, limit: Optional[int] = None, offset: Optional[int] = None
-    ) -> DataSequence[FeatureProfileInfo]:
-        """
-        Get all System Feature Profiles
-        """
-        payload = GetFeatureProfilesPayload(limit=limit if limit else None, offset=offset if offset else None)
-
-        return self.endpoint.get_sdwan_system_feature_profiles(payload)
-
-    def create_profile(self, name: str, description: str) -> FeatureProfileCreationResponse:
-        """
-        Create System Feature Profile
-        """
-        payload = FeatureProfileCreationPayload(name=name, description=description)
-        return self.endpoint.create_sdwan_system_feature_profile(payload)
-
-    def delete_profile(self, profile_id: UUID) -> None:
-        """
-        Delete System Feature Profile
-        """
-        self.endpoint.delete_sdwan_system_feature_profile(profile_id)
-
-    def get_schema(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[AnySystemParcel],
-    ) -> Json:
-        """
-        Get all System Parcels for selected profile_id and selected type or get one Policy Object given parcel id
-        """
-
-        return self.endpoint.get_schema(profile_id, parcel_type._get_parcel_type())
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[AAAParcel],
-    ) -> DataSequence[Parcel[AAAParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[BFDParcel],
-    ) -> DataSequence[Parcel[BFDParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[LoggingParcel],
-    ) -> DataSequence[Parcel[LoggingParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[BannerParcel],
-    ) -> DataSequence[Parcel[BannerParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[BasicParcel],
-    ) -> DataSequence[Parcel[BasicParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[GlobalParcel],
-    ) -> DataSequence[Parcel[GlobalParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[NTPParcel],
-    ) -> DataSequence[Parcel[NTPParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[MRFParcel],
-    ) -> DataSequence[Parcel[MRFParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[OMPParcel],
-    ) -> DataSequence[Parcel[OMPParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[SecurityParcel],
-    ) -> DataSequence[Parcel[SecurityParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[SNMPParcel],
-    ) -> DataSequence[Parcel[SNMPParcel]]:
-        ...
-
-    # get by id
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[AAAParcel],
-        parcel_id: UUID,
-    ) -> DataSequence[Parcel[AAAParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[BFDParcel],
-        parcel_id: UUID,
-    ) -> DataSequence[Parcel[BFDParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[LoggingParcel],
-        parcel_id: UUID,
-    ) -> DataSequence[Parcel[LoggingParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[BannerParcel],
-        parcel_id: UUID,
-    ) -> DataSequence[Parcel[BannerParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[BasicParcel],
-        parcel_id: UUID,
-    ) -> DataSequence[Parcel[BasicParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[GlobalParcel],
-        parcel_id: UUID,
-    ) -> DataSequence[Parcel[GlobalParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[NTPParcel],
-        parcel_id: UUID,
-    ) -> DataSequence[Parcel[NTPParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[MRFParcel],
-        parcel_id: UUID,
-    ) -> DataSequence[Parcel[MRFParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[OMPParcel],
-        parcel_id: UUID,
-    ) -> DataSequence[Parcel[OMPParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[SecurityParcel],
-        parcel_id: UUID,
-    ) -> DataSequence[Parcel[SecurityParcel]]:
-        ...
-
-    @overload
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[SNMPParcel],
-        parcel_id: UUID,
-    ) -> DataSequence[Parcel[SNMPParcel]]:
-        ...
-
-    def get_parcels(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[AnySystemParcel],
-        parcel_id: Union[UUID, None] = None,
-    ) -> DataSequence[Parcel[Any]]:
-        """
-        Get all System Parcels for selected profile_id and selected type or get one System Parcel given parcel id
-        """
-
-        if not parcel_id:
-            return self.endpoint.get_all(profile_id, parcel_type._get_parcel_type())
-        return self.endpoint.get_by_id(profile_id, parcel_type._get_parcel_type(), parcel_id)
-
-    def create_parcel(self, profile_id: UUID, payload: AnySystemParcel) -> ParcelCreationResponse:
-        """
-        Create System Parcel for selected profile_id based on payload type
-        """
-
-        return self.endpoint.create(profile_id, payload._get_parcel_type(), payload)
-
-    def update(self, profile_id: UUID, payload: AnySystemParcel, parcel_id: UUID) -> ParcelCreationResponse:
-        """
-        Update System Parcel for selected profile_id based on payload type
-        """
-
-        return self.endpoint.update(profile_id, payload._get_parcel_type(), parcel_id, payload)
-
-    @overload
-    def delete_parcel(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[AAAParcel],
-        parcel_id: UUID,
-    ) -> None:
-        ...
-
-    @overload
-    def delete_parcel(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[BFDParcel],
-        parcel_id: UUID,
-    ) -> None:
-        ...
-
-    @overload
-    def delete_parcel(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[LoggingParcel],
-        parcel_id: UUID,
-    ) -> None:
-        ...
-
-    @overload
-    def delete_parcel(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[BannerParcel],
-        parcel_id: UUID,
-    ) -> None:
-        ...
-
-    @overload
-    def delete_parcel(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[BasicParcel],
-        parcel_id: UUID,
-    ) -> None:
-        ...
-
-    @overload
-    def delete_parcel(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[GlobalParcel],
-        parcel_id: UUID,
-    ) -> None:
-        ...
-
-    @overload
-    def delete_parcel(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[NTPParcel],
-        parcel_id: UUID,
-    ) -> None:
-        ...
-
-    @overload
-    def delete_parcel(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[MRFParcel],
-        parcel_id: UUID,
-    ) -> None:
-        ...
-
-    @overload
-    def delete_parcel(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[OMPParcel],
-        parcel_id: UUID,
-    ) -> None:
-        ...
-
-    @overload
-    def delete_parcel(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[SecurityParcel],
-        parcel_id: UUID,
-    ) -> None:
-        ...
-
-    @overload
-    def delete_parcel(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[SNMPParcel],
-        parcel_id: UUID,
-    ) -> None:
-        ...
-
-    def delete_parcel(self, profile_id: UUID, parcel_type: Type[AnySystemParcel], parcel_id: UUID) -> None:
-        """
-        Delete System Parcel for selected profile_id based on payload type
-        """
-        return self.endpoint.delete(profile_id, parcel_type._get_parcel_type(), parcel_id)
-
-
 class PolicyObjectFeatureProfileAPI:
     """
     SDWAN Feature Profile Policy Object APIs
     """
 
     def __init__(self, session: ManagerSession):
         self.session = session
@@ -652,15 +159,15 @@
         ...
 
     @overload
     def get(self, profile_id: UUID, parcel_type: Type[LocalDomainParcel]) -> DataSequence[Parcel[Any]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[PolicerParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[PolicierParcel]) -> DataSequence[Parcel[Any]]:
         ...
 
     @overload
     def get(self, profile_id: UUID, parcel_type: Type[PreferredColorGroupParcel]) -> DataSequence[Parcel[Any]]:
         ...
 
     @overload
@@ -692,15 +199,19 @@
         ...
 
     @overload
     def get(self, profile_id: UUID, parcel_type: Type[TlocParcel]) -> DataSequence[Parcel[Any]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[URLParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[URLAllowParcel]) -> DataSequence[Parcel[Any]]:
+        ...
+
+    @overload
+    def get(self, profile_id: UUID, parcel_type: Type[URLBlockParcel]) -> DataSequence[Parcel[Any]]:
         ...
 
     # get by id
 
     @overload
     def get(
         self, profile_id: UUID, parcel_type: Type[ApplicationListParcel], parcel_id: UUID
@@ -760,15 +271,15 @@
         ...
 
     @overload
     def get(self, profile_id: UUID, parcel_type: Type[LocalDomainParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[PolicerParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[PolicierParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
         ...
 
     @overload
     def get(
         self, profile_id: UUID, parcel_type: Type[PreferredColorGroupParcel], parcel_id: UUID
     ) -> DataSequence[Parcel[Any]]:
         ...
@@ -814,51 +325,55 @@
         ...
 
     @overload
     def get(self, profile_id: UUID, parcel_type: Type[TlocParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[URLParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[URLAllowParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
+        ...
+
+    @overload
+    def get(self, profile_id: UUID, parcel_type: Type[URLBlockParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
         ...
 
     def get(
         self,
         profile_id: UUID,
         parcel_type: Type[AnyPolicyObjectParcel],
         parcel_id: Union[UUID, None] = None,
     ) -> DataSequence[Parcel[Any]]:
         """
         Get all Policy Objects for selected profile_id and selected type or get one Policy Object given parcel id
         """
 
-        policy_object_list_type = parcel_type._get_parcel_type()
+        policy_object_list_type = POLICY_OBJECT_PAYLOAD_ENDPOINT_MAPPING[parcel_type]
         if not parcel_id:
             return self.endpoint.get_all(profile_id=profile_id, policy_object_list_type=policy_object_list_type)
         parcel = self.endpoint.get_by_id(
             profile_id=profile_id, policy_object_list_type=policy_object_list_type, list_object_id=parcel_id
         )
         return DataSequence(Parcel, [parcel])
 
     def create(self, profile_id: UUID, payload: AnyPolicyObjectParcel) -> ParcelCreationResponse:
         """
         Create Policy Object for selected profile_id based on payload type
         """
 
-        policy_object_list_type = payload._get_parcel_type()
+        policy_object_list_type = POLICY_OBJECT_PAYLOAD_ENDPOINT_MAPPING[type(payload)]
         return self.endpoint.create(
             profile_id=profile_id, policy_object_list_type=policy_object_list_type, payload=payload
         )
 
     def update(self, profile_id: UUID, payload: AnyPolicyObjectParcel, list_object_id: UUID):
         """
         Update Policy Object for selected profile_id based on payload type
         """
 
-        policy_type = payload._get_parcel_type()
+        policy_type = POLICY_OBJECT_PAYLOAD_ENDPOINT_MAPPING[type(payload)]
         return self.endpoint.update(
             profile_id=profile_id, policy_object_list_type=policy_type, list_object_id=list_object_id, payload=payload
         )
 
     @overload
     def delete(self, profile_id: UUID, parcel_type: Type[ApplicationListParcel], list_object_id: UUID) -> None:
         ...
@@ -904,15 +419,15 @@
         ...
 
     @overload
     def delete(self, profile_id: UUID, parcel_type: Type[LocalDomainParcel], list_object_id: UUID) -> None:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[PolicerParcel], list_object_id: UUID) -> None:
+    def delete(self, profile_id: UUID, parcel_type: Type[PolicierParcel], list_object_id: UUID) -> None:
         ...
 
     @overload
     def delete(self, profile_id: UUID, parcel_type: Type[PreferredColorGroupParcel], list_object_id: UUID) -> None:
         ...
 
     @overload
@@ -944,19 +459,23 @@
         ...
 
     @overload
     def delete(self, profile_id: UUID, parcel_type: Type[TlocParcel], list_object_id: UUID) -> None:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[URLParcel], list_object_id: UUID) -> None:
+    def delete(self, profile_id: UUID, parcel_type: Type[URLAllowParcel], list_object_id: UUID) -> None:
+        ...
+
+    @overload
+    def delete(self, profile_id: UUID, parcel_type: Type[URLBlockParcel], list_object_id: UUID) -> None:
         ...
 
     def delete(self, profile_id: UUID, parcel_type: Type[AnyPolicyObjectParcel], list_object_id: UUID) -> None:
         """
         Delete Policy Object for selected profile_id based on payload type
         """
 
-        policy_object_list_type = parcel_type._get_parcel_type()
+        policy_object_list_type = POLICY_OBJECT_PAYLOAD_ENDPOINT_MAPPING[parcel_type]
         return self.endpoint.delete(
             profile_id=profile_id, policy_object_list_type=policy_object_list_type, list_object_id=list_object_id
         )
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/logs_api.py` & `catalystwan-0.32.0/catalystwan/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/monitoring_status_api.py` & `catalystwan-0.32.0/catalystwan/api/monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/mtt_aaa_api.py` & `catalystwan-0.32.0/catalystwan/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/omp_api.py` & `catalystwan-0.32.0/catalystwan/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/packet_capture_api.py` & `catalystwan-0.32.0/catalystwan/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/parcel_api.py` & `catalystwan-0.32.0/catalystwan/api/parcel_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/partition_manager_api.py` & `catalystwan-0.32.0/catalystwan/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/policy_api.py` & `catalystwan-0.32.0/catalystwan/api/policy_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,57 +1,117 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Tuple, Type, overload
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Type, overload
 from uuid import UUID
 
 from catalystwan.api.task_status_api import Task
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints, PolicyListEndpoints
-from catalystwan.endpoints.configuration.policy.definition.access_control_list import ConfigurationPolicyAclDefinition
+from catalystwan.endpoints.configuration.policy.definition.access_control_list import (
+    AclPolicyGetResponse,
+    ConfigurationPolicyAclDefinition,
+)
 from catalystwan.endpoints.configuration.policy.definition.access_control_list_ipv6 import (
+    AclIPv6PolicyGetResponse,
     ConfigurationPolicyAclIPv6Definition,
 )
-from catalystwan.endpoints.configuration.policy.definition.control import ConfigurationPolicyControlDefinition
+from catalystwan.endpoints.configuration.policy.definition.control import (
+    ConfigurationPolicyControlDefinition,
+    ControlPolicyGetResponse,
+)
 from catalystwan.endpoints.configuration.policy.definition.device_access import (
     ConfigurationPolicyDeviceAccessDefinition,
+    DeviceAccessPolicyGetResponse,
 )
 from catalystwan.endpoints.configuration.policy.definition.device_access_ipv6 import (
     ConfigurationPolicyDeviceAccessIPv6Definition,
+    DeviceAccessIPv6PolicyGetResponse,
+)
+from catalystwan.endpoints.configuration.policy.definition.hub_and_spoke import (
+    ConfigurationPolicyHubAndSpokeDefinition,
+    HubAndSpokePolicyGetResponse,
+)
+from catalystwan.endpoints.configuration.policy.definition.mesh import (
+    ConfigurationPolicyMeshDefinition,
+    MeshPolicyGetResponse,
+)
+from catalystwan.endpoints.configuration.policy.definition.qos_map import (
+    ConfigurationPolicyQoSMapDefinition,
+    QoSMapPolicyGetResponse,
+)
+from catalystwan.endpoints.configuration.policy.definition.rewrite import (
+    ConfigurationPolicyRewriteRuleDefinition,
+    RewritePolicyGetResponse,
+)
+from catalystwan.endpoints.configuration.policy.definition.rule_set import (
+    ConfigurationPolicyRuleSetDefinition,
+    RuleSetGetResponse,
 )
-from catalystwan.endpoints.configuration.policy.definition.hub_and_spoke import ConfigurationPolicyHubAndSpokeDefinition
-from catalystwan.endpoints.configuration.policy.definition.mesh import ConfigurationPolicyMeshDefinition
-from catalystwan.endpoints.configuration.policy.definition.qos_map import ConfigurationPolicyQoSMapDefinition
-from catalystwan.endpoints.configuration.policy.definition.rewrite import ConfigurationPolicyRewriteRuleDefinition
-from catalystwan.endpoints.configuration.policy.definition.rule_set import ConfigurationPolicyRuleSetDefinition
 from catalystwan.endpoints.configuration.policy.definition.security_group import (
     ConfigurationPolicySecurityGroupDefinition,
+    SecurityGroupGetResponse,
+)
+from catalystwan.endpoints.configuration.policy.definition.traffic_data import (
+    ConfigurationPolicyDataDefinition,
+    TrafficDataPolicy,
+    TrafficDataPolicyGetResponse,
 )
-from catalystwan.endpoints.configuration.policy.definition.traffic_data import ConfigurationPolicyDataDefinition
 from catalystwan.endpoints.configuration.policy.definition.vpn_membership import (
     ConfigurationPolicyVPNMembershipGroupDefinition,
+    VPNMembershipPolicyGetResponse,
 )
 from catalystwan.endpoints.configuration.policy.definition.zone_based_firewall import (
     ConfigurationPolicyZoneBasedFirewallDefinition,
+    ZoneBasedFWPolicyGetResponse,
 )
 from catalystwan.endpoints.configuration.policy.list.app import AppListInfo, ConfigurationPolicyApplicationList
-from catalystwan.endpoints.configuration.policy.list.app_probe import ConfigurationPolicyAppProbeClassList
+from catalystwan.endpoints.configuration.policy.list.app_probe import (
+    AppProbeClassListInfo,
+    ConfigurationPolicyAppProbeClassList,
+)
 from catalystwan.endpoints.configuration.policy.list.as_path import ASPathListInfo, ConfigurationPolicyASPathList
-from catalystwan.endpoints.configuration.policy.list.class_map import ConfigurationPolicyForwardingClassList
+from catalystwan.endpoints.configuration.policy.list.class_map import (
+    ClassMapListInfo,
+    ConfigurationPolicyForwardingClassList,
+)
 from catalystwan.endpoints.configuration.policy.list.color import ColorListInfo, ConfigurationPolicyColorList
-from catalystwan.endpoints.configuration.policy.list.community import ConfigurationPolicyCommunityList
-from catalystwan.endpoints.configuration.policy.list.data_ipv6_prefix import ConfigurationPolicyDataIPv6PrefixList
-from catalystwan.endpoints.configuration.policy.list.data_prefix import ConfigurationPolicyDataPrefixList
-from catalystwan.endpoints.configuration.policy.list.expanded_community import ConfigurationPolicyExpandedCommunityList
+from catalystwan.endpoints.configuration.policy.list.community import (
+    CommunityListInfo,
+    ConfigurationPolicyCommunityList,
+)
+from catalystwan.endpoints.configuration.policy.list.data_ipv6_prefix import (
+    ConfigurationPolicyDataIPv6PrefixList,
+    DataIPv6PrefixListInfo,
+)
+from catalystwan.endpoints.configuration.policy.list.data_prefix import (
+    ConfigurationPolicyDataPrefixList,
+    DataPrefixListInfo,
+)
+from catalystwan.endpoints.configuration.policy.list.expanded_community import (
+    ConfigurationPolicyExpandedCommunityList,
+    ExpandedCommunityListInfo,
+)
 from catalystwan.endpoints.configuration.policy.list.fqdn import ConfigurationPolicyFQDNList, FQDNListInfo
-from catalystwan.endpoints.configuration.policy.list.geo_location import ConfigurationPolicyGeoLocationList
-from catalystwan.endpoints.configuration.policy.list.ips_signature import ConfigurationPolicyIPSSignatureList
-from catalystwan.endpoints.configuration.policy.list.ipv6_prefix import ConfigurationPolicyIPv6PrefixList
+from catalystwan.endpoints.configuration.policy.list.geo_location import (
+    ConfigurationPolicyGeoLocationList,
+    GeoLocationListInfo,
+)
+from catalystwan.endpoints.configuration.policy.list.ips_signature import (
+    ConfigurationPolicyIPSSignatureList,
+    IPSSignatureListInfo,
+)
+from catalystwan.endpoints.configuration.policy.list.ipv6_prefix import (
+    ConfigurationPolicyIPv6PrefixList,
+    IPv6PrefixListInfo,
+)
 from catalystwan.endpoints.configuration.policy.list.local_app import ConfigurationPolicyLocalAppList, LocalAppListInfo
-from catalystwan.endpoints.configuration.policy.list.local_domain import ConfigurationPolicyLocalDomainList
+from catalystwan.endpoints.configuration.policy.list.local_domain import (
+    ConfigurationPolicyLocalDomainList,
+    LocalDomainListInfo,
+)
 from catalystwan.endpoints.configuration.policy.list.mirror import ConfigurationPolicyMirrorList, MirrorListInfo
 from catalystwan.endpoints.configuration.policy.list.policer import ConfigurationPolicyPolicerClassList, PolicerListInfo
 from catalystwan.endpoints.configuration.policy.list.port import ConfigurationPolicyPortList, PortListInfo
 from catalystwan.endpoints.configuration.policy.list.preferred_color_group import (
     ConfigurationPreferredColorGroupList,
     PreferredColorGroupListInfo,
 )
@@ -77,17 +137,30 @@
 from catalystwan.endpoints.configuration.policy.security_template import ConfigurationSecurityTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vedge_template import ConfigurationVEdgeTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vsmart_template import (
     ConfigurationVSmartTemplatePolicy,
     VSmartConnectivityStatus,
 )
 from catalystwan.models.misc.application_protocols import ApplicationProtocol
-from catalystwan.models.policy import (
-    AnyPolicyDefinition,
-    AnyPolicyList,
+from catalystwan.models.policy import AnyPolicyDefinition, AnyPolicyList
+from catalystwan.models.policy.centralized import CentralizedPolicy, CentralizedPolicyEditPayload, CentralizedPolicyInfo
+from catalystwan.models.policy.definitions.access_control_list import AclPolicy
+from catalystwan.models.policy.definitions.access_control_list_ipv6 import AclIPv6Policy
+from catalystwan.models.policy.definitions.control import ControlPolicy
+from catalystwan.models.policy.definitions.device_access import DeviceAccessPolicy
+from catalystwan.models.policy.definitions.device_access_ipv6 import DeviceAccessIPv6Policy
+from catalystwan.models.policy.definitions.hub_and_spoke import HubAndSpokePolicy
+from catalystwan.models.policy.definitions.mesh import MeshPolicy
+from catalystwan.models.policy.definitions.qos_map import QoSMapPolicy
+from catalystwan.models.policy.definitions.rewrite import RewritePolicy
+from catalystwan.models.policy.definitions.rule_set import RuleSet
+from catalystwan.models.policy.definitions.security_group import SecurityGroup
+from catalystwan.models.policy.definitions.vpn_membership import VPNMembershipPolicy
+from catalystwan.models.policy.definitions.zone_based_firewall import ZoneBasedFWPolicy
+from catalystwan.models.policy.lists import (
     AppList,
     AppProbeClassList,
     ASPathList,
     ClassMapList,
     ColorList,
     CommunityList,
     DataIPv6PrefixList,
@@ -97,66 +170,41 @@
     GeoLocationList,
     IPSSignatureList,
     IPv6PrefixList,
     LocalAppList,
     LocalDomainList,
     MirrorList,
     PolicerList,
+    PolicyListBase,
     PortList,
     PreferredColorGroupList,
     PrefixList,
     ProtocolNameList,
     RegionList,
     SiteList,
     SLAClassList,
     TLOCList,
     URLAllowList,
     URLBlockList,
     VPNList,
     ZoneList,
 )
-from catalystwan.models.policy.centralized import CentralizedPolicy, CentralizedPolicyEditPayload, CentralizedPolicyInfo
-from catalystwan.models.policy.definition.access_control_list import AclPolicy, AclPolicyGetResponse
-from catalystwan.models.policy.definition.access_control_list_ipv6 import AclIPv6Policy, AclIPv6PolicyGetResponse
-from catalystwan.models.policy.definition.control import ControlPolicy, ControlPolicyGetResponse
-from catalystwan.models.policy.definition.device_access import DeviceAccessPolicy, DeviceAccessPolicyGetResponse
-from catalystwan.models.policy.definition.device_access_ipv6 import (
-    DeviceAccessIPv6Policy,
-    DeviceAccessIPv6PolicyGetResponse,
-)
-from catalystwan.models.policy.definition.hub_and_spoke import HubAndSpokePolicy, HubAndSpokePolicyGetResponse
-from catalystwan.models.policy.definition.mesh import MeshPolicy, MeshPolicyGetResponse
-from catalystwan.models.policy.definition.qos_map import QoSMapPolicy, QoSMapPolicyGetResponse
-from catalystwan.models.policy.definition.rewrite import RewritePolicy, RewritePolicyGetResponse
-from catalystwan.models.policy.definition.rule_set import RuleSet, RuleSetGetResponse
-from catalystwan.models.policy.definition.security_group import SecurityGroup, SecurityGroupGetResponse
-from catalystwan.models.policy.definition.traffic_data import TrafficDataPolicy, TrafficDataPolicyGetResponse
-from catalystwan.models.policy.definition.vpn_membership import VPNMembershipPolicy, VPNMembershipPolicyGetResponse
-from catalystwan.models.policy.definition.zone_based_firewall import ZoneBasedFWPolicy, ZoneBasedFWPolicyGetResponse
-from catalystwan.models.policy.list.app_probe import AppProbeClassListInfo
-from catalystwan.models.policy.list.class_map import ClassMapListInfo
-from catalystwan.models.policy.list.communities import CommunityListInfo, ExpandedCommunityListInfo
-from catalystwan.models.policy.list.data_ipv6_prefix import DataIPv6PrefixListInfo
-from catalystwan.models.policy.list.data_prefix import DataPrefixListInfo
-from catalystwan.models.policy.list.geo_location import GeoLocationListInfo
-from catalystwan.models.policy.list.ips_signature import IPSSignatureListInfo
-from catalystwan.models.policy.list.ipv6_prefix import IPv6PrefixListInfo
-from catalystwan.models.policy.list.local_domain import LocalDomainListInfo
 from catalystwan.models.policy.localized import (
     LocalizedPolicy,
     LocalizedPolicyDeviceInfo,
     LocalizedPolicyEditResponse,
     LocalizedPolicyInfo,
 )
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionBase,
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
     PolicyDefinitionInfo,
 )
-from catalystwan.models.policy.policy_list import PolicyListBase
+from catalystwan.models.policy.policy_list import PolicyListEndpoints
 from catalystwan.models.policy.security import (
     AnySecurityPolicy,
     AnySecurityPolicyInfo,
     SecurityPolicy,
     SecurityPolicyEditResponse,
     UnifiedSecurityPolicy,
 )
@@ -587,20 +635,14 @@
 
     def get(self, type: Type[AnyPolicyList], id: Optional[UUID] = None) -> Any:
         endpoints = self.__get_list_endpoints_instance(type)
         if id is not None:
             return endpoints.get_lists_by_id(id=id)
         return endpoints.get_policy_lists()
 
-    def get_all(self) -> List[AnyPolicyList]:
-        infos: List[AnyPolicyList] = []
-        for list_type, _ in POLICY_LIST_ENDPOINTS_MAP.items():
-            infos.extend(self.get(list_type))
-        return infos
-
 
 class PolicyDefinitionsAPI:
     def __init__(self, session: ManagerSession):
         self._session = session
 
     def __get_definition_endpoints_instance(self, payload_type: type) -> PolicyDefinitionEndpoints:
         endpoints_class = POLICY_DEFINITION_ENDPOINTS_MAP.get(payload_type)
@@ -736,20 +778,14 @@
 
     def get(self, type: Type[AnyPolicyDefinition], id: Optional[UUID] = None) -> Any:
         endpoints = self.__get_definition_endpoints_instance(type)
         if id is not None:
             return endpoints.get_policy_definition(id=id)
         return endpoints.get_definitions()
 
-    def get_all(self) -> List[Tuple[type, PolicyDefinitionInfo]]:
-        all_items: List[Tuple[type, PolicyDefinitionInfo]] = []
-        for definition_type, _ in POLICY_DEFINITION_ENDPOINTS_MAP.items():
-            all_items.extend([(definition_type, info) for info in self.get(definition_type)])
-        return all_items
-
 
 class PolicyAPI:
     """This is exposing so called 'UX 1.0' API"""
 
     def __init__(self, session: ManagerSession):
         self._session = session
         self.centralized = CentralizedPolicyAPI(session)
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/resource_pool_api.py` & `catalystwan-0.32.0/catalystwan/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/software_action_api.py` & `catalystwan-0.32.0/catalystwan/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/speedtest_api.py` & `catalystwan-0.32.0/catalystwan/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/task_status_api.py` & `catalystwan-0.32.0/catalystwan/api/task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/template_api.py` & `catalystwan-0.32.0/catalystwan/api/template_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Copyright 2022 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
-import datetime as dt
 import json
 import logging
 from enum import Enum
-from typing import TYPE_CHECKING, Any, List, Optional, Type, overload
+from typing import TYPE_CHECKING, Any, Optional, Type, overload
 
 from ciscoconfparse import CiscoConfParse  # type: ignore
-from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.api.task_status_api import Task
 from catalystwan.api.templates.cli_template import CLITemplate
 from catalystwan.api.templates.device_template.device_template import (
     DeviceSpecificValue,
     DeviceTemplate,
     GeneralTemplate,
@@ -67,51 +65,14 @@
     LAWFUL_INTERCEPTION = "lawful-interception"
     CLOUD_DOCK = "cloud-dock"
     NETWORK_DESIGN = "network-design"
     VMANAGE_DEFAULT = "vmanage-default"
     ALL = "all"
 
 
-class TemplateInformation(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    last_updated_by: str = Field(serialization_alias="lastUpdatedBy", validation_alias="lastUpdatedBy")
-    id: str = Field(serialization_alias="templateId", validation_alias="templateId")
-    factory_default: bool = Field(serialization_alias="factoryDefault", validation_alias="factoryDefault")
-    name: str = Field(serialization_alias="templateName", validation_alias="templateName")
-    devices_attached: int = Field(serialization_alias="devicesAttached", validation_alias="devicesAttached")
-    description: str = Field(serialization_alias="templateDescription", validation_alias="templateDescription")
-    last_updated_on: dt.datetime = Field(serialization_alias="lastUpdatedOn", validation_alias="lastUpdatedOn")
-    resource_group: Optional[str] = Field(
-        default=None, serialization_alias="resourceGroup", validation_alias="resourceGroup"
-    )
-
-
-class FeatureTemplateInformation(TemplateInformation):
-    model_config = ConfigDict(populate_by_name=True)
-
-    template_type: str = Field(serialization_alias="templateType", validation_alias="templateType")
-    device_type: List[str] = Field(serialization_alias="deviceType", validation_alias="deviceType")
-    version: str = Field(serialization_alias="templateMinVersion", validation_alias="templateMinVersion")
-    template_definiton: Optional[str] = Field(
-        default=None, serialization_alias="templateDefinition", validation_alias="templateDefinition"
-    )
-
-
-class DeviceTemplateInformation(TemplateInformation):
-    model_config = ConfigDict(populate_by_name=True)
-
-    device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
-    template_class: str = Field(serialization_alias="templateClass", validation_alias="templateClass")
-    config_type: str = Field(serialization_alias="configType", validation_alias="configType")
-    template_attached: int = Field(serialization_alias="templateAttached", validation_alias="templateAttached")
-    draft_mode: Optional[str] = Field(default=None, serialization_alias="draftMode", validation_alias="draftMode")
-    device_role: Optional[str] = Field(default=None, serialization_alias="deviceRole", validation_alias="deviceRole")
-
-
 class TemplatesAPI:
     def __init__(self, session: ManagerSession) -> None:
         self.session = session
 
     @overload
     def get(self, template: Type[DeviceTemplate]) -> DataSequence[DeviceTemplateInfo]:  # type: ignore
         ...
@@ -733,23 +694,7 @@
         """
         encoded_uuid = device.uuid.replace("/", "%2F")
         endpoint = f"/dataservice/template/config/running/{encoded_uuid}"
         response = self.session.get_json(endpoint)
         config = CiscoConfParse(response["config"].splitlines())
         logger.debug(f"Template loaded from {device.hostname}.")
         return config
-
-    def get_feature_templates(self) -> DataSequence[FeatureTemplateInformation]:
-        endpoint = "/dataservice/template/feature"
-        fr_templates = self.session.get(endpoint)
-        return fr_templates.dataseq(FeatureTemplateInformation)
-
-    def get_device_templates(self) -> DataSequence[DeviceTemplateInformation]:
-        endpoint = "/dataservice/template/device"
-        params = {"feature": "all"}
-        templates = self.session.get(url=endpoint, params=params)
-        return templates.dataseq(DeviceTemplateInformation)
-
-    def get_device_template(self, template_id: str) -> DeviceTemplate:
-        endpoint = f"/dataservice/template/device/object/{template_id}"
-        response = self.session.get(endpoint)
-        return DeviceTemplate(**response.json())
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/README.md` & `catalystwan-0.32.0/catalystwan/api/templates/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/cli_template.py` & `catalystwan-0.32.0/catalystwan/api/templates/cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/device_template/device_template_payload.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/device_template/device_template_payload.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/feature_template.py` & `catalystwan-0.32.0/catalystwan/api/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/feature_template_field.py` & `catalystwan-0.32.0/catalystwan/api/templates/feature_template_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,67 +111,65 @@
                 vipValue="",
                 vipType=FeatureTemplateOptionType.VARIABLE_NAME,
                 vipObjectType=self.objectType,
                 vipVariableName=value.name,
             )
             return nest_value_in_output(vip_variable.model_dump(by_alias=True, exclude_none=True))
 
+        if value is not None and not self.children:
+            output["vipType"] = vip_type or FeatureTemplateOptionType.CONSTANT.value
+            output["vipValue"] = json_dumped_value
+        elif value is not None and self.children:
+            output["vipType"] = vip_type or FeatureTemplateOptionType.CONSTANT.value
+            children_output = []
+            for obj in value:
+                obj_json_dump = obj.model_dump(mode="json")
+                child_payload: dict = {}
+                for child in self.children:  # Child in schema
+                    obj: FeatureTemplate  # type: ignore
+
+                    # We are searching for the model field that
+                    # corresponds to the child element (field from vManage schema)
+                    # If this line fails, it means that the schema from vManage has more fields than the model
+                    # and the model needs to be updated (add missing fields)
+                    model_tuple = next(
+                        filter(
+                            lambda f: (
+                                f[1].alias == child.key
+                                or get_extra_field(f[1], "vmanage_key") == child.key
+                                or f[0] == child.key
+                            ),
+                            obj.model_fields.items(),
+                        )
+                    )
+                    # We get the pydantic model field and the value from the object
+                    model_field = model_tuple[1]
+                    obj_value = getattr(obj, model_tuple[0])
+                    obj_json_value = obj_json_dump.get(model_tuple[0])
+                    po = get_extra_field(model_field, "priority_order")
+                    vip_type = get_extra_field(model_field, "vip_type")
+                    # After we get the data, we create the payload by populating the schema
+                    # Then we merge the payload to the output
+                    merge(
+                        child_payload,
+                        child.payload_scheme(
+                            obj_value,
+                            json_dumped_value=obj_json_value,
+                            priority_order=po,
+                            vip_type=vip_type,
+                        ),
+                    )
+                    if priority_order:
+                        child_payload.update({"priority-order": priority_order})
+                children_output.append(child_payload)
+            output["vipValue"] = children_output
         else:
-            if value is not None:
-                output["vipType"] = vip_type or FeatureTemplateOptionType.CONSTANT.value
-                if self.children:
-                    children_output = []
-                    for obj in value:  # obj is User, atomic value. Loop every child
-                        obj_json_dump = obj.model_dump(mode="json")
-                        child_payload: dict = {}
-                        for child in self.children:  # Child in schema
-                            obj: FeatureTemplate  # type: ignore
-                            model_tuple = next(
-                                filter(
-                                    lambda f: get_extra_field(f[1], "data_path", []) == child.dataPath
-                                    and (
-                                        f[1].alias == child.key
-                                        or get_extra_field(f[1], "vmanage_key") == child.key
-                                        or f[0] == child.key
-                                    ),
-                                    obj.model_fields.items(),
-                                )
-                            )
-                            model_field = model_tuple[1]
-                            obj_value = getattr(obj, model_tuple[0])
-                            obj_json_value = obj_json_dump.get(model_tuple[0])
-                            po = get_extra_field(model_field, "priority_order")
-                            vip_type = get_extra_field(model_field, "vip_type")
-                            merge(
-                                child_payload,
-                                child.payload_scheme(
-                                    obj_value,
-                                    json_dumped_value=obj_json_value,
-                                    priority_order=po,
-                                    vip_type=vip_type,
-                                ),
-                            )
-                            if priority_order:
-                                child_payload.update({"priority-order": priority_order})
-                        children_output.append(child_payload)
-                    output["vipValue"] = children_output
-                else:
-                    output["vipValue"] = json_dumped_value
+            if value is None or "default" in self.dataType:
+                return {}
             else:
-                if value is None:
-                    return {}
-                if "default" in self.dataType:
-                    return {}
-                    # output["vipValue"] = self.dataType["default"] if value is None else value
-                    # output["vipType"] = self.defaultOption.value
-                else:
-                    output["vipValue"] = []
-                    output["vipType"] = FeatureTemplateOptionType.IGNORE.value
-
-        # TODO
-        # DataType to dataclass Model
-        # No default values for everything
+                output["vipValue"] = []
+                output["vipType"] = FeatureTemplateOptionType.IGNORE.value
 
         if self.primaryKeys:
             output["vipPrimaryKey"] = self.primaryKeys
 
         return nest_value_in_output(output)
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/feature_template_payload.py` & `catalystwan-0.32.0/catalystwan/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_aaa_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_banner_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_banner_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_bfd_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_bfd_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_bgp_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_bgp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_logging_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_logging_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_ntp_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ntp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_omp_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_omp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_ospf.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_ospfv3.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_secure_internet_gateway.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_secure_internet_gateway.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_snmp_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_snmp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_system.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_vpn_interface_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_vpn_interface_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/cisco_vpn_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_vpn_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,22 +73,33 @@
 
 class NextHopWithTrack(FeatureTemplateValidator):
     address: Optional[str] = None
     distance: Optional[int] = 1
     tracker: str
 
 
+class RouteInterface(FeatureTemplateValidator):
+    interface_name: str = Field(json_schema_extra={"vmanage_key": "interface-name"})
+    interface_next_hop: Optional[List[NextHop]] = Field(
+        default=None, json_schema_extra={"vmanage_key": "interface-next-hop", "priority_order": ["address", "distance"]}
+    )
+    model_config = ConfigDict(populate_by_name=True)
+
+
 class Routev4(FeatureTemplateValidator):
     prefix: Optional[str] = None
     next_hop: Optional[List[NextHop]] = Field(
         default=None, json_schema_extra={"vmanage_key": "next-hop", "priority_order": ["address", "distance"]}
     )
     next_hop_with_track: Optional[List[NextHopWithTrack]] = Field(
         default=None, json_schema_extra={"vmanage_key": "next-hop-with-track"}
     )
+    route_interface: Optional[RouteInterface] = Field(
+        default=None, json_schema_extra={"vmanage_key": "route-interface"}
+    )
     null0: Optional[bool] = None
     distance: Optional[int] = None
     vpn: Optional[int] = None
     dhcp: Optional[bool] = None
     model_config = ConfigDict(populate_by_name=True)
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/omp_vsmart_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/omp_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/security_vsmart_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/security_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/supported.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/supported.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/models/system_vsmart_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/models/system_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/aaa_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/aaa/feature/user.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/tenant/tenant.json.j2` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/templates/payloads/tenant/tenant_model.py` & `catalystwan-0.32.0/catalystwan/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/tenant_backup_restore_api.py` & `catalystwan-0.32.0/catalystwan/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/tenant_management_api.py` & `catalystwan-0.32.0/catalystwan/api/tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/tenant_migration_api.py` & `catalystwan-0.32.0/catalystwan/api/tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/api/versions_utils.py` & `catalystwan-0.32.0/catalystwan/api/versions_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/dataclasses.py` & `catalystwan-0.32.0/catalystwan/dataclasses.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/__init__.py` & `catalystwan-0.32.0/catalystwan/endpoints/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     Literal,
     Mapping,
     Optional,
     Protocol,
     Sequence,
     Set,
     Tuple,
-    Type,
     TypeVar,
     Union,
     runtime_checkable,
 )
 from uuid import UUID
 
 from packaging.specifiers import SpecifierSet  # type: ignore
@@ -113,55 +112,14 @@
     def json(cls) -> TypeSpecifier:
         return TypeSpecifier(present=True, is_json=True)
 
     @classmethod
     def model_union(cls, models: Sequence[type]) -> TypeSpecifier:
         return TypeSpecifier(present=True, payload_union_model_types=models)
 
-    @classmethod
-    def resolve_nested_base_model_unions(
-        cls, annotation: Any, models_types: List[Union[Type[BaseModelV1], Type[BaseModelV2]]]
-    ) -> List[Union[Type[BaseModelV1], Type[BaseModelV2]]]:
-        type_origin = get_origin(annotation)
-        if isclass(annotation):
-            try:
-                if issubclass(annotation, (BaseModelV1, BaseModelV2)):
-                    return [annotation]
-                raise APIEndpointError(f"Expected: {PayloadType}")
-            except TypeError:
-                raise APIEndpointError(f"Expected: {PayloadType}")
-        # Check if Annnotated[Union[PayloadModelType, ...]], only unions of pydantic models allowed
-        elif type_origin == Annotated:
-            if annotated_origin := get_args(annotation):
-                if (len(annotated_origin) >= 1) and get_origin(annotated_origin[0]) == Union:
-                    type_args = get_args(annotated_origin[0])
-                    if all(isclass(t) for t in type_args) and all(
-                        issubclass(t, (BaseModelV1, BaseModelV2)) for t in type_args
-                    ):
-                        models_types.extend(list(type_args))
-                        return models_types
-                    else:
-                        non_models = [t for t in type_args if not isclass(t)]
-                        for non_model in non_models:
-                            models_types.extend(cls.resolve_nested_base_model_unions(non_model, models_types))
-                        return models_types
-
-        # Check if Union[PayloadModelType, ...], only unions of pydantic models allowed
-        elif type_origin == Union:
-            type_args = get_args(annotation)
-            if all(isclass(t) for t in type_args) and all(issubclass(t, (BaseModelV1, BaseModelV2)) for t in type_args):
-                models_types.extend(list(type_args))
-                return models_types
-            else:
-                non_models = [t for t in type_args if not isclass(t)]
-                for non_model in non_models:
-                    models_types.extend(cls.resolve_nested_base_model_unions(non_model, models_types))
-                return models_types
-        raise APIEndpointError(f"Expected: {PayloadType}")
-
 
 @dataclass
 class APIEndpointRequestMeta:
     """Holds data for endpoints exctracted during decorating. Used for documentation"""
 
     func: Any
     http_request: str
@@ -491,18 +449,35 @@
                 if (
                     (type_args := get_args(annotation))
                     and (len(type_args) == 1)
                     and isclass(type_args[0])
                     and issubclass(type_args[0], (BaseModelV1, BaseModelV2))
                 ):
                     return TypeSpecifier(True, type_origin, type_args[0], None, False, is_optional)
-            else:
-                models = TypeSpecifier.resolve_nested_base_model_unions(annotation, [])
-                return TypeSpecifier.model_union(models)
-        raise APIEndpointError(f"'payload' param must be annotated with supported type: {PayloadType}")
+            # Check if Annnotated[Union[PayloadModelType, ...]], only unions of pydantic models allowed
+            elif type_origin == Annotated:
+                if annotated_origin := get_args(annotation):
+                    if (len(annotated_origin) >= 1) and get_origin(annotated_origin[0]) == Union:
+                        if (
+                            (type_args := get_args(annotated_origin[0]))
+                            and all(isclass(t) for t in type_args)
+                            and all(issubclass(t, (BaseModelV1, BaseModelV2)) for t in type_args)
+                        ):
+                            return TypeSpecifier.model_union(models=list(type_args))
+            # Check if Union[PayloadModelType, ...], only unions of pydantic models allowed
+            elif type_origin == Union:
+                if (
+                    (type_args := get_args(annotation))
+                    and all(isclass(t) for t in type_args)
+                    and all(issubclass(t, (BaseModelV1, BaseModelV2)) for t in type_args)
+                ):
+                    return TypeSpecifier.model_union(models=list(type_args))
+            raise APIEndpointError(f"Expected: {PayloadType} but found payload {annotation}")
+        else:
+            raise APIEndpointError(f"Expected: {PayloadType} but found payload {annotation}")
 
     def check_params(self):
         """Checks params in decorated method definition
 
         Raises:
             APIEndpointError: when decorated params not matching specification
         """
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/administration_user_and_group.py` & `catalystwan-0.32.0/catalystwan/endpoints/administration_user_and_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/certificate_management_device.py` & `catalystwan-0.32.0/catalystwan/endpoints/certificate_management_device.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/certificate_management_vmanage.py` & `catalystwan-0.32.0/catalystwan/endpoints/certificate_management_vmanage.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/client.py` & `catalystwan-0.32.0/catalystwan/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/cluster_management.py` & `catalystwan-0.32.0/catalystwan/endpoints/cluster_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/device/software_update.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/device/software_update.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/disaster_recovery.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/disaster_recovery.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,52 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from typing import Optional
-from uuid import UUID
 
 from catalystwan.api.configuration_groups.parcel import _ParcelBase
-from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
+from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileInfo,
     GetFeatureProfilesPayload,
-    Parcel,
     ParcelId,
+    SchemaTypeQuery,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class OtherFeatureProfile(APIEndpoints):
+class SystemFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.9"), raises=False)
-    @get("​/v1​/feature-profile​/sdwan​/other")
-    def get_sdwan_other_feature_profiles(
+    @get("/v1/feature-profile/sdwan/system/aaa/schema", resp_json_key="request")
+    def get_sdwan_system_aaa_parcel_schema(self, params: SchemaTypeQuery) -> JSON:
+        ...
+
+    @versions(supported_versions=(">=20.9"), raises=False)
+    @get("/v1/feature-profile/sdwan/system")
+    def get_sdwan_system_feature_profiles(
         self, payload: Optional[GetFeatureProfilesPayload]
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @post("/v1/feature-profile/sdwan/other")
-    def create_sdwan_other_feature_profile(
+    @post("/v1/feature-profile/sdwan/system")
+    def create_sdwan_system_feature_profile(
         self, payload: FeatureProfileCreationPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @delete("/v1/feature-profile/sdwan/other/{profile_id}")
-    def delete_sdwan_other_feature_profile(self, profile_id: UUID) -> None:
-        ...
-
-    @versions(supported_versions=(">=20.9"), raises=False)
-    @get("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}")
-    def get_all(self, profile_id: UUID, parcel_type: UUID) -> DataSequence[Parcel]:
-        ...
-
-    @versions(supported_versions=(">=20.9"), raises=False)
-    @get("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}/{parcel_id}")
-    def get_by_id(self, profile_id: UUID, parcel_type: str, parcel_id: UUID) -> Parcel:
-        ...
-
-    @versions(supported_versions=(">=20.9"), raises=False)
-    @put("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}/{parcel_id}")
-    def update(self, profile_id: UUID, parcel_type: str, parcel_id: UUID, payload: _ParcelBase) -> None:
+    @delete("/v1/feature-profile/sdwan/system/{system_id}")
+    def delete_sdwan_system_feature_profile(self, system_id: str) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @delete("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}/{parcel_id}")
-    def delete(self, profile_id: UUID, parcel_type: str, parcel_id: UUID) -> None:
+    @post("/v1/feature-profile/sdwan/system/{system_id}/aaa")
+    def create_aaa_profile_parcel_for_system(self, system_id: str, payload: _ParcelBase) -> ParcelId:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @post("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}")
-    def create(self, profile_id: UUID, parcel_type: str, payload: _ParcelBase) -> ParcelId:
+    @put("/v1/feature-profile/sdwan/system/{system_id}/aaa/{parcel_id}")
+    def edit_aaa_profile_parcel_for_system(self, system_id: str, parcel_id: str, payload: _ParcelBase) -> ParcelId:
         ...
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     FeatureProfileInfo,
     GetFeatureProfilesPayload,
     ParcelCreationResponse,
     ParcelId,
     SchemaTypeQuery,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.management.vpn import ManagementVPN
-from catalystwan.models.configuration.feature_profile.sdwan.transport import CellularControllerParcel
+from catalystwan.models.configuration.feature_profile.sdwan.transport.cellular_controller import CellularController
 from catalystwan.typed_list import DataSequence
 
 
 class TransportFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.13"), raises=False)
     @post("/v1/feature-profile/sdwan/transport")
     def create_transport_feature_profile(
@@ -104,10 +104,10 @@
     @delete("/v1/feature-profile/sdwan/transport/{transport_id}")
     def delete_sdwan_transport_feature_profile(self, transport_id: str) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @post("/v1/feature-profile/sdwan/transport/{transport_id}/cellular-controller")
     def create_cellular_controller_profile_parcel_for_transport(
-        self, transport_id: str, payload: CellularControllerParcel
+        self, transport_id: str, payload: CellularController
     ) -> ParcelId:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/abstractions.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/qos_map.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,62 @@
-from typing import Protocol
-from uuid import UUID
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
-from pydantic import BaseModel
+# mypy: disable-error-code="empty-body"
+from uuid import UUID
 
-from catalystwan.models.policy import AnyPolicyList
+from catalystwan.endpoints import APIEndpoints, delete, get, post, put
+from catalystwan.models.policy.definitions.qos_map import QoSMapPolicy
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
     PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
+    PolicyDefinitionPreview,
 )
-from catalystwan.models.policy.policy_list import PolicyListId, PolicyListInfo
 from catalystwan.typed_list import DataSequence
 
 
-class PolicyListEndpoints(Protocol):
-    def create_policy_list(self, payload: AnyPolicyList) -> PolicyListId:
-        ...
+class QoSMapPolicyEditPayload(QoSMapPolicy, PolicyDefinitionId):
+    pass
+
+
+class QoSMapPolicyGetResponse(QoSMapPolicy, PolicyDefinitionGetResponse):
+    pass
 
-    def delete_policy_list(self, id: UUID) -> None:
-        ...
 
-    def edit_policy_list(self, id: UUID, payload: AnyPolicyList) -> None:
+class ConfigurationPolicyQoSMapDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/qosmap")
+    def create_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionId:
         ...
 
-    def get_lists_by_id(self, id: UUID) -> PolicyListInfo:
+    @delete("/template/policy/definition/qosmap/{id}")
+    def delete_policy_definition(self, id: UUID) -> None:
         ...
 
-    def get_policy_lists(self) -> DataSequence[PolicyListInfo]:
+    def edit_multiple_policy_definition(self):
+        # PUT /template/policy/definition/qosmap/multiple/{id}
         ...
 
+    @put("/template/policy/definition/qosmap/{id}")
+    def edit_policy_definition(self, id: UUID, payload: QoSMapPolicyEditPayload) -> PolicyDefinitionEditResponse:
+        ...
 
-class PolicyDefinitionEndpoints(Protocol):
-    def create_policy_definition(self, payload: BaseModel) -> PolicyDefinitionId:
+    @get("/template/policy/definition/qosmap", "data")
+    def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    def delete_policy_definition(self, id: UUID) -> None:
+    @get("/template/policy/definition/qosmap/{id}")
+    def get_policy_definition(self, id: UUID) -> QoSMapPolicyGetResponse:
         ...
 
-    def edit_policy_definition(self, id: UUID, payload: BaseModel) -> PolicyDefinitionEditResponse:
+    @post("/template/policy/definition/qosmap/preview")
+    def preview_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionPreview:
         ...
 
-    def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
+    @get("/template/policy/definition/qosmap/preview/{id}")
+    def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
-    def get_policy_definition(self, id: UUID) -> PolicyDefinitionGetResponse:
+    def save_policy_definition_in_bulk(self):
+        # PUT /template/policy/definition/qosmap/bulk
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,63 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
+
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.access_control_list import (
-    AclPolicy,
-    AclPolicyEditPayload,
-    AclPolicyGetResponse,
-)
+from catalystwan.models.policy.definitions.traffic_data import TrafficDataPolicy
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyAclDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/acl")
-    def create_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionId:
+class TrafficDataPolicyEditPayload(TrafficDataPolicy, PolicyDefinitionId):
+    pass
+
+
+class TrafficDataPolicyGetResponse(TrafficDataPolicy, PolicyDefinitionGetResponse):
+    pass
+
+
+class ConfigurationPolicyDataDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/data")
+    def create_policy_definition(self, payload: TrafficDataPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/acl/{id}")
+    @delete("/template/policy/definition/data/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/acl/multiple/{id}
+        # PUT /template/policy/definition/data/multiple/{id}
         ...
 
-    @put("/template/policy/definition/acl/{id}")
-    def edit_policy_definition(self, id: UUID, payload: AclPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/data/{id}")
+    def edit_policy_definition(self, id: UUID, payload: TrafficDataPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/acl", "data")
+    @get("/template/policy/definition/data", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/acl/{id}")
-    def get_policy_definition(self, id: UUID) -> AclPolicyGetResponse:
+    @get("/template/policy/definition/data/{id}")
+    def get_policy_definition(self, id: UUID) -> TrafficDataPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/acl/preview")
-    def preview_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/data/preview")
+    def preview_policy_definition(self, payload: TrafficDataPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/acl/preview/{id}")
+    @get("/template/policy/definition/data/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/acl/bulk
+        # PUT /template/policy/definition/data/bulk
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.access_control_list_ipv6 import (
-    AclIPv6Policy,
-    AclIPv6PolicyEditPayload,
-    AclIPv6PolicyGetResponse,
-)
+from catalystwan.models.policy.definitions.access_control_list_ipv6 import AclIPv6Policy
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
+class AclIPv6PolicyEditPayload(AclIPv6Policy, PolicyDefinitionId):
+    pass
+
+
+class AclIPv6PolicyGetResponse(AclIPv6Policy, PolicyDefinitionGetResponse):
+    pass
+
+
 class ConfigurationPolicyAclIPv6Definition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/aclv6")
     def create_policy_definition(self, payload: AclIPv6Policy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/aclv6/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/control.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/control.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.control import (
-    ControlPolicy,
-    ControlPolicyEditPayload,
-    ControlPolicyGetResponse,
-)
+from catalystwan.models.policy.definitions.control import ControlPolicy
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
+class ControlPolicyEditPayload(ControlPolicy, PolicyDefinitionId):
+    pass
+
+
+class ControlPolicyGetResponse(ControlPolicy, PolicyDefinitionGetResponse):
+    pass
+
+
 class ConfigurationPolicyControlDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/control")
     def create_policy_definition(self, payload: ControlPolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/control/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/device_access.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/device_access.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.device_access import (
-    DeviceAccessPolicy,
-    DeviceAccessPolicyEditPayload,
-    DeviceAccessPolicyGetResponse,
-)
+from catalystwan.models.policy.definitions.device_access import DeviceAccessPolicy
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
+class DeviceAccessPolicyEditPayload(DeviceAccessPolicy, PolicyDefinitionId):
+    pass
+
+
+class DeviceAccessPolicyGetResponse(DeviceAccessPolicy, PolicyDefinitionGetResponse):
+    pass
+
+
 class ConfigurationPolicyDeviceAccessDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/deviceaccesspolicy")
     def create_policy_definition(self, payload: DeviceAccessPolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/deviceaccesspolicy/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/rule_set.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,62 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.device_access_ipv6 import (
-    DeviceAccessIPv6Policy,
-    DeviceAccessIPv6PolicyEditPayload,
-    DeviceAccessIPv6PolicyGetResponse,
-)
+from catalystwan.models.policy.definitions.rule_set import RuleSet
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyDeviceAccessIPv6Definition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/deviceaccesspolicyv6")
-    def create_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionId:
+class RuleSetEditPayload(RuleSet, PolicyDefinitionId):
+    pass
+
+
+class RuleSetGetResponse(RuleSet, PolicyDefinitionGetResponse):
+    pass
+
+
+class ConfigurationPolicyRuleSetDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/ruleset")
+    def create_policy_definition(self, payload: RuleSet) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/deviceaccesspolicyv6/{id}")
+    @delete("/template/policy/definition/ruleset/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/deviceaccesspolicyv6/multiple/{id}
+        # PUT /template/policy/definition/ruleset/multiple/{id}
         ...
 
-    @put("/template/policy/definition/deviceaccesspolicyv6/{id}")
-    def edit_policy_definition(
-        self, id: UUID, payload: DeviceAccessIPv6PolicyEditPayload
-    ) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/ruleset/{id}")
+    def edit_policy_definition(self, id: UUID, payload: RuleSetEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/deviceaccesspolicyv6", "data")
+    @get("/template/policy/definition/ruleset", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/deviceaccesspolicyv6/{id}")
-    def get_policy_definition(self, id: UUID) -> DeviceAccessIPv6PolicyGetResponse:
+    @get("/template/policy/definition/ruleset/{id}")
+    def get_policy_definition(self, id: UUID) -> RuleSetGetResponse:
         ...
 
-    @post("/template/policy/definition/deviceaccesspolicyv6/preview")
-    def preview_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/ruleset/preview")
+    def preview_policy_definition(self, payload: RuleSet) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/deviceaccesspolicyv6/preview/{id}")
+    @get("/template/policy/definition/ruleset/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/deviceaccesspolicyv6/bulk
+        # PUT /template/policy/definition/ruleset/bulk
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.hub_and_spoke import (
-    HubAndSpokePolicy,
-    HubAndSpokePolicyEditPayload,
-    HubAndSpokePolicyGetResponse,
-)
+from catalystwan.models.policy.definitions.hub_and_spoke import HubAndSpokePolicy
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
+class HubAndSpokePolicyEditPayload(HubAndSpokePolicy, PolicyDefinitionId):
+    pass
+
+
+class HubAndSpokePolicyGetResponse(HubAndSpokePolicy, PolicyDefinitionGetResponse):
+    pass
+
+
 class ConfigurationPolicyHubAndSpokeDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/hubandspoke")
     def create_policy_definition(self, payload: HubAndSpokePolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/hubandspoke/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/mesh.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,62 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.mesh import MeshPolicy, MeshPolicyEditPayload, MeshPolicyGetResponse
+from catalystwan.models.policy.definitions.vpn_membership import VPNMembershipPolicy
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyMeshDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/mesh")
-    def create_policy_definition(self, payload: MeshPolicy) -> PolicyDefinitionId:
+class VPNMembershipPolicyEditPayload(VPNMembershipPolicy, PolicyDefinitionId):
+    pass
+
+
+class VPNMembershipPolicyGetResponse(VPNMembershipPolicy, PolicyDefinitionGetResponse):
+    pass
+
+
+class ConfigurationPolicyVPNMembershipGroupDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/vpnmembershipgroup")
+    def create_policy_definition(self, payload: VPNMembershipPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/mesh/{id}")
+    @delete("/template/policy/definition/vpnmembershipgroup/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/mesh/multiple/{id}
+        # PUT /template/policy/definition/vpnmembershipgroup/multiple/{id}
         ...
 
-    @put("/template/policy/definition/mesh/{id}")
-    def edit_policy_definition(self, id: UUID, payload: MeshPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/vpnmembershipgroup/{id}")
+    def edit_policy_definition(self, id: UUID, payload: VPNMembershipPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/mesh", "data")
+    @get("/template/policy/definition/vpnmembershipgroup", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/mesh/{id}")
-    def get_policy_definition(self, id: UUID) -> MeshPolicyGetResponse:
+    @get("/template/policy/definition/vpnmembershipgroup/{id}")
+    def get_policy_definition(self, id: UUID) -> VPNMembershipPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/mesh/preview")
-    def preview_policy_definition(self, payload: MeshPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/vpnmembershipgroup/preview")
+    def preview_policy_definition(self, payload: VPNMembershipPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/mesh/preview/{id}")
+    @get("/template/policy/definition/vpnmembershipgroup/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/mesh/bulk
+        # PUT /template/policy/definition/vpnmembershipgroup/bulk
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/qos_map.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,62 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.qos_map import QoSMapPolicy, QoSMapPolicyEditPayload, QoSMapPolicyGetResponse
+from catalystwan.models.policy.definitions.access_control_list import AclPolicy
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyQoSMapDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/qosmap")
-    def create_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionId:
+class AclPolicyEditPayload(AclPolicy, PolicyDefinitionId):
+    pass
+
+
+class AclPolicyGetResponse(AclPolicy, PolicyDefinitionGetResponse):
+    pass
+
+
+class ConfigurationPolicyAclDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/acl")
+    def create_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/qosmap/{id}")
+    @delete("/template/policy/definition/acl/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/qosmap/multiple/{id}
+        # PUT /template/policy/definition/acl/multiple/{id}
         ...
 
-    @put("/template/policy/definition/qosmap/{id}")
-    def edit_policy_definition(self, id: UUID, payload: QoSMapPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/acl/{id}")
+    def edit_policy_definition(self, id: UUID, payload: AclPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/qosmap", "data")
+    @get("/template/policy/definition/acl", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/qosmap/{id}")
-    def get_policy_definition(self, id: UUID) -> QoSMapPolicyGetResponse:
+    @get("/template/policy/definition/acl/{id}")
+    def get_policy_definition(self, id: UUID) -> AclPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/qosmap/preview")
-    def preview_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/acl/preview")
+    def preview_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/qosmap/preview/{id}")
+    @get("/template/policy/definition/acl/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/qosmap/bulk
+        # PUT /template/policy/definition/acl/bulk
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/rewrite.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/rewrite.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.rewrite import (
-    RewritePolicy,
-    RewritePolicyEditPayload,
-    RewritePolicyGetResponse,
-)
+from catalystwan.models.policy.definitions.rewrite import RewritePolicy
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
+class RewritePolicyEditPayload(RewritePolicy, PolicyDefinitionId):
+    pass
+
+
+class RewritePolicyGetResponse(RewritePolicy, PolicyDefinitionGetResponse):
+    pass
+
+
 class ConfigurationPolicyRewriteRuleDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/rewriterule")
     def create_policy_definition(self, payload: RewritePolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/rewriterule/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/rule_set.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/security_group.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,62 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.rule_set import RuleSet, RuleSetEditPayload, RuleSetGetResponse
+from catalystwan.models.policy.definitions.security_group import SecurityGroup
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyRuleSetDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/ruleset")
-    def create_policy_definition(self, payload: RuleSet) -> PolicyDefinitionId:
+class SecurityGroupEditPayload(SecurityGroup, PolicyDefinitionId):
+    pass
+
+
+class SecurityGroupGetResponse(SecurityGroup, PolicyDefinitionGetResponse):
+    pass
+
+
+class ConfigurationPolicySecurityGroupDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/securitygroup")
+    def create_policy_definition(self, payload: SecurityGroup) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/ruleset/{id}")
+    @delete("/template/policy/definition/securitygroup/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/ruleset/multiple/{id}
+        # PUT /template/policy/definition/securitygroup/multiple/{id}
         ...
 
-    @put("/template/policy/definition/ruleset/{id}")
-    def edit_policy_definition(self, id: UUID, payload: RuleSetEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/securitygroup/{id}")
+    def edit_policy_definition(self, id: UUID, payload: SecurityGroupEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/ruleset", "data")
+    @get("/template/policy/definition/securitygroup", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/ruleset/{id}")
-    def get_policy_definition(self, id: UUID) -> RuleSetGetResponse:
+    @get("/template/policy/definition/securitygroup/{id}")
+    def get_policy_definition(self, id: UUID) -> SecurityGroupGetResponse:
         ...
 
-    @post("/template/policy/definition/ruleset/preview")
-    def preview_policy_definition(self, payload: RuleSet) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/securitygroup/preview")
+    def preview_policy_definition(self, payload: SecurityGroup) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/ruleset/preview/{id}")
+    @get("/template/policy/definition/securitygroup/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/ruleset/bulk
+        # PUT /template/policy/definition/securitygroup/bulk
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/security_group.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/security_template.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
-from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.security_group import (
-    SecurityGroup,
-    SecurityGroupEditPayload,
-    SecurityGroupGetResponse,
-)
-from catalystwan.models.policy.policy_definition import (
-    PolicyDefinitionEditResponse,
-    PolicyDefinitionId,
-    PolicyDefinitionInfo,
-    PolicyDefinitionPreview,
+from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put
+from catalystwan.models.policy.security import (
+    AnySecurityPolicy,
+    SecurityPolicyEditResponse,
+    SecurityPolicyInfoRoot,
+    SecurityPolicyRoot,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicySecurityGroupDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/securitygroup")
-    def create_policy_definition(self, payload: SecurityGroup) -> PolicyDefinitionId:
+class ConfigurationSecurityTemplatePolicy(APIEndpoints):
+    @post("/template/policy/security")
+    def create_security_template(self, payload: AnySecurityPolicy) -> None:
+        ...
+
+    @delete("/template/policy/security/{id}")
+    def delete_security_template(self, id: UUID, payload: JSON = {}) -> None:
         ...
 
-    @delete("/template/policy/definition/securitygroup/{id}")
-    def delete_policy_definition(self, id: UUID) -> None:
+    @put("/template/policy/security/{id}")
+    def edit_security_template(self, id: UUID, payload: AnySecurityPolicy) -> SecurityPolicyEditResponse:
+        # PUT /template/policy/security/{policyId}
         ...
 
-    def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/securitygroup/multiple/{id}
+    def edit_template_with_lenient_lock(self):
+        # PUT /template/policy/security/staging/{policyId}
         ...
 
-    @put("/template/policy/definition/securitygroup/{id}")
-    def edit_policy_definition(self, id: UUID, payload: SecurityGroupEditPayload) -> PolicyDefinitionEditResponse:
+    def generate_security_policy_summary(self):
+        # GET /template/policy/security/summary
         ...
 
-    @get("/template/policy/definition/securitygroup", "data")
-    def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
+    @get("/template/policy/security", "data")
+    def generate_security_template_list(self) -> DataSequence[SecurityPolicyInfoRoot]:
         ...
 
-    @get("/template/policy/definition/securitygroup/{id}")
-    def get_policy_definition(self, id: UUID) -> SecurityGroupGetResponse:
+    def get_device_list_by_id(self):
+        # GET /template/policy/security/devices/{policyId}
         ...
 
-    @post("/template/policy/definition/securitygroup/preview")
-    def preview_policy_definition(self, payload: SecurityGroup) -> PolicyDefinitionPreview:
+    def get_security_policy_device_list(self):
+        # GET /template/policy/security/devices
         ...
 
-    @get("/template/policy/definition/securitygroup/preview/{id}")
-    def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
+    @get("/template/policy/security/definition/{id}")
+    def get_security_template(self, id: UUID) -> SecurityPolicyRoot:
         ...
 
-    def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/securitygroup/bulk
+    def get_security_templates_for_device(self):
+        # GET /template/policy/security/{deviceModel}
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/traffic_data.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
-
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.traffic_data import (
-    TrafficDataPolicy,
-    TrafficDataPolicyEditPayload,
-    TrafficDataPolicyGetResponse,
-)
+from catalystwan.models.policy.definitions.zone_based_firewall import ZoneBasedFWPolicy
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyDataDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/data")
-    def create_policy_definition(self, payload: TrafficDataPolicy) -> PolicyDefinitionId:
+class ZoneBasedFWPolicyEditPayload(ZoneBasedFWPolicy, PolicyDefinitionId):
+    pass
+
+
+class ZoneBasedFWPolicyGetResponse(ZoneBasedFWPolicy, PolicyDefinitionGetResponse):
+    pass
+
+
+class ConfigurationPolicyZoneBasedFirewallDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/zonebasedfw")
+    def create_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/data/{id}")
+    @delete("/template/policy/definition/zonebasedfw/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/data/multiple/{id}
+        # PUT /template/policy/definition/zonebasedfw/multiple/{id}
         ...
 
-    @put("/template/policy/definition/data/{id}")
-    def edit_policy_definition(self, id: UUID, payload: TrafficDataPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/zonebasedfw/{id}")
+    def edit_policy_definition(self, id: UUID, payload: ZoneBasedFWPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/data", "data")
+    @get("/template/policy/definition/zonebasedfw", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/data/{id}")
-    def get_policy_definition(self, id: UUID) -> TrafficDataPolicyGetResponse:
+    @get("/template/policy/definition/zonebasedfw/{id}")
+    def get_policy_definition(self, id: UUID) -> ZoneBasedFWPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/data/preview")
-    def preview_policy_definition(self, payload: TrafficDataPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/zonebasedfw/preview")
+    def preview_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/data/preview/{id}")
+    @get("/template/policy/definition/zonebasedfw/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/data/bulk
+        # PUT /template/policy/definition/zonebasedfw/bulk
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,64 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
-from catalystwan.models.policy.definition.zone_based_firewall import (
-    ZoneBasedFWPolicy,
-    ZoneBasedFWPolicyEditPayload,
-    ZoneBasedFWPolicyGetResponse,
-)
+from catalystwan.models.policy.definitions.device_access_ipv6 import DeviceAccessIPv6Policy
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
+    PolicyDefinitionEndpoints,
+    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyZoneBasedFirewallDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/zonebasedfw")
-    def create_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionId:
+class DeviceAccessIPv6PolicyEditPayload(DeviceAccessIPv6Policy, PolicyDefinitionId):
+    pass
+
+
+class DeviceAccessIPv6PolicyGetResponse(DeviceAccessIPv6Policy, PolicyDefinitionGetResponse):
+    pass
+
+
+class ConfigurationPolicyDeviceAccessIPv6Definition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/deviceaccesspolicyv6")
+    def create_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/zonebasedfw/{id}")
+    @delete("/template/policy/definition/deviceaccesspolicyv6/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/zonebasedfw/multiple/{id}
+        # PUT /template/policy/definition/deviceaccesspolicyv6/multiple/{id}
         ...
 
-    @put("/template/policy/definition/zonebasedfw/{id}")
-    def edit_policy_definition(self, id: UUID, payload: ZoneBasedFWPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/deviceaccesspolicyv6/{id}")
+    def edit_policy_definition(
+        self, id: UUID, payload: DeviceAccessIPv6PolicyEditPayload
+    ) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/zonebasedfw", "data")
+    @get("/template/policy/definition/deviceaccesspolicyv6", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/zonebasedfw/{id}")
-    def get_policy_definition(self, id: UUID) -> ZoneBasedFWPolicyGetResponse:
+    @get("/template/policy/definition/deviceaccesspolicyv6/{id}")
+    def get_policy_definition(self, id: UUID) -> DeviceAccessIPv6PolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/zonebasedfw/preview")
-    def preview_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/deviceaccesspolicyv6/preview")
+    def preview_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/zonebasedfw/preview/{id}")
+    @get("/template/policy/definition/deviceaccesspolicyv6/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/zonebasedfw/bulk
+        # PUT /template/policy/definition/deviceaccesspolicyv6/bulk
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/app.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/zone.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.app import AppList, AppListEditPayload, AppListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import ZoneList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyApplicationList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/app")
-    def create_policy_list(self, payload: AppList) -> PolicyListId:
+class ZoneListEditPayload(ZoneList, PolicyListId):
+    pass
+
+
+class ZoneListInfo(ZoneList, PolicyListInfo):
+    pass
+
+
+class ConfigurationPolicyZoneList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/zone")
+    def create_policy_list(self, payload: ZoneList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/app/{id}")
+    @delete("/template/policy/list/zone/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/app")
+    @delete("/template/policy/list/zone")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/app/{id}")
-    def edit_policy_list(self, id: UUID, payload: AppListEditPayload) -> None:
+    @put("/template/policy/list/zone/{id}")
+    def edit_policy_list(self, id: UUID, payload: ZoneListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/app/{id}")
-    def get_lists_by_id(self, id: UUID) -> AppListInfo:
+    @get("/template/policy/list/zone/{id}")
+    def get_lists_by_id(self, id: UUID) -> ZoneListInfo:
         ...
 
-    @get("/template/policy/list/app", "data")
-    def get_policy_lists(self) -> DataSequence[AppListInfo]:
+    @get("/template/policy/list/zone", "data")
+    def get_policy_lists(self) -> DataSequence[ZoneListInfo]:
         ...
 
-    @get("/template/policy/list/app/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[AppListInfo]:
+    @get("/template/policy/list/zone/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[ZoneListInfo]:
         ...
 
-    @post("/template/policy/list/app/preview")
-    def preview_policy_list(self, payload: AppList) -> PolicyListPreview:
+    @post("/template/policy/list/zone/preview")
+    def preview_policy_list(self, payload: ZoneList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/app/preview/{id}")
+    @get("/template/policy/list/zone/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/app_probe.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/app_probe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.app_probe import (
-    AppProbeClassList,
-    AppProbeClassListEditPayload,
-    AppProbeClassListInfo,
+from catalystwan.models.policy.lists import AppProbeClassList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
 )
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
+class AppProbeClassListEditPayload(AppProbeClassList, PolicyListId):
+    pass
+
+
+class AppProbeClassListInfo(AppProbeClassList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyAppProbeClassList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/appprobe")
     def create_policy_list(self, payload: AppProbeClassList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/appprobe/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/as_path.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/as_path.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.as_path import ASPathList, ASPathListEditPayload, ASPathListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import ASPathList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
+class ASPathListEditPayload(ASPathList, PolicyListId):
+    pass
+
+
+class ASPathListInfo(ASPathList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyASPathList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/aspath")
     def create_policy_list(self, payload: ASPathList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/aspath/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/class_map.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/class_map.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.class_map import ClassMapList, ClassMapListEditPayload, ClassMapListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import ClassMapList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
+class ClassMapListEditPayload(ClassMapList, PolicyListId):
+    pass
+
+
+class ClassMapListInfo(ClassMapList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyForwardingClassList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/class")
     def create_policy_list(self, payload: ClassMapList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/class/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/color.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/color.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.color import ColorList, ColorListEditPayload, ColorListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import ColorList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
+class ColorListEditPayload(ColorList, PolicyListId):
+    pass
+
+
+class ColorListInfo(ColorList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyColorList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/color")
     def create_policy_list(self, payload: ColorList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/color/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/community.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/community.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.communities import CommunityList, CommunityListEditPayload, CommunityListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import CommunityList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
+class CommunityListEditPayload(CommunityList, PolicyListId):
+    pass
+
+
+class CommunityListInfo(CommunityList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyCommunityList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/community")
     def create_policy_list(self, payload: CommunityList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/community/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.data_ipv6_prefix import (
-    DataIPv6PrefixList,
-    DataIPv6PrefixListEditPayload,
-    DataIPv6PrefixListInfo,
+from catalystwan.models.policy.lists import DataIPv6PrefixList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
 )
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
+class DataIPv6PrefixListEditPayload(DataIPv6PrefixList, PolicyListId):
+    pass
+
+
+class DataIPv6PrefixListInfo(DataIPv6PrefixList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyDataIPv6PrefixList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/dataipv6prefix")
     def create_policy_list(self, payload: DataIPv6PrefixList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/dataipv6prefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/data_prefix.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/prefix.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.data_prefix import DataPrefixList, DataPrefixListEditPayload, DataPrefixListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import PrefixList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyDataPrefixList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/dataprefix")
-    def create_policy_list(self, payload: DataPrefixList) -> PolicyListId:
+class PrefixListEditPayload(PrefixList, PolicyListId):
+    pass
+
+
+class PrefixListInfo(PrefixList, PolicyListInfo):
+    pass
+
+
+class ConfigurationPolicyPrefixList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/prefix")
+    def create_policy_list(self, payload: PrefixList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/dataprefix/{id}")
+    @delete("/template/policy/list/prefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/dataprefix")
+    @delete("/template/policy/list/prefix")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/dataprefix/{id}")
-    def edit_policy_list(self, id: UUID, payload: DataPrefixListEditPayload) -> None:
+    @put("/template/policy/list/prefix/{id}")
+    def edit_policy_list(self, id: UUID, payload: PrefixListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/dataprefix/{id}")
-    def get_lists_by_id(self, id: UUID) -> DataPrefixListInfo:
+    @get("/template/policy/list/prefix/{id}")
+    def get_lists_by_id(self, id: UUID) -> PrefixListInfo:
         ...
 
-    @get("/template/policy/list/dataprefix", "data")
-    def get_policy_lists(self) -> DataSequence[DataPrefixListInfo]:
+    @get("/template/policy/list/prefix", "data")
+    def get_policy_lists(self) -> DataSequence[PrefixListInfo]:
         ...
 
-    @get("/template/policy/list/dataprefix/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[DataPrefixListInfo]:
+    @get("/template/policy/list/prefix/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[PrefixListInfo]:
         ...
 
-    @post("/template/policy/list/dataprefix/preview")
-    def preview_policy_list(self, payload: DataPrefixList) -> PolicyListPreview:
+    @post("/template/policy/list/prefix/preview")
+    def preview_policy_list(self, payload: PrefixList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/dataprefix/preview/{id}")
+    @get("/template/policy/list/prefix/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/expanded_community.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/expanded_community.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.communities import (
-    ExpandedCommunityList,
-    ExpandedCommunityListEditPayload,
-    ExpandedCommunityListInfo,
+from catalystwan.models.policy.lists import ExpandedCommunityList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
 )
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
+class ExpandedCommunityListEditPayload(ExpandedCommunityList, PolicyListId):
+    pass
+
+
+class ExpandedCommunityListInfo(ExpandedCommunityList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyExpandedCommunityList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/expandedcommunity")
     def create_policy_list(self, payload: ExpandedCommunityList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/expandedcommunity/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/fqdn.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/fqdn.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.fqdn import FQDNList, FQDNListEditPayload, FQDNListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import FQDNList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
+class FQDNListEditPayload(FQDNList, PolicyListId):
+    pass
+
+
+class FQDNListInfo(FQDNList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyFQDNList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/fqdn")
     def create_policy_list(self, payload: FQDNList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/fqdn/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/geo_location.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/local_app.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.geo_location import GeoLocationList, GeoLocationListEditPayload, GeoLocationListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import LocalAppList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyGeoLocationList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/geolocation")
-    def create_policy_list(self, payload: GeoLocationList) -> PolicyListId:
+class LocalAppListEditPayload(LocalAppList, PolicyListId):
+    pass
+
+
+class LocalAppListInfo(LocalAppList, PolicyListInfo):
+    pass
+
+
+class ConfigurationPolicyLocalAppList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/localapp")
+    def create_policy_list(self, payload: LocalAppList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/geolocation/{id}")
+    @delete("/template/policy/list/localapp/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/geolocation")
+    @delete("/template/policy/list/localapp")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/geolocation/{id}")
-    def edit_policy_list(self, id: UUID, payload: GeoLocationListEditPayload) -> None:
+    @put("/template/policy/list/localapp/{id}")
+    def edit_policy_list(self, id: UUID, payload: LocalAppListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/geolocation/{id}")
-    def get_lists_by_id(self, id: UUID) -> GeoLocationListInfo:
+    @get("/template/policy/list/localapp/{id}")
+    def get_lists_by_id(self, id: UUID) -> LocalAppListInfo:
         ...
 
-    @get("/template/policy/list/geolocation", "data")
-    def get_policy_lists(self) -> DataSequence[GeoLocationListInfo]:
+    @get("/template/policy/list/localapp", "data")
+    def get_policy_lists(self) -> DataSequence[LocalAppListInfo]:
         ...
 
-    @get("/template/policy/list/geolocation/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[GeoLocationListInfo]:
+    @get("/template/policy/list/localapp/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[LocalAppListInfo]:
         ...
 
-    @post("/template/policy/list/geolocation/preview")
-    def preview_policy_list(self, payload: GeoLocationList) -> PolicyListPreview:
+    @post("/template/policy/list/localapp/preview")
+    def preview_policy_list(self, payload: LocalAppList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/geolocation/preview/{id}")
+    @get("/template/policy/list/localapp/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/ips_signature.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/ips_signature.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.ips_signature import (
-    IPSSignatureList,
-    IPSSignatureListEditPayload,
-    IPSSignatureListInfo,
+from catalystwan.models.policy.lists import IPSSignatureList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
 )
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
+class IPSSignatureListEditPayload(IPSSignatureList, PolicyListId):
+    pass
+
+
+class IPSSignatureListInfo(IPSSignatureList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyIPSSignatureList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/ipssignature")
     def create_policy_list(self, payload: IPSSignatureList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/ipssignature/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/site.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,65 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.ipv6_prefix import IPv6PrefixList, IPv6PrefixListEditPayload, IPv6PrefixListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import SiteList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyIPv6PrefixList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/ipv6prefix")
-    def create_policy_list(self, payload: IPv6PrefixList) -> PolicyListId:
+class SiteListEditPayload(SiteList, PolicyListId):
+    pass
+
+
+class SiteListInfo(SiteList, PolicyListInfo):
+    pass
+
+
+class ConfigurationPolicySiteList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/site/defaultsite")
+    def create_default_site_list(self, payload: SiteList) -> PolicyListId:
+        ...
+
+    @post("/template/policy/list/site")
+    def create_policy_list(self, payload: SiteList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/ipv6prefix/{id}")
+    @delete("/template/policy/list/site/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/ipv6prefix")
+    @delete("/template/policy/list/site")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/ipv6prefix/{id}")
-    def edit_policy_list(self, id: UUID, payload: IPv6PrefixListEditPayload) -> None:
+    @put("/template/policy/list/site/{id}")
+    def edit_policy_list(self, id: UUID, payload: SiteListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/ipv6prefix/{id}")
-    def get_lists_by_id(self, id: UUID) -> IPv6PrefixListInfo:
+    @get("/template/policy/list/site/{id}")
+    def get_lists_by_id(self, id: UUID) -> SiteListInfo:
         ...
 
-    @get("/template/policy/list/ipv6prefix", "data")
-    def get_policy_lists(self) -> DataSequence[IPv6PrefixListInfo]:
+    @get("/template/policy/list/site", "data")
+    def get_policy_lists(self) -> DataSequence[SiteListInfo]:
         ...
 
-    @get("/template/policy/list/ipv6prefix/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[IPv6PrefixListInfo]:
+    @get("/template/policy/list/site/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SiteListInfo]:
         ...
 
-    @post("/template/policy/list/ipv6prefix/preview")
-    def preview_policy_list(self, payload: IPv6PrefixList) -> PolicyListPreview:
+    @post("/template/policy/list/site/preview")
+    def preview_policy_list(self, payload: SiteList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/ipv6prefix/preview/{id}")
+    @get("/template/policy/list/site/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/local_app.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/local_domain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.local_app import LocalAppList, LocalAppListEditPayload, LocalAppListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import LocalDomainList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyLocalAppList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/localapp")
-    def create_policy_list(self, payload: LocalAppList) -> PolicyListId:
+class LocalDomainListEditPayload(LocalDomainList, PolicyListId):
+    pass
+
+
+class LocalDomainListInfo(LocalDomainList, PolicyListInfo):
+    pass
+
+
+class ConfigurationPolicyLocalDomainList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/localdomain")
+    def create_policy_list(self, payload: LocalDomainList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/localapp/{id}")
+    @delete("/template/policy/list/localdomain/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/localapp")
+    @delete("/template/policy/list/localdomain")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/localapp/{id}")
-    def edit_policy_list(self, id: UUID, payload: LocalAppListEditPayload) -> None:
+    @put("/template/policy/list/localdomain/{id}")
+    def edit_policy_list(self, id: UUID, payload: LocalDomainListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/localapp/{id}")
-    def get_lists_by_id(self, id: UUID) -> LocalAppListInfo:
+    @get("/template/policy/list/localdomain/{id}")
+    def get_lists_by_id(self, id: UUID) -> LocalDomainListInfo:
         ...
 
-    @get("/template/policy/list/localapp", "data")
-    def get_policy_lists(self) -> DataSequence[LocalAppListInfo]:
+    @get("/template/policy/list/localdomain", "data")
+    def get_policy_lists(self) -> DataSequence[LocalDomainListInfo]:
         ...
 
-    @get("/template/policy/list/localapp/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[LocalAppListInfo]:
+    @get("/template/policy/list/localdomain/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[LocalDomainListInfo]:
         ...
 
-    @post("/template/policy/list/localapp/preview")
-    def preview_policy_list(self, payload: LocalAppList) -> PolicyListPreview:
+    @post("/template/policy/list/localdomain/preview")
+    def preview_policy_list(self, payload: LocalDomainList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/localapp/preview/{id}")
+    @get("/template/policy/list/localdomain/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/local_domain.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.local_domain import LocalDomainList, LocalDomainListEditPayload, LocalDomainListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import AppList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyLocalDomainList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/localdomain")
-    def create_policy_list(self, payload: LocalDomainList) -> PolicyListId:
+class AppListEditPayload(AppList, PolicyListId):
+    pass
+
+
+class AppListInfo(AppList, PolicyListInfo):
+    pass
+
+
+class ConfigurationPolicyApplicationList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/app")
+    def create_policy_list(self, payload: AppList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/localdomain/{id}")
+    @delete("/template/policy/list/app/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/localdomain")
+    @delete("/template/policy/list/app")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/localdomain/{id}")
-    def edit_policy_list(self, id: UUID, payload: LocalDomainListEditPayload) -> None:
+    @put("/template/policy/list/app/{id}")
+    def edit_policy_list(self, id: UUID, payload: AppListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/localdomain/{id}")
-    def get_lists_by_id(self, id: UUID) -> LocalDomainListInfo:
+    @get("/template/policy/list/app/{id}")
+    def get_lists_by_id(self, id: UUID) -> AppListInfo:
         ...
 
-    @get("/template/policy/list/localdomain", "data")
-    def get_policy_lists(self) -> DataSequence[LocalDomainListInfo]:
+    @get("/template/policy/list/app", "data")
+    def get_policy_lists(self) -> DataSequence[AppListInfo]:
         ...
 
-    @get("/template/policy/list/localdomain/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[LocalDomainListInfo]:
+    @get("/template/policy/list/app/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[AppListInfo]:
         ...
 
-    @post("/template/policy/list/localdomain/preview")
-    def preview_policy_list(self, payload: LocalDomainList) -> PolicyListPreview:
+    @post("/template/policy/list/app/preview")
+    def preview_policy_list(self, payload: AppList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/localdomain/preview/{id}")
+    @get("/template/policy/list/app/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/mirror.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/mirror.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.mirror import MirrorList, MirrorListEditPayload, MirrorListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import MirrorList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
+class MirrorListEditPayload(MirrorList, PolicyListId):
+    pass
+
+
+class MirrorListInfo(MirrorList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyMirrorList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/mirror")
     def create_policy_list(self, payload: MirrorList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/mirror/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/policer.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/policer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.policer import PolicerList, PolicerListEditPayload, PolicerListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import PolicerList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
+class PolicerListEditPayload(PolicerList, PolicyListId):
+    pass
+
+
+class PolicerListInfo(PolicerList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyPolicerClassList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/policer")
     def create_policy_list(self, payload: PolicerList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/policer/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/port.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/port.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.port import PortList, PortListEditPayload, PortListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import PortList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
+class PortListEditPayload(PortList, PolicyListId):
+    pass
+
+
+class PortListInfo(PortList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyPortList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/port")
     def create_policy_list(self, payload: PortList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/port/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.preferred_color_group import (
-    PreferredColorGroupList,
-    PreferredColorGroupListEditPayload,
-    PreferredColorGroupListInfo,
+from catalystwan.models.policy.lists import PreferredColorGroupList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
 )
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
+class PreferredColorGroupListEditPayload(PreferredColorGroupList, PolicyListId):
+    pass
+
+
+class PreferredColorGroupListInfo(PreferredColorGroupList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPreferredColorGroupList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/preferredcolorgroup")
     def create_policy_list(self, payload: PreferredColorGroupList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/preferredcolorgroup/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/prefix.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/vpn.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,63 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
+
+
 from uuid import UUID
 
-from catalystwan.api.templates.models.cisco_vpn_model import PrefixList
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.prefix import PrefixListEditPayload, PrefixListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import VPNList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyPrefixList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/prefix")
-    def create_policy_list(self, payload: PrefixList) -> PolicyListId:
+class VPNListEditPayload(VPNList, PolicyListId):
+    pass
+
+
+class VPNListInfo(VPNList, PolicyListInfo):
+    pass
+
+
+class ConfigurationPolicyVPNList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/vpn")
+    def create_policy_list(self, payload: VPNList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/prefix/{id}")
+    @delete("/template/policy/list/vpn/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/prefix")
+    @delete("/template/policy/list/vpn")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/prefix/{id}")
-    def edit_policy_list(self, id: UUID, payload: PrefixListEditPayload) -> None:
+    @put("/template/policy/list/vpn/{id}")
+    def edit_policy_list(self, id: UUID, payload: VPNListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/prefix/{id}")
-    def get_lists_by_id(self, id: UUID) -> PrefixListInfo:
+    @get("/template/policy/list/vpn/{id}")
+    def get_lists_by_id(self, id: UUID) -> VPNListInfo:
         ...
 
-    @get("/template/policy/list/prefix", "data")
-    def get_policy_lists(self) -> DataSequence[PrefixListInfo]:
+    @get("/template/policy/list/vpn", "data")
+    def get_policy_lists(self) -> DataSequence[VPNListInfo]:
         ...
 
-    @get("/template/policy/list/prefix/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[PrefixListInfo]:
+    @get("/template/policy/list/vpn/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[VPNListInfo]:
         ...
 
-    @post("/template/policy/list/prefix/preview")
-    def preview_policy_list(self, payload: PrefixList) -> PolicyListPreview:
+    @post("/template/policy/list/vpn/preview")
+    def preview_policy_list(self, payload: VPNList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/prefix/preview/{id}")
+    @get("/template/policy/list/vpn/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/protocol_name.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/protocol_name.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.protocol_name import (
-    ProtocolNameList,
-    ProtocolNameListEditPayload,
-    ProtocolNameListInfo,
+from catalystwan.models.policy.lists import ProtocolNameList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
 )
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
+class ProtocolNameListEditPayload(ProtocolNameList, PolicyListId):
+    pass
+
+
+class ProtocolNameListInfo(ProtocolNameList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyProtocolNameList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/protocolname")
     def create_policy_list(self, payload: ProtocolNameList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/protocolname/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/region.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/region.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.list.region import RegionList, RegionListEditPayload, RegionListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import RegionList
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListInfo, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
+class RegionListEditPayload(RegionList, PolicyListId):
+    pass
+
+
+class RegionListInfo(RegionList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyRegionList(APIEndpoints):
     @post("/template/policy/list/region")
     def create_policy_list(self, payload: RegionList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/region/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/site.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/sla.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.site import SiteList, SiteListEditPayload, SiteListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import SLAClassList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicySiteList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/site/defaultsite")
-    def create_default_site_list(self, payload: SiteList) -> PolicyListId:
-        ...
+class SLAClassListEditPayload(SLAClassList, PolicyListId):
+    pass
+
+
+class SLAClassListInfo(SLAClassList, PolicyListInfo):
+    pass
+
 
-    @post("/template/policy/list/site")
-    def create_policy_list(self, payload: SiteList) -> PolicyListId:
+class ConfigurationPolicySLAClassList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/sla")
+    def create_policy_list(self, payload: SLAClassList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/site/{id}")
+    @delete("/template/policy/list/sla/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/site")
+    @delete("/template/policy/list/sla")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/site/{id}")
-    def edit_policy_list(self, id: UUID, payload: SiteListEditPayload) -> None:
+    @put("/template/policy/list/sla/{id}")
+    def edit_policy_list(self, id: UUID, payload: SLAClassListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/site/{id}")
-    def get_lists_by_id(self, id: UUID) -> SiteListInfo:
+    @get("/template/policy/list/sla/{id}")
+    def get_lists_by_id(self, id: UUID) -> SLAClassListInfo:
         ...
 
-    @get("/template/policy/list/site", "data")
-    def get_policy_lists(self) -> DataSequence[SiteListInfo]:
+    @get("/template/policy/list/sla", "data")
+    def get_policy_lists(self) -> DataSequence[SLAClassListInfo]:
         ...
 
-    @get("/template/policy/list/site/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SiteListInfo]:
+    @get("/template/policy/list/sla/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SLAClassListInfo]:
         ...
 
-    @post("/template/policy/list/site/preview")
-    def preview_policy_list(self, payload: SiteList) -> PolicyListPreview:
+    @post("/template/policy/list/sla/preview")
+    def preview_policy_list(self, payload: SLAClassList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/site/preview/{id}")
+    @get("/template/policy/list/sla/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/sla.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/tloc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.sla import SLAClassList, SLAClassListEditPayload, SLAClassListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import TLOCList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicySLAClassList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/sla")
-    def create_policy_list(self, payload: SLAClassList) -> PolicyListId:
+class TLOCListEditPayload(TLOCList, PolicyListId):
+    pass
+
+
+class TLOCListInfo(TLOCList, PolicyListInfo):
+    pass
+
+
+class ConfigurationPolicyTLOCList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/tloc")
+    def create_policy_list(self, payload: TLOCList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/sla/{id}")
+    @delete("/template/policy/list/tloc/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/sla")
+    @delete("/template/policy/list/tloc")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/sla/{id}")
-    def edit_policy_list(self, id: UUID, payload: SLAClassListEditPayload) -> None:
+    @put("/template/policy/list/tloc/{id}")
+    def edit_policy_list(self, id: UUID, payload: TLOCListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/sla/{id}")
-    def get_lists_by_id(self, id: UUID) -> SLAClassListInfo:
+    @get("/template/policy/list/tloc/{id}")
+    def get_lists_by_id(self, id: UUID) -> TLOCListInfo:
         ...
 
-    @get("/template/policy/list/sla", "data")
-    def get_policy_lists(self) -> DataSequence[SLAClassListInfo]:
+    @get("/template/policy/list/tloc", "data")
+    def get_policy_lists(self) -> DataSequence[TLOCListInfo]:
         ...
 
-    @get("/template/policy/list/sla/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SLAClassListInfo]:
+    @get("/template/policy/list/tloc/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[TLOCListInfo]:
         ...
 
-    @post("/template/policy/list/sla/preview")
-    def preview_policy_list(self, payload: SLAClassList) -> PolicyListPreview:
+    @post("/template/policy/list/tloc/preview")
+    def preview_policy_list(self, payload: TLOCList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/sla/preview/{id}")
+    @get("/template/policy/list/tloc/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/tloc.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.tloc import TLOCList, TLOCListEditPayload, TLOCListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import IPv6PrefixList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyTLOCList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/tloc")
-    def create_policy_list(self, payload: TLOCList) -> PolicyListId:
+class IPv6PrefixListEditPayload(IPv6PrefixList, PolicyListId):
+    pass
+
+
+class IPv6PrefixListInfo(IPv6PrefixList, PolicyListInfo):
+    pass
+
+
+class ConfigurationPolicyIPv6PrefixList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/ipv6prefix")
+    def create_policy_list(self, payload: IPv6PrefixList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/tloc/{id}")
+    @delete("/template/policy/list/ipv6prefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/tloc")
+    @delete("/template/policy/list/ipv6prefix")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/tloc/{id}")
-    def edit_policy_list(self, id: UUID, payload: TLOCListEditPayload) -> None:
+    @put("/template/policy/list/ipv6prefix/{id}")
+    def edit_policy_list(self, id: UUID, payload: IPv6PrefixListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/tloc/{id}")
-    def get_lists_by_id(self, id: UUID) -> TLOCListInfo:
+    @get("/template/policy/list/ipv6prefix/{id}")
+    def get_lists_by_id(self, id: UUID) -> IPv6PrefixListInfo:
         ...
 
-    @get("/template/policy/list/tloc", "data")
-    def get_policy_lists(self) -> DataSequence[TLOCListInfo]:
+    @get("/template/policy/list/ipv6prefix", "data")
+    def get_policy_lists(self) -> DataSequence[IPv6PrefixListInfo]:
         ...
 
-    @get("/template/policy/list/tloc/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[TLOCListInfo]:
+    @get("/template/policy/list/ipv6prefix/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[IPv6PrefixListInfo]:
         ...
 
-    @post("/template/policy/list/tloc/preview")
-    def preview_policy_list(self, payload: TLOCList) -> PolicyListPreview:
+    @post("/template/policy/list/ipv6prefix/preview")
+    def preview_policy_list(self, payload: IPv6PrefixList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/tloc/preview/{id}")
+    @get("/template/policy/list/ipv6prefix/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/url_allow_list.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.url import URLAllowList, URLAllowListEditPayload, URLAllowListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import URLAllowList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
+class URLAllowListEditPayload(URLAllowList, PolicyListId):
+    pass
+
+
+class URLAllowListInfo(URLAllowList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyURLAllowList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/urlwhitelist")
     def create_policy_list(self, payload: URLAllowList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/urlwhitelist/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/url_block_list.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/url_block_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.url import URLBlockList, URLBlockListEditPayload, URLBlockListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import URLBlockList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
+class URLBlockListEditPayload(URLBlockList, PolicyListId):
+    pass
+
+
+class URLBlockListInfo(URLBlockList, PolicyListInfo):
+    pass
+
+
 class ConfigurationPolicyURLBlockList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/urlblacklist")
     def create_policy_list(self, payload: URLBlockList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/urlblacklist/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/vpn.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/data_prefix.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,61 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
-
-
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.vpn import VPNList, VPNListEditPayload, VPNListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import DataPrefixList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyVPNList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/vpn")
-    def create_policy_list(self, payload: VPNList) -> PolicyListId:
+class DataPrefixListEditPayload(DataPrefixList, PolicyListId):
+    pass
+
+
+class DataPrefixListInfo(DataPrefixList, PolicyListInfo):
+    pass
+
+
+class ConfigurationPolicyDataPrefixList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/dataprefix")
+    def create_policy_list(self, payload: DataPrefixList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/vpn/{id}")
+    @delete("/template/policy/list/dataprefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/vpn")
+    @delete("/template/policy/list/dataprefix")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/vpn/{id}")
-    def edit_policy_list(self, id: UUID, payload: VPNListEditPayload) -> None:
+    @put("/template/policy/list/dataprefix/{id}")
+    def edit_policy_list(self, id: UUID, payload: DataPrefixListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/vpn/{id}")
-    def get_lists_by_id(self, id: UUID) -> VPNListInfo:
+    @get("/template/policy/list/dataprefix/{id}")
+    def get_lists_by_id(self, id: UUID) -> DataPrefixListInfo:
         ...
 
-    @get("/template/policy/list/vpn", "data")
-    def get_policy_lists(self) -> DataSequence[VPNListInfo]:
+    @get("/template/policy/list/dataprefix", "data")
+    def get_policy_lists(self) -> DataSequence[DataPrefixListInfo]:
         ...
 
-    @get("/template/policy/list/vpn/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[VPNListInfo]:
+    @get("/template/policy/list/dataprefix/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[DataPrefixListInfo]:
         ...
 
-    @post("/template/policy/list/vpn/preview")
-    def preview_policy_list(self, payload: VPNList) -> PolicyListPreview:
+    @post("/template/policy/list/dataprefix/preview")
+    def preview_policy_list(self, payload: DataPrefixList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/vpn/preview/{id}")
+    @get("/template/policy/list/dataprefix/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/list/zone.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/geo_location.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
-from catalystwan.models.policy.list.zone import ZoneList, ZoneListEditPayload, ZoneListInfo
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
+from catalystwan.models.policy.lists import GeoLocationList
+from catalystwan.models.policy.policy_list import (
+    InfoTag,
+    PolicyListEndpoints,
+    PolicyListId,
+    PolicyListInfo,
+    PolicyListPreview,
+)
 from catalystwan.typed_list import DataSequence
 
 
-class ConfigurationPolicyZoneList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/zone")
-    def create_policy_list(self, payload: ZoneList) -> PolicyListId:
+class GeoLocationListEditPayload(GeoLocationList, PolicyListId):
+    pass
+
+
+class GeoLocationListInfo(GeoLocationList, PolicyListInfo):
+    pass
+
+
+class ConfigurationPolicyGeoLocationList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/geolocation")
+    def create_policy_list(self, payload: GeoLocationList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/zone/{id}")
+    @delete("/template/policy/list/geolocation/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/zone")
+    @delete("/template/policy/list/geolocation")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/zone/{id}")
-    def edit_policy_list(self, id: UUID, payload: ZoneListEditPayload) -> None:
+    @put("/template/policy/list/geolocation/{id}")
+    def edit_policy_list(self, id: UUID, payload: GeoLocationListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/zone/{id}")
-    def get_lists_by_id(self, id: UUID) -> ZoneListInfo:
+    @get("/template/policy/list/geolocation/{id}")
+    def get_lists_by_id(self, id: UUID) -> GeoLocationListInfo:
         ...
 
-    @get("/template/policy/list/zone", "data")
-    def get_policy_lists(self) -> DataSequence[ZoneListInfo]:
+    @get("/template/policy/list/geolocation", "data")
+    def get_policy_lists(self) -> DataSequence[GeoLocationListInfo]:
         ...
 
-    @get("/template/policy/list/zone/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[ZoneListInfo]:
+    @get("/template/policy/list/geolocation/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[GeoLocationListInfo]:
         ...
 
-    @post("/template/policy/list/zone/preview")
-    def preview_policy_list(self, payload: ZoneList) -> PolicyListPreview:
+    @post("/template/policy/list/geolocation/preview")
+    def preview_policy_list(self, payload: GeoLocationList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/zone/preview/{id}")
+    @get("/template/policy/list/geolocation/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/vedge_template.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/vedge_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/policy/vsmart_template.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/vsmart_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration/software_actions.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration/software_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_dashboard_status.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration_dashboard_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_device_actions.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration_device_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_device_inventory.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration_device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_device_template.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration_device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_feature_profile.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration_feature_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_group.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from datetime import datetime
 from typing import List, Optional
-from uuid import UUID
 
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.common import Solution
 from catalystwan.models.configuration.feature_profile.common import ProfileType
 from catalystwan.typed_list import DataSequence
 
 
 class ProfileId(BaseModel):
-    id: UUID
+    id: str
 
 
 # TODO Get mode from schema
 class ConfigGroupCreationPayload(BaseModel):
     name: str
     description: str
     solution: Solution
@@ -34,32 +33,18 @@
     created_by: str = Field(alias="createdBy")
     last_updated_by: str = Field(alias="lastUpdatedBy")
     created_on: datetime = Field(alias="createdOn")
     last_updated_on: datetime = Field(alias="lastUpdatedOn")
 
 
 class ConfigGroup(BaseModel):
-    id: UUID
     name: str
     description: Optional[str]
     solution: Solution
     profiles: Optional[List[FeatureProfile]]
-    source: Optional[str] = None
-    state: Optional[str] = None
-    devices: List = Field(default=[])
-    created_by: Optional[str] = Field(alias="createdBy")
-    last_updated_by: Optional[str] = Field(alias="lastUpdatedBy")
-    created_on: Optional[datetime] = Field(alias="createdOn")
-    last_updated_on: Optional[datetime] = Field(alias="lastUpdatedOn")
-    version: int
-    number_of_devices: int = Field(alias="numberOfDevices")
-    number_of_devices_up_to_date: int = Field(alias="numberOfDevicesUpToDate")
-    origin: Optional[str]
-    topology: Optional[str] = None
-    full_config_cli: bool = Field(alias="fullConfigCli")
 
 
 class ConfigGroupResponsePayload(BaseModel):
     config_groups: List[ConfigGroup]
 
 
 class ConfigGroupEditPayload(BaseModel):
@@ -117,15 +102,15 @@
 
 
 class ConfigGroupDisassociateResponse(BaseModel):
     parentTaskId: str
 
 
 class ConfigGroupCreationResponse(BaseModel):
-    id: UUID
+    id: str
 
 
 class EditedProfileId(BaseModel):
     profileId: str
 
 
 class ConfigGroupEditResponse(BaseModel):
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/configuration_settings.py` & `catalystwan-0.32.0/catalystwan/endpoints/configuration_settings.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/endpoints_container.py` & `catalystwan-0.32.0/catalystwan/endpoints/endpoints_container.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/misc.py` & `catalystwan-0.32.0/catalystwan/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/monitoring_device_details.py` & `catalystwan-0.32.0/catalystwan/endpoints/monitoring_device_details.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/monitoring_status.py` & `catalystwan-0.32.0/catalystwan/endpoints/monitoring_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/real_time_monitoring/reboot_history.py` & `catalystwan-0.32.0/catalystwan/endpoints/real_time_monitoring/reboot_history.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/sdavc_cloud_connector.py` & `catalystwan-0.32.0/catalystwan/endpoints/sdavc_cloud_connector.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/tenant_backup_restore.py` & `catalystwan-0.32.0/catalystwan/endpoints/tenant_backup_restore.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/tenant_management.py` & `catalystwan-0.32.0/catalystwan/endpoints/tenant_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/tenant_migration.py` & `catalystwan-0.32.0/catalystwan/endpoints/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py` & `catalystwan-0.32.0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/exceptions.py` & `catalystwan-0.32.0/catalystwan/exceptions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/integration_tests/test_find_template_values.py` & `catalystwan-0.32.0/catalystwan/integration_tests/test_find_template_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
+
 import json
 import os
 import unittest
 from typing import Any, List, cast
 
 from catalystwan.session import create_manager_session
 from catalystwan.utils.feature_template.find_template_values import find_template_values
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/logging.conf` & `catalystwan-0.32.0/catalystwan/logging.conf`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/config_migration.py` & `catalystwan-0.32.0/catalystwan/models/policy/security.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,152 +1,190 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
-from typing import Any, Dict, List, Set, Tuple, Union
+from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field, model_validator
+from pydantic import BaseModel, ConfigDict, Field, IPvAnyAddress, RootModel, field_validator
 from typing_extensions import Annotated
 
-from catalystwan.api.template_api import FeatureTemplateInformation, TemplateInformation
-from catalystwan.api.templates.device_template.device_template import DeviceTemplate
-from catalystwan.endpoints.configuration_group import ConfigGroupCreationPayload
-from catalystwan.models.configuration.feature_profile.common import FeatureProfileCreationPayload, ProfileType
-from catalystwan.models.configuration.feature_profile.sdwan.other import AnyOtherParcel
-from catalystwan.models.configuration.feature_profile.sdwan.policy_object import AnyPolicyObjectParcel
-from catalystwan.models.configuration.feature_profile.sdwan.service import AnyServiceParcel
-from catalystwan.models.configuration.feature_profile.sdwan.system import AnySystemParcel
-from catalystwan.models.configuration.feature_profile.sdwan.transport import AnyTransportParcel
-from catalystwan.models.configuration.topology_group import TopologyGroup
-from catalystwan.models.policy import AnyPolicyDefinitionInfo, AnyPolicyListInfo
-from catalystwan.models.policy.centralized import CentralizedPolicyInfo
-from catalystwan.models.policy.localized import LocalizedPolicyInfo
-from catalystwan.models.policy.security import AnySecurityPolicyInfo
-
-AnyParcel = Annotated[
-    Union[AnySystemParcel, AnyPolicyObjectParcel, AnyServiceParcel, AnyOtherParcel, AnyTransportParcel],
-    Field(discriminator="type_"),
+from catalystwan.models.policy.policy import (
+    AdvancedMalwareProtectionAssemblyItem,
+    DNSSecurityAssemblyItem,
+    IntrusionPreventionAssemblyItem,
+    NGFirewallAssemblyItem,
+    PolicyCreationPayload,
+    PolicyDefinition,
+    PolicyInfo,
+    SSLDecryptionAssemblyItem,
+    URLFilteringAssemblyItem,
+    ZoneBasedFWAssemblyItem,
+)
+
+SecurityPolicyAssemblyItem = Annotated[
+    Union[
+        ZoneBasedFWAssemblyItem,
+        IntrusionPreventionAssemblyItem,
+        URLFilteringAssemblyItem,
+        AdvancedMalwareProtectionAssemblyItem,
+        DNSSecurityAssemblyItem,
+        SSLDecryptionAssemblyItem,
+    ],
+    Field(discriminator="type"),
+]
+
+UnifiedSecurityPolicyAssemblyItem = Annotated[
+    Union[
+        NGFirewallAssemblyItem,
+        DNSSecurityAssemblyItem,
+    ],
+    Field(discriminator="type"),
+]
+
+FailureMode = Literal[
+    "open",
+    "close",
+]
+
+ZoneToNoZoneInternet = Literal[
+    "allow",
+    "deny",
 ]
 
 
-class DeviceTemplateWithInfo(DeviceTemplate):
+class HighSpeedLoggingEntry(BaseModel):
+    vrf: str
+    server_ip: IPvAnyAddress = Field(alias="serverIp")
+    port: str
+    source_interface: Optional[str] = Field(alias="sourceInterface")
     model_config = ConfigDict(populate_by_name=True)
-    template_id: str = Field(serialization_alias="templateId", validation_alias="templateId")
-    factory_default: bool = Field(serialization_alias="factoryDefault", validation_alias="factoryDefault")
-    devices_attached: int = Field(serialization_alias="devicesAttached", validation_alias="devicesAttached")
-
-    @staticmethod
-    def from_merged(template: DeviceTemplate, info: TemplateInformation) -> "DeviceTemplateWithInfo":
-        info_dict = template.model_dump()
-        return DeviceTemplateWithInfo(
-            template_id=info.id,
-            factory_default=info.factory_default,
-            devices_attached=info.devices_attached,
-            **info_dict
-        )
 
 
-class UX1Policies(BaseModel):
+class HighSpeedLoggingList(BaseModel):
+    entries: List[HighSpeedLoggingEntry]
+
+
+class LoggingEntry(BaseModel):
+    vpn: str
+    server_ip: IPvAnyAddress = Field(alias="serverIP")
     model_config = ConfigDict(populate_by_name=True)
-    centralized_policies: List[CentralizedPolicyInfo] = Field(
-        default=[], serialization_alias="centralizedPolicies", validation_alias="centralizedPolicies"
-    )
-    localized_policies: List[LocalizedPolicyInfo] = Field(
-        default=[], serialization_alias="localizedPolicies", validation_alias="localizedPolicies"
-    )
-    security_policies: List[AnySecurityPolicyInfo] = Field(
-        default=[], serialization_alias="securityPolicies", validation_alias="securityPolicies"
-    )
-    policy_definitions: List[AnyPolicyDefinitionInfo] = Field(
-        default=[], serialization_alias="policyDefinitions", validation_alias="policyDefinitions"
-    )
-    policy_lists: List[AnyPolicyListInfo] = Field(
-        default=[], serialization_alias="policyLists", validation_alias="policyLists"
-    )
 
 
-class UX1Templates(BaseModel):
-    feature_templates: List[FeatureTemplateInformation] = Field(
-        default=[], serialization_alias="featureTemplates", validation_alias="featureTemplates"
-    )
-    device_templates: List[DeviceTemplateWithInfo] = Field(
-        default=[], serialization_alias="deviceTemplates", validation_alias="deviceTemplates"
-    )
+class SecurityPolicySettings(BaseModel):
+    logging: Optional[List[LoggingEntry]] = None
+    failure_mode: Optional[FailureMode] = Field(default=None, alias="failureMode")
+    zone_to_no_zone_internet: ZoneToNoZoneInternet = Field(default="deny", alias="zoneToNozoneInternet")
+    tcp_syn_flood_limit: Optional[str] = Field(default=None, alias="tcpSynFloodLimit")
+    high_speed_logging: Optional[HighSpeedLoggingEntry] = Field(default=None, alias="highSpeedLogging")
+    audit_trail: Optional[str] = Field(default=None, alias="auditTrail")
+    platform_match: Optional[str] = Field(default=None, alias="platformMatch")
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class UX1Config(BaseModel):
-    # All UX1 Configuration items - Mega Model
-    policies: UX1Policies = UX1Policies()
-    templates: UX1Templates = UX1Templates()
+class UnifiedSecurityPolicySettings(BaseModel):
+    tcp_syn_flood_limit: Optional[str] = Field(default=None, alias="tcpSynFloodLimit")
+    max_incomplete_tcp_limit: Optional[str] = Field(default=None, alias="maxIncompleteTcpLimit")
+    max_incomplete_udp_limit: Optional[str] = Field(default=None, alias="maxIncompleteUdpLimit")
+    max_incomplete_icmp_limit: Optional[str] = Field(default=None, alias="maxIncompleteIcmpLimit")
+    high_speed_logging: Optional[HighSpeedLoggingList] = Field(default=None, alias="highSpeedLogging")
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class TransformHeader(BaseModel):
-    type: str = Field(
-        description="Needed to push item to specific endpoint."
-        "Type discriminator is not present in many UX2 item payloads"
-    )
-    origin: UUID = Field(description="Original UUID of converted item")
-    subelements: Set[UUID] = Field(default_factory=set)
+class SecurityPolicyDefinition(PolicyDefinition):
+    assembly: List[SecurityPolicyAssemblyItem] = []
+    settings: SecurityPolicySettings = SecurityPolicySettings()
 
 
-class TransformedTopologyGroup(BaseModel):
-    header: TransformHeader
-    topology_group: TopologyGroup
+class UnifiedSecurityPolicyDefinition(PolicyDefinition):
+    assembly: List[UnifiedSecurityPolicyAssemblyItem] = []
+    settings: UnifiedSecurityPolicySettings = UnifiedSecurityPolicySettings()
 
 
-class TransformedConfigGroup(BaseModel):
-    header: TransformHeader
-    config_group: ConfigGroupCreationPayload
+class SecurityPolicy(PolicyCreationPayload):
+    policy_mode: Literal["security"] = Field(default="security", alias="policyMode")
+    policy_type: str = Field(default="feature", alias="policyType")
+    policy_use_case: str = Field(default="custom", alias="policyUseCase")
+    policy_definition: SecurityPolicyDefinition = Field(default=SecurityPolicyDefinition(), alias="policyDefinition")
 
+    def add_item(self, item: SecurityPolicyAssemblyItem) -> None:
+        self.policy_definition.assembly.append(item)
 
-class TransformedFeatureProfile(BaseModel):
-    header: TransformHeader
-    feature_profile: FeatureProfileCreationPayload
+    def add_zone_based_fw(self, definition_id: UUID) -> None:
+        self.add_item(ZoneBasedFWAssemblyItem(definition_id=definition_id))
 
+    def add_dns_security(self, definition_id: UUID) -> None:
+        self.add_item(DNSSecurityAssemblyItem(definition_id=definition_id))
 
-class TransformedParcel(BaseModel):
-    header: TransformHeader
-    parcel: AnyParcel
+    def add_intrusion_prevention(self, definition_id: UUID) -> None:
+        self.add_item(IntrusionPreventionAssemblyItem(definition_id=definition_id))
 
+    def add_url_filtering(self, definition_id: UUID) -> None:
+        self.add_item(URLFilteringAssemblyItem(definition_id=definition_id))
 
-class UX2Config(BaseModel):
-    # All UX2 Configuration items - Mega Model
-    model_config = ConfigDict(populate_by_name=True)
-    topology_groups: List[TransformedTopologyGroup] = Field(
-        default=[], serialization_alias="topologyGroups", validation_alias="topologyGroups"
-    )
-    config_groups: List[TransformedConfigGroup] = Field(
-        default=[], serialization_alias="configurationGroups", validation_alias="configurationGroups"
-    )
-    policy_groups: List[TransformedConfigGroup] = Field(
-        default=[], serialization_alias="policyGroups", validation_alias="policyGroups"
-    )
-    feature_profiles: List[TransformedFeatureProfile] = Field(
-        default=[], serialization_alias="featureProfiles", validation_alias="featureProfiles"
-    )
-    profile_parcels: List[TransformedParcel] = Field(
-        default=[], serialization_alias="profileParcels", validation_alias="profileParcels"
-    )
+    def add_advanced_malware_protection(self, definition_id: UUID) -> None:
+        self.add_item(AdvancedMalwareProtectionAssemblyItem(definition_id=definition_id))
+
+    def add_ssl_decryption(self, definition_id: UUID) -> None:
+        self.add_item(SSLDecryptionAssemblyItem(definition_id=definition_id))
 
-    @model_validator(mode="before")
+    @field_validator("policy_definition", mode="before")
     @classmethod
-    def insert_parcel_type_from_headers(cls, values: Dict[str, Any]):
-        profile_parcels = values.get("profileParcels", [])
-        if not profile_parcels:
-            profile_parcels = values.get("profile_parcels", [])
-        for profile_parcel in profile_parcels:
-            profile_parcel["parcel"]["type_"] = profile_parcel["header"]["type"]
-        return values
+    def try_parse(cls, policy_definition):
+        if isinstance(policy_definition, str):
+            return SecurityPolicyDefinition.model_validate_json(policy_definition)
+        return policy_definition
 
 
-class UX2ConfigRollback(BaseModel):
-    config_group_ids: List[UUID] = Field(
-        default_factory=list, serialization_alias="ConfigGroupIds", validation_alias="ConfigGroupIds"
-    )
-    feature_profile_ids: List[Tuple[UUID, ProfileType]] = Field(
-        default_factory=list, serialization_alias="FeatureProfileIds", validation_alias="FeatureProfileIds"
+class UnifiedSecurityPolicy(PolicyCreationPayload):
+    policy_mode: Literal["unified"] = Field("unified", alias="policyMode")
+    policy_type: str = Field("feature", alias="policyType")
+    policy_use_case: str = Field("custom", alias="policyUseCase")
+    policy_definition: UnifiedSecurityPolicyDefinition = Field(
+        default=UnifiedSecurityPolicyDefinition(), alias="policyDefinition"
     )
 
-    def add_config_group(self, config_group_id: UUID) -> None:
-        self.config_group_ids.append(config_group_id)
+    def add_item(self, item: UnifiedSecurityPolicyAssemblyItem) -> None:
+        self.policy_definition.assembly.append(item)
+
+    def add_ng_firewall(self, definition_id: UUID) -> NGFirewallAssemblyItem:
+        ng_fw = NGFirewallAssemblyItem(definition_id=definition_id)
+        self.add_item(ng_fw)
+        return ng_fw
+
+    def add_dns_security(self, definition_id: UUID) -> None:
+        self.add_item(DNSSecurityAssemblyItem(definition_id=definition_id))
+
+    @field_validator("policy_definition", mode="before")
+    @classmethod
+    def try_parse(cls, policy_definition):
+        if isinstance(policy_definition, str):
+            return UnifiedSecurityPolicyDefinition.model_validate_json(policy_definition)
+        return policy_definition
+
+
+AnySecurityPolicy = Annotated[Union[SecurityPolicy, UnifiedSecurityPolicy], Field(discriminator="policy_mode")]
+
+
+class SecurityPolicyRoot(RootModel):
+    root: AnySecurityPolicy
+
+
+class SecurityPolicyEditResponse(BaseModel):
+    master_templates_affected: List[str] = Field(default=[], alias="masterTemplatesAffected")
+
+
+class SecurityPolicyInfo(SecurityPolicy, PolicyInfo):
+    virtual_application_templates: List[str] = Field(alias="virtualApplicationTemplates")
+    supported_devices: List[str] = Field(alias="supportedDevices")
+
+
+class UnifiedSecurityPolicyInfo(UnifiedSecurityPolicy, PolicyInfo):
+    virtual_application_templates: List[str] = Field(alias="virtualApplicationTemplates")
+    supported_devices: List[str] = Field(alias="supportedDevices")
+
+
+AnySecurityPolicyInfo = Annotated[
+    Union[SecurityPolicyInfo, UnifiedSecurityPolicyInfo], Field(discriminator="policy_mode")
+]
+
 
-    def add_feature_profile(self, feature_profile_id: UUID, profile_type: ProfileType) -> None:
-        self.feature_profile_ids.append((feature_profile_id, profile_type))
+class SecurityPolicyInfoRoot(RootModel):
+    root: AnySecurityPolicyInfo
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/README.md` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This README document provides guidelines on creating configuration groups within the `Cisco Catalyst WAN SDK` repository.
 
 ## How to create Parcel model
 
 Cellular controller Parcel will be used for example purposes. Please change the parcel according to which one you are implementing.
 
-1. Add new endpoints following the guide: https://github.com/CiscoDevNet/catalystwan/blob/main/CONTRIBUTING.md
+1. Add new endpoints following the guide: https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md
 2. Download a schema with new endpoint:
 ```python
     @versions(supported_versions=(">=20.9"), raises=False)
     @get("/v1/feature-profile/sdwan/transport/cellular-controller/schema", resp_json_key="request")
     def get_sdwan_transport_cellular_controller_parcel_schema(self, params: SchemaTypeQuery) -> JSON:
         ...
 ```
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/builder.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/builder.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/common.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     "transport",
     "system",
     "cli",
     "service",
     "application-priority",
     "policy-object",
     "embedded-security",
-    "other",
 ]
 
 SchemaType = Literal[
     "post",
     "put",
 ]
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Union
+from typing import List, Mapping, Union
 
 from pydantic import Field
 from typing_extensions import Annotated
 
 from .policy.app_probe import AppProbeMapItem, AppProbeParcel
 from .policy.application_list import ApplicationFamilyListEntry, ApplicationListEntry, ApplicationListParcel
 from .policy.color_list import ColorEntry, ColorParcel
 from .policy.data_prefix import DataPrefixEntry, DataPrefixParcel
 from .policy.expanded_community_list import ExpandedCommunityParcel
 from .policy.fowarding_class import FowardingClassParcel, FowardingClassQueueEntry
 from .policy.ipv6_data_prefix import IPv6DataPrefixEntry, IPv6DataPrefixParcel
 from .policy.ipv6_prefix_list import IPv6PrefixListEntry, IPv6PrefixListParcel
-from .policy.policer import PolicerEntry, PolicerParcel
+from .policy.policier import PolicierEntry, PolicierParcel
 from .policy.prefered_group_color import Preference, PreferredColorGroupEntry, PreferredColorGroupParcel
 from .policy.prefix_list import PrefixListEntry, PrefixListParcel
 from .policy.sla_class import FallbackBestTunnel, SLAAppProbeClass, SLAClassCriteria, SLAClassListEntry, SLAClassParcel
 from .policy.standard_community import StandardCommunityEntry, StandardCommunityParcel
 from .policy.tloc_list import TlocEntry, TlocParcel
 from .security.application_list import (
     SecurityApplicationFamilyListEntry,
@@ -27,47 +27,76 @@
 from .security.data_prefix import SecurityDataPrefixEntry, SecurityDataPrefixParcel
 from .security.fqdn import FQDNDomainParcel, FQDNListEntry
 from .security.geolocation_list import GeoLocationListEntry, GeoLocationListParcel
 from .security.ips_signature import IPSSignatureListEntry, IPSSignatureParcel
 from .security.local_domain import LocalDomainListEntry, LocalDomainParcel
 from .security.protocol_list import ProtocolListEntry, ProtocolListParcel
 from .security.security_port import SecurityPortListEntry, SecurityPortParcel
-from .security.url import BaseURLListEntry, URLAllowParcel, URLBlockParcel, URLParcel
+from .security.url import BaseURLListEntry, URLAllowParcel, URLBlockParcel
 from .security.zone import SecurityZoneListEntry, SecurityZoneListParcel
 
 AnyPolicyObjectParcel = Annotated[
     Union[
-        URLParcel,
-        ApplicationListParcel,
         AppProbeParcel,
+        ApplicationListParcel,
         ColorParcel,
         DataPrefixParcel,
         ExpandedCommunityParcel,
         FowardingClassParcel,
-        FQDNDomainParcel,
-        GeoLocationListParcel,
-        IPSSignatureParcel,
         IPv6DataPrefixParcel,
         IPv6PrefixListParcel,
-        LocalDomainParcel,
-        PolicerParcel,
-        PreferredColorGroupParcel,
         PrefixListParcel,
+        PolicierParcel,
+        PreferredColorGroupParcel,
+        SLAClassParcel,
+        TlocParcel,
+        StandardCommunityParcel,
+        LocalDomainParcel,
+        FQDNDomainParcel,
+        IPSSignatureParcel,
+        URLAllowParcel,
+        URLBlockParcel,
+        SecurityPortParcel,
         ProtocolListParcel,
+        GeoLocationListParcel,
+        SecurityZoneListParcel,
         SecurityApplicationListParcel,
         SecurityDataPrefixParcel,
-        SecurityPortParcel,
-        SecurityZoneListParcel,
-        SLAClassParcel,
-        StandardCommunityParcel,
-        TlocParcel,
     ],
-    Field(discriminator="type_"),
+    Field(discriminator="type"),
 ]
 
+POLICY_OBJECT_PAYLOAD_ENDPOINT_MAPPING: Mapping[type, str] = {
+    AppProbeParcel: "app-probe",
+    ApplicationListParcel: "app-list",
+    ColorParcel: "color",
+    DataPrefixParcel: "data-prefix",
+    ExpandedCommunityParcel: "expanded-community",
+    FowardingClassParcel: "class",
+    IPv6DataPrefixParcel: "data-ipv6-prefix",
+    IPv6PrefixListParcel: "ipv6-prefix",
+    PrefixListParcel: "prefix",
+    PolicierParcel: "policer",
+    PreferredColorGroupParcel: "preferred-color-group",
+    SLAClassParcel: "sla-class",
+    TlocParcel: "tloc",
+    StandardCommunityParcel: "standard-community",
+    LocalDomainParcel: "security-localdomain",
+    FQDNDomainParcel: "security-fqdn",
+    IPSSignatureParcel: "security-ipssignature",
+    URLAllowParcel: "security-urllist",
+    URLBlockParcel: "security-urllist",
+    SecurityPortParcel: "security-port",
+    ProtocolListParcel: "security-protocolname",
+    GeoLocationListParcel: "security-geolocation",
+    SecurityZoneListParcel: "security-zone",
+    SecurityApplicationListParcel: "security-localapp",
+    SecurityDataPrefixParcel: "security-data-ip-prefix",
+}
+
 __all__ = (
     "AnyPolicyObjectParcel",
     "ApplicationFamilyListEntry",
     "ApplicationListEntry",
     "ApplicationListParcel",
     "AppProbeEntry",
     "AppProbeMapItem",
@@ -89,16 +118,16 @@
     "IPSSignatureParcel",
     "IPv6DataPrefixEntry",
     "IPv6DataPrefixParcel",
     "IPv6PrefixListEntry",
     "IPv6PrefixListParcel",
     "LocalDomainListEntry",
     "LocalDomainParcel",
-    "PolicerEntry",
-    "PolicerParcel",
+    "PolicierEntry",
+    "PolicierParcel",
     "Preference",
     "PreferredColorGroupEntry",
     "PreferredColorGroupParcel",
     "PrefixListEntry",
     "PrefixListParcel",
     "ProtocolListEntry",
     "ProtocolListParcel",
@@ -115,15 +144,14 @@
     "SLAClassCriteria",
     "SLAClassListEntry",
     "SLAClassParcel",
     "StandardCommunityEntry",
     "StandardCommunityParcel",
     "TlocEntry",
     "TlocParcel",
-    "URLParcel",
     "URLAllowParcel",
     "URLBlockParcel",
 )
 
 
 def __dir__() -> "List[str]":
     return list(__all__)
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal
+from typing import List
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import TLOCColor
 
 
@@ -24,15 +24,14 @@
     map: List[AppProbeMapItem] = Field(default=[])
     forwarding_class_name: Global[str] = Field(
         serialization_alias="forwardingClass", validation_alias="forwardingClass"
     )
 
 
 class AppProbeParcel(_ParcelBase):
-    type_: Literal["app-probe"] = Field(default="app-probe", exclude=True)
     entries: List[AppProbeEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_fowarding_class(self, forwarding_class_name: str):
         self.entries.append(
             AppProbeEntry(
                 forwarding_class_name=as_global(forwarding_class_name),
             )
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal, Union
+from typing import List, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class ApplicationListEntry(BaseModel):
@@ -14,15 +14,14 @@
 
 class ApplicationFamilyListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     app_list_family: Global[str] = Field(serialization_alias="appFamily", validation_alias="appFamily")
 
 
 class ApplicationListParcel(_ParcelBase):
-    type_: Literal["app-list"] = Field(default="app-list", exclude=True)
     entries: List[Union[ApplicationListEntry, ApplicationFamilyListEntry]] = Field(
         default=[], validation_alias=AliasPath("data", "entries")
     )
 
     def add_application(self, application: str):
         self.entries.append(ApplicationListEntry(app_list=as_global(application)))
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Address, IPv4Network
-from typing import List, Literal
+from typing import List
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class DataPrefixEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     ipv4_address: Global[IPv4Address] = Field(serialization_alias="ipv4Address", validation_alias="ipv4Address")
     ipv4_prefix_length: Global[int] = Field(serialization_alias="ipv4PrefixLength", validation_alias="ipv4PrefixLength")
 
-    @staticmethod
-    def from_ipv4_network(ipv4_network: IPv4Network) -> "DataPrefixEntry":
-        return DataPrefixEntry(
-            ipv4_address=as_global(ipv4_network.network_address),
-            ipv4_prefix_length=as_global(ipv4_network.prefixlen),
-        )
-
 
 class DataPrefixParcel(_ParcelBase):
-    type_: Literal["data-prefix"] = Field(default="data-prefix", exclude=True)
     entries: List[DataPrefixEntry] = Field(default_factory=list, validation_alias=AliasPath("data", "entries"))
 
     def add_data_prefix(self, ipv4_network: IPv4Network):
-        self.entries.append(DataPrefixEntry.from_ipv4_network(ipv4_network))
+        self.entries.append(
+            DataPrefixEntry(
+                ipv4_address=as_global(ipv4_network.network_address),
+                ipv4_prefix_length=as_global(ipv4_network.prefixlen),
+            )
+        )
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import Literal
-
 from pydantic import AliasPath, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class ExpandedCommunityParcel(_ParcelBase):
-    type_: Literal["expanded-community"] = Field(default="expanded-community", exclude=True)
     model_config = ConfigDict(populate_by_name=True)
-    expanded_community_list: Global[list] = Field(
+    expandedCommunityList: Global[list] = Field(
         default=as_global([]),
         serialization_alias="expandedCommunityList",
         validation_alias=AliasPath("data", "expandedCommunityList"),
     )
 
     def add_community(self, expanded_community: str):
-        self.expanded_community_list.value.append(expanded_community)
+        self.expandedCommunityList.value.append(expanded_community)
 
-    @field_validator("expanded_community_list")
+    @field_validator("expandedCommunityList")
     @classmethod
-    def check_list_str(cls, expanded_community_list: Global):
+    def check_rate(cls, expanded_community_list: Global):
         assert all([isinstance(ec, str) for ec in expanded_community_list.value])
         return expanded_community_list
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal
+from typing import List
 
 from pydantic import AliasPath, BaseModel, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class FowardingClassQueueEntry(BaseModel):
@@ -14,12 +14,11 @@
     @classmethod
     def check_burst(cls, queue: Global):
         assert 0 <= int(queue.value) <= 7
         return queue
 
 
 class FowardingClassParcel(_ParcelBase):
-    type_: Literal["class"] = Field(default="class", exclude=True)
     entries: List[FowardingClassQueueEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_queue(self, queue: int):
         self.entries.append(FowardingClassQueueEntry(queue=as_global(str(queue))))
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv6Address, IPv6Interface
-from typing import List, Literal
+from ipaddress import IPv6Address, IPv6Network
+from typing import List
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class IPv6DataPrefixEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     ipv6_address: Global[IPv6Address] = Field(serialization_alias="ipv6Address", validation_alias="ipv6Address")
     ipv6_prefix_length: Global[int] = Field(serialization_alias="ipv6PrefixLength", validation_alias="ipv6PrefixLength")
 
 
 class IPv6DataPrefixParcel(_ParcelBase):
-    type_: Literal["data-ipv6-prefix"] = Field(default="data-ipv6-prefix", exclude=True)
     entries: List[IPv6DataPrefixEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
-    def add_prefix(self, ipv6_network: IPv6Interface):
+    def add_prefix(self, ipv6_network: IPv6Network):
         self.entries.append(
             IPv6DataPrefixEntry(
-                ipv6_address=as_global(ipv6_network.network.network_address),
-                ipv6_prefix_length=as_global(ipv6_network.network.prefixlen),
+                ipv6_address=as_global(ipv6_network.network_address),
+                ipv6_prefix_length=as_global(ipv6_network.prefixlen),
             )
         )
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal
+from typing import List
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
+from catalystwan.models.policy.lists_entries import PolicerExceedAction
 
-PolicerExceedAction = Literal[
-    "drop",
-    "remark",
-]
 
-
-class PolicerEntry(BaseModel):
+class PolicierEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     burst: Global[int]
     exceed: Global[PolicerExceedAction]
     rate: Global[int]
 
     @field_validator("burst")
     @classmethod
@@ -27,19 +23,18 @@
     @field_validator("rate")
     @classmethod
     def check_rate(cls, rate_str: Global):
         assert 8 <= rate_str.value <= 100_000_000_000
         return rate_str
 
 
-class PolicerParcel(_ParcelBase):
-    type_: Literal["policer"] = Field(default="policer", exclude=True)
-    entries: List[PolicerEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
+class PolicierParcel(_ParcelBase):
+    entries: List[PolicierEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_entry(self, burst: int, exceed: PolicerExceedAction, rate: int):
         self.entries.append(
-            PolicerEntry(
+            PolicierEntry(
                 burst=as_global(burst),
                 exceed=as_global(exceed, PolicerExceedAction),
                 rate=as_global(rate),
             )
         )
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal, Optional
+from typing import List, Optional
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import TLOCColor
-
-PathPreference = Literal[
-    "direct-path",
-    "multi-hop-path",
-    "all-paths",
-]
+from catalystwan.models.policy.lists_entries import PathPreference
 
 
 class Preference(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     color_preference: Global[list] = Field(serialization_alias="colorPreference", validation_alias="colorPreference")
     path_preference: Global[PathPreference] = Field(
         serialization_alias="pathPreference", validation_alias="pathPreference"
@@ -38,15 +33,14 @@
     def check_passwords_match(self) -> "PreferredColorGroupEntry":
         if not self.secondary_preference and self.tertiary_preference:
             raise ValueError("Preference Entry has to have a secondary prefrence when assigning tertiary preference.")
         return self
 
 
 class PreferredColorGroupParcel(_ParcelBase):
-    type_: Literal["preferred-color-group"] = Field(default="preferred-color-group", exclude=True)
     entries: List[PreferredColorGroupEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_primary(self, color_preference: List[TLOCColor], path_preference: PathPreference):
         self.entries.append(
             PreferredColorGroupEntry(
                 primary_preference=Preference(
                     color_preference=as_global(color_preference),
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv4Address, IPv4Network
-from typing import List, Literal
+from ipaddress import IPv6Address, IPv6Network
+from typing import List
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
-class PrefixListEntry(BaseModel):
+class IPv6PrefixListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    ipv4_address: Global[IPv4Address] = Field(serialization_alias="ipv4Address", validation_alias="ipv4Address")
-    ipv4_prefix_length: Global[int] = Field(serialization_alias="ipv4PrefixLength", validation_alias="ipv4PrefixLength")
+    ipv6_address: Global[IPv6Address] = Field(serialization_alias="ipv6Address", validation_alias="ipv6Address")
+    ipv6_prefix_length: Global[int] = Field(serialization_alias="ipv6PrefixLength", validation_alias="ipv6PrefixLength")
 
 
-class PrefixListParcel(_ParcelBase):
-    type_: Literal["prefix"] = Field(default="prefix", exclude=True)
-    entries: List[PrefixListEntry] = Field(default_factory=list, validation_alias=AliasPath("data", "entries"))
+class IPv6PrefixListParcel(_ParcelBase):
+    entries: List[IPv6PrefixListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
-    def add_prefix(self, ipv4_network: IPv4Network):
+    def add_prefix(self, ipv6_network: IPv6Network):
         self.entries.append(
-            PrefixListEntry(
-                ipv4_address=as_global(ipv4_network.network_address),
-                ipv4_prefix_length=as_global(ipv4_network.prefixlen),
+            IPv6PrefixListEntry(
+                ipv6_address=as_global(ipv6_network.network_address),
+                ipv6_prefix_length=as_global(ipv6_network.prefixlen),
             )
         )
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,14 @@
     # validators
     _jitter_validator = field_validator("jitter")(check_jitter_ms)
     _latency_validator = field_validator("latency")(check_latency_ms)
     _loss_validator = field_validator("loss")(check_loss_percent)
 
 
 class SLAClassParcel(_ParcelBase):
-    type_: Literal["sla-class"] = Field(default="sla-class", exclude=True)
     entries: List[SLAClassListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_entry(
         self,
         app_probe_class_id: UUID,
         loss: Optional[int] = None,
         jitter: Optional[int] = None,
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal
+from typing import List
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import WellKnownBGPCommunities
 
 
 class StandardCommunityEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    standard_community: Global[str] = Field(
+    standard_community: Global[WellKnownBGPCommunities] = Field(
         serialization_alias="standardCommunity", validation_alias="standardCommunity"
     )
 
 
 class StandardCommunityParcel(_ParcelBase):
-    type_: Literal["standard-community"] = Field(default="standard-community", exclude=True)
     entries: List[StandardCommunityEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
-    def _add_community(self, standard_community: str):
-        self.entries.append(StandardCommunityEntry(standard_community=as_global(standard_community)))
-
-    def add_well_known_community(self, standard_community: WellKnownBGPCommunities):
-        self._add_community(standard_community)
-
-    def add_community(self, as_number: int, community_number: int) -> None:
-        self._add_community(f"{as_number}:{community_number}")
+    def add_community(self, standard_community: WellKnownBGPCommunities):
+        self.entries.append(
+            StandardCommunityEntry(standard_community=as_global(standard_community, WellKnownBGPCommunities))
+        )
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Address
-from typing import List, Literal, Optional
+from typing import List, Optional
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import TLOCColor
-
-EncapType = Literal[
-    "ipsec",
-    "gre",
-]
+from catalystwan.models.policy.lists_entries import EncapType
 
 
 class TlocEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     tloc: Global[IPv4Address]
     color: Global[TLOCColor]
     encapsulation: Global[EncapType] = Field(serialization_alias="encap", validation_alias="encap")
@@ -28,15 +24,14 @@
             return v
         if not (0 <= int(v.value) < 4_294_967_295):
             raise ValueError('"preference" not in range 0 - 4 294 967 295 (2 ** 32 - 1)')
         return v
 
 
 class TlocParcel(_ParcelBase):
-    type_: Literal["tloc"] = Field(default="tloc", exclude=True)
     entries: List[TlocEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_entry(
         self, tloc: IPv4Address, color: TLOCColor, encapsulation: EncapType, preference: Optional[str] = None
     ):
         self.entries.append(
             TlocEntry(
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal, Union
+from typing import List, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class SecurityApplicationListEntry(BaseModel):
@@ -14,15 +14,14 @@
 
 class SecurityApplicationFamilyListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     app_list_family: Global[str] = Field(serialization_alias="appFamily", validation_alias="appFamily")
 
 
 class SecurityApplicationListParcel(_ParcelBase):
-    type_: Literal["security-localapp"] = Field(default="security-localapp", exclude=True)
     entries: List[Union[SecurityApplicationFamilyListEntry, SecurityApplicationListEntry]] = Field(
         default=[], validation_alias=AliasPath("data", "entries")
     )
 
     def add_application(self, application: str):
         self.entries.append(SecurityApplicationListEntry(app_list=as_global(application)))
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal, Optional
+from typing import List, Optional
 
 from pydantic import AliasPath, BaseModel, Field, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import check_fields_exclusive
 
 
@@ -17,15 +17,14 @@
     @model_validator(mode="after")
     def check_country_xor_continent(self):
         check_fields_exclusive(self.__dict__, {"country", "continent"}, True)
         return self
 
 
 class GeoLocationListParcel(_ParcelBase):
-    type_: Literal["security-geolocation"] = Field(default="security-geolocation", exclude=True)
     entries: List[GeoLocationListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_country(self, country: str):
         self.entries.append(GeoLocationListEntry(country=as_global(country)))
 
     def add_continent(self, continent: str):
         self.entries.append(GeoLocationListEntry(continent=as_global(continent)))
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal
+from typing import List
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class IPSSignatureListEntry(BaseModel):
@@ -26,15 +26,14 @@
     @classmethod
     def check_signature_id(cls, signature_id: Global):
         assert 0 <= int(signature_id.value) <= 4294967295
         return signature_id
 
 
 class IPSSignatureParcel(_ParcelBase):
-    type_: Literal["security-ipssignature"] = Field(default="security-ipssignature", exclude=True)
     entries: List[IPSSignatureListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_signature(self, signature: str):
         generator_id, signature_id = signature.split(":")
         self.entries.append(
             IPSSignatureListEntry(
                 generator_id=as_global(generator_id),
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal
+from typing import List
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class LocalDomainListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     name_server: Global[str] = Field(
         serialization_alias="nameServer", validation_alias="nameServer", description="Ex: cisco.com, *.cisco.com"
     )
 
 
 class LocalDomainParcel(_ParcelBase):
-    type_: Literal["security-localdomain"] = Field(default="security-localdomain", exclude=True)
     entries: List[LocalDomainListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def from_local_domains(self, domains: List[str]):
         for domain in domains:
             self.entries.append(LocalDomainListEntry(name_server=as_global(domain)))
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal
+from typing import List
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class ProtocolListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     protocol: Global[str] = Field(serialization_alias="protocolName", validation_alias="protocolName")
 
 
 class ProtocolListParcel(_ParcelBase):
-    type_: Literal["security-protocolname"] = Field(default="security-protocolname", exclude=True)
     entries: List[ProtocolListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_protocol(self, protocol: str):
         self.entries.append(ProtocolListEntry(protocol=as_global(protocol)))
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal
+from typing import List
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class BaseURLListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     pattern: Global[str]
 
 
-class URLParcel(_ParcelBase):
-    type_: Literal["security-urllist"] = Field(default="security-urllist", exclude=True)
-    type: Literal["urlallowed", "urlblocked"]
+class BaseURLParcel(_ParcelBase):
     entries: List[BaseURLListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_url(self, pattern: str):
         self.entries.append(BaseURLListEntry(pattern=as_global(pattern)))
 
 
-class URLAllowParcel(URLParcel):
-    type_: Literal["security-urllist"] = Field(default="security-urllist", exclude=True)
-    type: Literal["urlallowed"] = "urlallowed"
+class URLAllowParcel(BaseURLParcel):
+    parcel_type: str = Field(default="urlallowed", validation_alias="type", serialization_alias="type")
 
 
-class URLBlockParcel(URLParcel):
-    type_: Literal["security-urllist"] = Field(default="security-urllist", exclude=True)
-    type: Literal["urlblocked"] = "urlblocked"
+class URLBlockParcel(BaseURLParcel):
+    parcel_type: str = Field(default="urlblocked", validation_alias="type", serialization_alias="type")
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal, Optional
+from typing import List, Optional
 
 from pydantic import AliasPath, BaseModel, Field, field_validator, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import InterfaceType, check_fields_exclusive
 
 
@@ -21,23 +21,22 @@
     @model_validator(mode="after")
     def check_vpn_xor_interface(self):
         check_fields_exclusive(self.__dict__, {"vpn", "interface"}, True)
         return self
 
 
 class SecurityZoneListParcel(_ParcelBase):
-    type_: Literal["security-zone"] = Field(default="security-zone", exclude=True)
     entries: List[SecurityZoneListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_interface(self, interface: InterfaceType):
         self.entries.append(
             SecurityZoneListEntry(
                 interface=as_global(interface, InterfaceType),
             )
         )
 
     def add_vpn(self, vpn: str):
         self.entries.append(
             SecurityZoneListEntry(
-                vpn=as_global(vpn),
+                vpn=as_global(vpn, InterfaceType),
             )
         )
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv4Address
 from typing import List, Literal, Optional, Union
 
-from pydantic import AliasPath, BaseModel, ConfigDict, Field
+from pydantic import BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default, as_global
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
 
 VirtualApplicationType = Literal["dreopt"]
 
 ResourceProfile = Literal[
     "small",
     "medium",
     "large",
@@ -23,48 +22,14 @@
     "serviceNode",
     "serviceNodeWithDre",
     "forwarderAndServiceNodeWithDre",
 ]
 
 AppnavControllerGroupName = Literal["ACG-APPQOE"]
 ServiceNodeGroupName = Literal["SNG-APPQOE"]
-ServiceNodeGroupsNames = Literal[
-    "SNG-APPQOE",
-    "SNG-APPQOE1",
-    "SNG-APPQOE2",
-    "SNG-APPQOE3",
-    "SNG-APPQOE4",
-    "SNG-APPQOE5",
-    "SNG-APPQOE6",
-    "SNG-APPQOE7",
-    "SNG-APPQOE8",
-    "SNG-APPQOE9",
-    "SNG-APPQOE10",
-    "SNG-APPQOE11",
-    "SNG-APPQOE12",
-    "SNG-APPQOE13",
-    "SNG-APPQOE14",
-    "SNG-APPQOE15",
-    "SNG-APPQOE16",
-    "SNG-APPQOE17",
-    "SNG-APPQOE18",
-    "SNG-APPQOE19",
-    "SNG-APPQOE20",
-    "SNG-APPQOE21",
-    "SNG-APPQOE22",
-    "SNG-APPQOE23",
-    "SNG-APPQOE24",
-    "SNG-APPQOE25",
-    "SNG-APPQOE26",
-    "SNG-APPQOE27",
-    "SNG-APPQOE28",
-    "SNG-APPQOE29",
-    "SNG-APPQOE30",
-    "SNG-APPQOE31",
-]
 ForwarderAndServiceNodeAddress = Literal["192.168.2.2"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
 ForwarderAndServiceNodeControllerAddress = Literal[
     "192.168.2.1"
 ]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
 ServiceNodeExternalAddress = Literal["192.168.2.2"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
 ServiceNodeExternalVpgIp = Literal["192.168.2.1/24"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
 
@@ -97,16 +62,16 @@
         validation_alias="appnavControllerGroup",
     )
     service_node_group: Global[ServiceNodeGroupName] = Field(
         default=Global[ServiceNodeGroupName](value="SNG-APPQOE"),
         serialization_alias="serviceNodeGroup",
         validation_alias="serviceNodeGroup",
     )
-    service_node_groups: List[Global[ServiceNodeGroupsNames]] = Field(
-        default=[Global[ServiceNodeGroupsNames](value="SNG-APPQOE")],
+    service_node_groups: List[Global[ServiceNodeGroupName]] = Field(
+        default=[Global[ServiceNodeGroupName](value="SNG-APPQOE")],
         serialization_alias="serviceNodeGroups",
         validation_alias="serviceNodeGroups",
     )
     enable: Global[bool] = Global[bool](value=True)
     vpn: Union[Global[int], Default[None], Variable] = Field(default=Global[int](value=0))
 
 
@@ -115,24 +80,22 @@
     appqoe: List[Appqoe]
 
 
 # Frowarder
 
 
 class ServiceNodeInformation(BaseModel):
-    address: Global[IPv4Address]
+    address: Global[str]
 
 
 class ForwarderController(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    address: Union[Global[str], Global[IPv4Address], Variable]
-    vpn: Global[int] = Field(
-        default=Global[int](value=1), description="This is field is a depended on the Service VPN value."
-    )
+    address: Union[Global[str], Variable]
+    vpn: Global[int] = Global[int](value=1)
 
 
 class ForwarderAppnavControllerGroup(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     group_name: Default[AppnavControllerGroupName] = Field(
         default=Default(value="ACG-APPQOE"), serialization_alias="groupName", validation_alias="groupName"
@@ -243,25 +206,30 @@
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     service_node_group: List[ServiceNodeGroup] = Field(
         default=[ServiceNodeGroup()], serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
     )
 
 
-class AppqoeParcel(_ParcelBase):
+class AppqoeData(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    dreopt: Optional[Union[Global[bool], Default[bool]]] = Field(
-        default=as_default(False), validation_alias=AliasPath("data", "dreopt")
-    )
+    dreopt: Optional[Union[Global[bool], Default[bool]]] = Default[bool](value=False)
     virtual_application: Optional[List[VirtualApplication]] = Field(
-        default=None, validation_alias=AliasPath("data", "virtualApplication")
+        serialization_alias="virtualApplication", validation_alias="virtualApplication"
     )
     appqoe_device_role: Global[str] = Field(
-        default=as_global("forwarder"), validation_alias=AliasPath("data", "appqoeDeviceRole")
+        default=Global(value="forwarder"), serialization_alias="appqoeDeviceRole", validation_alias="appqoeDeviceRole"
     )
 
-    forwarder: Optional[ForwarderRole] = Field(default=None, validation_alias=AliasPath("data", "forwarder"))
+    forwarder: Optional[ForwarderRole]
     forwarder_and_service_node: Optional[ForwarderAndServiceNodeRole] = Field(
-        default=None, validation_alias=AliasPath("data", "forwarderAndServiceNode")
+        serialization_alias="forwarderAndServiceNode", validation_alias="forwarderAndServiceNode"
     )
-    service_node: Optional[ServiceNodeRole] = Field(default=None, validation_alias=AliasPath("data", "serviceNode"))
+    service_node: Optional[ServiceNodeRole] = Field(serialization_alias="serviceNode", validation_alias="serviceNode")
+
+
+class AppqoeCreationPayload(BaseModel):
+    name: str
+    description: Optional[str] = None
+    data: AppqoeData
+    metadata: Optional[dict] = None
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Address, IPv6Address
-from typing import List, Literal, Optional, Union
+from typing import List, Optional, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default, as_global
 
 
 class PubkeyChainItem(BaseModel):
-    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    model_config = ConfigDict(
+        extra="forbid",
+    )
     key_string: Global[str] = Field(
         validation_alias="keyString",
         serialization_alias="keyString",
         pattern="^AAAA[0-9A-Za-z+/]+[=]{0,3}$",
         description="Set the RSA key string",
     )
 
@@ -23,15 +25,15 @@
         serialization_alias="keyType",
         validation_alias="keyType",
         description="Only RSA is supported",
     )
 
 
 class UserItem(BaseModel):
-    model_config = ConfigDict(extra="ignore", populate_by_name=True)
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
 
     name: Union[Global[str], Variable] = Field(description="Set the username")
     password: Union[Global[str], Variable] = Field(
         description=(
             "Set the user password [Note: Catalyst SD-WAN Manager will encrypt this field before saving."
             "Cleartext strings will not be returned back to the user in GET responses for sensitive fields.]"
         )
@@ -254,17 +256,15 @@
         default=None,
         validation_alias="ifAuthenticated",
         serialization_alias="ifAuthenticated",
         description="Succeed if user has authenticated",
     )
 
 
-class AAAParcel(_ParcelBase):
-    type_: Literal["aaa"] = Field(default="aaa", exclude=True)
-    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+class AAA(_ParcelBase):
     authentication_group: Union[Variable, Global[bool], Default[bool]] = Field(
         default=as_default(False),
         validation_alias=AliasPath("data", "authenticationGroup"),
         description="Authentication configurations parameters",
     )
     accounting_group: Union[Variable, Global[bool], Default[bool]] = Field(
         default=as_default(False),
@@ -274,17 +274,15 @@
     # local, radius, tacacs
     server_auth_order: Global[List[str]] = Field(
         validation_alias=AliasPath("data", "serverAuthOrder"),
         min_length=1,
         max_length=4,
         description="ServerGroups priority order",
     )
-    user: Optional[List[UserItem]] = Field(
-        default=None, validation_alias=AliasPath("data", "user"), description="Create local login account", min_length=1
-    )
+    user: Optional[List[UserItem]] = Field(default=None, description="Create local login account", min_length=1)
     radius: Optional[List[Radius]] = Field(
         default=None, validation_alias=AliasPath("data", "radius"), description="Configure the Radius serverGroup"
     )
     tacacs: Optional[List[Tacacs]] = Field(
         default=None, validation_alias=AliasPath("data", "tacacs"), description="Configure the TACACS serverGroup"
     )
     accounting_rule: Optional[List[AccountingRuleItem]] = Field(
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,84 @@
-from __future__ import annotations
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal, Optional, Union
+from typing import List, Optional, Union
 
-from pydantic import AliasPath, BaseModel, ConfigDict, Field
+from pydantic import BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
 
-EnableMrfMigration = Literal["enabled", "enabled-from-bgp-core"]
-Role = Literal["edge-router", "border-router"]
 
+class OptionCodeAscii(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-class ManagementRegion(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    vrf_id: Union[Global[int], Default[None], Variable] = Field(
-        default=Default[None](value=None),
-        serialization_alias="vrfId",
-        validation_alias="vrfId",
-        description="VRF name for management region",
-    )
-    gateway_preference: Optional[Union[Global[List[int]], Default[None], Variable]] = Field(
-        default=Default[None](value=None),
-        serialization_alias="gatewayPreference",
-        validation_alias="gatewayPreference",
-        description="List of affinity group preferences for VRF",
-    )
-    management_gateway: Union[Global[bool], Default[bool], Variable] = Field(
-        default=as_default(False),
-        serialization_alias="managementGateway",
-        validation_alias="managementGateway",
-        description="Enable management gateway",
+    code: Union[Global[int], Variable]
+    ascii: Union[Global[str], Variable]
+
+
+class OptionCodeHex(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+
+    code: Union[Global[int], Variable]
+    hex: Union[Global[str], Variable]
+
+
+class OptionCodeIP(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+
+    code: Union[Global[int], Variable]
+    ip: Union[Global[List[str]], Variable]
+
+
+class StaticLease(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+
+    mac_address: Union[Global[str], Variable] = Field(serialization_alias="macAddress", validation_alias="macAddress")
+    ip: Union[Global[str], Variable]
+
+
+class DhcpAddressPool(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+
+    network_address: Union[Global[str], Variable] = Field(
+        serialization_alias="networkAddress", validation_alias="networkAddress"
     )
+    subnet_mask: Union[Global[str], Variable] = Field(serialization_alias="subnetMask", validation_alias="subnetMask")
 
 
-class MRFParcel(_ParcelBase):
-    type_: Literal["mrf"] = Field(default="mrf", exclude=True)
+class DhcpServerData(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
+    address_pool: DhcpAddressPool = Field(serialization_alias="addressPool", validation_alias="addressPool")
+    exclude: Optional[Union[Global[List[str]], Variable, Default[None]]] = None
+    lease_time: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="leaseTime", validation_alias="leaseTime", default=Default[int](value=86400)
     )
-    secondary_region: Union[Global[int], Variable, Default[None]] = Field(
-        default=Default[None](value=None),
-        validation_alias=AliasPath("data", "secondaryRegion"),
-        description="Set secondary region ID",
+    interface_mtu: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="interfaceMtu", validation_alias="interfaceMtu", default=None
     )
-    role: Union[Global[Role], Variable, Default[None]] = Field(
-        default=Default[None](value=None),
-        validation_alias=AliasPath("data", "role"),
-        description="Set the role for router",
+    domain_name: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="domainName", validation_alias="domainName", default=None
     )
-    enable_mrf_migration: Union[Global[EnableMrfMigration], Default[None]] = Field(
-        default=Default[None](value=None),
-        validation_alias=AliasPath("data", "enableMrfMigration"),
-        description="Enable migration mode to Multi-Region Fabric",
+    default_gateway: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="defaultGateway", validation_alias="defaultGateway", default=None
     )
-    migration_bgp_community: Optional[Union[Global[int], Default[None]]] = Field(
-        default=Default[None](value=None),
-        validation_alias=AliasPath("data", "migrationBgpCommunity"),
-        description="Set BGP community during migration from BGP-core based network",
+    dns_servers: Optional[Union[Global[List[str]], Variable, Default[None]]] = Field(
+        serialization_alias="dnsServers", validation_alias="dnsServers", default=None
     )
-    enable_management_region: Union[Global[bool], Default[bool], Variable] = Field(
-        default=as_default(False),
-        validation_alias=AliasPath("data", "enableManagementRegion"),
-        description="Enable management region",
+    tftp_servers: Optional[Union[Global[List[str]], Variable, Default[None]]] = Field(
+        serialization_alias="tftpServers", validation_alias="tftpServers", default=None
     )
-    management_region: ManagementRegion = Field(
-        default_factory=ManagementRegion,
-        validation_alias=AliasPath("data", "managementRegion"),
-        description="Management Region",
+    static_lease: Optional[List[StaticLease]] = Field(
+        serialization_alias="staticLease", validation_alias="staticLease", default=None
     )
+    option_code: Optional[List[Union[OptionCodeAscii, OptionCodeHex, OptionCodeIP]]] = Field(
+        serialization_alias="optionCode", validation_alias="optionCode", default=None
+    )
+
+
+class DhcpSeverCreationPayload(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+
+    name: str
+    description: Optional[str] = None
+    data: DhcpServerData
+    metadata: Optional[dict] = None
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py` & `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         default=None,
         description="Enable/Disable Firmware Auto Sim",
         serialization_alias="autoSim",
         validation_alias="autoSim",
     )
 
 
-class CellularControllerParcel(_ParcelBase):
-    type_: Literal["cellular-controller"] = Field(default="cellular-controller", exclude=True)
+class CellularController(_ParcelBase):
     config_type: Default[ConfigTypeValue] = Field(
         default=Default(value="non-eSim"), validation_alias=AliasPath("data", "configType")
     )
     controller_config: ControllerConfig = Field(validation_alias=AliasPath("data", "controllerConfig"))
 
     @staticmethod
     def add_controller_config(
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/device_inventory.py` & `catalystwan-0.32.0/catalystwan/models/device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/misc/application_protocols.py` & `catalystwan-0.32.0/catalystwan/models/misc/application_protocols.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/centralized.py` & `catalystwan-0.32.0/catalystwan/models/policy/centralized.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union, overload
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field, model_validator
+from pydantic import BaseModel, ConfigDict, Field, field_validator
 from typing_extensions import Annotated
 
 from catalystwan.models.policy.policy import (
     AssemblyItemBase,
     PolicyCreationPayload,
     PolicyDefinition,
     PolicyEditPayload,
@@ -157,35 +157,20 @@
     type: Literal["hubAndSpoke"] = "hubAndSpoke"
 
 
 class MeshPolicyItem(AssemblyItemBase):
     type: Literal["mesh"] = "mesh"
 
 
-class AppRoutePolicyItem(AssemblyItemBase):
-    type: Literal["appRoute"] = "appRoute"
-
-
-class CFlowDPolicyItem(AssemblyItemBase):
-    type: Literal["cflowd"] = "cflowd"
-
-
-class VpnMembershipGroupPolicyItem(AssemblyItemBase):
-    type: Literal["vpnMembershipGroup"] = "vpnMembershipGroup"
-
-
 AnyAssemblyItem = Annotated[
     Union[
         TrafficDataPolicyItem,
         ControlPolicyItem,
         MeshPolicyItem,
         HubAndSpokePolicyItem,
-        AppRoutePolicyItem,
-        CFlowDPolicyItem,
-        VpnMembershipGroupPolicyItem,
     ],
     Field(discriminator="type"),
 ]
 
 
 class CentralizedPolicyDefinition(PolicyDefinition):
     region_role_assembly: List = Field(
@@ -197,15 +182,15 @@
 
 class CentralizedPolicy(PolicyCreationPayload):
     policy_definition: CentralizedPolicyDefinition = Field(
         default=CentralizedPolicyDefinition(),
         serialization_alias="policyDefinition",
         validation_alias="policyDefinition",
     )
-    policy_type: Literal["feature", "cli"] = Field(
+    policy_type: Literal["feature"] = Field(
         default="feature", serialization_alias="policyType", validation_alias="policyType"
     )
 
     def add_traffic_data_policy(self, traffic_data_policy_id: UUID) -> TrafficDataPolicyItem:
         item = TrafficDataPolicyItem(definition_id=traffic_data_policy_id)
         self.policy_definition.assembly.append(item)
         return item
@@ -217,28 +202,24 @@
 
     def add_mesh_policy(self, mesh_policy_id: UUID) -> None:
         self.policy_definition.assembly.append(MeshPolicyItem(definition_id=mesh_policy_id))
 
     def add_hub_and_spoke_policy(self, hub_and_spoke_policy_id: UUID) -> None:
         self.policy_definition.assembly.append(HubAndSpokePolicyItem(definition_id=hub_and_spoke_policy_id))
 
-    @model_validator(mode="before")
+    @field_validator("policy_definition", mode="before")
     @classmethod
-    def try_parse_policy_definition_string(cls, values):
+    def try_parse(cls, policy_definition):
         # this is needed because GET /template/policy/vsmart contains string in policyDefinition field
         # while POST /template/policy/vsmart requires a regular object
         # it makes sense to reuse that model for both requests and present parsed data to the user
-        # TODO: this is workaround, probably it is better to provide separate models for "cli" and "feature"
-        if (policy_definition := values.get("policyDefinition")) and values.get("policyType") != "cli":
-            if isinstance(policy_definition, str):
-                values["policyDefinition"] = CentralizedPolicyDefinition.model_validate_json(policy_definition)
-        else:
-            values["policyDefinition"] = CentralizedPolicyDefinition()
-        return values
+        if isinstance(policy_definition, str):
+            return CentralizedPolicyDefinition.parse_raw(policy_definition)
+        return policy_definition
 
 
 class CentralizedPolicyEditPayload(PolicyEditPayload, CentralizedPolicy):
-    rid: Optional[int] = Field(default=None, serialization_alias="@rid", validation_alias="@rid")
+    rid: Optional[str] = Field(default=None, serialization_alias="@rid", validation_alias="@rid")
 
 
 class CentralizedPolicyInfo(PolicyInfo, CentralizedPolicyEditPayload):
     pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/access_control_list.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/access_control_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,14 @@
     MirrorAction,
     NextHopEntry,
     PacketLengthEntry,
     PLPEntry,
     PolicerAction,
     PolicyActionType,
     PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     ProtocolEntry,
     Reference,
     SourceDataPrefixListEntry,
     SourceIPEntry,
     SourcePortEntry,
     TCPEntry,
@@ -89,16 +87,16 @@
 
     def match_high_plp(self) -> None:
         self._insert_match(PLPEntry(value="high"))
 
     def match_protocols(self, protocols: Set[int]) -> None:
         self._insert_match(ProtocolEntry.from_protocol_set(protocols))
 
-    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
+    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
 
     def match_source_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(SourceIPEntry.from_ipv4_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
@@ -159,15 +157,7 @@
         seq = AclPolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         self.add(seq)
         return seq
-
-
-class AclPolicyEditPayload(AclPolicy, PolicyDefinitionId):
-    pass
-
-
-class AclPolicyGetResponse(AclPolicy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/access_control_list_ipv6.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,14 @@
     NextHeaderEntry,
     NextHopEntry,
     PacketLengthEntry,
     PLPEntry,
     PolicerAction,
     PolicyActionType,
     PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     Reference,
     SourceDataIPv6PrefixListEntry,
     SourceIPv6Entry,
     SourcePortEntry,
     TCPEntry,
     TrafficClassEntry,
@@ -159,15 +157,7 @@
         seq = AclIPv6PolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv6",
         )
         self.add(seq)
         return seq
-
-
-class AclIPv6PolicyEditPayload(AclIPv6Policy, PolicyDefinitionId):
-    pass
-
-
-class AclIPv6PolicyGetResponse(AclIPv6Policy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/control.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from ipaddress import IPv4Address
 from typing import Any, List, Literal, Optional, Union, overload
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
-from catalystwan.models.common import EncapType, TLOCColor
+from catalystwan.models.common import TLOCColor
+from catalystwan.models.policy.lists_entries import EncapType
 from catalystwan.models.policy.policy_definition import (
     AffinityEntry,
     Carrier,
     CarrierEntry,
     ColorListEntry,
     CommunityAdditiveEntry,
     CommunityEntry,
@@ -28,16 +29,14 @@
     OriginatorEntry,
     OriginEntry,
     OriginProtocol,
     PathType,
     PathTypeEntry,
     PolicyActionType,
     PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     PreferenceEntry,
     PrefixListEntry,
     RegionEntry,
     RegionListEntry,
     RoleEntry,
     ServiceEntry,
@@ -338,15 +337,7 @@
         seq = ControlPolicyTLOCSequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         self.add(seq)
         return seq
-
-
-class ControlPolicyEditPayload(ControlPolicy, PolicyDefinitionId):
-    pass
-
-
-class ControlPolicyGetResponse(ControlPolicy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/device_access.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/device_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,14 @@
     DestinationDataPrefixListEntry,
     DestinationIPEntry,
     DestinationPortEntry,
     DeviceAccessProtocol,
     Match,
     PolicyActionType,
     PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     SourceDataPrefixListEntry,
     SourceIPEntry,
     SourcePortEntry,
 )
 
 DeviceAccessPolicySequenceMatchEntry = Annotated[
@@ -59,16 +57,16 @@
     match: DeviceAccessPolicySequenceMatch = DeviceAccessPolicySequenceMatch()
     actions: List[DeviceAccessPolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_device_access_protocol(self, port: DeviceAccessProtocol) -> None:
         self._insert_match(DestinationPortEntry.from_port_set_and_ranges(ports={port}))
 
-    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
+    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
 
     def match_source_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(SourceIPEntry.from_ipv4_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
@@ -102,15 +100,7 @@
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         if device_access_protocol is not None:
             seq.match_device_access_protocol(port=device_access_protocol)
         self.add(seq)
         return seq
-
-
-class DeviceAccessPolicyEditPayload(DeviceAccessPolicy, PolicyDefinitionId):
-    pass
-
-
-class DeviceAccessPolicyGetResponse(DeviceAccessPolicy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/device_access_ipv6.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/device_access_ipv6.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,14 @@
     DestinationDataIPv6PrefixListEntry,
     DestinationIPv6Entry,
     DestinationPortEntry,
     DeviceAccessProtocol,
     Match,
     PolicyActionType,
     PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     SourceDataIPv6PrefixListEntry,
     SourceIPv6Entry,
     SourcePortEntry,
 )
 
 DeviceAccessIPv6PolicySequenceMatchEntry = Annotated[
@@ -102,15 +100,7 @@
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         if device_access_protocol is not None:
             seq.match_device_access_protocol(port=device_access_protocol)
         self.add(seq)
         return seq
-
-
-class DeviceAccessIPv6PolicyEditPayload(DeviceAccessIPv6Policy, PolicyDefinitionId):
-    pass
-
-
-class DeviceAccessIPv6PolicyGetResponse(DeviceAccessIPv6Policy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/hub_and_spoke.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/hub_and_spoke.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
-from catalystwan.models.policy.policy_definition import (
-    PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
-)
+from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
 
 
 class Hub(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     site_list: UUID = Field(validation_alias="siteList", serialization_alias="siteList")
     preference: Optional[str] = None
     prefix_lists: List[UUID] = Field(default=[], validation_alias="prefixLists", serialization_alias="prefixLists")
@@ -71,15 +67,7 @@
             equal_preference=True,
             advertise_tloc=(advertise_tloc_list is not None),
             tloc_list=advertise_tloc_list,
             spokes=spokes,
         )
         self.definition.sub_definitions.append(sub_definition)
         return sub_definition
-
-
-class HubAndSpokePolicyEditPayload(HubAndSpokePolicy, PolicyDefinitionId):
-    pass
-
-
-class HubAndSpokePolicyGetResponse(HubAndSpokePolicy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/mesh.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/mesh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
-from catalystwan.models.policy.policy_definition import (
-    PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
-)
+from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
 
 
 class Region(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     name: str
     site_lists: List[UUID] = Field(validation_alias="siteLists", serialization_alias="siteLists")
 
@@ -33,15 +29,7 @@
     def from_vpn_list(name: str, vpn_list: UUID) -> "MeshPolicy":
         return MeshPolicy(name=name, definition=MeshPolicyDefinition(vpn_list=vpn_list))
 
     def add_region(self, name: str, site_lists: List[UUID]) -> Region:
         region = Region(name=name, site_lists=site_lists)
         self.definition.regions.append(region)
         return region
-
-
-class MeshPolicyEditPayload(MeshPolicy, PolicyDefinitionId):
-    pass
-
-
-class MeshPolicyGetResponse(MeshPolicy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/qos_map.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/qos_map.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field, field_validator, model_validator
 
-from catalystwan.models.common import IntStr
-from catalystwan.models.policy.policy_definition import (
-    PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
-)
+from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
 
 QoSScheduling = Literal[
     "llq",
     "wrr",
 ]
 
 QoSDropType = Literal[
     "tail-drop",
     "red-drop",
 ]
 
 
 class QoSScheduler(BaseModel):
-    queue: IntStr = Field(ge=0, le=8)
-    class_map_ref: Optional[UUID] = Field(
-        default=None, serialization_alias="classMapRef", validation_alias="classMapRef"
-    )
-    bandwidth_percent: IntStr = Field(
-        default=1, ge=1, le=100, serialization_alias="bandwidthPercent", validation_alias="bandwidthPercent"
-    )
-    buffer_percent: IntStr = Field(
-        default=1, ge=1, le=100, serialization_alias="bufferPercent", validation_alias="bufferPercent"
-    )
-    burst: Optional[IntStr] = Field(default=None, ge=5000, le=10_000_000)
+    queue: str
+    class_map_ref: Union[UUID, Literal[""]] = Field(serialization_alias="classMapRef", validation_alias="classMapRef")
+    bandwidth_percent: str = Field("1", serialization_alias="bandwidthPercent", validation_alias="bandwidthPercent")
+    buffer_percent: str = Field("1", serialization_alias="bufferPercent", validation_alias="bufferPercent")
+    burst: Optional[str] = None
     scheduling: QoSScheduling = "wrr"
     drops: QoSDropType = "tail-drop"
     temp_key_values: Optional[str] = Field(
         default=None, serialization_alias="tempKeyValues", validation_alias="tempKeyValues"
     )
 
     @staticmethod
     def get_default_control_scheduler() -> "QoSScheduler":
         return QoSScheduler(
-            queue=0,
-            bandwidth_percent=100,
-            buffer_percent=100,
-            burst=15000,
+            queue="0",
+            class_map_ref="",
+            bandwidth_percent="100",
+            buffer_percent="100",
+            burst="15000",
             scheduling="llq",
             drops="tail-drop",
         )
 
     model_config = ConfigDict(populate_by_name=True)
 
-    @field_validator("class_map_ref", mode="before")
+    @field_validator("queue")
     @classmethod
-    def check_optional_class_map_ref(cls, class_map_ref: Union[str, None]):
-        # None and "" indicates missing value, both can be found in server responses
-        if not class_map_ref:
-            return None
-        return class_map_ref
+    def check_queue(cls, queue_str: str):
+        assert 0 <= int(queue_str) <= 7
+        return queue_str
+
+    @field_validator("bandwidth_percent", "buffer_percent")
+    @classmethod
+    def check_bandwidth_and_buffer_percent(cls, percent_str: str):
+        assert 1 <= int(percent_str) <= 100
+        return percent_str
+
+    @field_validator("burst")
+    @classmethod
+    def check_burst(cls, burst_val: Union[str, None]):
+        if burst_val is not None:
+            assert 5000 <= int(burst_val) <= 10_000_000
+        return burst_val
 
 
 class QoSMapDefinition(BaseModel):
     qos_schedulers: List[QoSScheduler] = Field(serialization_alias="qosSchedulers", validation_alias="qosSchedulers")
     model_config = ConfigDict(populate_by_name=True)
 
 
@@ -81,31 +82,23 @@
         buffer: int = 1,
         scheduling: QoSScheduling = "wrr",
         drops: QoSDropType = "tail-drop",
         burst: Optional[int] = None,
     ) -> None:
         self.definition.qos_schedulers.append(
             QoSScheduler(
-                queue=queue,
+                queue=str(queue),
                 class_map_ref=class_map_ref,
-                bandwidth_percent=bandwidth,
-                buffer_percent=buffer,
-                burst=burst,
+                bandwidth_percent=str(bandwidth),
+                buffer_percent=str(buffer),
+                burst=str(burst) if burst is not None else None,
                 scheduling=scheduling,
                 drops=drops,
             )
         )
 
     @model_validator(mode="after")
     def generate_default_control_scheduler(self):
         if not self.definition.qos_schedulers:
             # Only when creating (not when value obtained from remote is present)
             self.definition = QoSMapDefinition(qos_schedulers=[QoSScheduler.get_default_control_scheduler()])
         return self
-
-
-class QoSMapPolicyEditPayload(QoSMapPolicy, PolicyDefinitionId):
-    pass
-
-
-class QoSMapPolicyGetResponse(QoSMapPolicy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/rewrite.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/rewrite.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.models.policy.policy_definition import (
     DefinitionWithSequencesCommonBase,
     PLPEntryType,
     PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
 )
 
 
 class RewritePolicyHeader(PolicyDefinitionBase):
     type: Literal["rewriteRule"] = "rewriteRule"
 
 
@@ -33,15 +31,7 @@
 class RewritePolicy(RewritePolicyHeader, DefinitionWithSequencesCommonBase):
     definition: RewritePolicyDefinition = RewritePolicyDefinition()
 
     def add_rule(self, class_map_ref: UUID, dscp: int, l2cos: int, plp: PLPEntryType) -> None:
         self.definition.rules.append(RewritePolicyRule(class_=class_map_ref, plp=plp, dscp=str(dscp), l2cos=str(l2cos)))
 
     model_config = ConfigDict(populate_by_name=True)
-
-
-class RewritePolicyEditPayload(RewritePolicy, PolicyDefinitionId):
-    pass
-
-
-class RewritePolicyGetResponse(RewritePolicy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/rule_set.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/rule_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,15 @@
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field, model_validator
 from typing_extensions import Annotated
 
 from catalystwan.models.common import check_fields_exclusive
-from catalystwan.models.policy.policy_definition import (
-    PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
-    Reference,
-    VariableName,
-)
+from catalystwan.models.policy.policy_definition import PolicyDefinitionBase, Reference, VariableName
 
 
 class RuleBase(BaseModel):
     rule: str = ""
     order: str = ""
     action: str = "permit"
     source_security_group: Optional[Reference] = Field(
@@ -256,15 +250,7 @@
             destination_port=destination_port,
             destination_port_list=Reference(ref=destination_port_list_id) if destination_port_list_id else None,
             protocol=" ".join(str(p) for p in protocols) if protocols else None,
             protocol_name=" ".join(p for p in protocol_names) if protocol_names else None,
             protocol_name_list=Reference(ref=protocol_name_list_id) if protocol_name_list_id else None,
         )
         self.add(ipv4_rule)
-
-
-class RuleSetEditPayload(RuleSet, PolicyDefinitionId):
-    pass
-
-
-class RuleSetGetResponse(RuleSet, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/security_group.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/security_group.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,21 +2,15 @@
 
 from ipaddress import IPv4Network, IPv6Network
 from typing import Literal, Optional, Union
 
 from pydantic import BaseModel, ConfigDict, Field, model_validator
 
 from catalystwan.models.common import check_any_of_exclusive_field_sets, check_fields_exclusive
-from catalystwan.models.policy.policy_definition import (
-    PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
-    Reference,
-    VariableName,
-)
+from catalystwan.models.policy.policy_definition import PolicyDefinitionBase, Reference, VariableName
 
 SequenceIPType = Literal[
     "ipv4",
     "ipv6",
 ]
 
 
@@ -69,15 +63,7 @@
         if (
             self.sequence_ip_type == SequenceIPType.IPV4 and isinstance(self.definition, SecurityGroupIPv6Definition)
         ) or (
             self.sequence_ip_type == SequenceIPType.IPV6 and isinstance(self.definition, SecurityGroupIPv4Definition)
         ):
             raise ValueError(f"Incompatible definition for {self.sequence_ip_type} sequence")
         return self
-
-
-class SecurityGroupEditPayload(SecurityGroup, PolicyDefinitionId):
-    pass
-
-
-class SecurityGroupGetResponse(SecurityGroup, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/traffic_data.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/traffic_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from ipaddress import IPv4Address, IPv4Network
 from typing import Any, List, Literal, Optional, Set, Tuple, Union, overload
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
-from catalystwan.models.common import EncapType, ICMPMessageType, ServiceChainNumber, TLOCColor
+from catalystwan.models.common import ServiceChainNumber, TLOCColor
+from catalystwan.models.policy.lists_entries import EncapType
 from catalystwan.models.policy.policy_definition import (
     AppListEntry,
     CFlowDAction,
     CountAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataIPv6PrefixListEntry,
     DestinationDataPrefixListEntry,
@@ -21,15 +22,14 @@
     DNSAppListEntry,
     DNSEntry,
     DNSTypeEntryType,
     DREOptimizationAction,
     DSCPEntry,
     FallBackToRoutingAction,
     ForwardingClassEntry,
-    ICMPMessageEntry,
     LocalTLOCListEntry,
     LocalTLOCListEntryValue,
     LogAction,
     LossProtectionAction,
     LossProtectionFECAction,
     LossProtectionPacketDuplicationAction,
     LossProtectionType,
@@ -38,16 +38,14 @@
     NextHopEntry,
     NextHopLooseEntry,
     PacketLengthEntry,
     PLPEntry,
     PolicerListEntry,
     PolicyActionType,
     PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     PrefferedColorGroupListEntry,
     ProtocolEntry,
     RedirectDNSAction,
     SecureInternetGatewayAction,
     ServiceChainEntry,
     ServiceChainEntryValue,
@@ -64,33 +62,32 @@
     TrafficToEntry,
     VPNEntry,
     accept_action,
 )
 
 TrafficDataPolicySequenceEntry = Annotated[
     Union[
-        AppListEntry,
-        DestinationDataIPv6PrefixListEntry,
-        DestinationDataPrefixListEntry,
-        DestinationIPEntry,
-        DestinationPortEntry,
-        DestinationRegionEntry,
-        DNSAppListEntry,
-        DNSEntry,
-        DSCPEntry,
-        ICMPMessageEntry,
         PacketLengthEntry,
         PLPEntry,
         ProtocolEntry,
-        SourceDataIPv6PrefixListEntry,
-        SourceDataPrefixListEntry,
+        DSCPEntry,
         SourceIPEntry,
         SourcePortEntry,
+        DestinationIPEntry,
+        DestinationPortEntry,
         TCPEntry,
+        DNSEntry,
         TrafficToEntry,
+        SourceDataPrefixListEntry,
+        DestinationDataPrefixListEntry,
+        SourceDataIPv6PrefixListEntry,
+        DestinationDataIPv6PrefixListEntry,
+        DestinationRegionEntry,
+        DNSAppListEntry,
+        AppListEntry,
     ],
     Field(discriminator="field"),
 ]
 
 TrafficDataPolicySequenceActions = Any  # TODO
 
 
@@ -99,15 +96,15 @@
 
 
 class TrafficDataPolicySequenceMatch(Match):
     entries: List[TrafficDataPolicySequenceEntry] = []
 
 
 class TrafficDataPolicySequence(PolicyDefinitionSequenceBase):
-    sequence_type: Literal["applicationFirewall", "qos", "serviceChaining", "trafficEngineering", "data"] = Field(
+    sequence_type: Literal["data"] = Field(
         default="data", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
     match: TrafficDataPolicySequenceMatch = TrafficDataPolicySequenceMatch()
     actions: List[TrafficDataPolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_app_list(self, app_list_id: UUID) -> None:
@@ -121,31 +118,28 @@
 
     def match_dns_response(self) -> None:
         self._insert_match(DNSEntry(value="response"))
 
     def match_dscp(self, dscp: int) -> None:
         self._insert_match(DSCPEntry(value=str(dscp)))
 
-    def match_icmp(self, icmp_message_types: List[ICMPMessageType]) -> None:
-        self._insert_match(ICMPMessageEntry(value=icmp_message_types))
-
     def match_packet_length(self, packet_lengths: Tuple[int, int]) -> None:
         self._insert_match(PacketLengthEntry.from_range(packet_lengths))
 
     def match_low_plp(self) -> None:
         self._insert_match(PLPEntry(value="low"))
 
     def match_high_plp(self) -> None:
         self._insert_match(PLPEntry(value="high"))
 
     def match_protocols(self, protocols: Set[int]) -> None:
         self._insert_match(ProtocolEntry.from_protocol_set(protocols))
 
-    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
+    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
 
     def match_source_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(SourceIPEntry.from_ipv4_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
@@ -373,15 +367,7 @@
         seq = TrafficDataPolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         self.add(seq)
         return seq
-
-
-class TrafficDataPolicyEditPayload(TrafficDataPolicy, PolicyDefinitionId):
-    pass
-
-
-class TrafficDataPolicyGetResponse(TrafficDataPolicy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/vpn_membership.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/vpn_membership.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
-from catalystwan.models.policy.policy_definition import (
-    PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
-)
+from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
 
 
 class Site(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     site_list: UUID = Field(validation_alias="siteList", serialization_alias="siteList")
     vpn_list: List[UUID] = Field(validation_alias="vpnList", serialization_alias="vpnList")
 
@@ -28,15 +24,7 @@
     type: Literal["vpnMembershipGroup"] = "vpnMembershipGroup"
     definition: VPNMembershipPolicyDefinition = VPNMembershipPolicyDefinition()
 
     def add_site(self, site_list: UUID, vpn_lists: List[UUID]) -> Site:
         site = Site(site_list=site_list, vpn_list=vpn_lists)
         self.definition.sites.append(site)
         return site
-
-
-class VPNMembershipPolicyEditPayload(VPNMembershipPolicy, PolicyDefinitionId):
-    pass
-
-
-class VPNMembershipPolicyGetResponse(VPNMembershipPolicy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/definition/zone_based_firewall.py` & `catalystwan-0.32.0/catalystwan/models/policy/definitions/zone_based_firewall.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,27 @@
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from catalystwan.models.misc.application_protocols import ApplicationProtocol
 from catalystwan.models.policy.policy_definition import (
-    AdvancedInspectionProfileAction,
     AppListEntry,
-    AppListFlatEntry,
-    ConnectionEventsAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataPrefixListEntry,
     DestinationFQDNEntry,
     DestinationGeoLocationEntry,
     DestinationGeoLocationListEntry,
     DestinationIPEntry,
     DestinationPortEntry,
     DestinationPortListEntry,
     LogAction,
     Match,
     PolicyActionType,
     PolicyDefinitionBase,
-    PolicyDefinitionGetResponse,
-    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     ProtocolEntry,
     ProtocolNameEntry,
     ProtocolNameListEntry,
     RuleSetListEntry,
     SourceDataPrefixListEntry,
     SourceFQDNEntry,
@@ -41,15 +36,14 @@
     SourcePortEntry,
     SourcePortListEntry,
 )
 
 ZoneBasedFWPolicySequenceEntry = Annotated[
     Union[
         AppListEntry,
-        AppListFlatEntry,
         DestinationDataPrefixListEntry,
         DestinationFQDNEntry,
         DestinationGeoLocationEntry,
         DestinationGeoLocationListEntry,
         DestinationIPEntry,
         DestinationPortEntry,
         DestinationPortListEntry,
@@ -73,35 +67,26 @@
     Union[
         AppListEntry,
         RuleSetListEntry,
     ],
     Field(discriminator="field"),
 ]
 
-ZoneBasedFWPolicyActions = Annotated[
-    Union[
-        AdvancedInspectionProfileAction,
-        ConnectionEventsAction,
-        LogAction,
-    ],
-    Field(discriminator="type"),
-]
-
 
 class ZoneBasedFWPolicyMatches(Match):
     entries: List[ZoneBasedFWPolicySequenceEntry] = []
 
 
 class ZoneBasedFWPolicySequenceWithRuleSets(PolicyDefinitionSequenceBase):
     sequence_type: Literal["zoneBasedFW"] = Field(
         default="zoneBasedFW", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
     match: ZoneBasedFWPolicyMatches
     ruleset: bool = True
-    actions: List[ZoneBasedFWPolicyActions] = []
+    actions: List[LogAction] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_rule_set_lists(self, rule_set_ids: Set[UUID]) -> None:
         self._insert_match(RuleSetListEntry.from_rule_set_ids(rule_set_ids))
 
     def match_app_list(self, app_list_id: UUID) -> None:
         if self.base_action != "inspect":
@@ -156,16 +141,16 @@
         self._insert_match(ProtocolNameEntry.from_application_protocols(app_protocols))
         self._insert_match(DestinationPortEntry.from_application_protocols(app_protocols), False)
         self._insert_match(ProtocolEntry.from_application_protocols(app_protocols), False)
 
     def match_protocol_name_list(self, protocol_name_list_id: UUID) -> None:
         self._insert_match(ProtocolNameListEntry(ref=protocol_name_list_id))
 
-    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
+    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
 
     def match_source_fqdn(self, fqdn: str) -> None:
         self._insert_match(SourceFQDNEntry(value=fqdn))
 
     def match_source_fqdn_list(self, fqdn_list_id: UUID) -> None:
         self._insert_match(SourceFQDNListEntry(ref=fqdn_list_id))
 
@@ -202,15 +187,15 @@
 class ZoneBasedFWPolicyDefinition(DefinitionWithSequencesCommonBase):
     sequences: List[Union[ZoneBasedFWPolicySequence, ZoneBasedFWPolicySequenceWithRuleSets]] = []
     entries: List[ZoneBasedFWPolicyEntry] = []
 
 
 class ZoneBasedFWPolicy(ZoneBasedFWPolicyHeader):
     type: Literal["zoneBasedFW"] = "zoneBasedFW"
-    mode: Literal["security", "unified"] = "security"
+    mode: Literal["security"] = "security"
     definition: ZoneBasedFWPolicyDefinition = ZoneBasedFWPolicyDefinition()
 
     def add_ipv4_rule(
         self, name: str, base_action: PolicyActionType = "drop", log: bool = False
     ) -> ZoneBasedFWPolicySequence:
         """Adds new IPv4 Rule to Zone Based Firewall Policy
 
@@ -249,15 +234,7 @@
 
     def add_zone_pair(self, source_zone_id: UUID, destination_zone_id: UUID) -> None:
         entry = ZoneBasedFWPolicyEntry(
             source_zone_id=source_zone_id,
             destination_zone_id=destination_zone_id,
         )
         self.definition.entries.append(entry)
-
-
-class ZoneBasedFWPolicyEditPayload(ZoneBasedFWPolicy, PolicyDefinitionId):
-    pass
-
-
-class ZoneBasedFWPolicyGetResponse(ZoneBasedFWPolicy, PolicyDefinitionGetResponse):
-    pass
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/list/app.py` & `catalystwan-0.32.0/catalystwan/models/policy/policy_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,49 @@
-from typing import List, Literal, Optional
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
-from pydantic import BaseModel, ConfigDict, Field, model_validator
+import datetime
+from typing import List, Optional, Protocol
+from uuid import UUID
 
-from catalystwan.models.common import check_fields_exclusive
-from catalystwan.models.policy.policy_list import PolicyListBase, PolicyListId, PolicyListInfo
+from pydantic import BaseModel, Field
 
+from catalystwan.models.policy import AnyPolicyList
+from catalystwan.typed_list import DataSequence
 
-class AppListEntry(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
 
-    app_family: Optional[str] = Field(default=None, serialization_alias="appFamily", validation_alias="appFamily")
-    app: Optional[str] = None
+class InfoTag(BaseModel):
+    info_tag: Optional[str] = Field("", alias="infoTag")
 
-    @model_validator(mode="after")
-    def check_app_xor_appfamily(self):
-        check_fields_exclusive(self.__dict__, {"app", "app_family"}, True)
-        return self
 
+class PolicyListId(BaseModel):
+    list_id: UUID = Field(alias="listId")
 
-class AppList(PolicyListBase):
-    type: Literal["app"] = "app"
-    entries: List[AppListEntry] = []
 
-    def add_app(self, app: str) -> None:
-        self._add_entry(AppListEntry(app=app))
+class PolicyListInfo(PolicyListId, InfoTag):
+    last_updated: datetime.datetime = Field(alias="lastUpdated")
+    owner: str
+    read_only: bool = Field(alias="readOnly")
+    version: str
+    reference_count: int = Field(alias="referenceCount")
+    references: List
+    is_activated_by_vsmart: Optional[bool] = Field(None, alias="isActivatedByVsmart")
 
-    def add_app_family(self, app_family: str) -> None:
-        self._add_entry(AppListEntry(app_family=app_family))
 
+class PolicyListPreview(BaseModel):
+    preview: str
 
-class AppListEditPayload(AppList, PolicyListId):
-    pass
 
+class PolicyListEndpoints(Protocol):
+    def create_policy_list(self, payload: AnyPolicyList) -> PolicyListId:
+        ...
 
-class AppListInfo(AppList, PolicyListInfo):
-    pass
+    def delete_policy_list(self, id: UUID) -> None:
+        ...
+
+    def edit_policy_list(self, id: UUID, payload: AnyPolicyList) -> None:
+        ...
+
+    def get_lists_by_id(self, id: UUID) -> PolicyListInfo:
+        ...
+
+    def get_policy_lists(self) -> DataSequence[PolicyListInfo]:
+        ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/localized.py` & `catalystwan-0.32.0/catalystwan/models/policy/localized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/policy.py` & `catalystwan-0.32.0/catalystwan/models/policy/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 import datetime
-from typing import List, Literal, Optional, Sequence, Union
+from typing import List, Literal, Optional, Sequence
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
 
 class PolicyId(BaseModel):
     policy_id: UUID = Field(serialization_alias="policyId", validation_alias="policyId")
@@ -43,18 +43,14 @@
     type: Literal["intrusionPrevention"] = "intrusionPrevention"
 
 
 class URLFilteringAssemblyItem(AssemblyItemBase):
     type: Literal["urlFiltering"] = "urlFiltering"
 
 
-class AdvancedInspectionProfileAssemblyItem(AssemblyItemBase):
-    type: Literal["advancedInspectionProfile"] = "advancedInspectionProfile"
-
-
 class AdvancedMalwareProtectionAssemblyItem(AssemblyItemBase):
     type: Literal["advancedMalwareProtection"] = "advancedMalwareProtection"
 
 
 class SSLDecryptionAssemblyItem(AssemblyItemBase):
     type: Literal["sslDecryption"] = "sslDecryption"
 
@@ -70,15 +66,15 @@
         pattern="^[a-zA-Z0-9_-]{1,127}$",
         description="Can include only alpha-numeric characters, hyphen '-' or underscore '_'; maximum 127 characters",
     )
     policy_description: str = Field(
         default="default description", serialization_alias="policyDescription", validation_alias="policyDescription"
     )
     policy_type: str = Field(serialization_alias="policyType", validation_alias="policyType")
-    policy_definition: Union[PolicyDefinition, str] = Field(
+    policy_definition: PolicyDefinition = Field(
         serialization_alias="policyDefinition", validation_alias="policyDefinition"
     )
     is_policy_activated: bool = Field(
         default=False, serialization_alias="isPolicyActivated", validation_alias="isPolicyActivated"
     )
     model_config = ConfigDict(populate_by_name=True)
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/policy/policy_definition.py` & `catalystwan-0.32.0/catalystwan/models/policy/policy_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 import datetime
 from functools import wraps
 from ipaddress import IPv4Address, IPv4Network, IPv6Network
-from typing import Any, Dict, List, MutableSequence, Optional, Sequence, Set, Tuple, Union
+from typing import Any, Dict, List, MutableSequence, Optional, Protocol, Sequence, Set, Tuple, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field, RootModel, field_validator, model_validator
+from pydantic import BaseModel, ConfigDict, Field, RootModel, model_validator
 from typing_extensions import Annotated, Literal
 
-from catalystwan.models.common import (
-    EncapType,
-    ICMPMessageType,
-    ServiceChainNumber,
-    TLOCColor,
-    check_fields_exclusive,
-    str_as_str_list,
-    str_as_uuid_list,
-)
+from catalystwan.models.common import ServiceChainNumber, TLOCColor, check_fields_exclusive
 from catalystwan.models.misc.application_protocols import ApplicationProtocol
+from catalystwan.models.policy.lists_entries import EncapType
+from catalystwan.typed_list import DataSequence
 
 
 def port_set_and_ranges_to_str(ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> str:
     assert ports or port_ranges
     ports_str = " ".join(f"{port_begin}-{port_end}" for port_begin, port_end in port_ranges)
     ports_str += " " if ports_str else ""
     ports_str += " ".join(str(p) for p in ports)
@@ -489,26 +483,17 @@
     @staticmethod
     def from_nat_vpn(fallback: bool, vpn: int = 0) -> "NATVPNEntry":
         if fallback:
             return NATVPNEntry(root=[UseVPNEntry(value=str(vpn)), FallBackEntry()])
         return NATVPNEntry(root=[UseVPNEntry(value=str(vpn))])
 
 
-class ICMPMessageEntry(BaseModel):
-    field: Literal["icmpMessage"] = "icmpMessage"
-    value: List[ICMPMessageType]
-
-    _value = field_validator("value", mode="before")(str_as_str_list)
-
-
 class SourceDataPrefixListEntry(BaseModel):
     field: Literal["sourceDataPrefixList"] = "sourceDataPrefixList"
-    ref: List[UUID]
-
-    _ref = field_validator("ref", mode="before")(str_as_uuid_list)
+    ref: UUID
 
 
 class SourceDataIPv6PrefixListEntry(BaseModel):
     field: Literal["sourceDataIpv6PrefixList"] = "sourceDataIpv6PrefixList"
     ref: UUID
 
 
@@ -528,19 +513,14 @@
 
 
 class AppListEntry(BaseModel):
     field: Literal["appList"] = "appList"
     ref: UUID
 
 
-class AppListFlatEntry(BaseModel):
-    field: Literal["appListFlat"] = "appListFlat"
-    ref: UUID
-
-
 class SourceFQDNListEntry(BaseModel):
     field: Literal["sourceFqdnList"] = "sourceFqdnList"
     ref: UUID
 
 
 class DestinationFQDNListEntry(BaseModel):
     field: Literal["destinationFqdnList"] = "destinationFqdnList"
@@ -768,24 +748,14 @@
 
 
 class PolicerAction(BaseModel):
     type: Literal["policer"] = "policer"
     parameter: Reference
 
 
-class ConnectionEventsAction(BaseModel):
-    type: Literal["connectionEvents"] = "connectionEvents"
-    parameter: str = ""
-
-
-class AdvancedInspectionProfileAction(BaseModel):
-    type: Literal["advancedInspectionProfile"] = "advancedInspectionProfile"
-    parameter: Reference
-
-
 ActionSetEntry = Annotated[
     Union[
         AffinityEntry,
         CommunityAdditiveEntry,
         CommunityEntry,
         DSCPEntry,
         ForwardingClassEntry,
@@ -812,18 +782,16 @@
     type: Literal["set"] = "set"
     parameter: List[ActionSetEntry] = []
 
 
 ActionEntry = Annotated[
     Union[
         ActionSet,
-        AdvancedInspectionProfileAction,
         CFlowDAction,
         ClassMapAction,
-        ConnectionEventsAction,
         CountAction,
         DREOptimizationAction,
         FallBackToRoutingAction,
         LogAction,
         LossProtectionAction,
         LossProtectionFECAction,
         LossProtectionPacketDuplicationAction,
@@ -838,15 +806,14 @@
     ],
     Field(discriminator="type"),
 ]
 
 MatchEntry = Annotated[
     Union[
         AppListEntry,
-        AppListFlatEntry,
         CarrierEntry,
         ClassMapListEntry,
         ColorListEntry,
         CommunityListEntry,
         DestinationDataIPv6PrefixListEntry,
         DestinationDataPrefixListEntry,
         DestinationFQDNEntry,
@@ -860,15 +827,14 @@
         DestinationRegionEntry,
         DNSAppListEntry,
         DNSEntry,
         DomainIDEntry,
         DSCPEntry,
         ExpandedCommunityListEntry,
         GroupIDEntry,
-        ICMPMessageEntry,
         NextHeaderEntry,
         OMPTagEntry,
         OriginatorEntry,
         OriginEntry,
         PacketLengthEntry,
         PathTypeEntry,
         PLPEntry,
@@ -941,17 +907,15 @@
 class PolicyDefinitionSequenceBase(BaseModel):
     sequence_id: int = Field(default=0, serialization_alias="sequenceId", validation_alias="sequenceId")
     sequence_name: str = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
     base_action: PolicyActionType = Field(
         default="drop", serialization_alias="baseAction", validation_alias="baseAction"
     )
     sequence_type: SequenceType = Field(serialization_alias="sequenceType", validation_alias="sequenceType")
-    sequence_ip_type: Optional[SequenceIpType] = Field(
-        default="ipv4", serialization_alias="sequenceIpType", validation_alias="sequenceIpType"
-    )
+    sequence_ip_type: SequenceIpType = Field(serialization_alias="sequenceIpType", validation_alias="sequenceIpType")
     ruleset: Optional[bool] = None
     match: Match
     actions: Sequence[ActionEntry]
 
     @staticmethod
     def _check_field_collision(field: str, fields: Sequence[str]) -> None:
         existing_fields = set(fields)
@@ -1141,7 +1105,24 @@
     master_templates_affected: List[str] = Field(
         default=[], serialization_alias="masterTemplatesAffected", validation_alias="masterTemplatesAffected"
     )
 
 
 class PolicyDefinitionPreview(BaseModel):
     preview: str
+
+
+class PolicyDefinitionEndpoints(Protocol):
+    def create_policy_definition(self, payload: BaseModel) -> PolicyDefinitionId:
+        ...
+
+    def delete_policy_definition(self, id: UUID) -> None:
+        ...
+
+    def edit_policy_definition(self, id: UUID, payload: BaseModel) -> PolicyDefinitionEditResponse:
+        ...
+
+    def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    def get_policy_definition(self, id: UUID) -> PolicyDefinitionGetResponse:
+        ...
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/models/tenant.py` & `catalystwan-0.32.0/catalystwan/models/tenant.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/response.py` & `catalystwan-0.32.0/catalystwan/response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/session.py` & `catalystwan-0.32.0/catalystwan/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,16 @@
                 "Cannot determine session type for "
                 f"tenancy-mode: {tenancy_mode}, user-mode: {user_mode}, view-mode: {view_mode}"
             )
 
         self.logger.info(
             f"Logged to vManage({self.platform_version}) as {self.username}. The session type is {self.session_type}"
         )
-        self.cookies.set("JSESSIONID", self.auth.set_cookie.get("JSESSIONID"))
+        if jsessionid := self.auth.set_cookie.get("JSESSIONID"):
+            self.cookies.set("JSESSIONID", jsessionid)
         return self
 
     def wait_server_ready(self, timeout: int, poll_period: int = 10) -> None:
         """Waits until server is ready for API requests with given timeout in seconds"""
 
         begin = monotonic()
         self.logger.info(f"Waiting for server ready with timeout {timeout} seconds.")
@@ -422,32 +423,43 @@
             Virtual session token
         """
         url_path = f"/dataservice/tenant/{tenant_id}/vsessionid"
         response = self.post(url_path)
         return response.json()["VSessionId"]
 
     def logout(self) -> Optional[ManagerResponse]:
+        response = None
         if isinstance((version := self.api_version), NullVersion):
             self.logger.warning("Cannot perform logout operation without known api_version.")
-            return None
+            return response
         else:
-            return self.post("/logout") if version >= Version("20.12") else self.get("/logout")
+            # disable automatic relogin before performing logout request
+            _relogin = self.enable_relogin
+            try:
+                self.enable_relogin = False
+                if version >= Version("20.12"):
+                    response = self.post("/logout")
+                else:
+                    response = self.get("/logout")
+            finally:
+                # restore original setting after performing logout request
+                self.enable_relogin = _relogin
+        return response
 
     def close(self) -> None:
         """Closes the ManagerSession.
 
         This method is overrided from requests.Session.
         Firstly it cleans up any resources associated with vManage.
         Then it closes all adapters and as such the session.
 
         Note: It is generally recommended to use the session as a context manager
         using the `with` statement, which ensures that the session is properly
         closed and resources are cleaned up even in case of exceptions.
         """
-        self.enable_relogin = False
         self.logout()
         super().close()
 
     def __prepare_session(self, verify: bool, auth: Optional[AuthBase]) -> None:
         self.auth = auth
         self.verify = verify
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/banner_1.json` & `catalystwan-0.32.0/catalystwan/tests/templates/definitions/banner_1.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/basic/children.json` & `catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/basic/children_nested.json` & `catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json` & `catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/cisco_bfd.json` & `catalystwan-0.32.0/catalystwan/tests/templates/definitions/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/complex_aaa.json` & `catalystwan-0.32.0/catalystwan/tests/templates/definitions/complex_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/complex_cisco_vpn.json` & `catalystwan-0.32.0/catalystwan/tests/templates/definitions/complex_cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/default_cisco_system.json` & `catalystwan-0.32.0/catalystwan/tests/templates/definitions/default_cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/iuo.json` & `catalystwan-0.32.0/catalystwan/tests/templates/definitions/iuo.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/omp_2.json` & `catalystwan-0.32.0/catalystwan/tests/templates/definitions/omp_2.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/definitions/omp_3.json` & `catalystwan-0.32.0/catalystwan/tests/templates/definitions/omp_3.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/__init__.py` & `catalystwan-0.32.0/catalystwan/tests/templates/models/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/cisco_aaa.py` & `catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/cisco_bfd.py` & `catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/cisco_vpn.py` & `catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/models/omp_vsmart.py` & `catalystwan-0.32.0/catalystwan/tests/templates/models/omp_vsmart.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/alias.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/alias.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/basic.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/basic.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/children.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/children_nested.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/basic/data_path.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/data_path.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/cedge_aaa.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/cedge_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/cisco_banner.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_banner.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/cisco_bfd.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/cisco_system.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/cisco_vpn.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/schemas/omp-vsmart.json` & `catalystwan-0.32.0/catalystwan/tests/templates/schemas/omp-vsmart.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/test_chose_model.py` & `catalystwan-0.32.0/catalystwan/tests/templates/test_chose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/test_deserialize_model.py` & `catalystwan-0.32.0/catalystwan/tests/templates/test_deserialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/test_generate_payload.py` & `catalystwan-0.32.0/catalystwan/tests/templates/test_generate_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/templates/test_serialize_model.py` & `catalystwan-0.32.0/catalystwan/tests/templates/test_serialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_admin_tech_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_administration.py` & `catalystwan-0.32.0/catalystwan/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_alarms_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_cli_template.py` & `catalystwan-0.32.0/catalystwan/tests/test_cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_creation_tools.py` & `catalystwan-0.32.0/catalystwan/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_device_action_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_devices_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_endpoints.py` & `catalystwan-0.32.0/catalystwan/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_feature_template_field.py` & `catalystwan-0.32.0/catalystwan/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_logs_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_monitoring_status_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_mtt_aaa_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_omp_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_packet_capture.py` & `catalystwan-0.32.0/catalystwan/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_partition_manager_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_response.py` & `catalystwan-0.32.0/catalystwan/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_session.py` & `catalystwan-0.32.0/catalystwan/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_software_action_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_speed_test_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_task_status_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_templates.py` & `catalystwan-0.32.0/catalystwan/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_tenant_backup_restore_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_tenant_management_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_tenant_migration_api.py` & `catalystwan-0.32.0/catalystwan/tests/test_tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_typed_list.py` & `catalystwan-0.32.0/catalystwan/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_version.py` & `catalystwan-0.32.0/catalystwan/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_version_utils.py` & `catalystwan-0.32.0/catalystwan/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/tests/test_vmanage_auth.py` & `catalystwan-0.32.0/catalystwan/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/typed_list.py` & `catalystwan-0.32.0/catalystwan/typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/utils/creation_tools.py` & `catalystwan-0.32.0/catalystwan/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/utils/dashboard.py` & `catalystwan-0.32.0/catalystwan/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/utils/device_model.py` & `catalystwan-0.32.0/catalystwan/utils/device_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/utils/dict.py` & `catalystwan-0.32.0/catalystwan/utils/dict.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/utils/feature_template/choose_model.py` & `catalystwan-0.32.0/catalystwan/utils/feature_template/choose_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
+
 from typing import Any
 
 from catalystwan.api.templates.models.supported import available_models
 from catalystwan.exceptions import TemplateTypeError
 
 
 def choose_model(type_value: str) -> Any:
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/utils/feature_template/find_template_values.py` & `catalystwan-0.32.0/catalystwan/utils/feature_template/find_template_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
+
 from typing import Any, Dict, List, Optional, Union
 
 from catalystwan.api.templates.device_variable import DeviceVariable
 
 
 def find_template_values(
     template_definition: dict,
```

### Comparing `catalystwan-0.31.2.dev2/catalystwan/utils/operation_status.py` & `catalystwan-0.32.0/catalystwan/utils/operation_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/utils/upgrades_helper.py` & `catalystwan-0.32.0/catalystwan/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/version.py` & `catalystwan-0.32.0/catalystwan/version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/vmanage_auth.py` & `catalystwan-0.32.0/catalystwan/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/catalystwan/workflows/tenant_migration.py` & `catalystwan-0.32.0/catalystwan/workflows/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.31.2.dev2/pyproject.toml` & `catalystwan-0.32.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "catalystwan"
-version = "0.31.2dev2"
+version = "0.32.0"
 description = "Cisco Catalyst WAN SDK for Python"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
-repository = "https://github.com/CiscoDevNet/catalystwan"
+repository = "https://github.com/cisco-open/cisco-catalyst-wan-sdk"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 requests = "^2.27.1"
 python-dateutil = "^2.8.2"
 attrs = "^21.4.0"
 ciscoconfparse = "1.9.41"
```

### Comparing `catalystwan-0.31.2.dev2/setup.py` & `catalystwan-0.32.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,53 +18,39 @@
  'catalystwan.endpoints.configuration.feature_profile.sdwan',
  'catalystwan.endpoints.configuration.policy',
  'catalystwan.endpoints.configuration.policy.definition',
  'catalystwan.endpoints.configuration.policy.list',
  'catalystwan.endpoints.real_time_monitoring',
  'catalystwan.endpoints.troubleshooting_tools',
  'catalystwan.integration_tests',
- 'catalystwan.integration_tests.feature_profile.sdwan.other',
- 'catalystwan.integration_tests.feature_profile.sdwan.service',
- 'catalystwan.integration_tests.feature_profile.sdwan.system',
  'catalystwan.models',
  'catalystwan.models.configuration',
  'catalystwan.models.configuration.feature_profile',
  'catalystwan.models.configuration.feature_profile.sdwan.management',
- 'catalystwan.models.configuration.feature_profile.sdwan.other',
  'catalystwan.models.configuration.feature_profile.sdwan.policy_object',
  'catalystwan.models.configuration.feature_profile.sdwan.policy_object.policy',
  'catalystwan.models.configuration.feature_profile.sdwan.policy_object.security',
  'catalystwan.models.configuration.feature_profile.sdwan.service',
  'catalystwan.models.configuration.feature_profile.sdwan.service.lan',
  'catalystwan.models.configuration.feature_profile.sdwan.system',
  'catalystwan.models.configuration.feature_profile.sdwan.transport',
  'catalystwan.models.misc',
  'catalystwan.models.policy',
- 'catalystwan.models.policy.definition',
- 'catalystwan.models.policy.list',
+ 'catalystwan.models.policy.definitions',
  'catalystwan.tests',
- 'catalystwan.tests.config_migration',
  'catalystwan.tests.templates',
  'catalystwan.tests.templates.models',
  'catalystwan.utils',
- 'catalystwan.utils.config_migration.converters.feature_template',
- 'catalystwan.utils.config_migration.converters.policy',
- 'catalystwan.utils.config_migration.creators',
- 'catalystwan.utils.config_migration.creators.strategy',
- 'catalystwan.utils.config_migration.device_templates',
- 'catalystwan.utils.config_migration.factories',
- 'catalystwan.utils.config_migration.reverters',
  'catalystwan.utils.feature_template',
  'catalystwan.workflows']
 
 package_data = \
 {'': ['*'],
  'catalystwan.api.templates.payloads.aaa': ['feature/*'],
  'catalystwan.api.templates.payloads.cisco_vpn': ['feature/*'],
- 'catalystwan.models.configuration': ['docs/*'],
  'catalystwan.tests.templates': ['definitions/*',
                                  'definitions/basic/*',
                                  'schemas/*',
                                  'schemas/basic/*']}
 
 install_requires = \
 ['Jinja2>=3.1.2,<4.0.0',
@@ -78,22 +64,22 @@
  'requests-toolbelt>=1.0.0,<2.0.0',
  'requests>=2.27.1,<3.0.0',
  'tenacity>=8.1.0,<9.0.0',
  'typing-extensions>=4.6.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'catalystwan',
-    'version': '0.31.2.dev2',
+    'version': '0.32.0',
     'description': 'Cisco Catalyst WAN SDK for Python',
-    'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any Manager.\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        orgName="CiscoDevNet",\n        subDomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edgeConnectorEnable=True,\n        edgeConnectorSystemIp="172.16.255.81",\n        edgeConnectorTunnelInterfaceName="GigabitEthernet1",\n        wanEdgeForecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/CiscoDevNet/catalystwan/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/catalystwan/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/CiscoDevNet/catalystwan/issues), or directly via mail on vmngclient@cisco.com.\n',
+    'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any Manager.\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        orgName="CiscoDevNet",\n        subDomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edgeConnectorEnable=True,\n        edgeConnectorSystemIp="172.16.255.81",\n        edgeConnectorTunnelInterfaceName="GigabitEthernet1",\n        wanEdgeForecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on vmngclient@cisco.com.\n',
     'author': 'kagorski',
     'author_email': 'kagorski@cisco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/CiscoDevNet/catalystwan',
+    'url': 'https://github.com/cisco-open/cisco-catalyst-wan-sdk',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8.0,<4.0.0',
 }
```

#### html2text {}

```diff
@@ -9,52 +9,40 @@
 'catalystwan.endpoints.configuration.device',
 'catalystwan.endpoints.configuration.feature_profile.sdwan',
 'catalystwan.endpoints.configuration.policy',
 'catalystwan.endpoints.configuration.policy.definition',
 'catalystwan.endpoints.configuration.policy.list',
 'catalystwan.endpoints.real_time_monitoring',
 'catalystwan.endpoints.troubleshooting_tools', 'catalystwan.integration_tests',
-'catalystwan.integration_tests.feature_profile.sdwan.other',
-'catalystwan.integration_tests.feature_profile.sdwan.service',
-'catalystwan.integration_tests.feature_profile.sdwan.system',
 'catalystwan.models', 'catalystwan.models.configuration',
 'catalystwan.models.configuration.feature_profile',
 'catalystwan.models.configuration.feature_profile.sdwan.management',
-'catalystwan.models.configuration.feature_profile.sdwan.other',
 'catalystwan.models.configuration.feature_profile.sdwan.policy_object',
 'catalystwan.models.configuration.feature_profile.sdwan.policy_object.policy',
 'catalystwan.models.configuration.feature_profile.sdwan.policy_object.security',
 'catalystwan.models.configuration.feature_profile.sdwan.service',
 'catalystwan.models.configuration.feature_profile.sdwan.service.lan',
 'catalystwan.models.configuration.feature_profile.sdwan.system',
 'catalystwan.models.configuration.feature_profile.sdwan.transport',
 'catalystwan.models.misc', 'catalystwan.models.policy',
-'catalystwan.models.policy.definition', 'catalystwan.models.policy.list',
-'catalystwan.tests', 'catalystwan.tests.config_migration',
+'catalystwan.models.policy.definitions', 'catalystwan.tests',
 'catalystwan.tests.templates', 'catalystwan.tests.templates.models',
-'catalystwan.utils',
-'catalystwan.utils.config_migration.converters.feature_template',
-'catalystwan.utils.config_migration.converters.policy',
-'catalystwan.utils.config_migration.creators',
-'catalystwan.utils.config_migration.creators.strategy',
-'catalystwan.utils.config_migration.device_templates',
-'catalystwan.utils.config_migration.factories',
-'catalystwan.utils.config_migration.reverters',
-'catalystwan.utils.feature_template', 'catalystwan.workflows'] package_data = \
-{'': ['*'], 'catalystwan.api.templates.payloads.aaa': ['feature/*'],
+'catalystwan.utils', 'catalystwan.utils.feature_template',
+'catalystwan.workflows'] package_data = \ {'': ['*'],
+'catalystwan.api.templates.payloads.aaa': ['feature/*'],
 'catalystwan.api.templates.payloads.cisco_vpn': ['feature/*'],
-'catalystwan.models.configuration': ['docs/*'], 'catalystwan.tests.templates':
-['definitions/*', 'definitions/basic/*', 'schemas/*', 'schemas/basic/*']}
-install_requires = \ ['Jinja2>=3.1.2,<4.0.0', 'attrs>=21.4.0,<22.0.0',
-'ciscoconfparse==1.9.41', 'clint>=0.5.1,<0.6.0', 'flake8-quotes>=3.3.1,<4.0.0',
-'packaging>=23.0,<24.0', 'pydantic>=2.5,<3.0', 'python-dateutil>=2.8.2,<3.0.0',
-'requests-toolbelt>=1.0.0,<2.0.0', 'requests>=2.27.1,<3.0.0',
-'tenacity>=8.1.0,<9.0.0', 'typing-extensions>=4.6.1,<5.0.0'] setup_kwargs =
-{ 'name': 'catalystwan', 'version': '0.31.2.dev2', 'description': 'Cisco
-Catalyst WAN SDK for Python', 'long_description': '
+'catalystwan.tests.templates': ['definitions/*', 'definitions/basic/*',
+'schemas/*', 'schemas/basic/*']} install_requires = \ ['Jinja2>=3.1.2,<4.0.0',
+'attrs>=21.4.0,<22.0.0', 'ciscoconfparse==1.9.41', 'clint>=0.5.1,<0.6.0',
+'flake8-quotes>=3.3.1,<4.0.0', 'packaging>=23.0,<24.0', 'pydantic>=2.5,<3.0',
+'python-dateutil>=2.8.2,<3.0.0', 'requests-toolbelt>=1.0.0,<2.0.0',
+'requests>=2.27.1,<3.0.0', 'tenacity>=8.1.0,<9.0.0', 'typing-
+extensions>=4.6.1,<5.0.0'] setup_kwargs = { 'name': 'catalystwan', 'version':
+'0.32.0', 'description': 'Cisco Catalyst WAN SDK for Python',
+'long_description': '
                       \n _[_C_i_s_c_o_ _C_a_t_a_l_y_s_t_ _W_A_N_ _S_D_K_ _L_o_g_o_]_\_n
 \n\n[![Python-Supported](https://img.shields.io/static/
 v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)]
 (https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating
 simple and parallel automatic requests via official Manager API. It is intended
 to serve as a multiple session handler (provider, provider as a tenant,
 tenant). The library is not dependent on environment which is being run in, you
@@ -210,17 +198,17 @@
 your scripts (warning is suppressed when `catalystwan_devel` environment
 variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings
 (urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching
 Exceptions\n```python\ntry:\n session.api.users.delete("bogus-user-
 name")\nexcept ManagerHTTPError as error:\n # Process an error.\n print
 (error.response.status_code)\n print(error.info.code)\n print
 (error.info.message)\n print(error.info.details)\n\n```\n\n## [Supported API
-endpoints](https://github.com/CiscoDevNet/catalystwan/blob/main/
+endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/
 ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https:
-//github.com/CiscoDevNet/catalystwan/blob/main/CONTRIBUTING.md)\n\n## Seeking
-support\n\nYou can contact us by submitting [issues](https://github.com/
-CiscoDevNet/catalystwan/issues), or directly via mail on
+//github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n##
+Seeking support\n\nYou can contact us by submitting [issues](https://
+github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on
 vmngclient@cisco.com.\n', 'author': 'kagorski', 'author_email':
 'kagorski@cisco.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://github.com/CiscoDevNet/catalystwan', 'packages': packages,
+'https://github.com/cisco-open/cisco-catalyst-wan-sdk', 'packages': packages,
 'package_data': package_data, 'install_requires': install_requires,
 'python_requires': '>=3.8.0,<4.0.0', } setup(**setup_kwargs)
```

### Comparing `catalystwan-0.31.2.dev2/PKG-INFO` & `catalystwan-0.32.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: catalystwan
-Version: 0.31.2.dev2
+Version: 0.32.0
 Summary: Cisco Catalyst WAN SDK for Python
-Home-page: https://github.com/CiscoDevNet/catalystwan
+Home-page: https://github.com/cisco-open/cisco-catalyst-wan-sdk
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pydantic (>=2.5,<3.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Requires-Dist: typing-extensions (>=4.6.1,<5.0.0)
-Project-URL: Repository, https://github.com/CiscoDevNet/catalystwan
+Project-URL: Repository, https://github.com/cisco-open/cisco-catalyst-wan-sdk
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />
 </p>
 
 [![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)
@@ -421,16 +421,16 @@
     print(error.response.status_code)
     print(error.info.code)
     print(error.info.message)
     print(error.info.details)
 
 ```
 
-## [Supported API endpoints](https://github.com/CiscoDevNet/catalystwan/blob/main/ENDPOINTS.md)
+## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)
 
 
-## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/catalystwan/blob/main/CONTRIBUTING.md)
+## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)
 
 ## Seeking support
 
-You can contact us by submitting [issues](https://github.com/CiscoDevNet/catalystwan/issues), or directly via mail on vmngclient@cisco.com.
+You can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on vmngclient@cisco.com.
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: catalystwan Version: 0.31.2.dev2 Summary: Cisco
-Catalyst WAN SDK for Python Home-page: https://github.com/CiscoDevNet/
-catalystwan Author: kagorski Author-email: kagorski@cisco.com Requires-Python:
+Metadata-Version: 2.1 Name: catalystwan Version: 0.32.0 Summary: Cisco Catalyst
+WAN SDK for Python Home-page: https://github.com/cisco-open/cisco-catalyst-wan-
+sdk Author: kagorski Author-email: kagorski@cisco.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: attrs (>=21.4.0,<22.0.0) Requires-Dist: ciscoconfparse
 (==1.9.41) Requires-Dist: clint (>=0.5.1,<0.6.0) Requires-Dist: flake8-quotes
 (>=3.3.1,<4.0.0) Requires-Dist: packaging (>=23.0,<24.0) Requires-Dist:
 pydantic (>=2.5,<3.0) Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-
 Dist: requests (>=2.27.1,<3.0.0) Requires-Dist: requests-toolbelt
 (>=1.0.0,<2.0.0) Requires-Dist: tenacity (>=8.1.0,<9.0.0) Requires-Dist:
 typing-extensions (>=4.6.1,<5.0.0) Project-URL: Repository, https://github.com/
-CiscoDevNet/catalystwan Description-Content-Type: text/markdown
+cisco-open/cisco-catalyst-wan-sdk Description-Content-Type: text/markdown
                          _[_C_i_s_c_o_ _C_a_t_a_l_y_s_t_ _W_A_N_ _S_D_K_ _L_o_g_o_]
 [![Python-Supported](https://img.shields.io/static/
 v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)]
 (https://www.python.org/) Cisco Catalyst WAN SDK is a package for creating
 simple and parallel automatic requests via official Manager API. It is intended
 to serve as a multiple session handler (provider, provider as a tenant,
 tenant). The library is not dependent on environment which is being run in, you
@@ -157,12 +157,12 @@
 (warning is suppressed when `catalystwan_devel` environment variable is set):
 ```Python import urllib3 urllib3.disable_warnings
 (urllib3.exceptions.InsecureRequestWarning) ``` ## Catching Exceptions
 ```python try: session.api.users.delete("bogus-user-name") except
 ManagerHTTPError as error: # Process an error. print
 (error.response.status_code) print(error.info.code) print(error.info.message)
 print(error.info.details) ``` ## [Supported API endpoints](https://github.com/
-CiscoDevNet/catalystwan/blob/main/ENDPOINTS.md) ## [Contributing, bug reporting
-and feature requests](https://github.com/CiscoDevNet/catalystwan/blob/main/
-CONTRIBUTING.md) ## Seeking support You can contact us by submitting [issues]
-(https://github.com/CiscoDevNet/catalystwan/issues), or directly via mail on
-vmngclient@cisco.com.
+cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md) ## [Contributing, bug
+reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-
+wan-sdk/blob/main/CONTRIBUTING.md) ## Seeking support You can contact us by
+submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/
+issues), or directly via mail on vmngclient@cisco.com.
```

