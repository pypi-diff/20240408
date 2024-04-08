# Comparing `tmp/smol_k8s_lab-3.7.1.tar.gz` & `tmp/smol_k8s_lab-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smol_k8s_lab-3.7.1.tar", max compression
+gzip compressed data, was "smol_k8s_lab-4.0.0.tar", max compression
```

## Comparing `smol_k8s_lab-3.7.1.tar` & `smol_k8s_lab-4.0.0.tar`

### file list

```diff
@@ -1,107 +1,109 @@
--rw-r--r--   0        0        0    34260 2024-03-31 10:43:21.273501 smol_k8s_lab-3.7.1/LICENSE
--rw-r--r--   0        0        0    24729 2024-03-31 10:43:21.273501 smol_k8s_lab-3.7.1/README.md
--rw-r--r--   0        0        0     2266 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/pyproject.toml
--rwxr-xr-x   0        0        0    14992 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/__init__.py
--rwxr-xr-x   0        0        0    12779 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/bw_cli.py
--rw-r--r--   0        0        0     1679 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/tui/bitwarden.css
--rw-r--r--   0        0        0     2093 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
--rw-r--r--   0        0        0     4524 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
--rw-r--r--   0        0        0     2395 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
--rw-r--r--   0        0        0     6916 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
--rw-r--r--   0        0        0    61688 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/config/default_config.yaml
--rw-r--r--   0        0        0     5675 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/config/keycloak_config.json
--rw-r--r--   0        0        0      237 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/config/kind/kind-config-cilium.yaml
--rw-r--r--   0        0        0      385 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/config/kind/kind_cluster_config.yaml
--rwxr-xr-x   0        0        0     2318 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/constants.py
--rwxr-xr-x   0        0        0    12945 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/env_config.py
--rw-r--r--   0        0        0     9105 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/__init__.py
--rw-r--r--   0        0        0     5861 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/argocd.py
--rw-r--r--   0        0        0        0 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
--rw-r--r--   0        0        0     6716 2024-03-31 10:43:21.521501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
--rw-r--r--   0        0        0    10293 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
--rw-r--r--   0        0        0    14554 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
--rw-r--r--   0        0        0    20053 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
--rw-r--r--   0        0        0     3370 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
--rw-r--r--   0        0        0     1860 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
--rw-r--r--   0        0        0     9134 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/initial_special.py
--rw-r--r--   0        0        0        0 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/networking/__init__.py
--rw-r--r--   0        0        0     1761 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/networking/cilium.py
--rw-r--r--   0        0        0     2318 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/networking/metallb.py
--rw-r--r--   0        0        0    11178 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/networking/netmaker.py
--rw-r--r--   0        0        0     2107 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/__init__.py
--rw-r--r--   0        0        0      591 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/k8up_operater.py
--rw-r--r--   0        0        0      573 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/longhorn.py
--rw-r--r--   0        0        0    16270 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/minio.py
--rw-r--r--   0        0        0     4471 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
--rw-r--r--   0        0        0     4590 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
--rw-r--r--   0        0        0        0 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
--rw-r--r--   0        0        0     2671 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
--rw-r--r--   0        0        0     3889 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
--rw-r--r--   0        0        0     5089 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/secrets_management/vault.py
--rw-r--r--   0        0        0    15769 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/social/mastodon.py
--rwxr-xr-x   0        0        0     1702 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
--rw-r--r--   0        0        0    12253 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/social/matrix.py
--rw-r--r--   0        0        0    13293 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/social/nextcloud.py
--rwxr-xr-x   0        0        0     4129 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
--rw-r--r--   0        0        0     6497 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_distros/__init__.py
--rw-r--r--   0        0        0     3751 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_distros/k3d.py
--rw-r--r--   0        0        0     7779 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_distros/k3s.py
--rw-r--r--   0        0        0     4817 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_distros/kind.py
--rw-r--r--   0        0        0        1 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_tools/__init__.py
--rw-r--r--   0        0        0     5548 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_tools/argocd_util.py
--rwxr-xr-x   0        0        0     8032 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_tools/helm.py
--rw-r--r--   0        0        0    10312 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_tools/k8s_lib.py
--rw-r--r--   0        0        0      219 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_tools/k9s.py
--rw-r--r--   0        0        0     1358 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/__init__.py
--rw-r--r--   0        0        0    10866 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
--rw-r--r--   0        0        0     7501 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
--rw-r--r--   0        0        0     6827 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/input_widgets.py
--rwxr-xr-x   0        0        0     3533 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/invalid_apps.py
--rw-r--r--   0        0        0     6904 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/modify_globals.py
--rw-r--r--   0        0        0     3763 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/new_app_modal.py
--rwxr-xr-x   0        0        0    10680 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/apps_screen.py
--rw-r--r--   0        0        0    21462 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/base.py
--rw-r--r--   0        0        0     6151 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/base_cluster_modal.py
--rwxr-xr-x   0        0        0     8373 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/confirm_screen.py
--rw-r--r--   0        0        0      925 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/add_nodes_widget.tcss
--rw-r--r--   0        0        0     6076 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/apps_config.tcss
--rw-r--r--   0        0        0     1561 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/apps_init_config.tcss
--rw-r--r--   0        0        0     6386 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/base.tcss
--rw-r--r--   0        0        0      988 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/base_modal.tcss
--rw-r--r--   0        0        0     1116 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/cluster_modal.tcss
--rw-r--r--   0        0        0     1278 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/confirm.tcss
--rw-r--r--   0        0        0     1564 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/distro_config.tcss
--rw-r--r--   0        0        0      867 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/help.tcss
--rw-r--r--   0        0        0      855 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/invalid_apps.tcss
--rw-r--r--   0        0        0     1940 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/k3s.tcss
--rw-r--r--   0        0        0     1720 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/kind.tcss
--rw-r--r--   0        0        0     1247 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/modify_globals_modal.tcss
--rw-r--r--   0        0        0      770 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/new_app_modal.tcss
--rw-r--r--   0        0        0      112 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/new_option_modal.tcss
--rw-r--r--   0        0        0     1168 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/node_inputs_widget.tcss
--rw-r--r--   0        0        0     1101 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/node_modal.tcss
--rw-r--r--   0        0        0     3096 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
--rw-r--r--   0        0        0     2683 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/tui_config.tcss
--rwxr-xr-x   0        0        0    10237 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_screen.py
--rw-r--r--   0        0        0        0 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/__init__.py
--rw-r--r--   0        0        0    11500 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/add_nodes.py
--rw-r--r--   0        0        0    13289 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/k3s_config.py
--rw-r--r--   0        0        0     6754 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/kind_config.py
--rw-r--r--   0        0        0     6060 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
--rw-r--r--   0        0        0     4509 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
--rw-r--r--   0        0        0     4669 2024-03-31 10:43:21.525501 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
--rw-r--r--   0        0        0     4210 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/help_screen.py
--rwxr-xr-x   0        0        0     3733 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/make_screenshots.py
--rwxr-xr-x   0        0        0     7714 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/smol_k8s_config_screen.py
--rwxr-xr-x   0        0        0    10049 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/tui_config_screen.py
--rw-r--r--   0        0        0     9388 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/util.py
--rw-r--r--   0        0        0        0 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/validators/__init__.py
--rw-r--r--   0        0        0      579 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/tui/validators/already_exists.py
--rw-r--r--   0        0        0        0 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/utils/__init__.py
--rw-r--r--   0        0        0     1184 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/utils/passwords.py
--rwxr-xr-x   0        0        0     2423 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/utils/rich_cli/console_logging.py
--rwxr-xr-x   0        0        0     4624 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/utils/rich_cli/help_text.py
--rwxr-xr-x   0        0        0     7215 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/utils/subproc.py
--rw-r--r--   0        0        0      315 2024-03-31 10:43:21.529502 smol_k8s_lab-3.7.1/smol_k8s_lab/utils/yaml_with_comments.py
--rw-r--r--   0        0        0    26375 1970-01-01 00:00:00.000000 smol_k8s_lab-3.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-04-08 12:51:25.226617 smol_k8s_lab-4.0.0/LICENSE
+-rw-r--r--   0        0        0    27169 2024-04-08 12:51:25.226617 smol_k8s_lab-4.0.0/README.md
+-rw-r--r--   0        0        0     2266 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0    15143 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/__init__.py
+-rwxr-xr-x   0        0        0    12779 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/bw_cli.py
+-rw-r--r--   0        0        0     1679 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden.css
+-rw-r--r--   0        0        0     2093 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
+-rw-r--r--   0        0        0     4524 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
+-rw-r--r--   0        0        0     2395 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
+-rw-r--r--   0        0        0     6916 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
+-rw-r--r--   0        0        0    64187 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/config/default_config.yaml
+-rw-r--r--   0        0        0     5675 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/config/keycloak_config.json
+-rw-r--r--   0        0        0      237 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/config/kind/kind-config-cilium.yaml
+-rw-r--r--   0        0        0      385 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/config/kind/kind_cluster_config.yaml
+-rwxr-xr-x   0        0        0     2318 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/constants.py
+-rwxr-xr-x   0        0        0    12945 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/env_config.py
+-rw-r--r--   0        0        0     9486 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/argocd.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
+-rw-r--r--   0        0        0     6716 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
+-rw-r--r--   0        0        0    10293 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
+-rw-r--r--   0        0        0    14554 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
+-rw-r--r--   0        0        0    20412 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
+-rw-r--r--   0        0        0     3370 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
+-rw-r--r--   0        0        0     1860 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
+-rw-r--r--   0        0        0     9134 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/initial_special.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/__init__.py
+-rw-r--r--   0        0        0     1761 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/cilium.py
+-rw-r--r--   0        0        0     2318 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/metallb.py
+-rw-r--r--   0        0        0    11178 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/netmaker.py
+-rw-r--r--   0        0        0     2543 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/__init__.py
+-rw-r--r--   0        0        0      591 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/k8up_operater.py
+-rw-r--r--   0        0        0      573 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/longhorn.py
+-rw-r--r--   0        0        0    16270 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/minio.py
+-rw-r--r--   0        0        0     4471 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
+-rw-r--r--   0        0        0      520 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/prometheus.py
+-rw-r--r--   0        0        0     4590 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
+-rw-r--r--   0        0        0     2671 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
+-rw-r--r--   0        0        0     3889 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
+-rw-r--r--   0        0        0     5089 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py
+-rw-r--r--   0        0        0     4974 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/home_assistant.py
+-rw-r--r--   0        0        0    15769 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/mastodon.py
+-rwxr-xr-x   0        0        0     1702 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
+-rw-r--r--   0        0        0    12253 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/matrix.py
+-rw-r--r--   0        0        0    13293 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/nextcloud.py
+-rwxr-xr-x   0        0        0     4129 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
+-rw-r--r--   0        0        0     6497 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/__init__.py
+-rw-r--r--   0        0        0     3751 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/k3d.py
+-rw-r--r--   0        0        0     7779 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/k3s.py
+-rw-r--r--   0        0        0     4817 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/kind.py
+-rw-r--r--   0        0        0        1 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/__init__.py
+-rw-r--r--   0        0        0     5548 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/argocd_util.py
+-rwxr-xr-x   0        0        0     8032 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/helm.py
+-rw-r--r--   0        0        0    10312 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/k8s_lib.py
+-rw-r--r--   0        0        0      219 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/k9s.py
+-rw-r--r--   0        0        0     1358 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/__init__.py
+-rw-r--r--   0        0        0    10866 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
+-rw-r--r--   0        0        0     7501 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
+-rw-r--r--   0        0        0     6827 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/input_widgets.py
+-rwxr-xr-x   0        0        0     3533 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py
+-rw-r--r--   0        0        0     6904 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/modify_globals.py
+-rw-r--r--   0        0        0     3763 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py
+-rwxr-xr-x   0        0        0    10680 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/apps_screen.py
+-rw-r--r--   0        0        0    21507 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/base.py
+-rw-r--r--   0        0        0     6151 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/base_cluster_modal.py
+-rwxr-xr-x   0        0        0     8373 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/confirm_screen.py
+-rw-r--r--   0        0        0      925 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss
+-rw-r--r--   0        0        0     6076 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/apps_config.tcss
+-rw-r--r--   0        0        0     1561 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/apps_init_config.tcss
+-rw-r--r--   0        0        0     6386 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/base.tcss
+-rw-r--r--   0        0        0      988 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/base_modal.tcss
+-rw-r--r--   0        0        0     1116 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/cluster_modal.tcss
+-rw-r--r--   0        0        0     1278 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/confirm.tcss
+-rw-r--r--   0        0        0     1564 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/distro_config.tcss
+-rw-r--r--   0        0        0      867 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/help.tcss
+-rw-r--r--   0        0        0      855 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/invalid_apps.tcss
+-rw-r--r--   0        0        0     1940 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/k3s.tcss
+-rw-r--r--   0        0        0     1720 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/kind.tcss
+-rw-r--r--   0        0        0     1247 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss
+-rw-r--r--   0        0        0      770 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/new_app_modal.tcss
+-rw-r--r--   0        0        0      112 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/new_option_modal.tcss
+-rw-r--r--   0        0        0     1168 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss
+-rw-r--r--   0        0        0     1101 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/node_modal.tcss
+-rw-r--r--   0        0        0     3096 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
+-rw-r--r--   0        0        0     2683 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/tui_config.tcss
+-rwxr-xr-x   0        0        0    10237 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_screen.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/__init__.py
+-rw-r--r--   0        0        0    11500 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py
+-rw-r--r--   0        0        0    13289 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py
+-rw-r--r--   0        0        0     6754 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/kind_config.py
+-rw-r--r--   0        0        0     6060 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
+-rw-r--r--   0        0        0     4509 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
+-rw-r--r--   0        0        0     4669 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
+-rw-r--r--   0        0        0     4210 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/help_screen.py
+-rwxr-xr-x   0        0        0     3733 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/make_screenshots.py
+-rwxr-xr-x   0        0        0     7714 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/smol_k8s_config_screen.py
+-rwxr-xr-x   0        0        0    10049 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/tui_config_screen.py
+-rw-r--r--   0        0        0     9388 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/util.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/validators/__init__.py
+-rw-r--r--   0        0        0      579 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/validators/already_exists.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/__init__.py
+-rw-r--r--   0        0        0     1184 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/passwords.py
+-rwxr-xr-x   0        0        0     2423 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/rich_cli/console_logging.py
+-rwxr-xr-x   0        0        0     4624 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/rich_cli/help_text.py
+-rwxr-xr-x   0        0        0     7215 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/subproc.py
+-rw-r--r--   0        0        0      315 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/yaml_with_comments.py
+-rw-r--r--   0        0        0    28815 1970-01-01 00:00:00.000000 smol_k8s_lab-4.0.0/PKG-INFO
```

### Comparing `smol_k8s_lab-3.7.1/LICENSE` & `smol_k8s_lab-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/README.md` & `smol_k8s_lab-4.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   />
  🧸 <code>smol-k8s-lab</code>
   <a href="https://github.com/small-hack/smol-k8s-lab/releases">
     <img src="https://img.shields.io/github/v/release/small-hack/smol-k8s-lab?style=plastic&labelColor=484848&color=3CA324&logo=GitHub&logoColor=white">
   </a>
 </h2>
 <p align="center">
