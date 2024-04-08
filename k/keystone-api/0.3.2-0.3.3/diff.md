# Comparing `tmp/keystone_api-0.3.2.tar.gz` & `tmp/keystone_api-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystone_api-0.3.2.tar", max compression
+gzip compressed data, was "keystone_api-0.3.3.tar", max compression
```

## Comparing `keystone_api-0.3.2.tar` & `keystone_api-0.3.3.tar`

### file list

```diff
@@ -1,110 +1,111 @@
--rw-r--r--   0        0        0    13578 2024-04-01 21:46:47.669141 keystone_api-0.3.2/README.md
--rw-r--r--   0        0        0      428 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/__init__.py
--rw-r--r--   0        0        0     2619 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/clean.py
--rw-r--r--   0        0        0     2820 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
--rw-r--r--   0        0        0      471 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
--rw-r--r--   0        0        0     3479 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/quickstart.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/tests/__init__.py
--rw-r--r--   0        0        0      625 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/tests/test_managment.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/__init__.py
--rw-r--r--   0        0        0     4543 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/admin.py
--rw-r--r--   0        0        0     2173 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/managers.py
--rw-r--r--   0        0        0     3420 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0001_initial.py
--rw-r--r--   0        0        0     1298 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0002_initial.py
--rw-r--r--   0        0        0     1063 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/migrations/__init__.py
--rw-r--r--   0        0        0     4837 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/models.py
--rw-r--r--   0        0        0     3347 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/permissions.py
--rw-r--r--   0        0        0     1917 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/serializers.py
--rw-r--r--   0        0        0     4324 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/tasks.py
--rw-r--r--   0        0        0      516 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/allocations/urls.py
--rw-r--r--   0        0        0     3246 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/allocations/views.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/authentication/__init__.py
--rw-r--r--   0        0        0      346 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/authentication/urls.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/docs/__init__.py
--rw-r--r--   0        0        0      337 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/docs/urls.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/health/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/health/tests/__init__.py
--rw-r--r--   0        0        0     3199 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/health/tests/test_views.py
--rw-r--r--   0        0        0      244 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/health/urls.py
--rw-r--r--   0        0        0     2066 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/health/views.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/__init__.py
--rw-r--r--   0        0        0     1344 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/handlers.py
--rw-r--r--   0        0        0     1759 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/middleware.py
--rw-r--r--   0        0        0     1959 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/migrations/__init__.py
--rw-r--r--   0        0        0     1469 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/models.py
--rw-r--r--   0        0        0      868 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/serializers.py
--rw-r--r--   0        0        0      709 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/tasks.py
--rw-r--r--   0        0        0      278 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/urls.py
--rw-r--r--   0        0        0      949 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/views.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/__init__.py
--rw-r--r--   0        0        0     1518 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/admin.py
--rw-r--r--   0        0        0     1758 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/migrations/__init__.py
--rw-r--r--   0        0        0     1661 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/models.py
--rw-r--r--   0        0        0      868 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/serializers.py
--rw-r--r--   0        0        0      296 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/urls.py
--rw-r--r--   0        0        0      804 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/views.py
--rw-r--r--   0        0        0      141 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/scheduler/__init__.py
--rw-r--r--   0        0        0     1029 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/scheduler/admin.py
--rw-r--r--   0        0        0     1096 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/scheduler/celery.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/__init__.py
--rw-r--r--   0        0        0     1307 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/admin.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/management/commands/__init__.py
--rw-r--r--   0        0        0     1056 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/management/commands/ldap_update.py
--rw-r--r--   0        0        0     3134 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/managers.py
--rw-r--r--   0        0        0     3018 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/migrations/0001_initial.py
--rw-r--r--   0        0        0      405 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/migrations/__init__.py
--rw-r--r--   0        0        0     2370 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/models.py
--rw-r--r--   0        0        0      913 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/permissions.py
--rw-r--r--   0        0        0      887 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/serializers.py
--rw-r--r--   0        0        0     2102 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tasks.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_managers/__init__.py
--rw-r--r--   0        0        0     1374 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
--rw-r--r--   0        0        0     2399 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_managers/test_UserManager.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_models/__init__.py
--rw-r--r--   0        0        0     3210 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
--rw-r--r--   0        0        0      471 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_models/test_User.py
--rw-r--r--   0        0        0      748 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/utils.py
--rw-r--r--   0        0        0      329 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/urls.py
--rw-r--r--   0        0        0     1329 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/views.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/main/__init__.py
--rw-r--r--   0        0        0      169 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/main/asgi.py
--rw-r--r--   0        0        0     7768 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/main/settings.py
--rw-r--r--   0        0        0     1002 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/main/urls.py
--rw-r--r--   0        0        0      168 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/main/wsgi.py
--rwxr-xr-x   0        0        0      556 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/manage.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/plugins/__init__.py
--rw-r--r--   0        0        0     4728 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/plugins/slurm.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/__init__.py
--rw-r--r--   0        0        0     2923 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_allocations.py
--rw-r--r--   0        0        0     4229 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_allocations_pk.py
--rw-r--r--   0        0        0     2929 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_clusters.py
--rw-r--r--   0        0        0     3104 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_clusters_pk.py
--rw-r--r--   0        0        0     5631 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_requests.py
--rw-r--r--   0        0        0     5351 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_requests_pk.py
--rw-r--r--   0        0        0     2898 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_reviews.py
--rw-r--r--   0        0        0     4202 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_reviews_pk.py
--rw-r--r--   0        0        0     3015 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/fixtures/multi_research_group.yaml
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/health/__init__.py
--rw-r--r--   0        0        0     3102 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/health/test.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/logging/__init__.py
--rw-r--r--   0        0        0     2871 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/logging/test_apps.py
--rw-r--r--   0        0        0     2879 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/logging/test_requests.py
--rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/users/__init__.py
--rw-r--r--   0        0        0     2981 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/users/test_researchgroups.py
--rw-r--r--   0        0        0     4244 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/users/test_researchgroups_pk.py
--rw-r--r--   0        0        0     2964 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/users/test_users.py
--rw-r--r--   0        0        0     4471 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/users/test_users_pk.py
--rw-r--r--   0        0        0     2014 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/utils.py
--rw-r--r--   0        0        0      958 2024-04-01 21:47:02.201265 keystone_api-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    14780 1970-01-01 00:00:00.000000 keystone_api-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    13578 2024-04-08 17:43:08.833383 keystone_api-0.3.3/README.md
+-rw-r--r--   0        0        0      428 2024-04-08 17:43:08.833383 keystone_api-0.3.3/keystone_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/__init__.py
+-rw-r--r--   0        0        0     2619 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/clean.py
+-rw-r--r--   0        0        0     2820 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
+-rw-r--r--   0        0        0      471 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
+-rw-r--r--   0        0        0     3479 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/quickstart.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/tests/__init__.py
+-rw-r--r--   0        0        0      625 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/tests/test_managment.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/__init__.py
+-rw-r--r--   0        0        0     4543 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/admin.py
+-rw-r--r--   0        0        0     2173 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/managers.py
+-rw-r--r--   0        0        0     3420 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1298 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0002_initial.py
+-rw-r--r--   0        0        0     1063 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/migrations/__init__.py
+-rw-r--r--   0        0        0     4837 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/models.py
+-rw-r--r--   0        0        0     3347 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/permissions.py
+-rw-r--r--   0        0        0     1917 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/serializers.py
+-rw-r--r--   0        0        0     4324 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/tasks.py
+-rw-r--r--   0        0        0      516 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/urls.py
+-rw-r--r--   0        0        0     3246 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/views.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/authentication/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/authentication/tasks.py
+-rw-r--r--   0        0        0      444 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/authentication/urls.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/docs/__init__.py
+-rw-r--r--   0        0        0      337 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/docs/urls.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/health/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/health/tests/__init__.py
+-rw-r--r--   0        0        0     3199 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/health/tests/test_views.py
+-rw-r--r--   0        0        0      244 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/health/urls.py
+-rw-r--r--   0        0        0     2066 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/health/views.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/__init__.py
+-rw-r--r--   0        0        0     1344 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/handlers.py
+-rw-r--r--   0        0        0     1759 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/middleware.py
+-rw-r--r--   0        0        0     1959 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/migrations/__init__.py
+-rw-r--r--   0        0        0     1469 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/models.py
+-rw-r--r--   0        0        0      868 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/serializers.py
+-rw-r--r--   0        0        0      709 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/tasks.py
+-rw-r--r--   0        0        0      278 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/urls.py
+-rw-r--r--   0        0        0      949 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/views.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/__init__.py
+-rw-r--r--   0        0        0     1518 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/admin.py
+-rw-r--r--   0        0        0     1758 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/migrations/__init__.py
+-rw-r--r--   0        0        0     1661 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/models.py
+-rw-r--r--   0        0        0      868 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/serializers.py
+-rw-r--r--   0        0        0      296 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/urls.py
+-rw-r--r--   0        0        0      804 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/views.py
+-rw-r--r--   0        0        0      141 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/scheduler/__init__.py
+-rw-r--r--   0        0        0     1029 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/scheduler/admin.py
+-rw-r--r--   0        0        0     1344 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/scheduler/celery.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/__init__.py
+-rw-r--r--   0        0        0     1307 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/admin.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/management/commands/__init__.py
+-rw-r--r--   0        0        0     1056 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/management/commands/ldap_update.py
+-rw-r--r--   0        0        0     3134 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/managers.py
+-rw-r--r--   0        0        0     3018 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/migrations/0001_initial.py
+-rw-r--r--   0        0        0      405 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/migrations/__init__.py
+-rw-r--r--   0        0        0     2370 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/models.py
+-rw-r--r--   0        0        0      913 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/permissions.py
+-rw-r--r--   0        0        0      887 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/serializers.py
+-rw-r--r--   0        0        0     2095 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_managers/__init__.py
+-rw-r--r--   0        0        0     1374 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
+-rw-r--r--   0        0        0     2399 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_managers/test_UserManager.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_models/__init__.py
+-rw-r--r--   0        0        0     3210 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
+-rw-r--r--   0        0        0      471 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_models/test_User.py
+-rw-r--r--   0        0        0      748 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/utils.py
+-rw-r--r--   0        0        0      329 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/urls.py
+-rw-r--r--   0        0        0     1329 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/views.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/main/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/main/asgi.py
+-rw-r--r--   0        0        0     7865 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/main/settings.py
+-rw-r--r--   0        0        0     1002 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/main/urls.py
+-rw-r--r--   0        0        0      168 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/main/wsgi.py
+-rwxr-xr-x   0        0        0      556 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/manage.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/plugins/__init__.py
+-rw-r--r--   0        0        0     4728 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/plugins/slurm.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/__init__.py
+-rw-r--r--   0        0        0     2923 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_allocations.py
+-rw-r--r--   0        0        0     4229 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_allocations_pk.py
+-rw-r--r--   0        0        0     2929 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_clusters.py
+-rw-r--r--   0        0        0     3104 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_clusters_pk.py
+-rw-r--r--   0        0        0     5631 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_requests.py
+-rw-r--r--   0        0        0     5351 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_requests_pk.py
+-rw-r--r--   0        0        0     2898 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/allocations/test_reviews.py
+-rw-r--r--   0        0        0     4202 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/allocations/test_reviews_pk.py
+-rw-r--r--   0        0        0     3015 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/fixtures/multi_research_group.yaml
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/health/__init__.py
+-rw-r--r--   0        0        0     3102 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/health/test.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/logging/__init__.py
+-rw-r--r--   0        0        0     2871 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/logging/test_apps.py
+-rw-r--r--   0        0        0     2879 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/logging/test_requests.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/users/__init__.py
+-rw-r--r--   0        0        0     2981 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/users/test_researchgroups.py
+-rw-r--r--   0        0        0     4244 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/users/test_researchgroups_pk.py
+-rw-r--r--   0        0        0     2964 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/users/test_users.py
+-rw-r--r--   0        0        0     4471 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/users/test_users_pk.py
+-rw-r--r--   0        0        0     2014 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/utils.py
+-rw-r--r--   0        0        0      957 2024-04-08 17:43:29.901483 keystone_api-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    14773 1970-01-01 00:00:00.000000 keystone_api-0.3.3/PKG-INFO
```

### Comparing `keystone_api-0.3.2/README.md` & `keystone_api-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/clean.py` & `keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/clean.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py` & `keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/quickstart.py` & `keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/quickstart.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/admin_utils/tests/test_managment.py` & `keystone_api-0.3.3/keystone_api/apps/admin_utils/tests/test_managment.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/allocations/admin.py` & `keystone_api-0.3.3/keystone_api/apps/allocations/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/allocations/managers.py` & `keystone_api-0.3.3/keystone_api/apps/allocations/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0001_initial.py` & `keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0002_initial.py` & `keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py` & `keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/allocations/models.py` & `keystone_api-0.3.3/keystone_api/apps/allocations/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/allocations/permissions.py` & `keystone_api-0.3.3/keystone_api/apps/allocations/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/allocations/serializers.py` & `keystone_api-0.3.3/keystone_api/apps/allocations/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/allocations/tasks.py` & `keystone_api-0.3.3/keystone_api/apps/allocations/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/allocations/urls.py` & `keystone_api-0.3.3/keystone_api/apps/allocations/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/allocations/views.py` & `keystone_api-0.3.3/keystone_api/apps/allocations/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/health/tests/test_views.py` & `keystone_api-0.3.3/keystone_api/apps/health/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/health/views.py` & `keystone_api-0.3.3/keystone_api/apps/health/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/logging/handlers.py` & `keystone_api-0.3.3/keystone_api/apps/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/logging/middleware.py` & `keystone_api-0.3.3/keystone_api/apps/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/logging/migrations/0001_initial.py` & `keystone_api-0.3.3/keystone_api/apps/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/logging/models.py` & `keystone_api-0.3.3/keystone_api/apps/logging/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/logging/serializers.py` & `keystone_api-0.3.3/keystone_api/apps/logging/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/logging/tasks.py` & `keystone_api-0.3.3/keystone_api/apps/logging/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/logging/views.py` & `keystone_api-0.3.3/keystone_api/apps/logging/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/research_products/admin.py` & `keystone_api-0.3.3/keystone_api/apps/research_products/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/research_products/migrations/0001_initial.py` & `keystone_api-0.3.3/keystone_api/apps/research_products/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/research_products/models.py` & `keystone_api-0.3.3/keystone_api/apps/research_products/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/research_products/serializers.py` & `keystone_api-0.3.3/keystone_api/apps/research_products/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/research_products/views.py` & `keystone_api-0.3.3/keystone_api/apps/research_products/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/scheduler/admin.py` & `keystone_api-0.3.3/keystone_api/apps/scheduler/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/scheduler/celery.py` & `keystone_api-0.3.3/keystone_api/apps/scheduler/celery.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,9 +19,14 @@
         'schedule': crontab(minute='0'),
         'description': 'This task synchronizes user data against LDAP. If LDAP authentication is not being used, this task does nothing.'
     },
     'apps.logging.tasks.rotate_log_files': {
         'task': 'apps.logging.tasks.rotate_log_files',
         'schedule': crontab(hour='0', minute='0'),
         'description': 'This task deletes old log entries according to application settings.'
-    }
+    },
+    'apps.authentication.tasks.flush_expired_tokens': {
+        'task': 'apps.authentication.tasks.flush_expired_tokens',
+        'schedule': crontab(hour='0', minute='0'),
+        'description': 'This task clears the JWT token blacklist.'
+    },
 }
