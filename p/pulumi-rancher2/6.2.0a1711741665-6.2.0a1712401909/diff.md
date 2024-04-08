# Comparing `tmp/pulumi_rancher2-6.2.0a1711741665.tar.gz` & `tmp/pulumi_rancher2-6.2.0a1712401909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rancher2-6.2.0a1711741665.tar", last modified: Fri Mar 29 20:06:14 2024, max compression
+gzip compressed data, was "pulumi_rancher2-6.2.0a1712401909.tar", last modified: Sat Apr  6 11:21:25 2024, max compression
```

## Comparing `pulumi_rancher2-6.2.0a1711741665.tar` & `pulumi_rancher2-6.2.0a1712401909.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:06:14.746788 pulumi_rancher2-6.2.0a1711741665/
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-03-29 20:06:14.746788 pulumi_rancher2-6.2.0a1711741665/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:06:14.746788 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1389755 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    41229 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    42239 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/app_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    81707 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_active_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_adfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35072 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    79388 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_free_ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    37584 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_okta.py
--rw-r--r--   0 runner    (1001) docker     (127)    79475 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_open_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    27436 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    32888 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    34833 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    45542 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)   167286 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    39652 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    24090 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    25641 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    31618 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    25340 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    62895 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:06:14.746788 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    20013 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    32449 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/custom_user_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    22341 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    25608 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_global_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_node_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_node_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_pod_security_admission_configuration_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_principal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_role_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/global_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    21643 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/global_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    47171 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/machine_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    41806 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/node_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    84187 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/node_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    34584 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)  1816679 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/pod_security_admission_configuration_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    69311 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    37937 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    37864 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    25746 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    31939 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/role_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    23036 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12524 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    24712 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:06:14.746788 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-03-29 20:06:14.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-03-29 20:06:14.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 20:06:14.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 20:06:14.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 20:06:14.000000 pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-29 20:06:03.000000 pulumi_rancher2-6.2.0a1711741665/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 20:06:14.746788 pulumi_rancher2-6.2.0a1711741665/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:21:25.463430 pulumi_rancher2-6.2.0a1712401909/
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-06 11:21:25.463430 pulumi_rancher2-6.2.0a1712401909/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:21:25.459430 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1391177 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41229 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42239 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/app_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81707 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_adfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35072 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79388 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_free_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37584 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79475 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_open_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27436 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32888 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34833 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45542 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167286 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39652 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24090 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25641 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31618 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25340 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62895 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:21:25.463430 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20013 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32449 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/custom_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22341 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25608 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_global_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_node_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_pod_security_admission_configuration_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_principal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_role_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/global_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21643 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/global_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47171 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/machine_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41806 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83735 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/node_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34584 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1818101 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/pod_security_admission_configuration_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69311 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37937 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37864 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25746 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31939 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/role_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23036 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12524 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24712 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:21:25.463430 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-06 11:21:25.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-06 11:21:25.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:21:25.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 11:21:25.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 11:21:25.000000 pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-06 11:21:18.000000 pulumi_rancher2-6.2.0a1712401909/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:21:25.463430 pulumi_rancher2-6.2.0a1712401909/setup.cfg
```

### Comparing `pulumi_rancher2-6.2.0a1711741665/PKG-INFO` & `pulumi_rancher2-6.2.0a1712401909/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 6.2.0a1711741665
+Version: 6.2.0a1712401909
 Summary: A Pulumi package for creating and managing rancher2 resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi,rancher2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rancher2-6.2.0a1711741665/README.md` & `pulumi_rancher2-6.2.0a1712401909/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/__init__.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/_inputs.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1947,15 +1947,15 @@
         :param pulumi.Input[str] name: The name of the Cluster (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] availability_zones: The AKS node pool availability zones (list)
         :param pulumi.Input[int] count: The AKS node pool count. Default: `1` (int)
         :param pulumi.Input[bool] enable_auto_scaling: Is AKS node pool auto scaling enabled? Default: `false` (bool)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster (map)
         :param pulumi.Input[int] max_count: The AKS node pool max count. Required if `enable_auto_scaling=true` (int)
         :param pulumi.Input[int] max_pods: The AKS node pool max pods. Default: `110` (int)