-  A terminal based tool to install slimmer k8s distros on metal, with batteries included! 
+  A terminal based tool to install slimmer k8s distros on metal, with batteries included!
 </p>
 
 <p align="center">
   <a href="https://www.youtube.com/watch?v=UdOQM9n5hyU&t=0s">
     <img width="800" alt="Screenshot of smol-k8s-lab (on the welcome screen) in a video tutorial on youtube. please click this image, as it is a link to youtube where I explain everything about smol-k8s-lab. The video image screenshot shows the smol-k8s-lab create a cluster feature which is a text input" src="https://github.com/small-hack/smol-k8s-lab/assets/2389292/ee0ca93b-628e-495f-83ab-70aa9eb52295">
   </a><br>
   <sup>(Here's the <a href="https://youtu.be/2E9DVJpv440?feature=shared">same video with captions)</a></sup>
@@ -69,19 +69,85 @@
 
 ## Usage
 
 ### Initialization
 After you've followed the installation instructions, if you're *new* to `smol-k8s-lab`,  initialize a new config file:
 
 ```bash
-# we'll walk you through any configuration needed before 
+# we'll walk you through any configuration needed before
 # saving the config and deploying it for you
 smol-k8s-lab
 ```
 <details>
+  <summary><b>Upgrading config from v3.7.1 to v4.x</b></summary>
+
+If you've installed smol-k8s-lab prior to `v4.0.0`, please backup your old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the following with either pip or pipx:
+
+*if using pip*:
+```yaml
+# this upgrades smol-k8s-lab
+pip3.11 install --upgrade smol-k8s-lab
+
+# this initializes a new configuration
+smol-k8s-lab
+```
+
+*or if using pipx*:
+```yaml
+# this upgrades smol-k8s-lab
+pipx upgrade smol-k8s-lab
+
+# this initializes a new configuration
+smol-k8s-lab
+```
+
+The main breaking changes between `v3.7.1` and `v4.0.0` are that we now default enable metrics on most apps. Because of this, you need to have the Prometheus ServiceMonitor CRD installed ahead of time. Luckily, we now provide that as an app as well :) If you deleted your config and created a new one, it will already be there, but if you want to reuse your old config, you can add the app like this:
+
+```yaml
+apps:
+  prometheus_crds:
+    description: |
+      [link=https://prometheus.io/docs/introduction/overview/]Prometheus[/link] CRDs to start with.
+      You can optionally disable this if you don't want to deploy apps with metrics.
+
+    enabled: true
+    argo:
+      # secrets keys to make available to Argo CD ApplicationSets
+      secret_keys: {}
+      # git repo to install the Argo CD app from
+      repo: https://github.com/small-hack/argocd-apps
+      # path in the argo repo to point to. Trailing slash very important!
+      path: prometheus/crds/
+      # either the branch or tag to point at in the argo repo above
+      revision: main
+      # namespace to install the k8s app in
+      namespace: prometheus
+      # recurse directories in the provided git repo
+      directory_recursion: false
+      # source repos for Argo CD App Project (in addition to argo.repo)
+      project:
+        name: prometheus
+        source_repos:
+        - https://github.com/prometheus-community/helm-charts.git
+        destination:
+          # automatically includes the app's namespace and argocd's namespace
+          namespaces:
+          - kube-system
+          - prometheus
+```
+
+If using the default repos, please also disable directory directory_recursion for:
+- your prometheus stack app
+- zitadel
+
+For all changes, please check out [PR #206](https://github.com/small-hack/smol-k8s-lab/pull/206).
+
+</details>
+
+<details>
   <summary><b>Upgrading config from v2.2.4 to v3.x</b></summary>
 
 If you've installed smol-k8s-lab prior to `v3.0.0`, please backup your old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the following with either pip or pipx:
 
 *if using pip*:
 ```yaml
 # this upgrades smol-k8s-lab
```

#### html2text {}

```diff
@@ -37,25 +37,54 @@
  _[_O_u_t_p_u_t_ _o_f_ _s_m_o_l_-_k_8_s_-_l_a_b_ _-_-_h_e_l_p_ _a_f_t_e_r_ _c_l_o_n_i_n_g_ _t_h_e_ _d_i_r_e_c_t_o_r_y_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g_ _t_h_e
                                 _p_r_e_r_e_q_u_i_s_i_t_e_s_._]
 Checkout our [TUI docs](https://small-hack.github.io/smol-k8s-lab/tui/
 create_modify_screens/) for more info on how to get started playing with `smol-
 k8s-lab` :-) ## Usage ### Initialization After you've followed the installation
 instructions, if you're *new* to `smol-k8s-lab`, initialize a new config file:
 ```bash # we'll walk you through any configuration needed before # saving the
-config and deploying it for you smol-k8s-lab ``` UUppggrraaddiinngg ccoonnffiigg ffrroomm vv22..22..44
-ttoo vv33..xx If you've installed smol-k8s-lab prior to `v3.0.0`, please backup your
+config and deploying it for you smol-k8s-lab ``` UUppggrraaddiinngg ccoonnffiigg ffrroomm vv33..77..11
+ttoo vv44..xx If you've installed smol-k8s-lab prior to `v4.0.0`, please backup your
 old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or
 `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the
 following with either pip or pipx: *if using pip*: ```yaml # this upgrades
 smol-k8s-lab pip3.11 install --upgrade smol-k8s-lab # this initializes a new
 configuration smol-k8s-lab ``` *or if using pipx*: ```yaml # this upgrades
 smol-k8s-lab pipx upgrade smol-k8s-lab # this initializes a new configuration
-smol-k8s-lab ``` The main breaking changes between `v2.2.4` and `v3.0` are as
-follows: - *home assistant has graduated from demo app to live app* You'll need
-to change `apps.home_assistant.argo.path` to either `home-assistant/
+smol-k8s-lab ``` The main breaking changes between `v3.7.1` and `v4.0.0` are
+that we now default enable metrics on most apps. Because of this, you need to
+have the Prometheus ServiceMonitor CRD installed ahead of time. Luckily, we now
+provide that as an app as well :) If you deleted your config and created a new
+one, it will already be there, but if you want to reuse your old config, you
+can add the app like this: ```yaml apps: prometheus_crds: description: |
+[link=https://prometheus.io/docs/introduction/overview/]Prometheus[/link] CRDs
+to start with. You can optionally disable this if you don't want to deploy apps
+with metrics. enabled: true argo: # secrets keys to make available to Argo CD
+ApplicationSets secret_keys: {} # git repo to install the Argo CD app from
+repo: https://github.com/small-hack/argocd-apps # path in the argo repo to
+point to. Trailing slash very important! path: prometheus/crds/ # either the
+branch or tag to point at in the argo repo above revision: main # namespace to
+install the k8s app in namespace: prometheus # recurse directories in the
+provided git repo directory_recursion: false # source repos for Argo CD App
+Project (in addition to argo.repo) project: name: prometheus source_repos: -
+https://github.com/prometheus-community/helm-charts.git destination: #
+automatically includes the app's namespace and argocd's namespace namespaces: -
+kube-system - prometheus ``` If using the default repos, please also disable
+directory directory_recursion for: - your prometheus stack app - zitadel For
+all changes, please check out [PR #206](https://github.com/small-hack/smol-k8s-
+lab/pull/206). UUppggrraaddiinngg ccoonnffiigg ffrroomm vv22..22..44 ttoo vv33..xx If you've installed smol-
+k8s-lab prior to `v3.0.0`, please backup your old configuration, and then
+remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-
+lab/config.yaml`) file entirely, then run the following with either pip or
+pipx: *if using pip*: ```yaml # this upgrades smol-k8s-lab pip3.11 install --
+upgrade smol-k8s-lab # this initializes a new configuration smol-k8s-lab ```
+*or if using pipx*: ```yaml # this upgrades smol-k8s-lab pipx upgrade smol-k8s-
+lab # this initializes a new configuration smol-k8s-lab ``` The main breaking
+changes between `v2.2.4` and `v3.0` are as follows: - *home assistant has
+graduated from demo app to live app* You'll need to change
+`apps.home_assistant.argo.path` to either `home-assistant/
 toleration_and_affinity/` if you're using node labels and taints, or `home-
 assistant/` if you're deploying to a single node cluster. Here's an example
 with no tolerations or node affinity: ```yaml apps: home_assistant: enabled:
 false description: | [link=https://home-assistant.io]Home Assistant[/link] is a
 home IOT management solution. By default, we assume you want to use node
 affinity and tolerations to keep home assistant pods on certain nodes and keep
 other pods off said nodes. If you don't want to use either of these features
```

### Comparing `smol_k8s_lab-3.7.1/pyproject.toml` & `smol_k8s_lab-4.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "smol_k8s_lab"
-version       = "3.7.1"
+version       = "4.0.0"
 description   = "CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD"
 authors       = ["Jesse Hitch <jessebot@linux.com>",
                  "Max Roby <emax@cloudydev.net>"]
 readme        = "README.md"
 packages      = [{include = "smol_k8s_lab"}]
 license       = "AGPL-3.0-or-later"
 homepage      = "https://small-hack.github.io/smol-k8s-lab"
```

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/__init__.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3.11
 """
            NAME: smol-k8s-lab
     DESCRIPTION: package, cli, and tui for setting up k8s on metal with
                  k3s, KinD, and k3d, as well as installing our or your own
                  Argo CD Apps, ApplicationSets, and Projects.
-                 
+
          AUTHOR: jessebot(AT)linux(d0t)com
         LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE
 """
 
 from click import option, command
 import logging
 from os import environ as env
@@ -240,14 +240,15 @@
             api_tls_verify = False
         else:
             api_tls_verify = True
 
         # Setup minio, our local s3 provider, is essential for creating buckets
         # and cnpg operator, our postgresql operator for creating postgres clusters
         setup_operators(k8s_obj,
+                        apps.pop('prometheus_crds', {}),
                         apps.pop('longhorn', {}),
                         apps.pop('k8up', {}),
                         apps.pop('minio_operator', {}),
                         apps.pop('seaweedfs', {}),
                         apps.pop('cnpg_operator', {}),
                         apps.pop('postgres_operator', {}),
                         bw)
@@ -258,14 +259,15 @@
                 api_tls_verify,
                 apps.pop('zitadel', {}),
                 apps.pop('vouch', {}),
                 bw,
                 SECRETS['argo_cd_hostname']
                 )
 
+        # we need this for all the oidc apps we need to create
         zitadel_hostname = SECRETS.get('zitadel_hostname', "")
 
         # setup netmaker, a wireguard vpn management web interface
         netmaker_dict = apps.pop('netmaker', {'enabled': False})
         # only do this if the user has smol-k8s-lab init enabled
         if netmaker_dict['enabled']:
             configure_netmaker(k8s_obj,
@@ -274,14 +276,15 @@
                                zitadel_hostname,
                                bw,
                                oidc_obj)
 
         setup_federated_apps(
                 k8s_obj,
                 api_tls_verify,
+                apps.pop('home_assistant', {}),
                 apps.pop('nextcloud', {}),
                 apps.pop('mastodon', {}),
                 apps.pop('matrix', {}),
                 zitadel_hostname,
                 oidc_obj,
                 bw
                 )
```

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/bw_cli.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/bw_cli.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/tui/bitwarden.css` & `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden.css`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/tui/bitwarden_app.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/config/default_config.yaml` & `smol_k8s_lab-4.0.0/smol_k8s_lab/config/default_config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     # accessibility options for users that benefit from TTS and Bell sounds
     accessibility:
       bell:
         # ring the built in terminal bell on focus to new elements on the screen
         on_focus: true
         # ring the built in terminal bell when something is wrong
         on_error: true
-      text_to_speech: 
+      text_to_speech:
         # use a specific program for text to speech - needs to be a full path
         # macOS default: say
         speech_program: say
         # read aloud the screen title and description
         screen_titles: true
         # read aloud the element id, value, and tooltip each time you switch focus
         on_focus: false
@@ -64,15 +64,15 @@
 # NOTE: only kind and k3d are available on macOS at this time
 k8s_distros:
   k3s:
     # set to true to enable deploying a Kubernetes cluster using k3s
     enabled: false
     # if k8s_distro set to k3s/k3d, you can add an array of extra arguments to pass
     # to the k3s install script as a k3s.yaml file. If you enable cilium, we
-    # automatically pass in flannel-backend: none and disable-network-policy: true 
+    # automatically pass in flannel-backend: none and disable-network-policy: true
     k3s_yaml:
       # if you enable MetalLB, we automatically add servicelb to the disable list
       # enables encryption at rest for Kubernetes secrets
       secrets-encryption: true
       # disables traefik so we can enable ingress-nginx, remove if you're using traefik
       disable:
       - "traefik"
@@ -80,15 +80,15 @@
       - "ingress-ready=true"
       kubelet-arg:
       - "max-pods=150"
     # list of nodes to SSH to and join to cluster. example:
     # nodes:
     #   # name can be a hostname or ip address
     #   serverfriend1.lan:
-    #     # change ssh_key to the name of a local private key to use   
+    #     # change ssh_key to the name of a local private key to use
     #     ssh_key: id_rsa
     #     # must be node type of "worker" or "control_plane"
     #     node_type: worker
     #     # labels are optional, but may be useful for pod node affinity
     #     node_labels:
     #       - iot=true
     #     # taints are optional, but may be useful for pod tolerations
@@ -97,15 +97,15 @@
     nodes: {}
 
   k3d:
     # set to true to enable deploying a Kubernetes cluster using k3d
     enabled: false
     # if k8s_distro set to k3s/k3d, you can add an array of extra arguments to pass
     # to the k3s install script as a k3s.yaml file. if you enable cilium, we
-    # automatically pass in flannel-backend: none and disable-network-policy: true 
+    # automatically pass in flannel-backend: none and disable-network-policy: true
     k3s_yaml:
       # if you enable MetalLB, we automatically add servicelb to the disable list
       # enables encryption at rest for Kubernetes secrets
       secrets-encryption: true
       # disables traefik so we can enable ingress-nginx, remove if you're using traefik
       disable:
       - "traefik"
@@ -213,15 +213,15 @@
     init:
       # Deploys staging and prod ClusterIssuers and prompts you for
       # values if they were not set. Switch to false if you don't want
       # to deploy any ClusterIssuers
       enabled: true
       values:
         # Used for to generate certs and alert you if they're going to expire
-        email: "" 
+        email: ""
         # choose between "http01" or "dns01"
         cluster_issuer_acme_challenge_solver: http01
         # only needed if cluster_issuer_challenge_solver set to dns01
         # currently only cloudflare is supported
         cluster_issuer_acme_dns01_provider: cloudflare
       sensitive_values:
         # can be passed in as env vars if you pre-pend CERT_MANAGER_
@@ -384,15 +384,15 @@
           # you can change this your app's name
           namespaces:
             - generic-app
 
   generic_device_plugin:
     enabled: false
     description: |
-      This installs the [link=https://github.com/squat/generic-device-plugin/tree/main]squat/generic-device-plugin[/link], which is recommended for exposing generic devices such as USB devices to your k8s pods. This can useful if you have an IoT coordinator device such as the conbee 2 that you are using with deconz or home assistant. You can read more about device plugins in the [Kubernetes docs](https://kubernetes.io/docs/concepts/extend-kubernetes/compute-storage-net/device-plugins/).
+      This installs the [link=https://github.com/squat/generic-device-plugin/tree/main]squat/generic-device-plugin[/link], which is recommended for exposing generic devices such as USB devices to your k8s pods. This can useful if you have an IoT coordinator device such as the conbee 2 that you are using with deconz or home assistant. You can read more about device plugins in the [link=https://kubernetes.io/docs/concepts/extend-kubernetes/compute-storage-net/device-plugins/]Kubernetes docs[/link].
     argo:
       secret_keys: {}
       repo: https://github.com/small-hack/argocd-apps
       path: generic-device-plugin/
       revision: main
       namespace: kube-system
       directory_recursion: false
@@ -408,32 +408,64 @@
     enabled: false
     description: |
       [link=https://home-assistant.io]Home Assistant[/link] is a home IOT management solution.
 
       By default, we assume you want to use node affinity and tolerations to keep home assistant pods on certain nodes and keep other pods off said nodes. If you don't want to use either of these features but still want to use the small-hack/argocd-apps repo, first change the argo path to /home-assistant/ and then remove the 'toleration_' and 'affinity' secret_keys from the yaml file under apps.home_assistant.description.
 
       [b]NOTE[/b]: If you want to pass in a USB device, you will need the generic device plugin (which is available as a default Argo CD app via smol-k8s-lab 💙)
+
+      This app takes one sensitive value, password for the initial owner user. You can also pass it in as an enviornment variable called $HOME_ASSISTANT_PASSWORD.
+    # Initialization of the app through smol-k8s-lab
+    init:
+      # enable the creation of an initial owner user
+      enabled: true
+      values:
+        # -- owner user's name
+        name: "admin"
+        # -- owner user's username
+        user_name: "admin"
+        # -- owner user's language, default is english
+        language: "en"
+      sensitive_values:
+        - PASSWORD
     argo:
       secret_keys:
         hostname: ""
+        # name of your home assistant area, users often just use "home"
+        name: "home"
+        # default alpha-2 country code, default is NL which is The Netherlands
+        country: "NL"
+        # currency code to use for calculating costs, defaults to EUR for euro
+        currency: "EUR"
+        # other option is "imperial"
         unit_system: "metric"
+        # set to F for USA imperialist tempurature
         temperature_unit: "C"
+        # latitude of your personal coordinates
+        latitude: ""
+        # longitude of your personal coordinates
+        longitude: ""
+        # the elevation of your house?
+        elevation: ""
         # you can delete these if you're not using tolerations/affinity
         toleration_key: ""
         toleration_operator: ""
         toleration_value: ""
         toleration_effect: ""
-        # these are for node affinity
+        # these are for node affinity, delete if not in use
         affinity_key: ""
         affinity_value: ""
         # these are for passing in a USB device such as the conbee II
         usb_device_path: ""
         usb_device_mount_path: "/dev/ttyACM0"
         usb_device_index: "1"
-
+        # these are for passing in a bluetooth device
+        bluetooth_device_path: /run/dbus
+        bluetooth_device_mount_path: /run/dbus
+        bluetooth_device_index: '2'
       repo: https://github.com/small-hack/argocd-apps
       path: home-assistant/toleration_and_affinity/
       revision: main
       namespace: home-assistant
       directory_recursion: false
       project:
         name: home-assistant
@@ -720,15 +752,15 @@
         - RESTIC_REPO_PASSWORD
     argo:
       # secrets keys to make available to Argo CD ApplicationSets
       secret_keys:
         admin_user: tootadmin
         # hostname that users go to in the browser
         hostname: ""
-        # set the local s3 provider for mastodon's public data in one bucket 
+        # set the local s3 provider for mastodon's public data in one bucket
         # and private database backups in another. can be minio or seaweedfs
         s3_provider: seaweedfs
         # how large the backing pvc's capacity should be for minio or seaweedfs
         s3_pvc_capacity: 120Gi
         # local s3 endpoint for postgresql backups, backed up constantly
         s3_endpoint: ""
         s3_region: eu-west-1
@@ -763,15 +795,15 @@
 
   matrix:
     description: |
       [link=https://matrix.org/]Matrix[/link] is an open protocol for decentralised, secure communications.
       This deploys a matrix synapse server, element (web frontend), and turn server (voice)
 
       smol-k8s-lab supports initialization by creating initial secrets for your:
-        - matrix, element, and federation hostnames, 
+        - matrix, element, and federation hostnames,
         - credentials for: postgresql, admin user, S3 storage, and SMTP
 
       smol-k8s-lab also sets up an OIDC application via Zitadel.
 
       To provide sensitive values via environment variables to smol-k8s-lab use:
         - MATRIX_SMTP_PASSWORD
         - MATRIX_S3_BACKUP_ACCESS_ID
@@ -1095,14 +1127,44 @@
         - https://opensource.zalando.com/postgres-operator/charts/postgres-operator-ui
         - https://seaweedfs.github.io/seaweedfs/helm
         destination:
           # automatically includes the app's namespace and argocd's namespace
           namespaces:
           - postgres-operator
 
+  prometheus_crds:
+    description: |
+      [link=https://prometheus.io/docs/introduction/overview/]Prometheus[/link] CRDs to start with.
+      You can optionally disable this if you don't want to deploy apps with metrics.
+
+    enabled: true
+    argo:
+      # secrets keys to make available to Argo CD ApplicationSets
+      secret_keys: {}
+      # git repo to install the Argo CD app from
+      repo: https://github.com/small-hack/argocd-apps
+      # path in the argo repo to point to. Trailing slash very important!
+      path: prometheus/crds/
+      # either the branch or tag to point at in the argo repo above
+      revision: main
+      # namespace to install the k8s app in
+      namespace: prometheus
+      # recurse directories in the provided git repo
+      directory_recursion: false
+      # source repos for Argo CD App Project (in addition to argo.repo)
+      project:
+        name: prometheus
+        source_repos:
+        - https://github.com/prometheus-community/helm-charts.git
+        destination:
+          # automatically includes the app's namespace and argocd's namespace
+          namespaces:
+          - kube-system
+          - prometheus
+
   prometheus:
     description: |
       Full monitoring stack with [link=https://prometheus.io/docs/introduction/overview/]Prometheus[/link], grafana, loki, and alert manager.
 
       smol-k8s-lab supports initialization by setting up your ingress hostnames.
 
     enabled: false
@@ -1352,15 +1414,15 @@
       # if you want to use cockroachdb, change to zitadel/zitadel_and_cockroachdb
       path: "zitadel/app_of_apps/"
       # either the branch or tag to point at in the argo repo above
       revision: main
       # namespace to install the k8s app in
       namespace: "zitadel"
       # recurse directories in the provided git repo
-      directory_recursion: true
+      directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: zitadel
         source_repos:
           - https://charts.zitadel.com
           - https://zitadel.github.io/zitadel-charts
           - https://small-hack.github.io/cloudnative-pg-cluster-chart
```

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/config/keycloak_config.json` & `smol_k8s_lab-4.0.0/smol_k8s_lab/config/keycloak_config.json`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/constants.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/constants.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/env_config.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/env_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/__init__.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/initial_special.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,21 +156,23 @@
     ingress_nginx_enabled = ingress_dict["enabled"]
     # make sure helm is installed and the repos are up to date
     prepare_helm(k8s_distro, argo_enabled, metallb_enabled, cilium_enabled,
                  argo_secrets_plugin_enabled)
 
     # needed for network policy editor and hubble UI
     if cilium_enabled:
-        header("Installing [green]cilium[/green] so we have networking tools", '🛜')
+        header("Installing [green]cilium[/green] so we have networking tools",
+               '🛜')
         if cilium_dict['init']['enabled']:
             configure_cilium(cilium_dict)
 
     # needed for metal (non-cloud provider) installs
     if metallb_enabled:
-        header("Installing [green]metallb[/green] so we have an IP address pool.", '🛜')
+        header("Installing [green]metallb[/green] so we have an IP address pool",
+               '🛜')
         if metallb_dict['init']['enabled']:
             cidr = metallb_dict['init']['values']['address_pool']
             if not cidr:
                 m = "[green]Please enter a comma seperated list of IPs or CIDRs"
                 cidr = Prompt.ask(m).split(',')
 
             configure_metallb(k8s_obj, cidr)
```

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/argocd.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/argocd.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,17 @@
                            "nginx.ingress.kubernetes.io/ssl-passthrough": True,
                        },
                        "ingressClassName": "nginx",
                        "https": True,
                        "tls":  [{"secretName": "argocd-secret",
                                  "hosts": [argo_cd_domain]}]}}}
 