```

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/admin.py` & `keystone_api-0.3.3/keystone_api/apps/users/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/management/commands/ldap_update.py` & `keystone_api-0.3.3/keystone_api/apps/users/management/commands/ldap_update.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/managers.py` & `keystone_api-0.3.3/keystone_api/apps/users/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/migrations/0001_initial.py` & `keystone_api-0.3.3/keystone_api/apps/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/models.py` & `keystone_api-0.3.3/keystone_api/apps/users/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/permissions.py` & `keystone_api-0.3.3/keystone_api/apps/users/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/serializers.py` & `keystone_api-0.3.3/keystone_api/apps/users/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/tasks.py` & `keystone_api-0.3.3/keystone_api/apps/users/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     search = conn.search_s(settings.AUTH_LDAP_USER_SEARCH.base_dn, ldap.SCOPE_SUBTREE, '(objectClass=account)')
 
     # Fetch keystone usernames using the LDAP attribute map defined in settings
     ldap_username_attr = settings.AUTH_LDAP_USER_ATTR_MAP.get('username', 'uid')
     ldap_names = {uid.decode() for result in search for uid in result[1][ldap_username_attr]}
 
     for username in tqdm(ldap_names):
-        LDAPBackend().populate_user(username)
-        user = User.objects.get(username=username)
-        user.is_ldap_user = True
-        user.save()
+        user = LDAPBackend().populate_user(username)
+        if user is not None:
+            user.is_ldap_user = True
+            user.save()
 
     if prune:
         usernames = set(User.objects.filter(is_ldap=True).values_list('username', flat=True))
         users_to_delete = usernames - ldap_names
         User.objects.filter(username__in=users_to_delete).delete()
```

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py` & `keystone_api-0.3.3/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/tests/test_managers/test_UserManager.py` & `keystone_api-0.3.3/keystone_api/apps/users/tests/test_managers/test_UserManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py` & `keystone_api-0.3.3/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/tests/utils.py` & `keystone_api-0.3.3/keystone_api/apps/users/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/apps/users/views.py` & `keystone_api-0.3.3/keystone_api/apps/users/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/main/settings.py` & `keystone_api-0.3.3/keystone_api/main/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     'health_check.db',
     'health_check.storage',
     'health_check.contrib.migrations',
     'health_check.contrib.celery',
     'health_check.contrib.celery_ping',
     'health_check.contrib.redis',
     'rest_framework',