-        :param pulumi.Input[str] max_surge: The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        :param pulumi.Input[str] max_surge: The AKS node pool max surge (string), example value: `25%`
         :param pulumi.Input[int] min_count: The AKS node pool min count. Required if `enable_auto_scaling=true` (int)
         :param pulumi.Input[str] mode: The AKS node group mode. Default: `System` (string)
         :param pulumi.Input[str] orchestrator_version: The AKS node pool orchestrator version (string)
         :param pulumi.Input[int] os_disk_size_gb: The AKS node pool os disk size gb. Default: `128` (int)
         :param pulumi.Input[str] os_disk_type: The AKS node pool os disk type. Default: `Managed` (string)
         :param pulumi.Input[str] os_type: The AKS node pool os type. Default: `Linux` (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] taints: The GKE node config taints (List)
@@ -2077,15 +2077,15 @@
     def max_pods(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_pods", value)
 
     @property
     @pulumi.getter(name="maxSurge")
     def max_surge(self) -> Optional[pulumi.Input[str]]:
         """
-        The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        The AKS node pool max surge (string), example value: `25%`
         """
         return pulumi.get(self, "max_surge")
 
     @max_surge.setter
     def max_surge(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "max_surge", value)
 
@@ -9778,27 +9778,27 @@
 
 @pulumi.input_type
 class ClusterRkeConfigDnsUpdateStrategyRollingUpdateArgs:
     def __init__(__self__, *,
                  max_surge: Optional[pulumi.Input[int]] = None,
                  max_unavailable: Optional[pulumi.Input[int]] = None):
         """
-        :param pulumi.Input[int] max_surge: The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        :param pulumi.Input[int] max_surge: The AKS node pool max surge (string), example value: `25%`
         :param pulumi.Input[int] max_unavailable: Monitoring deployment rolling update max unavailable. Default: `1` (int)
         """
         if max_surge is not None:
             pulumi.set(__self__, "max_surge", max_surge)
         if max_unavailable is not None:
             pulumi.set(__self__, "max_unavailable", max_unavailable)
 
     @property
     @pulumi.getter(name="maxSurge")
     def max_surge(self) -> Optional[pulumi.Input[int]]:
         """
-        The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        The AKS node pool max surge (string), example value: `25%`
         """
         return pulumi.get(self, "max_surge")
 
     @max_surge.setter
     def max_surge(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_surge", value)
 
@@ -10376,27 +10376,27 @@
 
 @pulumi.input_type
 class ClusterRkeConfigMonitoringUpdateStrategyRollingUpdateArgs:
     def __init__(__self__, *,
                  max_surge: Optional[pulumi.Input[int]] = None,
                  max_unavailable: Optional[pulumi.Input[int]] = None):
         """
-        :param pulumi.Input[int] max_surge: The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        :param pulumi.Input[int] max_surge: The AKS node pool max surge (string), example value: `25%`
         :param pulumi.Input[int] max_unavailable: Monitoring deployment rolling update max unavailable. Default: `1` (int)
         """
         if max_surge is not None:
             pulumi.set(__self__, "max_surge", max_surge)
         if max_unavailable is not None:
             pulumi.set(__self__, "max_unavailable", max_unavailable)
 
     @property
     @pulumi.getter(name="maxSurge")
     def max_surge(self) -> Optional[pulumi.Input[int]]:
         """
-        The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        The AKS node pool max surge (string), example value: `25%`
         """
         return pulumi.get(self, "max_surge")
 
     @max_surge.setter
     def max_surge(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_surge", value)
 
@@ -13078,19 +13078,24 @@
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] configuration: Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
                
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
                ```
-               <!--End PulumiCodeChooser -->
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
+               ```
         :param pulumi.Input[str] name: The name of the Cluster (string)
         :param pulumi.Input[str] path: (Optional) Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -13099,19 +13104,24 @@
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input[str]]:
         """
         Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
         ```
-        <!--End PulumiCodeChooser -->
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
+        ```
         """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "configuration", value)
 