+        # TODO: add this to dict if debug logging is enabled for smol-k8s-lab:
+        # "global": {"logging": {"level": "debug"}}
+
         if secret_dict.get('global_cluster_issuer', None):
             val['server']['ingress']['annotations']['cert-manager.io/cluster-issuer'] = secret_dict['global_cluster_issuer']
 
         # if we're using bitwarden, generate a password & save it
         if bitwarden:
             sub_header(":lock: Creating a new password in BitWarden.")
             # if we're using bitwarden...
```

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/identity_provider/vouch.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,38 +428,47 @@
 
     def create_claim_action(self, script: str = "") -> None:
         """
         create an action for zitadel to run before sending user info or
         giving access token
         """
         log.info("Creating action...")
-        response = request("POST",
-                           self.api_url + "actions",
-                           headers=self.headers,
-                           data=script,
-                           verify=self.verify)
-        log.debug(response.text)
+        while True:
+            response = request("POST",
+                               self.api_url + "actions",
+                               headers=self.headers,
+                               data=script,
+                               verify=self.verify)
+            log.debug(response.text)
+            # if the response is not 200, just try again 🤷
+            if response.status_code == 200:
+                break
 
         log.debug("Creating action flow triggers...")
         action_id = response.json()['id']
         action_payload = dumps({"actionIds": [action_id]})
         log.debug(action_payload)
 
         # At the moment you have to send the ID of the Trigger Type:
         # PreUserinfoCreation=4, PreAccessTokenCreation=5
         for trigger_type in ['4', '5']:
             url = f"{self.api_url}flows/2/trigger/{trigger_type}"
             log.debug(f"url is {url}")
 
-            response = request("POST",
-                               url,
-                               headers=self.headers,
-                               data=action_payload,
-                               verify=self.verify)
-            log.debug(f"flows response is {response.text}")
+            while True:
+                response = request("POST",
+                                   url,
+                                   headers=self.headers,
+                                   data=action_payload,
+                                   verify=self.verify)
+                log.debug(f"flows response is {response.text}")
+
+                # if the response is not 200, just try again 🤷
+                if response.status_code == 200:
+                    break
 
     def create_role(self,
                     role_key: str = "",
                     display_name: str = "",
                     group: str = "") -> None:
         """
         create a role in zitadel from given:
@@ -477,28 +486,28 @@
 
         response = request("POST", url, headers=self.headers, data=payload,
                            verify=self.verify)
 
         log.info(response.text)
 
     def set_user_by_login_name(self, user: str) -> None:
-        """ 
+        """
         get the user's ID by their login name
         """
         url = f"{self.api_url}global/users/_by_login_name?loginName={user}"
 
         response = request("GET", url, headers=self.headers, data={},
                            verify=self.verify).json()
         log.debug(response)
 
         self.user_id = response['user']['id']
         self.resource_owner = response['user']['details']['resourceOwner']
 
     def set_project_by_name(self, project_name: str) -> str:
-        """ 
+        """
         project_name: str - name of the project to use for future app creation
 
         sets the current self.project_id after searching for the project by name
         """
         url = f"{self.api_url}projects/_search"
 
         payload = dumps({
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/ingress/cert_manager.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/initial_special.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from .networking.cilium import configure_cilium
 from .secrets_management.external_secrets_operator import configure_external_secrets
 from .secrets_management.infisical import configure_infisical
 from .secrets_management.vault import configure_vault
 from .social.matrix import configure_matrix
 from .social.mastodon import configure_mastodon
 from .social.nextcloud import configure_nextcloud
+from .social.home_assistant import configure_home_assistant
 
 
 def setup_k8s_secrets_management(k8s_obj: K8s,
                                  k8s_distro: str,
                                  eso_dict: dict = {},
                                  eso_provider: str = "",
                                  infisical_dict: dict = {},
@@ -40,31 +41,31 @@
     """
     sets up k8s secrets management tooling
     """
     # secrets management section
     header_msg = "Setting up K8s secret management with [green]"
 
     # setup external secrets operator and bitwarden external secrets
-    if eso_dict['enabled']:
+    if eso_dict.get('enabled', False):
         header_msg += f'External Secrets Operator[/] and [blue]{eso_provider}[/] as the Provider'
         header(header_msg, '🤫')
         configure_external_secrets(k8s_obj,
                                    eso_dict,
                                    eso_provider,
                                    k8s_distro,
                                    bitwarden)
 
     # setup infisical - an secrets manager and operator for k8s that replaces eso
-    elif infisical_dict['enabled']:
+    elif infisical_dict.get('enabled', False):
         header_msg += 'Infisical Secrets Operator[/]'
         header(header_msg, '🤫')
         configure_infisical(k8s_obj, infisical_dict)
 
     # setup hashicorp's vault, a secret key management system that works with eso
-    if vault_dict['enabled']:
+    if vault_dict.get('enabled', False):
         configure_vault(k8s_obj, vault_dict)
 
 
 def setup_oidc_provider(k8s_obj: K8s,
                         api_tls_verify: bool = False,
                         zitadel_dict: dict = {},
                         vouch_dict: dict = {},
@@ -74,19 +75,19 @@
     sets up oidc provider. only zitadel is supported right now
     if we choose to add keycloak back, we'll be adding the following arg
     keycloak_dict: dict = {}
     """
     header("Setting up [green]OIDC[/]/[green]Oauth[/] Applications")
 
     # keycloak_enabled = keycloak_dict['enabled']
-    zitadel_enabled = zitadel_dict['enabled']
+    zitadel_enabled = zitadel_dict.get('enabled', False)
 
     vouch_enabled = False
     if vouch_dict:
-        vouch_enabled = vouch_dict['enabled']
+        vouch_enabled = vouch_dict.get('enabled', False)
 
     # setup keycloak if we're using that for OIDC
     # if keycloak_enabled:
     #     log.debug("Setting up keycloak")
     #     configure_keycloak(k8s_obj, keycloak_dict, bw)
     #     realm = keycloak_dict['argo']['secret_keys']['default_realm']
     #     user = keycloak_dict['init']['values']['username']
@@ -142,37 +143,35 @@
                     metallb_dict: dict = {},
                     ingress_dict: dict = {},
                     cert_manager_dict: dict = {},
                     argo_enabled: bool = False,
                     argo_secrets_plugin_enabled: bool = False,
                     plugin_secrets: dict = {},
                     bw: BwCLI = None) -> None:
-    """ 
+    """
     Uses Helm to install all base apps that need to be running being argo cd:
         cilium, metallb, ingess-nginx, cert-manager, argo cd, argocd secrets plugin
     All Needed for getting Argo CD up and running.
     """
-    metallb_enabled = metallb_dict['enabled']
-    cilium_enabled = cilium_dict['enabled']
-    ingress_nginx_enabled = ingress_dict["enabled"]
+    metallb_enabled = metallb_dict.get('enabled', False)
+    cilium_enabled = cilium_dict.get('enabled', False)
+    ingress_nginx_enabled = ingress_dict.get('enabled', False)
     # make sure helm is installed and the repos are up to date
     prepare_helm(k8s_distro, argo_enabled, metallb_enabled, cilium_enabled,
                  argo_secrets_plugin_enabled)
 
     # needed for network policy editor and hubble UI
     if cilium_enabled:
-        header("Installing [green]cilium[/green] so we have networking tools",
-               '🛜')
+        header("Installing [green]cilium[/green] so we have networking tools", '🛜')
         if cilium_dict['init']['enabled']:
             configure_cilium(cilium_dict)
 
     # needed for metal (non-cloud provider) installs
     if metallb_enabled:
-        header("Installing [green]metallb[/green] so we have an IP address pool",
-               '🛜')
+        header("Installing [green]metallb[/green] so we have an IP address pool.", '🛜')
         if metallb_dict['init']['enabled']:
             cidr = metallb_dict['init']['values']['address_pool']
             if not cidr:
                 m = "[green]Please enter a comma seperated list of IPs or CIDRs"
                 cidr = Prompt.ask(m).split(',')
 
             configure_metallb(k8s_obj, cidr)
@@ -182,40 +181,44 @@
         # nginx just because that's most supported, treafik support may be added later
         header("Installing [green]ingress-nginx-controller[/green] to access web"
                " apps outside the cluster", "🌐")
         configure_ingress_nginx(k8s_obj, k8s_distro)
 
     # manager SSL/TLS certificates via lets-encrypt
     header("Installing [green]cert-manager[/green] for TLS certificates...", '📜')
-    if cert_manager_dict["enabled"]:
+    if cert_manager_dict.get('enabled', False):
         configure_cert_manager(k8s_obj, cert_manager_dict['init'])
 
     # then we install argo cd if it's enabled
     if argo_enabled:
         configure_argocd(k8s_obj,
-                         bw, 
+                         bw,
                          argo_secrets_plugin_enabled,
                          plugin_secrets)
 
     if ingress_nginx_enabled and argo_enabled:
         install_ingress_nginx_argocd_app(k8s_obj, ingress_dict)
 
 
 def setup_federated_apps(k8s_obj: K8s,
                          api_tls_verify: bool = False,
+                         home_assistant_dict: dict = {},
                          nextcloud_dict: dict = {},
                          mastodon_dict: dict = {},
                          matrix_dict: dict = {},
                          zitadel_hostname: str = "",
                          zitadel_obj: Zitadel = None,
                          bw: BwCLI = None) -> None:
     """
     Setup any federated apps with initialization supported
     """
-    if nextcloud_dict['enabled']:
+    if home_assistant_dict.get('enabled', False):
+        configure_home_assistant(k8s_obj, home_assistant_dict, api_tls_verify, bw)
+
+    if nextcloud_dict.get('enabled', False):
         configure_nextcloud(k8s_obj, nextcloud_dict, bw, zitadel_obj)
 
-    if mastodon_dict['enabled']:
+    if mastodon_dict.get('enabled', False):
         configure_mastodon(k8s_obj, mastodon_dict, bw)
 
-    if matrix_dict['enabled']:
+    if matrix_dict.get('enabled', False):
         configure_matrix(k8s_obj, matrix_dict, zitadel_obj, bw)
```

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/networking/cilium.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/cilium.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/networking/metallb.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/metallb.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/networking/netmaker.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/netmaker.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/__init__.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 from smol_k8s_lab.k8s_tools.k8s_lib import K8s
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI
 from smol_k8s_lab.utils.rich_cli.console_logging import header
 from .longhorn import configure_longhorn
 from .k8up_operater import configure_k8up_operator
 from .minio import configure_minio_operator
 from .postgres_operators import configure_cnpg_operator, configure_postgres_operator
