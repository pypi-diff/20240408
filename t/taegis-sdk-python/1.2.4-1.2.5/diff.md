# Comparing `tmp/taegis-sdk-python-1.2.4.tar.gz` & `tmp/taegis-sdk-python-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taegis-sdk-python-1.2.4.tar", last modified: Tue Mar 26 19:08:40 2024, max compression
+gzip compressed data, was "taegis-sdk-python-1.2.5.tar", last modified: Mon Apr  8 15:02:18 2024, max compression
```

## Comparing `taegis-sdk-python-1.2.4.tar` & `taegis-sdk-python-1.2.5.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.197553 taegis-sdk-python-1.2.4/
--rw-rw-rw-   0 root         (0) root         (0)    10173 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2839 2024-03-26 19:08:40.197553 taegis-sdk-python-1.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2119 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 19:08:40.197553 taegis-sdk-python-1.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.161552 taegis-sdk-python-1.2.4/taegis_sdk_python/
--rw-rw-rw-   0 root         (0) root         (0)      895 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/_consts.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-26 19:08:39.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8742 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2636 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    14018 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/service_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.165552 taegis-sdk-python-1.2.4/taegis_sdk_python/services/
--rw-rw-rw-   0 root         (0) root         (0)    17514 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.165552 taegis-sdk-python-1.2.4/taegis_sdk_python/services/access_points/
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/access_points/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2419 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/access_points/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2313 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/access_points/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/access_points/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1377 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/access_points/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.165552 taegis-sdk-python-1.2.4/taegis_sdk_python/services/agent/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/agent/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3167 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/agent/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/agent/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5316 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/agent/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.165552 taegis-sdk-python-1.2.4/taegis_sdk_python/services/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4785 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/alerts/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6011 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/alerts/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/alerts/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    78668 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/alerts/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.169552 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets/
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16354 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23548 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.169552 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets2/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16070 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    42319 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.169552 taegis-sdk-python-1.2.4/taegis_sdk_python/services/audits/
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/audits/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1361 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/audits/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3909 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/audits/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/audits/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    12825 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/audits/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.169552 taegis-sdk-python-1.2.4/taegis_sdk_python/services/authz/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/authz/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3484 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/authz/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14226 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/authz/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/authz/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    13076 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/authz/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.169552 taegis-sdk-python-1.2.4/taegis_sdk_python/services/byoti/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/byoti/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2761 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/byoti/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/byoti/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/byoti/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10026 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/byoti/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.173553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/clients/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4001 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/clients/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/clients/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/clients/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7361 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/clients/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.173553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/collector/
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/collector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17250 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/collector/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    27472 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/collector/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/collector/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    43430 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/collector/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.173553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/comments/
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/comments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4946 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/comments/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7300 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/comments/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/comments/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5118 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/comments/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.173553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/datasources/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/datasources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/datasources/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/datasources/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/datasources/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2862 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/datasources/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.173553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/detector_registry/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/detector_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/detector_registry/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/detector_registry/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/detector_registry/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3164 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/detector_registry/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.177553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_command_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_command_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7325 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_command_manager/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3523 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_command_manager/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8546 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_command_manager/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.177553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_management_service/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_management_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6935 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_management_service/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7179 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_management_service/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    21447 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_management_service/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.177553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/event_search/
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/event_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/event_search/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/event_search/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/event_search/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3609 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/event_search/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.177553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/events/
--rw-rw-rw-   0 root         (0) root         (0)     1215 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1346 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/events/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2775 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/events/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/events/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11044 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.177553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/exports/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/exports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13614 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/exports/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    10457 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/exports/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/exports/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25646 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/exports/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.177553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/fast_ioc/
--rw-rw-rw-   0 root         (0) root         (0)     1201 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/fast_ioc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/fast_ioc/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3177 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/fast_ioc/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/fast_ioc/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/fast_ioc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.181553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/file_info/
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/file_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4508 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/file_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2911 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/file_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/file_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    39710 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/file_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.181553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22228 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    28039 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    37546 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.181553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations2/
--rw-rw-rw-   0 root         (0) root         (0)     1019 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15493 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     8585 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    58884 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.181553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/mitre_attack_info/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/mitre_attack_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/mitre_attack_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9291 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/mitre_attack_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/mitre_attack_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.181553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_context/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4584 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_context/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     4704 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_context/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_context/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6279 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_context/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.185553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_ioc/
--rw-rw-rw-   0 root         (0) root         (0)     1313 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_ioc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_ioc/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3229 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_ioc/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      910 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_ioc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.185553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)      928 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notebooks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notebooks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notebooks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notebooks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.185553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6906 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notifications/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notifications/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notifications/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8811 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/notifications/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.185553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/preferences/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/preferences/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7272 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/preferences/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7360 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/preferences/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/preferences/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    16267 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/preferences/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.185553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/queries/
--rw-rw-rw-   0 root         (0) root         (0)      915 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/queries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3852 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/queries/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/queries/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/queries/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10778 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/queries/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.189553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/roadrunner/
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/roadrunner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/roadrunner/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6420 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/roadrunner/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/roadrunner/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    14157 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/roadrunner/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.189553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/rules/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14238 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/rules/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    17159 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/rules/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/rules/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24776 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/rules/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.189553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/sharelinks/
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/sharelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/sharelinks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/sharelinks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/sharelinks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/sharelinks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.189553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/subjects/
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/subjects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/subjects/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1451 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/subjects/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/subjects/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3651 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/subjects/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.189553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenant_profiles/
--rw-rw-rw-   0 root         (0) root         (0)     1010 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenant_profiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19209 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenant_profiles/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    11166 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenant_profiles/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenant_profiles/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23270 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenant_profiles/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.193553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenants/
--rw-rw-rw-   0 root         (0) root         (0)     1349 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17846 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenants/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7989 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenants/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenants/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    46328 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenants/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.193553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat/
--rw-rw-rw-   0 root         (0) root         (0)      894 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3715 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14808 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    53410 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.193553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat_score/
--rw-rw-rw-   0 root         (0) root         (0)      966 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat_score/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat_score/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat_score/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat_score/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4092 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat_score/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.193553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/trip/
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/trip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/trip/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3993 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/trip/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/trip/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8879 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/trip/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.193553 taegis-sdk-python-1.2.4/taegis_sdk_python/services/users/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12152 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/users/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7321 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/users/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/users/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25986 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/services/users/types.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2024-03-26 19:01:46.000000 taegis-sdk-python-1.2.4/taegis_sdk_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:08:40.193553 taegis-sdk-python-1.2.4/taegis_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2839 2024-03-26 19:08:39.000000 taegis-sdk-python-1.2.4/taegis_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10499 2024-03-26 19:08:40.000000 taegis-sdk-python-1.2.4/taegis_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 19:08:39.000000 taegis-sdk-python-1.2.4/taegis_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      135 2024-03-26 19:08:39.000000 taegis-sdk-python-1.2.4/taegis_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-26 19:08:39.000000 taegis-sdk-python-1.2.4/taegis_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.426053 taegis-sdk-python-1.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)    10173 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2839 2024-04-08 15:02:18.426053 taegis-sdk-python-1.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2119 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 15:02:18.426053 taegis-sdk-python-1.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.370065 taegis-sdk-python-1.2.5/taegis_sdk_python/
+-rw-rw-rw-   0 root         (0) root         (0)      895 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-08 15:02:17.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8742 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2636 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    14018 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/service_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.370065 taegis-sdk-python-1.2.5/taegis_sdk_python/services/
+-rw-rw-rw-   0 root         (0) root         (0)    17514 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.370065 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.374064 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3167 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5316 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.374064 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4785 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6011 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    78668 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.374064 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16354 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23548 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.378063 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16070 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    42319 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.378063 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12825 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.378063 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3484 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14226 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13254 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.382062 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2761 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10026 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.382062 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7361 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.386062 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17250 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    27472 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    43430 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.386062 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4946 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7300 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.386062 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2862 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.390061 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3164 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.390061 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7325 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8618 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.390061 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6935 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7179 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    21447 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.394060 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3609 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.394060 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11022 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.394060 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13614 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10457 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25646 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.394060 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.398059 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4508 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    39710 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.398059 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22228 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    28039 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    37546 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.398059 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15493 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     8585 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    59951 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.402058 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9291 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.402058 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4584 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4704 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6279 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.406057 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/
+-rw-rw-rw-   0 root         (0) root         (0)     1313 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3229 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      910 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.406057 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.406057 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6906 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.406057 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7272 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7360 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    16267 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.410056 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3852 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10778 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.410056 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6420 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14157 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.414056 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14238 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    17159 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24776 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.414056 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.414056 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      850 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3651 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.418055 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19209 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    11166 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23270 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.418055 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17846 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7989 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    46328 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.418055 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/
+-rw-rw-rw-   0 root         (0) root         (0)      894 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13551 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    46416 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.422054 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4092 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.422054 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3993 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8879 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.422054 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12152 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7321 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25986 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.422054 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2839 2024-04-08 15:02:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10499 2024-04-08 15:02:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:02:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2024-04-08 15:02:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-08 15:02:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/top_level.txt
```

### Comparing `taegis-sdk-python-1.2.4/LICENSE` & `taegis-sdk-python-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/PKG-INFO` & `taegis-sdk-python-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.2.4
+Version: 1.2.5
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.2.4/README.md` & `taegis-sdk-python-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/setup.py` & `taegis-sdk-python-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/_consts.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/_consts.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/authentication.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/config.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/config.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/errors.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/errors.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/service_core.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/service_core.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/access_points/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/access_points/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/access_points/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/access_points/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/access_points/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/agent/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/agent/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/agent/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/agent/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/agent/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/alerts/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/alerts/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/alerts/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/alerts/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/alerts/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets2/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets2/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets2/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets2/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/assets2/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/audits/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/audits/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/audits/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/audits/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/audits/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/authz/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/authz/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/authz/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/authz/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/authz/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 class AuthzSupportedFeatureTarget(str, Enum):
     """AuthzSupportedFeatureTarget."""
 
     TENANT = "TENANT"
     CHILD_TENANTS = "CHILD_TENANTS"