@@ -13144,37 +13154,47 @@
 class ClusterRkeConfigServicesKubeApiAuditLogArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs']] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs'] configuration: Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
                
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
                ```
-               <!--End PulumiCodeChooser -->
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
+               ```
         :param pulumi.Input[bool] enabled: Enable the authorized cluster endpoint. Default `true` (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs']]:
         """
         Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
         ```
-        <!--End PulumiCodeChooser -->
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
+        ```
         """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs']]):
         pulumi.set(self, "configuration", value)
 
@@ -13204,19 +13224,25 @@
         :param pulumi.Input[str] format: Audit log format. Default: 'json' (string)
         :param pulumi.Input[int] max_age: Audit log max age. Default: `30` (int)
         :param pulumi.Input[int] max_backup: Audit log max backup. Default: `10` (int)
         :param pulumi.Input[int] max_size: The EKS node group maximum size. Default `2` (int)
         :param pulumi.Input[str] path: (Optional) Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
         :param pulumi.Input[str] policy: Audit policy yaml encoded definition. `apiVersion` and `kind: Policy\\nrules:"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string) Ex:
                
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
                ```
-               <!--End PulumiCodeChooser -->
+               policy = <<EOF
+               apiVersion: audit.k8s.io/v1
+               kind: Policy
+               rules:
+               - level: RequestResponse
+               resources:
+               - resources:
+               - pods
+               EOF
+               ```
         """
         if format is not None:
             pulumi.set(__self__, "format", format)
         if max_age is not None:
             pulumi.set(__self__, "max_age", max_age)
         if max_backup is not None:
             pulumi.set(__self__, "max_backup", max_backup)
@@ -13289,19 +13315,25 @@
 
     @property
     @pulumi.getter
     def policy(self) -> Optional[pulumi.Input[str]]:
         """
         Audit policy yaml encoded definition. `apiVersion` and `kind: Policy\\nrules:"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string) Ex:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
         ```
-        <!--End PulumiCodeChooser -->
+        policy = <<EOF
+        apiVersion: audit.k8s.io/v1
+        kind: Policy
+        rules:
+        - level: RequestResponse
+        resources:
+        - resources:
+        - pods
+        EOF
+        ```
         """
         return pulumi.get(self, "policy")
 
     @policy.setter
     def policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "policy", value)
 
@@ -13310,37 +13342,47 @@
 class ClusterRkeConfigServicesKubeApiEventRateLimitArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[str] configuration: Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
                
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
                ```
-               <!--End PulumiCodeChooser -->
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
+               ```
         :param pulumi.Input[bool] enabled: Enable the authorized cluster endpoint. Default `true` (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input[str]]:
         """
         Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
         ```
-        <!--End PulumiCodeChooser -->
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
+        ```
         """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "configuration", value)
 
@@ -13361,37 +13403,59 @@
 class ClusterRkeConfigServicesKubeApiSecretsEncryptionConfigArgs:
     def __init__(__self__, *,
                  custom_config: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[str] custom_config: Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string) Ex:
                
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
                ```
-               <!--End PulumiCodeChooser -->
+               custom_config = <<EOF
+               apiVersion: apiserver.config.k8s.io/v1
+               kind: EncryptionConfiguration
+               resources:
+               - resources:
+               - secrets
+               providers:
+               - aescbc:
+               keys:
+               - name: k-fw5hn
+               secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=
+               identity: {}
+               EOF
+               
+               ```
         :param pulumi.Input[bool] enabled: Enable the authorized cluster endpoint. Default `true` (bool)
         """
         if custom_config is not None:
             pulumi.set(__self__, "custom_config", custom_config)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter(name="customConfig")
     def custom_config(self) -> Optional[pulumi.Input[str]]:
         """
         Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string) Ex:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
         ```
-        <!--End PulumiCodeChooser -->
+        custom_config = <<EOF
+        apiVersion: apiserver.config.k8s.io/v1
+        kind: EncryptionConfiguration
+        resources:
+        - resources:
+        - secrets
+        providers:
+        - aescbc:
+        keys:
+        - name: k-fw5hn
+        secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=
+        identity: {}
+        EOF
+
+        ```
         """
         return pulumi.get(self, "custom_config")
 
     @custom_config.setter
     def custom_config(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_config", value)
 
@@ -13811,15 +13875,15 @@
                  drain_input: Optional[pulumi.Input['ClusterRkeConfigUpgradeStrategyDrainInputArgs']] = None,
                  max_unavailable_controlplane: Optional[pulumi.Input[str]] = None,
                  max_unavailable_worker: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[bool] drain: RKE drain nodes. Default: `false` (bool)
         :param pulumi.Input['ClusterRkeConfigUpgradeStrategyDrainInputArgs'] drain_input: RKE drain node input (list Maxitems: 1)
         :param pulumi.Input[str] max_unavailable_controlplane: RKE max unavailable controlplane nodes. Default: `1` (string)
-        :param pulumi.Input[str] max_unavailable_worker: RKE max unavailable worker nodes. Default: `10%!`(MISSING) (string)
+        :param pulumi.Input[str] max_unavailable_worker: RKE max unavailable worker nodes. Default: `10%` (string)
         """
         if drain is not None:
             pulumi.set(__self__, "drain", drain)
         if drain_input is not None:
             pulumi.set(__self__, "drain_input", drain_input)
         if max_unavailable_controlplane is not None:
             pulumi.set(__self__, "max_unavailable_controlplane", max_unavailable_controlplane)
@@ -13862,15 +13926,15 @@
     def max_unavailable_controlplane(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "max_unavailable_controlplane", value)
 
     @property
     @pulumi.getter(name="maxUnavailableWorker")
     def max_unavailable_worker(self) -> Optional[pulumi.Input[str]]:
         """
-        RKE max unavailable worker nodes. Default: `10%!`(MISSING) (string)
+        RKE max unavailable worker nodes. Default: `10%` (string)
         """
         return pulumi.get(self, "max_unavailable_worker")
 
     @max_unavailable_worker.setter
     def max_unavailable_worker(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "max_unavailable_worker", value)
```

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/_utilities.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/app.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/app_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/app_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_active_directory.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_adfs.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_adfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_azure_ad.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_free_ipa.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_free_ipa.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_github.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_keycloak.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_keycloak.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_okta.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_open_ldap.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_open_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/auth_config_ping.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/auth_config_ping.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/bootstrap.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/catalog.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/catalog_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/certificate.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cloud_credential.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_alert_group.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_alert_rule.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_driver.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_role_template_binding.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_sync.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_sync.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_template.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/cluster_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/cluster_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/config/__init__.pyi` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/config/vars.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/config_map_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/custom_user_token.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/custom_user_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/etcd_backup.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/feature.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/feature.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_app.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_catalog.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_catalog_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_certificate.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cloud_credential.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_alert_group.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_alert_rule.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_driver.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_role_template_binding.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_template.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_cluster_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_cluster_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_config_map_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_etcd_backup.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_global_dns_provider.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_global_role.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_global_role_binding.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_multi_cluster_app.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_namespace.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_node_driver.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_node_pool.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_node_template.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_notifier.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_pod_security_admission_configuration_template.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_pod_security_admission_configuration_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_pod_security_policy_template.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_principal.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_principal.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_project.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_project_alert_group.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_project_alert_rule.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_project_role_template_binding.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_registry.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_role_template.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_secret.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_secret_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_setting.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_storage_class_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/get_user.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/global_dns.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/global_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/global_dns_provider.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/global_role.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/global_role_binding.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/machine_config_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/machine_config_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/multi_cluster_app.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/namespace.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/node_driver.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/node_pool.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/node_template.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/node_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1085,20 +1085,14 @@
         <!--End PulumiCodeChooser -->
 
         ## Upgrading to Rancher v2.3.3
 
         **Important** This process could update `NodeTemplate` data on tfstate file. Be sure to save a copy of tfstate file before proceed
 
         Due to [this feature](https://github.com/rancher/rancher/pull/23718) included on Rancher v2.3.3, `NodeTemplate` are now global scoped objects with RBAC around them, instead of user scoped objects as they were. This means that existing node templates `id` field is changing on upgrade. Provider implements `fixNodeTemplateID()` that will update tfstate with proper id.
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->sh
-        $ pulumi import rancher2:index/nodeTemplate:NodeTemplate foo &lt;node_template_id&gt;
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['NodeTemplateAmazonec2ConfigArgs']] amazonec2_config: AWS config for the Node Template (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for Node Template object (map)
         :param pulumi.Input[str] auth_certificate_authority: Auth certificate authority for the Node Template (string)
         :param pulumi.Input[str] auth_key: Auth key for the Node Template (string)
@@ -1269,20 +1263,14 @@
         <!--End PulumiCodeChooser -->
 
         ## Upgrading to Rancher v2.3.3
 
         **Important** This process could update `NodeTemplate` data on tfstate file. Be sure to save a copy of tfstate file before proceed
 
         Due to [this feature](https://github.com/rancher/rancher/pull/23718) included on Rancher v2.3.3, `NodeTemplate` are now global scoped objects with RBAC around them, instead of user scoped objects as they were. This means that existing node templates `id` field is changing on upgrade. Provider implements `fixNodeTemplateID()` that will update tfstate with proper id.
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->sh
-        $ pulumi import rancher2:index/nodeTemplate:NodeTemplate foo &lt;node_template_id&gt;
 
         :param str resource_name: The name of the resource.
         :param NodeTemplateArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/notifier.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/outputs.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2114,15 +2114,15 @@
         :param str name: The name of the Cluster (string)
         :param Sequence[str] availability_zones: The AKS node pool availability zones (list)
         :param int count: The AKS node pool count. Default: `1` (int)
         :param bool enable_auto_scaling: Is AKS node pool auto scaling enabled? Default: `false` (bool)
         :param Mapping[str, Any] labels: Labels for the Cluster (map)
         :param int max_count: The AKS node pool max count. Required if `enable_auto_scaling=true` (int)
         :param int max_pods: The AKS node pool max pods. Default: `110` (int)
-        :param str max_surge: The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        :param str max_surge: The AKS node pool max surge (string), example value: `25%`
         :param int min_count: The AKS node pool min count. Required if `enable_auto_scaling=true` (int)
         :param str mode: The AKS node group mode. Default: `System` (string)
         :param str orchestrator_version: The AKS node pool orchestrator version (string)
         :param int os_disk_size_gb: The AKS node pool os disk size gb. Default: `128` (int)
         :param str os_disk_type: The AKS node pool os disk type. Default: `Managed` (string)
         :param str os_type: The AKS node pool os type. Default: `Linux` (string)
         :param Sequence[str] taints: The GKE node config taints (List)
@@ -2216,15 +2216,15 @@
         """
         return pulumi.get(self, "max_pods")
 
     @property
     @pulumi.getter(name="maxSurge")
     def max_surge(self) -> Optional[str]:
         """
-        The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        The AKS node pool max surge (string), example value: `25%`
         """
         return pulumi.get(self, "max_surge")
 
     @property
     @pulumi.getter(name="minCount")
     def min_count(self) -> Optional[int]:
         """
@@ -9505,27 +9505,27 @@
         ClusterRkeConfigDnsUpdateStrategyRollingUpdate.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  max_surge: Optional[int] = None,
                  max_unavailable: Optional[int] = None):
         """
-        :param int max_surge: The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        :param int max_surge: The AKS node pool max surge (string), example value: `25%`
         :param int max_unavailable: Monitoring deployment rolling update max unavailable. Default: `1` (int)
         """
         if max_surge is not None:
             pulumi.set(__self__, "max_surge", max_surge)
         if max_unavailable is not None:
             pulumi.set(__self__, "max_unavailable", max_unavailable)
 
     @property
     @pulumi.getter(name="maxSurge")
     def max_surge(self) -> Optional[int]:
         """
-        The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        The AKS node pool max surge (string), example value: `25%`
         """
         return pulumi.get(self, "max_surge")
 
     @property
     @pulumi.getter(name="maxUnavailable")
     def max_unavailable(self) -> Optional[int]:
         """
@@ -10087,27 +10087,27 @@
         ClusterRkeConfigMonitoringUpdateStrategyRollingUpdate.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  max_surge: Optional[int] = None,
                  max_unavailable: Optional[int] = None):
         """
-        :param int max_surge: The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        :param int max_surge: The AKS node pool max surge (string), example value: `25%`
         :param int max_unavailable: Monitoring deployment rolling update max unavailable. Default: `1` (int)
         """
         if max_surge is not None:
             pulumi.set(__self__, "max_surge", max_surge)
         if max_unavailable is not None:
             pulumi.set(__self__, "max_unavailable", max_unavailable)
 
     @property
     @pulumi.getter(name="maxSurge")
     def max_surge(self) -> Optional[int]:
         """
-        The AKS node pool max surge (string), example value: `25%!`(MISSING)
+        The AKS node pool max surge (string), example value: `25%`
         """
         return pulumi.get(self, "max_surge")
 
     @property
     @pulumi.getter(name="maxUnavailable")
     def max_unavailable(self) -> Optional[int]:
         """
@@ -12545,19 +12545,24 @@
     def __init__(__self__, *,
                  configuration: Optional[str] = None,
                  name: Optional[str] = None,
                  path: Optional[str] = None):
         """
         :param str configuration: Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
                
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
                ```
-               <!--End PulumiCodeChooser -->
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
+               ```
         :param str name: The name of the Cluster (string)
         :param str path: (Optional) Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -12566,19 +12571,24 @@
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[str]:
         """
         Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
         ```
-        <!--End PulumiCodeChooser -->
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
+        ```
         """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -12599,37 +12609,47 @@
 class ClusterRkeConfigServicesKubeApiAuditLog(dict):
     def __init__(__self__, *,
                  configuration: Optional['outputs.ClusterRkeConfigServicesKubeApiAuditLogConfiguration'] = None,
                  enabled: Optional[bool] = None):
         """
         :param 'ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs' configuration: Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
                
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
                ```
-               <!--End PulumiCodeChooser -->
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
+               ```
         :param bool enabled: Enable the authorized cluster endpoint. Default `true` (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional['outputs.ClusterRkeConfigServicesKubeApiAuditLogConfiguration']:
         """
         Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
         ```
-        <!--End PulumiCodeChooser -->
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
+        ```
         """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
@@ -12672,19 +12692,25 @@
         :param str format: Audit log format. Default: 'json' (string)
         :param int max_age: Audit log max age. Default: `30` (int)
         :param int max_backup: Audit log max backup. Default: `10` (int)
         :param int max_size: The EKS node group maximum size. Default `2` (int)
         :param str path: (Optional) Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
         :param str policy: Audit policy yaml encoded definition. `apiVersion` and `kind: Policy\\nrules:"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string) Ex:
                
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
                ```
-               <!--End PulumiCodeChooser -->
+               policy = <<EOF
+               apiVersion: audit.k8s.io/v1
+               kind: Policy
+               rules:
+               - level: RequestResponse
+               resources:
+               - resources:
+               - pods
+               EOF
+               ```
         """
         if format is not None:
             pulumi.set(__self__, "format", format)
         if max_age is not None:
             pulumi.set(__self__, "max_age", max_age)
         if max_backup is not None:
             pulumi.set(__self__, "max_backup", max_backup)
@@ -12737,54 +12763,70 @@
 
     @property
     @pulumi.getter
     def policy(self) -> Optional[str]:
         """
         Audit policy yaml encoded definition. `apiVersion` and `kind: Policy\\nrules:"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string) Ex:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
         ```
-        <!--End PulumiCodeChooser -->
+        policy = <<EOF
+        apiVersion: audit.k8s.io/v1
+        kind: Policy
+        rules:
+        - level: RequestResponse
+        resources:
+        - resources:
+        - pods
+        EOF
+        ```
         """
         return pulumi.get(self, "policy")
 
 
 @pulumi.output_type
 class ClusterRkeConfigServicesKubeApiEventRateLimit(dict):
     def __init__(__self__, *,
                  configuration: Optional[str] = None,
                  enabled: Optional[bool] = None):
         """
         :param str configuration: Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
                
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
                ```
-               <!--End PulumiCodeChooser -->
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
+               ```
         :param bool enabled: Enable the authorized cluster endpoint. Default `true` (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[str]:
         """
         Event rate limit configuration yaml encoded definition. `apiVersion` and `kind: Configuration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string) Ex:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
         ```
-        <!--End PulumiCodeChooser -->
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
+        ```
         """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
@@ -12814,37 +12856,59 @@
 
     def __init__(__self__, *,
                  custom_config: Optional[str] = None,
                  enabled: Optional[bool] = None):
         """
         :param str custom_config: Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string) Ex:
                
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
                ```
-               <!--End PulumiCodeChooser -->
+               custom_config = <<EOF
+               apiVersion: apiserver.config.k8s.io/v1
+               kind: EncryptionConfiguration
+               resources:
+               - resources:
+               - secrets
+               providers:
+               - aescbc:
+               keys:
+               - name: k-fw5hn
+               secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=
+               identity: {}
+               EOF
+               
+               ```
         :param bool enabled: Enable the authorized cluster endpoint. Default `true` (bool)
         """
         if custom_config is not None:
             pulumi.set(__self__, "custom_config", custom_config)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter(name="customConfig")
     def custom_config(self) -> Optional[str]:
         """
         Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string) Ex:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
         ```
-        <!--End PulumiCodeChooser -->
+        custom_config = <<EOF
+        apiVersion: apiserver.config.k8s.io/v1
+        kind: EncryptionConfiguration
+        resources:
+        - resources:
+        - secrets
+        providers:
+        - aescbc:
+        keys:
+        - name: k-fw5hn
+        secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=
+        identity: {}
+        EOF
+
+        ```
         """
         return pulumi.get(self, "custom_config")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
@@ -13283,15 +13347,15 @@
                  drain_input: Optional['outputs.ClusterRkeConfigUpgradeStrategyDrainInput'] = None,
                  max_unavailable_controlplane: Optional[str] = None,
                  max_unavailable_worker: Optional[str] = None):
         """
         :param bool drain: RKE drain nodes. Default: `false` (bool)
         :param 'ClusterRkeConfigUpgradeStrategyDrainInputArgs' drain_input: RKE drain node input (list Maxitems: 1)
         :param str max_unavailable_controlplane: RKE max unavailable controlplane nodes. Default: `1` (string)
-        :param str max_unavailable_worker: RKE max unavailable worker nodes. Default: `10%!`(MISSING) (string)
+        :param str max_unavailable_worker: RKE max unavailable worker nodes. Default: `10%` (string)
         """
         if drain is not None:
             pulumi.set(__self__, "drain", drain)
         if drain_input is not None:
             pulumi.set(__self__, "drain_input", drain_input)
         if max_unavailable_controlplane is not None:
             pulumi.set(__self__, "max_unavailable_controlplane", max_unavailable_controlplane)
@@ -13322,15 +13386,15 @@
         """
         return pulumi.get(self, "max_unavailable_controlplane")
 
     @property
     @pulumi.getter(name="maxUnavailableWorker")
     def max_unavailable_worker(self) -> Optional[str]:
         """
-        RKE max unavailable worker nodes. Default: `10%!`(MISSING) (string)
+        RKE max unavailable worker nodes. Default: `10%` (string)
         """
         return pulumi.get(self, "max_unavailable_worker")
 
 
 @pulumi.output_type
 class ClusterRkeConfigUpgradeStrategyDrainInput(dict):
     @staticmethod
```

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/pod_security_admission_configuration_template.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/pod_security_admission_configuration_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/pod_security_policy_template.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/project.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/project_alert_group.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/project_alert_rule.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/project_role_template_binding.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/provider.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/registry.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/role_template.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/secret.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/secret_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/setting.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/storage_class_v2.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/token.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2/user.py` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2.egg-info/PKG-INFO` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 6.2.0a1711741665
+Version: 6.2.0a1712401909
 Summary: A Pulumi package for creating and managing rancher2 resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi,rancher2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rancher2-6.2.0a1711741665/pulumi_rancher2.egg-info/SOURCES.txt` & `pulumi_rancher2-6.2.0a1712401909/pulumi_rancher2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1711741665/pyproject.toml` & `pulumi_rancher2-6.2.0a1712401909/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_rancher2"
   description = "A Pulumi package for creating and managing rancher2 resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "rancher2"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "6.2.0a1711741665"
+  version = "6.2.0a1712401909"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-rancher2"
 
 [build-system]
```