+from .prometheus import configure_prometheus_crds
 from .seaweedfs import configure_seaweedfs
 
 
 def setup_operators(k8s_obj: K8s,
+                    prometheus_config: dict = {},
                     longhorn_config: dict = {},
                     k8up_config: dict = {},
                     minio_config: dict = {},
                     seaweed_config: dict = {},
                     cnpg_config: dict = {},
                     pg_config: dict = {},
                     bitwarden: BwCLI = None) -> None:
-    """ 
+    """
     deploy all k8s operators that can block other apps:
+        - prometheus
+        - longhorn
+        - k8up
         - minio operator
+        - seaweedfs
         - cnpg (cloud native postgres) operator
+        - zalando postgres operator
     """
     header("Setting up Operators", "⚙️ ")
 
+    # deploy the prometheus CRDs before everything else so that apps with metrics don't fail
+    if prometheus_config and prometheus_config.get('enabled', False):
+        configure_prometheus_crds(k8s_obj, prometheus_config)
+
     # longhorn operator is used to have expanding volumes that span multiple nodes
     if longhorn_config and longhorn_config.get('enabled', False):
         configure_longhorn(k8s_obj, longhorn_config)
 
     # k8up operator is a postgres operator for creating postgresql clusters
     if k8up_config and k8up_config.get('enabled', False):
         configure_k8up_operator(k8s_obj, k8up_config)
```

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/k8up_operater.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/k8up_operater.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/longhorn.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/longhorn.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/minio.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/minio.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/postgres_operators.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/operators/seaweedfs.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/secrets_management/infisical.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/secrets_management/vault.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/social/mastodon.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/mastodon.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/social/mastodon_rake.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/social/matrix.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/matrix.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/social/nextcloud.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/nextcloud.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_distros/__init__.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_distros/k3d.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/k3d.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_distros/k3s.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/k3s.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_distros/kind.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/kind.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_tools/argocd_util.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/argocd_util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_tools/helm.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/helm.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/k8s_tools/k8s_lib.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/k8s_lib.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/__init__.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/argocd_widgets.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/input_widgets.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/input_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/invalid_apps.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/modify_globals.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/modify_globals.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/app_widgets/new_app_modal.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/apps_screen.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/apps_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/base.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # list of approved words for nouns
 CUTE_NOUNS = [
         "bunny", "hoglet", "puppy", "kitten", "knuffel", "friend", "egel",
         "meerkoet", "raccoon", "wasbeertje"
         ]
 
 CUTE_ADJECTIVE = [
-        "lovely", "adorable", "cute", "friendly", "nice", "leuke", "mooie", 
+        "lovely", "adorable", "cute", "friendly", "nice", "leuke", "mooie",
         "vriendelijke", "cool", "soft", "smol", "small", "klein"
         ]
 
 class BaseApp(App):
     BINDINGS = [
             Binding(key="?,h",
                     key_display="?",
@@ -74,14 +74,15 @@
         self.cfg = user_config
         self.show_footer = self.cfg['smol_k8s_lab']['tui']['show_footer']
         self.cluster_names = []
         self.current_cluster = ""
         self.sensitive_values = {
                 'cert_manager': {},
                 'nextcloud': {},
+                'home_assistant': {},
                 'matrix': {},
                 'mastodon': {},
                 'postgres_operator': {},
                 'zitadel': {}
                 }
 
         # configure global accessibility
@@ -138,30 +139,30 @@
             self.get_widget_by_id("base-screen-container").add_class("no-cluster-table")
             if self.speak_screen_titles:
                 self.action_say("Welcome to smol-k8s-lab. Press tab, then C, to configure "
                                 "accessibility options.")
 
 
     def generate_cluster_table(self, clusters: list) -> None:
-        """ 
+        """
         generate a readable table for all the clusters.
 
         Each row is has a height of 3 and is centered to make it easier to read
         for people with dyslexia
         """
         data_table = DataTable(zebra_stripes=True,
                                id="clusters-data-table",
                                cursor_type="row")
 
         # then fill in the cluster table
         data_table.add_column(Text("Cluster", justify="center"))
         data_table.add_column(Text("Distro", justify="center"))
 
         for row in clusters:
