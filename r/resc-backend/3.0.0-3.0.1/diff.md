# Comparing `tmp/resc_backend-3.0.0.tar.gz` & `tmp/resc_backend-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_backend-3.0.0.tar", last modified: Fri Feb  2 13:56:52 2024, max compression
+gzip compressed data, was "resc_backend-3.0.1.tar", last modified: Mon Apr  8 09:09:33 2024, max compression
```

## Comparing `resc_backend-3.0.0.tar` & `resc_backend-3.0.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.829447 resc_backend-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-02 13:56:44.000000 resc_backend-3.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-02-02 13:56:52.829447 resc_backend-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-02-02 13:56:44.000000 resc_backend-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-02 13:56:52.829447 resc_backend-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-02 13:56:44.000000 resc_backend-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.809446 resc_backend-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.813446 resc_backend-3.0.0/src/resc_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.813446 resc_backend-3.0.0/src/resc_backend/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/bin/rabbitmq_bootup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.813446 resc_backend-3.0.0/src/resc_backend/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.817447 resc_backend-3.0.0/src/resc_backend/db/model/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/db/model/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.817447 resc_backend-3.0.0/src/resc_backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/helpers/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/helpers/git_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.817447 resc_backend-3.0.0/src/resc_backend/helpers/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/helpers/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/helpers/rabbitmq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.817447 resc_backend-3.0.0/src/resc_backend/resc_web_service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.821447 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16301 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    39847 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.821447 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    13748 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    22520 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    17671 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    15716 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.825446 resc_backend-3.0.0/src/resc_backend/resc_web_service/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/helpers/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.829447 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/date_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/date_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/finding_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/status_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/time_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.829447 resc_backend-3.0.0/src/resc_backend/resc_web_service_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service_interface/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service_interface/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service_interface/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service_interface/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-02 13:56:44.000000 resc_backend-3.0.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:56:52.829447 resc_backend-3.0.0/src/resc_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-02-02 13:56:52.000000 resc_backend-3.0.0/src/resc_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-02-02 13:56:52.000000 resc_backend-3.0.0/src/resc_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 13:56:52.000000 resc_backend-3.0.0/src/resc_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-02 13:56:52.000000 resc_backend-3.0.0/src/resc_backend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 13:56:52.000000 resc_backend-3.0.0/src/resc_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-02 13:56:52.000000 resc_backend-3.0.0/src/resc_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-02 13:56:52.000000 resc_backend-3.0.0/src/resc_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.774733 resc_backend-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 09:09:29.000000 resc_backend-3.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-08 09:09:33.774733 resc_backend-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-08 09:09:29.000000 resc_backend-3.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-08 09:09:33.774733 resc_backend-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 09:09:29.000000 resc_backend-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.758733 resc_backend-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.758733 resc_backend-3.0.1/src/resc_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.762733 resc_backend-3.0.1/src/resc_backend/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/bin/rabbitmq_bootup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.762733 resc_backend-3.0.1/src/resc_backend/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/engine_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.762733 resc_backend-3.0.1/src/resc_backend/db/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/db/model/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.762733 resc_backend-3.0.1/src/resc_backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/helpers/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/helpers/environment_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.762733 resc_backend-3.0.1/src/resc_backend/helpers/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/helpers/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/helpers/rabbitmq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.766733 resc_backend-3.0.1/src/resc_backend/resc_web_service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.766733 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38141 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18001 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.770733 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13093 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20677 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17691 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.770733 resc_backend-3.0.1/src/resc_backend/resc_web_service/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/helpers/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/helpers/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.774733 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/date_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/date_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/finding_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/finding_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/repository_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/rule_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/status_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/time_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.774733 resc_backend-3.0.1/src/resc_backend/resc_web_service_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service_interface/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service_interface/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service_interface/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service_interface/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-08 09:09:29.000000 resc_backend-3.0.1/src/resc_backend/resc_web_service_interface/vcs_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:09:33.762733 resc_backend-3.0.1/src/resc_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-08 09:09:33.000000 resc_backend-3.0.1/src/resc_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-08 09:09:33.000000 resc_backend-3.0.1/src/resc_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:09:33.000000 resc_backend-3.0.1/src/resc_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 09:09:33.000000 resc_backend-3.0.1/src/resc_backend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:09:33.000000 resc_backend-3.0.1/src/resc_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-08 09:09:33.000000 resc_backend-3.0.1/src/resc_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 09:09:33.000000 resc_backend-3.0.1/src/resc_backend.egg-info/top_level.txt
```

### Comparing `resc_backend-3.0.0/LICENSE.md` & `resc_backend-3.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.0/src/resc_backend/bin/rabbitmq_bootup.py` & `resc_backend-3.0.1/src/resc_backend/bin/rabbitmq_bootup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-# pylint: disable=E1101
 # Standard Library
 import logging
 import sys
 from argparse import ArgumentParser, Namespace
 
 # First Party
 from resc_backend.helpers.environment_wrapper import validate_environment
 from resc_backend.helpers.rabbitmq.configuration import (
     REQUIRED_ENV_VARS,
     RESC_RABBITMQ_SERVICE_HOST,
-    RESC_RABBITMQ_SERVICE_PORT_MGMT
+    RESC_RABBITMQ_SERVICE_PORT_MGMT,
 )
 from resc_backend.helpers.rabbitmq.rabbitmq_initialization import (
     create_queue_user_and_set_permission,
-    wait_for_rabbitmq_server_to_up
+    wait_for_rabbitmq_server_to_up,
 )
 
 env_variables = validate_environment(REQUIRED_ENV_VARS)
 logger = logging.getLogger(__name__)
 
 
 def create_cli_argparser() -> ArgumentParser:
     rabbitmq_service_host = f"{env_variables[RESC_RABBITMQ_SERVICE_HOST]}"
     rabbitmq_service_port = f"{env_variables[RESC_RABBITMQ_SERVICE_PORT_MGMT]}"
-    rabbitmq_api_base_url = "http://" + rabbitmq_service_host + ":" + rabbitmq_service_port
+    rabbitmq_api_base_url = (
+        "http://" + rabbitmq_service_host + ":" + rabbitmq_service_port
+    )
 
     parser: ArgumentParser = ArgumentParser()
-    parser.add_argument("--rabbitmq-url", type=str, default=rabbitmq_api_base_url,
-                        help="RabbitMQ URL")
+    parser.add_argument(
+        "--rabbitmq-url", type=str, default=rabbitmq_api_base_url, help="RabbitMQ URL"
+    )
 
     return parser
 
 
-def validate_cli_arguments(args: Namespace):  # pylint: disable=R0912
+def validate_cli_arguments(args: Namespace):
     valid_arguments = True
     if not args.rabbitmq_url:
         logger.error("RabbtMQ URL needs to be specified")
         valid_arguments = False
     if not valid_arguments:
         return False
     return args
@@ -46,14 +48,16 @@
     """
     This function creates users in RabbitMQ server along with required permissions.
     """
     parser: ArgumentParser = create_cli_argparser()
     args: Namespace = parser.parse_args()
     args = validate_cli_arguments(args)
     if not args:
-        logger.error("CLI arguments validation failed while bootstrapping rabbitmq users")
+        logger.error(
+            "CLI arguments validation failed while bootstrapping rabbitmq users"
+        )
         sys.exit(-1)
 
     server_up = wait_for_rabbitmq_server_to_up(rabbitmq_api_base_url=args.rabbitmq_url)
     if not server_up:
         raise TimeoutError("Wait for rabbitmq server to up has been failed.")
     create_queue_user_and_set_permission(rabbitmq_api_base_url=args.rabbitmq_url)
```

### Comparing `resc_backend-3.0.0/src/resc_backend/common.py` & `resc_backend-3.0.1/src/resc_backend/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,20 @@
         base_dir = path.dirname(__file__)
 
     return base_dir + "/static/logging.ini"
 
 
 def initialise_logs(log_file_path: str, debug=True):
     logging_ini_file = get_logging_settings_path()
-    logging.config.fileConfig(logging_ini_file, defaults={'log_file_path': log_file_path},
-                              disable_existing_loggers=False)
-    logger_config = logging.getLogger('root')
+    logging.config.fileConfig(
+        logging_ini_file,
+        defaults={"log_file_path": log_file_path},
+        disable_existing_loggers=False,
+    )
+    logger_config = logging.getLogger("root")
     if int(debug) == 1:
         logger_config.setLevel(logging.DEBUG)
     else:
         logger_config.setLevel(logging.INFO)
     return logger_config
```

### Comparing `resc_backend-3.0.0/src/resc_backend/constants.py` & `resc_backend-3.0.1/src/resc_backend/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,25 +75,29 @@
 # Logging
 LOG_FILE_PATH_RABBITMQ = "rabbitmq_initialization.log"
 LOG_FILE_CACHING = "redis_cache.log"
 LOGGING_FILE = "logging.ini"
 
 # Error message
 ERROR_MESSAGE_500 = "Internal server error. Contact your system administrator"
-ERROR_MESSAGE_503 = "Unable to communicate with DataBase, Please contact your system administrator"
+ERROR_MESSAGE_503 = (
+    "Unable to communicate with DataBase, Please contact your system administrator"
+)
 
 # Redis Cache
-REDIS_CACHE_EXPIRE = 60*60*24  # set to 24 hours
+REDIS_CACHE_EXPIRE = 60 * 60 * 24  # set to 24 hours
 
 # HTTP Security Response Headers
 STRICT_TRANSPORT_SECURITY = "max-age=31536000; includeSubDomains; preload"
 CACHE_CONTROL = "no-cache, no-store"
 CROSS_ORIGIN_RESOURCE_POLICY = "same-site"
 REFERRER_POLICY = "same-origin"
 X_PERMITTED_CROSS_DOMAIN_POLICIES = "none"
 X_CONTENT_TYPE_OPTIONS = "nosniff"
 X_FRAME_OPTIONS = "DENY"
 X_XSS_PROTECTION = "1; mode=block"
-CONTENT_SECURITY_POLICY = "default-src 'none'; script-src 'self' https://cdn.jsdelivr.net 'unsafe-inline'; " \
-                          "connect-src 'self'; img-src 'self' https://fastapi.tiangolo.com data:;style-src " \
-                          "'self' https://fonts.googleapis.com https://cdn.jsdelivr.net 'unsafe-inline';" \
-                          "frame-ancestors 'self'; form-action 'self';"
+CONTENT_SECURITY_POLICY = (
+    "default-src 'none'; script-src 'self' https://cdn.jsdelivr.net 'unsafe-inline'; "
+    "connect-src 'self'; img-src 'self' https://fastapi.tiangolo.com data:;style-src "
+    "'self' https://fonts.googleapis.com https://cdn.jsdelivr.net 'unsafe-inline';"
+    "frame-ancestors 'self'; form-action 'self';"
+)
```

### Comparing `resc_backend-3.0.0/src/resc_backend/db/connection.py` & `resc_backend-3.0.1/src/resc_backend/db/connection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# pylint: disable=C0413
 # Standard Library
 import logging
 import os
 import urllib
 
 # Third Party
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 
 # First Party
+from resc_backend.db.engine_azure import create_azure_engine
 from resc_backend.db.model import Base
 
 basedir = os.path.abspath(os.path.dirname(__file__))
 logger = logging.getLogger(__name__)
 
 DB_CONNECTION_STRING = os.environ.get("DB_CONNECTION_STRING")
 try:
@@ -25,21 +25,47 @@
     DB_CONNECTION_STRING = DB_CONNECTION_STRING.format(**env_variables)
 except AttributeError:
     logger.warning("Missing DB Connection environment variables, using SQLite database")
     DB_CONNECTION_STRING = ""
 SQL_ALCHEMY_POOL_SIZE_DEFAULT = 25
 SQL_ALCHEMY_MAX_OVERFLOW_DEFAULT = 15
 
-echo_queries = os.getenv('SQL_ALCHEMY_ECHO_QUERIES', 'False').lower() in ('true', '1', 'y')
+echo_queries = os.getenv("SQL_ALCHEMY_ECHO_QUERIES", "False").lower() in (
+    "true",
+    "1",
+    "y",
+)
 pool_size = int(os.environ.get("SQL_ALCHEMY_POOL_SIZE", SQL_ALCHEMY_POOL_SIZE_DEFAULT))
-max_overflow = int(os.environ.get("SQL_ALCHEMY_MAX_OVERFLOW", SQL_ALCHEMY_MAX_OVERFLOW_DEFAULT))
+max_overflow = int(
+    os.environ.get("SQL_ALCHEMY_MAX_OVERFLOW", SQL_ALCHEMY_MAX_OVERFLOW_DEFAULT)
+)
 
 if DB_CONNECTION_STRING:
     logger.info("Using provided environment variable to connect to the Database")
-    engine = create_engine(DB_CONNECTION_STRING, echo=echo_queries, pool_size=pool_size, max_overflow=max_overflow)
+    use_azure_token_auth = os.environ.get(
+        "DB_USE_AZURE_TOKEN_AUTH", "False"
+    ).lower() in ("true", "1", "y")
+    if use_azure_token_auth:
+        engine = create_azure_engine(
+            connection_string=DB_CONNECTION_STRING,
+            echo_queries=echo_queries,
+            pool_size=pool_size,
+            max_overflow=max_overflow,
+        )
+    else:
+        engine = create_engine(
+            DB_CONNECTION_STRING,
+            echo=echo_queries,
+            pool_size=pool_size,
+            max_overflow=max_overflow,
+        )
 else:
-    DATABASE_URL = 'sqlite:///' + os.path.join(basedir, 'db.sqlite?check_same_thread=False')
-    logger.info(f"Database environment variables were not provided, defaulting to {DATABASE_URL}")
+    DATABASE_URL = "sqlite:///" + os.path.join(
+        basedir, "db.sqlite?check_same_thread=False"
+    )
+    logger.info(
+        f"Database environment variables were not provided, defaulting to {DATABASE_URL}"
+    )
     engine = create_engine(DATABASE_URL, echo=echo_queries)
     Base.metadata.create_all(engine, checkfirst=True)
 
 Session = sessionmaker()
```

### Comparing `resc_backend-3.0.0/src/resc_backend/db/model/__init__.py` & `resc_backend-3.0.1/src/resc_backend/db/model/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# pylint: disable=C0413
+# ruff: noqa: E402
+# ruff: noqa: F401
 # Standard Library
 import logging
 import os
 
 # Third Party
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base()
 basedir = os.path.abspath(os.path.dirname(__file__))
 logger = logging.getLogger(__name__)
 
-
 # First Party
 from resc_backend.db.model.audit import DBaudit
 from resc_backend.db.model.finding import DBfinding
 from resc_backend.db.model.repository import DBrepository
 from resc_backend.db.model.rule import DBrule
 from resc_backend.db.model.rule_allow_list import DBruleAllowList
 from resc_backend.db.model.rule_pack import DBrulePack
```

### Comparing `resc_backend-3.0.0/src/resc_backend/db/model/audit.py` & `resc_backend-3.0.1/src/resc_backend/db/model/audit.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,32 +10,38 @@
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 
 
 class DBaudit(Base):
     __tablename__ = "audit"
     id_ = Column("id", Integer, primary_key=True)
     finding_id = Column(Integer, ForeignKey("finding.id"), nullable=False)
-    status = Column(Enum(FindingStatus), default=FindingStatus.NOT_ANALYZED, server_default="NOT_ANALYZED",
-                    nullable=False)
+    status = Column(
+        Enum(FindingStatus),
+        default=FindingStatus.NOT_ANALYZED,
+        server_default="NOT_ANALYZED",
+        nullable=False,
+    )
     auditor = Column(String(200))
     comment = Column(String(255), nullable=True)
     timestamp = Column(DateTime, nullable=False, default=datetime.utcnow)
 
     def __init__(self, finding_id, status, auditor, comment, timestamp):
         sanitized_comment = html.escape(comment) if comment else comment
         self.finding_id = finding_id
         self.status = status
         self.auditor = auditor
         self.comment = sanitized_comment
         self.timestamp = timestamp
 
     @staticmethod
-    def create_from_metadata(finding_id: int, status: str, auditor: str, comment: str, timestamp: datetime):
+    def create_from_metadata(
+        finding_id: int, status: str, auditor: str, comment: str, timestamp: datetime
+    ):
         sanitized_comment = html.escape(comment) if comment else comment
         db_audit = DBaudit(
             finding_id=finding_id,
             auditor=auditor,
             status=status,
             comment=sanitized_comment,
-            timestamp=timestamp
+            timestamp=timestamp,
         )
         return db_audit
```

### Comparing `resc_backend-3.0.0/src/resc_backend/db/model/finding.py` & `resc_backend-3.0.1/src/resc_backend/db/model/finding.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-# pylint: disable=R0902
 # Standard Library
 from datetime import datetime
 
 # Third Party
-from sqlalchemy import Column, DateTime, ForeignKey, Integer, String, Text, UniqueConstraint
+from sqlalchemy import (
+    Column,
+    DateTime,
+    ForeignKey,
+    Integer,
+    String,
+    Text,
+    UniqueConstraint,
+)
 
 # First Party
 from resc_backend.db.model import Base
 
 
 class DBfinding(Base):
     __tablename__ = "finding"
@@ -21,19 +28,42 @@
     commit_id = Column(String(120))
     commit_message = Column(Text)
     commit_timestamp = Column(DateTime, default=datetime.utcnow().isoformat())
     author = Column(String(200))
     email = Column(String(100))
     event_sent_on = Column(DateTime, nullable=True)
 
-    __table_args__ = (UniqueConstraint("commit_id", "repository_id", "rule_name", "file_path", "line_number",
-                                       "column_start", "column_end", name="uc_finding_per_repository"),)
-
-    def __init__(self, rule_name, file_path, line_number, commit_id, commit_message, commit_timestamp, author,
-                 email, event_sent_on, repository_id, column_start, column_end):
+    __table_args__ = (
+        UniqueConstraint(
+            "commit_id",
+            "repository_id",
+            "rule_name",
+            "file_path",
+            "line_number",
+            "column_start",
+            "column_end",
+            name="uc_finding_per_repository",
+        ),
+    )
+
+    def __init__(
+        self,
+        rule_name,
+        file_path,
+        line_number,
+        commit_id,
+        commit_message,
+        commit_timestamp,
+        author,
+        email,
+        event_sent_on,
+        repository_id,
+        column_start,
+        column_end,
+    ):
         self.email = email
         self.author = author
         self.commit_timestamp = commit_timestamp
         self.commit_message = commit_message
         self.commit_id = commit_id
         self.line_number = line_number
         self.file_path = file_path
@@ -53,10 +83,10 @@
             commit_id=finding.commit_id,
             commit_message=finding.commit_message,
             commit_timestamp=finding.commit_timestamp,
             author=finding.author,
             event_sent_on=finding.event_sent_on,
             repository_id=finding.repository_id,
             column_start=finding.column_start,
-            column_end=finding.column_end
+            column_end=finding.column_end,
         )
         return db_finding
```

### Comparing `resc_backend-3.0.0/src/resc_backend/db/model/repository.py` & `resc_backend-3.0.1/src/resc_backend/db/model/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,35 @@
     __tablename__ = "repository"
     id_ = Column("id", Integer, primary_key=True)
     vcs_instance = Column(Integer, ForeignKey("vcs_instance.id"), nullable=False)
     project_key = Column(String(100), nullable=False)
     repository_id = Column(String(100), nullable=False)
     repository_name = Column(String(100), nullable=False)
     repository_url = Column(String(200), nullable=False)
-    __table_args__ = (UniqueConstraint("project_key", "repository_id", "vcs_instance",
-                                       name="unique_repository_id_per_project"),)
+    __table_args__ = (
+        UniqueConstraint(
+            "project_key",
+            "repository_id",
+            "vcs_instance",
+            name="unique_repository_id_per_project",
+        ),
+    )
 
-    def __init__(self, project_key, repository_id, repository_name, repository_url, vcs_instance):
+    def __init__(
+        self, project_key, repository_id, repository_name, repository_url, vcs_instance
+    ):
         self.project_key = project_key
         self.repository_id = repository_id
         self.repository_name = repository_name
         self.repository_url = repository_url
         self.vcs_instance = vcs_instance
 
     @staticmethod
     def create_from_repository(repository: Repository):
         db_repository = DBrepository(
             project_key=repository.project_key,
             repository_id=repository.repository_id,
             repository_name=repository.repository_name,
             repository_url=repository.repository_url,
-            vcs_instance=repository.vcs_instance
+            vcs_instance=repository.vcs_instance,
         )
         return db_repository
```

### Comparing `resc_backend-3.0.0/src/resc_backend/db/model/rule.py` & `resc_backend-3.0.1/src/resc_backend/db/model/rule.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,17 @@
-# pylint: disable=R0902
 # Third Party
-from sqlalchemy import Column, Float, ForeignKey, Integer, String, Text, UniqueConstraint
+from sqlalchemy import (
+    Column,
+    Float,
+    ForeignKey,
+    Integer,
+    String,
+    Text,
+    UniqueConstraint,
+)
 
 # First Party
 from resc_backend.db.model import Base
 from resc_backend.db.model.rule_allow_list import DBruleAllowList
 from resc_backend.db.model.rule_pack import DBrulePack
 
 
@@ -16,38 +23,59 @@
     rule_name = Column(String(400), nullable=False)
     description = Column(String(2000), nullable=True)
     entropy = Column(Float, nullable=True)
     secret_group = Column(Integer, nullable=True)
     regex = Column(Text, nullable=True)
     path = Column(Text, nullable=True)
     keywords = Column(Text, nullable=True)
-    __table_args__ = (UniqueConstraint("rule_name", "rule_pack", name="unique_rule_name_per_rule_pack_version"),)
+    __table_args__ = (
+        UniqueConstraint(
+            "rule_name", "rule_pack", name="unique_rule_name_per_rule_pack_version"
+        ),
+    )
 
-    def __init__(self, rule_pack: str, rule_name: str, description: str, allow_list: int = None,
-                 entropy: float = None, secret_group: str = None, regex: str = None, path: str = None,
-                 keywords: str = None):
+    def __init__(
+        self,
+        rule_pack: str,
+        rule_name: str,
+        description: str,
+        allow_list: int = None,
+        entropy: float = None,
+        secret_group: str = None,
+        regex: str = None,
+        path: str = None,
+        keywords: str = None,
+    ):
         self.rule_pack = rule_pack
         self.allow_list = allow_list
         self.rule_name = rule_name
         self.description = description
         self.entropy = entropy
         self.secret_group = secret_group
         self.regex = regex
         self.path = path
         self.keywords = keywords
 
     @staticmethod
-    def create_from_metadata(rule_pack: str, rule_name: str, description: str, entropy: float,
-                             secret_group: str, regex: str, path: str, keywords: str,
-                             allow_list: int):
+    def create_from_metadata(
+        rule_pack: str,
+        rule_name: str,
+        description: str,
+        entropy: float,
+        secret_group: str,
+        regex: str,
+        path: str,
+        keywords: str,
+        allow_list: int,
+    ):
         db_rule = DBrule(
             rule_pack=rule_pack,
             rule_name=rule_name,
             description=description,
             entropy=entropy,
             secret_group=secret_group,
             regex=regex,
             path=path,
             keywords=keywords,
-            allow_list=allow_list
+            allow_list=allow_list,
         )
         return db_rule
```

### Comparing `resc_backend-3.0.0/src/resc_backend/db/model/rule_allow_list.py` & `resc_backend-3.0.1/src/resc_backend/db/model/rule_allow_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,25 +10,33 @@
     id_ = Column("id", Integer, primary_key=True)
     description = Column(String(2000), nullable=True)
     regexes = Column(Text, nullable=True)
     paths = Column(Text, nullable=True)
     commits = Column(Text, nullable=True)
     stop_words = Column(Text, nullable=True)
 
-    def __init__(self, description: str, regexes: str = None, paths: str = None, commits: str = None,
-                 stop_words: str = None):
+    def __init__(
+        self,
+        description: str,
+        regexes: str = None,
+        paths: str = None,
+        commits: str = None,
+        stop_words: str = None,
+    ):
         self.description = description
         self.regexes = regexes
         self.paths = paths
         self.commits = commits
         self.stop_words = stop_words
 
     @staticmethod
-    def create_from_metadata(description: str, regexes: str, paths: str, commits: str, stop_words: str):
+    def create_from_metadata(
+        description: str, regexes: str, paths: str, commits: str, stop_words: str
+    ):
         db_rule_allow_list = DBruleAllowList(
             description=description,
             regexes=regexes,
             paths=paths,
             commits=commits,
-            stop_words=stop_words
+            stop_words=stop_words,
         )
         return db_rule_allow_list
```

### Comparing `resc_backend-3.0.0/src/resc_backend/db/model/rule_pack.py` & `resc_backend-3.0.1/src/resc_backend/db/model/rule_pack.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,30 @@
 class DBrulePack(Base):
     __tablename__ = "rule_pack"
     version = Column("version", String(100), primary_key=True)
     global_allow_list = Column(Integer, ForeignKey(DBruleAllowList.id_), nullable=True)
     active = Column(Boolean, nullable=False, default=False)
     created = Column(DateTime, nullable=False, default=datetime.utcnow)
 
-    def __init__(self, version: str, global_allow_list: int = None, active: bool = False,
-                 created: datetime = datetime.utcnow()):
+    def __init__(
+        self,
+        version: str,
+        global_allow_list: int = None,
+        active: bool = False,
+        created: datetime = datetime.utcnow(),
+    ):
         self.version = version
         self.global_allow_list = global_allow_list
         self.active = active
         self.created = created
 
     @staticmethod
-    def create_from_metadata(version: str, global_allow_list: int, active: bool, created: datetime):
+    def create_from_metadata(
+        version: str, global_allow_list: int, active: bool, created: datetime
+    ):
         db_rule_pack = DBrulePack(
             version=version,
             global_allow_list=global_allow_list,
             active=active,
-            created=created
+            created=created,
         )
         return db_rule_pack
```

### Comparing `resc_backend-3.0.0/src/resc_backend/db/model/scan.py` & `resc_backend-3.0.1/src/resc_backend/db/model/scan.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,33 +14,50 @@
 
 
 class DBscan(Base):
     __tablename__ = "scan"
     id_ = Column("id", Integer, primary_key=True)
     repository_id = Column(Integer, ForeignKey(REPOSITORY_ID))
     rule_pack = Column(String(100), ForeignKey(DBrulePack.version), nullable=False)
-    scan_type = Column(Enum(ScanType), default=ScanType.BASE, server_default=BASE_SCAN, nullable=False)
+    scan_type = Column(
+        Enum(ScanType), default=ScanType.BASE, server_default=BASE_SCAN, nullable=False
+    )
     last_scanned_commit = Column(String(100), nullable=False)
     timestamp = Column(DateTime, nullable=False, default=datetime.utcnow)
-    increment_number = Column(Integer, server_default=text("0"), default=0, nullable=False)
+    increment_number = Column(
+        Integer, server_default=text("0"), default=0, nullable=False
+    )
 
-    def __init__(self, repository_id: int, scan_type: ScanType, last_scanned_commit: str, timestamp: datetime,
-                 increment_number: int, rule_pack: str):
+    def __init__(
+        self,
+        repository_id: int,
+        scan_type: ScanType,
+        last_scanned_commit: str,
+        timestamp: datetime,
+        increment_number: int,
+        rule_pack: str,
+    ):
         self.repository_id = repository_id
         self.scan_type = scan_type
         self.last_scanned_commit = last_scanned_commit
         self.timestamp = timestamp
         self.increment_number = increment_number
         self.rule_pack = rule_pack
 
     @staticmethod
-    def create_from_metadata(timestamp: datetime, scan_type: ScanType, last_scanned_commit: str, increment_number: int,
-                             rule_pack: str, repository_id: int):
+    def create_from_metadata(
+        timestamp: datetime,
+        scan_type: ScanType,
+        last_scanned_commit: str,
+        increment_number: int,
+        rule_pack: str,
+        repository_id: int,
+    ):
         db_scan = DBscan(
             timestamp=timestamp,
             scan_type=scan_type,
             last_scanned_commit=last_scanned_commit,
             increment_number=increment_number,
             rule_pack=rule_pack,
-            repository_id=repository_id
+            repository_id=repository_id,
         )
         return db_scan
```

### Comparing `resc_backend-3.0.0/src/resc_backend/helpers/dict_remapper.py` & `resc_backend-3.0.1/src/resc_backend/helpers/dict_remapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 from functools import reduce
 from typing import List
 
 
 def remap_dict_keys(input_dict: dict, transformation_map: List):
     new_keys = [val[1] for val in transformation_map]
     for old_key, new_key in transformation_map:
-        create_nested_dictionary(input_dict, new_key,  get_value_from_nested_dictionary(input_dict, *old_key))
-
-    output_dict = {k: v for k, v in input_dict.items() if k in [key[0] for key in new_keys]}
+        create_nested_dictionary(
+            input_dict, new_key, get_value_from_nested_dictionary(input_dict, *old_key)
+        )
+
+    output_dict = {
+        k: v for k, v in input_dict.items() if k in [key[0] for key in new_keys]
+    }
 
     return output_dict
 
 
 def create_nested_dictionary(dictionary, keys, value):
     for key in keys[:-1]:
         dictionary = dictionary.setdefault(key, {})
```

### Comparing `resc_backend-3.0.0/src/resc_backend/helpers/environment_wrapper.py` & `resc_backend-3.0.1/src/resc_backend/helpers/environment_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,9 +18,11 @@
         value = os.environ.get(env_variable.key_name, env_variable.default)
         if not value and env_variable.required:
             missing.append(f"{env_variable.key_name}: {env_variable.help_text}")
         else:
             values[env_variable.key_name] = value
 
     if missing:
-        raise EnvironmentError(f"The following env variables need to be set: {', '.join(missing)}")
+        raise EnvironmentError(
+            f"The following env variables need to be set: {', '.join(missing)}"
+        )
     return values
```

### Comparing `resc_backend-3.0.0/src/resc_backend/helpers/rabbitmq/configuration.py` & `resc_backend-3.0.1/src/resc_backend/helpers/rabbitmq/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,9 +49,9 @@
         required=True,
     ),
     EnvironmentVariable(
         DEBUG_MODE,
         "Show debug log statements, if set to '0' only INFO logs and above will be shown.",
         required=False,
         default="0",
-    )
+    ),
 ]
```

### Comparing `resc_backend-3.0.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py` & `resc_backend-3.0.1/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-# pylint: disable=E1101
 # Standard Library
 import logging
 
 # Third Party
 import requests
 from requests.adapters import HTTPAdapter
 from requests.auth import HTTPBasicAuth
 from urllib3 import Retry
 
 # First Party
 from resc_backend.common import initialise_logs
-from resc_backend.constants import LOG_FILE_PATH_RABBITMQ, PROJECT_QUEUE, REPOSITORY_QUEUE
+from resc_backend.constants import (
+    LOG_FILE_PATH_RABBITMQ,
+    PROJECT_QUEUE,
+    REPOSITORY_QUEUE,
+)
 from resc_backend.helpers.environment_wrapper import validate_environment
 from resc_backend.helpers.rabbitmq.configuration import (
     RABBITMQ_DEFAULT_PASSWORD,
     RABBITMQ_DEFAULT_USER,
     RABBITMQ_DEFAULT_VHOST,
     RABBITMQ_PASSWORD,
     RABBITMQ_USERNAME,
-    REQUIRED_ENV_VARS
+    REQUIRED_ENV_VARS,
 )
 
 env_variables = validate_environment(REQUIRED_ENV_VARS)
 logger_config = initialise_logs(LOG_FILE_PATH_RABBITMQ)
 logger = logging.getLogger(__name__)
 
 
@@ -32,30 +35,31 @@
     :param rabbitmq_api_base_url:
         RabbitMQ API base url
     """
     rabbitmq_admin_user = f"{env_variables[RABBITMQ_DEFAULT_USER]}"
     rabbitmq_admin_password = f"{env_variables[RABBITMQ_DEFAULT_PASSWORD]}"
 
     session = requests.Session()
-    retries = Retry(total=100,
-                    backoff_factor=1,
-                    status_forcelist=[500, 502, 503, 504])
+    retries = Retry(total=100, backoff_factor=1, status_forcelist=[500, 502, 503, 504])
     uri = rabbitmq_api_base_url + "/api/health/checks/alarms"
     session.mount("http://", HTTPAdapter(max_retries=retries))
-    response = session.get(uri,
-                           auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password))
+    response = session.get(
+        uri, auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password)
+    )
 
     if hasattr(response, "status_code") and int(response.status_code) == 200:
         logger.debug("Rabbitmq server is up.")
         return True
     logger.error(f"Rabbitmq server is down, HTTP status: '{response.status_code}'")
     return False
 
 
-def create_user(rabbitmq_api_base_url: str, username: str, password: str, role: str) -> bool:
+def create_user(
+    rabbitmq_api_base_url: str, username: str, password: str, role: str
+) -> bool:
     """
         Creates a user in RabbitMQ server, it would return true if the operation was a success, false otherwise
     :param rabbitmq_api_base_url:
         RabbitMQ API base url
     :param username:
         Username to be created
     :param password:
@@ -65,31 +69,43 @@
     :return: True if user creation is successful else returns False.
     """
     rabbitmq_admin_user = f"{env_variables[RABBITMQ_DEFAULT_USER]}"
     rabbitmq_admin_password = f"{env_variables[RABBITMQ_DEFAULT_PASSWORD]}"
 
     uri = rabbitmq_api_base_url + "/api/users/" + username
     user_data = {"password": password, "tags": role}
-    response = requests.put(uri, json=user_data,
-                            auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password), timeout=10)
+    response = requests.put(
+        uri,
+        json=user_data,
+        auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password),
+        timeout=10,
+    )
 
     if hasattr(response, "status_code") and int(response.status_code) == 201:
         logger.info(f"User: {username} with role: {role} created successfully.")
         return True
     if hasattr(response, "status_code") and int(response.status_code) == 204:
         logger.info(f"User: {username} with role: {role} already exists.")
         return True
-    logger.error(f"Failed while creating user: '{username}' "
-                 f"with role: '{role}' "
-                 f", HTTP status: '{response.status_code}'")
+    logger.error(
+        f"Failed while creating user: '{username}' "
+        f"with role: '{role}' "
+        f", HTTP status: '{response.status_code}'"
+    )
     return False
 
 
-def set_resource_permissions(rabbitmq_api_base_url: str, v_host: str, username: str, configure_resources_regex: str,
-                             read_resources_regex: str, write_resources_regex: str) -> bool:
+def set_resource_permissions(
+    rabbitmq_api_base_url: str,
+    v_host: str,
+    username: str,
+    configure_resources_regex: str,
+    read_resources_regex: str,
+    write_resources_regex: str,
+) -> bool:
     """
         Sets permission for resources, it would return true if the operation was a success, false otherwise
     :param rabbitmq_api_base_url:
         RabbitMQ API base url
     :param v_host:
         Virtual host name of the RabbitMQ server
     :param username:
@@ -102,30 +118,47 @@
         Regex of write permission
     :return: True if permission assigned to user is successful else returns False.
     """
     rabbitmq_admin_user = f"{env_variables[RABBITMQ_DEFAULT_USER]}"
     rabbitmq_admin_password = f"{env_variables[RABBITMQ_DEFAULT_PASSWORD]}"
 
     uri = rabbitmq_api_base_url + "/api/permissions/" + v_host + "/" + username
-    permission_data = {"configure": configure_resources_regex, "write": write_resources_regex,
-                       "read": read_resources_regex}
-
-    response = requests.put(uri, json=permission_data,
-                            auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password), timeout=10)
+    permission_data = {
+        "configure": configure_resources_regex,
+        "write": write_resources_regex,
+        "read": read_resources_regex,
+    }
+
+    response = requests.put(
+        uri,
+        json=permission_data,
+        auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password),
+        timeout=10,
+    )
     if hasattr(response, "status_code") and int(response.status_code) == 201:
-        logger.debug(f"vHost permission successfully assigned to user: {username} for vHost: {v_host}.")
+        logger.debug(
+            f"vHost permission successfully assigned to user: {username} for vHost: {v_host}."
+        )
         return True
-    logger.error(f"Failed while assigning vhost permission to user: '{username}' "
-                 f"for vhost: '{v_host}' "
-                 f", HTTP status: '{response.status_code}'")
+    logger.error(
+        f"Failed while assigning vhost permission to user: '{username}' "
+        f"for vhost: '{v_host}' "
+        f", HTTP status: '{response.status_code}'"
+    )
     return False
 
 
-def set_topic_permissions(rabbitmq_api_base_url: str, v_host: str, username: str, topic_name: str, allow_read: bool,
-                          allow_write: bool) -> bool:
+def set_topic_permissions(
+    rabbitmq_api_base_url: str,
+    v_host: str,
+    username: str,
+    topic_name: str,
+    allow_read: bool,
+    allow_write: bool,
+) -> bool:
     """
         Sets permission for topics, it would return true if the operation was a success, false otherwise
     :param rabbitmq_api_base_url:
         RabbitMQ API base url
     :param v_host:
         Virtual host name of the RabbitMQ server
     :param username:
@@ -148,48 +181,79 @@
     if allow_write:
         write_permission = permission_allow
 
     rabbitmq_admin_user = f"{env_variables[RABBITMQ_DEFAULT_USER]}"
     rabbitmq_admin_password = f"{env_variables[RABBITMQ_DEFAULT_PASSWORD]}"
 
     uri = rabbitmq_api_base_url + "/api/topic-permissions/" + v_host + "/" + username
-    topic_permission_data = {"exchange": topic_name, "write": write_permission, "read": read_permission}
-
-    response = requests.put(uri, json=topic_permission_data,
-                            auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password), timeout=10)
-
-    if hasattr(response, "status_code") and (int(response.status_code) == 201 or int(response.status_code) == 204):
+    topic_permission_data = {
+        "exchange": topic_name,
+        "write": write_permission,
+        "read": read_permission,
+    }
+
+    response = requests.put(
+        uri,
+        json=topic_permission_data,
+        auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password),
+        timeout=10,
+    )
+
+    if hasattr(response, "status_code") and (
+        int(response.status_code) == 201 or int(response.status_code) == 204
+    ):
         logger.debug(
-            f"Topic permission successfully assigned to user: {username} for topic: {topic_name} in vhost: {v_host}.")
+            f"Topic permission successfully assigned to user: {username} for topic: {topic_name} in vhost: {v_host}."
+        )
         return True
-    logger.error(f"Failed while assigning topic permission to user: '{username}' "
-                 f"with vhost: '{v_host}' "
-                 f"for topic: '{topic_name}' "
-                 f", HTTP status: '{response.status_code}'")
+    logger.error(
+        f"Failed while assigning topic permission to user: '{username}' "
+        f"with vhost: '{v_host}' "
+        f"for topic: '{topic_name}' "
+        f", HTTP status: '{response.status_code}'"
+    )
     return False
 
 
 def create_queue_user_and_set_permission(rabbitmq_api_base_url: str):
     """
         This function creates user for queue and assigns required permission.
     :param rabbitmq_api_base_url:
         RabbitMQ API base url
     """
     rabbitmq_vhost = f"{env_variables[RABBITMQ_DEFAULT_VHOST]}"
     queue_user = f"{env_variables[RABBITMQ_USERNAME]}"
     queue_password = f"{env_variables[RABBITMQ_PASSWORD]}"
 
-    user_created = create_user(rabbitmq_api_base_url=rabbitmq_api_base_url, username=queue_user,
-                               password=queue_password, role="monitoring")
+    user_created = create_user(
+        rabbitmq_api_base_url=rabbitmq_api_base_url,
+        username=queue_user,
+        password=queue_password,
+        role="monitoring",
+    )
     if user_created:
-        set_resource_permissions(rabbitmq_api_base_url=rabbitmq_api_base_url, v_host=rabbitmq_vhost,
-                                 username=queue_user,
-                                 configure_resources_regex=f"^({PROJECT_QUEUE}|{REPOSITORY_QUEUE}"
-                                                           f"|.*celery.*)$",
-                                 read_resources_regex=f"^{PROJECT_QUEUE}|{REPOSITORY_QUEUE}"
-                                                      f"|.*celery.*$",
-                                 write_resources_regex=f"^{PROJECT_QUEUE}|{REPOSITORY_QUEUE}"
-                                                       f"|amq.default|.*celery.*$")
-        set_topic_permissions(rabbitmq_api_base_url=rabbitmq_api_base_url, v_host=rabbitmq_vhost, username=queue_user,
-                              topic_name=f"{PROJECT_QUEUE}", allow_read=True, allow_write=True)
-        set_topic_permissions(rabbitmq_api_base_url=rabbitmq_api_base_url, v_host=rabbitmq_vhost, username=queue_user,
-                              topic_name=f"{REPOSITORY_QUEUE}", allow_read=True, allow_write=True)
+        set_resource_permissions(
+            rabbitmq_api_base_url=rabbitmq_api_base_url,
+            v_host=rabbitmq_vhost,
+            username=queue_user,
+            configure_resources_regex=f"^({PROJECT_QUEUE}|{REPOSITORY_QUEUE}"
+            f"|.*celery.*)$",
+            read_resources_regex=f"^{PROJECT_QUEUE}|{REPOSITORY_QUEUE}" f"|.*celery.*$",
+            write_resources_regex=f"^{PROJECT_QUEUE}|{REPOSITORY_QUEUE}"
+            f"|amq.default|.*celery.*$",
+        )
+        set_topic_permissions(
+            rabbitmq_api_base_url=rabbitmq_api_base_url,
+            v_host=rabbitmq_vhost,
+            username=queue_user,
+            topic_name=f"{PROJECT_QUEUE}",
+            allow_read=True,
+            allow_write=True,
+        )
+        set_topic_permissions(
+            rabbitmq_api_base_url=rabbitmq_api_base_url,
+            v_host=rabbitmq_vhost,
+            username=queue_user,
+            topic_name=f"{REPOSITORY_QUEUE}",
+            allow_read=True,
+            allow_write=True,
+        )
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/api.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=C0413,W0611,W0404
 # Standard Library
 import logging.config
 
 # Third Party
 from fastapi import Depends, FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from starlette.responses import RedirectResponse
@@ -14,35 +13,37 @@
 from resc_backend.constants import RWS_VERSION_PREFIX
 from resc_backend.db.connection import Session, engine
 from resc_backend.helpers.environment_wrapper import validate_environment
 from resc_backend.resc_web_service.configuration import (
     AUTHENTICATION_REQUIRED,
     CORS_ALLOWED_DOMAINS,
     ENABLE_CORS,
-    WEB_SERVICE_ENV_VARS
+    WEB_SERVICE_ENV_VARS,
 )
 from resc_backend.resc_web_service.dependencies import (
     check_db_initialized,
     requires_auth,
     requires_no_auth,
-    add_security_headers
+    add_security_headers,
 )
 from resc_backend.resc_web_service.endpoints import (
     common,
     detailed_findings,
     findings,
     health,
     metrics,
     repositories,
     rules,
     rule_packs,
     scans,
-    vcs_instances
+    vcs_instances,
+)
+from resc_backend.resc_web_service.helpers.exception_handler import (
+    add_exception_handlers,
 )
-from resc_backend.resc_web_service.helpers.exception_handler import add_exception_handlers
 from resc_backend.resc_web_service.cache_manager import CacheManager
 
 # Check and load environment variables
 env_variables = validate_environment(WEB_SERVICE_ENV_VARS)
 
 
 def generate_logger_config(log_file_path, debug=True):
@@ -75,30 +76,30 @@
             },
             "file": {
                 "level": logging_level,
                 "class": "logging.handlers.RotatingFileHandler",
                 "formatter": "generic-log-formatter",
                 "filename": log_file_path,
                 "maxBytes": 100 * 1024 * 1024,
-                "backupCount": 5
-            }
+                "backupCount": 5,
+            },
         },
         "loggers": {
             "": {
                 "handlers": ["console", "file"],
                 "level": logging_level,
-                "propagate": True
+                "propagate": True,
             },
-        }
+        },
     }
 
     return logging_config
 
 
-logging.config.dictConfig(generate_logger_config('local_logs.log'))
+logging.config.dictConfig(generate_logger_config("local_logs.log"))
 logger = logging.getLogger(__name__)
 tags_metadata = [
     {"name": "health", "description": "Checks health for API"},
     {"name": "resc-common", "description": "Manage common information"},
     {"name": "resc-rules", "description": "Manage rule information"},
     {"name": "resc-rule-packs", "description": "Manage rule pack information"},
     {"name": "resc-repositories", "description": "Manage repository information"},
@@ -108,36 +109,40 @@
     {"name": "resc-metrics", "description": "Retrieve metrics"},
 ]
 
 # Check if authentication is required for api endpoints
 auth_disabled = env_variables[AUTHENTICATION_REQUIRED].lower() in ["false"]
 AUTH = [Depends(requires_no_auth)] if auth_disabled else [Depends(requires_auth)]
 
-app = FastAPI(title="Repository Scanner (RESC)",
-              description="RESC API helps you to perform several operations upon findings "
-                          "obtained from multiple source code repositories.",
-              version=get_package_version(),
-              openapi_tags=tags_metadata)
+app = FastAPI(
+    title="Repository Scanner (RESC)",
+    description="RESC API helps you to perform several operations upon findings "
+    "obtained from multiple source code repositories.",
+    version=get_package_version(),
+    openapi_tags=tags_metadata,
+)
 
 if env_variables[ENABLE_CORS].lower() in ["true"]:
-    origins = env_variables[CORS_ALLOWED_DOMAINS].split(', ')
+    origins = env_variables[CORS_ALLOWED_DOMAINS].split(", ")
     app.add_middleware(
         CORSMiddleware,
         allow_origins=origins,
         allow_credentials=True,
         allow_methods=["*"],
         allow_headers=["*"],
     )
 
 app.include_router(health.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(common.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(rules.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(rule_packs.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(findings.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
-app.include_router(detailed_findings.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
+app.include_router(
+    detailed_findings.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH
+)
 app.include_router(repositories.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(scans.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(vcs_instances.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(metrics.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 
 # Apply the security headers to the app in the form of middleware
 app.middleware("http")(add_security_headers)
@@ -151,15 +156,17 @@
     CacheManager.initialize_cache(env_variables=env_variables)
     try:
         _ = Session(bind=engine)
         check_db_initialized()
 
         logger.info("Database is connected, expected table(s) found")
     except RetryError as exc:
-        raise SystemExit("Error while connecting to the database, retry timed out") from exc
+        raise SystemExit(
+            "Error while connecting to the database, retry timed out"
+        ) from exc
 
 
 @app.on_event("shutdown")
 async def app_shutdown():
     await CacheManager.clear_all_cache()
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/cache_manager.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/cache_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,51 +13,57 @@
 from resc_backend.constants import CACHE_PREFIX, LOG_FILE_CACHING
 from resc_backend.helpers.environment_wrapper import validate_environment
 from resc_backend.resc_web_service.configuration import (
     CONDITIONAL_REDIS_ENV_VARS,
     REDIS_PASSWORD,
     RESC_REDIS_CACHE_ENABLE,
     RESC_REDIS_SERVICE_HOST,
-    RESC_REDIS_SERVICE_PORT
+    RESC_REDIS_SERVICE_PORT,
 )
 
 logger_config = initialise_logs(LOG_FILE_CACHING)
 logger = logging.getLogger(__name__)
 
 
 class CacheManager:
-
     @classmethod
     def initialize_cache(cls, env_variables):
         cache_enabled = env_variables[RESC_REDIS_CACHE_ENABLE].lower() in ["true"]
         if cache_enabled:
             env_variables.update(validate_environment(CONDITIONAL_REDIS_ENV_VARS))
             redis_host = f"{env_variables[RESC_REDIS_SERVICE_HOST]}"
             redis_port = f"{env_variables[RESC_REDIS_SERVICE_PORT]}"
             redis_password = f"{env_variables[REDIS_PASSWORD]}"
-            redis_backend = cls.get_cache_client(host=redis_host, port=int(redis_port), password=redis_password)
-            FastAPICache.init(RedisBackend(redis_backend),
-                              prefix=CACHE_PREFIX,
-                              key_builder=cls.request_key_builder,
-                              enable=cache_enabled)
+            redis_backend = cls.get_cache_client(
+                host=redis_host, port=int(redis_port), password=redis_password
+            )
+            FastAPICache.init(
+                RedisBackend(redis_backend),
+                prefix=CACHE_PREFIX,
+                key_builder=cls.request_key_builder,
+                enable=cache_enabled,
+            )
         else:
             FastAPICache.init(backend=RedisBackend(None), enable=cache_enabled)
 
     @staticmethod
     def get_cache_client(host: str, port: int, password: str):
         cache_client = aioredis.from_url(f"redis://{host}:{port}", password=password)
         return cache_client
 
     @staticmethod
-    def request_key_builder(func: Callable[..., Any],  # pylint: disable=W0613
-                            namespace: str = "",
-                            *,
-                            request: Request = None,
-                            response: Response = None,  # pylint: disable=W0613
-                            args: Tuple[Any, ...], kwargs: Dict[str, Any]) -> str:  # pylint: disable=W0613
+    def request_key_builder(
+        func: Callable[..., Any],
+        namespace: str = "",
+        *,
+        request: Request = None,
+        response: Response = None,
+        args: Tuple[Any, ...],
+        kwargs: Dict[str, Any],
+    ) -> str:
         """
         Build a unique key for caching based on the provided function, namespace, request, response,
         arguments (args), and keyword arguments (kwargs).
 
         Args:
             func (Callable): The function for which the key is being built.
             namespace (str, optional): A namespace to differentiate keys (default "").
@@ -66,31 +72,36 @@
             args (Tuple[Any, ...]): Positional arguments passed to the function.
             kwargs (Dict[str, Any]): Keyword arguments passed to the function.
 
         Returns:
             str: A unique key based on the input parameters.
         """
 
-        cache_key = ":".join([
-            FastAPICache.get_prefix(),
-            namespace,
-            request.method.lower(),
-            request.url.path,
-            repr(sorted(request.query_params.items()))
-        ])
+        cache_key = ":".join(
+            [
+                FastAPICache.get_prefix(),
+                namespace,
+                request.method.lower(),
+                request.url.path,
+                repr(sorted(request.query_params.items())),
+            ]
+        )
         logger.debug(f"Cache created with key: {cache_key}")
         return cache_key
 
     @staticmethod
-    def personalized_key_builder(func: Callable[..., Any],  # pylint: disable=W0613
-                                 namespace: str = "",
-                                 *,
-                                 request: Request = None,
-                                 response: Response = None,  # pylint: disable=W0613
-                                 args: Tuple[Any, ...], kwargs: Dict[str, Any]) -> str:  # pylint: disable=W0613
+    def personalized_key_builder(
+        func: Callable[..., Any],
+        namespace: str = "",
+        *,
+        request: Request = None,
+        response: Response = None,
+        args: Tuple[Any, ...],
+        kwargs: Dict[str, Any],
+    ) -> str:
         """
         Build a personalized unique key for caching based logged-in user on the provided function, namespace, request,
         response, arguments (args), and keyword arguments (kwargs).
         This should be used for apis specific to logged-in user.
 
         Args:
             func (Callable): The function for which the key is being built.
@@ -99,22 +110,24 @@
             response (Response, optional): The response object (default None).
             args (Tuple[Any, ...]): Positional arguments passed to the function.
             kwargs (Dict[str, Any]): Keyword arguments passed to the function.
 
         Returns:
             str: A unique key based on the input parameters.
         """
-        cache_key = ":".join([
-            CACHE_PREFIX,
-            namespace,
-            request.user,
-            request.method.lower(),
-            request.url.path,
-            repr(sorted(request.query_params.items()))
-        ])
+        cache_key = ":".join(
+            [
+                CACHE_PREFIX,
+                namespace,
+                request.user,
+                request.method.lower(),
+                request.url.path,
+                repr(sorted(request.query_params.items())),
+            ]
+        )
         logger.debug(f"Cache created with key: {cache_key}")
         return cache_key
 
     @staticmethod
     async def clear_cache_by_namespace(namespace):
         cache_enabled = FastAPICache.get_enable()
         if cache_enabled:
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/configuration.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding=utf-8
 # First Party
 from resc_backend.helpers.environment_wrapper import EnvironmentVariable
 
-ENABLE_CORS = 'ENABLE_CORS'
-CORS_ALLOWED_DOMAINS = 'CORS_ALLOWED_DOMAINS'
+ENABLE_CORS = "ENABLE_CORS"
+CORS_ALLOWED_DOMAINS = "CORS_ALLOWED_DOMAINS"
 
-AUTHENTICATION_REQUIRED = 'AUTHENTICATION_REQUIRED'
-SSO_ACCESS_TOKEN_ISSUER_URL = 'SSO_ACCESS_TOKEN_ISSUER_URL'
-SSO_ACCESS_TOKEN_JWKS_URL = 'SSO_ACCESS_TOKEN_JWKS_URL'
-SSO_JWT_SIGN_ALGORITHM = 'SSO_JWT_SIGN_ALGORITHM'
-SSO_JWT_REQUIRED_CLAIMS = 'SSO_JWT_REQUIRED_CLAIMS'
-SSO_JWT_CLAIM_KEY_USER_ID = 'SSO_JWT_CLAIM_KEY_USER_ID'
-SSO_JWT_CLAIM_KEY_AUTHORIZATION = 'SSO_JWT_CLAIM_KEY_AUTHORIZATION'
-SSO_JWT_CLAIM_VALUE_AUTHORIZATION = 'SSO_JWT_CLAIM_VALUE_AUTHORIZATION'
+AUTHENTICATION_REQUIRED = "AUTHENTICATION_REQUIRED"
+SSO_ACCESS_TOKEN_ISSUER_URL = "SSO_ACCESS_TOKEN_ISSUER_URL"
+SSO_ACCESS_TOKEN_JWKS_URL = "SSO_ACCESS_TOKEN_JWKS_URL"
+SSO_JWT_SIGN_ALGORITHM = "SSO_JWT_SIGN_ALGORITHM"
+SSO_JWT_REQUIRED_CLAIMS = "SSO_JWT_REQUIRED_CLAIMS"
+SSO_JWT_CLAIM_KEY_USER_ID = "SSO_JWT_CLAIM_KEY_USER_ID"
+SSO_JWT_CLAIM_KEY_AUTHORIZATION = "SSO_JWT_CLAIM_KEY_AUTHORIZATION"
+SSO_JWT_CLAIM_VALUE_AUTHORIZATION = "SSO_JWT_CLAIM_VALUE_AUTHORIZATION"
 
-RESC_REDIS_CACHE_ENABLE = 'RESC_REDIS_CACHE_ENABLE'
-RESC_REDIS_SERVICE_HOST = 'RESC_REDIS_SERVICE_HOST'
-RESC_REDIS_SERVICE_PORT = 'RESC_REDIS_SERVICE_PORT'
-REDIS_PASSWORD = 'REDIS_PASSWORD'
+RESC_REDIS_CACHE_ENABLE = "RESC_REDIS_CACHE_ENABLE"
+RESC_REDIS_SERVICE_HOST = "RESC_REDIS_SERVICE_HOST"
+RESC_REDIS_SERVICE_PORT = "RESC_REDIS_SERVICE_PORT"
+REDIS_PASSWORD = "REDIS_PASSWORD"
 
 WEB_SERVICE_ENV_VARS = [
     EnvironmentVariable(
         ENABLE_CORS,
         "Enable by providing the value true to allow CORS requests.",
         required=False,
-        default='',
+        default="",
     ),
     EnvironmentVariable(
         CORS_ALLOWED_DOMAINS,
         "Comma separated lists of domains to allow in the CORS policy if ENABLE_CORS is true",
         required=False,
-        default='',
+        default="",
     ),
     EnvironmentVariable(
         AUTHENTICATION_REQUIRED,
         "set to false to disable authentication, any other value will enable SSO authentication",
         required=False,
-        default='',
+        default="",
     ),
     EnvironmentVariable(
         RESC_REDIS_CACHE_ENABLE,
         "Set to true to enable the redis cache, its expected to be running separately from this instance",
         required=False,
-        default='False',
-    )
+        default="False",
+    ),
 ]
 
 CONDITIONAL_SSO_ENV_VARS = [
     EnvironmentVariable(
         SSO_ACCESS_TOKEN_ISSUER_URL,
         "URL of the access token issuer",
         required=True,
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/audit.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/audit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-# pylint: disable=R0916,R0912,C0121,not-callable
 # Standard Library
 import logging
 from datetime import datetime, timedelta
+from typing import List
 
 # Third Party
 from sqlalchemy import and_, extract, func, or_
 from sqlalchemy.engine import Row
 from sqlalchemy.orm import Session
 
 # First Party
-from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
-from resc_backend.db import model
+from resc_backend.constants import (
+    DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    MAX_RECORDS_PER_PAGE_LIMIT,
+)
+from resc_backend.db.model import DBaudit
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.time_period import TimePeriod
 
 logger = logging.getLogger(__name__)
 
 
-def create_audit(db_connection: Session, finding_id: int, auditor: str,
-                 status: FindingStatus, comment: str = "") -> model.DBaudit:
+def create_audit(
+    db_connection: Session,
+    finding_id: int,
+    auditor: str,
+    status: FindingStatus,
+    comment: str = "",
+) -> DBaudit:
     """
         Audit finding, updating the status and comment
     :param db_connection:
         Session of the database connection
     :param finding_id:
         id of the finding to audit
     :param auditor:
@@ -30,121 +38,164 @@
     :param status:
         audit status to set, type FindingStatus
     :param comment:
         audit comment to set
     :return: DBaudit
         The output will contain the audit that was created
     """
-    db_audit = model.audit.DBaudit(
+
+    db_audit = DBaudit(
         finding_id=finding_id,
         auditor=auditor,
         status=status,
         comment=comment,
-        timestamp=datetime.utcnow()
+        timestamp=datetime.utcnow(),
     )
     db_connection.add(db_audit)
     db_connection.commit()
     db_connection.refresh(db_audit)
 
     return db_audit
 
 
-def get_finding_audits(db_connection: Session, finding_id: int, skip: int = 0,
-                       limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT) -> [model.DBaudit]:
+def get_finding_audits(
+    db_connection: Session,
+    finding_id: int,
+    skip: int = 0,
+    limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
+) -> List[DBaudit]:
     """
         Get Audit entries for finding
     :param db_connection:
         Session of the database connection
     :param finding_id:
         id of the finding to audit
     :param skip:
         integer amount of records to skip to support pagination
     :param limit:
         integer amount of records to return, to support pagination
     :return: [DBaudit]
         The output will contain the list of audit items for the given finding
     """
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
-    query = db_connection.query(model.DBaudit).filter(model.DBaudit.finding_id == finding_id)
-    query = query.order_by(model.DBaudit.id_.desc()).offset(skip).limit(limit_val)
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
+    query = db_connection.query(DBaudit).filter(DBaudit.finding_id == finding_id)
+    query = query.order_by(DBaudit.id_.desc()).offset(skip).limit(limit_val)
     finding_audits = query.all()
     return finding_audits
 
 
 def get_finding_audits_count(db_connection: Session, finding_id: int) -> int:
     """
         Get count of Audit entries for finding
     :param db_connection:
         Session of the database connection
     :param finding_id:
         id of the finding to audit
     :return: total_count
         count of audit entries
     """
-    total_count = db_connection.query(func.count(model.DBaudit.id_)) \
-        .filter(model.DBaudit.finding_id == finding_id).scalar()
+    total_count = (
+        db_connection.query(func.count(DBaudit.id_))
+        .filter(DBaudit.finding_id == finding_id)
+        .scalar()
+    )
     return total_count
 
 
-def get_audit_count_by_auditor_over_time(db_connection: Session, weeks: int = 13) -> list[Row]:
+def get_audit_count_by_auditor_over_time(
+    db_connection: Session, weeks: int = 13
+) -> list[Row]:
     """
         Retrieve count audits by auditor over time for given weeks
     :param db_connection:
         Session of the database connection
     :param weeks:
         optional, filter on last n weeks, default 13
     :return: count_over_time
         list of rows containing audit count over time per week
     """
     last_nth_week_date_time = datetime.utcnow() - timedelta(weeks=weeks)
 
-    query = db_connection.query(extract('year', model.DBaudit.timestamp).label("year"),
-                                extract('week', model.DBaudit.timestamp).label("week"),
-                                model.DBaudit.auditor,
-                                func.count(model.DBaudit.id_).label("audit_count")) \
-        .filter(or_(extract('year', model.DBaudit.timestamp) > extract('year', last_nth_week_date_time),
-                and_(extract('year', model.DBaudit.timestamp) == extract('year', last_nth_week_date_time),
-                extract('week', model.DBaudit.timestamp) >= extract('week', last_nth_week_date_time)))) \
-        .group_by(extract('year', model.DBaudit.timestamp).label("year"),
-                  extract('week', model.DBaudit.timestamp).label("week"),
-                  model.DBaudit.auditor) \
-        .order_by(extract('year', model.DBaudit.timestamp).label("year"),
-                  extract('week', model.DBaudit.timestamp).label("week"),
-                  model.DBaudit.auditor)
+    query = (
+        db_connection.query(
+            extract("year", DBaudit.timestamp).label("year"),
+            extract("week", DBaudit.timestamp).label("week"),
+            DBaudit.auditor,
+            func.count(DBaudit.id_).label("audit_count"),
+        )
+        .filter(
+            or_(
+                extract("year", DBaudit.timestamp)
+                > extract("year", last_nth_week_date_time),
+                and_(
+                    extract("year", DBaudit.timestamp)
+                    == extract("year", last_nth_week_date_time),
+                    extract("week", DBaudit.timestamp)
+                    >= extract("week", last_nth_week_date_time),
+                ),
+            )
+        )
+        .group_by(
+            extract("year", DBaudit.timestamp).label("year"),
+            extract("week", DBaudit.timestamp).label("week"),
+            DBaudit.auditor,
+        )
+        .order_by(
+            extract("year", DBaudit.timestamp).label("year"),
+            extract("week", DBaudit.timestamp).label("week"),
+            DBaudit.auditor,
+        )
+    )
     finding_audits = query.all()
 
     return finding_audits
 
 
-def get_personal_audit_count(db_connection: Session, auditor: str, time_period: TimePeriod) -> int:
+def get_personal_audit_count(
+    db_connection: Session, auditor: str, time_period: TimePeriod
+) -> int:
     """
         Get count of Audit entries for finding
     :param db_connection:
         Session of the database connection
     :param auditor:
         id of the auditor
     :param time_period:
         period for which to retrieve the audit counts
     :return: total_count
         count of audit entries
     """
     date_today = datetime.utcnow()
 
-    total_count = db_connection.query(func.count(model.DBaudit.id_))
+    total_count = db_connection.query(func.count(DBaudit.id_))
 
     if time_period in (time_period.DAY, time_period.MONTH, time_period.YEAR):
-        total_count = total_count.filter(extract('year', model.DBaudit.timestamp) == extract('year', date_today))
+        total_count = total_count.filter(
+            extract("year", DBaudit.timestamp) == extract("year", date_today)
+        )
 
         if time_period in (time_period.DAY, time_period.MONTH):
-            total_count = total_count.filter(extract('month', model.DBaudit.timestamp) == extract('month', date_today))
+            total_count = total_count.filter(
+                extract("month", DBaudit.timestamp) == extract("month", date_today)
+            )
 
             if time_period == time_period.DAY:
-                total_count = total_count.filter(extract('day', model.DBaudit.timestamp) == extract('day', date_today))
+                total_count = total_count.filter(
+                    extract("day", DBaudit.timestamp) == extract("day", date_today)
+                )
 
     if time_period in (time_period.WEEK, time_period.LAST_WEEK):
         date_last_week = datetime.utcnow() - timedelta(weeks=1)
-        date_week = date_last_week if time_period == time_period.LAST_WEEK else date_today
-        total_count = total_count.filter(extract('year', model.DBaudit.timestamp) == extract('year', date_week))
-        total_count = total_count.filter(extract('week', model.DBaudit.timestamp) == extract('week', date_week))
+        date_week = (
+            date_last_week if time_period == time_period.LAST_WEEK else date_today
+        )
+        total_count = total_count.filter(
+            extract("year", DBaudit.timestamp) == extract("year", date_week)
+        )
+        total_count = total_count.filter(
+            extract("week", DBaudit.timestamp) == extract("week", date_week)
+        )
 
-    total_count = total_count.filter(model.DBaudit.auditor == auditor).scalar()
+    total_count = total_count.filter(DBaudit.auditor == auditor).scalar()
     return total_count
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/finding.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/finding.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,139 @@
-# pylint: disable=R0916,R0912,C0121,not-callable
 # Standard Library
 import logging
 from datetime import datetime, timedelta
 from typing import List
 
 # Third Party
 from sqlalchemy import and_, extract, func, or_, union
 from sqlalchemy.engine import Row
 from sqlalchemy.orm import Session
 
 # First Party
-from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
-from resc_backend.db import model
+from resc_backend.constants import (
+    DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    MAX_RECORDS_PER_PAGE_LIMIT,
+)
+from resc_backend.db.model import (
+    DBaudit,
+    DBfinding,
+    DBrepository,
+    DBrule,
+    DBruleTag,
+    DBscan,
+    DBscanFinding,
+    DBtag,
+    DBVcsInstance,
+)
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.filters import FindingsFilter
 from resc_backend.resc_web_service.schema import finding as finding_schema
 from resc_backend.resc_web_service.schema.date_filter import DateFilter
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 logger = logging.getLogger(__name__)
 
 
-def patch_finding(db_connection: Session, finding_id: int, finding_update: finding_schema.FindingPatch):
-    db_finding = db_connection.query(model.DBfinding).filter_by(id_=finding_id).first()
+def patch_finding(
+    db_connection: Session, finding_id: int, finding_update: finding_schema.FindingPatch
+):
+    db_finding = db_connection.query(DBfinding).filter_by(id_=finding_id).first()
 
     finding_update_dict = finding_update.dict(exclude_unset=True)
     for key in finding_update_dict:
         setattr(db_finding, key, finding_update_dict[key])
 
     db_connection.commit()
     db_connection.refresh(db_finding)
     return db_finding
 
 
-def create_findings(db_connection: Session, findings: List[finding_schema.FindingCreate]) -> List[model.DBfinding]:
+def create_findings(
+    db_connection: Session, findings: List[finding_schema.FindingCreate]
+) -> List[DBfinding]:
     if len(findings) < 1:
         # Function is called with an empty list of findings
         return []
     repository_id = findings[0].repository_id
 
     # get a list of known / registered findings for this repository
-    db_repository_findings = db_connection.query(model.DBfinding).\
-        filter(model.DBfinding.repository_id == repository_id).all()
+    db_repository_findings = (
+        db_connection.query(DBfinding)
+        .filter(DBfinding.repository_id == repository_id)
+        .all()
+    )
 
     # Compare new findings list with findings in the db
     new_findings = findings[:]
     db_findings = []
     for finding in findings:
         for repository_finding in db_repository_findings:
             # Compare based on the unique key in the findings table
-            if repository_finding.commit_id == finding.commit_id and \
-                    repository_finding.rule_name == finding.rule_name and \
-                    repository_finding.file_path == finding.file_path and \
-                    repository_finding.line_number == finding.line_number and \
-                    repository_finding.column_start == finding.column_start and \
-                    repository_finding.column_end == finding.column_end:
+            if (
+                repository_finding.commit_id == finding.commit_id
+                and repository_finding.rule_name == finding.rule_name
+                and repository_finding.file_path == finding.file_path
+                and repository_finding.line_number == finding.line_number
+                and repository_finding.column_start == finding.column_start
+                and repository_finding.column_end == finding.column_end
+            ):
                 # Store the already known finding
                 db_findings.append(repository_finding)
                 # Remove from the db_repository_findings to increase performance for the next loop
                 db_repository_findings.remove(repository_finding)
                 # Remove from the to be created findings
                 new_findings.remove(finding)
                 break
-    logger.info(f"create_findings repository {repository_id}, Requested: {len(findings)}. "
-                f"New findings: {len(new_findings)}. Already in db: {len(db_findings)}")
+    logger.info(
+        f"create_findings repository {repository_id}, Requested: {len(findings)}. "
+        f"New findings: {len(new_findings)}. Already in db: {len(db_findings)}"
+    )
 
     db_create_findings = []
     # Map the to be created findings to the DBfinding type object
     for new_finding in new_findings:
-        db_create_finding = model.finding.DBfinding.create_from_finding(new_finding)
+        db_create_finding = DBfinding.create_from_finding(new_finding)
         db_create_findings.append(db_create_finding)
     # Store all the to be created findings in the database
     if len(db_create_findings) >= 1:
         db_connection.add_all(db_create_findings)
         db_connection.flush()
         db_connection.commit()
         db_findings.extend(db_create_findings)
     # Return the known findings that are part of the request and the newly created findings
     return db_findings
 
 
 def get_finding(db_connection: Session, finding_id: int):
-    finding = db_connection.query(model.DBfinding)
-    finding = finding.filter(model.finding.DBfinding.id_ == finding_id).first()
+    finding = db_connection.query(DBfinding)
+    finding = finding.filter(DBfinding.id_ == finding_id).first()
     return finding
 
 
-def get_findings(db_connection: Session, skip: int = 0,
-                 limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT):
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
-    findings = db_connection.query(model.DBfinding)
-    findings = findings.order_by(model.finding.DBfinding.id_).offset(skip).limit(limit_val).all()
+def get_findings(
+    db_connection: Session, skip: int = 0, limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT
+):
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
+    findings = db_connection.query(DBfinding)
+    findings = findings.order_by(DBfinding.id_).offset(skip).limit(limit_val).all()
     return findings
 
 
-def get_scans_findings(db_connection, scan_ids: [int], skip: int = 0, limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
-                       rules_filter: [str] = None, statuses_filter: [FindingStatus] = None) -> [model.DBfinding]:
+def get_scans_findings(
+    db_connection,
+    scan_ids: List[int],
+    skip: int = 0,
+    limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    rules_filter: List[str] = None,
+    statuses_filter: List[FindingStatus] = None,
+) -> List[DBfinding]:
     """
         Retrieve all finding child objects of a scan object from the database
     :param db_connection:
         Session of the database connection
     :param scan_ids:
         ids of the parent scan object of which to retrieve finding objects
     :param skip:
@@ -114,144 +146,198 @@
         optional, filter on status of findings
     :return: [DBfinding]
         The output will contain a list of DBfinding type objects,
         or an empty list if no finding was found for the given scan_ids
     """
     if len(scan_ids) == 0:
         return []
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
 
-    query = db_connection.query(model.DBfinding)
-    query = query.join(model.DBscanFinding,
-                       model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_)
+    query = db_connection.query(DBfinding)
+    query = query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
 
     if statuses_filter:
         # subquery to select latest audit ids findings
-        max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
-                                                 func.max(model.DBaudit.id_).label("audit_id")) \
-            .group_by(model.DBaudit.finding_id).subquery()
-
-        query = query \
-            .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
-                  isouter=True) \
-            .join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
-                                      model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
-                  isouter=True)
+        max_audit_subquery = (
+            db_connection.query(
+                DBaudit.finding_id, func.max(DBaudit.id_).label("audit_id")
+            )
+            .group_by(DBaudit.finding_id)
+            .subquery()
+        )
+
+        query = query.join(
+            max_audit_subquery,
+            max_audit_subquery.c.finding_id == DBfinding.id_,
+            isouter=True,
+        ).join(
+            DBaudit,
+            and_(
+                DBaudit.finding_id == DBfinding.id_,
+                DBaudit.id_ == max_audit_subquery.c.audit_id,
+            ),
+            isouter=True,
+        )
         if FindingStatus.NOT_ANALYZED in statuses_filter:
-            query = query.filter(or_(model.DBaudit.status.in_(statuses_filter),
-                                     model.DBaudit.status == None))  # noqa: E711
+            query = query.filter(
+                or_(DBaudit.status.in_(statuses_filter), DBaudit.status == None)  # noqa: E711
+            )
         else:
-            query = query.filter(model.DBaudit.status.in_(statuses_filter))
+            query = query.filter(DBaudit.status.in_(statuses_filter))
 
-    query = query.filter(model.DBscanFinding.scan_id.in_(scan_ids))
+    query = query.filter(DBscanFinding.scan_id.in_(scan_ids))
 
     if rules_filter:
-        query = query.filter(model.DBfinding.rule_name.in_(rules_filter))
+        query = query.filter(DBfinding.rule_name.in_(rules_filter))
 
-    findings = query.order_by(model.finding.DBfinding.id_).offset(skip).limit(limit_val).all()
+    findings = query.order_by(DBfinding.id_).offset(skip).limit(limit_val).all()
     return findings
 
 
-def get_total_findings_count(db_connection: Session, findings_filter: FindingsFilter = None) -> int:
+def get_total_findings_count(
+    db_connection: Session, findings_filter: FindingsFilter = None
+) -> int:
     """
         Retrieve count of finding records of a given scan
     :param findings_filter:
     :param db_connection:
         Session of the database connection
     :return: total_count
         count of findings
     """
 
-    total_count_query = db_connection.query(func.count(model.DBfinding.id_))
+    total_count_query = db_connection.query(func.count(DBfinding.id_))
     if findings_filter:
         if findings_filter.finding_statuses:
             # subquery to select latest audit ids findings
-            max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
-                                                     func.max(model.DBaudit.id_).label("audit_id")) \
-                .group_by(model.DBaudit.finding_id).subquery()
-
-            total_count_query = total_count_query \
-                .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
-                      isouter=True) \
-                .join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
-                                          model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
-                      isouter=True)
-        if (findings_filter.vcs_providers and findings_filter.vcs_providers is not None) \
-                or findings_filter.project_name \
-                or findings_filter.repository_name or findings_filter.start_date_time \
-                or findings_filter.end_date_time:
-            total_count_query = total_count_query \
-                .join(model.DBscanFinding,
-                      model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_) \
-                .join(model.DBscan,
-                      model.scan.DBscan.id_ == model.scan_finding.DBscanFinding.scan_id) \
-                .join(model.DBrepository,
-                      model.repository.DBrepository.id_ == model.scan.DBscan.repository_id) \
-                .join(model.DBVcsInstance,
-                      model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
+            max_audit_subquery = (
+                db_connection.query(
+                    DBaudit.finding_id, func.max(DBaudit.id_).label("audit_id")
+                )
+                .group_by(DBaudit.finding_id)
+                .subquery()
+            )
+
+            total_count_query = total_count_query.join(
+                max_audit_subquery,
+                max_audit_subquery.c.finding_id == DBfinding.id_,
+                isouter=True,
+            ).join(
+                DBaudit,
+                and_(
+                    DBaudit.finding_id == DBfinding.id_,
+                    DBaudit.id_ == max_audit_subquery.c.audit_id,
+                ),
+                isouter=True,
+            )
+        if (
+            (
+                findings_filter.vcs_providers
+                and findings_filter.vcs_providers is not None
+            )
+            or findings_filter.project_name
+            or findings_filter.repository_name
+            or findings_filter.start_date_time
+            or findings_filter.end_date_time
+        ):
+            total_count_query = (
+                total_count_query.join(
+                    DBscanFinding, DBscanFinding.finding_id == DBfinding.id_
+                )
+                .join(DBscan, DBscan.id_ == DBscanFinding.scan_id)
+                .join(DBrepository, DBrepository.id_ == DBscan.repository_id)
+                .join(DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance)
+            )
 
         if findings_filter.start_date_time:
             total_count_query = total_count_query.filter(
-                model.scan.DBscan.timestamp >= findings_filter.start_date_time)
+                DBscan.timestamp >= findings_filter.start_date_time
+            )
         if findings_filter.end_date_time:
-            total_count_query = total_count_query.filter(model.scan.DBscan.timestamp <= findings_filter.end_date_time)
+            total_count_query = total_count_query.filter(
+                DBscan.timestamp <= findings_filter.end_date_time
+            )
 
         if findings_filter.repository_name:
             total_count_query = total_count_query.filter(
-                model.DBrepository.repository_name == findings_filter.repository_name)
+                DBrepository.repository_name == findings_filter.repository_name
+            )
 
         if findings_filter.vcs_providers and findings_filter.vcs_providers is not None:
             total_count_query = total_count_query.filter(
-                model.vcs_instance.DBVcsInstance.provider_type.in_(findings_filter.vcs_providers))
+                DBVcsInstance.provider_type.in_(findings_filter.vcs_providers)
+            )
         if findings_filter.project_name:
             total_count_query = total_count_query.filter(
-                model.repository.DBrepository.project_key == findings_filter.project_name)
+                DBrepository.project_key == findings_filter.project_name
+            )
         if findings_filter.rule_names:
-            total_count_query = total_count_query.filter(model.DBfinding.rule_name.in_(findings_filter.rule_names))
+            total_count_query = total_count_query.filter(
+                DBfinding.rule_name.in_(findings_filter.rule_names)
+            )
         if findings_filter.finding_statuses:
             if FindingStatus.NOT_ANALYZED in findings_filter.finding_statuses:
-                total_count_query = total_count_query. \
-                    filter(or_(model.DBaudit.status.in_(findings_filter.finding_statuses),
-                               model.DBaudit.status == None))  # noqa: E711
+                total_count_query = total_count_query.filter(
+                    or_(
+                        DBaudit.status.in_(findings_filter.finding_statuses),
+                        DBaudit.status == None,  # noqa: E711
+                    )
+                )
             else:
-                total_count_query = total_count_query.filter(model.DBaudit.status.in_(findings_filter.finding_statuses))
+                total_count_query = total_count_query.filter(
+                    DBaudit.status.in_(findings_filter.finding_statuses)
+                )
         if findings_filter.scan_ids and len(findings_filter.scan_ids) == 1:
             total_count_query = total_count_query.join(
-                model.DBscanFinding, model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_)
+                DBscanFinding, DBscanFinding.finding_id == DBfinding.id_
+            )
             total_count_query = total_count_query.filter(
-                model.scan_finding.DBscanFinding.scan_id == findings_filter.scan_ids[0])
+                DBscanFinding.scan_id == findings_filter.scan_ids[0]
+            )
 
         if findings_filter.scan_ids and len(findings_filter.scan_ids) >= 2:
             total_count_query = total_count_query.join(
-                model.DBscanFinding, model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_)
+                DBscanFinding, DBscanFinding.finding_id == DBfinding.id_
+            )
             total_count_query = total_count_query.filter(
-                model.scan_finding.DBscanFinding.scan_id.in_(findings_filter.scan_ids))
+                DBscanFinding.scan_id.in_(findings_filter.scan_ids)
+            )
 
     total_count = total_count_query.scalar()
     return total_count
 
 
-def get_findings_by_rule(db_connection: Session, skip: int = 0, limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
-                         rule_name: str = ""):
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
-    findings = db_connection.query(model.DBfinding)
-    findings = findings.filter(model.DBfinding.rule_name == rule_name)
-    findings = findings.order_by(model.finding.DBfinding.id_).offset(skip).limit(limit_val).all()
+def get_findings_by_rule(
+    db_connection: Session,
+    skip: int = 0,
+    limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    rule_name: str = "",
+):
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
+    findings = db_connection.query(DBfinding)
+    findings = findings.filter(DBfinding.rule_name == rule_name)
+    findings = findings.order_by(DBfinding.id_).offset(skip).limit(limit_val).all()
     return findings
 
 
-def get_distinct_rules_from_findings(db_connection: Session, scan_id: int = -1,
-                                     finding_statuses: [FindingStatus] = None,
-                                     vcs_providers: [VCSProviders] = None,
-                                     project_name: str = "",
-                                     repository_name: str = "",
-                                     start_date_time: datetime = None,
-                                     end_date_time: datetime = None,
-                                     rule_pack_versions: [str] = None) -> \
-        List[model.DBrule]:
+def get_distinct_rules_from_findings(
+    db_connection: Session,
+    scan_id: int = -1,
+    finding_statuses: List[FindingStatus] = None,
+    vcs_providers: List[VCSProviders] = None,
+    project_name: str = "",
+    repository_name: str = "",
+    start_date_time: datetime = None,
+    end_date_time: datetime = None,
+    rule_pack_versions: List[str] = None,
+) -> List[DBrule]:
     """
         Retrieve distinct rules detected
     :param db_connection:
         Session of the database connection
     :param scan_id:
         Optional filter by the id of a scan
     :param finding_statuses:
@@ -267,215 +353,283 @@
     :param end_date_time:
         optional, filter on end date
     :param rule_pack_versions:
         optional, filter on rule pack version
     :return: rules
         List of unique rules
     """
-    query = db_connection.query(model.DBfinding.rule_name)
+    query = db_connection.query(DBfinding.rule_name)
 
-    if (vcs_providers or project_name or repository_name or start_date_time or end_date_time or rule_pack_versions) \
-            and scan_id < 0:
-        query = query \
-            .join(model.DBscanFinding,
-                  model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_) \
-            .join(model.DBscan,
-                  model.scan.DBscan.id_ == model.scan_finding.DBscanFinding.scan_id) \
-            .join(model.DBrepository,
-                  model.repository.DBrepository.id_ == model.scan.DBscan.repository_id) \
-            .join(model.DBVcsInstance,
-                  model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
+    if (
+        vcs_providers
+        or project_name
+        or repository_name
+        or start_date_time
+        or end_date_time
+        or rule_pack_versions
+    ) and scan_id < 0:
+        query = (
+            query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
+            .join(DBscan, DBscan.id_ == DBscanFinding.scan_id)
+            .join(DBrepository, DBrepository.id_ == DBscan.repository_id)
+            .join(DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance)
+        )
     if finding_statuses:
         # subquery to select latest audit ids findings
-        max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
-                                                 func.max(model.DBaudit.id_).label("audit_id")) \
-            .group_by(model.DBaudit.finding_id).subquery()
-
-        query = query \
-            .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
-                  isouter=True) \
-            .join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
-                                      model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
-                  isouter=True)
+        max_audit_subquery = (
+            db_connection.query(
+                DBaudit.finding_id, func.max(DBaudit.id_).label("audit_id")
+            )
+            .group_by(DBaudit.finding_id)
+            .subquery()
+        )
+
+        query = query.join(
+            max_audit_subquery,
+            max_audit_subquery.c.finding_id == DBfinding.id_,
+            isouter=True,
+        ).join(
+            DBaudit,
+            and_(
+                DBaudit.finding_id == DBfinding.id_,
+                DBaudit.id_ == max_audit_subquery.c.audit_id,
+            ),
+            isouter=True,
+        )
     if scan_id > 0:
-        query = query.join(model.DBscanFinding,
-                           model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_)
-        query = query.filter(model.DBscanFinding.scan_id == scan_id)
+        query = query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
+        query = query.filter(DBscanFinding.scan_id == scan_id)
     else:
         if finding_statuses:
             if FindingStatus.NOT_ANALYZED in finding_statuses:
-                query = query. \
-                    filter(or_(model.DBaudit.status.in_(finding_statuses),
-                               model.DBaudit.status == None))  # noqa: E711
+                query = query.filter(
+                    or_(DBaudit.status.in_(finding_statuses), DBaudit.status == None)  # noqa: E711
+                )
             else:
-                query = query.filter(model.DBaudit.status.in_(finding_statuses))
+                query = query.filter(DBaudit.status.in_(finding_statuses))
 
         if vcs_providers:
-            query = query.filter(model.DBVcsInstance.provider_type.in_(vcs_providers))
+            query = query.filter(DBVcsInstance.provider_type.in_(vcs_providers))
 
         if project_name:
-            query = query.filter(model.DBrepository.project_key == project_name)
+            query = query.filter(DBrepository.project_key == project_name)
 
         if repository_name:
-            query = query.filter(model.DBrepository.repository_name == repository_name)
+            query = query.filter(DBrepository.repository_name == repository_name)
 
         if start_date_time:
-            query = query.filter(model.scan.DBscan.timestamp >= start_date_time)
+            query = query.filter(DBscan.timestamp >= start_date_time)
 
         if end_date_time:
-            query = query.filter(model.scan.DBscan.timestamp <= end_date_time)
+            query = query.filter(DBscan.timestamp <= end_date_time)
 
         if rule_pack_versions:
-            query = query.filter(model.DBscan.rule_pack.in_(rule_pack_versions))
+            query = query.filter(DBscan.rule_pack.in_(rule_pack_versions))
 
-    rules = query.distinct().order_by(model.DBfinding.rule_name).all()
+    rules = query.distinct().order_by(DBfinding.rule_name).all()
     return rules
 
 
-def get_findings_count_by_status(db_connection: Session, scan_ids: List[int] = None,
-                                 finding_statuses: [FindingStatus] = None, rule_name: str = ""):
+def get_findings_count_by_status(
+    db_connection: Session,
+    scan_ids: List[int] = None,
+    finding_statuses: List[FindingStatus] = None,
+    rule_name: str = "",
+):
     """
         Retrieve count of findings based on finding status
     :param db_connection:
         Session of the database connection
     :param scan_ids:
         List of scan ids for which findings should be filtered
     :param finding_statuses:
         finding statuses to filter, type FindingStatus
     :param rule_name:
         rule_name to filter on
     :return: findings_count
         count of findings
     """
     # subquery to select latest audit ids findings
-    max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
-                                             func.max(model.DBaudit.id_).label("audit_id")) \
-        .group_by(model.DBaudit.finding_id).subquery()
-
-    query = db_connection.query(func.count(model.DBfinding.id_).label('status_count'), model.DBaudit.status)
-
-    query = query \
-        .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
-              isouter=True) \
-        .join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
-                                  model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
-              isouter=True)
+    max_audit_subquery = (
+        db_connection.query(DBaudit.finding_id, func.max(DBaudit.id_).label("audit_id"))
+        .group_by(DBaudit.finding_id)
+        .subquery()
+    )
+
+    query = db_connection.query(
+        func.count(DBfinding.id_).label("status_count"), DBaudit.status
+    )
+
+    query = query.join(
+        max_audit_subquery,
+        max_audit_subquery.c.finding_id == DBfinding.id_,
+        isouter=True,
+    ).join(
+        DBaudit,
+        and_(
+            DBaudit.finding_id == DBfinding.id_,
+            DBaudit.id_ == max_audit_subquery.c.audit_id,
+        ),
+        isouter=True,
+    )
 
     if scan_ids and len(scan_ids) > 0:
-        query = query \
-            .join(model.DBscanFinding,
-                  model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_) \
-            .join(model.DBscan,
-                  model.scan.DBscan.id_ == model.scan_finding.DBscanFinding.scan_id) \
-            .filter(model.DBscan.id_.in_(scan_ids))
+        query = (
+            query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
+            .join(DBscan, DBscan.id_ == DBscanFinding.scan_id)
+            .filter(DBscan.id_.in_(scan_ids))
+        )
     if finding_statuses:
         if FindingStatus.NOT_ANALYZED in finding_statuses:
-            query = query. \
-                filter(or_(model.DBaudit.status.in_(finding_statuses),
-                           model.DBaudit.status == None))  # noqa: E711
+            query = query.filter(
+                or_(DBaudit.status.in_(finding_statuses), DBaudit.status == None)  # noqa: E711
+            )
         else:
-            query = query.filter(model.DBaudit.status.in_(finding_statuses))
+            query = query.filter(DBaudit.status.in_(finding_statuses))
     if rule_name:
-        query = query.filter(model.DBfinding.rule_name == rule_name)
+        query = query.filter(DBfinding.rule_name == rule_name)
 
-    findings_count_by_status = query.group_by(model.DBaudit.status).all()
+    findings_count_by_status = query.group_by(DBaudit.status).all()
 
     return findings_count_by_status
 
 
-def get_rule_findings_count_by_status(db_connection: Session, rule_pack_versions: [str] = None,
-                                      rule_tags: [str] = None):
+def get_rule_findings_count_by_status(
+    db_connection: Session,
+    rule_pack_versions: List[str] = None,
+    rule_tags: List[str] = None,
+):
     """
         Retrieve count of findings based on rulename and status
     :param db_connection:
         Session of the database connection
     :param rule_pack_versions:
         optional, filter on rule pack version
     :param rule_tags:
         optional, filter on rule tag
     :return: findings_count
         per rulename and status the count of findings
     """
-    query = db_connection.query(model.DBfinding.rule_name,
-                                model.DBaudit.status,
-                                func.count(model.DBfinding.id_))
-
-    max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
-                                                 func.max(model.DBscan.id_).label("latest_base_scan_id"))
-    max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
+    query = db_connection.query(
+        DBfinding.rule_name, DBaudit.status, func.count(DBfinding.id_)
+    )
+
+    max_base_scan_subquery = db_connection.query(
+        DBscan.repository_id, func.max(DBscan.id_).label("latest_base_scan_id")
+    )
+    max_base_scan_subquery = max_base_scan_subquery.filter(
+        DBscan.scan_type == ScanType.BASE
+    )
     if rule_pack_versions:
-        max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.rule_pack.in_(rule_pack_versions))
-    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
-
-    max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
-                                             func.max(model.DBaudit.id_).label("audit_id")) \
-        .group_by(model.DBaudit.finding_id).subquery()
-
-    query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
-    query = query.join(max_base_scan_subquery, model.DBfinding.repository_id == max_base_scan_subquery.c.repository_id)
-    query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
-                                          model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
+        max_base_scan_subquery = max_base_scan_subquery.filter(
+            DBscan.rule_pack.in_(rule_pack_versions)
+        )
+    max_base_scan_subquery = max_base_scan_subquery.group_by(
+        DBscan.repository_id
+    ).subquery()
+
+    max_audit_subquery = (
+        db_connection.query(DBaudit.finding_id, func.max(DBaudit.id_).label("audit_id"))
+        .group_by(DBaudit.finding_id)
+        .subquery()
+    )
+
+    query = query.join(DBscanFinding, DBfinding.id_ == DBscanFinding.finding_id)
+    query = query.join(
+        max_base_scan_subquery,
+        DBfinding.repository_id == max_base_scan_subquery.c.repository_id,
+    )
+    query = query.join(
+        DBscan,
+        and_(
+            DBscanFinding.scan_id == DBscan.id_,
+            DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id,
+        ),
+    )
     if rule_tags:
-        rule_tag_subquery = db_connection.query(model.DBruleTag.rule_id) \
-            .join(model.DBtag, model.DBruleTag.tag_id == model.DBtag.id_)
+        rule_tag_subquery = db_connection.query(DBruleTag.rule_id).join(
+            DBtag, DBruleTag.tag_id == DBtag.id_
+        )
         if rule_pack_versions:
-            rule_tag_subquery = rule_tag_subquery.join(model.DBrule, model.DBrule.id_ == model.DBruleTag.rule_id)
-            rule_tag_subquery = rule_tag_subquery.filter(model.DBrule.rule_pack.in_(rule_pack_versions))
-
-        rule_tag_subquery = rule_tag_subquery.filter(model.DBtag.name.in_(rule_tags))
-        rule_tag_subquery = rule_tag_subquery.group_by(model.DBruleTag.rule_id).subquery()
-
-        query = query.join(model.DBrule, and_(model.DBrule.rule_name == model.DBfinding.rule_name,
-                                              model.DBrule.rule_pack == model.DBscan.rule_pack))
-        query = query.join(rule_tag_subquery, model.DBrule.id_ == rule_tag_subquery.c.rule_id)
+            rule_tag_subquery = rule_tag_subquery.join(
+                DBrule, DBrule.id_ == DBruleTag.rule_id
+            )
+            rule_tag_subquery = rule_tag_subquery.filter(
+                DBrule.rule_pack.in_(rule_pack_versions)
+            )
+
+        rule_tag_subquery = rule_tag_subquery.filter(DBtag.name.in_(rule_tags))
+        rule_tag_subquery = rule_tag_subquery.group_by(DBruleTag.rule_id).subquery()
+
+        query = query.join(
+            DBrule,
+            and_(
+                DBrule.rule_name == DBfinding.rule_name,
+                DBrule.rule_pack == DBscan.rule_pack,
+            ),
+        )
+        query = query.join(rule_tag_subquery, DBrule.id_ == rule_tag_subquery.c.rule_id)
 
     if rule_pack_versions:
-        query = query.filter(model.DBscan.rule_pack.in_(rule_pack_versions))
+        query = query.filter(DBscan.rule_pack.in_(rule_pack_versions))
 
-    query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.DBscanFinding.finding_id,
-                       isouter=True)
-    query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.DBscanFinding.finding_id,
-                                           model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id), isouter=True)
-    query = query.group_by(model.DBfinding.rule_name, model.DBaudit.status)
-    query = query.order_by(model.DBfinding.rule_name, model.DBaudit.status)
+    query = query.join(
+        max_audit_subquery,
+        max_audit_subquery.c.finding_id == DBscanFinding.finding_id,
+        isouter=True,
+    )
+    query = query.join(
+        DBaudit,
+        and_(
+            DBaudit.finding_id == DBscanFinding.finding_id,
+            DBaudit.id_ == max_audit_subquery.c.audit_id,
+        ),
+        isouter=True,
+    )
+    query = query.group_by(DBfinding.rule_name, DBaudit.status)
+    query = query.order_by(DBfinding.rule_name, DBaudit.status)
     status_counts = query.all()
 
     rule_count_dict = {}
     for status_count in status_counts:
         rule_count_dict[status_count[0]] = {
             "true_positive": 0,
             "false_positive": 0,
             "not_analyzed": 0,
             "under_review": 0,
             "clarification_required": 0,
-            "total_findings_count": 0
+            "total_findings_count": 0,
         }
 
     for status_count in status_counts:
         rule_count_dict[status_count[0]]["total_findings_count"] += status_count[2]
         if status_count[1] == FindingStatus.NOT_ANALYZED or status_count[1] is None:
             rule_count_dict[status_count[0]]["not_analyzed"] += status_count[2]
         elif status_count[1] == FindingStatus.FALSE_POSITIVE:
             rule_count_dict[status_count[0]]["false_positive"] += status_count[2]
         elif status_count[1] == FindingStatus.TRUE_POSITIVE:
             rule_count_dict[status_count[0]]["true_positive"] += status_count[2]
         elif status_count[1] == FindingStatus.UNDER_REVIEW:
             rule_count_dict[status_count[0]]["under_review"] += status_count[2]
         elif status_count[1] == FindingStatus.CLARIFICATION_REQUIRED:
-            rule_count_dict[status_count[0]]["clarification_required"] += status_count[2]
+            rule_count_dict[status_count[0]]["clarification_required"] += status_count[
+                2
+            ]
 
     return rule_count_dict
 
 
-def get_findings_count_by_time(db_connection: Session,
-                               date_type: DateFilter,
-                               start_date_time: datetime = None,
-                               end_date_time: datetime = None,
-                               skip: int = 0,
-                               limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT):
+def get_findings_count_by_time(
+    db_connection: Session,
+    date_type: DateFilter,
+    start_date_time: datetime = None,
+    end_date_time: datetime = None,
+    skip: int = 0,
+    limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
+):
     """
         Retrieve count based on date_type
     :param db_connection:
         Session of the database connection
     :param date_type:
         required, filter on time_type
     :param start_date_time:
@@ -484,300 +638,428 @@
         optional, filter on end date
     :param skip:
         integer amount of records to skip to support pagination
     :param limit:
         integer amount of records to return, to support pagination
     """
     if date_type == DateFilter.MONTH:
-        query = db_connection.query(extract('year', model.DBscan.timestamp), extract('month', model.DBscan.timestamp),
-                                    func.count(model.DBscanFinding.finding_id))
+        query = db_connection.query(
+            extract("year", DBscan.timestamp),
+            extract("month", DBscan.timestamp),
+            func.count(DBscanFinding.finding_id),
+        )
     elif date_type == DateFilter.WEEK:
-        query = db_connection.query(extract('year', model.DBscan.timestamp), extract('week', model.DBscan.timestamp),
-                                    func.count(model.DBscanFinding.finding_id))
+        query = db_connection.query(
+            extract("year", DBscan.timestamp),
+            extract("week", DBscan.timestamp),
+            func.count(DBscanFinding.finding_id),
+        )
     elif date_type == DateFilter.DAY:
-        query = db_connection.query(extract('year', model.DBscan.timestamp), extract('month', model.DBscan.timestamp),
-                                    extract('day', model.DBscan.timestamp), func.count(model.DBscanFinding.finding_id))
+        query = db_connection.query(
+            extract("year", DBscan.timestamp),
+            extract("month", DBscan.timestamp),
+            extract("day", DBscan.timestamp),
+            func.count(DBscanFinding.finding_id),
+        )
 
-    query = query.join(model.DBscanFinding, model.DBscanFinding.scan_id == model.DBscan.id_)
+    query = query.join(DBscanFinding, DBscanFinding.scan_id == DBscan.id_)
 
     if start_date_time:
-        query = query.filter(model.DBscan.timestamp >= start_date_time)
+        query = query.filter(DBscan.timestamp >= start_date_time)
     if end_date_time:
-        query = query.filter(model.DBscan.timestamp <= end_date_time)
+        query = query.filter(DBscan.timestamp <= end_date_time)
 
     if date_type == DateFilter.MONTH:
-        query = query.group_by(extract('year', model.DBscan.timestamp), extract('month', model.DBscan.timestamp))
-        query = query.order_by(extract('year', model.DBscan.timestamp), extract('month', model.DBscan.timestamp))
+        query = query.group_by(
+            extract("year", DBscan.timestamp), extract("month", DBscan.timestamp)
+        )
+        query = query.order_by(
+            extract("year", DBscan.timestamp), extract("month", DBscan.timestamp)
+        )
     elif date_type == DateFilter.WEEK:
-        query = query.group_by(extract('year', model.DBscan.timestamp), extract('week', model.DBscan.timestamp))
-        query = query.order_by(extract('year', model.DBscan.timestamp), extract('week', model.DBscan.timestamp))
+        query = query.group_by(
+            extract("year", DBscan.timestamp), extract("week", DBscan.timestamp)
+        )
+        query = query.order_by(
+            extract("year", DBscan.timestamp), extract("week", DBscan.timestamp)
+        )
     elif date_type == DateFilter.DAY:
-        query = query.group_by(extract('year', model.DBscan.timestamp), extract('month', model.DBscan.timestamp),
-                               extract('day', model.DBscan.timestamp))
-        query = query.order_by(extract('year', model.DBscan.timestamp), extract('month', model.DBscan.timestamp),
-                               extract('day', model.DBscan.timestamp))
+        query = query.group_by(
+            extract("year", DBscan.timestamp),
+            extract("month", DBscan.timestamp),
+            extract("day", DBscan.timestamp),
+        )
+        query = query.order_by(
+            extract("year", DBscan.timestamp),
+            extract("month", DBscan.timestamp),
+            extract("day", DBscan.timestamp),
+        )
 
     finding_count = query.offset(skip).limit(limit).all()
     return finding_count
 
 
-def get_findings_count_by_time_total(db_connection: Session,
-                                     date_type: DateFilter,
-                                     start_date_time: datetime = None,
-                                     end_date_time: datetime = None):
+def get_findings_count_by_time_total(
+    db_connection: Session,
+    date_type: DateFilter,
+    start_date_time: datetime = None,
+    end_date_time: datetime = None,
+):
     """
         Retrieve total count on date_type
     :param db_connection:
         Session of the database connection
     :param date_type:
         required, filter on time_type
     :param start_date_time:
         optional, filter on start date
     :param end_date_time:
         optional, filter on end date
     """
     if date_type == DateFilter.MONTH:
-        query = db_connection.query(extract('year', model.DBscan.timestamp), extract('month', model.DBscan.timestamp))
+        query = db_connection.query(
+            extract("year", DBscan.timestamp), extract("month", DBscan.timestamp)
+        )
     elif date_type == DateFilter.WEEK:
-        query = db_connection.query(extract('year', model.DBscan.timestamp), extract('week', model.DBscan.timestamp))
+        query = db_connection.query(
+            extract("year", DBscan.timestamp), extract("week", DBscan.timestamp)
+        )
     elif date_type == DateFilter.DAY:
-        query = db_connection.query(extract('year', model.DBscan.timestamp), extract('month', model.DBscan.timestamp),
-                                    extract('day', model.DBscan.timestamp))
+        query = db_connection.query(
+            extract("year", DBscan.timestamp),
+            extract("month", DBscan.timestamp),
+            extract("day", DBscan.timestamp),
+        )
 
     if start_date_time:
-        query = query.filter(model.DBscan.timestamp >= start_date_time)
+        query = query.filter(DBscan.timestamp >= start_date_time)
     if end_date_time:
-        query = query.filter(model.DBscan.timestamp <= end_date_time)
+        query = query.filter(DBscan.timestamp <= end_date_time)
 
     query = query.distinct()
 
     result = query.count()
     return result
 
 
-def get_distinct_rules_from_scans(db_connection: Session, scan_ids: List[int] = None) -> \
-        List[model.DBrule]:
+def get_distinct_rules_from_scans(
+    db_connection: Session, scan_ids: List[int] = None
+) -> List[DBrule]:
     """
         Retrieve distinct rules detected
     :param db_connection:
         Session of the database connection
     :param scan_ids:
         List of scan ids
     :return: rules
         List of unique rules
     """
-    query = db_connection.query(model.DBfinding.rule_name)
+    query = db_connection.query(DBfinding.rule_name)
 
     if scan_ids:
-        query = query.join(model.DBscanFinding,
-                           model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_)
-        query = query.filter(model.DBscanFinding.scan_id.in_(scan_ids))
+        query = query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
+        query = query.filter(DBscanFinding.scan_id.in_(scan_ids))
 
-    rules = query.distinct().order_by(model.DBfinding.rule_name).all()
+    rules = query.distinct().order_by(DBfinding.rule_name).all()
     return rules
 
 
-def delete_finding(db_connection: Session, finding_id: int, delete_related: bool = False):
+def delete_finding(
+    db_connection: Session, finding_id: int, delete_related: bool = False
+):
     """
         Delete a finding object
     :param db_connection:
         Session of the database connection
     :param finding_id:
         id of the finding to be deleted
     :param delete_related:
         if related records need to be deleted
     """
     if delete_related:
         scan_finding_crud.delete_scan_finding(db_connection, finding_id=finding_id)
 
-    db_connection.query(model.DBfinding) \
-        .filter(model.finding.DBfinding.id_ == finding_id) \
-        .delete(synchronize_session=False)
+    db_connection.query(DBfinding).filter(DBfinding.id_ == finding_id).delete(
+        synchronize_session=False
+    )
     db_connection.commit()
 
 
 def delete_findings_by_repository_id(db_connection: Session, repository_id: int):
     """
         Delete findings for a given repository
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository
     """
-    db_connection.query(model.DBfinding) \
-        .filter(model.finding.DBfinding.repository_id == repository_id) \
-        .delete(synchronize_session=False)
+    db_connection.query(DBfinding).filter(
+        DBfinding.repository_id == repository_id
+    ).delete(synchronize_session=False)
     db_connection.commit()
 
 
 def delete_findings_by_vcs_instance_id(db_connection: Session, vcs_instance_id: int):
     """
         Delete findings for a given vcs instance
     :param db_connection:
         Session of the database connection
     :param vcs_instance_id:
         id of the vcs instance
     """
-    db_connection.query(model.DBfinding) \
-        .filter(model.finding.DBfinding.repository_id == model.repository.DBrepository.id_,
-                model.repository.DBrepository.vcs_instance == model.vcs_instance.DBVcsInstance.id_,
-                model.vcs_instance.DBVcsInstance.id_ == vcs_instance_id) \
-        .delete(synchronize_session=False)
+    db_connection.query(DBfinding).filter(
+        DBfinding.repository_id == DBrepository.id_,
+        DBrepository.vcs_instance == DBVcsInstance.id_,
+        DBVcsInstance.id_ == vcs_instance_id,
+    ).delete(synchronize_session=False)
     db_connection.commit()
 
 
-def get_finding_audit_status_count_over_time(db_connection: Session, status: FindingStatus, weeks: int = 13) -> dict:
+def get_finding_audit_status_count_over_time(
+    db_connection: Session, status: FindingStatus, weeks: int = 13
+) -> dict:
     """
         Retrieve count of true positive findings over time for given weeks
     :param db_connection:
         Session of the database connection
     :param status:
         mandatory, status for which to get the audit counts over time
     :param weeks:
         optional, filter on last n weeks, default 13
     :return: true_positive_count_over_time
         list of rows containing finding statuses count over time per week
     """
     all_tables = []
     for week in range(0, weeks):
         last_nth_week_date_time = datetime.utcnow() - timedelta(weeks=week)
-        query = db_connection.query(extract('year', last_nth_week_date_time).label("year"),
-                                    extract('week', last_nth_week_date_time).label("week"),
-                                    model.DBVcsInstance.provider_type.label("provider_type"),
-                                    func.count(model.DBaudit.id_).label("finding_count")
-                                    )
-        max_audit_subquery = db_connection.query(func.max(model.DBaudit.id_).label("audit_id")) \
-            .filter(or_(extract('year', model.DBaudit.timestamp) < extract('year', last_nth_week_date_time),
-                        and_(extract('year', model.DBaudit.timestamp) == extract('year', last_nth_week_date_time),
-                        extract('week', model.DBaudit.timestamp) <= extract('week', last_nth_week_date_time))))\
-            .group_by(model.DBaudit.finding_id).subquery()
-        query = query.join(max_audit_subquery, max_audit_subquery.c.audit_id == model.DBaudit.id_)
-        query = query.join(model.DBfinding, model.DBfinding.id_ == model.DBaudit.finding_id)
-        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBfinding.repository_id)
-        query = query.join(model.DBVcsInstance, model.DBVcsInstance.id_ == model.DBrepository.vcs_instance)
-        query = query.filter(model.DBaudit.status == status)
-        query = query.group_by(model.DBVcsInstance.provider_type)
+        query = db_connection.query(
+            extract("year", last_nth_week_date_time).label("year"),
+            extract("week", last_nth_week_date_time).label("week"),
+            DBVcsInstance.provider_type.label("provider_type"),
+            func.count(DBaudit.id_).label("finding_count"),
+        )
+        max_audit_subquery = (
+            db_connection.query(func.max(DBaudit.id_).label("audit_id"))
+            .filter(
+                or_(
+                    extract("year", DBaudit.timestamp)
+                    < extract("year", last_nth_week_date_time),
+                    and_(
+                        extract("year", DBaudit.timestamp)
+                        == extract("year", last_nth_week_date_time),
+                        extract("week", DBaudit.timestamp)
+                        <= extract("week", last_nth_week_date_time),
+                    ),
+                )
+            )
+            .group_by(DBaudit.finding_id)
+            .subquery()
+        )
+        query = query.join(
+            max_audit_subquery, max_audit_subquery.c.audit_id == DBaudit.id_
+        )
+        query = query.join(DBfinding, DBfinding.id_ == DBaudit.finding_id)
+        query = query.join(DBrepository, DBrepository.id_ == DBfinding.repository_id)
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
+        query = query.filter(DBaudit.status == status)
+        query = query.group_by(DBVcsInstance.provider_type)
 
         all_tables.append(query)
 
     # union
     unioned_query = union(*all_tables)
     status_count_over_time = db_connection.execute(unioned_query).all()
     return status_count_over_time
 
 
-def get_finding_count_by_vcs_provider_over_time(db_connection: Session, weeks: int = 13) -> list[Row]:
+def get_finding_count_by_vcs_provider_over_time(
+    db_connection: Session, weeks: int = 13
+) -> list[Row]:
     """
         Retrieve count findings over time for given weeks
     :param db_connection:
         Session of the database connection
     :param weeks:
         optional, filter on last n weeks, default 13
     :return: count_over_time
         list of rows containing finding count over time per week
     """
     all_tables = []
     for week in range(0, weeks):
         last_nth_week_date_time = datetime.utcnow() - timedelta(weeks=week)
-        query = db_connection.query(extract('year', last_nth_week_date_time).label("year"),
-                                    extract('week', last_nth_week_date_time).label("week"),
-                                    model.DBVcsInstance.provider_type.label("provider_type"),
-                                    func.count(model.DBfinding.id_).label("finding_count")
-                                    )
-        max_base_scan = db_connection.query(func.max(model.DBscan.id_).label("scan_id"),
-                                            model.DBscan.repository_id) \
-            .filter(or_(extract('year', model.DBaudit.timestamp) < extract('year', last_nth_week_date_time),
-                        and_(extract('year', model.DBaudit.timestamp) == extract('year', last_nth_week_date_time),
-                        extract('week', model.DBaudit.timestamp) <= extract('week', last_nth_week_date_time))))\
-            .filter(model.DBscan.scan_type == ScanType.BASE) \
-            .group_by(model.DBscan.repository_id).subquery()
-
-        query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
-        query = query.join(model.DBscan, model.DBscan.id_ == model.DBscanFinding.scan_id)
-        query = query.join(max_base_scan, and_(max_base_scan.c.repository_id == model.DBscan.repository_id,
-                                               or_(model.DBscan.id_ == max_base_scan.c.scan_id,
-                                                   (and_(model.DBscan.id_ > max_base_scan.c.scan_id,
-                                                         model.DBscan.scan_type == ScanType.INCREMENTAL,
-                                                         extract('week', model.DBscan.timestamp) <=
-                                                         extract('week', last_nth_week_date_time),
-                                                         extract('year', model.DBscan.timestamp) ==
-                                                         extract('year', last_nth_week_date_time)))
-                                                   )
-                                               )
-                           )
-        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBscan.repository_id)
-        query = query.join(model.DBVcsInstance, model.DBVcsInstance.id_ == model.DBrepository.vcs_instance)
-        query = query.group_by(model.DBVcsInstance.provider_type)
+        query = db_connection.query(
+            extract("year", last_nth_week_date_time).label("year"),
+            extract("week", last_nth_week_date_time).label("week"),
+            DBVcsInstance.provider_type.label("provider_type"),
+            func.count(DBfinding.id_).label("finding_count"),
+        )
+        max_base_scan = (
+            db_connection.query(
+                func.max(DBscan.id_).label("scan_id"), DBscan.repository_id
+            )
+            .filter(
+                or_(
+                    extract("year", DBaudit.timestamp)
+                    < extract("year", last_nth_week_date_time),
+                    and_(
+                        extract("year", DBaudit.timestamp)
+                        == extract("year", last_nth_week_date_time),
+                        extract("week", DBaudit.timestamp)
+                        <= extract("week", last_nth_week_date_time),
+                    ),
+                )
+            )
+            .filter(DBscan.scan_type == ScanType.BASE)
+            .group_by(DBscan.repository_id)
+            .subquery()
+        )
+
+        query = query.join(DBscanFinding, DBfinding.id_ == DBscanFinding.finding_id)
+        query = query.join(DBscan, DBscan.id_ == DBscanFinding.scan_id)
+        query = query.join(
+            max_base_scan,
+            and_(
+                max_base_scan.c.repository_id == DBscan.repository_id,
+                or_(
+                    DBscan.id_ == max_base_scan.c.scan_id,
+                    (
+                        and_(
+                            DBscan.id_ > max_base_scan.c.scan_id,
+                            DBscan.scan_type == ScanType.INCREMENTAL,
+                            extract("week", DBscan.timestamp)
+                            <= extract("week", last_nth_week_date_time),
+                            extract("year", DBscan.timestamp)
+                            == extract("year", last_nth_week_date_time),
+                        )
+                    ),
+                ),
+            ),
+        )
+        query = query.join(DBrepository, DBrepository.id_ == DBscan.repository_id)
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
+        query = query.group_by(DBVcsInstance.provider_type)
 
         all_tables.append(query)
 
     # union
     unioned_query = union(*all_tables)
     count_over_time = db_connection.execute(unioned_query).all()
     return count_over_time
 
 
-def get_un_triaged_finding_count_by_vcs_provider_over_time(db_connection: Session, weeks: int = 13) -> list[Row]:
+def get_un_triaged_finding_count_by_vcs_provider_over_time(
+    db_connection: Session, weeks: int = 13
+) -> list[Row]:
     """
         Retrieve count of un triaged findings over time for given weeks
     :param db_connection:
         Session of the database connection
     :param weeks:
         optional, filter on last n weeks, default 13
     :return: count_over_time
         list of rows containing un triaged findings count over time per week
     """
     all_tables = []
     for week in range(0, weeks):
         last_nth_week_date_time = datetime.utcnow() - timedelta(weeks=week)
-        query = db_connection.query(extract('year', last_nth_week_date_time).label("year"),
-                                    extract('week', last_nth_week_date_time).label("week"),
-                                    model.DBVcsInstance.provider_type.label("provider_type"),
-                                    func.count(model.DBfinding.id_).label("finding_count")
-                                    )
-        max_base_scan = db_connection.query(func.max(model.DBscan.id_).label("scan_id"),
-                                            model.DBscan.repository_id) \
-            .filter(or_(extract('year', model.DBaudit.timestamp) < extract('year', last_nth_week_date_time),
-                        and_(extract('year', model.DBaudit.timestamp) == extract('year', last_nth_week_date_time),
-                        extract('week', model.DBaudit.timestamp) <= extract('week', last_nth_week_date_time))))\
-            .filter(model.DBscan.scan_type == ScanType.BASE) \
-            .group_by(model.DBscan.repository_id).subquery()
-
-        max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
-                                                 func.max(model.DBaudit.id_).label("audit_id")) \
-            .filter(or_(extract('year', model.DBaudit.timestamp) < extract('year', last_nth_week_date_time),
-                        and_(extract('year', model.DBaudit.timestamp) == extract('year', last_nth_week_date_time),
-                        extract('week', model.DBaudit.timestamp) <= extract('week', last_nth_week_date_time))))\
-            .group_by(model.DBaudit.finding_id).subquery()
-
-        query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
-        query = query.join(model.DBscan, model.DBscan.id_ == model.DBscanFinding.scan_id)
-        query = query.join(max_base_scan, and_(max_base_scan.c.repository_id == model.DBscan.repository_id,
-                                               or_(model.DBscan.id_ == max_base_scan.c.scan_id,
-                                                   (and_(model.DBscan.id_ > max_base_scan.c.scan_id,
-                                                         model.DBscan.scan_type == ScanType.INCREMENTAL,
-                                                         extract('week', model.DBscan.timestamp) <=
-                                                         extract('week', last_nth_week_date_time),
-                                                         extract('year', model.DBscan.timestamp) ==
-                                                         extract('year', last_nth_week_date_time)))
-                                                   )
-                                               )
-                           )
-        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBscan.repository_id)
-        query = query.join(model.DBVcsInstance, model.DBVcsInstance.id_ == model.DBrepository.vcs_instance)
-
-        query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
-                           isouter=True)
-        query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
-                                               model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
-                           isouter=True)
+        query = db_connection.query(
+            extract("year", last_nth_week_date_time).label("year"),
+            extract("week", last_nth_week_date_time).label("week"),
+            DBVcsInstance.provider_type.label("provider_type"),
+            func.count(DBfinding.id_).label("finding_count"),
+        )
+        max_base_scan = (
+            db_connection.query(
+                func.max(DBscan.id_).label("scan_id"), DBscan.repository_id
+            )
+            .filter(
+                or_(
+                    extract("year", DBaudit.timestamp)
+                    < extract("year", last_nth_week_date_time),
+                    and_(
+                        extract("year", DBaudit.timestamp)
+                        == extract("year", last_nth_week_date_time),
+                        extract("week", DBaudit.timestamp)
+                        <= extract("week", last_nth_week_date_time),
+                    ),
+                )
+            )
+            .filter(DBscan.scan_type == ScanType.BASE)
+            .group_by(DBscan.repository_id)
+            .subquery()
+        )
+
+        max_audit_subquery = (
+            db_connection.query(
+                DBaudit.finding_id, func.max(DBaudit.id_).label("audit_id")
+            )
+            .filter(
+                or_(
+                    extract("year", DBaudit.timestamp)
+                    < extract("year", last_nth_week_date_time),
+                    and_(
+                        extract("year", DBaudit.timestamp)
+                        == extract("year", last_nth_week_date_time),
+                        extract("week", DBaudit.timestamp)
+                        <= extract("week", last_nth_week_date_time),
+                    ),
+                )
+            )
+            .group_by(DBaudit.finding_id)
+            .subquery()
+        )
+
+        query = query.join(DBscanFinding, DBfinding.id_ == DBscanFinding.finding_id)
+        query = query.join(DBscan, DBscan.id_ == DBscanFinding.scan_id)
+        query = query.join(
+            max_base_scan,
+            and_(
+                max_base_scan.c.repository_id == DBscan.repository_id,
+                or_(
+                    DBscan.id_ == max_base_scan.c.scan_id,
+                    (
+                        and_(
+                            DBscan.id_ > max_base_scan.c.scan_id,
+                            DBscan.scan_type == ScanType.INCREMENTAL,
+                            extract("week", DBscan.timestamp)
+                            <= extract("week", last_nth_week_date_time),
+                            extract("year", DBscan.timestamp)
+                            == extract("year", last_nth_week_date_time),
+                        )
+                    ),
+                ),
+            ),
+        )
+        query = query.join(DBrepository, DBrepository.id_ == DBscan.repository_id)
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
+
+        query = query.join(
+            max_audit_subquery,
+            max_audit_subquery.c.finding_id == DBfinding.id_,
+            isouter=True,
+        )
+        query = query.join(
+            DBaudit,
+            and_(
+                DBaudit.finding_id == DBfinding.id_,
+                DBaudit.id_ == max_audit_subquery.c.audit_id,
+            ),
+            isouter=True,
+        )
         query = query.filter(
-            or_(model.DBaudit.id_ == None, model.DBaudit.status == FindingStatus.NOT_ANALYZED))  # noqa: E711
+            or_(DBaudit.id_ == None, DBaudit.status == FindingStatus.NOT_ANALYZED)  # noqa: E711
+        )
 
-        query = query.group_by(model.DBVcsInstance.provider_type)
+        query = query.group_by(DBVcsInstance.provider_type)
 
         all_tables.append(query)
 
     # union
     unioned_query = union(*all_tables)
     count_over_time = db_connection.execute(unioned_query).all()
     return count_over_time
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/repository.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,44 @@
-# pylint:disable=not-callable
+# Standard Library
+from typing import List
+
 # Third Party
 from sqlalchemy import and_, func
 from sqlalchemy.orm import Session
 
 # First Party
-from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
-from resc_backend.db import model
+from resc_backend.constants import (
+    DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    MAX_RECORDS_PER_PAGE_LIMIT,
+)
+from resc_backend.db.model import (
+    DBaudit,
+    DBrepository,
+    DBscan,
+    DBscanFinding,
+    DBVcsInstance,
+)
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.crud import scan as scan_crud
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.schema import repository as repository_schema
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 
-def get_repositories(db_connection: Session, vcs_providers: [VCSProviders] = None, skip: int = 0,
-                     limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT, project_filter: str = "",
-                     repository_filter: str = "", only_if_has_findings: bool = False):
+def get_repositories(
+    db_connection: Session,
+    vcs_providers: List[VCSProviders] = None,
+    skip: int = 0,
+    limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    project_filter: str = "",
+    repository_filter: str = "",
+    only_if_has_findings: bool = False,
+):
     """
         Retrieve repository records optionally filtered
     :param db_connection:
         Session of the database connection
     :param skip:
         integer amount of records to skip to support pagination
     :param limit:
@@ -33,72 +50,102 @@
     :param repository_filter:
         optional, filter on repository name. Is used as a string contains filter
     :param only_if_has_findings:
         optional, filter on repositories with findings
     :return: repositories
         list of DBrepository objects
     """
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
 
     # Get the latest scan for repository
-    repo_last_scan_sub_query = db_connection.query(model.DBscan.repository_id,
-                                                   func.max(model.DBscan.timestamp).label("max_timestamp"))
-    repo_last_scan_sub_query = repo_last_scan_sub_query.group_by(model.DBscan.repository_id).subquery()
+    repo_last_scan_sub_query = db_connection.query(
+        DBscan.repository_id, func.max(DBscan.timestamp).label("max_timestamp")
+    )
+    repo_last_scan_sub_query = repo_last_scan_sub_query.group_by(
+        DBscan.repository_id
+    ).subquery()
 
     query = db_connection.query(
-        model.DBrepository.id_,
-        model.DBrepository.project_key,
-        model.DBrepository.repository_id,
-        model.DBrepository.repository_name,
-        model.DBrepository.repository_url,
-        model.DBrepository.vcs_instance,
-        model.DBVcsInstance.provider_type,
-        func.coalesce(model.DBscan.id_, None).label('last_scan_id'),
-        func.coalesce(model.DBscan.timestamp, None).label('last_scan_timestamp'))
-    query = query.join(model.DBVcsInstance,
-                       model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
-    query = query.join(repo_last_scan_sub_query,
-                       model.repository.DBrepository.id_ == repo_last_scan_sub_query.c.repository_id, isouter=True)
-    query = query.join(model.DBscan,
-                       and_(model.scan.DBscan.repository_id == repo_last_scan_sub_query.c.repository_id,
-                            model.scan.DBscan.timestamp == repo_last_scan_sub_query.c.max_timestamp), isouter=True)
+        DBrepository.id_,
+        DBrepository.project_key,
+        DBrepository.repository_id,
+        DBrepository.repository_name,
+        DBrepository.repository_url,
+        DBrepository.vcs_instance,
+        DBVcsInstance.provider_type,
+        func.coalesce(DBscan.id_, None).label("last_scan_id"),
+        func.coalesce(DBscan.timestamp, None).label("last_scan_timestamp"),
+    )
+    query = query.join(DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance)
+    query = query.join(
+        repo_last_scan_sub_query,
+        DBrepository.id_ == repo_last_scan_sub_query.c.repository_id,
+        isouter=True,
+    )
+    query = query.join(
+        DBscan,
+        and_(
+            DBscan.repository_id == repo_last_scan_sub_query.c.repository_id,
+            DBscan.timestamp == repo_last_scan_sub_query.c.max_timestamp,
+        ),
+        isouter=True,
+    )
 
     if only_if_has_findings:
-        max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
-                                                     func.max(model.DBscan.id_).label("latest_base_scan_id"))
-        max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
-        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
-
-        sub_query = db_connection.query(model.DBrepository.id_)
-        sub_query = sub_query.join(max_base_scan_subquery,
-                                   model.DBrepository.id_ == max_base_scan_subquery.c.repository_id)
-        sub_query = sub_query.join(model.DBscan, and_(model.DBrepository.id_ == model.DBscan.repository_id,
-                                                      model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
-        sub_query = sub_query.join(model.DBscanFinding, model.DBscan.id_ == model.DBscanFinding.scan_id)
+        max_base_scan_subquery = db_connection.query(
+            DBscan.repository_id, func.max(DBscan.id_).label("latest_base_scan_id")
+        )
+        max_base_scan_subquery = max_base_scan_subquery.filter(
+            DBscan.scan_type == ScanType.BASE
+        )
+        max_base_scan_subquery = max_base_scan_subquery.group_by(
+            DBscan.repository_id
+        ).subquery()
+
+        sub_query = db_connection.query(DBrepository.id_)
+        sub_query = sub_query.join(
+            max_base_scan_subquery,
+            DBrepository.id_ == max_base_scan_subquery.c.repository_id,
+        )
+        sub_query = sub_query.join(
+            DBscan,
+            and_(
+                DBrepository.id_ == DBscan.repository_id,
+                DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id,
+            ),
+        )
+        sub_query = sub_query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
         sub_query = sub_query.distinct()
 
         # Filter on repositories that are in the selection
-        query = query.filter(model.DBrepository.id_.in_(sub_query))
+        query = query.filter(DBrepository.id_.in_(sub_query))
 
     if vcs_providers and vcs_providers is not None:
-        query = query.filter(model.DBVcsInstance.provider_type.in_(vcs_providers))
+        query = query.filter(DBVcsInstance.provider_type.in_(vcs_providers))
 
     if project_filter:
-        query = query.filter(model.DBrepository.project_key == project_filter)
+        query = query.filter(DBrepository.project_key == project_filter)
 
     if repository_filter:
-        query = query.filter(model.DBrepository.repository_name == repository_filter)
+        query = query.filter(DBrepository.repository_name == repository_filter)
 
-    repositories = query.order_by(model.DBrepository.id_).offset(skip).limit(limit_val).all()
+    repositories = query.order_by(DBrepository.id_).offset(skip).limit(limit_val).all()
 
     return repositories
 
 
-def get_repositories_count(db_connection: Session, vcs_providers: [VCSProviders] = None, project_filter: str = "",
-                           repository_filter: str = "", only_if_has_findings: bool = False) -> int:
+def get_repositories_count(
+    db_connection: Session,
+    vcs_providers: List[VCSProviders] = None,
+    project_filter: str = "",
+    repository_filter: str = "",
+    only_if_has_findings: bool = False,
+) -> int:
     """
         Retrieve count of repository records optionally filtered
     :param db_connection:
         Session of the database connection
     :param vcs_providers:
         optional [string] filtering the VCS provider
     :param project_filter:
@@ -106,261 +153,367 @@
     :param repository_filter:
         optional, filter on repository name
     :param only_if_has_findings:
         optional, filter on repositories with findings
     :return: total_count
         count of repositories
     """
-    query = db_connection.query(func.count(model.DBrepository.id_))
+    query = db_connection.query(func.count(DBrepository.id_))
 
     if only_if_has_findings:
-        max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
-                                                     func.max(model.DBscan.id_).label("latest_base_scan_id"))
-        max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
-        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
-
-        sub_query = db_connection.query(model.DBrepository.id_)
-        sub_query = sub_query.join(max_base_scan_subquery,
-                                   model.DBrepository.id_ == max_base_scan_subquery.c.repository_id)
-        sub_query = sub_query.join(model.DBscan, and_(model.DBrepository.id_ == model.DBscan.repository_id,
-                                                      model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
-        sub_query = sub_query.join(model.DBscanFinding, model.DBscan.id_ == model.DBscanFinding.scan_id)
+        max_base_scan_subquery = db_connection.query(
+            DBscan.repository_id, func.max(DBscan.id_).label("latest_base_scan_id")
+        )
+        max_base_scan_subquery = max_base_scan_subquery.filter(
+            DBscan.scan_type == ScanType.BASE
+        )
+        max_base_scan_subquery = max_base_scan_subquery.group_by(
+            DBscan.repository_id
+        ).subquery()
+
+        sub_query = db_connection.query(DBrepository.id_)
+        sub_query = sub_query.join(
+            max_base_scan_subquery,
+            DBrepository.id_ == max_base_scan_subquery.c.repository_id,
+        )
+        sub_query = sub_query.join(
+            DBscan,
+            and_(
+                DBrepository.id_ == DBscan.repository_id,
+                DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id,
+            ),
+        )
+        sub_query = sub_query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
         sub_query = sub_query.distinct()
 
         # Filter on repositories that are in the selection
-        query = query.filter(model.DBrepository.id_.in_(sub_query))
+        query = query.filter(DBrepository.id_.in_(sub_query))
 
     if vcs_providers and vcs_providers is not None:
-        query = query.join(model.DBVcsInstance,
-                           model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
-        query = query.filter(model.DBVcsInstance.provider_type.in_(vcs_providers))
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
+        query = query.filter(DBVcsInstance.provider_type.in_(vcs_providers))
 
     if project_filter:
-        query = query.filter(model.DBrepository.project_key == project_filter)
+        query = query.filter(DBrepository.project_key == project_filter)
 
     if repository_filter:
-        query = query.filter(model.DBrepository.repository_name == repository_filter)
+        query = query.filter(DBrepository.repository_name == repository_filter)
 
     total_count = query.scalar()
     return total_count
 
 
 def get_repository(db_connection: Session, repository_id: int):
-    repository = db_connection.query(model.DBrepository) \
-        .filter(model.repository.DBrepository.id_ == repository_id).first()
+    repository = (
+        db_connection.query(DBrepository)
+        .filter(DBrepository.id_ == repository_id)
+        .first()
+    )
     return repository
 
 
 def update_repository(
-        db_connection: Session, repository_id: int, repository: repository_schema.RepositoryCreate):
-    db_repository = db_connection.query(model.DBrepository).filter_by(id_=repository_id).first()
+    db_connection: Session,
+    repository_id: int,
+    repository: repository_schema.RepositoryCreate,
+):
+    db_repository = (
+        db_connection.query(DBrepository).filter_by(id_=repository_id).first()
+    )
 
     db_repository.repository_name = repository.repository_name
     db_repository.repository_url = repository.repository_url
     db_repository.vcs_instance = repository.vcs_instance
 
     db_connection.commit()
     db_connection.refresh(db_repository)
     return db_repository
 
 
-def create_repository(db_connection: Session, repository: repository_schema.RepositoryCreate):
-    db_repository = model.repository.DBrepository(
+def create_repository(
+    db_connection: Session, repository: repository_schema.RepositoryCreate
+):
+    db_repository = DBrepository(
         project_key=repository.project_key,
         repository_id=repository.repository_id,
         repository_name=repository.repository_name,
         repository_url=repository.repository_url,
-        vcs_instance=repository.vcs_instance
+        vcs_instance=repository.vcs_instance,
     )
     db_connection.add(db_repository)
     db_connection.commit()
     db_connection.refresh(db_repository)
     return db_repository
 
 
-def create_repository_if_not_exists(db_connection: Session,
-                                    repository: repository_schema.RepositoryCreate):
+def create_repository_if_not_exists(
+    db_connection: Session, repository: repository_schema.RepositoryCreate
+):
     # Query the database to see if the repository object exists based on the unique constraint parameters
-    db_select_repository = db_connection.query(model.DBrepository) \
-        .filter(model.repository.DBrepository.project_key == repository.project_key,
-                model.repository.DBrepository.repository_id == repository.repository_id,
-                model.repository.DBrepository.vcs_instance == repository.vcs_instance).first()
+    db_select_repository = (
+        db_connection.query(DBrepository)
+        .filter(
+            DBrepository.project_key == repository.project_key,
+            DBrepository.repository_id == repository.repository_id,
+            DBrepository.vcs_instance == repository.vcs_instance,
+        )
+        .first()
+    )
     if db_select_repository is not None:
         return db_select_repository
 
     # Create non-existing repository object
     return create_repository(db_connection, repository)
 
 
-def get_distinct_projects(db_connection: Session, vcs_providers: [VCSProviders] = None, repository_filter: str = "",
-                          only_if_has_findings: bool = False):
+def get_distinct_projects(
+    db_connection: Session,
+    vcs_providers: List[VCSProviders] = None,
+    repository_filter: str = "",
+    only_if_has_findings: bool = False,
+):
     """
         Retrieve all unique project names
     :param db_connection:
         Session of the database connection
     :param vcs_providers:
         optional, filter of supported vcs provider types
     :param repository_filter:
         optional, filter on repository name. Is used as a string contains filter
     :param only_if_has_findings:
         optional, filter on repositories that have findings
     :return: distinct_projects
         The output will contain a list of unique projects
     """
-    query = db_connection.query(model.DBrepository.project_key)
+    query = db_connection.query(DBrepository.project_key)
 
     if only_if_has_findings:
-        max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
-                                                     func.max(model.DBscan.id_).label("latest_base_scan_id"))
-        max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
-        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
-
-        query = query.join(max_base_scan_subquery, model.DBrepository.id_ == max_base_scan_subquery.c.repository_id)
-        query = query.join(model.DBscan, and_(model.DBrepository.id_ == model.DBscan.repository_id,
-                                              model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
-        query = query.join(model.DBscanFinding, model.DBscan.id_ == model.DBscanFinding.scan_id)
+        max_base_scan_subquery = db_connection.query(
+            DBscan.repository_id, func.max(DBscan.id_).label("latest_base_scan_id")
+        )
+        max_base_scan_subquery = max_base_scan_subquery.filter(
+            DBscan.scan_type == ScanType.BASE
+        )
+        max_base_scan_subquery = max_base_scan_subquery.group_by(
+            DBscan.repository_id
+        ).subquery()
+
+        query = query.join(
+            max_base_scan_subquery,
+            DBrepository.id_ == max_base_scan_subquery.c.repository_id,
+        )
+        query = query.join(
+            DBscan,
+            and_(
+                DBrepository.id_ == DBscan.repository_id,
+                DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id,
+            ),
+        )
+        query = query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
 
     if vcs_providers and vcs_providers is not None:
-        query = query.join(model.DBVcsInstance,
-                           model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
-        query = query.filter(model.DBVcsInstance.provider_type.in_(vcs_providers))
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
+        query = query.filter(DBVcsInstance.provider_type.in_(vcs_providers))
 
     if repository_filter:
-        query = query.filter(model.DBrepository.repository_name == repository_filter)
+        query = query.filter(DBrepository.repository_name == repository_filter)
 
     distinct_projects = query.distinct().all()
     return distinct_projects
 
 
-def get_distinct_repositories(db_connection: Session, vcs_providers: [VCSProviders] = None, project_name: str = "",
-                              only_if_has_findings: bool = False):
+def get_distinct_repositories(
+    db_connection: Session,
+    vcs_providers: List[VCSProviders] = None,
+    project_name: str = "",
+    only_if_has_findings: bool = False,
+):
     """
         Retrieve all unique repository names
     :param db_connection:
         Session of the database connection
     :param vcs_providers:
         optional, filter of supported vcs provider types
     :param project_name:
         optional, filter on project name. Is used as a full string match filter
     :param only_if_has_findings:
         optional, filter on repositories that have findings
     :return: distinct_repositories
         The output will contain a list of unique repositories
     """
-    query = db_connection.query(model.DBrepository.repository_name)
+    query = db_connection.query(DBrepository.repository_name)
 
     if only_if_has_findings:
-        max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
-                                                     func.max(model.DBscan.id_).label("latest_base_scan_id"))
-        max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
-        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
-
-        query = query.join(max_base_scan_subquery, model.DBrepository.id_ == max_base_scan_subquery.c.repository_id)
-        query = query.join(model.DBscan, and_(model.DBrepository.id_ == model.DBscan.repository_id,
-                                              model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
-        query = query.join(model.DBscanFinding, model.DBscan.id_ == model.DBscanFinding.scan_id)
+        max_base_scan_subquery = db_connection.query(
+            DBscan.repository_id, func.max(DBscan.id_).label("latest_base_scan_id")
+        )
+        max_base_scan_subquery = max_base_scan_subquery.filter(
+            DBscan.scan_type == ScanType.BASE
+        )
+        max_base_scan_subquery = max_base_scan_subquery.group_by(
+            DBscan.repository_id
+        ).subquery()
+
+        query = query.join(
+            max_base_scan_subquery,
+            DBrepository.id_ == max_base_scan_subquery.c.repository_id,
+        )
+        query = query.join(
+            DBscan,
+            and_(
+                DBrepository.id_ == DBscan.repository_id,
+                DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id,
+            ),
+        )
+        query = query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
 
     if vcs_providers and vcs_providers is not None:
-        query = query.join(model.DBVcsInstance,
-                           model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
-        query = query.filter(model.DBVcsInstance.provider_type.in_(vcs_providers))
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
+        query = query.filter(DBVcsInstance.provider_type.in_(vcs_providers))
 
     if project_name:
-        query = query.filter(model.DBrepository.project_key == project_name)
+        query = query.filter(DBrepository.project_key == project_name)
 
     distinct_repositories = query.distinct().all()
     return distinct_repositories
 
 
-def get_findings_metadata_by_repository_id(db_connection: Session, repository_ids: list[int]):
+def get_findings_metadata_by_repository_id(
+    db_connection: Session, repository_ids: list[int]
+):
     """
         Retrieves the finding metadata for a repository id from the database with most recent scan information
     :param db_connection:
         Session of the database connection
     :param repository_ids:
         ids of the repository for which findings metadata to be retrieved
     :return: findings_metadata
         findings_metadata containing the count for each status
     """
-    query = db_connection.query(model.DBrepository.id_,
-                                model.DBaudit.status,
-                                func.count(model.DBscanFinding.finding_id))
-
-    max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
-                                                 func.max(model.DBscan.id_).label("latest_base_scan_id"))
-    max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
-    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
-
-    max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
-                                             func.max(model.DBaudit.id_).label("audit_id")) \
-        .group_by(model.DBaudit.finding_id).subquery()
-
-    query = query.join(max_base_scan_subquery, model.DBrepository.id_ == max_base_scan_subquery.c.repository_id)
-    query = query.join(model.DBscan, and_(model.DBrepository.id_ == model.DBscan.repository_id,
-                                          model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
-    query = query.join(model.DBscanFinding, model.DBscan.id_ == model.DBscanFinding.scan_id)
-    query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.DBscanFinding.finding_id,
-                       isouter=True)
-    query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.DBscanFinding.finding_id,
-                                           model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id), isouter=True)
-    query = query.filter(model.DBrepository.id_.in_(repository_ids))
-    query = query.group_by(model.DBrepository.id_, model.DBaudit.status, )
+    query = db_connection.query(
+        DBrepository.id_, DBaudit.status, func.count(DBscanFinding.finding_id)
+    )
+
+    max_base_scan_subquery = db_connection.query(
+        DBscan.repository_id, func.max(DBscan.id_).label("latest_base_scan_id")
+    )
+    max_base_scan_subquery = max_base_scan_subquery.filter(
+        DBscan.scan_type == ScanType.BASE
+    )
+    max_base_scan_subquery = max_base_scan_subquery.group_by(
+        DBscan.repository_id
+    ).subquery()
+
+    max_audit_subquery = (
+        db_connection.query(DBaudit.finding_id, func.max(DBaudit.id_).label("audit_id"))
+        .group_by(DBaudit.finding_id)
+        .subquery()
+    )
+
+    query = query.join(
+        max_base_scan_subquery,
+        DBrepository.id_ == max_base_scan_subquery.c.repository_id,
+    )
+    query = query.join(
+        DBscan,
+        and_(
+            DBrepository.id_ == DBscan.repository_id,
+            DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id,
+        ),
+    )
+    query = query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
+    query = query.join(
+        max_audit_subquery,
+        max_audit_subquery.c.finding_id == DBscanFinding.finding_id,
+        isouter=True,
+    )
+    query = query.join(
+        DBaudit,
+        and_(
+            DBaudit.finding_id == DBscanFinding.finding_id,
+            DBaudit.id_ == max_audit_subquery.c.audit_id,
+        ),
+        isouter=True,
+    )
+    query = query.filter(DBrepository.id_.in_(repository_ids))
+    query = query.group_by(
+        DBrepository.id_,
+        DBaudit.status,
+    )
     status_counts = query.all()
     repo_count_dict = {}
     for repository_id in repository_ids:
         repo_count_dict[repository_id] = {
             "true_positive": 0,
             "false_positive": 0,
             "not_analyzed": 0,
             "under_review": 0,
             "clarification_required": 0,
-            "total_findings_count": 0
+            "total_findings_count": 0,
         }
     for status_count in status_counts:
         repo_count_dict[status_count[0]]["total_findings_count"] += status_count[2]
         if status_count[1] == FindingStatus.NOT_ANALYZED or status_count[1] is None:
             repo_count_dict[status_count[0]]["not_analyzed"] += status_count[2]
         elif status_count[1] == FindingStatus.FALSE_POSITIVE:
             repo_count_dict[status_count[0]]["false_positive"] += status_count[2]
         elif status_count[1] == FindingStatus.TRUE_POSITIVE:
             repo_count_dict[status_count[0]]["true_positive"] += status_count[2]
         elif status_count[1] == FindingStatus.UNDER_REVIEW:
             repo_count_dict[status_count[0]]["under_review"] += status_count[2]
         elif status_count[1] == FindingStatus.CLARIFICATION_REQUIRED:
-            repo_count_dict[status_count[0]]["clarification_required"] += status_count[2]
+            repo_count_dict[status_count[0]]["clarification_required"] += status_count[
+                2
+            ]
 
     return repo_count_dict
 
 
-def delete_repository(db_connection: Session, repository_id: int, delete_related: bool = False):
+def delete_repository(
+    db_connection: Session, repository_id: int, delete_related: bool = False
+):
     """
         Delete a repository object
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository to be deleted
     :param delete_related:
         if related records need to be deleted
     """
     if delete_related:
-        scan_finding_crud.delete_scan_finding_by_repository_id(db_connection, repository_id=repository_id)
-        finding_crud.delete_findings_by_repository_id(db_connection, repository_id=repository_id)
-        scan_crud.delete_scans_by_repository_id(db_connection, repository_id=repository_id)
-    db_connection.query(model.DBrepository) \
-        .filter(model.repository.DBrepository.id_ == repository_id) \
-        .delete(synchronize_session=False)
+        scan_finding_crud.delete_scan_finding_by_repository_id(
+            db_connection, repository_id=repository_id
+        )
+        finding_crud.delete_findings_by_repository_id(
+            db_connection, repository_id=repository_id
+        )
+        scan_crud.delete_scans_by_repository_id(
+            db_connection, repository_id=repository_id
+        )
+    db_connection.query(DBrepository).filter(DBrepository.id_ == repository_id).delete(
+        synchronize_session=False
+    )
     db_connection.commit()
 
 
-def delete_repositories_by_vcs_instance_id(db_connection: Session, vcs_instance_id: int):
+def delete_repositories_by_vcs_instance_id(
+    db_connection: Session, vcs_instance_id: int
+):
     """
         Delete repositories for a given vcs instance
     :param db_connection:
         Session of the database connection
     :param vcs_instance_id:
         id of the vcs instance
     """
-    db_connection.query(model.DBrepository) \
-        .filter(model.repository.DBrepository.vcs_instance == model.vcs_instance.DBVcsInstance.id_,
-                model.vcs_instance.DBVcsInstance.id_ == vcs_instance_id) \
-        .delete(synchronize_session=False)
+    db_connection.query(DBrepository).filter(
+        DBrepository.vcs_instance == DBVcsInstance.id_,
+        DBVcsInstance.id_ == vcs_instance_id,
+    ).delete(synchronize_session=False)
     db_connection.commit()
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/rule.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/rule.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# pylint:disable=not-callable
 # Standard Library
 import logging
 from typing import List
 
 # Third Party
 from sqlalchemy.orm import Session
 
 # First Party
-from resc_backend.db import model
-from resc_backend.resc_web_service.schema import rule_allow_list as rule_allow_list_schema
+from resc_backend.db.model import DBrule, DBruleAllowList, DBrulePack, DBscan
+from resc_backend.resc_web_service.schema import (
+    rule_allow_list as rule_allow_list_schema,
+)
 from resc_backend.resc_web_service.schema.rule import RuleCreate, RuleRead
 
 logger = logging.getLogger(__name__)
 
 
 def get_rules_by_scan_id(db_connection: Session, scan_id: int) -> List[RuleRead]:
     """
@@ -20,35 +21,37 @@
     :param db_connection:
         Session of the database connection
     :param scan_id:
         scan id for which rules need to be fetched
     :return: List[RuleRead]
         The output contains list of rules
     """
-    rule_query = db_connection.query(model.DBrule)
-    rule_query = rule_query.join(model.DBscan, model.DBscan.rule_pack == model.DBrule.rule_pack)
-    rule_query = rule_query.filter(model.DBscan.id_ == scan_id)
+    rule_query = db_connection.query(DBrule)
+    rule_query = rule_query.join(DBscan, DBscan.rule_pack == DBrule.rule_pack)
+    rule_query = rule_query.filter(DBscan.id_ == scan_id)
     rules: List[RuleRead] = rule_query.all()
     return rules
 
 
-def create_rule_allow_list(db_connection: Session, rule_allow_list: rule_allow_list_schema.RuleAllowList):
+def create_rule_allow_list(
+    db_connection: Session, rule_allow_list: rule_allow_list_schema.RuleAllowList
+):
     """
         Create rule allow list in database
     :param db_connection:
         Session of the database connection
     :param rule_allow_list:
         RuleAllowList object to be created
     """
-    db_rule_allow_list = model.rule_allow_list.DBruleAllowList(
+    db_rule_allow_list = DBruleAllowList(
         description=rule_allow_list.description,
         regexes=rule_allow_list.regexes,
         paths=rule_allow_list.paths,
         commits=rule_allow_list.commits,
-        stop_words=rule_allow_list.stop_words
+        stop_words=rule_allow_list.stop_words,
     )
     db_connection.add(db_rule_allow_list)
     db_connection.commit()
     db_connection.refresh(db_rule_allow_list)
     return db_rule_allow_list
 
 
@@ -56,81 +59,87 @@
     """
         Create rule in database
     :param db_connection:
         Session of the database connection
     :param rule:
         RuleCreate object to be created
     """
-    db_rule = model.rule.DBrule(
+    db_rule = DBrule(
         rule_name=rule.rule_name,
         description=rule.description,
         entropy=rule.entropy,
         secret_group=rule.secret_group,
         regex=rule.regex,
         path=rule.path,
         keywords=rule.keywords,
         rule_pack=rule.rule_pack,
         allow_list=rule.allow_list,
-
     )
     db_connection.add(db_rule)
     db_connection.commit()
     db_connection.refresh(db_rule)
     return db_rule
 
 
-def get_rules_by_rule_pack_version(db_connection: Session, rule_pack_version: str) -> List[str]:
+def get_rules_by_rule_pack_version(
+    db_connection: Session, rule_pack_version: str
+) -> List[str]:
     """
         Fetch rules by rule pack version
     :param db_connection:
         Session of the database connection
     :param rule_pack_version:
         rule pack version
     :return: List[str]
         The output contains list of strings of global allow list
     """
-    query = db_connection.query(
-        model.DBrule.id_,
-        model.DBrule.rule_pack,
-        model.DBrule.rule_name,
-        model.DBrule.entropy,
-        model.DBrule.secret_group,
-        model.DBrule.regex,
-        model.DBrule.path,
-        model.DBrule.keywords,
-        model.rule_allow_list.DBruleAllowList.description,
-        model.rule_allow_list.DBruleAllowList.regexes,
-        model.rule_allow_list.DBruleAllowList.paths,
-        model.rule_allow_list.DBruleAllowList.commits,
-        model.rule_allow_list.DBruleAllowList.stop_words) \
-        .join(model.rule_pack.DBrulePack,
-              model.rule_pack.DBrulePack.version == model.rule.DBrule.rule_pack) \
-        .join(model.rule_allow_list.DBruleAllowList,
-              model.rule_allow_list.DBruleAllowList.id_ == model.rule.DBrule.allow_list, isouter=True)
-    db_rules = query.filter(model.rule.DBrule.rule_pack == rule_pack_version).order_by(
-        model.rule.DBrule.id_).all()
+    query = (
+        db_connection.query(
+            DBrule.id_,
+            DBrule.rule_pack,
+            DBrule.rule_name,
+            DBrule.entropy,
+            DBrule.secret_group,
+            DBrule.regex,
+            DBrule.path,
+            DBrule.keywords,
+            DBruleAllowList.description,
+            DBruleAllowList.regexes,
+            DBruleAllowList.paths,
+            DBruleAllowList.commits,
+            DBruleAllowList.stop_words,
+        )
+        .join(DBrulePack, DBrulePack.version == DBrule.rule_pack)
+        .join(DBruleAllowList, DBruleAllowList.id_ == DBrule.allow_list, isouter=True)
+    )
+    db_rules = (
+        query.filter(DBrule.rule_pack == rule_pack_version).order_by(DBrule.id_).all()
+    )
     return db_rules
 
 
-def get_global_allow_list_by_rule_pack_version(db_connection: Session, rule_pack_version: str) -> List[str]:
+def get_global_allow_list_by_rule_pack_version(
+    db_connection: Session, rule_pack_version: str
+) -> List[str]:
     """
         Retrieve global allow list by rule pack version
     :param db_connection:
         Session of the database connection
     :param rule_pack_version:
         rule pack version
     :return: List[str]
         The output contains list of strings of global allow list
     """
     query = db_connection.query(
-        model.rule_pack.DBrulePack.version,
-        model.rule_allow_list.DBruleAllowList.description,
-        model.rule_allow_list.DBruleAllowList.regexes,
-        model.rule_allow_list.DBruleAllowList.paths,
-        model.rule_allow_list.DBruleAllowList.commits,
-        model.rule_allow_list.DBruleAllowList.stop_words) \
-        .join(model.rule_allow_list.DBruleAllowList,
-              model.rule_allow_list.DBruleAllowList.id_ == model.rule_pack.DBrulePack.global_allow_list)
-    db_global_allow_list = query.filter(
-        model.rule_pack.DBrulePack.version == rule_pack_version).order_by(
-        model.rule_allow_list.DBruleAllowList.id_).first()
+        DBrulePack.version,
+        DBruleAllowList.description,
+        DBruleAllowList.regexes,
+        DBruleAllowList.paths,
+        DBruleAllowList.commits,
+        DBruleAllowList.stop_words,
+    ).join(DBruleAllowList, DBruleAllowList.id_ == DBrulePack.global_allow_list)
+    db_global_allow_list = (
+        query.filter(DBrulePack.version == rule_pack_version)
+        .order_by(DBruleAllowList.id_)
+        .first()
+    )
     return db_global_allow_list
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/rule_pack.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/rule_pack.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# pylint:disable=not-callable
 # Standard Library
 import logging
 from typing import List, Optional
 
 # Third Party
 from packaging.version import Version
 from sqlalchemy import and_, func, update
 from sqlalchemy.orm import Session
 from sqlalchemy.sql.expression import true
 
 # First Party
-from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
-from resc_backend.db import model
+from resc_backend.constants import (
+    DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    MAX_RECORDS_PER_PAGE_LIMIT,
+)
+from resc_backend.db.model import DBrule, DBrulePack, DBruleTag, DBtag
 from resc_backend.resc_web_service.schema import rule_pack as rule_pack_schema
 
 logger = logging.getLogger(__name__)
 
 
 def get_rule_pack(
     db_connection: Session, version: Optional[str]
@@ -25,35 +27,35 @@
     :param db_connection:
         Session of the database connection
     :param version:
         optional, version of the rule pack to be fetched else latest rule pack version will be fetched
     :return: RulePackRead
         The output returns RulePackRead type object
     """
-    query = db_connection.query(model.rule_pack.DBrulePack)
+    query = db_connection.query(DBrulePack)
     if version:
-        query = query.filter(model.rule_pack.DBrulePack.version == version)
+        query = query.filter(DBrulePack.version == version)
     else:
         logger.debug("rule pack version not specified, fetching currently active one")
-        query = query.filter(model.rule_pack.DBrulePack.active == true())
+        query = query.filter(DBrulePack.active == true())
     rule_pack = query.first()
     return rule_pack
 
 
 def create_rule_pack_version(
     db_connection: Session, rule_pack: rule_pack_schema.RulePackCreate
 ):
     """
         Create rule pack version in database
     :param db_connection:
         Session of the database connection
     :param rule_pack:
         RulePackCreate object to be created
     """
-    db_rule_pack = model.rule_pack.DBrulePack(
+    db_rule_pack = DBrulePack(
         version=rule_pack.version,
         global_allow_list=rule_pack.global_allow_list,
         active=rule_pack.active,
     )
     db_connection.add(db_rule_pack)
     db_connection.commit()
     db_connection.refresh(db_rule_pack)
@@ -64,15 +66,15 @@
     """
         Fetch the newest rule pack from database
     :param db_connection:
         Session of the database connection
     :return: RulePackRead
         The output returns RulePackRead type object
     """
-    rule_packs = db_connection.query(model.DBrulePack).all()
+    rule_packs = db_connection.query(DBrulePack).all()
     newest_rule_pack = None
     if rule_packs:
         newest_rule_pack: rule_pack_schema.RulePackRead = rule_packs[0]
         for rule_pack in rule_packs[1:]:
             if Version(rule_pack.version) > Version(newest_rule_pack.version):
                 newest_rule_pack = rule_pack
     return newest_rule_pack
@@ -80,15 +82,15 @@
 
 def get_rule_packs(
     db_connection: Session,
     version: str = None,
     active: bool = None,
     skip: int = 0,
     limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
-) -> List[model.rule_pack.DBrulePack]:
+) -> List[DBrulePack]:
     """
         Retrieve rule packs from database
     :param db_connection:
         Session of the database connection
     :param version:
         optional, filter on rule pack version
     :param active:
@@ -100,66 +102,63 @@
     :return: [RulePackRead]
         The output will contain a PaginationModel containing the list of RulePackRead type objects,
         or an empty list if no rule pack was found
     """
     limit_val = (
         MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
     )
-    query = db_connection.query(model.rule_pack.DBrulePack)
+    query = db_connection.query(DBrulePack)
 
     if version:
-        query = query.filter(model.rule_pack.DBrulePack.version == version)
+        query = query.filter(DBrulePack.version == version)
     if active is not None:
-        query = query.filter(model.rule_pack.DBrulePack.active == active)
+        query = query.filter(DBrulePack.active == active)
     rule_packs = (
-        query.order_by(model.rule_pack.DBrulePack.version.desc())
-        .offset(skip)
-        .limit(limit_val)
-        .all()
+        query.order_by(DBrulePack.version.desc()).offset(skip).limit(limit_val).all()
     )
     return rule_packs
 
 
 def get_current_active_rule_pack(
     db_connection: Session,
-) -> Optional[model.rule_pack.DBrulePack]:
+) -> Optional[DBrulePack]:
     """
         Return the currently active rule_pack, if any.
     :param db_connection:
         Session of the database connection
     :return: DBRulePack
         returns the DBRulePack containing the active rule pack
     """
-    query = db_connection.query(model.rule_pack.DBrulePack)
-    active_rule_pack = query.filter(model.rule_pack.DBrulePack.active == 1).one()
+    query = db_connection.query(DBrulePack)
+    active_rule_pack = query.filter(DBrulePack.active == 1).one()
     return active_rule_pack
 
 
 def get_rule_packs_tags(db_connection: Session, versions: list) -> List[str]:
     """
         Retrieve rule packs tags for versions from database
     :param db_connection:
         Session of the database connection
     :param versions:
         optional, filter on rule pack version
     :return: [str]
         The output will contain the list of str that are the tags, or an empty list.
     """
 
-    query = db_connection.query(model.DBtag.name)
-    query = query.join(model.DBruleTag, model.DBruleTag.tag_id == model.DBtag.id_)
+    query = db_connection.query(DBtag.name)
+    query = query.join(DBruleTag, DBruleTag.tag_id == DBtag.id_)
     query = query.join(
-        model.DBrule,
+        DBrule,
         and_(
-            model.DBrule.id_ == model.DBruleTag.rule_id,
-            model.DBrule.rule_pack.in_(versions),
+            DBrule.id_ == DBruleTag.rule_id,
+            DBrule.rule_pack.in_(versions),
         ),
     )
     rule_packs_tags = query.distinct().all()
-    rule_packs_tags = [t for t, in rule_packs_tags]
+    rule_packs_tags = [t for (t,) in rule_packs_tags]
     return rule_packs_tags
 
 
 def get_total_rule_packs_count(
     db_connection: Session, version: str = None, active: bool = None
 ) -> int:
     """
@@ -169,25 +168,19 @@
     :param version:
         optional, filter on rule pack version
     :param active:
         optional, filter on active rule pack
     :return: int
         The output contains total count of rule packs
     """
-    total_count_query = db_connection.query(
-        func.count(model.rule_pack.DBrulePack.version)
-    )
+    total_count_query = db_connection.query(func.count(DBrulePack.version))
     if version:
-        total_count_query = total_count_query.filter(
-            model.rule_pack.DBrulePack.version == version
-        )
+        total_count_query = total_count_query.filter(DBrulePack.version == version)
     if active is not None:
-        total_count_query = total_count_query.filter(
-            model.rule_pack.DBrulePack.active == active
-        )
+        total_count_query = total_count_query.filter(DBrulePack.active == active)
 
     total_count = total_count_query.scalar()
     return total_count
 
 
 def make_older_rule_packs_to_inactive(
     latest_rule_pack_version: str, db_connection: Session
@@ -196,12 +189,12 @@
         Make older rule packs to inactive
     :param latest_rule_pack_version:
         latest rule pack version
     :param db_connection:
         Session of the database connection
     """
     db_connection.execute(
-        update(model.rule_pack.DBrulePack)
-        .where(model.rule_pack.DBrulePack.version != latest_rule_pack_version)
+        update(DBrulePack)
+        .where(DBrulePack.version != latest_rule_pack_version)
         .values(active=False)
     )
     db_connection.commit()
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/scan.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/scan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,238 +1,280 @@
-# pylint: disable=E1101,not-callable
 # Standard Library
 from datetime import datetime
 from typing import List
 
 # Third Party
 from sqlalchemy import and_, func
 from sqlalchemy.orm import Session
 
 # First Party
-from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
-from resc_backend.db import model
+from resc_backend.constants import (
+    DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    MAX_RECORDS_PER_PAGE_LIMIT,
+)
+from resc_backend.db.model import (
+    DBfinding,
+    DBrepository,
+    DBscan,
+    DBscanFinding,
+    DBVcsInstance,
+)
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.schema import scan as scan_schema
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 
 
-def get_scan(db_connection: Session, scan_id: int) -> model.DBscan:
-    scan = db_connection.query(model.DBscan).filter(model.scan.DBscan.id_ == scan_id).first()
+def get_scan(db_connection: Session, scan_id: int) -> DBscan:
+    scan = db_connection.query(DBscan).filter(DBscan.id_ == scan_id).first()
     return scan
 
 
-def get_latest_scan_for_repository(db_connection: Session, repository_id: int) -> model.DBscan:
+def get_latest_scan_for_repository(
+    db_connection: Session, repository_id: int
+) -> DBscan:
     """
         Retrieve the most recent scan of a given repository object
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository object for which to retrieve the most recent scan
     :return: scan
         scan object having the most recent timestamp for a given repository object
     """
-    subquery = (db_connection.query(func.max(model.DBscan.timestamp).label("max_time"))
-                .filter(model.scan.DBscan.repository_id == repository_id)).subquery()
-
-    scan = db_connection.query(model.DBscan) \
-        .join(subquery,
-              and_(model.DBscan.timestamp == subquery.c.max_time)) \
-        .filter(model.scan.DBscan.repository_id == repository_id).first()
+    subquery = (
+        db_connection.query(func.max(DBscan.timestamp).label("max_time")).filter(
+            DBscan.repository_id == repository_id
+        )
+    ).subquery()
+
+    scan = (
+        db_connection.query(DBscan)
+        .join(subquery, and_(DBscan.timestamp == subquery.c.max_time))
+        .filter(DBscan.repository_id == repository_id)
+        .first()
+    )
 
     return scan
 
 
-def get_scans(db_connection: Session, skip: int = 0,
-              limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT, repository_id: int = -1) -> List[model.DBscan]:
+def get_scans(
+    db_connection: Session,
+    skip: int = 0,
+    limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    repository_id: int = -1,
+) -> List[DBscan]:
     """
         Retrieve the scan records, ordered by scan_id and optionally filtered by repository_id
     :param db_connection:
         Session of the database connection
     :param repository_id:
         optional int filtering the repository for which to retrieve scans
     :param skip:
         integer amount of records to skip to support pagination
     :param limit:
         integer amount of records to return, to support pagination
     :return: [DBscan]
         List of DBScan objects
     """
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
-    query = db_connection.query(model.DBscan)
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
+    query = db_connection.query(DBscan)
 
     if repository_id > 0:
-        query = query.filter(model.DBscan.repository_id == repository_id)
+        query = query.filter(DBscan.repository_id == repository_id)
 
-    scans = query.order_by(model.scan.DBscan.id_).offset(skip).limit(limit_val).all()
+    scans = query.order_by(DBscan.id_).offset(skip).limit(limit_val).all()
     return scans
 
 
 def get_scans_count(db_connection: Session, repository_id: int = -1) -> int:
     """
         Retrieve count of scan records optionally filtered by VCS provider
     :param db_connection:
         Session of the database connection
     :param repository_id:
         optional int filtering the repository for which to retrieve scans
     :return: total_count
         count of scans
     """
-    query = db_connection.query(func.count(model.DBscan.id_))
+    query = db_connection.query(func.count(DBscan.id_))
 
     if repository_id > 0:
-        query = query.filter(model.DBscan.repository_id == repository_id)
+        query = query.filter(DBscan.repository_id == repository_id)
 
     total_count = query.scalar()
     return total_count
 
 
-def update_scan(db_connection: Session, scan_id: int, scan: scan_schema.ScanCreate) -> model.DBscan:
-    db_scan = db_connection.query(model.DBscan).filter_by(id_=scan_id).first()
+def update_scan(
+    db_connection: Session, scan_id: int, scan: scan_schema.ScanCreate
+) -> DBscan:
+    db_scan = db_connection.query(DBscan).filter_by(id_=scan_id).first()
     db_scan.scan_type = scan.scan_type
     db_scan.last_scanned_commit = scan.last_scanned_commit
     db_scan.timestamp = scan.timestamp
     db_scan.increment_number = scan.increment_number
     db_scan.rule_pack = scan.rule_pack
     db_connection.commit()
     db_connection.refresh(db_scan)
     return db_scan
 
 
-def create_scan(db_connection: Session, scan: scan_schema.ScanCreate) -> model.DBscan:
-    db_scan = model.scan.DBscan(
+def create_scan(db_connection: Session, scan: scan_schema.ScanCreate) -> DBscan:
+    db_scan = DBscan(
         scan_type=scan.scan_type,
         last_scanned_commit=scan.last_scanned_commit,
         repository_id=scan.repository_id,
         timestamp=scan.timestamp,
         increment_number=scan.increment_number,
-        rule_pack=scan.rule_pack
+        rule_pack=scan.rule_pack,
     )
     db_connection.add(db_scan)
     db_connection.commit()
     db_connection.refresh(db_scan)
     return db_scan
 
 
-def get_repository_findings_metadata_for_latest_scan(db_connection: Session, repository_id: int,
-                                                     scan_timestamp: datetime):
+def get_repository_findings_metadata_for_latest_scan(
+    db_connection: Session, repository_id: int, scan_timestamp: datetime
+):
     """
         Retrieves the finding metadata for latest scan of a repository from the database
     :param db_connection:
         Session of the database connection
     :param repository_id:
         repository id of the latest scan
     :param scan_timestamp:
         timestamp of the latest scan
     :return: findings_metadata
         findings_metadata containing the count for each status
     """
     scan_ids_latest_to_base = []
-    scans = get_scans(db_connection=db_connection,
-                      repository_id=repository_id, limit=1000000)
+    scans = get_scans(
+        db_connection=db_connection, repository_id=repository_id, limit=1000000
+    )
     scans.sort(key=lambda x: x.timestamp, reverse=True)
     for scan in scans:
         if scan.timestamp <= scan_timestamp:
             scan_ids_latest_to_base.append(scan.id_)
             if scan.scan_type == ScanType.BASE:
                 break
 
-    true_positive_count = false_positive_count = not_analyzed_count = \
-        under_review_count = clarification_required_count = 0
+    true_positive_count = false_positive_count = not_analyzed_count = (
+        under_review_count
+    ) = clarification_required_count = 0
     if len(scan_ids_latest_to_base) > 0:
         findings_count_by_status = finding_crud.get_findings_count_by_status(
-            db_connection, scan_ids=scan_ids_latest_to_base, finding_statuses=FindingStatus)
+            db_connection,
+            scan_ids=scan_ids_latest_to_base,
+            finding_statuses=FindingStatus,
+        )
         for finding in findings_count_by_status:
             finding_status = finding[1]
             count = finding[0]
             if finding_status == FindingStatus.TRUE_POSITIVE:
                 true_positive_count = count
             if finding_status == FindingStatus.FALSE_POSITIVE:
                 false_positive_count = count
             if finding_status == FindingStatus.NOT_ANALYZED or finding_status is None:
                 not_analyzed_count += count
             if finding_status == FindingStatus.UNDER_REVIEW:
                 under_review_count = count
             if finding_status == FindingStatus.CLARIFICATION_REQUIRED:
                 clarification_required_count = count
 
-    total_findings_count = \
-        true_positive_count + false_positive_count + not_analyzed_count + under_review_count + \
-        clarification_required_count
+    total_findings_count = (
+        true_positive_count
+        + false_positive_count
+        + not_analyzed_count
+        + under_review_count
+        + clarification_required_count
+    )
 
     findings_metadata = {
         "true_positive": true_positive_count,
         "false_positive": false_positive_count,
         "not_analyzed": not_analyzed_count,
         "under_review": under_review_count,
         "clarification_required": clarification_required_count,
-        "total_findings_count": total_findings_count
+        "total_findings_count": total_findings_count,
     }
 
     return findings_metadata
 
 
-def delete_repository_findings_not_linked_to_any_scan(db_connection: Session, repository_id: int):
+def delete_repository_findings_not_linked_to_any_scan(
+    db_connection: Session, repository_id: int
+):
     """
         Delete findings for a given repository which are not linked to any scans
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository
     """
-    sub_query = db_connection.query(model.DBscanFinding.finding_id).distinct()
-    db_connection.query(model.DBfinding) \
-        .filter(model.finding.DBfinding.id_.not_in(sub_query), model.finding.DBfinding.repository_id == repository_id) \
-        .delete(synchronize_session=False)
+    sub_query = db_connection.query(DBscanFinding.finding_id).distinct()
+    db_connection.query(DBfinding).filter(
+        DBfinding.id_.not_in(sub_query), DBfinding.repository_id == repository_id
+    ).delete(synchronize_session=False)
     db_connection.commit()
 
 
-def delete_scan(db_connection: Session, repository_id: int, scan_id: int, delete_related: bool = False):
+def delete_scan(
+    db_connection: Session,
+    repository_id: int,
+    scan_id: int,
+    delete_related: bool = False,
+):
     """
         Delete a scan object
     :param db_connection:
         Session of the database connection
     :param repository_id:
         repository_id for which findings will be deleted which are not linked to any scans
     :param scan_id:
         id of the scan to be deleted
     :param delete_related:
         if related records need to be deleted
     """
     if delete_related:
         scan_finding_crud.delete_scan_finding(db_connection, scan_id=scan_id)
-    db_connection.query(model.DBscan) \
-        .filter(model.scan.DBscan.id_ == scan_id) \
-        .delete(synchronize_session=False)
+    db_connection.query(DBscan).filter(DBscan.id_ == scan_id).delete(
+        synchronize_session=False
+    )
     db_connection.commit()
-    delete_repository_findings_not_linked_to_any_scan(db_connection, repository_id=repository_id)
+    delete_repository_findings_not_linked_to_any_scan(
+        db_connection, repository_id=repository_id
+    )
 
 
 def delete_scans_by_repository_id(db_connection: Session, repository_id: int):
     """
         Delete scans for a given repository
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository
     """
-    db_connection.query(model.DBscan) \
-        .filter(model.scan.DBscan.repository_id == repository_id) \
-        .delete(synchronize_session=False)
+    db_connection.query(DBscan).filter(DBscan.repository_id == repository_id).delete(
+        synchronize_session=False
+    )
     db_connection.commit()
 
 
 def delete_scans_by_vcs_instance_id(db_connection: Session, vcs_instance_id: int):
     """
         Delete scans for a given vcs instance
     :param db_connection:
         Session of the database connection
     :param vcs_instance_id:
         id of the vcs instance
     """
-    db_connection.query(model.DBscan) \
-        .filter(model.scan.DBscan.repository_id == model.repository.DBrepository.id_,
-                model.repository.DBrepository.vcs_instance == model.vcs_instance.DBVcsInstance.id_,
-                model.vcs_instance.DBVcsInstance.id_ == vcs_instance_id) \
-        .delete(synchronize_session=False)
+    db_connection.query(DBscan).filter(
+        DBscan.repository_id == DBrepository.id_,
+        DBrepository.vcs_instance == DBVcsInstance.id_,
+        DBVcsInstance.id_ == vcs_instance_id,
+    ).delete(synchronize_session=False)
     db_connection.commit()
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/crud/vcs_instance.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/crud/vcs_instance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,44 @@
-# pylint: disable=E1101,not-callable
 # Standard Library
 from typing import List
 
 # Third Party
 from sqlalchemy import func
 from sqlalchemy.orm import Session
 
 # First Party
-from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
-from resc_backend.db import model
+from resc_backend.constants import (
+    DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    MAX_RECORDS_PER_PAGE_LIMIT,
+)
+from resc_backend.db.model import DBVcsInstance
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.crud import repository as repository_crud
 from resc_backend.resc_web_service.crud import scan as scan_crud
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.schema import vcs_instance as vcs_instance_schema
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 
 def get_vcs_instance(db_connection: Session, vcs_instance_id: int):
-    vcs_instance = db_connection.query(
-        model.DBVcsInstance).filter(model.vcs_instance.DBVcsInstance.id_ == vcs_instance_id).first()
+    vcs_instance = (
+        db_connection.query(DBVcsInstance)
+        .filter(DBVcsInstance.id_ == vcs_instance_id)
+        .first()
+    )
     return vcs_instance
 
 
-def get_vcs_instances(db_connection: Session, skip: int = 0, limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
-                      vcs_provider_type: VCSProviders = None, vcs_instance_name: str = None) \
-        -> List[model.DBVcsInstance]:
+def get_vcs_instances(
+    db_connection: Session,
+    skip: int = 0,
+    limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    vcs_provider_type: VCSProviders = None,
+    vcs_instance_name: str = None,
+) -> List[DBVcsInstance]:
     """
         Retrieve all vcs_instances records
     :param db_connection:
         Session of the database connection
     :param vcs_provider_type:
         optional filtering by VCS Provider type
     :param vcs_instance_name:
@@ -37,116 +46,145 @@
     :param skip:
         integer amount of records to skip to support pagination
     :param limit:
         integer amount of records to return, to support pagination
     :return: [DBVcsInstance]
         List of DBVcsInstance objects
     """
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
-    query = db_connection.query(model.DBVcsInstance)
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
+    query = db_connection.query(DBVcsInstance)
 
     if vcs_provider_type:
-        query = query.filter(model.DBVcsInstance.provider_type == vcs_provider_type)
+        query = query.filter(DBVcsInstance.provider_type == vcs_provider_type)
 
     if vcs_instance_name:
-        query = query.filter(model.DBVcsInstance.name == vcs_instance_name)
+        query = query.filter(DBVcsInstance.name == vcs_instance_name)
 
-    vcs_instances = query.order_by(model.vcs_instance.DBVcsInstance.id_).offset(skip).limit(limit_val).all()
+    vcs_instances = (
+        query.order_by(DBVcsInstance.id_).offset(skip).limit(limit_val).all()
+    )
     return vcs_instances
 
 
-def get_vcs_instances_count(db_connection: Session,
-                            vcs_provider_type: VCSProviders = None, vcs_instance_name: str = None) -> int:
+def get_vcs_instances_count(
+    db_connection: Session,
+    vcs_provider_type: VCSProviders = None,
+    vcs_instance_name: str = None,
+) -> int:
     """
         Retrieve count of vcs_instances records optionally filtered by VCS provider
     :param db_connection:
         Session of the database connection
     :param vcs_provider_type:
         optional vcs_provider_type filtering the vcs provider type for which to count vcs instances
     :param vcs_instance_name:
         optional vcs_instance_name filtering the vcs provider name for which to count vcs instances
     :return: total_count
         count of vcs instances
     """
-    query = db_connection.query(func.count(model.DBVcsInstance.id_))
+    query = db_connection.query(func.count(DBVcsInstance.id_))
 
     if vcs_provider_type:
-        query = query.filter(model.DBVcsInstance.provider_type == vcs_provider_type)
+        query = query.filter(DBVcsInstance.provider_type == vcs_provider_type)
 
     if vcs_instance_name:
-        query = query.filter(model.DBVcsInstance.name == vcs_instance_name)
+        query = query.filter(DBVcsInstance.name == vcs_instance_name)
 
     total_count = query.scalar()
     return total_count
 
 
 def update_vcs_instance(
-        db_connection: Session,
-        vcs_instance_id: int,
-        vcs_instance: vcs_instance_schema.VCSInstanceCreate) -> model.DBVcsInstance:
-    db_vcs_instance: model.DBVcsInstance = \
-        db_connection.query(model.DBVcsInstance).filter_by(id_=vcs_instance_id).first()
+    db_connection: Session,
+    vcs_instance_id: int,
+    vcs_instance: vcs_instance_schema.VCSInstanceCreate,
+) -> DBVcsInstance:
+    db_vcs_instance: DBVcsInstance = (
+        db_connection.query(DBVcsInstance).filter_by(id_=vcs_instance_id).first()
+    )
     db_vcs_instance.name = vcs_instance.name
     db_vcs_instance.provider_type = vcs_instance.provider_type
     db_vcs_instance.port = vcs_instance.port
     db_vcs_instance.scheme = vcs_instance.scheme
     db_vcs_instance.organization = vcs_instance.organization
     db_vcs_instance.hostname = vcs_instance.hostname
     db_vcs_instance.scope = ",".join(vcs_instance.scope)
     db_vcs_instance.exceptions = ",".join(vcs_instance.exceptions)
 
     db_connection.commit()
     db_connection.refresh(db_vcs_instance)
     return db_vcs_instance
 
 
-def create_vcs_instance(db_connection: Session, vcs_instance: vcs_instance_schema.VCSInstanceCreate) \
-        -> model.DBVcsInstance:
-    db_vcs_instance = model.vcs_instance.DBVcsInstance(
+def create_vcs_instance(
+    db_connection: Session, vcs_instance: vcs_instance_schema.VCSInstanceCreate
+) -> DBVcsInstance:
+    db_vcs_instance = DBVcsInstance(
         name=vcs_instance.name,
         provider_type=vcs_instance.provider_type,
         port=vcs_instance.port,
         scheme=vcs_instance.scheme,
         organization=vcs_instance.organization,
         hostname=vcs_instance.hostname,
         scope=",".join(vcs_instance.scope),
-        exceptions=",".join(vcs_instance.exceptions)
+        exceptions=",".join(vcs_instance.exceptions),
     )
     db_connection.add(db_vcs_instance)
     db_connection.commit()
     db_connection.refresh(db_vcs_instance)
     return db_vcs_instance
 
 
-def create_vcs_instance_if_not_exists(db_connection: Session, vcs_instance: vcs_instance_schema.VCSInstanceCreate):
+def create_vcs_instance_if_not_exists(
+    db_connection: Session, vcs_instance: vcs_instance_schema.VCSInstanceCreate
+):
     # Query the database to see if the vcs_instance object exists based on the unique constraint parameters
-    db_select_vcs_instance = db_connection.query(model.DBVcsInstance) \
-        .filter(model.DBVcsInstance.provider_type == vcs_instance.provider_type,
-                model.DBVcsInstance.scheme == vcs_instance.scheme,
-                model.DBVcsInstance.hostname == vcs_instance.hostname,
-                model.DBVcsInstance.port == vcs_instance.port,
-                model.DBVcsInstance.organization == vcs_instance.organization).first()
+    db_select_vcs_instance = (
+        db_connection.query(DBVcsInstance)
+        .filter(
+            DBVcsInstance.provider_type == vcs_instance.provider_type,
+            DBVcsInstance.scheme == vcs_instance.scheme,
+            DBVcsInstance.hostname == vcs_instance.hostname,
+            DBVcsInstance.port == vcs_instance.port,
+            DBVcsInstance.organization == vcs_instance.organization,
+        )
+        .first()
+    )
     if db_select_vcs_instance is not None:
         return db_select_vcs_instance
 
     # Create non-existing vcs_instance object
     return create_vcs_instance(db_connection, vcs_instance)
 
 
-def delete_vcs_instance(db_connection: Session, vcs_instance_id: int, delete_related: bool = False):
+def delete_vcs_instance(
+    db_connection: Session, vcs_instance_id: int, delete_related: bool = False
+):
     """
         Delete a vcs instance object
     :param db_connection:
         Session of the database connection
     :param vcs_instance_id:
         id of the vcs instance to be deleted
     :param delete_related:
         if related records need to be deleted
     """
     if delete_related:
-        scan_finding_crud.delete_scan_finding_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
-        finding_crud.delete_findings_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
-        scan_crud.delete_scans_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
-        repository_crud.delete_repositories_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
-    db_vcs_instance = db_connection.query(model.DBVcsInstance).filter_by(id_=vcs_instance_id).first()
+        scan_finding_crud.delete_scan_finding_by_vcs_instance_id(
+            db_connection, vcs_instance_id=vcs_instance_id
+        )
+        finding_crud.delete_findings_by_vcs_instance_id(
+            db_connection, vcs_instance_id=vcs_instance_id
+        )
+        scan_crud.delete_scans_by_vcs_instance_id(
+            db_connection, vcs_instance_id=vcs_instance_id
+        )
+        repository_crud.delete_repositories_by_vcs_instance_id(
+            db_connection, vcs_instance_id=vcs_instance_id
+        )
+    db_vcs_instance = (
+        db_connection.query(DBVcsInstance).filter_by(id_=vcs_instance_id).first()
+    )
     db_connection.delete(db_vcs_instance)
     db_connection.commit()
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/dependencies.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/dependencies.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,132 +17,164 @@
     CONTENT_SECURITY_POLICY,
     CROSS_ORIGIN_RESOURCE_POLICY,
     REFERRER_POLICY,
     STRICT_TRANSPORT_SECURITY,
     X_CONTENT_TYPE_OPTIONS,
     X_FRAME_OPTIONS,
     X_PERMITTED_CROSS_DOMAIN_POLICIES,
-    X_XSS_PROTECTION
+    X_XSS_PROTECTION,
 )
 from resc_backend.db.connection import Session, engine
 from resc_backend.db.model import DBfinding, DBrepository, DBrule, DBscan, DBscanFinding
 from resc_backend.helpers.environment_wrapper import validate_environment
 from resc_backend.resc_web_service.configuration import (
     CONDITIONAL_SSO_ENV_VARS,
     SSO_ACCESS_TOKEN_ISSUER_URL,
     SSO_ACCESS_TOKEN_JWKS_URL,
     SSO_JWT_CLAIM_KEY_AUTHORIZATION,
     SSO_JWT_CLAIM_KEY_USER_ID,
     SSO_JWT_CLAIM_VALUE_AUTHORIZATION,
     SSO_JWT_REQUIRED_CLAIMS,
-    SSO_JWT_SIGN_ALGORITHM
+    SSO_JWT_SIGN_ALGORITHM,
 )
 
 security = HTTPBearer()
 logger = logging.getLogger(__name__)
 
 
-async def requires_auth(request: Request, credentials: HTTPBasicCredentials = Depends(security)):
+async def requires_auth(
+    request: Request, credentials: HTTPBasicCredentials = Depends(security)
+):
     """
-        Function that is used to validate the JWT access token
+    Function that is used to validate the JWT access token
     """
     # Check and load environment variables
     env_variables = validate_environment(CONDITIONAL_SSO_ENV_VARS)
 
     access_token = credentials.credentials
     algorithm = [env_variables[SSO_JWT_SIGN_ALGORITHM]]
     issuer = env_variables[SSO_ACCESS_TOKEN_ISSUER_URL]
     jwks_url = env_variables[SSO_ACCESS_TOKEN_JWKS_URL]
     jwt_options = {
-        "verify_signature": True, "verify_iss": True, "verify_exp": True,
-        "require": env_variables[SSO_JWT_REQUIRED_CLAIMS].split(",")
+        "verify_signature": True,
+        "verify_iss": True,
+        "verify_exp": True,
+        "require": env_variables[SSO_JWT_REQUIRED_CLAIMS].split(","),
     }
     try:
-        ssl._create_default_https_context = ssl._create_unverified_context  # pylint: disable=W0212
+        ssl._create_default_https_context = ssl._create_unverified_context
         jwks_client = PyJWKClient(jwks_url)
         signing_key = jwks_client.get_signing_key_from_jwt(access_token)
         claims = jwt.decode(
             access_token,
             signing_key.key,
             algorithms=algorithm,
             issuer=issuer,
             options=jwt_options,
         )
         user_id = claims[env_variables[SSO_JWT_CLAIM_KEY_USER_ID]]
         if not user_is_authorized(claims, env_variables):
             logger.error(f"Invalid login attempt for user {user_id}")
-            raise HTTPException(status_code=status.HTTP_403_FORBIDDEN,
-                                detail="You don't have permission to access this resource.")
+            raise HTTPException(
+                status_code=status.HTTP_403_FORBIDDEN,
+                detail="You don't have permission to access this resource.",
+            )
         request.scope["user"] = user_id
     except urllib.error.URLError as error:
-        logger.error(f"Unable to contact server for token validation {jwks_url} Message: {error}")
-        raise HTTPException(status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
-                            detail="Unable to contact server for token validation") from error
+        logger.error(
+            f"Unable to contact server for token validation {jwks_url} Message: {error}"
+        )
+        raise HTTPException(
+            status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
+            detail="Unable to contact server for token validation",
+        ) from error
 
     except jwt.InvalidAlgorithmError as error:
-        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="Algorithm is invalid for decoding token",
-                            headers={"WWW-Authenticate": "Bearer"}) from error
+        raise HTTPException(
+            status_code=status.HTTP_401_UNAUTHORIZED,
+            detail="Algorithm is invalid for decoding token",
+            headers={"WWW-Authenticate": "Bearer"},
+        ) from error
     except jwt.PyJWKClientError as error:
-        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="Unable to find the signing key",
-                            headers={"WWW-Authenticate": "Bearer"}) from error
+        raise HTTPException(
+            status_code=status.HTTP_401_UNAUTHORIZED,
+            detail="Unable to find the signing key",
+            headers={"WWW-Authenticate": "Bearer"},
+        ) from error
     except jwt.InvalidKeyError as error:
-        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="JWKS key is not in the proper format",
-                            headers={"WWW-Authenticate": "Bearer"}) from error
+        raise HTTPException(
+            status_code=status.HTTP_401_UNAUTHORIZED,
+            detail="JWKS key is not in the proper format",
+            headers={"WWW-Authenticate": "Bearer"},
+        ) from error
     except jwt.InvalidIssuerError as error:
-        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED,
-                            detail="Token's issuer claim does not match with the expected issuer",
-                            headers={"WWW-Authenticate": "Bearer"}) from error
+        raise HTTPException(
+            status_code=status.HTTP_401_UNAUTHORIZED,
+            detail="Token's issuer claim does not match with the expected issuer",
+            headers={"WWW-Authenticate": "Bearer"},
+        ) from error
     except jwt.ExpiredSignatureError as error:
-        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="Token has expired",
-                            headers={"WWW-Authenticate": "Bearer"}) from error
+        raise HTTPException(
+            status_code=status.HTTP_401_UNAUTHORIZED,
+            detail="Token has expired",
+            headers={"WWW-Authenticate": "Bearer"},
+        ) from error
     except jwt.InvalidSignatureError as error:
-        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="Token's signature did not match",
-                            headers={"WWW-Authenticate": "Bearer"}) from error
+        raise HTTPException(
+            status_code=status.HTTP_401_UNAUTHORIZED,
+            detail="Token's signature did not match",
+            headers={"WWW-Authenticate": "Bearer"},
+        ) from error
     except jwt.DecodeError as error:
-        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED,
-                            detail="Token can not be decoded because it failed validation",
-                            headers={"WWW-Authenticate": "Bearer"}) from error
+        raise HTTPException(
+            status_code=status.HTTP_401_UNAUTHORIZED,
+            detail="Token can not be decoded because it failed validation",
+            headers={"WWW-Authenticate": "Bearer"},
+        ) from error
     except jwt.InvalidTokenError as error:
-        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="Invalid token",
-                            headers={"WWW-Authenticate": "Bearer"}) from error
+        raise HTTPException(
+            status_code=status.HTTP_401_UNAUTHORIZED,
+            detail="Invalid token",
+            headers={"WWW-Authenticate": "Bearer"},
+        ) from error
 
 
 async def add_security_headers(request: Request, call_next):
     """
-        Function that is used to add several security headers to the API
+    Function that is used to add several security headers to the API
     """
     security_headers = {
         "Strict-Transport-Security": STRICT_TRANSPORT_SECURITY,
         "Cache-Control": CACHE_CONTROL,
         "Cross-Origin-Resource-Policy": CROSS_ORIGIN_RESOURCE_POLICY,
         "Referrer-Policy": REFERRER_POLICY,
         "X-Permitted-Cross-Domain-Policies": X_PERMITTED_CROSS_DOMAIN_POLICIES,
         "X-Content-Type-Options": X_CONTENT_TYPE_OPTIONS,
         "X-Frame-Options": X_FRAME_OPTIONS,
         "X-XSS-Protection": X_XSS_PROTECTION,
-        "Content-Security-Policy": CONTENT_SECURITY_POLICY
+        "Content-Security-Policy": CONTENT_SECURITY_POLICY,
     }
     response = await call_next(request)
     for header, value in security_headers.items():
         response.headers[header] = value
     return response
 
 
 def user_is_authorized(claims: dict, env_variables: dict) -> bool:
     """
-        Function that is used to determine if the user has the required claim and value to access the web service
+    Function that is used to determine if the user has the required claim and value to access the web service
     """
     claim_key = env_variables[SSO_JWT_CLAIM_KEY_AUTHORIZATION]
     claim_check_value = env_variables[SSO_JWT_CLAIM_VALUE_AUTHORIZATION]
     return bool(claim_key in claims and claim_check_value in claims[claim_key])
 
 
 def requires_no_auth(request: Request):
     """
-        Function that is used for unauthenticated access
+    Function that is used for unauthenticated access
     """
     request.scope["user"] = "Anonymous"
 
 
 def get_db_connection():
     db_connection = Session(bind=engine)
     try:
@@ -154,26 +186,28 @@
 @retry(wait=wait_exponential(multiplier=1, min=2, max=10), stop=stop_after_attempt(100))
 def check_db_initialized():
     required_table_names = [
         DBfinding.__tablename__,
         DBrepository.__tablename__,
         DBrule.__tablename__,
         DBscan.__tablename__,
-        DBscanFinding.__tablename__
+        DBscanFinding.__tablename__,
     ]
     try:
         # Create a sqlalchemy inspector, will cause an exception if the db connection can't be established
         inspector = sqlalchemy.inspect(engine)
 
         # Check existence of required tables
         not_found_tables = []
         for table_name in required_table_names:
             table_exists = inspector.has_table(table_name)
             if not table_exists:
                 not_found_tables.append(table_name)
 
         if len(not_found_tables) > 0:
-            raise RuntimeError(f"Unable to determine existence of required table(s) "
-                               f"{', '.join(not_found_tables)}")
+            raise RuntimeError(
+                f"Unable to determine existence of required table(s) "
+                f"{', '.join(not_found_tables)}"
+            )
     except Exception as ex:
         logger.error(f"Database is NOT connected or initialized | {ex} | Retrying...")
         raise
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/common.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,51 +9,55 @@
 from resc_backend.constants import (
     CACHE_NAMESPACE_VCS_INSTANCE,
     COMMON_TAG,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
     REDIS_CACHE_EXPIRE,
     RWS_ROUTE_AUTH_CHECK,
-    RWS_ROUTE_SUPPORTED_VCS_PROVIDERS
+    RWS_ROUTE_SUPPORTED_VCS_PROVIDERS,
 )
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 router = APIRouter(tags=[COMMON_TAG])
 
 
-@router.get(f"{RWS_ROUTE_SUPPORTED_VCS_PROVIDERS}",
-            response_model=List[str],
-            summary="Get supported vcs-providers",
-            description="Retrieve the supported vcs-providers, example: Bitbucket, AzureDevOps, Github etc",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve the supported vcs-providers"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_SUPPORTED_VCS_PROVIDERS}",
+    response_model=List[str],
+    summary="Get supported vcs-providers",
+    description="Retrieve the supported vcs-providers, example: Bitbucket, AzureDevOps, Github etc",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve the supported vcs-providers"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_VCS_INSTANCE, expire=REDIS_CACHE_EXPIRE)
 def get_supported_vcs_providers() -> List[str]:
     """
         Retrieve all supported vcs providers
     :return: List[str]
         The output will contain a list of strings of unique vcs providers
     """
     supported_vcs = [vcs for vcs in VCSProviders if vcs]
     return supported_vcs
 
 
-@router.get(f"{RWS_ROUTE_AUTH_CHECK}",
-            summary="Authorization check",
-            description="The output returns 200 OK if auth check is successful else returns 403 Forbidden",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Validate authorization check from the access-token"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_AUTH_CHECK}",
+    summary="Authorization check",
+    description="The output returns 200 OK if auth check is successful else returns 403 Forbidden",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Validate authorization check from the access-token"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 def auth_check():
     """
         Validates authorization check from the access token
     :return: str
         The output will contain 200 OK if auth check is successful else it will return 403 Forbidden
     """
     return {"message": "OK"}
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/detailed_findings.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,44 +11,48 @@
 from resc_backend.constants import (
     CACHE_NAMESPACE_FINDING,
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
     FINDINGS_TAG,
     REDIS_CACHE_EXPIRE,
-    RWS_ROUTE_DETAILED_FINDINGS
+    RWS_ROUTE_DETAILED_FINDINGS,
 )
 from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.crud import detailed_finding as detailed_finding_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.filters import FindingsFilter
 from resc_backend.resc_web_service.helpers.resc_swagger_models import Model404
-from resc_backend.resc_web_service.schema import detailed_finding as detailed_finding_schema
+from resc_backend.resc_web_service.schema import (
+    detailed_finding as detailed_finding_schema,
+)
 from resc_backend.resc_web_service.schema.pagination_model import PaginationModel
 
 router = APIRouter(prefix=f"{RWS_ROUTE_DETAILED_FINDINGS}", tags=[FINDINGS_TAG])
 logger = logging.getLogger(__name__)
 
 
-@router.get("",
-            response_model=PaginationModel[detailed_finding_schema.DetailedFindingRead],
-            summary="Get all detailed findings",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the findings"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    "",
+    response_model=PaginationModel[detailed_finding_schema.DetailedFindingRead],
+    summary="Get all detailed findings",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the findings"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
-def get_all_detailed_findings(skip: int = Query(default=0, ge=0),
-                              limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                              db_connection: Session = Depends(get_db_connection),
-                              query_string: str = None
-                              ) \
-        -> PaginationModel[detailed_finding_schema.DetailedFindingRead]:
+def get_all_detailed_findings(
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    db_connection: Session = Depends(get_db_connection),
+    query_string: str = None,
+) -> PaginationModel[detailed_finding_schema.DetailedFindingRead]:
     """
         Retrieve all findings objects paginated
     - **query_string**
 
         A query string with the following format:
             param1=value1&param2=value2&param3=value3
 
@@ -93,61 +97,76 @@
 
         The output will contain a PaginationModel containing the list of DetailedFinding type objects,
         or an empty list if no finding was found
     """
 
     parsed_query_string_params = dict(urllib.parse.parse_qsl(query_string))
 
-    if parsed_query_string_params.get('scan_ids'):
-        parsed_query_string_params['scan_ids'] = json.loads(parsed_query_string_params['scan_ids'])
-    if parsed_query_string_params.get('vcs_providers'):
-        parsed_query_string_params['vcs_providers'] = json.loads(parsed_query_string_params['vcs_providers']
-                                                                 .replace('\'', '"'))
-    if parsed_query_string_params.get('finding_statuses'):
-        parsed_query_string_params['finding_statuses'] = json.loads(parsed_query_string_params['finding_statuses']
-                                                                    .replace('\'', '"'))
-    if parsed_query_string_params.get('rule_names'):
-        parsed_query_string_params['rule_names'] = json.loads(parsed_query_string_params['rule_names']
-                                                              .replace('\'', '"'))
-    if parsed_query_string_params.get('rule_tags'):
-        parsed_query_string_params['rule_tags'] = json.loads(parsed_query_string_params['rule_tags']
-                                                             .replace('\'', '"'))
-    if parsed_query_string_params.get('rule_pack_versions'):
-        parsed_query_string_params['rule_pack_versions'] = json.loads(parsed_query_string_params['rule_pack_versions']
-                                                                      .replace('\'', '"'))
+    if parsed_query_string_params.get("scan_ids"):
+        parsed_query_string_params["scan_ids"] = json.loads(
+            parsed_query_string_params["scan_ids"]
+        )
+    if parsed_query_string_params.get("vcs_providers"):
+        parsed_query_string_params["vcs_providers"] = json.loads(
+            parsed_query_string_params["vcs_providers"].replace("'", '"')
+        )
+    if parsed_query_string_params.get("finding_statuses"):
+        parsed_query_string_params["finding_statuses"] = json.loads(
+            parsed_query_string_params["finding_statuses"].replace("'", '"')
+        )
+    if parsed_query_string_params.get("rule_names"):
+        parsed_query_string_params["rule_names"] = json.loads(
+            parsed_query_string_params["rule_names"].replace("'", '"')
+        )
+    if parsed_query_string_params.get("rule_tags"):
+        parsed_query_string_params["rule_tags"] = json.loads(
+            parsed_query_string_params["rule_tags"].replace("'", '"')
+        )
+    if parsed_query_string_params.get("rule_pack_versions"):
+        parsed_query_string_params["rule_pack_versions"] = json.loads(
+            parsed_query_string_params["rule_pack_versions"].replace("'", '"')
+        )
 
     findings_filter = FindingsFilter(**parsed_query_string_params)
 
     findings = detailed_finding_crud.get_detailed_findings(
-        db_connection, findings_filter=findings_filter, skip=skip, limit=limit)
+        db_connection, findings_filter=findings_filter, skip=skip, limit=limit
+    )
     total_findings = detailed_finding_crud.get_detailed_findings_count(
-        db_connection, findings_filter=findings_filter)
+        db_connection, findings_filter=findings_filter
+    )
 
     return PaginationModel[detailed_finding_schema.DetailedFindingRead](
-        data=findings, total=total_findings, limit=limit, skip=skip)
+        data=findings, total=total_findings, limit=limit, skip=skip
+    )
 
 
-@router.get("/{finding_id}",
-            response_model=detailed_finding_schema.DetailedFindingRead,
-            summary="Fetch detailed finding by ID",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve detailed finding <finding_id>"},
-                404: {"model": Model404, "description": "Finding <finding_id> not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    "/{finding_id}",
+    response_model=detailed_finding_schema.DetailedFindingRead,
+    summary="Fetch detailed finding by ID",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve detailed finding <finding_id>"},
+        404: {"model": Model404, "description": "Finding <finding_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
-def read_finding(finding_id: int, db_connection: Session = Depends(get_db_connection)) \
-        -> detailed_finding_schema.DetailedFindingRead:
+def read_finding(
+    finding_id: int, db_connection: Session = Depends(get_db_connection)
+) -> detailed_finding_schema.DetailedFindingRead:
     """
         Retrieve detailed finding by its ID
 
     - **db_connection**: Session of the database connection
     - **finding_id**: ID of the finding for which details need to be fetched
     - **return**: [DetailedFindingRead]
         The output will contain the details of a finding
     """
-    db_finding = detailed_finding_crud.get_detailed_finding(db_connection, finding_id=finding_id)
+    db_finding = detailed_finding_crud.get_detailed_finding(
+        db_connection, finding_id=finding_id
+    )
     if db_finding is None:
         raise HTTPException(status_code=404, detail="Finding not found")
     return db_finding
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/findings.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/findings.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     FINDINGS_TAG,
     REDIS_CACHE_EXPIRE,
     RWS_ROUTE_AUDIT,
     RWS_ROUTE_BY_RULE,
     RWS_ROUTE_COUNT_BY_TIME,
     RWS_ROUTE_FINDINGS,
     RWS_ROUTE_SUPPORTED_STATUSES,
-    RWS_ROUTE_TOTAL_COUNT_BY_RULE
+    RWS_ROUTE_TOTAL_COUNT_BY_RULE,
 )
 from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.cache_manager import CacheManager
 from resc_backend.resc_web_service.crud import audit as audit_crud
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
@@ -38,57 +38,66 @@
 from resc_backend.resc_web_service.schema.finding import FindingRead
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.pagination_model import PaginationModel
 
 router = APIRouter(prefix=f"{RWS_ROUTE_FINDINGS}", tags=[FINDINGS_TAG])
 
 
-@router.get("",
-            response_model=PaginationModel[finding_schema.FindingRead],
-            summary="Get findings",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the findings"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    "",
+    response_model=PaginationModel[finding_schema.FindingRead],
+    summary="Get findings",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the findings"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
-def get_all_findings(skip: int = Query(default=0, ge=0),
-                     limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                     db_connection: Session = Depends(get_db_connection)) \
-        -> PaginationModel[finding_schema.FindingRead]:
+def get_all_findings(
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[finding_schema.FindingRead]:
     """
         Retrieve all findings objects paginated
 
     - **db_connection**: Session of the database connection
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **return**: [FindingRead]
         The output will contain a PaginationModel containing the list of FindingRead type objects,
         or an empty list if no finding was found
     """
     findings = finding_crud.get_findings(db_connection, skip=skip, limit=limit)
 
     total_findings = finding_crud.get_total_findings_count(db_connection)
 
-    return PaginationModel[finding_schema.FindingRead](data=findings, total=total_findings, limit=limit, skip=skip)
+    return PaginationModel[finding_schema.FindingRead](
+        data=findings, total=total_findings, limit=limit, skip=skip
+    )
 
 
-@router.post("",
-             response_model=int,
-             summary="Create a finding",
-             status_code=status.HTTP_201_CREATED,
-             responses={
-                 201: {"description": "Create new findings"},
-                 400: {"model": Model400, "description": "Error creating findings"},
-                 500: {"description": ERROR_MESSAGE_500},
-                 503: {"description": ERROR_MESSAGE_503}
-             })
-async def create_findings(findings: List[finding_schema.FindingCreate],
-                          db_connection: Session = Depends(get_db_connection)) -> int:
+@router.post(
+    "",
+    response_model=int,
+    summary="Create a finding",
+    status_code=status.HTTP_201_CREATED,
+    responses={
+        201: {"description": "Create new findings"},
+        400: {"model": Model400, "description": "Error creating findings"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+async def create_findings(
+    findings: List[finding_schema.FindingCreate],
+    db_connection: Session = Depends(get_db_connection),
+) -> int:
     """
           Create new findings
 
     - **db_connection**: Session of the database connection
     - **file_path**: file path
     - **line_number**: Line number
     - **commit_id**: commit hash
@@ -97,180 +106,215 @@
     - **author**: Author name
     - **email**: Email of the author
     - **event_sent_on**: event sent timestamp
     - **rule_name**: rule name
     - **repository_id**: repository id of the finding
     - **return**: int
           The output will contain the number of successful created findings
-      """
+    """
     try:
-        created_findings = finding_crud.create_findings(db_connection=db_connection, findings=findings)
+        created_findings = finding_crud.create_findings(
+            db_connection=db_connection, findings=findings
+        )
 
         # Clear cache related to findings
         await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
         await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_RULE)
     except KeyError as err:
         raise HTTPException(status_code=400, detail=str(err)) from err
     return len(created_findings)
 
 
-@router.get("/{finding_id}",
-            response_model=finding_schema.FindingRead,
-            summary="Fetch a finding by ID",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve finding <finding_id>"},
-                404: {"model": Model404, "description": "Finding <finding_id> not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    "/{finding_id}",
+    response_model=finding_schema.FindingRead,
+    summary="Fetch a finding by ID",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve finding <finding_id>"},
+        404: {"model": Model404, "description": "Finding <finding_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
 def read_finding(finding_id: int, db_connection: Session = Depends(get_db_connection)):
     """
         Read a finding by ID
 
     - **db_connection**: Session of the database connection
     - **finding_id**: ID of the finding for which details need to be fetched
     """
     db_finding = finding_crud.get_finding(db_connection, finding_id=finding_id)
     if db_finding is None:
         raise HTTPException(status_code=404, detail="Finding not found")
-    db_scan_findings = scan_finding_crud.get_scan_findings(db_connection, finding_id=finding_id)
+    db_scan_findings = scan_finding_crud.get_scan_findings(
+        db_connection, finding_id=finding_id
+    )
     scan_ids = [x.scan_id for x in db_scan_findings]
     return FindingRead.create_from_db_entities(db_finding=db_finding, scan_ids=scan_ids)
 
 
-@router.patch("/{finding_id}",
-              response_model=finding_schema.FindingRead,
-              summary="Partially update a finding by ID",
-              status_code=status.HTTP_200_OK,
-              responses={
-                  200: {"description": "Modify finding <finding_id>"},
-                  404: {"model": Model404, "description": "Finding <finding_id> not found"},
-                  500: {"description": ERROR_MESSAGE_500},
-                  503: {"description": ERROR_MESSAGE_503}
-              })
+@router.patch(
+    "/{finding_id}",
+    response_model=finding_schema.FindingRead,
+    summary="Partially update a finding by ID",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Modify finding <finding_id>"},
+        404: {"model": Model404, "description": "Finding <finding_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 async def patch_finding(
-        finding_id: int,
-        finding_update: finding_schema.FindingPatch,
-        db_connection: Session = Depends(get_db_connection)
+    finding_id: int,
+    finding_update: finding_schema.FindingPatch,
+    db_connection: Session = Depends(get_db_connection),
 ):
     """
         Partially update a finding by ID
 
     - **db_connection**: Session of the database connection
     - **finding_id**: ID of the finding for which details need to be updated
     - **event_sent_on**: Event sent timestamp
     """
     db_finding = finding_crud.get_finding(db_connection, finding_id=finding_id)
-    db_sca_findings = scan_finding_crud.get_scan_findings(db_connection, finding_id=finding_id)
+    db_sca_findings = scan_finding_crud.get_scan_findings(
+        db_connection, finding_id=finding_id
+    )
     scan_ids = [x.scan_id for x in db_sca_findings]
 
     # Clear cache related to findings
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
     if db_finding is None:
         raise HTTPException(status_code=404, detail="Finding not found")
     return FindingRead.create_from_db_entities(
-        finding_crud.patch_finding(db_connection, finding_id=finding_id, finding_update=finding_update),
-        scan_ids
+        finding_crud.patch_finding(
+            db_connection, finding_id=finding_id, finding_update=finding_update
+        ),
+        scan_ids,
     )
 
 
-@router.delete("/{finding_id}",
-               summary="Delete a finding",
-               status_code=status.HTTP_200_OK,
-               responses={
-                   200: {"description": "Delete finding <finding_id>"},
-                   404: {"model": Model404, "description": "Finding <finding_id> not found"},
-                   500: {"description": ERROR_MESSAGE_500},
-                   503: {"description": ERROR_MESSAGE_503}
-               })
-async def delete_finding(finding_id: int, db_connection: Session = Depends(get_db_connection)):
+@router.delete(
+    "/{finding_id}",
+    summary="Delete a finding",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Delete finding <finding_id>"},
+        404: {"model": Model404, "description": "Finding <finding_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+async def delete_finding(
+    finding_id: int, db_connection: Session = Depends(get_db_connection)
+):
     """
         Delete a finding object
 
     - **db_connection**: Session of the database connection
     - **finding_id**: ID of the finding to delete
     - **return**: The output will contain a success or error message based on the success of the deletion
     """
     db_finding = finding_crud.get_finding(db_connection, finding_id=finding_id)
     if db_finding is None:
         raise HTTPException(status_code=404, detail="Finding not found")
-    finding_crud.delete_finding(db_connection, finding_id=finding_id, delete_related=True)
+    finding_crud.delete_finding(
+        db_connection, finding_id=finding_id, delete_related=True
+    )
 
     # Clear cache related to findings
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
     return {"ok": True}
 
 
-@router.get(f"{RWS_ROUTE_TOTAL_COUNT_BY_RULE}""/{rule_name}",
-            summary="Get total findings count by rule",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve total findings count of rule <rule_name>"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_TOTAL_COUNT_BY_RULE}" "/{rule_name}",
+    summary="Get total findings count by rule",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve total findings count of rule <rule_name>"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
-def get_total_findings_count_by_rule(rule_name: str, db_connection: Session = Depends(get_db_connection)):
+def get_total_findings_count_by_rule(
+    rule_name: str, db_connection: Session = Depends(get_db_connection)
+):
     """
         Retrieve total findings count for a given rule
 
     - **db_connection**: Session of the database connection
     - **rule_name**: name of the rule
     """
     findings_filter = FindingsFilter(rule_names=[rule_name])
-    return finding_crud.get_total_findings_count(db_connection, findings_filter=findings_filter)
+    return finding_crud.get_total_findings_count(
+        db_connection, findings_filter=findings_filter
+    )
 
 
-@router.get(f"{RWS_ROUTE_BY_RULE}""/{rule_name}",
-            response_model=PaginationModel[finding_schema.FindingRead],
-            summary="Get findings by rule",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the findings of rule <rule_name>"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_BY_RULE}" "/{rule_name}",
+    response_model=PaginationModel[finding_schema.FindingRead],
+    summary="Get findings by rule",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the findings of rule <rule_name>"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
-def get_findings_by_rule(rule_name: str, skip: int = Query(default=0, ge=0),
-                         limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                         db_connection: Session = Depends(get_db_connection)) \
-        -> PaginationModel[finding_schema.FindingRead]:
+def get_findings_by_rule(
+    rule_name: str,
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[finding_schema.FindingRead]:
     """
         Retrieve all findings objects paginated by rule
 
     - **db_connection**: Session of the database connection
     - **rule_name**: Name of the rule to filter the findings by
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **return**: [FindingRead]
         The output will contain a PaginationModel containing the list of FindingRead type objects,
         or an empty list if no finding was found for the given rule
     """
-    findings = finding_crud.get_findings_by_rule(db_connection, skip=skip, limit=limit, rule_name=rule_name)
+    findings = finding_crud.get_findings_by_rule(
+        db_connection, skip=skip, limit=limit, rule_name=rule_name
+    )
     total_findings = finding_crud.get_total_findings_count(
-        db_connection, findings_filter=FindingsFilter(rule_names=[rule_name]))
-    return PaginationModel[finding_schema.FindingRead](data=findings, total=total_findings, limit=limit, skip=skip)
+        db_connection, findings_filter=FindingsFilter(rule_names=[rule_name])
+    )
+    return PaginationModel[finding_schema.FindingRead](
+        data=findings, total=total_findings, limit=limit, skip=skip
+    )
 
 
-@router.post(f"{RWS_ROUTE_AUDIT}/",
-             response_model=int,
-             summary="audit single/multiple findings",
-             status_code=status.HTTP_201_CREATED,
-             responses={
-                 201: {"description": "Audit(s) successfully saved"},
-                 404: {"model": Model404, "description": "Finding <finding_id> not found"},
-                 500: {"description": ERROR_MESSAGE_500},
-                 503: {"description": ERROR_MESSAGE_503}
-             })
+@router.post(
+    f"{RWS_ROUTE_AUDIT}/",
+    response_model=int,
+    summary="audit single/multiple findings",
+    status_code=status.HTTP_201_CREATED,
+    responses={
+        201: {"description": "Audit(s) successfully saved"},
+        404: {"model": Model404, "description": "Finding <finding_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 async def audit_findings(
-        request: Request,
-        audit: audit_schema.AuditMultiple,
-        db_connection: Session = Depends(get_db_connection)
+    request: Request,
+    audit: audit_schema.AuditMultiple,
+    db_connection: Session = Depends(get_db_connection),
 ) -> int:
     """
         Audit single/multiple findings, updating the status and comment
 
     - **db_connection**: Session of the database connection
     - **finding_ids**: List of finding IDs for which audit to be performed
     - **status**: Status of the finding, Valid values are NOT_ANALYZED, UNDER_REVIEW,
@@ -279,116 +323,157 @@
     - **return**: int
         The output will contain count of successful saved audits
     """
     audits = []
     for finding_id in audit.finding_ids:
         db_finding = finding_crud.get_finding(db_connection, finding_id=finding_id)
         if db_finding is None:
-            raise HTTPException(status_code=404, detail=f"Finding {finding_id} not found")
+            raise HTTPException(
+                status_code=404, detail=f"Finding {finding_id} not found"
+            )
         audits.append(
-            audit_crud.create_audit(db_connection=db_connection, finding_id=db_finding.id_,
-                                    auditor=request.user, status=audit.status, comment=audit.comment)
+            audit_crud.create_audit(
+                db_connection=db_connection,
+                finding_id=db_finding.id_,
+                auditor=request.user,
+                status=audit.status,
+                comment=audit.comment,
+            )
         )
 
         # Clear cache related to findings
         await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
     return len(audits)
 
 
-@router.get("/{finding_id}"f"{RWS_ROUTE_AUDIT}",
-            response_model=PaginationModel[audit_schema.AuditRead],
-            summary="Get audit(s) for finding",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the audit entries for a finding"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    "/{finding_id}" f"{RWS_ROUTE_AUDIT}",
+    response_model=PaginationModel[audit_schema.AuditRead],
+    summary="Get audit(s) for finding",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the audit entries for a finding"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
-def get_finding_audits(finding_id: int, skip: int = Query(default=0, ge=0),
-                       limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                       db_connection: Session = Depends(get_db_connection)) \
-        -> PaginationModel[audit_schema.AuditRead]:
+def get_finding_audits(
+    finding_id: int,
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[audit_schema.AuditRead]:
     """
         Retrieve all audit objects paginated for a finding
 
     - **db_connection**: Session of the database connection
     - **finding_id**: id of the finding to get the audit for
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **return**: [AuditRead]
         The output will contain a PaginationModel containing the list of AuditRead type objects,
         or an empty list if no audit info was found
     """
-    audits = audit_crud.get_finding_audits(db_connection, skip=skip, limit=limit, finding_id=finding_id)
-    total_audits = audit_crud.get_finding_audits_count(db_connection, finding_id=finding_id)
-    return PaginationModel[audit_schema.AuditRead](data=audits, total=total_audits, limit=limit, skip=skip)
+    audits = audit_crud.get_finding_audits(
+        db_connection, skip=skip, limit=limit, finding_id=finding_id
+    )
+    total_audits = audit_crud.get_finding_audits_count(
+        db_connection, finding_id=finding_id
+    )
+    return PaginationModel[audit_schema.AuditRead](
+        data=audits, total=total_audits, limit=limit, skip=skip
+    )
 
 
-@router.get(f"{RWS_ROUTE_SUPPORTED_STATUSES}/",
-            response_model=List[str],
-            summary="Get all supported statuses for findings",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the supported statuses for the findings"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_SUPPORTED_STATUSES}/",
+    response_model=List[str],
+    summary="Get all supported statuses for findings",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the supported statuses for the findings"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING_STATUS, expire=REDIS_CACHE_EXPIRE)
 def get_supported_statuses() -> List[str]:
     """
         Retrieve all supported statuses for findings
 
     - **return**: List[str]
         The output will contain a list of strings of unique statuses supported
     """
-    supported_finding_statuses = [finding_status for finding_status in FindingStatus if finding_status]
+    supported_finding_statuses = [
+        finding_status for finding_status in FindingStatus if finding_status
+    ]
     return supported_finding_statuses
 
 
-@router.get(f"{RWS_ROUTE_COUNT_BY_TIME}/""{time_type}",
-            response_model=PaginationModel[DateCountModel],
-            summary="Get all the findings by time period",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the findings by time-period <time_type>"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def get_count_by_time(time_type: DateFilter,
-                      skip: int = Query(default=0, ge=0),
-                      limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                      start_date_time: Optional[datetime] = Query(None),
-                      end_date_time: Optional[datetime] = Query(None),
-                      db_connection: Session = Depends(get_db_connection)) \
-        -> PaginationModel[DateCountModel]:
+@router.get(
+    f"{RWS_ROUTE_COUNT_BY_TIME}/" "{time_type}",
+    response_model=PaginationModel[DateCountModel],
+    summary="Get all the findings by time period",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the findings by time-period <time_type>"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def get_count_by_time(
+    time_type: DateFilter,
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    start_date_time: Optional[datetime] = Query(None),
+    end_date_time: Optional[datetime] = Query(None),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[DateCountModel]:
     """
         Retrieve all findings count by time period objects paginated
 
     - **db_connection**: Session of the database connection
     - **time_type**: required, filter on time type. Available values: month, week, day
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **start_date_time**: Optional, filter on start date
     - **end_date_time**: Optional, filter on end date
     - **return**: PaginationModel[DateCountModel]
         The output will contain a PaginationModel containing the list of DateCountModel type objects,
         or an empty list if no data was found
     """
     date_counts = []
-    findings = finding_crud.get_findings_count_by_time(db_connection=db_connection, date_type=time_type,
-                                                       start_date_time=start_date_time, end_date_time=end_date_time,
-                                                       skip=skip, limit=limit)
-    total_findings = finding_crud.get_findings_count_by_time_total(db_connection=db_connection, date_type=time_type,
-                                                                   start_date_time=start_date_time,
-                                                                   end_date_time=end_date_time)
+    findings = finding_crud.get_findings_count_by_time(
+        db_connection=db_connection,
+        date_type=time_type,
+        start_date_time=start_date_time,
+        end_date_time=end_date_time,
+        skip=skip,
+        limit=limit,
+    )
+    total_findings = finding_crud.get_findings_count_by_time_total(
+        db_connection=db_connection,
+        date_type=time_type,
+        start_date_time=start_date_time,
+        end_date_time=end_date_time,
+    )
     for finding in findings:
         if time_type == DateFilter.MONTH:
-            date_count = DateCountModel(finding_count=finding[2], date_lable=f"{finding[0]}-{finding[1]}")
+            date_count = DateCountModel(
+                finding_count=finding[2], date_lable=f"{finding[0]}-{finding[1]}"
+            )
         elif time_type == DateFilter.WEEK:
-            date_count = DateCountModel(finding_count=finding[2], date_lable=f"{finding[0]}-W{finding[1]}")
+            date_count = DateCountModel(
+                finding_count=finding[2], date_lable=f"{finding[0]}-W{finding[1]}"
+            )
         elif time_type == DateFilter.DAY:
-            date_count = DateCountModel(finding_count=finding[3], date_lable=f"{finding[0]}-{finding[1]}-{finding[2]}")
+            date_count = DateCountModel(
+                finding_count=finding[3],
+                date_lable=f"{finding[0]}-{finding[1]}-{finding[2]}",
+            )
 
         date_counts.append(date_count)
 
-    return PaginationModel[DateCountModel](data=date_counts, total=total_findings, limit=limit, skip=skip)
+    return PaginationModel[DateCountModel](
+        data=date_counts, total=total_findings, limit=limit, skip=skip
+    )
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/health.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/health.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # Standard Library
 import logging
 
 # Third Party
 from fastapi import APIRouter, status
 
 # First Party
-from resc_backend.constants import ERROR_MESSAGE_500, ERROR_MESSAGE_503, HEALTH_TAG, RWS_ROUTE_HEALTH
+from resc_backend.constants import (
+    ERROR_MESSAGE_500,
+    ERROR_MESSAGE_503,
+    HEALTH_TAG,
+    RWS_ROUTE_HEALTH,
+)
 
 router = APIRouter(tags=[HEALTH_TAG])
 
 logger = logging.getLogger(__name__)
 
 
-@router.get(f"{RWS_ROUTE_HEALTH}",
-            summary="Health check",
-            description="Retrieve the health status of RESC APIs",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve the health status"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_HEALTH}",
+    summary="Health check",
+    description="Retrieve the health status of RESC APIs",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve the health status"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 def health_check():
     return {"status": "OK"}
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/metrics.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,114 +15,147 @@
     METRICS_TAG,
     REDIS_CACHE_EXPIRE,
     RWS_ROUTE_AUDIT_COUNT_BY_AUDITOR_OVER_TIME,
     RWS_ROUTE_AUDITED_COUNT_OVER_TIME,
     RWS_ROUTE_COUNT_PER_VCS_PROVIDER_BY_WEEK,
     RWS_ROUTE_METRICS,
     RWS_ROUTE_PERSONAL_AUDITS,
-    RWS_ROUTE_UN_TRIAGED_COUNT_OVER_TIME
+    RWS_ROUTE_UN_TRIAGED_COUNT_OVER_TIME,
 )
 from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.cache_manager import CacheManager
 from resc_backend.resc_web_service.crud import audit as audit_crud
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
-from resc_backend.resc_web_service.schema.audit_count_over_time import AuditCountOverTime
-from resc_backend.resc_web_service.schema.finding_count_over_time import FindingCountOverTime
+from resc_backend.resc_web_service.schema.audit_count_over_time import (
+    AuditCountOverTime,
+)
+from resc_backend.resc_web_service.schema.finding_count_over_time import (
+    FindingCountOverTime,
+)
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
-from resc_backend.resc_web_service.schema.personal_audit_metrics import PersonalAuditMetrics
+from resc_backend.resc_web_service.schema.personal_audit_metrics import (
+    PersonalAuditMetrics,
+)
 from resc_backend.resc_web_service.schema.time_period import TimePeriod
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 router = APIRouter(prefix=f"{RWS_ROUTE_METRICS}", tags=[METRICS_TAG])
 logger = logging.getLogger(__name__)
 
 
-@router.get(f"{RWS_ROUTE_AUDITED_COUNT_OVER_TIME}",
-            response_model=list[FindingCountOverTime],
-            summary="Get count of audit status over time for given weeks per vcs provider",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve count of audit status over time for given weeks per vcs provider"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_AUDITED_COUNT_OVER_TIME}",
+    response_model=list[FindingCountOverTime],
+    summary="Get count of audit status over time for given weeks per vcs provider",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {
+            "description": "Retrieve count of audit status over time for given weeks per vcs provider"
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
-def get_finding_audit_count_over_time(db_connection: Session = Depends(get_db_connection),
-                                      weeks: Optional[int] = Query(default=13, ge=1),
-                                      audit_status: Optional[FindingStatus] = Query(default=FindingStatus.TRUE_POSITIVE)
-                                      ) -> list[FindingCountOverTime]:
+def get_finding_audit_count_over_time(
+    db_connection: Session = Depends(get_db_connection),
+    weeks: Optional[int] = Query(default=13, ge=1),
+    audit_status: Optional[FindingStatus] = Query(default=FindingStatus.TRUE_POSITIVE),
+) -> list[FindingCountOverTime]:
     """
         Retrieve count of audited findings over time for given weeks per vcs provider
     - **db_connection**: Session of the database connection
     - **weeks**: Nr of weeks for which to retrieve the audit status count
     - **audit_status**: audit status for which to retrieve the counts, defaults to True positive
     - **return**: [DateCountModel]
         The output will contain a list of DateCountModel type objects
     """
-    audit_counts = finding_crud.get_finding_audit_status_count_over_time(db_connection=db_connection,
-                                                                         status=audit_status,
-                                                                         weeks=weeks)
-    output = convert_rows_to_finding_count_over_time(count_over_time=audit_counts, weeks=weeks)
+    audit_counts = finding_crud.get_finding_audit_status_count_over_time(
+        db_connection=db_connection, status=audit_status, weeks=weeks
+    )
+    output = convert_rows_to_finding_count_over_time(
+        count_over_time=audit_counts, weeks=weeks
+    )
     return output
 
 
-@router.get(f"{RWS_ROUTE_COUNT_PER_VCS_PROVIDER_BY_WEEK}",
-            response_model=list[FindingCountOverTime],
-            summary="Get count of findings over time for given weeks per vcs provider",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve count of findings over time for given weeks per vcs provider"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_COUNT_PER_VCS_PROVIDER_BY_WEEK}",
+    response_model=list[FindingCountOverTime],
+    summary="Get count of findings over time for given weeks per vcs provider",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {
+            "description": "Retrieve count of findings over time for given weeks per vcs provider"
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
-def get_finding_total_count_over_time(db_connection: Session = Depends(get_db_connection),
-                                      weeks: Optional[int] = Query(default=13, ge=1)) -> list[FindingCountOverTime]:
+def get_finding_total_count_over_time(
+    db_connection: Session = Depends(get_db_connection),
+    weeks: Optional[int] = Query(default=13, ge=1),
+) -> list[FindingCountOverTime]:
     """
         Retrieve count of findings over time for given weeks per vcs provider
     - **db_connection**: Session of the database connection
     - **weeks**: Nr of weeks for which to retrieve the audit status count
     - **audit_status**: audit status for which to retrieve the counts, defaults to True positive
     - **return**: [DateCountModel]
         The output will contain a list of DateCountModel type objects
     """
-    audit_counts = finding_crud.get_finding_count_by_vcs_provider_over_time(db_connection=db_connection, weeks=weeks)
-    output = convert_rows_to_finding_count_over_time(count_over_time=audit_counts, weeks=weeks)
+    audit_counts = finding_crud.get_finding_count_by_vcs_provider_over_time(
+        db_connection=db_connection, weeks=weeks
+    )
+    output = convert_rows_to_finding_count_over_time(
+        count_over_time=audit_counts, weeks=weeks
+    )
     return output
 
 
-@router.get(f"{RWS_ROUTE_UN_TRIAGED_COUNT_OVER_TIME}",
-            response_model=list[FindingCountOverTime],
-            summary="Get count of UnTriaged findings over time for given weeks per vcs provider",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve count of UnTriaged findings over time for given weeks per vcs provider"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_UN_TRIAGED_COUNT_OVER_TIME}",
+    response_model=list[FindingCountOverTime],
+    summary="Get count of UnTriaged findings over time for given weeks per vcs provider",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {
+            "description": "Retrieve count of UnTriaged findings over time for given weeks per vcs provider"
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
-def get_finding_un_triaged_count_over_time(db_connection: Session = Depends(get_db_connection),
-                                           weeks: Optional[int] = Query(default=13, ge=1)) \
-        -> list[FindingCountOverTime]:
+def get_finding_un_triaged_count_over_time(
+    db_connection: Session = Depends(get_db_connection),
+    weeks: Optional[int] = Query(default=13, ge=1),
+) -> list[FindingCountOverTime]:
     """
         Retrieve count of UnTriaged findings over time for given weeks per vcs provider
     - **db_connection**: Session of the database connection
     - **weeks**: Nr of weeks for which to retrieve the audit status count
     - **audit_status**: audit status for which to retrieve the counts, defaults to True positive
     - **return**: [DateCountModel]
         The output will contain a list of DateCountModel type objects
     """
-    audit_counts = finding_crud.get_un_triaged_finding_count_by_vcs_provider_over_time(db_connection=db_connection,
-                                                                                       weeks=weeks)
-    output = convert_rows_to_finding_count_over_time(count_over_time=audit_counts, weeks=weeks)
+    audit_counts = finding_crud.get_un_triaged_finding_count_by_vcs_provider_over_time(
+        db_connection=db_connection, weeks=weeks
+    )
+    output = convert_rows_to_finding_count_over_time(
+        count_over_time=audit_counts, weeks=weeks
+    )
     return output
 
 
-def convert_rows_to_finding_count_over_time(count_over_time: dict, weeks: int) -> list[FindingCountOverTime]:
+def convert_rows_to_finding_count_over_time(
+    count_over_time: dict, weeks: int
+) -> list[FindingCountOverTime]:
     """
         Convert the rows from the database to the format of list[FindingCountOverTime]
     :param count_over_time:
         rows from the database
     :param weeks:
         number fo weeks that are in the data
     :return: output
@@ -132,134 +165,174 @@
     vcs_provider_types = list(VCSProviders)
 
     # create defaults with 0 value
     week_groups = {}
     for week in range(0, weeks):
         nth_week = datetime.utcnow() - timedelta(weeks=week)
         week = f"{nth_week.isocalendar().year} W{nth_week.isocalendar().week:02d}"
-        week_groups[week] = {vcs_provider_type: 0 for vcs_provider_type in vcs_provider_types + ["total"]}
+        week_groups[week] = {
+            vcs_provider_type: 0 for vcs_provider_type in vcs_provider_types + ["total"]
+        }
 
     # loop over the counts from the database
     for data in count_over_time:
         week = f"{getattr(data, 'year')} W{getattr(data, 'week'):02d}"
-        finding_count = getattr(data, 'finding_count')
+        finding_count = getattr(data, "finding_count")
 
-        week_groups[week][getattr(data, 'provider_type')] += finding_count
+        week_groups[week][getattr(data, "provider_type")] += finding_count
         week_groups[week]["total"] += finding_count
 
     # Convert to the output format
     output = []
     for week in sorted(week_groups.keys()):
-        week_data = FindingCountOverTime(time_period=week, total=week_groups[week]["total"])
+        week_data = FindingCountOverTime(
+            time_period=week, total=week_groups[week]["total"]
+        )
         for vcs_provider_type in vcs_provider_types:
-            setattr(week_data.vcs_provider_finding_count, vcs_provider_type, week_groups[week][vcs_provider_type])
+            setattr(
+                week_data.vcs_provider_finding_count,
+                vcs_provider_type,
+                week_groups[week][vcs_provider_type],
+            )
 
         output.append(week_data)
     return output
 
 
-@router.get(f"{RWS_ROUTE_AUDIT_COUNT_BY_AUDITOR_OVER_TIME}",
-            response_model=list[AuditCountOverTime],
-            summary="Get count of Audits by Auditor over time for given weeks",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve count of Audits by Auditor over time for given weeks"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_AUDIT_COUNT_BY_AUDITOR_OVER_TIME}",
+    response_model=list[AuditCountOverTime],
+    summary="Get count of Audits by Auditor over time for given weeks",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {
+            "description": "Retrieve count of Audits by Auditor over time for given weeks"
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
-def get_audit_count_by_auditor_over_time(db_connection: Session = Depends(get_db_connection),
-                                         weeks: Optional[int] = Query(default=13, ge=1)) \
-        -> list[AuditCountOverTime]:
+def get_audit_count_by_auditor_over_time(
+    db_connection: Session = Depends(get_db_connection),
+    weeks: Optional[int] = Query(default=13, ge=1),
+) -> list[AuditCountOverTime]:
     """
         Retrieve count of Audits by Auditor over time for given weeks
     - **db_connection**: Session of the database connection
     - **weeks**: Nr of weeks for which to retrieve the audit counts
     - **return**: [AuditCountOverTime]
         The output will contain a list of AuditCountOverTime type objects
     """
-    audit_counts = audit_crud.get_audit_count_by_auditor_over_time(db_connection=db_connection, weeks=weeks)
+    audit_counts = audit_crud.get_audit_count_by_auditor_over_time(
+        db_connection=db_connection, weeks=weeks
+    )
 
     # get the unique auditors from the data
     auditors_default = {}
     for audit in audit_counts:
-        auditors_default[getattr(audit, 'auditor')] = 0
+        auditors_default[getattr(audit, "auditor")] = 0
 
     # default to 0 per auditor for all weeks in range
     weekly_audit_counts = {}
     for week in range(0, weeks):
         nth_week = datetime.utcnow() - timedelta(weeks=week)
         week = f"{nth_week.isocalendar().year} W{nth_week.isocalendar().week:02d}"
-        weekly_audit_counts[week] = AuditCountOverTime(time_period=week, audit_by_auditor_count=dict(auditors_default))
+        weekly_audit_counts[week] = AuditCountOverTime(
+            time_period=week, audit_by_auditor_count=dict(auditors_default)
+        )
     weekly_audit_counts = dict(sorted(weekly_audit_counts.items()))
 
     # set the counts based on the data from the database
     for audit in audit_counts:
         audit_week = f"{getattr(audit, 'year')} W{getattr(audit, 'week'):02d}"
         if audit_week in weekly_audit_counts:
-            weekly_audit_counts.get(audit_week).audit_by_auditor_count[getattr(audit, 'auditor')] = \
-                getattr(audit, 'audit_count')
-            weekly_audit_counts.get(audit_week).total += getattr(audit, 'audit_count')
+            weekly_audit_counts.get(audit_week).audit_by_auditor_count[
+                getattr(audit, "auditor")
+            ] = getattr(audit, "audit_count")
+            weekly_audit_counts.get(audit_week).total += getattr(audit, "audit_count")
 
     sorted_weekly_audit_counts = dict(sorted(weekly_audit_counts.items()))
     output = list(sorted_weekly_audit_counts.values())
     return output
 
 
-@router.get(f"{RWS_ROUTE_PERSONAL_AUDITS}",
-            response_model=PersonalAuditMetrics,
-            summary="Get personal audit metrics",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Get personal audit metrics"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-@cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE, key_builder=CacheManager.personalized_key_builder)
-def get_personal_audit_metrics(request: Request, db_connection: Session = Depends(get_db_connection)) \
-        -> PersonalAuditMetrics:
+@router.get(
+    f"{RWS_ROUTE_PERSONAL_AUDITS}",
+    response_model=PersonalAuditMetrics,
+    summary="Get personal audit metrics",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Get personal audit metrics"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+@cache(
+    namespace=CACHE_NAMESPACE_FINDING,
+    expire=REDIS_CACHE_EXPIRE,
+    key_builder=CacheManager.personalized_key_builder,
+)
+def get_personal_audit_metrics(
+    request: Request, db_connection: Session = Depends(get_db_connection)
+) -> PersonalAuditMetrics:
     """
         Retrieve personal audit metrics
     - **db_connection**: Session of the database connection
     - **return**: [DateCountModel]
         The output will contain a PersonalAuditMetrics type objects
     """
     audit_counts = PersonalAuditMetrics()
-    audit_counts.today = audit_crud.get_personal_audit_count(db_connection=db_connection,
-                                                             auditor=request.user, time_period=TimePeriod.DAY)
-    audit_counts.current_week = audit_crud.get_personal_audit_count(db_connection=db_connection,
-                                                                    auditor=request.user, time_period=TimePeriod.WEEK)
-    audit_counts.last_week = audit_crud.get_personal_audit_count(db_connection=db_connection,
-                                                                 auditor=request.user, time_period=TimePeriod.LAST_WEEK)
-    audit_counts.current_month = audit_crud.get_personal_audit_count(db_connection=db_connection,
-                                                                     auditor=request.user, time_period=TimePeriod.MONTH)
-    audit_counts.current_year = audit_crud.get_personal_audit_count(db_connection=db_connection,
-                                                                    auditor=request.user, time_period=TimePeriod.YEAR)
-    audit_counts.forever = audit_crud.get_personal_audit_count(db_connection=db_connection,
-                                                               auditor=request.user, time_period=TimePeriod.FOREVER)
-
-    audit_counts.rank_current_week = determine_audit_rank_current_week(auditor=request.user,
-                                                                       db_connection=db_connection)
+    audit_counts.today = audit_crud.get_personal_audit_count(
+        db_connection=db_connection, auditor=request.user, time_period=TimePeriod.DAY
+    )
+    audit_counts.current_week = audit_crud.get_personal_audit_count(
+        db_connection=db_connection, auditor=request.user, time_period=TimePeriod.WEEK
+    )
+    audit_counts.last_week = audit_crud.get_personal_audit_count(
+        db_connection=db_connection,
+        auditor=request.user,
+        time_period=TimePeriod.LAST_WEEK,
+    )
+    audit_counts.current_month = audit_crud.get_personal_audit_count(
+        db_connection=db_connection, auditor=request.user, time_period=TimePeriod.MONTH
+    )
+    audit_counts.current_year = audit_crud.get_personal_audit_count(
+        db_connection=db_connection, auditor=request.user, time_period=TimePeriod.YEAR
+    )
+    audit_counts.forever = audit_crud.get_personal_audit_count(
+        db_connection=db_connection,
+        auditor=request.user,
+        time_period=TimePeriod.FOREVER,
+    )
+
+    audit_counts.rank_current_week = determine_audit_rank_current_week(
+        auditor=request.user, db_connection=db_connection
+    )
     return audit_counts
 
 
 def determine_audit_rank_current_week(auditor: str, db_connection: Session) -> int:
     """
         Retrieve personal audit ranking this week, compared to other auditors
     - **db_connection**: Session of the database connection
     - **auditor**: id of the auditor
     - **return**: int
         The output will be an integer nr of the ranking this week, defaulting to 0 if no audit was done by the auditor
     """
     audit_rank = 0
-    audit_counts_db = audit_crud.get_audit_count_by_auditor_over_time(db_connection=db_connection, weeks=0)
+    audit_counts_db = audit_crud.get_audit_count_by_auditor_over_time(
+        db_connection=db_connection, weeks=0
+    )
 
     auditor_counts = {}
     for audit in audit_counts_db:
-        auditor_counts[getattr(audit, 'auditor')] = getattr(audit, 'audit_count')
+        auditor_counts[getattr(audit, "auditor")] = getattr(audit, "audit_count")
 
-    sorted_auditor_counts = sorted(auditor_counts.items(), key=lambda x: x[1], reverse=True)
+    sorted_auditor_counts = sorted(
+        auditor_counts.items(), key=lambda x: x[1], reverse=True
+    )
     for auditor_count in dict(sorted_auditor_counts):
         audit_rank += 1
         if auditor_count == auditor:
             return audit_rank
     return 0
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/repositories.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/repositories.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,319 +15,387 @@
     REDIS_CACHE_EXPIRE,
     REPOSITORIES_TAG,
     RWS_ROUTE_DISTINCT_PROJECTS,
     RWS_ROUTE_DISTINCT_REPOSITORIES,
     RWS_ROUTE_FINDINGS_METADATA,
     RWS_ROUTE_LAST_SCAN,
     RWS_ROUTE_REPOSITORIES,
-    RWS_ROUTE_SCANS
+    RWS_ROUTE_SCANS,
 )
 from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.cache_manager import CacheManager
 from resc_backend.resc_web_service.crud import repository as repository_crud
 from resc_backend.resc_web_service.crud import scan as scan_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.helpers.resc_swagger_models import Model404
 from resc_backend.resc_web_service.schema import repository as repository_schema
-from resc_backend.resc_web_service.schema import repository_enriched as repository_enriched_schema
+from resc_backend.resc_web_service.schema import (
+    repository_enriched as repository_enriched_schema,
+)
 from resc_backend.resc_web_service.schema import scan as scan_schema
 from resc_backend.resc_web_service.schema.finding_count_model import FindingCountModel
 from resc_backend.resc_web_service.schema.pagination_model import PaginationModel
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 router = APIRouter(prefix=f"{RWS_ROUTE_REPOSITORIES}", tags=[REPOSITORIES_TAG])
 
 
-@router.get("",
-            response_model=PaginationModel[repository_schema.RepositoryRead],
-            summary="Get repositories",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the repositories"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def get_all_repositories(skip: int = Query(default=0, ge=0),
-                         limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                         vcsproviders: List[VCSProviders] = Query(None, alias="vcsprovider", title="VCSProviders"),
-                         projectfilter: Optional[str] = Query('', pattern=r"^[A-z0-9 .\-_%]*$"),
-                         repositoryfilter: Optional[str] = Query('', pattern=r"^[A-z0-9 .\-_%]*$"),
-                         db_connection: Session = Depends(get_db_connection)) \
-        -> PaginationModel[repository_schema.RepositoryRead]:
+@router.get(
+    "",
+    response_model=PaginationModel[repository_schema.RepositoryRead],
+    summary="Get repositories",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the repositories"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def get_all_repositories(
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    vcsproviders: List[VCSProviders] = Query(
+        None, alias="vcsprovider", title="VCSProviders"
+    ),
+    projectfilter: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
+    repositoryfilter: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[repository_schema.RepositoryRead]:
     """
         Retrieve all repository objects paginated
 
     - **db_connection**: Session of the database connection
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **vcsproviders**: Optional, filter on supported vcs provider types
     - **projectfilter**: Optional, filter on project name. It is used as a string contains filter
     - **repositoryfilter**: Optional, filter on repository name. It is used as a string contains filter
     - **return**: [RepositoryRead]
         The output will contain a PaginationModel containing the list of RepositoryRead type objects,
         or an empty list if no repository
     """
 
-    repositories = repository_crud.get_repositories(db_connection, skip=skip, limit=limit,
-                                                    vcs_providers=vcsproviders,
-                                                    project_filter=projectfilter,
-                                                    repository_filter=repositoryfilter)
-
-    total_repositories = repository_crud.get_repositories_count(db_connection, vcs_providers=vcsproviders,
-                                                                project_filter=projectfilter,
-                                                                repository_filter=repositoryfilter)
-
-    return PaginationModel[repository_schema.RepositoryRead](data=repositories, total=total_repositories,
-                                                             limit=limit, skip=skip)
-
-
-@router.post("",
-             response_model=repository_schema.RepositoryRead,
-             summary="Create a repository",
-             status_code=status.HTTP_201_CREATED,
-             responses={
-                 201: {"description": "Create a new repository"},
-                 500: {"description": ERROR_MESSAGE_500},
-                 503: {"description": ERROR_MESSAGE_503}
-             })
+    repositories = repository_crud.get_repositories(
+        db_connection,
+        skip=skip,
+        limit=limit,
+        vcs_providers=vcsproviders,
+        project_filter=projectfilter,
+        repository_filter=repositoryfilter,
+    )
+
+    total_repositories = repository_crud.get_repositories_count(
+        db_connection,
+        vcs_providers=vcsproviders,
+        project_filter=projectfilter,
+        repository_filter=repositoryfilter,
+    )
+
+    return PaginationModel[repository_schema.RepositoryRead](
+        data=repositories, total=total_repositories, limit=limit, skip=skip
+    )
+
+
+@router.post(
+    "",
+    response_model=repository_schema.RepositoryRead,
+    summary="Create a repository",
+    status_code=status.HTTP_201_CREATED,
+    responses={
+        201: {"description": "Create a new repository"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 async def create_repository(
-        repository: repository_schema.RepositoryCreate,
-        db_connection: Session = Depends(get_db_connection)):
+    repository: repository_schema.RepositoryCreate,
+    db_connection: Session = Depends(get_db_connection),
+):
     """
         Create a repository with all the information
 
     - **db_connection**: Session of the database connection
     - **project_key**: each repository must have a project name or key
     - **repository_id**: repository id
     - **repository_name**: repository name
     - **repository_url**: repository url
     - **vcs_instance**: vcs instance id
     """
-    repository = repository_crud.create_repository_if_not_exists(db_connection=db_connection, repository=repository)
+    repository = repository_crud.create_repository_if_not_exists(
+        db_connection=db_connection, repository=repository
+    )
 
     # Clear cache related to repository
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_REPOSITORY)
     return repository
 
 
-@router.get("/{repository_id}",
-            response_model=repository_schema.RepositoryRead,
-            summary="Fetch a repository by ID",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve repository <repository_id>"},
-                404: {"model": Model404, "description": "Repository <repository_id> not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def read_repository(repository_id: int, db_connection: Session = Depends(get_db_connection)):
+@router.get(
+    "/{repository_id}",
+    response_model=repository_schema.RepositoryRead,
+    summary="Fetch a repository by ID",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve repository <repository_id>"},
+        404: {"model": Model404, "description": "Repository <repository_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def read_repository(
+    repository_id: int, db_connection: Session = Depends(get_db_connection)
+):
     """
         Read a repository by ID
 
     - **db_connection**: Session of the database connection
     - **repository_id**: ID of the repository for which details need to be fetched
     """
-    db_repository = repository_crud.get_repository(db_connection, repository_id=repository_id)
+    db_repository = repository_crud.get_repository(
+        db_connection, repository_id=repository_id
+    )
     if db_repository is None:
         raise HTTPException(status_code=404, detail="Repository not found")
     return db_repository
 
 
-@router.put("/{repository_id}",
-            response_model=repository_schema.RepositoryRead,
-            summary="Update an existing repository",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Update repository <repository_id>"},
-                404: {"model": Model404, "description": "Repository <repository_id> not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.put(
+    "/{repository_id}",
+    response_model=repository_schema.RepositoryRead,
+    summary="Update an existing repository",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Update repository <repository_id>"},
+        404: {"model": Model404, "description": "Repository <repository_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 async def update_repository(
-        repository_id: int,
-        repository: repository_schema.RepositoryCreate,
-        db_connection: Session = Depends(get_db_connection)
+    repository_id: int,
+    repository: repository_schema.RepositoryCreate,
+    db_connection: Session = Depends(get_db_connection),
 ):
     """
         Update an existing repository
 
     - **db_connection**: Session of the database connection
     - **repository_id**: ID of the repository
     - **project_key**: project name that needs to be updated
     - **repository_id**: repository id that needs to be updated
     - **repository_name**: repository name that needs to be updated
     - **repository_url**: repository url that needs to be updated
     - **vcs_instance**: vcs instance id that needs to be updated
     """
-    db_repository = repository_crud.get_repository(db_connection, repository_id=repository_id)
+    db_repository = repository_crud.get_repository(
+        db_connection, repository_id=repository_id
+    )
     if db_repository is None:
         raise HTTPException(status_code=404, detail="Repository not found")
 
     updated_repository = repository_crud.update_repository(
-        db_connection=db_connection, repository_id=repository_id, repository=repository)
+        db_connection=db_connection, repository_id=repository_id, repository=repository
+    )
 
     # Clear cache related to repository
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_REPOSITORY)
     return updated_repository
 
 
-@router.delete("/{repository_id}",
-               summary="Delete a repository",
-               status_code=status.HTTP_200_OK,
-               responses={
-                   200: {"description": "Delete repository <repository_id>"},
-                   404: {"model": Model404, "description": "Repository <repository_id> not found"},
-                   500: {"description": ERROR_MESSAGE_500},
-                   503: {"description": ERROR_MESSAGE_503}
-               })
-async def delete_repository(repository_id: int, db_connection: Session = Depends(get_db_connection)):
+@router.delete(
+    "/{repository_id}",
+    summary="Delete a repository",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Delete repository <repository_id>"},
+        404: {"model": Model404, "description": "Repository <repository_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+async def delete_repository(
+    repository_id: int, db_connection: Session = Depends(get_db_connection)
+):
     """
         Delete a repository
 
     - **db_connection**: Session of the database connection
     - **repository_id**: ID of the repository to delete
     - **return**: The output will contain a success or error message based on the success of the deletion
     """
-    db_repository = repository_crud.get_repository(db_connection, repository_id=repository_id)
+    db_repository = repository_crud.get_repository(
+        db_connection, repository_id=repository_id
+    )
     if db_repository is None:
         raise HTTPException(status_code=404, detail="Repository not found")
-    repository_crud.delete_repository(db_connection, repository_id=repository_id, delete_related=True)
+    repository_crud.delete_repository(
+        db_connection, repository_id=repository_id, delete_related=True
+    )
 
     # Clear cache related to repository
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_REPOSITORY)
     return {"ok": True}
 
 
-@router.get(f"{RWS_ROUTE_DISTINCT_PROJECTS}/",
-            response_model=List[str],
-            summary="Get all unique project names",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the unique project-names"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_DISTINCT_PROJECTS}/",
+    response_model=List[str],
+    summary="Get all unique project names",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the unique project-names"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_REPOSITORY, expire=REDIS_CACHE_EXPIRE)
-def get_distinct_projects(vcsproviders: List[VCSProviders] = Query(None, alias="vcsprovider", title="VCSProviders"),
-                          repositoryfilter: Optional[str] = Query('', pattern=r"^[A-z0-9 .\-_%]*$"),
-                          onlyifhasfindings: bool = Query(default=False),
-                          db_connection: Session = Depends(get_db_connection)) -> List[str]:
+def get_distinct_projects(
+    vcsproviders: List[VCSProviders] = Query(
+        None, alias="vcsprovider", title="VCSProviders"
+    ),
+    repositoryfilter: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
+    onlyifhasfindings: bool = Query(default=False),
+    db_connection: Session = Depends(get_db_connection),
+) -> List[str]:
     """
         Retrieve all unique project names
 
     - **db_connection**: Session of the database connection
     - **vcsproviders**: Optional, filter on supported vcs provider types
     - **repositoryfilter**: Optional, filter on repository name. It is used as a string contains filter
     - **onlyifhasfindings**: Optional, filter all projects those have findings
     - **return**: List[str]
         The output will contain a list of unique projects
     """
 
-    distinct_projects = repository_crud.get_distinct_projects(db_connection,
-                                                              vcs_providers=vcsproviders,
-                                                              repository_filter=repositoryfilter,
-                                                              only_if_has_findings=onlyifhasfindings)
+    distinct_projects = repository_crud.get_distinct_projects(
+        db_connection,
+        vcs_providers=vcsproviders,
+        repository_filter=repositoryfilter,
+        only_if_has_findings=onlyifhasfindings,
+    )
     projects = [project.project_key for project in distinct_projects]
     return projects
 
 
-@router.get(f"{RWS_ROUTE_DISTINCT_REPOSITORIES}/",
-            response_model=List[str],
-            summary="Get all unique repository names",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the unique repository names"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_DISTINCT_REPOSITORIES}/",
+    response_model=List[str],
+    summary="Get all unique repository names",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the unique repository names"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_REPOSITORY, expire=REDIS_CACHE_EXPIRE)
-def get_distinct_repositories(vcsproviders: List[VCSProviders] = Query(None, alias="vcsprovider", title="VCSProviders"),
-                              projectname: Optional[str] = Query('', pattern=r"^[A-z0-9 .\-_%]*$"),
-                              onlyifhasfindings: bool = Query(default=False),
-                              db_connection: Session = Depends(get_db_connection)) -> List[str]:
+def get_distinct_repositories(
+    vcsproviders: List[VCSProviders] = Query(
+        None, alias="vcsprovider", title="VCSProviders"
+    ),
+    projectname: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
+    onlyifhasfindings: bool = Query(default=False),
+    db_connection: Session = Depends(get_db_connection),
+) -> List[str]:
     """
         Retrieve all unique repository names
 
     - **db_connection**: Session of the database connection
     - **vcsproviders**: Optional, filter of supported vcs provider types
     - **projectname**: Optional, filter on project name. It is used as a full string match filter
     - **onlyifhasfindings**: Optional, filter all repositories that have findings
     - **return**: List[str]
         The output will contain a list of unique repositories
     """
 
-    distinct_repositories = repository_crud.get_distinct_repositories(db_connection,
-                                                                      vcs_providers=vcsproviders,
-                                                                      project_name=projectname,
-                                                                      only_if_has_findings=onlyifhasfindings)
+    distinct_repositories = repository_crud.get_distinct_repositories(
+        db_connection,
+        vcs_providers=vcsproviders,
+        project_name=projectname,
+        only_if_has_findings=onlyifhasfindings,
+    )
     repositories = [repo.repository_name for repo in distinct_repositories]
     return repositories
 
 
-@router.get("/{repository_id}"f"{RWS_ROUTE_FINDINGS_METADATA}",
-            response_model=FindingCountModel[repository_schema.RepositoryRead],
-            summary="Get findings metadata for a repository",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve findings metadata for repository <repository_id>"},
-                404: {"model": Model404, "description": "Repository <repository_id> not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def get_findings_metadata_for_repository(repository_id: int,
-                                         db_connection: Session = Depends(get_db_connection)) \
-        -> FindingCountModel[repository_schema.RepositoryRead]:
+@router.get(
+    "/{repository_id}" f"{RWS_ROUTE_FINDINGS_METADATA}",
+    response_model=FindingCountModel[repository_schema.RepositoryRead],
+    summary="Get findings metadata for a repository",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {
+            "description": "Retrieve findings metadata for repository <repository_id>"
+        },
+        404: {"model": Model404, "description": "Repository <repository_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def get_findings_metadata_for_repository(
+    repository_id: int, db_connection: Session = Depends(get_db_connection)
+) -> FindingCountModel[repository_schema.RepositoryRead]:
     """
         Retrieve findings metadata for a repository
 
     - **db_connection**: Session of the database connection
     - **repository_id**: ID of the repository object for which findings metadata to be retrieved
     - **return**: RepositoryRead, findings count per status
         The output will contain a RepositoryRead type object along with findings count per status,
         or empty if no scan was found
     """
-    repository = repository_crud.get_repository(db_connection, repository_id=repository_id)
+    repository = repository_crud.get_repository(
+        db_connection, repository_id=repository_id
+    )
     if repository is None:
         raise HTTPException(status_code=404, detail="Repository not found")
 
     findings_meta_data = repository_crud.get_findings_metadata_by_repository_id(
-        db_connection, repository_ids=[repository_id])
+        db_connection, repository_ids=[repository_id]
+    )
 
     return FindingCountModel[repository_schema.RepositoryRead](
         data=repository,
         true_positive=findings_meta_data[repository_id]["true_positive"],
         false_positive=findings_meta_data[repository_id]["false_positive"],
         not_analyzed=findings_meta_data[repository_id]["not_analyzed"],
         under_review=findings_meta_data[repository_id]["under_review"],
-        clarification_required=findings_meta_data[repository_id]["clarification_required"],
-        total_findings_count=findings_meta_data[repository_id]["total_findings_count"])
-
-
-@router.get(f"{RWS_ROUTE_FINDINGS_METADATA}/",
-            response_model=PaginationModel[repository_enriched_schema.RepositoryEnrichedRead],
-            summary="Get all repositories with findings metadata",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the findings metadata for all the repositories"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+        clarification_required=findings_meta_data[repository_id][
+            "clarification_required"
+        ],
+        total_findings_count=findings_meta_data[repository_id]["total_findings_count"],
+    )
+
+
+@router.get(
+    f"{RWS_ROUTE_FINDINGS_METADATA}/",
+    response_model=PaginationModel[repository_enriched_schema.RepositoryEnrichedRead],
+    summary="Get all repositories with findings metadata",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {
+            "description": "Retrieve all the findings metadata for all the repositories"
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
 def get_all_repositories_with_findings_metadata(
-        skip: int = Query(default=0, ge=0),
-        limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-        vcsproviders: List[VCSProviders] = Query(None, alias="vcsprovider",
-                                                 title="VCSProviders"),
-        projectfilter: Optional[str] = Query('',
-                                             pattern=r"^[A-z0-9 .\-_%]*$"),
-        repositoryfilter: Optional[str] = Query('',
-                                                pattern=r"^[A-z0-9 .\-_%]*$"),
-        onlyifhasfindings: bool = Query(default=False),
-        db_connection: Session = Depends(get_db_connection)) \
-        -> PaginationModel[repository_enriched_schema.RepositoryEnrichedRead]:
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    vcsproviders: List[VCSProviders] = Query(
+        None, alias="vcsprovider", title="VCSProviders"
+    ),
+    projectfilter: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
+    repositoryfilter: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
+    onlyifhasfindings: bool = Query(default=False),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[repository_enriched_schema.RepositoryEnrichedRead]:
     """
         Retrieve all repository objects paginated
 
     - **db_connection**: Session of the database connection
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **vcsproviders**: Optional, filter on supported vcs provider types
@@ -335,101 +403,126 @@
     - **repositoryfilter**: Optional, filter on repository name. It is used as a string contains filter
     - **onlyifhasfindings**: Optional, filter all repositories those have findings
     - **return**: [RepositoryEnrichedRead]
         The output will contain a PaginationModel containing the list of RepositoryEnrichedRead type objects,
         or an empty list if no repository
     """
 
-    repositories = repository_crud.get_repositories(db_connection, skip=skip, limit=limit,
-                                                    vcs_providers=vcsproviders,
-                                                    project_filter=projectfilter,
-                                                    repository_filter=repositoryfilter,
-                                                    only_if_has_findings=onlyifhasfindings)
-
-    total_repositories = repository_crud.get_repositories_count(db_connection, vcs_providers=vcsproviders,
-                                                                project_filter=projectfilter,
-                                                                repository_filter=repositoryfilter,
-                                                                only_if_has_findings=onlyifhasfindings)
+    repositories = repository_crud.get_repositories(
+        db_connection,
+        skip=skip,
+        limit=limit,
+        vcs_providers=vcsproviders,
+        project_filter=projectfilter,
+        repository_filter=repositoryfilter,
+        only_if_has_findings=onlyifhasfindings,
+    )
+
+    total_repositories = repository_crud.get_repositories_count(
+        db_connection,
+        vcs_providers=vcsproviders,
+        project_filter=projectfilter,
+        repository_filter=repositoryfilter,
+        only_if_has_findings=onlyifhasfindings,
+    )
     repository_list = []
     repo_ids = [repo.id_ for repo in repositories]
     repo_findings_meta_data = repository_crud.get_findings_metadata_by_repository_id(
-        db_connection, repository_ids=repo_ids)
+        db_connection, repository_ids=repo_ids
+    )
     for repo in repositories:
         enriched_repository = repository_enriched_schema.RepositoryEnrichedRead(
             id_=repo.id_,
             project_key=repo.project_key,
             repository_id=repo.repository_id,
             repository_name=repo.repository_name,
             repository_url=repo.repository_url,
             vcs_provider=repo.provider_type,
             last_scan_id=repo.last_scan_id,
             last_scan_timestamp=repo.last_scan_timestamp,
             true_positive=repo_findings_meta_data[repo.id_]["true_positive"],
             false_positive=repo_findings_meta_data[repo.id_]["false_positive"],
             not_analyzed=repo_findings_meta_data[repo.id_]["not_analyzed"],
             under_review=repo_findings_meta_data[repo.id_]["under_review"],
-            clarification_required=repo_findings_meta_data[repo.id_]["clarification_required"],
-            total_findings_count=repo_findings_meta_data[repo.id_]["total_findings_count"]
+            clarification_required=repo_findings_meta_data[repo.id_][
+                "clarification_required"
+            ],
+            total_findings_count=repo_findings_meta_data[repo.id_][
+                "total_findings_count"
+            ],
         )
         repository_list.append(enriched_repository)
 
-    return PaginationModel[repository_enriched_schema.RepositoryEnrichedRead](data=repository_list,
-                                                                              total=total_repositories,
-                                                                              limit=limit, skip=skip)
-
-
-@router.get("/{repository_id}"f"{RWS_ROUTE_LAST_SCAN}",
-            response_model=scan_schema.ScanRead,
-            summary="Get latest scan for repository",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve the latest scan related to a repository"},
-                404: {"description": "Scan not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def get_last_scan_for_repository(repository_id: int, db_connection: Session = Depends(get_db_connection)) \
-        -> scan_schema.ScanRead:
+    return PaginationModel[repository_enriched_schema.RepositoryEnrichedRead](
+        data=repository_list, total=total_repositories, limit=limit, skip=skip
+    )
+
+
+@router.get(
+    "/{repository_id}" f"{RWS_ROUTE_LAST_SCAN}",
+    response_model=scan_schema.ScanRead,
+    summary="Get latest scan for repository",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve the latest scan related to a repository"},
+        404: {"description": "Scan not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def get_last_scan_for_repository(
+    repository_id: int, db_connection: Session = Depends(get_db_connection)
+) -> scan_schema.ScanRead:
     """
         Retrieve the latest scan object related to a repository
 
     - **db_connection**: Session of the database connection
     - **repository_id**: ID of the parent repository object for which scan objects to be retrieved
     - **return**: ScanRead
         The output will contain a ScanRead type object,
         or empty if no scan was found
     """
-    last_scan = scan_crud.get_latest_scan_for_repository(db_connection, repository_id=repository_id)
+    last_scan = scan_crud.get_latest_scan_for_repository(
+        db_connection, repository_id=repository_id
+    )
     if last_scan is None:
         raise HTTPException(status_code=404, detail="Scan not found")
     return last_scan
 
 
-@router.get("/{repository_id}"f"{RWS_ROUTE_SCANS}",
-            summary="Get scans for repository",
-            response_model=PaginationModel[scan_schema.ScanRead],
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the scans related to a repository"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def get_scans_for_repository(repository_id: int, skip: int = Query(default=0, ge=0),
-                             limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                             db_connection: Session = Depends(get_db_connection)) \
-        -> PaginationModel[scan_schema.ScanRead]:
+@router.get(
+    "/{repository_id}" f"{RWS_ROUTE_SCANS}",
+    summary="Get scans for repository",
+    response_model=PaginationModel[scan_schema.ScanRead],
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the scans related to a repository"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def get_scans_for_repository(
+    repository_id: int,
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[scan_schema.ScanRead]:
     """
         Retrieve all scan objects related to a repository paginated
 
     - **db_connection**: Session of the database connection
     - **repository_id**: ID of the parent repository object for which scan objects to be retrieved
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **return**: [ScanRead]
         The output will contain a PaginationModel containing the list of ScanRead type objects,
         or an empty list if no scan was found
     """
-    scans = scan_crud.get_scans(db_connection, skip=skip, limit=limit, repository_id=repository_id)
+    scans = scan_crud.get_scans(
+        db_connection, skip=skip, limit=limit, repository_id=repository_id
+    )
 
     total_scans = scan_crud.get_scans_count(db_connection, repository_id=repository_id)
 
-    return PaginationModel[scan_schema.ScanRead](data=scans, total=total_scans, limit=limit, skip=skip)
+    return PaginationModel[scan_schema.ScanRead](
+        data=scans, total=total_scans, limit=limit, skip=skip
+    )
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/rule_packs.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,231 +17,321 @@
     CACHE_NAMESPACE_RULE,
     CACHE_NAMESPACE_RULE_PACK,
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
     REDIS_CACHE_EXPIRE,
     RULE_PACKS_TAG,
-    RWS_ROUTE_RULE_PACKS
+    RWS_ROUTE_RULE_PACKS,
 )
 from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.cache_manager import CacheManager
 from resc_backend.resc_web_service.crud import rule as rule_crud
 from resc_backend.resc_web_service.crud import rule_pack as rule_pack_crud
 from resc_backend.resc_web_service.crud import rule_tag as rule_tag_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
-from resc_backend.resc_web_service.helpers.resc_swagger_models import Model400, Model404, Model409, Model422
+from resc_backend.resc_web_service.helpers.resc_swagger_models import (
+    Model400,
+    Model404,
+    Model409,
+    Model422,
+)
 from resc_backend.resc_web_service.helpers.rule import (
     create_toml_dictionary,
     create_toml_rule_file,
     get_mapped_global_allow_list_obj,
     map_dictionary_to_rule_allow_list_object,
-    validate_uploaded_file_and_read_content
+    validate_uploaded_file_and_read_content,
 )
 from resc_backend.resc_web_service.schema.pagination_model import PaginationModel
 from resc_backend.resc_web_service.schema.rule import RuleCreate
 from resc_backend.resc_web_service.schema.rule_allow_list import RuleAllowList
 from resc_backend.resc_web_service.schema.rule_pack import RulePackCreate, RulePackRead
 
 router = APIRouter(prefix=f"{RWS_ROUTE_RULE_PACKS}", tags=[RULE_PACKS_TAG])
 
 logger = logging.getLogger(__name__)
 
 
-@router.get("/versions",
-            response_model=PaginationModel[RulePackRead],
-            summary="Get rule packs",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the rule-packs"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    "/versions",
+    response_model=PaginationModel[RulePackRead],
+    summary="Get rule packs",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the rule-packs"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_RULE_PACK, expire=REDIS_CACHE_EXPIRE)
-def get_rule_packs(version: Optional[str] = Query(None, pattern=r"^\d+(?:\.\d+){2}$"),
-                   active: Optional[bool] = Query(None, description="Filter on active rule packs"),
-                   skip: int = Query(default=0, ge=0),
-                   limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                   db_connection: Session = Depends(get_db_connection)) -> PaginationModel[RulePackRead]:
+def get_rule_packs(
+    version: Optional[str] = Query(None, pattern=r"^\d+(?:\.\d+){2}$"),
+    active: Optional[bool] = Query(None, description="Filter on active rule packs"),
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[RulePackRead]:
     """
         Retrieve rule packs
 
     - **db_connection**: Session of the database connection
     - **version**: Optional, filter on rule pack version
     - **active**: Optional, filter on active rule pack
     - **skip**: Integer amount of records to skip, to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **return**: [RulePackRead]
         The output will contain a PaginationModel containing the list of RulePackRead type objects,
         or an empty list if no rule pack was found
     """
-    rule_packs = rule_pack_crud.get_rule_packs(db_connection=db_connection, version=version, active=active, skip=skip,
-                                               limit=limit)
-    total_rule_packs_count = rule_pack_crud.get_total_rule_packs_count(db_connection=db_connection, version=version,
-                                                                       active=active)
-    return PaginationModel[RulePackRead](data=rule_packs, total=total_rule_packs_count, limit=limit, skip=skip)
-
-
-@router.get("",
-            summary="Download rule pack in TOML format",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Download the rule-pack in TOML format"},
-                404: {"model": Model404, "description": "No rule-pack of version <version_id> found"},
-                422: {"model": Model422, "description": "Version <version_id> is not a valid semantic version"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-async def download_rule_pack_toml_file(version: Optional[str] = Query(None, pattern=r"^\d+(?:\.\d+){2}$"),
-                                       db_connection: Session = Depends(get_db_connection)) -> FileResponse:
+    rule_packs = rule_pack_crud.get_rule_packs(
+        db_connection=db_connection,
+        version=version,
+        active=active,
+        skip=skip,
+        limit=limit,
+    )
+    total_rule_packs_count = rule_pack_crud.get_total_rule_packs_count(
+        db_connection=db_connection, version=version, active=active
+    )
+    return PaginationModel[RulePackRead](
+        data=rule_packs, total=total_rule_packs_count, limit=limit, skip=skip
+    )
+
+
+@router.get(
+    "",
+    summary="Download rule pack in TOML format",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Download the rule-pack in TOML format"},
+        404: {
+            "model": Model404,
+            "description": "No rule-pack of version <version_id> found",
+        },
+        422: {
+            "model": Model422,
+            "description": "Version <version_id> is not a valid semantic version",
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+async def download_rule_pack_toml_file(
+    version: Optional[str] = Query(None, pattern=r"^\d+(?:\.\d+){2}$"),
+    db_connection: Session = Depends(get_db_connection),
+) -> FileResponse:
     """
         Download rule pack in TOML format
 
     - **db_connection**: Session of the database connection
     - **version**: Optional, filter on rule pack version
     - **return**: [FileResponse] The output returns rule pack file downloaded in TOML format
     """
     if not version:
-        logger.info("rule pack version not specified, downloading the currently active version")
+        logger.info(
+            "rule pack version not specified, downloading the currently active version"
+        )
     rule_pack_from_db = read_rule_pack(version=version, db_connection=db_connection)
     if rule_pack_from_db:
         version = rule_pack_from_db.version
-        rules = rule_crud.get_rules_by_rule_pack_version(db_connection=db_connection, rule_pack_version=version)
-        rule_tag_names = rule_tag_crud.get_rule_tag_names_by_rule_pack_version(db_connection=db_connection,
-                                                                               rule_pack_version=version)
-        global_allow_list = rule_crud.get_global_allow_list_by_rule_pack_version(db_connection=db_connection,
-                                                                                 rule_pack_version=version)
-        generated_toml_dict = create_toml_dictionary(version, rules, global_allow_list, rule_tag_names)
+        rules = rule_crud.get_rules_by_rule_pack_version(
+            db_connection=db_connection, rule_pack_version=version
+        )
+        rule_tag_names = rule_tag_crud.get_rule_tag_names_by_rule_pack_version(
+            db_connection=db_connection, rule_pack_version=version
+        )
+        global_allow_list = rule_crud.get_global_allow_list_by_rule_pack_version(
+            db_connection=db_connection, rule_pack_version=version
+        )
+        generated_toml_dict = create_toml_dictionary(
+            version, rules, global_allow_list, rule_tag_names
+        )
     else:
-        raise HTTPException(status_code=404, detail=f"No rule pack found with version {version}")
+        raise HTTPException(
+            status_code=404, detail=f"No rule pack found with version {version}"
+        )
 
     toml_file = create_toml_rule_file(generated_toml_dict)
     return FileResponse(toml_file.name, filename="RESC-SECRETS-RULE.toml")
 
 
-@router.post("",
-             summary="Upload rule pack in TOML format",
-             status_code=status.HTTP_200_OK,
-             responses={
-                 200: {"description": "Upload the rule-pack in TOML format"},
-                 400: {"model": Model400, "description": "No properties defined for rule allow list"},
-                 409: {"model": Model409, "description": "Rule-pack version <version_id> already exists"},
-                 422: {"model": Model422, "description": "Version <version_id> is not a valid semantic version"},
-                 500: {"description": ERROR_MESSAGE_500},
-                 503: {"description": ERROR_MESSAGE_503}
-             })
-async def upload_rule_pack_toml_file(version: str = Query(default=Required, pattern=r"^\d+(?:\.\d+){2}$"),
-                                     rule_file: UploadFile = File(...),
-                                     db_connection: Session = Depends(get_db_connection)) -> dict:
+@router.post(
+    "",
+    summary="Upload rule pack in TOML format",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Upload the rule-pack in TOML format"},
+        400: {
+            "model": Model400,
+            "description": "No properties defined for rule allow list",
+        },
+        409: {
+            "model": Model409,
+            "description": "Rule-pack version <version_id> already exists",
+        },
+        422: {
+            "model": Model422,
+            "description": "Version <version_id> is not a valid semantic version",
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+async def upload_rule_pack_toml_file(
+    version: str = Query(default=Required, pattern=r"^\d+(?:\.\d+){2}$"),
+    rule_file: UploadFile = File(...),
+    db_connection: Session = Depends(get_db_connection),
+) -> dict:
     """
         Upload TOML rule pack to database
 
     - **db_connection**: Session of the database connection
     - **version**: Version of the rule pack to be uploaded
     - **rule_file**: TOML rule pack file to be uploaded
     - **return**: dict The output returns uploaded rule pack name in dictionary format
     """
     content = validate_uploaded_file_and_read_content(rule_file)
     toml_rule_dictionary = tomlkit.loads(content)
 
     # Check if rule pack version exists
     rule_pack_from_db = read_rule_pack(version=version, db_connection=db_connection)
     if rule_pack_from_db:
-        raise HTTPException(status_code=409, detail=f"Unable to process rules. Rule pack version "
-                                                    f"{version} already exists")
+        raise HTTPException(
+            status_code=409,
+            detail=f"Unable to process rules. Rule pack version "
+            f"{version} already exists",
+        )
 
     # Insert in to RULE_ALLOW_LIST for storing global allow list
     created_global_rule_allow_list = None
-    global_allow_list: RuleAllowList = get_mapped_global_allow_list_obj(toml_rule_dictionary)
+    global_allow_list: RuleAllowList = get_mapped_global_allow_list_obj(
+        toml_rule_dictionary
+    )
     if global_allow_list:
-        created_global_rule_allow_list = create_rule_allow_list(rule_allow_list=global_allow_list,
-                                                                db_connection=db_connection)
+        created_global_rule_allow_list = create_rule_allow_list(
+            rule_allow_list=global_allow_list, db_connection=db_connection
+        )
         if not created_global_rule_allow_list.id_:
             logger.warning("Creating global rule allow list failed with an error")
 
     # # Insert in to RULE_PACK
-    global_allow_list_id = created_global_rule_allow_list.id_ if \
-        created_global_rule_allow_list and created_global_rule_allow_list.id_ else None
+    global_allow_list_id = (
+        created_global_rule_allow_list.id_
+        if created_global_rule_allow_list and created_global_rule_allow_list.id_
+        else None
+    )
 
     # Determine if uploaded rule pack needs to be activated
     current_newest_rule_pack = rule_pack_crud.get_newest_rule_pack(db_connection)
-    activate_uploaded_rule_pack = determine_uploaded_rule_pack_activation(version, current_newest_rule_pack)
-
-    rule_pack = RulePackCreate(version=version, active=activate_uploaded_rule_pack,
-                               global_allow_list=global_allow_list_id)
-    created_rule_pack_version = create_rule_pack_version(rule_pack=rule_pack, db_connection=db_connection)
+    activate_uploaded_rule_pack = determine_uploaded_rule_pack_activation(
+        version, current_newest_rule_pack
+    )
+
+    rule_pack = RulePackCreate(
+        version=version,
+        active=activate_uploaded_rule_pack,
+        global_allow_list=global_allow_list_id,
+    )
+    created_rule_pack_version = create_rule_pack_version(
+        rule_pack=rule_pack, db_connection=db_connection
+    )
     if created_rule_pack_version.version and activate_uploaded_rule_pack:
         # Update older rule packs to inactive
-        rule_pack_crud.make_older_rule_packs_to_inactive(latest_rule_pack_version=version,
-                                                         db_connection=db_connection)
+        rule_pack_crud.make_older_rule_packs_to_inactive(
+            latest_rule_pack_version=version, db_connection=db_connection
+        )
     else:
         logger.warning("Creating rule pack failed with an error")
 
     # Insert in to RULES
     if created_rule_pack_version and created_rule_pack_version.version:
-        insert_rules(version=version, toml_rule_dictionary=toml_rule_dictionary,
-                     db_connection=db_connection)
+        insert_rules(
+            version=version,
+            toml_rule_dictionary=toml_rule_dictionary,
+            db_connection=db_connection,
+        )
 
         # Clear cache related to rule-pack
         await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_RULE)
         await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_RULE_PACK)
         await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
     return {"filename": rule_file.filename}
 
 
-def read_rule_pack(version: Optional[str] = None,
-                   db_connection: Session = Depends(get_db_connection)) -> RulePackRead:
+def read_rule_pack(
+    version: Optional[str] = None, db_connection: Session = Depends(get_db_connection)
+) -> RulePackRead:
     """
         Read active rule pack from database
     :param version:
         optional, version of the rule pack to be fetched else latest rule pack version will be fetched
     :param db_connection:
         Session of the database connection
     :return: RulePackRead
         The output returns RulePackRead type object
     """
     if version:
         regex = re.compile(r"^\d+(?:\.\d+){2}$")
         if not re.fullmatch(regex, version):
-            raise HTTPException(status_code=422, detail=f"Version {version} is not a valid semantic version")
-    db_rule_pack = rule_pack_crud.get_rule_pack(db_connection=db_connection, version=version)
+            raise HTTPException(
+                status_code=422,
+                detail=f"Version {version} is not a valid semantic version",
+            )
+    db_rule_pack = rule_pack_crud.get_rule_pack(
+        db_connection=db_connection, version=version
+    )
     return db_rule_pack
 
 
 def create_rule_pack_version(
-        rule_pack: RulePackCreate,
-        db_connection: Session = Depends(get_db_connection)):
+    rule_pack: RulePackCreate, db_connection: Session = Depends(get_db_connection)
+):
     """
         Create rule pack version in database
     :param rule_pack:
         RulePackCreate object to be created
     :param db_connection:
         Session of the database connection
     """
-    return rule_pack_crud.create_rule_pack_version(db_connection=db_connection,
-                                                   rule_pack=rule_pack)
+    return rule_pack_crud.create_rule_pack_version(
+        db_connection=db_connection, rule_pack=rule_pack
+    )
 
 
 def create_rule_allow_list(
-        rule_allow_list: RuleAllowList,
-        db_connection: Session = Depends(get_db_connection)):
+    rule_allow_list: RuleAllowList, db_connection: Session = Depends(get_db_connection)
+):
     """
         Create rule allow list in database
     :param rule_allow_list:
         RuleAllowList object to be created
     :param db_connection:
         Session of the database connection
     """
-    if rule_allow_list.paths or rule_allow_list.commits or rule_allow_list.stop_words \
-            or rule_allow_list.description or rule_allow_list.regexes:
-        return rule_crud.create_rule_allow_list(db_connection=db_connection, rule_allow_list=rule_allow_list)
-    raise HTTPException(status_code=400, detail="No properties defined for rule allow list")
-
-
-def insert_rules(version: str, toml_rule_dictionary: dict, db_connection: Session = Depends(get_db_connection)):
+    if (
+        rule_allow_list.paths
+        or rule_allow_list.commits
+        or rule_allow_list.stop_words
+        or rule_allow_list.description
+        or rule_allow_list.regexes
+    ):
+        return rule_crud.create_rule_allow_list(
+            db_connection=db_connection, rule_allow_list=rule_allow_list
+        )
+    raise HTTPException(
+        status_code=400, detail="No properties defined for rule allow list"
+    )
+
+
+def insert_rules(
+    version: str,
+    toml_rule_dictionary: dict,
+    db_connection: Session = Depends(get_db_connection),
+):
     """
         Create rules in database
     :param version:
         version of the rule pack
     :param toml_rule_dictionary:
         rule pack toml in dictionary format
     :param db_connection:
@@ -263,87 +353,120 @@
                 keywords = ",".join(keyword_array)
 
             # Insert in to RULE_ALLOW_LIST for storing individual rule specific  allow list
             allow_list = rule["allowlist"] if "allowlist" in rule else None
             rule_allow_list_obj = map_dictionary_to_rule_allow_list_object(allow_list)
             created_rule_allow_list = None
             if rule_allow_list_obj:
-                created_rule_allow_list = create_rule_allow_list(rule_allow_list=rule_allow_list_obj,
-                                                                 db_connection=db_connection)
+                created_rule_allow_list = create_rule_allow_list(
+                    rule_allow_list=rule_allow_list_obj, db_connection=db_connection
+                )
 
             # Insert in to RULES
             if allow_list and created_rule_allow_list and created_rule_allow_list.id_:
                 created_allow_list_id = created_rule_allow_list.id_
             else:
                 created_allow_list_id = None
-            rule_obj = RuleCreate(rule_pack=version,
-                                  allow_list=created_allow_list_id,
-                                  rule_name=rule_name, description=description, entropy=entropy,
-                                  secret_group=secret_group, regex=regex, path=path, keywords=keywords)
-            created_rule = rule_crud.create_rule(rule=rule_obj, db_connection=db_connection)
+            rule_obj = RuleCreate(
+                rule_pack=version,
+                allow_list=created_allow_list_id,
+                rule_name=rule_name,
+                description=description,
+                entropy=entropy,
+                secret_group=secret_group,
+                regex=regex,
+                path=path,
+                keywords=keywords,
+            )
+            created_rule = rule_crud.create_rule(
+                rule=rule_obj, db_connection=db_connection
+            )
             if not created_rule.id_:
                 logger.warning(f"Creating rule failed for Rule: {rule_name}")
             if "tags" in rule:
-                _ = rule_tag_crud.create_rule_tag(db_connection=db_connection, rule_id=created_rule.id_,
-                                                  tags=rule["tags"])
-
-
-@router.get("/tags",
-            response_model=List[str],
-            summary="Get rule packs' tags",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the tags related to a rule-pack[s]"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+                _ = rule_tag_crud.create_rule_tag(
+                    db_connection=db_connection,
+                    rule_id=created_rule.id_,
+                    tags=rule["tags"],
+                )
+
+
+@router.get(
+    "/tags",
+    response_model=List[str],
+    summary="Get rule packs' tags",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the tags related to a rule-pack[s]"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_RULE_PACK, expire=REDIS_CACHE_EXPIRE)
-def get_rule_packs_tags(versions: Optional[List[str]] = Query(None, alias="version", title="version"),
-                        db_connection: Session = Depends(get_db_connection)) -> List[str]:
+def get_rule_packs_tags(
+    versions: Optional[List[str]] = Query(None, alias="version", title="version"),
+    db_connection: Session = Depends(get_db_connection),
+) -> List[str]:
     """
         Retrieve rule pack related tags
 
     :param db_connection: Session of the database connection
     :param versions: Optional, filter on rule pack version, if not provided filter on active.
     :return: List[str]
         The output will contain a list of tags related to one or more rule-packs.
     """
     if not versions:
-        active_rule_pack = rule_pack_crud.get_current_active_rule_pack(db_connection=db_connection)
+        active_rule_pack = rule_pack_crud.get_current_active_rule_pack(
+            db_connection=db_connection
+        )
         if not active_rule_pack:
-            raise HTTPException(status_code=500, detail="No currently active rule pack.")
+            raise HTTPException(
+                status_code=500, detail="No currently active rule pack."
+            )
         versions = [active_rule_pack.version]
-    rule_packs_tags = rule_pack_crud.get_rule_packs_tags(db_connection=db_connection, versions=versions)
+    rule_packs_tags = rule_pack_crud.get_rule_packs_tags(
+        db_connection=db_connection, versions=versions
+    )
     return rule_packs_tags
 
 
-def determine_uploaded_rule_pack_activation(requested_rule_pack_version: str,
-                                            latest_rule_pack_from_db: RulePackRead) -> bool:
+def determine_uploaded_rule_pack_activation(
+    requested_rule_pack_version: str, latest_rule_pack_from_db: RulePackRead
+) -> bool:
     """
         Determine if rule pack needs to be activated
     :param requested_rule_pack_version:
         version of the rule pack uploaded
     :param latest_rule_pack_from_db:
         latest rule pack in RulePackRead object
     :return: boolean
         The output returns true if rule pack needs to be activated else returns false
     """
     if latest_rule_pack_from_db:
-        if Version(latest_rule_pack_from_db.version) < Version(requested_rule_pack_version):
-            logger.info(f"Uploaded rule pack is of version '{requested_rule_pack_version}', using it to replace "
-                        f"'{latest_rule_pack_from_db.version}' as the active one.")
+        if Version(latest_rule_pack_from_db.version) < Version(
+            requested_rule_pack_version
+        ):
+            logger.info(
+                f"Uploaded rule pack is of version '{requested_rule_pack_version}', using it to replace "
+                f"'{latest_rule_pack_from_db.version}' as the active one."
+            )
             activate_uploaded_rule_pack = True
         else:
             if not latest_rule_pack_from_db.active:
-                logger.info(f"There is already a more recent rule pack present in the database "
-                            f"'{latest_rule_pack_from_db.version}', but it is set to inactive. "
-                            f"Activating the uploaded rule pack '{requested_rule_pack_version}'")
+                logger.info(
+                    f"There is already a more recent rule pack present in the database "
+                    f"'{latest_rule_pack_from_db.version}', but it is set to inactive. "
+                    f"Activating the uploaded rule pack '{requested_rule_pack_version}'"
+                )
                 activate_uploaded_rule_pack = True
             else:
-                logger.info(f"Uploaded rule pack is of version '{requested_rule_pack_version}', the existing rule pack "
-                            f"'{latest_rule_pack_from_db.version}' is kept as the active one.")
+                logger.info(
+                    f"Uploaded rule pack is of version '{requested_rule_pack_version}', the existing rule pack "
+                    f"'{latest_rule_pack_from_db.version}' is kept as the active one."
+                )
                 activate_uploaded_rule_pack = False
     else:
         logger.info(
-            f"No existing rule pack found, So activating the uploaded rule pack '{requested_rule_pack_version}'")
+            f"No existing rule pack found, So activating the uploaded rule pack '{requested_rule_pack_version}'"
+        )
         activate_uploaded_rule_pack = True
     return activate_uploaded_rule_pack
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/rules.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/rules.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,109 +13,144 @@
     CACHE_NAMESPACE_RULE,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
     REDIS_CACHE_EXPIRE,
     RULES_TAG,
     RWS_ROUTE_DETECTED_RULES,
     RWS_ROUTE_FINDING_STATUS_COUNT,
-    RWS_ROUTE_RULES
+    RWS_ROUTE_RULES,
 )
 from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.rule_count_model import RuleFindingCountModel
 from resc_backend.resc_web_service.schema.status_count import StatusCount
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 router = APIRouter(tags=[RULES_TAG])
 
 logger = logging.getLogger(__name__)
 
 
-@router.get(f"{RWS_ROUTE_DETECTED_RULES}",
-            response_model=List[str],
-            summary="Get unique rules from findings",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the unique detected rules across all the findings"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_DETECTED_RULES}",
+    response_model=List[str],
+    summary="Get unique rules from findings",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {
+            "description": "Retrieve all the unique detected rules across all the findings"
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_RULE, expire=REDIS_CACHE_EXPIRE)
 def get_distinct_rules_from_findings(
-        finding_statuses: List[FindingStatus] = Query(None, alias="findingstatus", title="FindingStatuses"),
-        vcs_providers: List[VCSProviders] = Query(None, alias="vcsprovider", title="VCSProviders"),
-        project_name: Optional[str] = Query('', pattern=r"^[A-z0-9 .\-_%]*$"),
-        repository_name: Optional[str] = Query('', pattern=r"^[A-z0-9 .\-_%]*$"),
-        start_date_time: Optional[datetime] = Query(None),
-        end_date_time: Optional[datetime] = Query(None),
-        rule_pack_versions: Optional[List[str]] = Query(None, alias="rule_pack_version", title="RulePackVersion"),
-        db_connection: Session = Depends(get_db_connection)) -> List[str]:
+    finding_statuses: List[FindingStatus] = Query(
+        None, alias="findingstatus", title="FindingStatuses"
+    ),
+    vcs_providers: List[VCSProviders] = Query(
+        None, alias="vcsprovider", title="VCSProviders"
+    ),
+    project_name: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
+    repository_name: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
+    start_date_time: Optional[datetime] = Query(None),
+    end_date_time: Optional[datetime] = Query(None),
+    rule_pack_versions: Optional[List[str]] = Query(
+        None, alias="rule_pack_version", title="RulePackVersion"
+    ),
+    db_connection: Session = Depends(get_db_connection),
+) -> List[str]:
     """
         Retrieve all uniquely detected rules across all findings in the database
 
     - **db_connection**: Session of the database connection
     - **finding_statuses**: Optional, filter on supported finding statuses
     - **vcs_providers**: Optional, filter on supported vcs provider types
     - **project_name**: Optional, filter on project name. It is used as a full string match filter
     - **repository_name**: Optional, filter on repository name. It is used as a string contains filter
     - **start_date_time**: Optional, filter on start date
     - **end_date_time**: Optional, filter on end date
     - **rule_pack_version**: Optional, filter on rule pack version
     - **return**: List[str] The output will contain a list of strings of unique rules in the findings table
     """
-    distinct_rules = finding_crud.get_distinct_rules_from_findings(db_connection,
-                                                                   finding_statuses=finding_statuses,
-                                                                   vcs_providers=vcs_providers,
-                                                                   project_name=project_name,
-                                                                   repository_name=repository_name,
-                                                                   start_date_time=start_date_time,
-                                                                   end_date_time=end_date_time,
-                                                                   rule_pack_versions=rule_pack_versions)
+    distinct_rules = finding_crud.get_distinct_rules_from_findings(
+        db_connection,
+        finding_statuses=finding_statuses,
+        vcs_providers=vcs_providers,
+        project_name=project_name,
+        repository_name=repository_name,
+        start_date_time=start_date_time,
+        end_date_time=end_date_time,
+        rule_pack_versions=rule_pack_versions,
+    )
     rules = [rule.rule_name for rule in distinct_rules]
     return rules
 
 
-@router.get(f"{RWS_ROUTE_RULES}{RWS_ROUTE_FINDING_STATUS_COUNT}",
-            response_model=List[RuleFindingCountModel],
-            summary="Get detected rules with counts per status",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the detected rules with counts per status"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    f"{RWS_ROUTE_RULES}{RWS_ROUTE_FINDING_STATUS_COUNT}",
+    response_model=List[RuleFindingCountModel],
+    summary="Get detected rules with counts per status",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the detected rules with counts per status"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
 def get_rules_finding_status_count(
-        rule_pack_versions: Optional[List[str]] = Query(None, alias="rule_pack_version", title="RulePackVersion"),
-        rule_tags: Optional[List[str]] = Query(None, alias="rule_tag", title="RuleTag"),
-        db_connection: Session = Depends(get_db_connection)) -> List[RuleFindingCountModel]:
+    rule_pack_versions: Optional[List[str]] = Query(
+        None, alias="rule_pack_version", title="RulePackVersion"
+    ),
+    rule_tags: Optional[List[str]] = Query(None, alias="rule_tag", title="RuleTag"),
+    db_connection: Session = Depends(get_db_connection),
+) -> List[RuleFindingCountModel]:
     """
         Retrieve all detected rules with finding counts per supported status
 
     - **rule_pack_version**: Optional, filter on rule pack version
     - **rule_tag**: Optional, filter on rule tag
     - **db_connection**: Session of the database connection
     - **return**: List[str] The output will contain a list of strings of unique rules with counts per status
     """
-    rule_finding_counts = finding_crud.get_rule_findings_count_by_status(db_connection,
-                                                                         rule_pack_versions=rule_pack_versions,
-                                                                         rule_tags=rule_tags)
+    rule_finding_counts = finding_crud.get_rule_findings_count_by_status(
+        db_connection, rule_pack_versions=rule_pack_versions, rule_tags=rule_tags
+    )
     rule_findings_counts = []
 
     for rule_name, rule_counts in rule_finding_counts.items():
-        rule_finding_count = RuleFindingCountModel(rule_name=rule_name,
-                                                   finding_count=rule_counts["total_findings_count"])
+        rule_finding_count = RuleFindingCountModel(
+            rule_name=rule_name, finding_count=rule_counts["total_findings_count"]
+        )
         rule_finding_count.finding_statuses_count.append(
-            StatusCount(status=FindingStatus.TRUE_POSITIVE, count=rule_counts["true_positive"]))
+            StatusCount(
+                status=FindingStatus.TRUE_POSITIVE, count=rule_counts["true_positive"]
+            )
+        )
         rule_finding_count.finding_statuses_count.append(
-            StatusCount(status=FindingStatus.FALSE_POSITIVE, count=rule_counts["false_positive"]))
+            StatusCount(
+                status=FindingStatus.FALSE_POSITIVE, count=rule_counts["false_positive"]
+            )
+        )
         rule_finding_count.finding_statuses_count.append(
-            StatusCount(status=FindingStatus.NOT_ANALYZED, count=rule_counts["not_analyzed"]))
+            StatusCount(
+                status=FindingStatus.NOT_ANALYZED, count=rule_counts["not_analyzed"]
+            )
+        )
         rule_finding_count.finding_statuses_count.append(
-            StatusCount(status=FindingStatus.UNDER_REVIEW, count=rule_counts["under_review"]))
+            StatusCount(
+                status=FindingStatus.UNDER_REVIEW, count=rule_counts["under_review"]
+            )
+        )
         rule_finding_count.finding_statuses_count.append(
-            StatusCount(status=FindingStatus.CLARIFICATION_REQUIRED, count=rule_counts["clarification_required"]))
+            StatusCount(
+                status=FindingStatus.CLARIFICATION_REQUIRED,
+                count=rule_counts["clarification_required"],
+            )
+        )
         rule_findings_counts.append(rule_finding_count)
 
     return rule_findings_counts
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/scans.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/scans.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     CACHE_NAMESPACE_RULE,
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
     RWS_ROUTE_DETECTED_RULES,
     RWS_ROUTE_FINDINGS,
     RWS_ROUTE_SCANS,
-    SCANS_TAG
+    SCANS_TAG,
 )
 from resc_backend.db.connection import Session
 from resc_backend.db.model import DBscanFinding
 from resc_backend.resc_web_service.cache_manager import CacheManager
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.crud import scan as scan_crud
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
@@ -33,115 +33,136 @@
 from resc_backend.resc_web_service.schema.pagination_model import PaginationModel
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 
 router = APIRouter(prefix=f"{RWS_ROUTE_SCANS}", tags=[SCANS_TAG])
 logger = logging.getLogger(__name__)
 
 
-@router.get("",
-            response_model=PaginationModel[scan_schema.ScanRead],
-            summary="Get scans",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the scan objects"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def get_all_scans(skip: int = Query(default=0, ge=0), limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                  db_connection: Session = Depends(get_db_connection)) -> PaginationModel[scan_schema.ScanRead]:
+@router.get(
+    "",
+    response_model=PaginationModel[scan_schema.ScanRead],
+    summary="Get scans",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the scan objects"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def get_all_scans(
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[scan_schema.ScanRead]:
     """
         Retrieve all scan objects paginated
 
     - **db_connection**: Session of the database connection
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **return**: [ScanRead]
         The output will contain a PaginationModel containing the list of ScanRead type objects,
         or an empty list if no scan was found
     """
     scans = scan_crud.get_scans(db_connection, skip=skip, limit=limit)
 
     total_scans = scan_crud.get_scans_count(db_connection)
 
-    return PaginationModel[scan_schema.ScanRead](data=scans, total=total_scans, limit=limit, skip=skip)
-
-
-@router.post("",
-             response_model=scan_schema.ScanRead,
-             summary="Create a scan",
-             status_code=status.HTTP_201_CREATED,
-             responses={
-                 201: {"description": "Create a new scan"},
-                 400: {"model": Model400, "description": "Error creating a new scan"},
-                 500: {"description": ERROR_MESSAGE_500},
-                 503: {"description": ERROR_MESSAGE_503}
-             })
-def create_scan(scan: scan_schema.ScanCreate, db_connection: Session = Depends(get_db_connection)):
+    return PaginationModel[scan_schema.ScanRead](
+        data=scans, total=total_scans, limit=limit, skip=skip
+    )
+
+
+@router.post(
+    "",
+    response_model=scan_schema.ScanRead,
+    summary="Create a scan",
+    status_code=status.HTTP_201_CREATED,
+    responses={
+        201: {"description": "Create a new scan"},
+        400: {"model": Model400, "description": "Error creating a new scan"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def create_scan(
+    scan: scan_schema.ScanCreate, db_connection: Session = Depends(get_db_connection)
+):
     """
         Create a scan with all the information
 
     - **db_connection**: Session of the database connection
     - **scan_type**: scan type, supported values are BASE or INCREMENTAL
     - **last_scanned_commit**: last scanned commit hash
     - **timestamp**: creation timestamp
     - **increment_number**: scan increment number
     - **rule_pack**: rule pack version
     - **repository_id**: repository id
     """
     # Determine the increment number if needed and not supplied
-    if scan.scan_type == ScanType.INCREMENTAL and (not scan.increment_number or scan.increment_number <= 0):
-        last_scan = scan_crud.get_latest_scan_for_repository(db_connection, repository_id=scan.repository_id)
+    if scan.scan_type == ScanType.INCREMENTAL and (
+        not scan.increment_number or scan.increment_number <= 0
+    ):
+        last_scan = scan_crud.get_latest_scan_for_repository(
+            db_connection, repository_id=scan.repository_id
+        )
         new_increment = last_scan.increment_number + 1
         scan.increment_number = new_increment
 
     try:
         created_scan = scan_crud.create_scan(db_connection=db_connection, scan=scan)
     except IntegrityError as err:
         logger.debug(f"Error creating new scan object: {err}")
-        raise HTTPException(status_code=400, detail="Error creating new scan object") from err
+        raise HTTPException(
+            status_code=400, detail="Error creating new scan object"
+        ) from err
     return created_scan
 
 
-@router.get("/{scan_id}",
-            response_model=scan_schema.ScanRead,
-            summary="Fetch a scan by ID",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve scan <scan_id>"},
-                404: {"model": Model404, "description": "Scan <scan_id> not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.get(
+    "/{scan_id}",
+    response_model=scan_schema.ScanRead,
+    summary="Fetch a scan by ID",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve scan <scan_id>"},
+        404: {"model": Model404, "description": "Scan <scan_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 def read_scan(scan_id: int, db_connection: Session = Depends(get_db_connection)):
     """
         Read a scan by ID
 
     - **db_connection**: Session of the database connection
     - **scan_id**: ID of the scan for which details need to be fetched
     """
     db_scan = scan_crud.get_scan(db_connection, scan_id=scan_id)
     if db_scan is None:
         raise HTTPException(status_code=404, detail="Scan not found")
     return db_scan
 
 
-@router.put("/{scan_id}",
-            response_model=scan_schema.ScanRead,
-            summary="Update an existing scan",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Update scan <scan_id>"},
-                404: {"model": Model404, "description": "Scan <scan_id> not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.put(
+    "/{scan_id}",
+    response_model=scan_schema.ScanRead,
+    summary="Update an existing scan",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Update scan <scan_id>"},
+        404: {"model": Model404, "description": "Scan <scan_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 def update_scan(
-        scan_id: int,
-        scan: scan_schema.ScanCreate,
-        db_connection: Session = Depends(get_db_connection)
+    scan_id: int,
+    scan: scan_schema.ScanCreate,
+    db_connection: Session = Depends(get_db_connection),
 ):
     """
         Update an existing scan
 
     - **db_connection**: Session of the database connection
     - **scan_type**: scan type, supported values are BASE or INCREMENTAL
     - **last_scanned_commit**: last scanned commit
@@ -150,54 +171,68 @@
     - **rule_pack**: rule pack version
     - **repository_id**: repository id
 
     """
     db_scan = scan_crud.get_scan(db_connection, scan_id=scan_id)
     if db_scan is None:
         raise HTTPException(status_code=404, detail="Scan not found")
-    return scan_crud.update_scan(db_connection=db_connection, scan_id=scan_id, scan=scan)
+    return scan_crud.update_scan(
+        db_connection=db_connection, scan_id=scan_id, scan=scan
+    )
 
 
-@router.delete("/{scan_id}",
-               summary="Delete a scan",
-               status_code=status.HTTP_200_OK,
-               responses={
-                   200: {"description": "Delete scan <scan_id>"},
-                   404: {"model": Model404, "description": "Scan <scan_id> not found"},
-                   500: {"description": ERROR_MESSAGE_500},
-                   503: {"description": ERROR_MESSAGE_503}
-               })
+@router.delete(
+    "/{scan_id}",
+    summary="Delete a scan",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Delete scan <scan_id>"},
+        404: {"model": Model404, "description": "Scan <scan_id> not found"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
 def delete_scan(scan_id: int, db_connection: Session = Depends(get_db_connection)):
     """
         Delete a scan object
 
     - **db_connection**: Session of the database connection
     - **scan_id**: ID of the scan to delete
     - **return**: The output will contain a success or error message based on the success of the deletion
     """
     db_scan = scan_crud.get_scan(db_connection, scan_id=scan_id)
     if db_scan is None:
         raise HTTPException(status_code=404, detail="Scan not found")
-    scan_crud.delete_scan(db_connection, repository_id=db_scan.repository_id, scan_id=scan_id, delete_related=True)
+    scan_crud.delete_scan(
+        db_connection,
+        repository_id=db_scan.repository_id,
+        scan_id=scan_id,
+        delete_related=True,
+    )
     return {"ok": True}
 
 
-@router.post("/{scan_id}"f"{RWS_ROUTE_FINDINGS}",
-             response_model=int,
-             summary="Create scan findings",
-             status_code=status.HTTP_201_CREATED,
-             responses={
-                 201: {"description": "Create findings and their associated scan_findings for scan <scan_id>"},
-                 500: {"description": ERROR_MESSAGE_500},
-                 503: {"description": ERROR_MESSAGE_503}
-             })
-async def create_scan_findings(scan_id: int,
-                               findings: List[finding_schema.FindingCreate],
-                               db_connection: Session = Depends(get_db_connection)) \
-        -> int:
+@router.post(
+    "/{scan_id}" f"{RWS_ROUTE_FINDINGS}",
+    response_model=int,
+    summary="Create scan findings",
+    status_code=status.HTTP_201_CREATED,
+    responses={
+        201: {
+            "description": "Create findings and their associated scan_findings for scan <scan_id>"
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+async def create_scan_findings(
+    scan_id: int,
+    findings: List[finding_schema.FindingCreate],
+    db_connection: Session = Depends(get_db_connection),
+) -> int:
     """
         Creates findings and their associated scan_findings for a given scan
 
     - **db_connection**: Session of the database connection
     - **scan_id**:  Id of the scan for which findings need to be inserted
     - **file_path**: file path
     - **line_number**: Line number
@@ -215,123 +250,169 @@
     - **rule_name**: rule name
     - **repository_id**: repository id of the finding
     - **return**: [FindingRead]
         The output will contain a PaginationModel containing the list of FindingRead type objects,
         or an empty list if no scan was found
     """
 
-    created_findings = finding_crud.create_findings(db_connection=db_connection, findings=findings)
+    created_findings = finding_crud.create_findings(
+        db_connection=db_connection, findings=findings
+    )
     scan_findings = []
     for finding in created_findings:
         scan_finding = DBscanFinding(finding_id=finding.id_, scan_id=scan_id)
         scan_findings.append(scan_finding)
 
     _ = scan_finding_crud.create_scan_findings(
-        db_connection=db_connection, scan_findings=scan_findings)
+        db_connection=db_connection, scan_findings=scan_findings
+    )
 
     # Clear cache related to findings
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_RULE)
 
     return len(created_findings)
 
 
-@router.get("/{scan_id}"f"{RWS_ROUTE_FINDINGS}",
-            response_model=PaginationModel[finding_schema.FindingRead],
-            summary="Get scan findings associated with a scan ID",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve findings associated with scan <scan_id>"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def get_scan_findings(scan_id: int, skip: int = Query(default=0, ge=0),
-                      limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                      rules: List[str] = Query([], pattern=r"^[A-z0-9 .\-_%]*$", alias="rule", title="rule"),
-                      statuses: List[FindingStatus] = Query(None, alias="status", title="status"),
-                      db_connection: Session = Depends(get_db_connection)) \
-        -> PaginationModel[finding_schema.FindingRead]:
+@router.get(
+    "/{scan_id}" f"{RWS_ROUTE_FINDINGS}",
+    response_model=PaginationModel[finding_schema.FindingRead],
+    summary="Get scan findings associated with a scan ID",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve findings associated with scan <scan_id>"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def get_scan_findings(
+    scan_id: int,
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    rules: List[str] = Query(
+        [], pattern=r"^[A-z0-9 .\-_%]*$", alias="rule", title="rule"
+    ),
+    statuses: List[FindingStatus] = Query(None, alias="status", title="status"),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[finding_schema.FindingRead]:
     """
         Retrieve all finding objects paginated related to a scan_id
 
     - **db_connection**: Session of the database connection
     - **scan_id**: Id of the scan for which to retrieve the findings
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **rules**: optional, filter on rule name. It is used as a string contains filter
     - **statuses**:  optional, filter on status of findings
     - **return**: [FindingRead]
         The output will contain a PaginationModel containing the list of FindingRead type objects,
         or an empty list if no scan was found
     """
-    findings = finding_crud.get_scans_findings(db_connection, scan_ids=[scan_id], skip=skip, limit=limit,
-                                               rules_filter=rules, statuses_filter=statuses)
-
-    findings_filter = FindingsFilter(scan_ids=[scan_id], rule_names=rules, finding_statuses=statuses)
-    total_findings = finding_crud.get_total_findings_count(db_connection, findings_filter=findings_filter)
-
-    return PaginationModel[finding_schema.FindingRead](data=findings, total=total_findings, limit=limit, skip=skip)
-
-
-@router.get(f"{RWS_ROUTE_FINDINGS}/",
-            response_model=PaginationModel[finding_schema.FindingRead],
-            summary="Get scan findings",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve findings associated with scan <scan_id>"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def get_scans_findings(scan_ids: List[int] = Query([], alias="scan_id", title="Scan ids"),
-                       skip: int = Query(default=0, ge=0),
-                       limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                       rules: List[str] = Query([], pattern=r"^[A-z0-9 .\-_%]*$", alias="rule", title="rule"),
-                       statuses: List[FindingStatus] = Query(None, alias="status", title="status"),
-                       db_connection: Session = Depends(get_db_connection)) \
-        -> PaginationModel[finding_schema.FindingRead]:
+    findings = finding_crud.get_scans_findings(
+        db_connection,
+        scan_ids=[scan_id],
+        skip=skip,
+        limit=limit,
+        rules_filter=rules,
+        statuses_filter=statuses,
+    )
+
+    findings_filter = FindingsFilter(
+        scan_ids=[scan_id], rule_names=rules, finding_statuses=statuses
+    )
+    total_findings = finding_crud.get_total_findings_count(
+        db_connection, findings_filter=findings_filter
+    )
+
+    return PaginationModel[finding_schema.FindingRead](
+        data=findings, total=total_findings, limit=limit, skip=skip
+    )
+
+
+@router.get(
+    f"{RWS_ROUTE_FINDINGS}/",
+    response_model=PaginationModel[finding_schema.FindingRead],
+    summary="Get scan findings",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve findings associated with scan <scan_id>"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def get_scans_findings(
+    scan_ids: List[int] = Query([], alias="scan_id", title="Scan ids"),
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    rules: List[str] = Query(
+        [], pattern=r"^[A-z0-9 .\-_%]*$", alias="rule", title="rule"
+    ),
+    statuses: List[FindingStatus] = Query(None, alias="status", title="status"),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[finding_schema.FindingRead]:
     """
         Retrieve all finding objects paginated related to a scan_id
 
     - **db_connection**: Session of the database connection
     - **scan_ids**: Optional, List of scan IDs for which findings to be retrieved
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **rule**: optional, filter on rule name. It is used as a string contains filter
     - **statuses**:  optional, filter on status of findings
     - **return**: [FindingRead]
         The output will contain a PaginationModel containing the list of FindingRead type objects,
         or an empty list if no scan was found
     """
-    findings = finding_crud.get_scans_findings(db_connection, scan_ids=scan_ids, skip=skip, limit=limit,
-                                               rules_filter=rules, statuses_filter=statuses)
-
-    findings_filter = FindingsFilter(scan_ids=scan_ids, rule_names=rules, finding_statuses=statuses)
-    total_findings = finding_crud.get_total_findings_count(db_connection, findings_filter=findings_filter)
-
-    return PaginationModel[finding_schema.FindingRead](data=findings, total=total_findings, limit=limit, skip=skip)
-
-
-@router.get(f"{RWS_ROUTE_DETECTED_RULES}/",
-            response_model=List[str],
-            summary="Get unique rules from scans",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the unique rules associated with specified scans"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def get_distinct_rules_from_scans(scan_ids: List[int] = Query([], alias="scan_id", title="Scan ids"),
-                                  db_connection: Session = Depends(get_db_connection)) -> List[str]:
+    findings = finding_crud.get_scans_findings(
+        db_connection,
+        scan_ids=scan_ids,
+        skip=skip,
+        limit=limit,
+        rules_filter=rules,
+        statuses_filter=statuses,
+    )
+
+    findings_filter = FindingsFilter(
+        scan_ids=scan_ids, rule_names=rules, finding_statuses=statuses
+    )
+    total_findings = finding_crud.get_total_findings_count(
+        db_connection, findings_filter=findings_filter
+    )
+
+    return PaginationModel[finding_schema.FindingRead](
+        data=findings, total=total_findings, limit=limit, skip=skip
+    )
+
+
+@router.get(
+    f"{RWS_ROUTE_DETECTED_RULES}/",
+    response_model=List[str],
+    summary="Get unique rules from scans",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {
+            "description": "Retrieve all the unique rules associated with specified scans"
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def get_distinct_rules_from_scans(
+    scan_ids: List[int] = Query([], alias="scan_id", title="Scan ids"),
+    db_connection: Session = Depends(get_db_connection),
+) -> List[str]:
     """
         Retrieve all uniquely detected rules for given scans
 
     - **db_connection**: Session of the database connection
     - **scan_ids**: scan ids for which to retrieve the unique rules
     - **return**: List[str]
         The output will contain a list of strings of unique rules for given scan ids
     """
     return_rules = []
     if scan_ids:
-        rules = finding_crud.get_distinct_rules_from_scans(db_connection, scan_ids=scan_ids)
+        rules = finding_crud.get_distinct_rules_from_scans(
+            db_connection, scan_ids=scan_ids
+        )
         for rule in rules:
             return_rules.append(rule.rule_name)
     return return_rules
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/endpoints/vcs_instances.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,142 +9,184 @@
 # First Party
 from resc_backend.constants import (
     CACHE_NAMESPACE_VCS_INSTANCE,
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
     RWS_ROUTE_VCS,
-    VCS_TAG
+    VCS_TAG,
 )
 from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.cache_manager import CacheManager
 from resc_backend.resc_web_service.crud import vcs_instance as vcs_instance_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.helpers.resc_swagger_models import Model400, Model404
 from resc_backend.resc_web_service.schema import vcs_instance as vcs_instance_schema
 from resc_backend.resc_web_service.schema.pagination_model import PaginationModel
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 router = APIRouter(prefix=f"{RWS_ROUTE_VCS}", tags=[VCS_TAG])
 logger = logging.getLogger(__name__)
 
 
-@router.post("", response_model=vcs_instance_schema.VCSInstanceRead,
-             summary="Create a VCS instance",
-             status_code=status.HTTP_201_CREATED,
-             responses={
-                 201: {"description": "Create new VCS instance"},
-                 400: {"model": Model400, "description": "Error creating new VCS instance"},
-                 500: {"description": ERROR_MESSAGE_500},
-                 503: {"description": ERROR_MESSAGE_503}
-             })
-async def create_vcs_instance(vcs_instance: vcs_instance_schema.VCSInstanceCreate,
-                              db_connection: Session = Depends(get_db_connection)) \
-        -> vcs_instance_schema.VCSInstanceRead:
+@router.post(
+    "",
+    response_model=vcs_instance_schema.VCSInstanceRead,
+    summary="Create a VCS instance",
+    status_code=status.HTTP_201_CREATED,
+    responses={
+        201: {"description": "Create new VCS instance"},
+        400: {"model": Model400, "description": "Error creating new VCS instance"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+async def create_vcs_instance(
+    vcs_instance: vcs_instance_schema.VCSInstanceCreate,
+    db_connection: Session = Depends(get_db_connection),
+) -> vcs_instance_schema.VCSInstanceRead:
     """
         Create new VCS instance object
 
     - **db_connection**: Session of the database connection
     - **vcs_instance**: VCSInstanceCreate type object of the VCS Instance to create
     - **return**: VCSInstanceRead
         The output will contain a VCSInstanceRead type object if the creation was successful
     """
     try:
-        created_vcs_instance = vcs_instance_crud.create_vcs_instance_if_not_exists(db_connection=db_connection,
-                                                                                   vcs_instance=vcs_instance)
+        created_vcs_instance = vcs_instance_crud.create_vcs_instance_if_not_exists(
+            db_connection=db_connection, vcs_instance=vcs_instance
+        )
     except IntegrityError as err:
         logger.debug(f"Error creating new vcs_instance object: {err}")
-        raise HTTPException(status_code=400, detail="Error creating new vcs_instance object") from err
-    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(created_vcs_instance)
+        raise HTTPException(
+            status_code=400, detail="Error creating new vcs_instance object"
+        ) from err
+    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(
+        created_vcs_instance
+    )
 
     # Clear cache related to VCS instances
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_VCS_INSTANCE)
     return vcs_instance
 
 
-@router.get("/{vcs_instance_id}",
-            response_model=vcs_instance_schema.VCSInstanceRead,
-            summary="Fetch a VCS instance by ID",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve VCS Instance <vcs_instance_id>"},
-                404: {"model": Model404, "description": "VCS Instance <vcs_instance_id> not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def read_vcs_instance(vcs_instance_id: int, db_connection: Session = Depends(get_db_connection)) \
-        -> vcs_instance_schema.VCSInstanceRead:
+@router.get(
+    "/{vcs_instance_id}",
+    response_model=vcs_instance_schema.VCSInstanceRead,
+    summary="Fetch a VCS instance by ID",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve VCS Instance <vcs_instance_id>"},
+        404: {
+            "model": Model404,
+            "description": "VCS Instance <vcs_instance_id> not found",
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def read_vcs_instance(
+    vcs_instance_id: int, db_connection: Session = Depends(get_db_connection)
+) -> vcs_instance_schema.VCSInstanceRead:
     """
         Retrieve a VCS instance object based on the provided id
 
     - **db_connection**: Session of the database connection
     - **vcs_instance_id**: ID of the VCS instance for which details need to be fetched
     - **return**: VCSInstanceRead
         The output will contain a VCSInstanceRead type object from the requested ID
     """
-    db_vcs_instance = vcs_instance_crud.get_vcs_instance(db_connection, vcs_instance_id=vcs_instance_id)
+    db_vcs_instance = vcs_instance_crud.get_vcs_instance(
+        db_connection, vcs_instance_id=vcs_instance_id
+    )
     if db_vcs_instance is None:
         raise HTTPException(status_code=404, detail="VCS Instance not found")
-    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(db_vcs_instance)
+    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(
+        db_vcs_instance
+    )
     return vcs_instance
 
 
-@router.get("", response_model=PaginationModel[vcs_instance_schema.VCSInstanceRead],
-            summary="Get all VCS instances",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the VCS Instances"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def get_all_vcs_instances(skip: int = Query(default=0, ge=0),
-                          limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                          vcs_provider_type: Optional[VCSProviders] = Query(None),
-                          vcs_instance_name: Optional[str] = Query(None),
-                          db_connection: Session = Depends(get_db_connection)) \
-        -> PaginationModel[vcs_instance_schema.VCSInstanceRead]:
+@router.get(
+    "",
+    response_model=PaginationModel[vcs_instance_schema.VCSInstanceRead],
+    summary="Get all VCS instances",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Retrieve all the VCS Instances"},
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+def get_all_vcs_instances(
+    skip: int = Query(default=0, ge=0),
+    limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+    vcs_provider_type: Optional[VCSProviders] = Query(None),
+    vcs_instance_name: Optional[str] = Query(None),
+    db_connection: Session = Depends(get_db_connection),
+) -> PaginationModel[vcs_instance_schema.VCSInstanceRead]:
     """
         Retrieve all VCS instance objects paginated
 
     - **db_connection**: Session of the database connection
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **vcs_provider_type**: Optional filter on the VCS provider type
     - **vcs_instance_name**: Optional filter on VCS instance name
     - **return**: [VCSInstanceRead]
         The output will contain a PaginationModel containing the list of VCSInstanceRead type objects,
         or an empty list if no VCS instance was found
     """
-    db_vcs_instances = vcs_instance_crud.get_vcs_instances(db_connection, skip=skip, limit=limit,
-                                                           vcs_provider_type=vcs_provider_type,
-                                                           vcs_instance_name=vcs_instance_name)
+    db_vcs_instances = vcs_instance_crud.get_vcs_instances(
+        db_connection,
+        skip=skip,
+        limit=limit,
+        vcs_provider_type=vcs_provider_type,
+        vcs_instance_name=vcs_instance_name,
+    )
     vcs_instances = []
     for db_vcs_instance in db_vcs_instances:
-        vcs_instances.append(vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(db_vcs_instance))
-
-    total_vcs_instances = vcs_instance_crud.get_vcs_instances_count(db_connection, vcs_provider_type=vcs_provider_type,
-                                                                    vcs_instance_name=vcs_instance_name)
-
-    return PaginationModel[vcs_instance_schema.VCSInstanceRead](data=vcs_instances, total=total_vcs_instances,
-                                                                limit=limit, skip=skip)
-
-
-@router.put("/{vcs_instance_id}",
-            response_model=vcs_instance_schema.VCSInstanceRead,
-            summary="Update an existing VCS instance",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Update VCS Instance <vcs_instance_id>"},
-                404: {"model": Model404, "description": "VCS Instance <vcs_instance_id> not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-async def update_vcs_instance(vcs_instance_id: int, vcs_instance: vcs_instance_schema.VCSInstanceCreate,
-                              db_connection: Session = Depends(get_db_connection)) \
-        -> vcs_instance_schema.VCSInstanceRead:
+        vcs_instances.append(
+            vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(
+                db_vcs_instance
+            )
+        )
+
+    total_vcs_instances = vcs_instance_crud.get_vcs_instances_count(
+        db_connection,
+        vcs_provider_type=vcs_provider_type,
+        vcs_instance_name=vcs_instance_name,
+    )
+
+    return PaginationModel[vcs_instance_schema.VCSInstanceRead](
+        data=vcs_instances, total=total_vcs_instances, limit=limit, skip=skip
+    )
+
+
+@router.put(
+    "/{vcs_instance_id}",
+    response_model=vcs_instance_schema.VCSInstanceRead,
+    summary="Update an existing VCS instance",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Update VCS Instance <vcs_instance_id>"},
+        404: {
+            "model": Model404,
+            "description": "VCS Instance <vcs_instance_id> not found",
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+async def update_vcs_instance(
+    vcs_instance_id: int,
+    vcs_instance: vcs_instance_schema.VCSInstanceCreate,
+    db_connection: Session = Depends(get_db_connection),
+) -> vcs_instance_schema.VCSInstanceRead:
     """
         Update a VCS instance
 
     - **db_connection**: Session of the database connection
     - **vcs_instance_id**: ID of the VCS instance to update
     - **provider_type**: VCS instance name that needs to be updated
     - **hostname**: Host name of the VCS instance that needs to be updated
@@ -152,44 +194,62 @@
     - **scheme**: Scheme of the VCS instance that needs to be updated. Allowed values http or https
     - **exceptions**: List of projects which needs to be updated to exception list, default empty list
     - **scope**: List of projects which needs to be updated to scope
     - **organization**: Name of organization to be updated, default is empty
     - **return**: VCSInstanceRead
         The output will contain a VCSInstanceRead type object with the new properties
     """
-    db_vcs_instance = vcs_instance_crud.get_vcs_instance(db_connection, vcs_instance_id=vcs_instance_id)
+    db_vcs_instance = vcs_instance_crud.get_vcs_instance(
+        db_connection, vcs_instance_id=vcs_instance_id
+    )
     if db_vcs_instance is None:
         raise HTTPException(status_code=404, detail="VCS instance not found")
-    db_vcs_instance = vcs_instance_crud.update_vcs_instance(db_connection=db_connection,
-                                                            vcs_instance_id=vcs_instance_id, vcs_instance=vcs_instance)
-    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(db_vcs_instance)
+    db_vcs_instance = vcs_instance_crud.update_vcs_instance(
+        db_connection=db_connection,
+        vcs_instance_id=vcs_instance_id,
+        vcs_instance=vcs_instance,
+    )
+    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(
+        db_vcs_instance
+    )
 
     # Clear cache related to VCS instances
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_VCS_INSTANCE)
     return vcs_instance
 
 
-@router.delete("/{vcs_instance_id}",
-               summary="Delete a VCS instance",
-               status_code=status.HTTP_200_OK,
-               responses={
-                   200: {"description": "Delete VCS Instance <vcs_instance_id>"},
-                   404: {"model": Model404, "description": "VCS Instance <vcs_instance_id> not found"},
-                   500: {"description": ERROR_MESSAGE_500},
-                   503: {"description": ERROR_MESSAGE_503}
-               })
-async def delete_vcs_instance(vcs_instance_id: int, db_connection: Session = Depends(get_db_connection)):
+@router.delete(
+    "/{vcs_instance_id}",
+    summary="Delete a VCS instance",
+    status_code=status.HTTP_200_OK,
+    responses={
+        200: {"description": "Delete VCS Instance <vcs_instance_id>"},
+        404: {
+            "model": Model404,
+            "description": "VCS Instance <vcs_instance_id> not found",
+        },
+        500: {"description": ERROR_MESSAGE_500},
+        503: {"description": ERROR_MESSAGE_503},
+    },
+)
+async def delete_vcs_instance(
+    vcs_instance_id: int, db_connection: Session = Depends(get_db_connection)
+):
     """
         Delete a VCS instance by ID
 
     - **db_connection**: Session of the database connection
     - **vcs_instance_id**: ID of the VCS instance to delete
     - **return**: The output will contain a success or error message based on the success of the deletion
     """
-    db_vcs_instance = vcs_instance_crud.get_vcs_instance(db_connection, vcs_instance_id=vcs_instance_id)
+    db_vcs_instance = vcs_instance_crud.get_vcs_instance(
+        db_connection, vcs_instance_id=vcs_instance_id
+    )
     if db_vcs_instance is None:
         raise HTTPException(status_code=404, detail="VCS instance not found")
-    vcs_instance_crud.delete_vcs_instance(db_connection, vcs_instance_id=vcs_instance_id, delete_related=True)
+    vcs_instance_crud.delete_vcs_instance(
+        db_connection, vcs_instance_id=vcs_instance_id, delete_related=True
+    )
 
     # Clear cache related to VCS instances
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_VCS_INSTANCE)
     return {"ok": True}
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/filters.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=R0902
 # Standard Library
 from datetime import datetime
 from typing import List
 
 # Third Party
 from pydantic import validator
 from pydantic.dataclasses import dataclass
@@ -27,10 +26,12 @@
     rule_pack_versions: List[str] = None
 
     @validator("end_date_time")
     @classmethod
     def date_range_check(cls, end_date_time: datetime, values: dict):
         if end_date_time and values["start_date_time"]:
             if values["start_date_time"] >= end_date_time:
-                raise ValueError("the start of the date range needs to be prior to the end of it.")
+                raise ValueError(
+                    "the start of the date range needs to be prior to the end of it."
+                )
 
         return end_date_time
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/helpers/exception_handler.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/helpers/exception_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
 # First Party
 from resc_backend.constants import ERROR_MESSAGE_500, ERROR_MESSAGE_503
 
 
 def add_exception_handlers(app: FastAPI):
     @app.exception_handler(RequestValidationError)
-    async def validation_exception_handler(request: Request, exc: RequestValidationError):
+    async def validation_exception_handler(
+        request: Request, exc: RequestValidationError
+    ):
         log_warning(request, exc, "422 Unprocessable Entity")
         return JSONResponse(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             content=jsonable_encoder({"detail": exc.errors(), "body": exc.body}),
         )
 
     @app.exception_handler(ValueError)
@@ -30,22 +32,28 @@
             status_code=status.HTTP_400_BAD_REQUEST,
             content=jsonable_encoder({"detail": exc.errors(), "body": exc.body}),
         )
 
     @app.exception_handler(Exception)
     async def internal_server_error_exception_handler(request: Request, exc: Exception):
         log_error(request, exc, "500 Internal Server Error")
-        return JSONResponse(status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
-                            content={"detail": ERROR_MESSAGE_500})
+        return JSONResponse(
+            status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
+            content={"detail": ERROR_MESSAGE_500},
+        )
 
     @app.exception_handler(OperationalError)
-    async def service_unavailable_exception_handler(request: Request, exc: OperationalError):
+    async def service_unavailable_exception_handler(
+        request: Request, exc: OperationalError
+    ):
         log_error(request, exc, "503 Service Unavailable")
-        return JSONResponse(status_code=status.HTTP_503_SERVICE_UNAVAILABLE,
-                            content={"detail": ERROR_MESSAGE_503})
+        return JSONResponse(
+            status_code=status.HTTP_503_SERVICE_UNAVAILABLE,
+            content={"detail": ERROR_MESSAGE_503},
+        )
 
 
 def log_error(request: Request, exc: Exception, response_status: str):
     """
         Send error details to log file
     :param request:
         Request object for the endpoint
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=no-name-in-module
 # Third Party
 from pydantic import BaseModel
 
 
 class RescResponseModel(BaseModel):
     """
     Generic schema to be used for a response from resc scanner.
@@ -11,33 +10,24 @@
 
 class Model400(RescResponseModel):
     """
     Response schema to be used for a 400 BAD REQUEST.
     """
 
     class Config:
-        schema_extra = {
-            "example": {
-                "detail": "Bad Request"
-            }
-        }
+        schema_extra = {"example": {"detail": "Bad Request"}}
 
 
 class Model404(RescResponseModel):
     """
     Response schema to be used for a 404 NOT FOUND.
     """
 
     class Config:
-        schema_extra = {
-            "example": {
-                "data": {},
-                "detail": "<id> not found"
-            }
-        }
+        schema_extra = {"example": {"data": {}, "detail": "<id> not found"}}
 
 
 class Model409(RescResponseModel):
     """
     Response schema to be used for a 409 CONFLICT.
     """
 
@@ -49,10 +39,8 @@
 
 class Model422(RescResponseModel):
     """
     Response schema to be used for a 422 UNPROCESSABLE ENTITY.
     """
 
     class Config:
-        schema_extra = {
-            "example": {"detail": "Entity cannot be processed"}
-        }
+        schema_extra = {"example": {"detail": "Entity cannot be processed"}}
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/helpers/rule.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/helpers/rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-# pylint: disable=R0912
 # Standard Library
 import logging
 import os
 import re
 from typing import List
 
 # Third Party
 import tomlkit
 from fastapi import File, HTTPException
 from tomlkit import aot, comment, document, nl, table
 from tomlkit.items import String, StringType
 
 # First Party
-from resc_backend.constants import ALLOWED_EXTENSION, TEMP_RULE_FILE, TOML_CUSTOM_DELIMITER
+from resc_backend.constants import (
+    ALLOWED_EXTENSION,
+    TEMP_RULE_FILE,
+    TOML_CUSTOM_DELIMITER,
+)
 from resc_backend.resc_web_service.schema.rule import Rule
 from resc_backend.resc_web_service.schema.rule_allow_list import RuleAllowList
 
 FILE_NAME_REGEX = r"^[a-zA-Z0-9-_]+$"
 
 logger = logging.getLogger(__name__)
 
@@ -73,16 +76,20 @@
     if rule.keywords:
         rule_dict["keywords"] = rule.keywords
     if allow_list_dict:
         rule_dict["allow_list"] = allow_list_dict
     return rule_dict
 
 
-def create_toml_dictionary(rule_pack_version: str, rules: List[str], global_allow_list: List[str], rule_tag_names) \
-        -> dict:
+def create_toml_dictionary(
+    rule_pack_version: str,
+    rules: List[str],
+    global_allow_list: List[str],
+    rule_tag_names,
+) -> dict:
     """
         Create a dictionary for gitleaks toml rule for specified rule pack version, rules and global allow list
     :param rule_pack_version:
         Rule pack version
     :param rules:
         Rule list
     :param global_allow_list:
@@ -94,15 +101,15 @@
     """
     rule_list = []
     for rule in rules:
         allow_list_dict = create_allow_list_dictionary(rule)
         tags_list = [x.name for x in rule_tag_names if x.rule_name == rule.rule_name]
         tags = None
         if len(tags_list) >= 1:
-            tags = ','.join(tags_list)
+            tags = ",".join(tags_list)
         rule_dict = create_rule_dictionary(rule, allow_list_dict, tags)
         rule_list.append(rule_dict)
 
     global_allow_list_dict = create_allow_list_dictionary(global_allow_list)
 
     rule_toml_dict = {"title": "gitleaks config"}
     if rule_pack_version:
@@ -121,31 +128,39 @@
         TOML rule dictionary
     :return: RuleAllowList
         The output will contain an object of RuleAllowList
     """
     global_allow_list_obj = None
     if "allowlist" in toml_rule_dictionary:
         global_allow_list = toml_rule_dictionary.get("allowlist")
-        global_allow_list_obj = map_dictionary_to_rule_allow_list_object(global_allow_list)
+        global_allow_list_obj = map_dictionary_to_rule_allow_list_object(
+            global_allow_list
+        )
     else:
         logger.info("No global allow list is present in the toml file!")
     return global_allow_list_obj
 
 
-def map_dictionary_to_rule_allow_list_object(allow_list_dictionary: dict) -> RuleAllowList:
+def map_dictionary_to_rule_allow_list_object(
+    allow_list_dictionary: dict,
+) -> RuleAllowList:
     """
         Convert allow list dictionary to RuleAllowList object
     :param allow_list_dictionary:
         AllowList dictionary
     :return: RuleAllowList
         The output will contain an object of RuleAllowList
     """
     rule_allow_list = None
     if allow_list_dictionary:
-        description = allow_list_dictionary["description"] if "description" in allow_list_dictionary else None
+        description = (
+            allow_list_dictionary["description"]
+            if "description" in allow_list_dictionary
+            else None
+        )
         regexes = None
         paths = None
         commits = None
         stopwords = None
 
         if "regexes" in allow_list_dictionary:
             regexes = ""
@@ -169,16 +184,21 @@
             commits_array = allow_list_dictionary["commits"]
             commits = ",".join(commits_array)
 
         if "stopwords" in allow_list_dictionary:
             stopword_array = allow_list_dictionary["stopwords"]
             stopwords = ",".join(stopword_array)
 
-        rule_allow_list = RuleAllowList(description=description, regexes=regexes,
-                                        paths=paths, commits=commits, stop_words=stopwords)
+        rule_allow_list = RuleAllowList(
+            description=description,
+            regexes=regexes,
+            paths=paths,
+            commits=commits,
+            stop_words=stopwords,
+        )
     return rule_allow_list
 
 
 def create_toml_rule_file(parsed_toml_dictionary: dict):
     """
         Create a TOML file from a dictionary
     :param parsed_toml_dictionary:
@@ -186,43 +206,50 @@
     :return: toml_file
         Returns toml file
     """
     doc = document()
     doc.add(comment("This is a gitleaks configuration file."))
     doc.add(comment("Rules and allowlists are defined within this file."))
     doc.add(comment("Rules instruct gitleaks on what should be considered a secret."))
-    doc.add(comment("Allowlists instruct gitleaks on what is allowed, i.e. not a secret."))
+    doc.add(
+        comment("Allowlists instruct gitleaks on what is allowed, i.e. not a secret.")
+    )
     doc.add(nl())
 
     if "title" in parsed_toml_dictionary:
         doc.add("title", parsed_toml_dictionary["title"])
     doc.add(nl())
     if "version" in parsed_toml_dictionary:
         doc.add("version", parsed_toml_dictionary["version"])
     doc.add(nl())
 
     # Global allow list table
-    global_allow_list_table = create_allow_list_toml_table(input_dictionary=parsed_toml_dictionary, key="allowlist")
+    global_allow_list_table = create_allow_list_toml_table(
+        input_dictionary=parsed_toml_dictionary, key="allowlist"
+    )
     if global_allow_list_table:
-        doc.add('allowlist', global_allow_list_table)
+        doc.add("allowlist", global_allow_list_table)
         doc.add(nl())
 
     # Rules table
-    rule_array_table = create_rule_array_toml_table(rule_dictionary=parsed_toml_dictionary)
+    rule_array_table = create_rule_array_toml_table(
+        rule_dictionary=parsed_toml_dictionary
+    )
     doc.add("rules", rule_array_table)
 
     toml_string = tomlkit.dumps(doc)
     with open(TEMP_RULE_FILE, "w", encoding="utf-8") as toml_file:
         toml_file.write(toml_string)
         toml_file.close()
     return toml_file
 
 
-def get_multiline_array_for_toml_file(input_dictionary: dict, key: str, string_type: str,
-                                      delimiter: str) -> tomlkit.array():
+def get_multiline_array_for_toml_file(
+    input_dictionary: dict, key: str, string_type: str, delimiter: str
+) -> tomlkit.array():
     """
         Create multiline toml array for the input dictionary value
     :param input_dictionary:
         Input dictionary
     :param key:
         key of Input dictionary
     :param string_type:
@@ -238,59 +265,71 @@
         multiline_array.append(String.from_raw(String.from_raw(value_str), string_type))
         multiline_array.multiline(True)
     return multiline_array
 
 
 def create_allow_list_toml_table(input_dictionary: dict, key: str) -> table():
     """
-       Create a TOML table for rule allow list
-   :param input_dictionary:
-       AllowList dictionary
-    :param key:
-       Key in AllowList dictionary
-   :return: table
-       Returns allow list TOML table
-   """
+        Create a TOML table for rule allow list
+    :param input_dictionary:
+        AllowList dictionary
+     :param key:
+        Key in AllowList dictionary
+    :return: table
+        Returns allow list TOML table
+    """
     allow_list_table = None
     if key in input_dictionary:
         allow_list_table = table()
         allow_list_dict = input_dictionary[key]
         if "description" in allow_list_dict:
             allow_list_table.add("description", allow_list_dict["description"])
         if "paths" in allow_list_dict:
-            multiline_path_array = get_multiline_array_for_toml_file(input_dictionary=allow_list_dict,
-                                                                     key="paths", string_type=StringType.MLL,
-                                                                     delimiter=TOML_CUSTOM_DELIMITER)
+            multiline_path_array = get_multiline_array_for_toml_file(
+                input_dictionary=allow_list_dict,
+                key="paths",
+                string_type=StringType.MLL,
+                delimiter=TOML_CUSTOM_DELIMITER,
+            )
             allow_list_table.add("paths", multiline_path_array)
         if "regexes" in allow_list_dict:
-            multiline_regex_array = get_multiline_array_for_toml_file(input_dictionary=allow_list_dict,
-                                                                      key="regexes", string_type=StringType.MLL,
-                                                                      delimiter=TOML_CUSTOM_DELIMITER)
+            multiline_regex_array = get_multiline_array_for_toml_file(
+                input_dictionary=allow_list_dict,
+                key="regexes",
+                string_type=StringType.MLL,
+                delimiter=TOML_CUSTOM_DELIMITER,
+            )
             allow_list_table.add("regexes", multiline_regex_array)
         if "commits" in allow_list_dict:
-            multiline_commit_array = get_multiline_array_for_toml_file(input_dictionary=allow_list_dict,
-                                                                       key="commits", string_type=StringType.SLB,
-                                                                       delimiter=",")
+            multiline_commit_array = get_multiline_array_for_toml_file(
+                input_dictionary=allow_list_dict,
+                key="commits",
+                string_type=StringType.SLB,
+                delimiter=",",
+            )
             allow_list_table.add("commits", multiline_commit_array)
         if "stop_words" in allow_list_dict:
-            multiline_stopword_array = get_multiline_array_for_toml_file(input_dictionary=allow_list_dict,
-                                                                         key="stop_words", string_type=StringType.SLB,
-                                                                         delimiter=",")
+            multiline_stopword_array = get_multiline_array_for_toml_file(
+                input_dictionary=allow_list_dict,
+                key="stop_words",
+                string_type=StringType.SLB,
+                delimiter=",",
+            )
             allow_list_table.add("stopwords", multiline_stopword_array)
     return allow_list_table
 
 
 def create_rule_array_toml_table(rule_dictionary: dict) -> aot():
     """
-      Create an array of table for rule list
-   :param rule_dictionary:
-       Rule dictionary
-   :return: table
-       Return an array of table
-   """
+       Create an array of table for rule list
+    :param rule_dictionary:
+        Rule dictionary
+    :return: table
+        Return an array of table
+    """
 
     # Rule Table
     rule_array_table = aot()
     if "rules" in rule_dictionary:
         for rule_dict in rule_dictionary["rules"]:
             rule_table = table()
             if "id" in rule_dict:
@@ -298,65 +337,83 @@
             if "description" in rule_dict:
                 rule_table.add("description", rule_dict["description"])
             if "entropy" in rule_dict:
                 rule_table.add("entropy", rule_dict["entropy"])
             if "secret_group" in rule_dict:
                 rule_table.add("secretGroup", rule_dict["secret_group"])
             if "regex" in rule_dict:
-                rule_table.add("regex", String.from_raw(rule_dict["regex"], StringType.MLL))
+                rule_table.add(
+                    "regex", String.from_raw(rule_dict["regex"], StringType.MLL)
+                )
             if "path" in rule_dict:
-                rule_table.add("path", String.from_raw(rule_dict["path"], StringType.MLL))
+                rule_table.add(
+                    "path", String.from_raw(rule_dict["path"], StringType.MLL)
+                )
             if "tags" in rule_dict:
-                multiline_tag_array = get_multiline_array_for_toml_file(input_dictionary=rule_dict,
-                                                                        key="tags",
-                                                                        string_type=StringType.SLB,
-                                                                        delimiter=",")
+                multiline_tag_array = get_multiline_array_for_toml_file(
+                    input_dictionary=rule_dict,
+                    key="tags",
+                    string_type=StringType.SLB,
+                    delimiter=",",
+                )
                 rule_table.add("tags", multiline_tag_array)
             if "keywords" in rule_dict:
-                multiline_keyword_array = get_multiline_array_for_toml_file(input_dictionary=rule_dict,
-                                                                            key="keywords",
-                                                                            string_type=StringType.SLB,
-                                                                            delimiter=",")
+                multiline_keyword_array = get_multiline_array_for_toml_file(
+                    input_dictionary=rule_dict,
+                    key="keywords",
+                    string_type=StringType.SLB,
+                    delimiter=",",
+                )
                 rule_table.add("keywords", multiline_keyword_array)
 
             # Rule Allow List Table
             if "allow_list" in rule_dict:
-                allow_list_table = create_allow_list_toml_table(input_dictionary=rule_dict, key="allow_list")
-                rule_table.append('allowlist', allow_list_table)
+                allow_list_table = create_allow_list_toml_table(
+                    input_dictionary=rule_dict, key="allow_list"
+                )
+                rule_table.append("allowlist", allow_list_table)
 
             rule_array_table.append(rule_table)
     return rule_array_table
 
 
 def validate_uploaded_file_and_read_content(rule_file: File) -> str:
     """
-      Validate the uploaded file and read content
-   :param rule_file:
-       File uploaded
-   :return: content
-       Return file content
-   """
+       Validate the uploaded file and read content
+    :param rule_file:
+        File uploaded
+    :return: content
+        Return file content
+    """
     file_name = os.path.splitext(rule_file.filename)[0]
 
     # File name validation
     is_valid_file_name = bool(re.match(FILE_NAME_REGEX, file_name))
     if not is_valid_file_name:
-        raise HTTPException(500, detail=f"Invalid characters in File name - {file_name}")
+        raise HTTPException(
+            500, detail=f"Invalid characters in File name - {file_name}"
+        )
 
     # File name max length validation
     if len(file_name) > 255:
-        raise HTTPException(500, detail="File name value exceeds maximum length of 255 characters")
+        raise HTTPException(
+            500, detail="File name value exceeds maximum length of 255 characters"
+        )
 
     # File extension validation
-    if rule_file.content_type != "application/octet-stream" or not rule_file.filename.lower().endswith(
-            ALLOWED_EXTENSION):
-        raise HTTPException(500, detail="Invalid document type, only TOML file is supported")
+    if (
+        rule_file.content_type != "application/octet-stream"
+        or not rule_file.filename.lower().endswith(ALLOWED_EXTENSION)
+    ):
+        raise HTTPException(
+            500, detail="Invalid document type, only TOML file is supported"
+        )
 
     # File size validation
     max_size: int = 1000000
     content = rule_file.file.read()
     file_size = len(content)
     if file_size > max_size:
         raise HTTPException(500, detail="File size exceeds the maximum limit 1 MB")
 
-    toml_content = str(content, 'utf-8')
+    toml_content = str(content, "utf-8")
     return toml_content
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/audit.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/audit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=no-name-in-module
 # Standard Library
 import datetime
 from typing import Optional
 
 # Third Party
 from pydantic import BaseModel, conint, conlist, constr
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/detailed_finding.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/detailed_finding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# pylint: disable=no-name-in-module
-# pylint: disable=E0213
-
 # Standard Library
 import datetime
 from typing import Dict, Optional
 
 # Third Party
 from pydantic import BaseModel, HttpUrl, conint, constr, root_validator
 
@@ -42,64 +39,75 @@
 
 
 class DetailedFindingRead(DetailedFinding):
     id_: conint(gt=0)
     commit_url: Optional[constr(min_length=1)]
 
     @staticmethod
-    def build_bitbucket_commit_url(repository_url: str,
-                                   repository_name: str,
-                                   project_key: str,
-                                   file_path: str,
-                                   commit_id: str) -> str:
-
-        arr = repository_url.split('/')
+    def build_bitbucket_commit_url(
+        repository_url: str,
+        repository_name: str,
+        project_key: str,
+        file_path: str,
+        commit_id: str,
+    ) -> str:
+        arr = repository_url.split("/")
         if len(arr) >= 3:
-            repo_base_url = arr[0] + '//' + arr[2]
+            repo_base_url = arr[0] + "//" + arr[2]
         else:
             repo_base_url = repository_url
-        bitbucket_commit_url = f"{repo_base_url}/projects/{project_key}/repos/" \
-                               f"{repository_name}/browse/{file_path}?at={commit_id}"
+        bitbucket_commit_url = (
+            f"{repo_base_url}/projects/{project_key}/repos/"
+            f"{repository_name}/browse/{file_path}?at={commit_id}"
+        )
         commit_url = bitbucket_commit_url
         return commit_url
 
     @staticmethod
-    def build_ado_commit_url(repository_url: str,
-                             file_path: str,
-                             commit_id: str) -> str:
+    def build_ado_commit_url(
+        repository_url: str, file_path: str, commit_id: str
+    ) -> str:
         ado_commit_url = f"{repository_url}/commit/{commit_id}?path=/{file_path}"
         return ado_commit_url
 
     @staticmethod
-    def build_github_commit_url(repository_url: str,
-                                file_path: str,
-                                commit_id: str) -> str:
+    def build_github_commit_url(
+        repository_url: str, file_path: str, commit_id: str
+    ) -> str:
         github_commit_url = f"{repository_url}/commit/{commit_id}?path=/{file_path}"
         return github_commit_url
 
     @root_validator
     def build_commit_url(cls, values) -> Dict:
         if values["status"] is None:
             values["status"] = FindingStatus.NOT_ANALYZED
         if values["comment"] is None:
             values["comment"] = ""
         if values["vcs_provider"] == VCSProviders.BITBUCKET:
-            values["commit_url"] = cls.build_bitbucket_commit_url(repository_url=values["repository_url"],
-                                                                  repository_name=values["repository_name"],
-                                                                  project_key=values["project_key"],
-                                                                  file_path=values["file_path"],
-                                                                  commit_id=values["commit_id"])
+            values["commit_url"] = cls.build_bitbucket_commit_url(
+                repository_url=values["repository_url"],
+                repository_name=values["repository_name"],
+                project_key=values["project_key"],
+                file_path=values["file_path"],
+                commit_id=values["commit_id"],
+            )
         elif values["vcs_provider"] == VCSProviders.AZURE_DEVOPS:
-            values["commit_url"] = cls.build_ado_commit_url(repository_url=values["repository_url"],
-                                                            file_path=values["file_path"],
-                                                            commit_id=values["commit_id"])
+            values["commit_url"] = cls.build_ado_commit_url(
+                repository_url=values["repository_url"],
+                file_path=values["file_path"],
+                commit_id=values["commit_id"],
+            )
 
         elif values["vcs_provider"] == VCSProviders.GITHUB_PUBLIC:
-            values["commit_url"] = cls.build_github_commit_url(repository_url=values["repository_url"],
-                                                               file_path=values["file_path"],
-                                                               commit_id=values["commit_id"])
+            values["commit_url"] = cls.build_github_commit_url(
+                repository_url=values["repository_url"],
+                file_path=values["file_path"],
+                commit_id=values["commit_id"],
+            )
         else:
-            raise NotImplementedError(f"Unsupported VCSProvider: {values['vcs_provider']}")
+            raise NotImplementedError(
+                f"Unsupported VCSProvider: {values['vcs_provider']}"
+            )
         return values
 
     class Config:
         orm_mode = True
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/finding.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/finding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=no-name-in-module
 # Standard Library
 import datetime
 import sys
 from typing import List, Optional
 
 # Third Party
 from pydantic import BaseModel, conint, conlist, constr
@@ -60,9 +59,9 @@
             commit_message=db_finding.commit_message,
             commit_timestamp=db_finding.commit_timestamp,
             author=db_finding.author,
             email=db_finding.email,
             event_sent_on=db_finding.event_sent_on,
             rule_name=db_finding.rule_name,
             repository_id=db_finding.repository_id,
-            scan_ids=scan_ids
+            scan_ids=scan_ids,
         )
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/finding_count_model.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/finding_count_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Standard Library
 from typing import Generic, Optional, TypeVar
 
 # Third Party
-# pylint: disable=no-name-in-module
 from pydantic import BaseModel, conint
 from pydantic.generics import GenericModel
 
 Model = TypeVar("Model", bound=BaseModel)
 
 
 class FindingCountModel(GenericModel, Generic[Model]):
@@ -14,14 +13,15 @@
         Generic encapsulation class for findings count end points to standardize output of the API
         example creation, FindingCountModel[FindingRead](data=db_findings, true_positive=true_positive,
         false_positive=false_positive, not_analyzed=not_analyzed, under_review=under_review,
         clarification_required=clarification_required, total_findings_count=total_findings_count)
     :param Generic[Model]:
         Type of the object in the data list
     """
+
     data: Optional[Model]
     true_positive: conint(gt=-1)
     false_positive: conint(gt=-1)
     not_analyzed: conint(gt=-1)
     under_review: conint(gt=-1)
     clarification_required: conint(gt=-1)
     total_findings_count: conint(gt=-1)
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/pagination_model.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/pagination_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class PaginationModel(GenericModel, Generic[Model]):
     """
         Generic encapsulation class for paginated endpoints to standardize output of the API
         example creation, PaginationModel[FindingRead](data=db_findings, total=total, limit=limit, skip=skip)
     :param Generic[Model]:
         Type of the object in the data list
     """
+
     # data: List[Model]
     data: conlist(item_type=Model, min_items=None, max_items=500)
     total: conint(gt=-1)
     limit: conint(gt=-1)
     skip: conint(gt=-1)
 
     class Config:
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/repository.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable=no-name-in-module
-
 # Third Party
 from pydantic import BaseModel, HttpUrl, conint, constr
 
 
 class RepositoryBase(BaseModel):
     project_key: constr(min_length=1, max_length=100)
     repository_id: constr(min_length=1, max_length=100)
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/repository_enriched.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/repository_enriched.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=no-name-in-module
 # Standard Library
 import datetime
 
 # Third Party
 from pydantic import BaseModel, HttpUrl, conint, constr
 
 # First Party
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/rule.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/rule.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=no-name-in-module
 # Standard Library
 from typing import Optional
 
 # Third Party
 from pydantic import BaseModel, conint, constr
 
 
@@ -13,19 +12,21 @@
     secret_group: Optional[int] = None
     regex: Optional[str] = None
     path: Optional[str] = None
     keywords: Optional[str] = None
 
 
 class RuleCreate(RuleBase):
-    rule_pack: constr(regex=r'^(\d+\.)?(\d+\.)?(\*|\d+)$')
+    rule_pack: constr(regex=r"^(\d+\.)?(\d+\.)?(\*|\d+)$")
     allow_list: Optional[conint(gt=0)] = None
 
     @classmethod
-    def create_from_base_class(cls, base_object: RuleBase, rule_pack: str, allow_list=int):
+    def create_from_base_class(
+        cls, base_object: RuleBase, rule_pack: str, allow_list=int
+    ):
         return cls(**(dict(base_object)), rule_pack=rule_pack, allow_list=allow_list)
 
 
 class Rule(RuleBase):
     pass
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/rule_allow_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=no-name-in-module
 # Standard Library
 from typing import Optional
 
 # Third Party
 from pydantic import BaseModel, conint, constr
 
 
@@ -11,15 +10,14 @@
     regexes: Optional[str]
     paths: Optional[str]
     commits: Optional[str]
     stop_words: Optional[str]
 
 
 class RuleAllowListCreate(RuleAllowListBase):
-
     @classmethod
     def create_from_base_class(cls, base_object: RuleAllowListBase):
         return cls(**(dict(base_object)))
 
 
 class RuleAllowList(RuleAllowListBase):
     pass
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/rule_pack.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/rule_pack.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=no-name-in-module
 # Standard Library
 import datetime
 from typing import Optional
 
 # Third Party
 from pydantic import BaseModel, conint, constr
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/scan.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=no-name-in-module
 # Standard Library
 import datetime
 
 # Third Party
 from pydantic import BaseModel, conint, constr
 
 # First Party
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service/schema/vcs_instance.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service/schema/vcs_instance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=no-name-in-module
 # Standard Library
 from typing import Optional
 
 # Third Party
 from pydantic import BaseModel, conint, conlist, constr, validator
 
 # First Party
@@ -21,30 +20,36 @@
     organization: Optional[constr(max_length=200)]
 
     @validator("scheme", pre=True)
     @classmethod
     def check_scheme(cls, value):
         allowed_schemes = ["http", "https"]
         if value not in allowed_schemes:
-            raise ValueError(f"The scheme '{value}' must be one of the following {', '.join(allowed_schemes)}")
+            raise ValueError(
+                f"The scheme '{value}' must be one of the following {', '.join(allowed_schemes)}"
+            )
         return value
 
     @validator("organization", pre=True)
     @classmethod
     def check_organization(cls, value, values):
         if not value and values.get("provider_type", None) == AZURE_DEVOPS:
-            raise ValueError("The organization field needs to be specified for Azure devops vcs instances")
+            raise ValueError(
+                "The organization field needs to be specified for Azure devops vcs instances"
+            )
         return value
 
     @validator("scope", pre=True)
     @classmethod
     def check_scope_and_exceptions(cls, value, values):
         if value and values.get("exceptions", None):
-            raise ValueError("You cannot specify bot the scope and exceptions to the scan, only one setting"
-                             " is supported.")
+            raise ValueError(
+                "You cannot specify bot the scope and exceptions to the scan, only one setting"
+                " is supported."
+            )
         return value
 
 
 class VCSInstanceCreate(VCSInstanceBase):
     pass
 
 
@@ -56,21 +61,23 @@
         exceptions = []
         scope = []
         if db_vcs_instance.exceptions:
             exceptions = db_vcs_instance.exceptions.split(",")
         if db_vcs_instance.scope:
             scope = db_vcs_instance.scope.split(",")
 
-        vcs_instance_read = cls(id_=db_vcs_instance.id_,
-                                name=db_vcs_instance.name,
-                                provider_type=db_vcs_instance.provider_type,
-                                hostname=db_vcs_instance.hostname,
-                                port=db_vcs_instance.port,
-                                scheme=db_vcs_instance.scheme,
-                                exceptions=exceptions,
-                                scope=scope,
-                                organization=db_vcs_instance.organization)
+        vcs_instance_read = cls(
+            id_=db_vcs_instance.id_,
+            name=db_vcs_instance.name,
+            provider_type=db_vcs_instance.provider_type,
+            hostname=db_vcs_instance.hostname,
+            port=db_vcs_instance.port,
+            scheme=db_vcs_instance.scheme,
+            exceptions=exceptions,
+            scope=scope,
+            organization=db_vcs_instance.organization,
+        )
 
         return vcs_instance_read
 
     class Config:
         orm_mode = True
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service_interface/findings.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service_interface/findings.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,33 +3,45 @@
 import logging
 from typing import List
 
 # Third Party
 import requests
 
 # First Party
-from resc_backend.constants import RWS_ROUTE_FINDINGS, RWS_ROUTE_SCANS, RWS_VERSION_PREFIX
+from resc_backend.constants import (
+    RWS_ROUTE_FINDINGS,
+    RWS_ROUTE_SCANS,
+    RWS_VERSION_PREFIX,
+)
 from resc_backend.resc_web_service.schema.finding import FindingCreate
 
 logger = logging.getLogger(__name__)
 
 
 def create_findings(url: str, findings: List[FindingCreate]) -> requests.Response:
     api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_FINDINGS}"
 
     findings_json = []
     for finding in findings:
         findings_json.append(json.loads(finding.json()))
 
-    response = requests.post(api_url, json=findings_json, proxies={"http": "", "https": ""}, timeout=10)
+    response = requests.post(
+        api_url, json=findings_json, proxies={"http": "", "https": ""}, timeout=10
+    )
     return response
 
 
-def create_findings_with_scan_id(url: str, findings: List[FindingCreate], scan_id: int) -> requests.Response:
-    api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_SCANS}/{scan_id}{RWS_ROUTE_FINDINGS}"
+def create_findings_with_scan_id(
+    url: str, findings: List[FindingCreate], scan_id: int
+) -> requests.Response:
+    api_url = (
+        f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_SCANS}/{scan_id}{RWS_ROUTE_FINDINGS}"
+    )
 
     findings_json = []
     for finding in findings:
         findings_json.append(json.loads(finding.json()))
 
-    response = requests.post(api_url, json=findings_json, proxies={"http": "", "https": ""}, timeout=10)
+    response = requests.post(
+        api_url, json=findings_json, proxies={"http": "", "https": ""}, timeout=10
+    )
     return response
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service_interface/repositories.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service_interface/repositories.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # Standard Library
 import logging
 
 # Third Party
 import requests
 
 # First Party
-from resc_backend.constants import RWS_ROUTE_LAST_SCAN, RWS_ROUTE_REPOSITORIES, RWS_VERSION_PREFIX
+from resc_backend.constants import (
+    RWS_ROUTE_LAST_SCAN,
+    RWS_ROUTE_REPOSITORIES,
+    RWS_VERSION_PREFIX,
+)
 from resc_backend.resc_web_service.schema.repository import Repository
 
 logger = logging.getLogger(__name__)
 
 
 def create_repository(url: str, repository: Repository):
     api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_REPOSITORIES}"
-    response = requests.post(api_url, data=repository.json(), proxies={"http": "", "https": ""}, timeout=10)
+    response = requests.post(
+        api_url, data=repository.json(), proxies={"http": "", "https": ""}, timeout=10
+    )
     return response
 
 
 def get_last_scan_for_repository(url: str, repository_id: int):
     api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_REPOSITORIES}/{repository_id}{RWS_ROUTE_LAST_SCAN}"
     response = requests.get(api_url, proxies={"http": "", "https": ""}, timeout=10)
     return response
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service_interface/rule_packs.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service_interface/rule_packs.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,44 +3,71 @@
 from typing import Optional
 
 # Third Party
 import requests
 from requests import Response
 
 # First Party
-from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, RWS_ROUTE_RULE_PACKS, RWS_VERSION_PREFIX
+from resc_backend.constants import (
+    DEFAULT_RECORDS_PER_PAGE_LIMIT,
+    RWS_ROUTE_RULE_PACKS,
+    RWS_VERSION_PREFIX,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def upload_rule_pack_toml_file(url: str, rule_file_path: str):
     with open(rule_file_path, "rb") as toml_file:
-        files = {"rule_file": ("RESC-SECRETS-RULE.toml", toml_file, "application/octet-stream")}
-        response = requests.post(url=url, files=files, proxies={"http": "", "https": ""}, timeout=10)
+        files = {
+            "rule_file": (
+                "RESC-SECRETS-RULE.toml",
+                toml_file,
+                "application/octet-stream",
+            )
+        }
+        response = requests.post(
+            url=url, files=files, proxies={"http": "", "https": ""}, timeout=10
+        )
         toml_file.close()
     return response
 
 
-def download_rule_pack_toml_file(rws_url: str, rule_pack_version: Optional[str] = "") -> Response:
+def download_rule_pack_toml_file(
+    rws_url: str, rule_pack_version: Optional[str] = ""
+) -> Response:
     params = {}
     if rule_pack_version:
         params = {"rule_pack_version": rule_pack_version}
-    response = requests.get(url=f"{rws_url}{RWS_VERSION_PREFIX}{RWS_ROUTE_RULE_PACKS}",
-                            params=params, timeout=10)
+    response = requests.get(
+        url=f"{rws_url}{RWS_VERSION_PREFIX}{RWS_ROUTE_RULE_PACKS}",
+        params=params,
+        timeout=10,
+    )
 
     if response.status_code == 200:
         logger.debug(
-            f"Rule pack version: {rule_pack_version} has been successfully downloaded")
+            f"Rule pack version: {rule_pack_version} has been successfully downloaded"
+        )
     else:
-        logger.error(f"Downloading rule pack version {rule_pack_version} failed with "
-                     f"error: {response.status_code}->{response.text}")
+        logger.error(
+            f"Downloading rule pack version {rule_pack_version} failed with "
+            f"error: {response.status_code}->{response.text}"
+        )
     return response
 
 
-def get_rule_packs(url: str, version: Optional[str] = None, active: Optional[bool] = None, skip: Optional[int] = 0,
-                   limit: Optional[int] = DEFAULT_RECORDS_PER_PAGE_LIMIT):
+def get_rule_packs(
+    url: str,
+    version: Optional[str] = None,
+    active: Optional[bool] = None,
+    skip: Optional[int] = 0,
+    limit: Optional[int] = DEFAULT_RECORDS_PER_PAGE_LIMIT,
+):
     api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_RULE_PACKS}/versions"
     params = {"active": active, "skip": skip, "limit": limit}
     if version:
         params["version"] = version
-    response = requests.get(api_url, params=params, proxies={"http": "", "https": ""}, timeout=10)
+    response = requests.get(
+        api_url, params=params, proxies={"http": "", "https": ""}, timeout=10
+    )
     return response
```

### Comparing `resc_backend-3.0.0/src/resc_backend/resc_web_service_interface/vcs_instances.py` & `resc_backend-3.0.1/src/resc_backend/resc_web_service_interface/vcs_instances.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,9 +9,11 @@
 from resc_backend.resc_web_service.schema.vcs_instance import VCSInstanceCreate
 
 logger = logging.getLogger(__name__)
 
 
 def create_vcs_instance(url: str, vcs_instance: VCSInstanceCreate):
     api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_VCS}"
-    response = requests.post(api_url, data=vcs_instance.json(), proxies={"http": "", "https": ""}, timeout=10)
+    response = requests.post(
+        api_url, data=vcs_instance.json(), proxies={"http": "", "https": ""}, timeout=10
+    )
     return response
```

### Comparing `resc_backend-3.0.0/src/resc_backend.egg-info/SOURCES.txt` & `resc_backend-3.0.1/src/resc_backend.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE.md
-README.md
+requirements.txt
 setup.cfg
 setup.py
 src/resc_backend/__init__.py
 src/resc_backend/common.py
 src/resc_backend/constants.py
 src/resc_backend.egg-info/PKG-INFO
 src/resc_backend.egg-info/SOURCES.txt
@@ -12,14 +12,15 @@
 src/resc_backend.egg-info/not-zip-safe
 src/resc_backend.egg-info/requires.txt
 src/resc_backend.egg-info/top_level.txt
 src/resc_backend/bin/__init__.py
 src/resc_backend/bin/rabbitmq_bootup.py
 src/resc_backend/db/__init__.py
 src/resc_backend/db/connection.py
+src/resc_backend/db/engine_azure.py
 src/resc_backend/db/model/__init__.py
 src/resc_backend/db/model/audit.py
 src/resc_backend/db/model/finding.py
 src/resc_backend/db/model/repository.py
 src/resc_backend/db/model/rule.py
 src/resc_backend/db/model/rule_allow_list.py
 src/resc_backend/db/model/rule_pack.py
@@ -27,15 +28,14 @@
 src/resc_backend/db/model/scan.py
 src/resc_backend/db/model/scan_finding.py
 src/resc_backend/db/model/tag.py
 src/resc_backend/db/model/vcs_instance.py
 src/resc_backend/helpers/__init__.py
 src/resc_backend/helpers/dict_remapper.py
 src/resc_backend/helpers/environment_wrapper.py
-src/resc_backend/helpers/git_operation.py
 src/resc_backend/helpers/rabbitmq/__init__.py
 src/resc_backend/helpers/rabbitmq/configuration.py
 src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
 src/resc_backend/resc_web_service/__init__.py
 src/resc_backend/resc_web_service/api.py
 src/resc_backend/resc_web_service/cache_manager.py
 src/resc_backend/resc_web_service/configuration.py
```