+    'rest_framework_simplejwt.token_blacklist',
     'django_celery_beat',
     'django_celery_results',
     'django_filters',
     'drf_spectacular',
     'apps.admin_utils',
     'apps.allocations',
     'apps.docs',
@@ -107,15 +108,15 @@
 
 # Base styling for the Admin UI
 
 JAZZMIN_SETTINGS = {
     "site_title": "Keystone",
     "site_header": "Keystone",
     "site_brand": "Keystone",
-    "hide_apps": ["sites", "auth"],
+    "hide_apps": ["sites", "auth", "token_blacklist"],
     "order_with_respect_to": [
         "users",
         "allocations",
         "research_products",
         "sites"
     ],
     "icons": {},
@@ -163,16 +164,17 @@
 _redis_port = env.int('REDIS_PORT', 6379)
 _redis_db = env.int('REDIS_DB', 0)
 _redis_pass = env.str('REDIS_PASSWORD', '')
 
 REDIS_URL = f'redis://:{_redis_pass}@{_redis_host}:{_redis_port}'
 
 CELERY_BROKER_URL = REDIS_URL + f'/{_redis_db}'
-CELERY_RESULT_BACKEND = 'django-db'
 CELERY_CACHE_BACKEND = 'django-cache'
+CELERY_RESULT_BACKEND = 'django-db'
+CELERY_RESULT_EXTENDED = True
 
 # Database
 
 DATABASES = dict()
 DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
 
 _db_name = env.str('DB_NAME', 'keystone')
```

### Comparing `keystone_api-0.3.2/keystone_api/main/urls.py` & `keystone_api-0.3.3/keystone_api/main/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/manage.py` & `keystone_api-0.3.3/keystone_api/manage.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/plugins/slurm.py` & `keystone_api-0.3.3/keystone_api/plugins/slurm.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/allocations/test_allocations.py` & `keystone_api-0.3.3/keystone_api/tests/allocations/test_allocations.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/allocations/test_allocations_pk.py` & `keystone_api-0.3.3/keystone_api/tests/allocations/test_allocations_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/allocations/test_clusters.py` & `keystone_api-0.3.3/keystone_api/tests/allocations/test_clusters.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/allocations/test_clusters_pk.py` & `keystone_api-0.3.3/keystone_api/tests/allocations/test_clusters_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/allocations/test_requests.py` & `keystone_api-0.3.3/keystone_api/tests/allocations/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/allocations/test_requests_pk.py` & `keystone_api-0.3.3/keystone_api/tests/allocations/test_requests_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/allocations/test_reviews.py` & `keystone_api-0.3.3/keystone_api/tests/allocations/test_reviews.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/allocations/test_reviews_pk.py` & `keystone_api-0.3.3/keystone_api/tests/allocations/test_reviews_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/fixtures/multi_research_group.yaml` & `keystone_api-0.3.3/keystone_api/tests/fixtures/multi_research_group.yaml`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/health/test.py` & `keystone_api-0.3.3/keystone_api/tests/health/test.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/logging/test_apps.py` & `keystone_api-0.3.3/keystone_api/tests/logging/test_apps.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/logging/test_requests.py` & `keystone_api-0.3.3/keystone_api/tests/logging/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/users/test_researchgroups.py` & `keystone_api-0.3.3/keystone_api/tests/users/test_researchgroups.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/users/test_researchgroups_pk.py` & `keystone_api-0.3.3/keystone_api/tests/users/test_researchgroups_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/users/test_users.py` & `keystone_api-0.3.3/keystone_api/tests/users/test_users.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/users/test_users_pk.py` & `keystone_api-0.3.3/keystone_api/tests/users/test_users_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/keystone_api/tests/utils.py` & `keystone_api-0.3.3/keystone_api/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.2/pyproject.toml` & `keystone_api-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "keystone-api"
-version = "0.3.2"
+version = "0.3.3"
 readme = "README.md"
 description = "A REST API for managing user resource allocations on HPC systems."
 authors = ["Pitt Center for Research Computing"]
 keywords = ["Pitt", "CRC", "HPC", "django"]
 
 [tool.poetry.scripts]
 keystone-api = "keystone_api.manage:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 django = "5.0.3"
 django-auth-ldap = "4.7.0"
 django-celery-beat = "2.6.0"
 django-celery-results = "2.5.1"
-django-cors-headers = "^4.3.1"
+django-cors-headers = "4.3.1"
 django-environ = "0.11.2"
 django-filter = "24.2"
 django-health-check = "3.18.1"
 django-jazzmin = "2.6.1"
 djangorestframework = "3.15.1"
 djangorestframework-simplejwt = "5.3.1"
 drf_spectacular = { version = "0.27.1", extras = ["sidecar"] }
```

### Comparing `keystone_api-0.3.2/PKG-INFO` & `keystone_api-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: keystone-api
-Version: 0.3.2
+Version: 0.3.3
 Summary: A REST API for managing user resource allocations on HPC systems.
 Keywords: Pitt,CRC,HPC,django
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (==5.0.3)
 Requires-Dist: django-auth-ldap (==4.7.0)
 Requires-Dist: django-celery-beat (==2.6.0)
 Requires-Dist: django-celery-results (==2.5.1)
-Requires-Dist: django-cors-headers (>=4.3.1,<5.0.0)
+Requires-Dist: django-cors-headers (==4.3.1)
 Requires-Dist: django-environ (==0.11.2)
 Requires-Dist: django-filter (==24.2)
 Requires-Dist: django-health-check (==3.18.1)
 Requires-Dist: django-jazzmin (==2.6.1)
 Requires-Dist: djangorestframework (==3.15.1)
 Requires-Dist: djangorestframework-simplejwt (==5.3.1)
 Requires-Dist: drf_spectacular[sidecar] (==0.27.1)
```