-            # we use an extra line to center the rows vertically 
+            # we use an extra line to center the rows vertically
             styled_row = [Text(str("\n" + cell), justify="center") for cell in row]
 
             # we add extra height to make the rows more readable
             data_table.add_row(*styled_row, height=3, key=row[0])
 
             self.cluster_names.append(row[0])
 
@@ -237,15 +238,15 @@
         press button for new cluster
         """
         new_cluster_button = self.get_widget_by_id("new-cluster-button")
         if not new_cluster_button.disabled:
             new_cluster_button.action_press()
 
     def action_request_apps_cfg(self,
-                                app_to_highlight: str = "", 
+                                app_to_highlight: str = "",
                                 modify_cluster: bool = False) -> None:
         """
         launches the argo app config screen
         """
         self.app.push_screen(AppsConfig(self.cfg['apps'],
                                         app_to_highlight,
                                         modify_cluster))
@@ -278,15 +279,15 @@
     def action_request_help(self,) -> None:
         """
         if the user presses 'h' or '?', show the help modal screen
         """
         self.push_screen(HelpScreen())
 
     def action_request_config(self,) -> None:
-        """ 
+        """
         if the user pressed 'c', show the TUI config screen
         """
         self.push_screen(TuiConfigScreen(self.cfg['smol_k8s_lab']['tui']))
 
     def action_toggle_footer(self) -> None:
         """
         don't display the footer, or do 🤷
@@ -311,15 +312,15 @@
         """
         yaml = YAML()
 
         with open(config_file, 'w') as smol_k8s_config:
             yaml.dump(self.cfg, smol_k8s_config)
 
     def action_say(self, text_for_speech: str = "") -> None:
-        """ 
+        """
         Use the configured speech program to read a string aloud. If no string
         is passed in, and self.speak_on_key_press is True, we read the currently
         focused element id
         """
         say = self.speech_program
         if text_for_speech:
             text_for_speech = text_for_speech.replace("(", "").replace(")", "")
@@ -358,15 +359,15 @@
         column2 = columns[1].label
 
         system(f"{self.speech_program} Selected {column1}: {row_column1}."
                f" {column2}: {row_column2}")
 
     @on(DescendantFocus)
     def on_focus(self, event: DescendantFocus) -> None:
-        """ 
+        """
         on focus, say the id of each element and the value or label if possible
         """
         if self.speak_on_focus:
             id = event.widget.id
             self.action_say(f"element is {id}")
 
             # input fields
@@ -425,15 +426,15 @@
                         if init_sensitive_values:
 
                             prompts = self.check_for_env_vars(app, metadata)
                             if prompts:
                                 skip = False
 
                                 # cert manager is special
-                                if app == "cert_manager": 
+                                if app == "cert_manager":
                                     solver = init_values['cluster_issuer_acme_challenge_solver']
                                     if solver == "http01":
                                         skip = True
 
                                 for value in prompts:
                                     if not self.sensitive_values[app].get(value, ""):
                                         if not skip:
@@ -463,30 +464,30 @@
 
         # provided there's actually any env vars to go get...
         if env_vars:
             # iterate through list of env vars to check
             for item in env_vars:
                 # check env and self.sensitive_values
                 value = environ.get(
-                        "_".join([app.upper(), item]),
+                        "_".join([app.replace("-", "_").upper(), item]),
                         default=self.sensitive_values[app].get(item.lower(), ""))
 
                 if not value:
                     # append any missing values to prompt_values
                     prompt_values.append(item.lower())
 
                 self.sensitive_values[app][item.lower()] = value
 
         return set(prompt_values)
 
 
 class NewClusterInput(Static):
-    """ 
+    """
     small widget with an input and button that takes the names of a cluster,
-    and changes the 
+    and changes the
     """
     def compose(self) -> ComposeResult:
         with Grid(id="new-cluster-button-container"):
             input = Input(validators=[
                               Length(minimum=2),
                               CheckIfNameAlreadyInUse(self.app.cluster_names)
                               ],
@@ -504,15 +505,15 @@
     def on_mount(self) -> None:
         input = self.get_widget_by_id("cluster-name-input")
         input.value = random.choice(CUTE_ADJECTIVE) + '-' + random.choice(CUTE_NOUNS)
 
     @on(Input.Changed)
     @on(Input.Submitted)
     def input_validation(self, event: Input.Changed | Input.Submitted) -> None:
-        """ 
+        """
         Takes events matching Input.Changed and Input.Submitted events, and
         checks if input is valid. If the user presses enter (Input.Submitted),
         and the input is valid, we also press the button for them.
         """
         new_cluster_button = self.get_widget_by_id("new-cluster-button")
 
         if event.validation_result.is_valid:
```

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/base_cluster_modal.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/base_cluster_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/confirm_screen.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/confirm_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/add_nodes_widget.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/apps_config.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/apps_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/apps_init_config.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/apps_init_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/base.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/base.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/base_modal.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/base_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/cluster_modal.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/cluster_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/confirm.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/confirm.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/distro_config.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/distro_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/help.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/help.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/invalid_apps.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/invalid_apps.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/k3s.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/k3s.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/kind.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/kind.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/modify_globals_modal.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/new_app_modal.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/new_app_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/node_inputs_widget.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/node_modal.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/node_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/css/tui_config.tcss` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/tui_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_screen.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/add_nodes.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/k3s_config.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/kind_config.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/kind_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/kubelet_config.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/distro_widgets/node_adjustment.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/help_screen.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/help_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/make_screenshots.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/make_screenshots.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/smol_k8s_config_screen.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/smol_k8s_config_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/tui_config_screen.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/tui_config_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/util.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/tui/validators/already_exists.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/validators/already_exists.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/utils/passwords.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/utils/passwords.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/utils/rich_cli/console_logging.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/utils/rich_cli/console_logging.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/utils/rich_cli/help_text.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/utils/rich_cli/help_text.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/smol_k8s_lab/utils/subproc.py` & `smol_k8s_lab-4.0.0/smol_k8s_lab/utils/subproc.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-3.7.1/PKG-INFO` & `smol_k8s_lab-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smol_k8s_lab
-Version: 3.7.1
+Version: 4.0.0
 Summary: CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD
 Home-page: https://small-hack.github.io/smol-k8s-lab
 License: AGPL-3.0-or-later
 Keywords: kubernetes,homelab,kind,k3s,k8s
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
@@ -44,15 +44,15 @@
   />
  🧸 <code>smol-k8s-lab</code>
   <a href="https://github.com/small-hack/smol-k8s-lab/releases">
     <img src="https://img.shields.io/github/v/release/small-hack/smol-k8s-lab?style=plastic&labelColor=484848&color=3CA324&logo=GitHub&logoColor=white">
   </a>
 </h2>
 <p align="center">
