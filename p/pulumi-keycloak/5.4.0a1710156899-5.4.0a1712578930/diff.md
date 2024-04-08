# Comparing `tmp/pulumi_keycloak-5.4.0a1710156899.tar.gz` & `tmp/pulumi_keycloak-5.4.0a1712578930.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_keycloak-5.4.0a1710156899.tar", last modified: Mon Mar 11 11:49:24 2024, max compression
+gzip compressed data, was "pulumi_keycloak-5.4.0a1712578930.tar", last modified: Mon Apr  8 12:25:50 2024, max compression
```

## Comparing `pulumi_keycloak-5.4.0a1710156899.tar` & `pulumi_keycloak-5.4.0a1712578930.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:49:24.655811 pulumi_keycloak-5.4.0a1710156899/
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-03-11 11:49:24.655811 pulumi_keycloak-5.4.0a1710156899/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:49:24.639811 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/
--rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91136 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    28024 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/attribute_to_role_identity_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:49:24.639811 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16911 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    15662 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/execution_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    23414 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/subflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:49:24.639811 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/custom_identity_provider_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    28535 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/custom_user_federation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8754 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/default_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    22625 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/generic_client_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    22921 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/generic_client_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24066 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/generic_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    22483 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/generic_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_authentication_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_authentication_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    26906 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_client_description_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    38664 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_realm_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_user_realm_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/group_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15820 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/hardcoded_role_identity_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24616 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:49:24.643811 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/custom_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/full_name_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    45018 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18611 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/hardcoded_group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/hardcoded_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14490 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    46697 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    32408 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/user_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    89276 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/user_federation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:49:24.643811 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/oidc/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70210 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/oidc/google_identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    82524 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/oidc/identity_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:49:24.651811 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28803 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/audience_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19023 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
--rw-r--r--   0 runner    (1001) docker     (127)    90703 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_aggregate_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_authorization_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_authorization_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_authorization_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_default_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_group_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_js_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_optional_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21986 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_role_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15715 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_service_account_realm_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_service_account_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_time_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_user_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22830 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/full_name_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31435 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/get_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/get_client_authorization_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/get_client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/get_client_service_account_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26284 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/group_membership_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31053 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19300 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35232 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    36170 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    38993 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31198 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    34306 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    30599 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    82512 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   107528 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19091 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    18366 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_aes_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    17615 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_ecdsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    19338 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_hmac_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    25256 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_java_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    22162 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)    19137 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_rsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    18288 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    17346 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/required_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:49:24.655811 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    71743 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/client_default_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    16971 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    24353 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/get_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/get_client_installation_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)   101072 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28415 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20640 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20547 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24612 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20351 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/users_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:49:24.655811 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-03-11 11:49:24.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-03-11 11:49:24.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 11:49:24.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-11 11:49:24.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-11 11:49:24.000000 pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-11 11:49:17.000000 pulumi_keycloak-5.4.0a1710156899/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 11:49:24.655811 pulumi_keycloak-5.4.0a1710156899/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:25:50.802566 pulumi_keycloak-5.4.0a1712578930/
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-08 12:25:50.802566 pulumi_keycloak-5.4.0a1712578930/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:25:50.786566 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/
+-rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91136 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28024 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/attribute_to_role_identity_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:25:50.790566 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16911 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15662 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/execution_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23414 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/subflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:25:50.790566 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/custom_identity_provider_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28535 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/custom_user_federation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8754 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/default_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22625 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/generic_client_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22921 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/generic_client_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24066 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/generic_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22483 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/generic_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_authentication_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_authentication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26906 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_client_description_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38664 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_realm_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_user_realm_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/group_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15820 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/hardcoded_role_identity_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24616 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:25:50.794566 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/custom_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/full_name_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45018 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18611 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/hardcoded_group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/hardcoded_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14490 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46697 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32408 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/user_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89276 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/user_federation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:25:50.794566 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70210 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/oidc/google_identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82524 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/oidc/identity_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:25:50.802566 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28803 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/audience_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19023 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90703 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_aggregate_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_authorization_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_authorization_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_authorization_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_default_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_group_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_js_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_optional_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21986 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_role_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15715 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_service_account_realm_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_service_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_time_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_user_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22830 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/full_name_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31435 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/get_client_authorization_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/get_client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/get_client_service_account_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26284 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/group_membership_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31053 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19300 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35232 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36170 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38993 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31198 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34306 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30599 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82512 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   107528 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19091 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18366 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_aes_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17615 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_ecdsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19338 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_hmac_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25256 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_java_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22162 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19137 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_rsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18288 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17346 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/required_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:25:50.802566 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71743 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/client_default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16971 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24353 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/get_client_installation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101072 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28415 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20640 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20547 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24612 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20351 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/users_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:25:50.802566 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-08 12:25:50.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-04-08 12:25:50.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:25:50.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 12:25:50.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 12:25:50.000000 pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 12:25:44.000000 pulumi_keycloak-5.4.0a1712578930/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:25:50.802566 pulumi_keycloak-5.4.0a1712578930/setup.cfg
```

### Comparing `pulumi_keycloak-5.4.0a1710156899/PKG-INFO` & `pulumi_keycloak-5.4.0a1712578930/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_keycloak
-Version: 5.4.0a1710156899
+Version: 5.4.0a1712578930
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi,keycloak
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_keycloak-5.4.0a1710156899/README.md` & `pulumi_keycloak-5.4.0a1712578930/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/__init__.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/_inputs.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/_utilities.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/attribute_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/attribute_importer_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/attribute_to_role_identity_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/attribute_to_role_identity_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/bindings.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/bindings.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/execution.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/execution.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/execution_config.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/execution_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/flow.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/authentication/subflow.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/authentication/subflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/config/__init__.pyi` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/config/vars.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/custom_identity_provider_mapping.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/custom_identity_provider_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                  identity_provider_mapper: pulumi.Input[str],
                  realm: pulumi.Input[str],
                  extra_config: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a CustomIdentityProviderMapping resource.
         :param pulumi.Input[str] identity_provider_alias: The alias of the associated identity provider.
-        :param pulumi.Input[str] identity_provider_mapper: The type of the identity provider mapper. This can be a format string that includes a `%!s(MISSING)` - this will be replaced by the provider id.
+        :param pulumi.Input[str] identity_provider_mapper: The type of the identity provider mapper. This can be a format string that includes a `%s` - this will be replaced by the provider id.
         :param pulumi.Input[str] realm: The name of the realm.
         :param pulumi.Input[Mapping[str, Any]] extra_config: Key/value attributes to add to the identity provider mapper model that is persisted to Keycloak. This can be used to extend the base model with new Keycloak features.
         :param pulumi.Input[str] name: The name of the mapper.
         """
         pulumi.set(__self__, "identity_provider_alias", identity_provider_alias)
         pulumi.set(__self__, "identity_provider_mapper", identity_provider_mapper)
         pulumi.set(__self__, "realm", realm)
@@ -47,15 +47,15 @@
     def identity_provider_alias(self, value: pulumi.Input[str]):
         pulumi.set(self, "identity_provider_alias", value)
 
     @property
     @pulumi.getter(name="identityProviderMapper")
     def identity_provider_mapper(self) -> pulumi.Input[str]:
         """
-        The type of the identity provider mapper. This can be a format string that includes a `%!s(MISSING)` - this will be replaced by the provider id.
+        The type of the identity provider mapper. This can be a format string that includes a `%s` - this will be replaced by the provider id.
         """
         return pulumi.get(self, "identity_provider_mapper")
 
     @identity_provider_mapper.setter
     def identity_provider_mapper(self, value: pulumi.Input[str]):
         pulumi.set(self, "identity_provider_mapper", value)
 
@@ -104,15 +104,15 @@
                  identity_provider_mapper: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  realm: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering CustomIdentityProviderMapping resources.
         :param pulumi.Input[Mapping[str, Any]] extra_config: Key/value attributes to add to the identity provider mapper model that is persisted to Keycloak. This can be used to extend the base model with new Keycloak features.
         :param pulumi.Input[str] identity_provider_alias: The alias of the associated identity provider.
-        :param pulumi.Input[str] identity_provider_mapper: The type of the identity provider mapper. This can be a format string that includes a `%!s(MISSING)` - this will be replaced by the provider id.
+        :param pulumi.Input[str] identity_provider_mapper: The type of the identity provider mapper. This can be a format string that includes a `%s` - this will be replaced by the provider id.
         :param pulumi.Input[str] name: The name of the mapper.
         :param pulumi.Input[str] realm: The name of the realm.
         """
         if extra_config is not None:
             pulumi.set(__self__, "extra_config", extra_config)
         if identity_provider_alias is not None:
             pulumi.set(__self__, "identity_provider_alias", identity_provider_alias)
@@ -147,15 +147,15 @@
     def identity_provider_alias(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "identity_provider_alias", value)
 
     @property
     @pulumi.getter(name="identityProviderMapper")
     def identity_provider_mapper(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of the identity provider mapper. This can be a format string that includes a `%!s(MISSING)` - this will be replaced by the provider id.
+        The type of the identity provider mapper. This can be a format string that includes a `%s` - this will be replaced by the provider id.
         """
         return pulumi.get(self, "identity_provider_mapper")
 
     @identity_provider_mapper.setter
     def identity_provider_mapper(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "identity_provider_mapper", value)
 
@@ -240,15 +240,15 @@
         $ pulumi import keycloak:index/customIdentityProviderMapping:CustomIdentityProviderMapping test_mapper my-realm/my-mapper/f446db98-7133-4e30-b18a-3d28fde7ca1b
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] extra_config: Key/value attributes to add to the identity provider mapper model that is persisted to Keycloak. This can be used to extend the base model with new Keycloak features.
         :param pulumi.Input[str] identity_provider_alias: The alias of the associated identity provider.
-        :param pulumi.Input[str] identity_provider_mapper: The type of the identity provider mapper. This can be a format string that includes a `%!s(MISSING)` - this will be replaced by the provider id.
+        :param pulumi.Input[str] identity_provider_mapper: The type of the identity provider mapper. This can be a format string that includes a `%s` - this will be replaced by the provider id.
         :param pulumi.Input[str] name: The name of the mapper.
         :param pulumi.Input[str] realm: The name of the realm.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -359,15 +359,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] extra_config: Key/value attributes to add to the identity provider mapper model that is persisted to Keycloak. This can be used to extend the base model with new Keycloak features.
         :param pulumi.Input[str] identity_provider_alias: The alias of the associated identity provider.
-        :param pulumi.Input[str] identity_provider_mapper: The type of the identity provider mapper. This can be a format string that includes a `%!s(MISSING)` - this will be replaced by the provider id.
+        :param pulumi.Input[str] identity_provider_mapper: The type of the identity provider mapper. This can be a format string that includes a `%s` - this will be replaced by the provider id.
         :param pulumi.Input[str] name: The name of the mapper.
         :param pulumi.Input[str] realm: The name of the realm.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _CustomIdentityProviderMappingState.__new__(_CustomIdentityProviderMappingState)
 
@@ -394,15 +394,15 @@
         """
         return pulumi.get(self, "identity_provider_alias")
 
     @property
     @pulumi.getter(name="identityProviderMapper")
     def identity_provider_mapper(self) -> pulumi.Output[str]:
         """
-        The type of the identity provider mapper. This can be a format string that includes a `%!s(MISSING)` - this will be replaced by the provider id.
+        The type of the identity provider mapper. This can be a format string that includes a `%s` - this will be replaced by the provider id.
         """
         return pulumi.get(self, "identity_provider_mapper")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/custom_user_federation.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/custom_user_federation.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/default_groups.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/default_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/default_roles.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/default_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/generic_client_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/generic_client_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/generic_client_role_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/generic_client_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/generic_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/generic_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/generic_role_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/generic_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_authentication_execution.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_authentication_execution.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_authentication_flow.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_authentication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_client_description_converter.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_client_description_converter.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_group.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_realm.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_realm.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_realm_keys.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_realm_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_role.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_user.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/get_user_realm_roles.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/get_user_realm_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/group.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/group_memberships.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/group_permissions.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/group_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/group_roles.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/group_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/hardcoded_role_identity_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/hardcoded_role_identity_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/__init__.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/_inputs.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/custom_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/custom_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/full_name_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/full_name_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/group_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/group_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/hardcoded_group_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/hardcoded_group_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/hardcoded_role_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/hardcoded_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/msad_user_account_control_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/msad_user_account_control_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/outputs.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/role_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/user_attribute_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/user_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/ldap/user_federation.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/ldap/user_federation.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/oidc/google_identity_provider.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/oidc/google_identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/oidc/identity_provider.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/oidc/identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/__init__.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/_inputs.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/audience_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/audience_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_aggregate_policy.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_aggregate_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_authorization_permission.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_authorization_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_authorization_resource.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_authorization_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_authorization_scope.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_authorization_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_default_scopes.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_default_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_group_policy.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_group_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_js_policy.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_js_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_optional_scopes.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_optional_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_permissions.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_policy.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_role_policy.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_role_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_scope.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_service_account_realm_role.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_service_account_realm_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_service_account_role.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_service_account_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_time_policy.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_time_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/client_user_policy.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/client_user_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/full_name_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/full_name_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/get_client.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/get_client_authorization_policy.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/get_client_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/get_client_scope.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/get_client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/get_client_service_account_user.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/get_client_service_account_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/group_membership_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/group_membership_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/outputs.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/script_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/script_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/user_attribute_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/user_client_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/user_client_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/user_property_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/user_property_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/openid/user_session_note_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/openid/user_session_note_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/outputs.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/provider.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_events.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_aes_generated.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_aes_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_ecdsa_generated.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_ecdsa_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_hmac_generated.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_hmac_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_java_generated.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_java_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_rsa.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_rsa.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_keystore_rsa_generated.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_keystore_rsa_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/realm_user_profile.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/realm_user_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/required_action.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/required_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/role.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/__init__.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/_inputs.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/client.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/client_default_scope.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/client_default_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/client_scope.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/get_client.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/get_client_installation_provider.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/get_client_installation_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/identity_provider.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/outputs.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/script_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/script_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/user_attribute_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/saml/user_property_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/saml/user_property_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/user.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/user_groups.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/user_roles.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/user_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/user_template_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/user_template_importer_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak/users_permissions.py` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak/users_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak.egg-info/PKG-INFO` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_keycloak
-Version: 5.4.0a1710156899
+Version: 5.4.0a1712578930
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi,keycloak
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_keycloak-5.4.0a1710156899/pulumi_keycloak.egg-info/SOURCES.txt` & `pulumi_keycloak-5.4.0a1712578930/pulumi_keycloak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1710156899/pyproject.toml` & `pulumi_keycloak-5.4.0a1712578930/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_keycloak"
   description = "A Pulumi package for creating and managing keycloak cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "keycloak"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "5.4.0a1710156899"
+  version = "5.4.0a1712578930"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-keycloak"
 
 [build-system]
```