+    PARTNER_TENANTS = "PARTNER_TENANTS"
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class Subject:
     """Subject."""
 
@@ -181,14 +182,17 @@
 
     enabled_in_tenant: Optional[bool] = field(
         default=None, metadata=config(field_name="enabledInTenant")
     )
     enabled_in_child_tenants: Optional[bool] = field(
         default=None, metadata=config(field_name="enabledInChildTenants")
     )
+    enabled_in_partner_tenants: Optional[bool] = field(
+        default=None, metadata=config(field_name="enabledInPartnerTenants")
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AuthzPermission:
     """AuthzPermission."""
```

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/byoti/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/byoti/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/byoti/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/byoti/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/byoti/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/clients/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/clients/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/clients/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/clients/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/clients/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/collector/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/collector/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/collector/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/collector/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/collector/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/comments/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/comments/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/comments/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/comments/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/comments/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/datasources/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/datasources/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/datasources/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/datasources/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/datasources/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/detector_registry/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/detector_registry/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/detector_registry/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/detector_registry/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/detector_registry/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_command_manager/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_command_manager/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_command_manager/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_command_manager/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,23 @@
     SHA512 = "SHA512"
 
 
 class FetchRequestPathTypeEnum(str, Enum):
     """FetchRequestPathTypeEnum."""
 
     FILE = "FILE"
+    DIAGNOSTICS = "DIAGNOSTICS"
 
 
 class FetchRequestReasonCodeEnum(str, Enum):
     """FetchRequestReasonCodeEnum."""
 
     REASONCODE_UNSPECIFIED = "REASONCODE_UNSPECIFIED"
     POSSIBLY_MALICIOUS = "POSSIBLY_MALICIOUS"
+    TROUBLESHOOTING = "TROUBLESHOOTING"
 
 
 class StatusEnum(str, Enum):
     """StatusEnum."""
 
     ISSUED = "ISSUED"
     PENDING = "PENDING"
```

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_management_service/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_management_service/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_management_service/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_management_service/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/endpoint_management_service/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/event_search/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/event_search/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/event_search/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/event_search/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/event_search/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/events/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/events/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/events/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/events/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/events/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from dataclasses_json import dataclass_json, config
 
 
 class SearchTarget(str, Enum):
     """SearchTarget."""
 
     ATHENA = "Athena"
-    PRESTO = "Presto"
     ATHENA_HUDI = "AthenaHudi"
     ATHENA_HUDI_STAGING = "AthenaHudiStaging"
 
 
 class BaseType(str, Enum):
     """BaseType."""
```

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/exports/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/exports/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/exports/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/exports/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/exports/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/fast_ioc/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/fast_ioc/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/fast_ioc/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/fast_ioc/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/fast_ioc/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/file_info/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/file_info/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/file_info/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/file_info/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/file_info/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations2/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations2/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations2/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations2/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/investigations2/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,14 +690,22 @@
     """TDRUser."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class TenantV4:
+    """TenantV4."""
+
+    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class Subject:
     """Subject."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
 
 
 @dataclass_json
@@ -892,14 +900,28 @@
     type: Optional[InvestigationType] = field(
         default=None, metadata=config(field_name="type")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class InvestigationTenantCount:
+    """InvestigationTenantCount."""
+
+    tenant_id: Optional[str] = field(
+        default=None, metadata=config(field_name="tenantId")
+    )
+    count: Optional[int] = field(default=None, metadata=config(field_name="count"))
+    tenant: Optional[TenantV4] = field(
+        default=None, metadata=config(field_name="tenant")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class InvestigationsV2Arguments:
     """InvestigationsV2Arguments."""
 
     page: Optional[int] = field(default=None, metadata=config(field_name="page"))
     per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
     cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
     search_children_tenants: Optional[bool] = field(
@@ -1109,14 +1131,30 @@
     visibility: Optional[CommentVisibilityFilter] = field(
         default=None, metadata=config(field_name="visibility")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class InvestigationProcessingStatus:
+    """InvestigationProcessingStatus."""
+
+    assets: Optional[InvestigationProcessingState] = field(
+        default=None, metadata=config(field_name="assets")
+    )
+    events: Optional[InvestigationProcessingState] = field(
+        default=None, metadata=config(field_name="events")
+    )
+    alerts: Optional[InvestigationProcessingState] = field(
+        default=None, metadata=config(field_name="alerts")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class AggregatedCounts:
     """AggregatedCounts."""
 
     archived_count: Optional[int] = field(
         default=None, metadata=config(field_name="archivedCount")
     )
     status: Optional[List[InvestigationStatusCount]] = field(
@@ -1124,29 +1162,16 @@
     )
     type: Optional[List[InvestigationTypeCount]] = field(
         default=None, metadata=config(field_name="type")
     )
     priority: Optional[List[InvestigationPriorityCount]] = field(
         default=None, metadata=config(field_name="priority")
     )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class InvestigationProcessingStatus:
-    """InvestigationProcessingStatus."""
-
-    assets: Optional[InvestigationProcessingState] = field(
-        default=None, metadata=config(field_name="assets")
-    )
-    events: Optional[InvestigationProcessingState] = field(
-        default=None, metadata=config(field_name="events")
-    )
-    alerts: Optional[InvestigationProcessingState] = field(
-        default=None, metadata=config(field_name="alerts")
+    tenant: Optional[List[InvestigationTenantCount]] = field(
+        default=None, metadata=config(field_name="tenant")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationTemplate:
     """InvestigationTemplate."""
@@ -1535,14 +1560,17 @@
     )
     contributor_subjects: Optional[List[Subject]] = field(
         default=None, metadata=config(field_name="contributorSubjects")
     )
     assignee_subject: Optional[Subject] = field(
         default=None, metadata=config(field_name="assigneeSubject")
     )
+    tenant: Optional[TenantV4] = field(
+        default=None, metadata=config(field_name="tenant")
+    )
     created_by: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="createdBy")
     )
     created_by_subject: Optional[Subject] = field(
         default=None, metadata=config(field_name="createdBySubject")
     )
     updated_by: Optional[TDRUser] = field(
@@ -1556,15 +1584,17 @@
     )
     processing_status: Optional[InvestigationProcessingStatus] = field(
         default=None, metadata=config(field_name="processingStatus")
     )
     comments_count: Optional[InvestigationCommentsCount] = field(
         default=None, metadata=config(field_name="commentsCount")
     )
-    metric: Optional[Metric] = field(default=None, metadata=config(field_name="metric"))
+    metrics: Optional[Metric] = field(
+        default=None, metadata=config(field_name="metrics")
+    )
     entities_evidence: Optional[List[EntityEvidence]] = field(
         default=None,
         metadata=config(
             metadata={
                 "deprecated": True,
                 "deprecation_reason": "call the entity api directly",
             },
@@ -1574,14 +1604,21 @@
     assignee: Optional[TDRUser] = field(
         default=None,
         metadata=config(
             metadata={"deprecated": True, "deprecation_reason": "use assigneeSubject"},
             field_name="assignee",
         ),
     )
+    metric: Optional[Metric] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use metrics"},
+            field_name="metric",
+        ),
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationTemplates:
     """InvestigationTemplates."""
```

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/mitre_attack_info/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/mitre_attack_info/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/mitre_attack_info/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/mitre_attack_info/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/mitre_attack_info/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_context/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_context/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_context/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_context/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_context/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_ioc/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_ioc/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_ioc/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/multi_tenant_ioc/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/notebooks/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/notebooks/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/notebooks/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/notebooks/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/notebooks/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/notifications/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/notifications/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/notifications/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/notifications/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/notifications/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/preferences/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/preferences/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/preferences/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/preferences/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/preferences/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/queries/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/queries/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/queries/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/queries/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/queries/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/roadrunner/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/roadrunner/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/roadrunner/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/roadrunner/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/roadrunner/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/rules/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/rules/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/rules/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/rules/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/rules/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/sharelinks/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/sharelinks/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/sharelinks/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/sharelinks/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/sharelinks/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/subjects/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/subjects/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/subjects/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/subjects/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/subjects/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenant_profiles/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenant_profiles/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenant_profiles/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenant_profiles/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenant_profiles/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenants/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenants/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenants/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenants/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/tenants/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/mutations.py`

 * *Files 22% similar despite different names*

```diff
@@ -55,64 +55,7 @@
                 "id": prepare_input(id_),
             },
             output="",
         )
         if result.get(endpoint) is not None:
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for mutation threatDeleteDocument")
-
-    def create_list(self, input_: CreateListInput) -> ThreatList:
-        """None."""
-        endpoint = "createList"
-
-        log.warning(
-            f"GraphQL Mutation `{endpoint}` is deprecated: 'No longer supported'"
-        )
-
-        result = self.service.execute_mutation(
-            endpoint=endpoint,
-            variables={
-                "input": prepare_input(input_),
-            },
-            output=build_output_string(ThreatList),
-        )
-        if result.get(endpoint) is not None:
-            return ThreatList.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for mutation createList")
-
-    def delete_list(self, input_: DeleteListInput) -> bool:
-        """None."""
-        endpoint = "deleteList"
-
-        log.warning(
-            f"GraphQL Mutation `{endpoint}` is deprecated: 'No longer supported'"
-        )
-
-        result = self.service.execute_mutation(
-            endpoint=endpoint,
-            variables={
-                "input": prepare_input(input_),
-            },
-            output="",
-        )
-        if result.get(endpoint) is not None:
-            return result.get(endpoint)
-        raise GraphQLNoRowsInResultSetError("for mutation deleteList")
-
-    def restore_list(self, input_: DeleteListInput) -> bool:
-        """None."""
-        endpoint = "restoreList"
-
-        log.warning(
-            f"GraphQL Mutation `{endpoint}` is deprecated: 'No longer supported'"
-        )
-
-        result = self.service.execute_mutation(
-            endpoint=endpoint,
-            variables={
-                "input": prepare_input(input_),
-            },
-            output="",
-        )
-        if result.get(endpoint) is not None:
-            return result.get(endpoint)
-        raise GraphQLNoRowsInResultSetError("for mutation restoreList")
```

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -166,15 +166,17 @@
             output=build_output_string(ThreatResult),
         )
         if result.get(endpoint) is not None:
             return [parse_union_result(ThreatResult, r) for r in result.get(endpoint)]
         raise GraphQLNoRowsInResultSetError("for query threatGetRelated")
 
     def threat_watchlist(self, type_: ThreatParentType) -> List[ThreatRelationship]:
-        """Gets a watchlist by type. All results are considered **high confidence**.."""
+        """Gets a watchlist by type. All results are considered **high confidence**.
+        Only IP and DOMAIN types are supported. Used the paged service threatTimsMalwareFiles for FILE types..
+        """
         endpoint = "threatWatchlist"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "type": prepare_input(type_),
             },
@@ -182,14 +184,38 @@
         )
         if result.get(endpoint) is not None:
             return ThreatRelationship.schema().load(
                 [r or {} for r in result.get(endpoint)], many=True
             )
         raise GraphQLNoRowsInResultSetError("for query threatWatchlist")
 
+    def threat_tims_malware_files(
+        self, last_created: Optional[str] = None
+    ) -> PagedMalwareFiles:
+        """Get all TIMS 2.0 Malware file hashes. All results are considered **high confidence**.
+        This is a paged service, requiring repeated queries. Total number of results can number over 750k.
+        For the initial query, do not provide any search parameters or set 'last_created' to null.
+        Subsequent queries should include the previous query's 'last_created' result from 'PagedMalwareFiles.last_created'
+        as the input parameter. Returns pages of 10,000 at a time, sorted by the indicators field 'created' in desc order.
+        The returned field 'has_more' will be false when the last page is returned.
+        * Note: 'created' refers to an internal field associated with the indicator, not the time the indicator was first found.
+        It is only used for sorting.."""
+        endpoint = "threatTimsMalwareFiles"
+
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={
+                "last_created": prepare_input(last_created),
+            },
+            output=build_output_string(PagedMalwareFiles),
+        )
+        if result.get(endpoint) is not None:
+            return PagedMalwareFiles.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for query threatTimsMalwareFiles")
+
     def threat_indicator_publications(self, id_: str) -> List[ThreatReport]:
         """Gets publications related to indicators.."""
         endpoint = "threatIndicatorPublications"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
@@ -311,78 +337,7 @@
             output=build_output_string(ThreatIndicatorIntelligence),
         )
         if result.get(endpoint) is not None:
             return ThreatIndicatorIntelligence.schema().load(
                 [r or {} for r in result.get(endpoint)], many=True
             )
         raise GraphQLNoRowsInResultSetError("for query threatIndicatorsIntelligence")
-
-    def lists(self, arguments: ListsArguments) -> Lists:
-        """Retrieves Custom Lists for the respective tenant."""
-        endpoint = "lists"
-
-        log.warning(f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported'")
-
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={
-                "arguments": prepare_input(arguments),
-            },
-            output=build_output_string(Lists),
-        )
-        if result.get(endpoint) is not None:
-            return Lists.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for query lists")
-
-    def list(self, id_: str, arguments: ListsArguments) -> ThreatList:
-        """Retrieves a custom list by ID."""
-        endpoint = "list"
-
-        log.warning(f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported'")
-
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={
-                "id": prepare_input(id_),
-                "arguments": prepare_input(arguments),
-            },
-            output=build_output_string(ThreatList),
-        )
-        if result.get(endpoint) is not None:
-            return ThreatList.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for query list")
-
-    def list_items_by_tag(self, tag: str, arguments: ListsArguments) -> ListItems:
-        """Retrieves list items that contains the specified tag (case sensitive)."""
-        endpoint = "listItemsByTag"
-
-        log.warning(f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported'")
-
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={
-                "tag": prepare_input(tag),
-                "arguments": prepare_input(arguments),
-            },
-            output=build_output_string(ListItems),
-        )
-        if result.get(endpoint) is not None:
-            return ListItems.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for query listItemsByTag")
-
-    def list_items_by_name(self, name: str, arguments: ListsArguments) -> ListItems:
-        """Retrieves list items by indicator name."""
-        endpoint = "listItemsByName"
-
-        log.warning(f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported'")
-
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={
-                "name": prepare_input(name),
-                "arguments": prepare_input(arguments),
-            },
-            output=build_output_string(ListItems),
-        )
-        if result.get(endpoint) is not None:
-            return ListItems.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for query listItemsByName")
```

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     STATIC_ANALYSIS_OF = "static_analysis_of"
     DYNAMIC_ANALYSIS_OF = "dynamic_analysis_of"
     LISTS = "lists"
     LISTED_ON = "listed_on"
     RELATED_TO = "related_to"
     INDIRECT = "indirect"
     HAS_VID = "has_vid"