-  A terminal based tool to install slimmer k8s distros on metal, with batteries included! 
+  A terminal based tool to install slimmer k8s distros on metal, with batteries included!
 </p>
 
 <p align="center">
   <a href="https://www.youtube.com/watch?v=UdOQM9n5hyU&t=0s">
     <img width="800" alt="Screenshot of smol-k8s-lab (on the welcome screen) in a video tutorial on youtube. please click this image, as it is a link to youtube where I explain everything about smol-k8s-lab. The video image screenshot shows the smol-k8s-lab create a cluster feature which is a text input" src="https://github.com/small-hack/smol-k8s-lab/assets/2389292/ee0ca93b-628e-495f-83ab-70aa9eb52295">
   </a><br>
   <sup>(Here's the <a href="https://youtu.be/2E9DVJpv440?feature=shared">same video with captions)</a></sup>
@@ -107,19 +107,85 @@
 
 ## Usage
 
 ### Initialization
 After you've followed the installation instructions, if you're *new* to `smol-k8s-lab`,  initialize a new config file:
 
 ```bash
-# we'll walk you through any configuration needed before 
+# we'll walk you through any configuration needed before
 # saving the config and deploying it for you
 smol-k8s-lab
 ```
 <details>
+  <summary><b>Upgrading config from v3.7.1 to v4.x</b></summary>
+
+If you've installed smol-k8s-lab prior to `v4.0.0`, please backup your old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the following with either pip or pipx:
+
+*if using pip*:
+```yaml
+# this upgrades smol-k8s-lab
+pip3.11 install --upgrade smol-k8s-lab
+
+# this initializes a new configuration
+smol-k8s-lab
+```
+
+*or if using pipx*:
+```yaml
+# this upgrades smol-k8s-lab
+pipx upgrade smol-k8s-lab
+
+# this initializes a new configuration
+smol-k8s-lab
+```
+
+The main breaking changes between `v3.7.1` and `v4.0.0` are that we now default enable metrics on most apps. Because of this, you need to have the Prometheus ServiceMonitor CRD installed ahead of time. Luckily, we now provide that as an app as well :) If you deleted your config and created a new one, it will already be there, but if you want to reuse your old config, you can add the app like this:
+
+```yaml
+apps:
+  prometheus_crds:
+    description: |
+      [link=https://prometheus.io/docs/introduction/overview/]Prometheus[/link] CRDs to start with.
+      You can optionally disable this if you don't want to deploy apps with metrics.
+
+    enabled: true
+    argo:
+      # secrets keys to make available to Argo CD ApplicationSets
+      secret_keys: {}
+      # git repo to install the Argo CD app from
+      repo: https://github.com/small-hack/argocd-apps
+      # path in the argo repo to point to. Trailing slash very important!
+      path: prometheus/crds/
+      # either the branch or tag to point at in the argo repo above
+      revision: main
+      # namespace to install the k8s app in
+      namespace: prometheus
+      # recurse directories in the provided git repo
+      directory_recursion: false
+      # source repos for Argo CD App Project (in addition to argo.repo)
+      project:
+        name: prometheus
+        source_repos:
+        - https://github.com/prometheus-community/helm-charts.git
+        destination:
+          # automatically includes the app's namespace and argocd's namespace
+          namespaces:
+          - kube-system
+          - prometheus
+```
+
+If using the default repos, please also disable directory directory_recursion for:
+- your prometheus stack app
+- zitadel
+
+For all changes, please check out [PR #206](https://github.com/small-hack/smol-k8s-lab/pull/206).
+
+</details>
+
+<details>
   <summary><b>Upgrading config from v2.2.4 to v3.x</b></summary>
 
 If you've installed smol-k8s-lab prior to `v3.0.0`, please backup your old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the following with either pip or pipx:
 
 *if using pip*:
 ```yaml
 # this upgrades smol-k8s-lab
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smol_k8s_lab Version: 3.7.1 Summary: CLI and TUI to
+Metadata-Version: 2.1 Name: smol_k8s_lab Version: 4.0.0 Summary: CLI and TUI to
 quickly install slimmer Kubernetes distros and then manage apps declaratively
 using Argo CD Home-page: https://small-hack.github.io/smol-k8s-lab License:
 AGPL-3.0-or-later Keywords: kubernetes,homelab,kind,k3s,k8s Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 or later (AGPLv3+) Classifier: Operating System :: MacOS :: MacOS X
@@ -59,25 +59,54 @@
  _[_O_u_t_p_u_t_ _o_f_ _s_m_o_l_-_k_8_s_-_l_a_b_ _-_-_h_e_l_p_ _a_f_t_e_r_ _c_l_o_n_i_n_g_ _t_h_e_ _d_i_r_e_c_t_o_r_y_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g_ _t_h_e
                                 _p_r_e_r_e_q_u_i_s_i_t_e_s_._]
 Checkout our [TUI docs](https://small-hack.github.io/smol-k8s-lab/tui/
 create_modify_screens/) for more info on how to get started playing with `smol-
 k8s-lab` :-) ## Usage ### Initialization After you've followed the installation
 instructions, if you're *new* to `smol-k8s-lab`, initialize a new config file:
 ```bash # we'll walk you through any configuration needed before # saving the
-config and deploying it for you smol-k8s-lab ``` UUppggrraaddiinngg ccoonnffiigg ffrroomm vv22..22..44
-ttoo vv33..xx If you've installed smol-k8s-lab prior to `v3.0.0`, please backup your
+config and deploying it for you smol-k8s-lab ``` UUppggrraaddiinngg ccoonnffiigg ffrroomm vv33..77..11
+ttoo vv44..xx If you've installed smol-k8s-lab prior to `v4.0.0`, please backup your
 old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or
 `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the
 following with either pip or pipx: *if using pip*: ```yaml # this upgrades
 smol-k8s-lab pip3.11 install --upgrade smol-k8s-lab # this initializes a new
 configuration smol-k8s-lab ``` *or if using pipx*: ```yaml # this upgrades
 smol-k8s-lab pipx upgrade smol-k8s-lab # this initializes a new configuration
-smol-k8s-lab ``` The main breaking changes between `v2.2.4` and `v3.0` are as
-follows: - *home assistant has graduated from demo app to live app* You'll need
-to change `apps.home_assistant.argo.path` to either `home-assistant/
+smol-k8s-lab ``` The main breaking changes between `v3.7.1` and `v4.0.0` are
+that we now default enable metrics on most apps. Because of this, you need to
+have the Prometheus ServiceMonitor CRD installed ahead of time. Luckily, we now
+provide that as an app as well :) If you deleted your config and created a new
+one, it will already be there, but if you want to reuse your old config, you
+can add the app like this: ```yaml apps: prometheus_crds: description: |
+[link=https://prometheus.io/docs/introduction/overview/]Prometheus[/link] CRDs
+to start with. You can optionally disable this if you don't want to deploy apps
+with metrics. enabled: true argo: # secrets keys to make available to Argo CD
+ApplicationSets secret_keys: {} # git repo to install the Argo CD app from
+repo: https://github.com/small-hack/argocd-apps # path in the argo repo to
+point to. Trailing slash very important! path: prometheus/crds/ # either the
+branch or tag to point at in the argo repo above revision: main # namespace to
+install the k8s app in namespace: prometheus # recurse directories in the
+provided git repo directory_recursion: false # source repos for Argo CD App
+Project (in addition to argo.repo) project: name: prometheus source_repos: -
+https://github.com/prometheus-community/helm-charts.git destination: #
+automatically includes the app's namespace and argocd's namespace namespaces: -
+kube-system - prometheus ``` If using the default repos, please also disable
+directory directory_recursion for: - your prometheus stack app - zitadel For
+all changes, please check out [PR #206](https://github.com/small-hack/smol-k8s-
+lab/pull/206). UUppggrraaddiinngg ccoonnffiigg ffrroomm vv22..22..44 ttoo vv33..xx If you've installed smol-
+k8s-lab prior to `v3.0.0`, please backup your old configuration, and then
+remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-
+lab/config.yaml`) file entirely, then run the following with either pip or
+pipx: *if using pip*: ```yaml # this upgrades smol-k8s-lab pip3.11 install --
+upgrade smol-k8s-lab # this initializes a new configuration smol-k8s-lab ```
+*or if using pipx*: ```yaml # this upgrades smol-k8s-lab pipx upgrade smol-k8s-
+lab # this initializes a new configuration smol-k8s-lab ``` The main breaking
+changes between `v2.2.4` and `v3.0` are as follows: - *home assistant has
+graduated from demo app to live app* You'll need to change
+`apps.home_assistant.argo.path` to either `home-assistant/
 toleration_and_affinity/` if you're using node labels and taints, or `home-
 assistant/` if you're deploying to a single node cluster. Here's an example
 with no tolerations or node affinity: ```yaml apps: home_assistant: enabled:
 false description: | [link=https://home-assistant.io]Home Assistant[/link] is a
 home IOT management solution. By default, we assume you want to use node
 affinity and tolerations to keep home assistant pods on certain nodes and keep
 other pods off said nodes. If you don't want to use either of these features
```