+    HOSTED_ON = "hosted_on"
 
 
 class ThreatMalwareType(str, Enum):
     """ThreatMalwareType."""
 
     ADWARE = "adware"
     BACKDOOR = "backdoor"
@@ -263,46 +264,14 @@
     IDENTITY = "identity"
     RELATIONSHIP = "relationship"
     MALWARE = "malware"
     INTRUSIONSET = "intrusionset"
     REPORT = "report"
 
 
-class ListAction(str, Enum):
-    """ListAction."""
-
-    ALLOW = "allow"
-    BLOCK = "block"
-    WARN = "warn"
-
-
-class ItemType(str, Enum):
-    """ItemType."""
-
-    USER = "user"
-    CERTIFICATE = "certificate"
-    ASSET = "asset"
-    DOMAIN = "domain"
-    IPV4 = "ipv4"
-    IPV6 = "ipv6"
-    CIDR = "cidr"
-    URL = "url"
-    MD5 = "md5"
-    SHA256 = "sha256"
-    SHA1 = "sha1"
-    UNKNOWN = "unknown"
-
-
-class OrderByOptions(str, Enum):
-    """OrderByOptions."""
-
-    ASC = "asc"
-    DESC = "desc"
-
-
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class PageInfo:
     """PageInfo."""
 
     end_cursor: Optional[str] = field(
         default=None, metadata=config(field_name="endCursor")
@@ -523,14 +492,36 @@
     latitude: Optional[float] = field(
         default=None, metadata=config(field_name="Latitude")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class TimsMalwareFile:
+    """TimsMalwareFile."""
+
+    file_hash: Optional[str] = field(
+        default=None, metadata=config(field_name="file_hash")
+    )
+    information_source: Optional[str] = field(
+        default=None, metadata=config(field_name="information_source")
+    )
+    threat_description: Optional[str] = field(
+        default=None, metadata=config(field_name="threat_description")
+    )
+    confidence: Optional[int] = field(
+        default=None, metadata=config(field_name="confidence")
+    )
+    source_internal: Optional[bool] = field(
+        default=None, metadata=config(field_name="source_internal")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class ThreatWhois:
     """ThreatWhois."""
 
     domain_name: Optional[str] = field(
         default=None, metadata=config(field_name="DomainName")
     )
     registrar_name: Optional[str] = field(
@@ -727,43 +718,14 @@
     )
     content: Optional[str] = field(default=None, metadata=config(field_name="content"))
     tags: Optional[List[str]] = field(default=None, metadata=config(field_name="tags"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class ListOwner:
-    """ListOwner."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    tenant_id: Optional[str] = field(
-        default=None, metadata=config(field_name="tenant_id")
-    )
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="created_at")
-    )
-    modified_at: Optional[str] = field(
-        default=None, metadata=config(field_name="modified_at")
-    )
-    age_at: Optional[str] = field(default=None, metadata=config(field_name="age_at"))
-    deleted_at: Optional[str] = field(
-        default=None, metadata=config(field_name="deleted_at")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class DeleteListInput:
-    """DeleteListInput."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class ThreatGroup:
     """ThreatGroup."""
 
     spec_version: Optional[str] = field(
         default=None, metadata=config(field_name="spec_version")
     )
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
@@ -802,14 +764,30 @@
     type: Optional[ThreatObjectType] = field(
         default=None, metadata=config(field_name="type")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class PagedMalwareFiles:
+    """PagedMalwareFiles."""
+
+    last_created: Optional[str] = field(
+        default=None, metadata=config(field_name="last_created")
+    )
+    has_more: Optional[bool] = field(
+        default=None, metadata=config(field_name="has_more")
+    )
+    files: Optional[List[TimsMalwareFile]] = field(
+        default=None, metadata=config(field_name="files")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class ThreatReport:
     """ThreatReport."""
 
     spec_version: Optional[str] = field(
         default=None, metadata=config(field_name="spec_version")
     )
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
@@ -835,137 +813,14 @@
     type: Optional[ThreatObjectType] = field(
         default=None, metadata=config(field_name="type")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class ListItem:
-    """ListItem."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    reference_id: Optional[str] = field(
-        default=None, metadata=config(field_name="reference_id")
-    )
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
-    description: Optional[str] = field(
-        default=None, metadata=config(field_name="description")
-    )
-    confidence: Optional[int] = field(
-        default=None, metadata=config(field_name="confidence")
-    )
-    severity: Optional[int] = field(
-        default=None, metadata=config(field_name="severity")
-    )
-    tags: Optional[List[str]] = field(default=None, metadata=config(field_name="tags"))
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="created_at")
-    )
-    modified_at: Optional[str] = field(
-        default=None, metadata=config(field_name="modified_at")
-    )
-    age_at: Optional[str] = field(default=None, metadata=config(field_name="age_at"))
-    deleted_at: Optional[str] = field(
-        default=None, metadata=config(field_name="deleted_at")
-    )
-    item_type: Optional[ItemType] = field(
-        default=None, metadata=config(field_name="item_type")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class ListInfo:
-    """ListInfo."""
-
-    list_id: Optional[str] = field(default=None, metadata=config(field_name="list_id"))
-    list_item_count: Optional[int] = field(
-        default=None, metadata=config(field_name="list_item_count")
-    )
-    list_name: Optional[str] = field(
-        default=None, metadata=config(field_name="list_name")
-    )
-    list_action: Optional[ListAction] = field(
-        default=None, metadata=config(field_name="list_action")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class Lists:
-    """Lists."""
-
-    list_info: Optional[List[ListInfo]] = field(
-        default=None, metadata=config(field_name="list_info")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class ListItemToList:
-    """ListItemToList."""
-
-    list_id: Optional[str] = field(default=None, metadata=config(field_name="listID"))
-    list_name: Optional[str] = field(
-        default=None, metadata=config(field_name="listName")
-    )
-    list_item: Optional[ListItem] = field(
-        default=None, metadata=config(field_name="listItem")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class ListItems:
-    """ListItems."""
-
-    list_item_map: Optional[List[ListItemToList]] = field(
-        default=None, metadata=config(field_name="listItemMap")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class ListItemInput:
-    """ListItemInput."""
-
-    reference_id: Optional[str] = field(
-        default=None, metadata=config(field_name="reference_id")
-    )
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
-    description: Optional[str] = field(
-        default=None, metadata=config(field_name="description")
-    )
-    confidence: Optional[int] = field(
-        default=None, metadata=config(field_name="confidence")
-    )
-    severity: Optional[int] = field(
-        default=None, metadata=config(field_name="severity")
-    )
-    tags: Optional[List[str]] = field(default=None, metadata=config(field_name="tags"))
-    item_type: Optional[ItemType] = field(
-        default=None, metadata=config(field_name="item_type")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class ListsArguments:
-    """ListsArguments."""
-
-    global_: Optional[bool] = field(default=None, metadata=config(field_name="global"))
-    page: Optional[int] = field(default=None, metadata=config(field_name="page"))
-    per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
-    order_by: Optional[OrderByOptions] = field(
-        default=None, metadata=config(field_name="orderBy")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class ThreatIdentityInput:
     """ThreatIdentityInput."""
 
     name: Optional[str] = field(default=None, metadata=config(field_name="name"))
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
     )
@@ -996,41 +851,14 @@
     sectors: Optional[List[ThreatIndustrySectors]] = field(
         default=None, metadata=config(field_name="sectors")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class CreateListInput:
-    """CreateListInput."""
-
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
-    description: Optional[str] = field(
-        default=None, metadata=config(field_name="description")
-    )
-    download_url: Optional[str] = field(
-        default=None, metadata=config(field_name="download_url")
-    )
-    confidence: Optional[int] = field(
-        default=None, metadata=config(field_name="confidence")
-    )
-    severity: Optional[int] = field(
-        default=None, metadata=config(field_name="severity")
-    )
-    tags: Optional[List[str]] = field(default=None, metadata=config(field_name="tags"))
-    items: Optional[List[ListItemInput]] = field(
-        default=None, metadata=config(field_name="items")
-    )
-    list_action: Optional[ListAction] = field(
-        default=None, metadata=config(field_name="list_action")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class ThreatVid:
     """ThreatVid."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="ID"))
     name: Optional[str] = field(default=None, metadata=config(field_name="Name"))
     swids: Optional[List[ThreatSwid]] = field(
         default=None, metadata=config(field_name="Swids")
@@ -1250,62 +1078,14 @@
     kill_chain_phases: Optional[List[ThreatKillChainPhaseInput]] = field(
         default=None, metadata=config(field_name="kill_chain_phases")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class ThreatList:
-    """ThreatList."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
-    description: Optional[str] = field(
-        default=None, metadata=config(field_name="description")
-    )
-    download_url: Optional[str] = field(
-        default=None, metadata=config(field_name="download_url")
-    )
-    item_count: Optional[int] = field(
-        default=None, metadata=config(field_name="item_count")
-    )
-    global_: Optional[bool] = field(default=None, metadata=config(field_name="global"))
-    internal: Optional[bool] = field(
-        default=None, metadata=config(field_name="internal")
-    )
-    confidence: Optional[int] = field(
-        default=None, metadata=config(field_name="confidence")
-    )
-    severity: Optional[int] = field(
-        default=None, metadata=config(field_name="severity")
-    )
-    tags: Optional[List[str]] = field(default=None, metadata=config(field_name="tags"))
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="created_at")
-    )
-    modified_at: Optional[str] = field(
-        default=None, metadata=config(field_name="modified_at")
-    )
-    age_at: Optional[str] = field(default=None, metadata=config(field_name="age_at"))
-    deleted_at: Optional[str] = field(
-        default=None, metadata=config(field_name="deleted_at")
-    )
-    owner: Optional[ListOwner] = field(
-        default=None, metadata=config(field_name="owner")
-    )
-    items: Optional[List[ListItem]] = field(
-        default=None, metadata=config(field_name="items")
-    )
-    list_action: Optional[ListAction] = field(
-        default=None, metadata=config(field_name="list_action")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class ThreatMalware:
     """ThreatMalware."""
 
     spec_version: Optional[str] = field(
         default=None, metadata=config(field_name="spec_version")
     )
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
```

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat_score/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat_score/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat_score/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat_score/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/threat_score/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/trip/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/trip/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/trip/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/trip/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/trip/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/users/__init__.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/users/mutations.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/users/queries.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/users/subscriptions.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/services/users/types.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/tokens.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/tokens.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python/utils.py` & `taegis-sdk-python-1.2.5/taegis_sdk_python/utils.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python.egg-info/PKG-INFO` & `taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.2.4
+Version: 1.2.5
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.2.4/taegis_sdk_python.egg-info/SOURCES.txt` & `taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

