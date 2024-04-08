# Comparing `tmp/lamindb_setup-0.68.5.tar.gz` & `tmp/lamindb_setup-0.69.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.68.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.69.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.68.5.tar` & `lamindb_setup-0.69.0.tar`

### file list

```diff
@@ -1,89 +1,87 @@
--rw-r--r--   0        0        0     8290 2024-03-29 13:22:22.689587 lamindb_setup-0.68.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.68.5/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.68.5/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-02-29 20:00:56.143781 lamindb_setup-0.68.5/.gitignore
--rw-r--r--   0        0        0     1931 2024-02-29 20:00:56.143838 lamindb_setup-0.68.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.68.5/LICENSE
--rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.68.5/README.md
--rw-r--r--   0        0        0    94692 2024-04-04 17:27:13.567863 lamindb_setup-0.68.5/docs/changelog.md
--rw-r--r--   0        0        0     7378 2024-03-07 18:05:18.839544 lamindb_setup-0.68.5/docs/hub-cloud/01-init-on-prem-instance.ipynb
--rw-r--r--   0        0        0     4054 2024-03-07 18:05:18.839906 lamindb_setup-0.68.5/docs/hub-cloud/02-connect-on-prem-instance.ipynb
--rw-r--r--   0        0        0     5812 2024-03-07 18:05:18.840396 lamindb_setup-0.68.5/docs/hub-cloud/03-set-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-03-07 00:06:34.620916 lamindb_setup-0.68.5/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     3106 2024-04-04 16:22:51.378892 lamindb_setup-0.68.5/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     2944 2024-04-04 16:22:51.379248 lamindb_setup-0.68.5/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     3160 2024-03-07 16:07:21.923709 lamindb_setup-0.68.5/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.621529 lamindb_setup-0.68.5/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-03-07 18:05:18.841099 lamindb_setup-0.68.5/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-03-26 10:01:31.777978 lamindb_setup-0.68.5/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-03-18 14:07:20.594957 lamindb_setup-0.68.5/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2706 2024-03-07 00:06:34.621901 lamindb_setup-0.68.5/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-03-09 06:05:04.471802 lamindb_setup-0.68.5/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-03-07 00:06:34.622152 lamindb_setup-0.68.5/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-03-07 00:06:34.622232 lamindb_setup-0.68.5/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6181 2024-03-22 15:00:34.131177 lamindb_setup-0.68.5/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.622645 lamindb_setup-0.68.5/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.68.5/docs/index.md
--rw-r--r--   0        0        0      486 2024-03-26 10:01:31.778544 lamindb_setup-0.68.5/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.68.5/docs/reference.md
--rw-r--r--   0        0        0     1558 2024-04-04 17:26:58.556364 lamindb_setup-0.68.5/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     1802 2024-03-29 23:29:05.334743 lamindb_setup-0.68.5/lamindb_setup/_add_remote_storage.py
--rw-r--r--   0        0        0      809 2024-02-29 20:00:56.145929 lamindb_setup-0.68.5/lamindb_setup/_cache.py
--rw-r--r--   0        0        0       92 2024-02-29 20:00:56.145990 lamindb_setup-0.68.5/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2543 2024-03-08 11:38:29.530179 lamindb_setup-0.68.5/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1150 2024-03-06 12:44:01.598158 lamindb_setup-0.68.5/lamindb_setup/_close.py
--rw-r--r--   0        0        0    10793 2024-03-30 23:41:21.159941 lamindb_setup-0.68.5/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     3111 2024-03-22 15:00:34.131907 lamindb_setup-0.68.5/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1500 2024-03-06 12:44:01.598969 lamindb_setup-0.68.5/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2052 2024-03-09 06:05:04.472107 lamindb_setup-0.68.5/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1788 2024-02-29 20:00:56.146417 lamindb_setup-0.68.5/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11400 2024-03-29 23:29:05.334965 lamindb_setup-0.68.5/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     7356 2024-03-08 11:38:29.531124 lamindb_setup-0.68.5/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      795 2024-03-08 11:38:29.531409 lamindb_setup-0.68.5/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      642 2024-03-08 11:38:29.531579 lamindb_setup-0.68.5/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     3657 2024-03-29 23:29:05.335131 lamindb_setup-0.68.5/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1548 2024-02-29 20:00:56.147217 lamindb_setup-0.68.5/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      490 2024-03-05 11:00:49.974555 lamindb_setup-0.68.5/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     2403 2024-03-05 09:37:50.121079 lamindb_setup-0.68.5/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2491 2024-03-05 09:37:50.121160 lamindb_setup-0.68.5/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      240 2024-03-05 09:37:50.121230 lamindb_setup-0.68.5/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5215 2024-03-17 22:17:13.346585 lamindb_setup-0.68.5/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    11678 2024-03-29 09:14:09.554146 lamindb_setup-0.68.5/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4505 2024-03-29 23:01:12.640293 lamindb_setup-0.68.5/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1862 2024-03-05 09:37:50.121645 lamindb_setup-0.68.5/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3241 2024-03-14 13:29:19.826564 lamindb_setup-0.68.5/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    11565 2024-03-14 17:58:31.758814 lamindb_setup-0.68.5/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3744 2024-03-14 17:58:31.759147 lamindb_setup-0.68.5/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2563 2024-03-18 14:07:20.595611 lamindb_setup-0.68.5/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    11782 2024-04-04 17:11:25.342942 lamindb_setup-0.68.5/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     1929 2024-03-14 17:58:31.759632 lamindb_setup-0.68.5/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1281 2024-03-07 18:05:18.845546 lamindb_setup-0.68.5/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     2908 2024-03-05 09:37:50.122398 lamindb_setup-0.68.5/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6835 2024-03-26 10:01:31.779365 lamindb_setup-0.68.5/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     7589 2024-04-04 16:22:51.380220 lamindb_setup-0.68.5/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      275 2024-03-08 11:38:29.532093 lamindb_setup-0.68.5/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2011 2024-03-12 21:48:08.236470 lamindb_setup-0.68.5/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      308 2024-03-05 11:00:49.975018 lamindb_setup-0.68.5/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    23830 2024-04-04 16:22:51.380455 lamindb_setup-0.68.5/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     4154 2024-03-26 15:38:38.001047 lamindb_setup-0.68.5/noxfile.py
--rw-r--r--   0        0        0      992 2024-03-26 10:01:31.780237 lamindb_setup-0.68.5/pyproject.toml
--rw-r--r--   0        0        0     5492 2024-03-29 23:10:03.082274 lamindb_setup-0.68.5/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      285 2024-03-07 00:06:34.623314 lamindb_setup-0.68.5/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     7021 2024-03-07 01:53:25.975859 lamindb_setup-0.68.5/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      502 2024-03-07 00:06:34.623653 lamindb_setup-0.68.5/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      469 2024-03-07 00:06:34.623714 lamindb_setup-0.68.5/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      338 2024-03-07 18:05:18.846365 lamindb_setup-0.68.5/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0     2784 2024-03-22 15:00:34.134178 lamindb_setup-0.68.5/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11280 2024-03-29 23:01:12.640680 lamindb_setup-0.68.5/tests/hub-local/test_all.py
--rw-r--r--   0        0        0     1361 2024-03-22 15:00:34.134342 lamindb_setup-0.68.5/tests/hub-local/test_check_s3_storage_empty.py
--rw-r--r--   0        0        0     1149 2024-03-22 15:00:34.134525 lamindb_setup-0.68.5/tests/hub-local/test_hosted_instance_deletion_gate.py
--rw-r--r--   0        0        0      452 2024-03-07 00:06:34.623879 lamindb_setup-0.68.5/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      365 2024-03-07 18:05:18.846587 lamindb_setup-0.68.5/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      285 2024-03-07 00:06:34.624007 lamindb_setup-0.68.5/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1438 2024-03-07 01:53:25.976258 lamindb_setup-0.68.5/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0      595 2024-03-07 00:06:34.624340 lamindb_setup-0.68.5/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1411 2024-03-12 21:17:07.347266 lamindb_setup-0.68.5/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     1985 2024-03-07 18:05:18.846898 lamindb_setup-0.68.5/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      787 2024-03-28 20:35:14.618464 lamindb_setup-0.68.5/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      842 2024-03-26 15:38:38.001397 lamindb_setup-0.68.5/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.68.5/PKG-INFO
+-rw-r--r--   0        0        0     8290 2024-03-29 13:22:22.689587 lamindb_setup-0.69.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.69.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.69.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-02-29 20:00:56.143781 lamindb_setup-0.69.0/.gitignore
+-rw-r--r--   0        0        0     1931 2024-02-29 20:00:56.143838 lamindb_setup-0.69.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.69.0/LICENSE
+-rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.69.0/README.md
+-rw-r--r--   0        0        0    95916 2024-04-08 10:45:38.348479 lamindb_setup-0.69.0/docs/changelog.md
+-rw-r--r--   0        0        0     7378 2024-03-07 18:05:18.839544 lamindb_setup-0.69.0/docs/hub-cloud/01-init-on-prem-instance.ipynb
+-rw-r--r--   0        0        0     4054 2024-03-07 18:05:18.839906 lamindb_setup-0.69.0/docs/hub-cloud/02-connect-on-prem-instance.ipynb
+-rw-r--r--   0        0        0     5812 2024-03-07 18:05:18.840396 lamindb_setup-0.69.0/docs/hub-cloud/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-03-07 00:06:34.620916 lamindb_setup-0.69.0/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3106 2024-04-08 06:13:37.564530 lamindb_setup-0.69.0/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3383 2024-04-08 09:34:48.611032 lamindb_setup-0.69.0/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3160 2024-03-07 16:07:21.923709 lamindb_setup-0.69.0/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 00:06:34.621529 lamindb_setup-0.69.0/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-03-07 18:05:18.841099 lamindb_setup-0.69.0/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-03-26 10:01:31.777978 lamindb_setup-0.69.0/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-03-18 14:07:20.594957 lamindb_setup-0.69.0/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2706 2024-03-07 00:06:34.621901 lamindb_setup-0.69.0/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-03-09 06:05:04.471802 lamindb_setup-0.69.0/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-03-07 00:06:34.622152 lamindb_setup-0.69.0/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-03-07 00:06:34.622232 lamindb_setup-0.69.0/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6181 2024-03-22 15:00:34.131177 lamindb_setup-0.69.0/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 00:06:34.622645 lamindb_setup-0.69.0/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.69.0/docs/index.md
+-rw-r--r--   0        0        0      486 2024-03-26 10:01:31.778544 lamindb_setup-0.69.0/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.69.0/docs/reference.md
+-rw-r--r--   0        0        0     1558 2024-04-08 10:45:26.010300 lamindb_setup-0.69.0/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     1802 2024-03-29 23:29:05.334743 lamindb_setup-0.69.0/lamindb_setup/_add_remote_storage.py
+-rw-r--r--   0        0        0      809 2024-02-29 20:00:56.145929 lamindb_setup-0.69.0/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0       92 2024-02-29 20:00:56.145990 lamindb_setup-0.69.0/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2543 2024-03-08 11:38:29.530179 lamindb_setup-0.69.0/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1150 2024-03-06 12:44:01.598158 lamindb_setup-0.69.0/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    11848 2024-04-08 10:44:47.691260 lamindb_setup-0.69.0/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     3111 2024-03-22 15:00:34.131907 lamindb_setup-0.69.0/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1500 2024-03-06 12:44:01.598969 lamindb_setup-0.69.0/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2052 2024-03-09 06:05:04.472107 lamindb_setup-0.69.0/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1788 2024-02-29 20:00:56.146417 lamindb_setup-0.69.0/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11479 2024-04-08 10:33:42.801066 lamindb_setup-0.69.0/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     7356 2024-03-08 11:38:29.531124 lamindb_setup-0.69.0/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      795 2024-03-08 11:38:29.531409 lamindb_setup-0.69.0/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      642 2024-03-08 11:38:29.531579 lamindb_setup-0.69.0/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     3657 2024-03-29 23:29:05.335131 lamindb_setup-0.69.0/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1548 2024-02-29 20:00:56.147217 lamindb_setup-0.69.0/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      416 2024-04-05 12:59:33.027651 lamindb_setup-0.69.0/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     1762 2024-04-08 09:34:48.611370 lamindb_setup-0.69.0/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2491 2024-03-05 09:37:50.121160 lamindb_setup-0.69.0/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      240 2024-03-05 09:37:50.121230 lamindb_setup-0.69.0/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5215 2024-03-17 22:17:13.346585 lamindb_setup-0.69.0/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    11522 2024-04-08 09:34:48.611681 lamindb_setup-0.69.0/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4505 2024-03-29 23:01:12.640293 lamindb_setup-0.69.0/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1862 2024-03-05 09:37:50.121645 lamindb_setup-0.69.0/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3241 2024-03-14 13:29:19.826564 lamindb_setup-0.69.0/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    11565 2024-03-14 17:58:31.758814 lamindb_setup-0.69.0/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3744 2024-03-14 17:58:31.759147 lamindb_setup-0.69.0/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2563 2024-03-18 14:07:20.595611 lamindb_setup-0.69.0/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    11515 2024-04-08 09:34:48.612020 lamindb_setup-0.69.0/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     1929 2024-03-14 17:58:31.759632 lamindb_setup-0.69.0/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1281 2024-03-07 18:05:18.845546 lamindb_setup-0.69.0/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     2908 2024-03-05 09:37:50.122398 lamindb_setup-0.69.0/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6835 2024-03-26 10:01:31.779365 lamindb_setup-0.69.0/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     5924 2024-04-08 10:33:42.801416 lamindb_setup-0.69.0/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      275 2024-03-08 11:38:29.532093 lamindb_setup-0.69.0/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2011 2024-03-12 21:48:08.236470 lamindb_setup-0.69.0/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      497 2024-04-05 12:59:33.028024 lamindb_setup-0.69.0/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    23860 2024-04-08 06:08:13.400154 lamindb_setup-0.69.0/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     4265 2024-04-08 09:34:48.612298 lamindb_setup-0.69.0/noxfile.py
+-rw-r--r--   0        0        0      992 2024-03-26 10:01:31.780237 lamindb_setup-0.69.0/pyproject.toml
+-rw-r--r--   0        0        0     5492 2024-03-29 23:10:03.082274 lamindb_setup-0.69.0/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      285 2024-03-07 00:06:34.623314 lamindb_setup-0.69.0/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     7021 2024-03-07 01:53:25.975859 lamindb_setup-0.69.0/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      502 2024-03-07 00:06:34.623653 lamindb_setup-0.69.0/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      469 2024-03-07 00:06:34.623714 lamindb_setup-0.69.0/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      338 2024-03-07 18:05:18.846365 lamindb_setup-0.69.0/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0      548 2024-04-08 09:34:48.612599 lamindb_setup-0.69.0/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11280 2024-03-29 23:01:12.640680 lamindb_setup-0.69.0/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0      452 2024-03-07 00:06:34.623879 lamindb_setup-0.69.0/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      365 2024-03-07 18:05:18.846587 lamindb_setup-0.69.0/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      285 2024-03-07 00:06:34.624007 lamindb_setup-0.69.0/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1438 2024-03-07 01:53:25.976258 lamindb_setup-0.69.0/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0      595 2024-03-07 00:06:34.624340 lamindb_setup-0.69.0/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1411 2024-03-12 21:17:07.347266 lamindb_setup-0.69.0/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     1985 2024-03-07 18:05:18.846898 lamindb_setup-0.69.0/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      787 2024-03-28 20:35:14.618464 lamindb_setup-0.69.0/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      842 2024-03-26 15:38:38.001397 lamindb_setup-0.69.0/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.69.0/PKG-INFO
```

### Comparing `lamindb_setup-0.68.5/.github/workflows/build.yml` & `lamindb_setup-0.69.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/.github/workflows/latest-changes.yml` & `lamindb_setup-0.69.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/.gitignore` & `lamindb_setup-0.69.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/.pre-commit-config.yaml` & `lamindb_setup-0.69.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/LICENSE` & `lamindb_setup-0.69.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/changelog.md` & `lamindb_setup-0.69.0/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚸 Skip hub request for a purely local instance | [713](https://github.com/laminlabs/lamindb-setup/pull/713) | [falexwolf](https://github.com/falexwolf) | 2024-04-08 | 0.69.0
+🐛 Fix clashes for multi process | [712](https://github.com/laminlabs/lamindb-setup/pull/712) | [falexwolf](https://github.com/falexwolf) | 2024-04-08 |
+♻️ No longer need AWS account | [711](https://github.com/laminlabs/lamindb-setup/pull/711) | [falexwolf](https://github.com/falexwolf) | 2024-04-08 |
+📝 Fix docs | [709](https://github.com/laminlabs/lamindb-setup/pull/709) | [falexwolf](https://github.com/falexwolf) | 2024-04-05 |
+♻️ Replace TypeVar with TypeAlias | [707](https://github.com/laminlabs/lamindb-setup/pull/707) | [falexwolf](https://github.com/falexwolf) | 2024-04-04 |
+♻️ Refactor clean up | [706](https://github.com/laminlabs/lamindb-setup/pull/706) | [falexwolf](https://github.com/falexwolf) | 2024-04-04 |
+🩹 Do bucket injection trick only for s3 | [705](https://github.com/laminlabs/lamindb-setup/pull/705) | [Koncopd](https://github.com/Koncopd) | 2024-04-04 |
+🚸 Add region param | [704](https://github.com/laminlabs/lamindb-setup/pull/704) | [falexwolf](https://github.com/falexwolf) | 2024-04-04 |
 🐛 Avoid the error due to deleting the same file by multiple processes | [703](https://github.com/laminlabs/lamindb-setup/pull/703) | [Koncopd](https://github.com/Koncopd) | 2024-04-04 | 0.68.5
 🐛 Fix directory uploads for hosted instances | [702](https://github.com/laminlabs/lamindb-setup/pull/702) | [Koncopd](https://github.com/Koncopd) | 2024-04-04 |
 🚑️ Temp fix for non-hosted buckets | [700](https://github.com/laminlabs/lamindb-setup/pull/700) | [sunnyosun](https://github.com/sunnyosun) | 2024-04-02 |
 🍱 Add the scverse spatial hackathon bucket | [699](https://github.com/laminlabs/lamindb-setup/pull/699) | [falexwolf](https://github.com/falexwolf) | 2024-03-30 |
 ♻️ More fine-grained db credentials management | [698](https://github.com/laminlabs/lamindb-setup/pull/698) | [falexwolf](https://github.com/falexwolf) | 2024-03-29 | 0.68.2
 ✨ `upath.to_url()` | [695](https://github.com/laminlabs/lamindb-setup/pull/695) | [falexwolf](https://github.com/falexwolf) | 2024-03-28 |
 ♻️ Enable to choose skip_suffixes | [693](https://github.com/laminlabs/lamindb-setup/pull/693) | [falexwolf](https://github.com/falexwolf) | 2024-03-27 | 0.68.1
```

### Comparing `lamindb_setup-0.68.5/docs/hub-cloud/01-init-on-prem-instance.ipynb` & `lamindb_setup-0.69.0/docs/hub-cloud/01-init-on-prem-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-cloud/02-connect-on-prem-instance.ipynb` & `lamindb_setup-0.69.0/docs/hub-cloud/02-connect-on-prem-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-cloud/03-set-storage.ipynb` & `lamindb_setup-0.69.0/docs/hub-cloud/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.69.0/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.69.0/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.69.0/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9789351851851852%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'import pytest\\n'), (5, 'from lamindb_setup.core.upath "*

 * *            "import InstanceNotEmpty\\n')]}}, insert: [(8, OrderedDict([('cell_type', 'markdown'), "*

 * *            "('metadata', OrderedDict()), ('source', ['Test that instance can not be deleted from "*

 * *            "hub:'])])), (9, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', ['with "*

 * *            "pytest.raises(InstanceNot […]*

```diff
@@ -9,18 +9,20 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "import pytest\n",
                 "import shutil\n",
                 "import lamindb_setup as ln_setup\n",
                 "from lamindb_setup.core.upath import UPath\n",
                 "from lamindb_setup.core._hub_core import delete_instance\n",
+                "from lamindb_setup.core.upath import InstanceNotEmpty\n",
                 "\n",
                 "instance_name = \"my-hosted\"\n",
                 "assert ln_setup.settings.user.handle == \"testuser1\""
             ]
         },
         {
             "cell_type": "code",
@@ -89,14 +91,31 @@
                 "assert target_dir.is_dir()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "Test that instance can not be deleted from hub:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "with pytest.raises(InstanceNotEmpty):\n",
+                "    delete_instance(f\"testuser1/{instance_name}\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "Delete everything:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `lamindb_setup-0.68.5/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.69.0/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.69.0/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.69.0/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.69.0/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.69.0/docs/hub-prod/test-empty-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.69.0/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.69.0/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.69.0/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.69.0/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/__init__.py` & `lamindb_setup-0.69.0/lamindb_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.68.5"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.69.0"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._close import close  # noqa
 from ._delete import delete  # noqa
```

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_add_remote_storage.py` & `lamindb_setup-0.69.0/lamindb_setup/_add_remote_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_cache.py` & `lamindb_setup-0.69.0/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_check_setup.py` & `lamindb_setup-0.69.0/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_close.py` & `lamindb_setup-0.69.0/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.69.0/lamindb_setup/_connect_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,112 +92,131 @@
 
     Args:
         slug: The instance slug `account_handle/instance_name` or URL.
             If the instance is owned by you, it suffices to pass the instance name.
         db: Load the instance with an updated database URL.
         storage: Load the instance with an updated default storage.
     """
-    owner, name = get_owner_name_from_identifier(slug)
+    isettings: InstanceSettings = None  # type: ignore
+    try:
+        owner, name = get_owner_name_from_identifier(slug)
+
+        if _check_instance_setup() and not _test:
+            if (
+                settings._instance_exists
+                and f"{owner}/{name}" == settings.instance.slug
+            ):
+                logger.info(f"connected lamindb: {settings.instance.slug}")
+                return None
+            else:
+                raise RuntimeError(MESSAGE_NO_MULTIPLE_INSTANCE)
+        elif settings._instance_exists and f"{owner}/{name}" != settings.instance.slug:
+            close_instance(mute=True)
 
-    if _check_instance_setup() and not _test:
-        if settings._instance_exists and f"{owner}/{name}" == settings.instance.slug:
-            logger.info(f"connected lamindb: {settings.instance.slug}")
-            return None
-        else:
-            raise RuntimeError(MESSAGE_NO_MULTIPLE_INSTANCE)
-    elif settings._instance_exists and f"{owner}/{name}" != settings.instance.slug:
-        close_instance(mute=True)
-
-    settings_file = instance_settings_file(name, owner)
-
-    # the following will return a string if the instance does not exist
-    # on the hub
-    hub_result = connect_instance_from_hub(owner=owner, name=name)
-
-    # if hub_result is not a string, it means it made a request
-    # that successfully returned metadata
-    if not isinstance(hub_result, str):
-        instance_result, storage_result = hub_result
-        db_updated = update_db_using_local(instance_result, settings_file, db=db)
-        ssettings = StorageSettings(
-            root=storage_result["root"],
-            region=storage_result["region"],
-            uid=storage_result["lnid"],
-        )
-        isettings = InstanceSettings(
-            id=UUID(instance_result["id"]),
-            owner=owner,
-            name=name,
-            storage=ssettings,
-            db=db_updated,
-            schema=instance_result["schema_str"],
-            git_repo=instance_result["git_repo"],
-        )
-        from importlib import metadata
-
-        try:
-            lamindb_version = metadata.version("lamindb")
-        except metadata.PackageNotFoundError:
-            lamindb_version = None
-        logger.important(
-            f"last migration: lamindb=={instance_result['lamindb_version']} <> your"
-            f" env: lamindb=={lamindb_version}"
-        )
-    else:
-        error_message = (
-            f"'{owner}/{name}' not loadable:"
-            f" '{hub_result}'\nCheck your permissions:"
-            f" https://lamin.ai/{owner}/{name}?tab=collaborators"
-        )
+        settings_file = instance_settings_file(name, owner)
+
+        make_hub_request = True
         if settings_file.exists():
             isettings = load_instance_settings(settings_file)
-            if isettings.is_remote:
-                if _raise_not_reachable_error:
-                    raise SystemExit(error_message)
-                return "instance-not-reachable"
-            logger.info(f"found cached instance metadata: {settings_file}")
-        else:
-            if _raise_not_reachable_error:
-                raise SystemExit(error_message)
-            return "instance-not-reachable"
-        # mimic instance_result from hub
-        instance_result = {"id": isettings.id.hex}
-
-    if storage is not None:
-        update_isettings_with_storage(isettings, storage)
-    if _test:
-        isettings._persist()  # this is to test the settings
-        return None
-    silence_loggers()
-    check, msg = isettings._load_db(
-        do_not_lock_for_laminapp_admin=True
-    )  # this also updates local SQLite
-    if not check:
-        local_db = isettings._is_cloud_sqlite and isettings._sqlite_file_local.exists()
-        if local_db:
-            logger.warning(
-                "SQLite file does not exist in the cloud, but exists locally:"
-                f" {isettings._sqlite_file_local}\nTo push the file to the cloud, call:"
-                " lamin close"
-            )
-        elif _raise_not_reachable_error:
-            raise SystemExit(msg)
-        else:
-            logger.warning(
-                f"instance exists with id {isettings.id.hex}, but database is not"
-                " loadable: re-initializing"
+            # skip hub request for a purely local instance
+            make_hub_request = isettings.is_remote
+
+        if make_hub_request:
+            # the following will return a string if the instance does not exist
+            # on the hub
+            hub_result = connect_instance_from_hub(owner=owner, name=name)
+            # if hub_result is not a string, it means it made a request
+            # that successfully returned metadata
+            if not isinstance(hub_result, str):
+                instance_result, storage_result = hub_result
+                db_updated = update_db_using_local(
+                    instance_result, settings_file, db=db
+                )
+                ssettings = StorageSettings(
+                    root=storage_result["root"],
+                    region=storage_result["region"],
+                    uid=storage_result["lnid"],
+                )
+                isettings = InstanceSettings(
+                    id=UUID(instance_result["id"]),
+                    owner=owner,
+                    name=name,
+                    storage=ssettings,
+                    db=db_updated,
+                    schema=instance_result["schema_str"],
+                    git_repo=instance_result["git_repo"],
+                )
+                from importlib import metadata
+
+                try:
+                    lamindb_version = metadata.version("lamindb")
+                except metadata.PackageNotFoundError:
+                    lamindb_version = None
+                logger.important(
+                    f"last migration: lamindb=={instance_result['lamindb_version']} <>"
+                    f" your env: lamindb=={lamindb_version}"
+                )
+            else:
+                error_message = (
+                    f"'{owner}/{name}' not loadable:"
+                    f" '{hub_result}'\nCheck your permissions:"
+                    f" https://lamin.ai/{owner}/{name}?tab=collaborators"
+                )
+                if settings_file.exists():
+                    isettings = load_instance_settings(settings_file)
+                    if isettings.is_remote:
+                        if _raise_not_reachable_error:
+                            raise SystemExit(error_message)
+                        return "instance-not-reachable"
+
+                else:
+                    if _raise_not_reachable_error:
+                        raise SystemExit(error_message)
+                    return "instance-not-reachable"
+                # mimic instance_result from hub
+                instance_result = {"id": isettings.id.hex}
+
+        if storage is not None:
+            update_isettings_with_storage(isettings, storage)
+        isettings._persist()
+        if _test:
+            return None
+        silence_loggers()
+        check, msg = isettings._load_db(
+            do_not_lock_for_laminapp_admin=True
+        )  # this also updates local SQLite
+        if not check:
+            local_db = (
+                isettings._is_cloud_sqlite and isettings._sqlite_file_local.exists()
             )
-            return "instance-corrupted-or-deleted", instance_result
-    # this is for testing purposes only
-    if _TEST_FAILED_LOAD:
-        raise RuntimeError("Technical testing error.")
-
-    if storage is not None and isettings.dialect == "sqlite":
-        update_root_field_in_default_storage(isettings)
-    load_from_isettings(isettings)
+            if local_db:
+                logger.warning(
+                    "SQLite file does not exist in the cloud, but exists locally:"
+                    f" {isettings._sqlite_file_local}\nTo push the file to the cloud,"
+                    " call: lamin close"
+                )
+            elif _raise_not_reachable_error:
+                raise SystemExit(msg)
+            else:
+                logger.warning(
+                    f"instance exists with id {isettings.id.hex}, but database is not"
+                    " loadable: re-initializing"
+                )
+                return "instance-corrupted-or-deleted", instance_result
+        # this is for testing purposes only
+        if _TEST_FAILED_LOAD:
+            raise RuntimeError("Technical testing error.")
+
+        if storage is not None and isettings.dialect == "sqlite":
+            update_root_field_in_default_storage(isettings)
+        load_from_isettings(isettings)
+    except Exception as e:
+        if isettings is not None:
+            isettings._get_settings_file().unlink(missing_ok=True)  # type: ignore
+        raise e
     return None
 
 
 def load(
     slug: str,
     *,
     db: Optional[str] = None,
```

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_delete.py` & `lamindb_setup-0.69.0/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_django.py` & `lamindb_setup-0.69.0/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_exportdb.py` & `lamindb_setup-0.69.0/lamindb_setup/_exportdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_importdb.py` & `lamindb_setup-0.69.0/lamindb_setup/_importdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_init_instance.py` & `lamindb_setup-0.69.0/lamindb_setup/_init_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,16 +241,16 @@
             db=db,
             schema=schema,
             uid=ssettings.uid,
         )
         if isettings.is_remote and instance_state != "instance-corrupted-or-deleted":
             init_instance_hub(isettings)
         validate_sqlite_state(isettings)
+        isettings._persist()
         if _test:
-            isettings._persist()
             return None
         isettings._init_db()
         load_from_isettings(isettings, init=True)
         if isettings._is_cloud_sqlite:
             isettings._cloud_sqlite_locker.lock()
             logger.warning(
                 "locked instance (to unlock and push changes to the cloud SQLite file,"
@@ -263,14 +263,15 @@
         from ._delete import delete_by_isettings
         from .core._hub_core import delete_storage_record as delete_storage_record
         from .core._hub_core import delete_instance_record as delete_instance_record
 
         if isettings is not None:
             delete_by_isettings(isettings)
             delete_instance_record(isettings.id)
+            isettings._get_settings_file().unlink(missing_ok=True)  # type: ignore
         if ssettings is not None:
             delete_storage_record(ssettings.uuid)  # type: ignore
         raise e
     return None
 
 
 def load_from_isettings(
```

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_migrate.py` & `lamindb_setup-0.69.0/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_register_instance.py` & `lamindb_setup-0.69.0/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_schema.py` & `lamindb_setup-0.69.0/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_setup_user.py` & `lamindb_setup-0.69.0/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.69.0/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_hub_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from ._settings_storage import StorageSettings, base62
 
 
 from ._hub_client import (
     connect_hub,
     call_with_fallback_auth,
     call_with_fallback,
-    AuthUnknownError,
 )
 from ._hub_crud import (
     select_instance_by_owner_name,
     select_instance_by_id_with_storage,
     select_account_by_handle,
     select_db_user_by_instance,
     select_instance_by_name,
@@ -249,23 +248,21 @@
     for retry in range(max_retries):
         try:
             response = client.functions.invoke(
                 "access-aws",
                 invoke_options={"body": {"storage_root": storage_root}},
             )
         except (FunctionsRelayError, FunctionsHttpError, json.JSONDecodeError) as error:
-            if isinstance(error, json.JSONDecodeError):
-                raise AuthUnknownError(message=str(error), original_error=error)
             print("no valid response, retry", response)
             sleep(1)
             if retry == max_retries - 1:
                 raise error
             else:
                 continue
-        if response is not None and response != {}:
+        if response is not None and response != b"{}":
             loaded_credentials = json.loads(response)["Credentials"]
             credentials = {}
             credentials["key"] = loaded_credentials["AccessKeyId"]
             credentials["secret"] = loaded_credentials["SecretAccessKey"]
             credentials["token"] = loaded_credentials["SessionToken"]
             return credentials
         elif lamindb_setup._TESTING:
```

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_settings.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_settings_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 from lamin_utils import logger
 from pathlib import Path
 from typing import Any, Optional, Union
-from ._aws_storage import find_closest_aws_region, get_aws_account_id
+from ._aws_storage import find_closest_aws_region
 from appdirs import AppDirs
 from ._settings_save import save_system_storage_settings
 from ._settings_store import system_storage_settings_file
 from .upath import LocalPathClasses, UPath, create_path, convert_pathlike
 from uuid import UUID
 import string
 import secrets
@@ -59,57 +59,50 @@
     # we need to touch a 0-byte object in the storage location to avoid
     # permission errors from leveraging s3fs on an empty hosted storage location
     root_upath = convert_pathlike(root)
     mark_upath = root_upath / IS_INITIALIZED_KEY
     mark_upath.touch()
 
 
-def init_storage(storage: UPathStr) -> "StorageSettings":
-    if storage is None:
-        raise ValueError("storage argument can't be `None`")
-    root = str(storage)  # ensure we have a string
+def init_storage(root: UPathStr) -> "StorageSettings":
+    if root is None:
+        raise ValueError("`storage` argument can't be `None`")
+    root_str = str(root)  # ensure we have a string
     uid = base62(8)
     region = None
-    if root.startswith("create-s3"):
-        if root != "create-s3":
-            assert "--" in root, "example: `create-s3--eu-central-1`"
-            region = root.replace("create-s3--", "")
+    lamin_env = os.getenv("LAMIN_ENV")
+    if root_str.startswith("create-s3"):
+        if root_str != "create-s3":
+            assert "--" in root_str, "example: `create-s3--eu-central-1`"
+            region = root_str.replace("create-s3--", "")
         if region is None:
             region = find_closest_aws_region()
         else:
             if region not in hosted_regions:
                 raise ValueError(f"region has to be one of {hosted_regions}")
-        lamin_env = os.getenv("LAMIN_ENV")
         if lamin_env is None or lamin_env == "prod":
-            root = f"s3://lamin-{region}/{uid}"
+            root_str = f"s3://lamin-{region}/{uid}"
         else:
-            root = f"s3://lamin-hosted-test/{uid}"
-    elif root.startswith(("gs://", "s3://")):
-        # check for existence happens in get_storage_region
+            root_str = f"s3://lamin-hosted-test/{uid}"
+    elif root_str.startswith(("gs://", "s3://")):
         pass
     else:  # local path
         try:
-            _ = Path(root)
+            _ = Path(root_str)
         except Exception as e:
-            logger.error(
-                "`storage` is neither a valid local, a Google Cloud nor an S3 path."
-            )
+            logger.error("`storage` is not a valid local, GCP storage or AWS S3 path")
             raise e
-    ssettings = StorageSettings(uid=uid, root=root, region=region)
+    ssettings = StorageSettings(uid=uid, root=root_str, region=region)
     if ssettings.is_cloud:
         from ._hub_core import init_storage as init_storage_hub
 
-        if storage == "create-s3":
-            ssettings._aws_account_id = 767398070972
-        elif root.startswith("s3://"):
-            ssettings._aws_account_id = get_aws_account_id()
         ssettings._description = f"Created as default storage for instance {uid}"
         ssettings._uuid = init_storage_hub(ssettings)
         logger.important(f"registered storage: {ssettings.root_as_str}")
-    if ssettings.is_cloud and storage == "create-s3":
+    if ssettings.is_cloud and root_str.startswith("create-s3"):
         mark_storage_root(ssettings.root)
     return ssettings
 
 
 def _process_cache_path(cache_path: Union[str, Path, UPath, None]):
     if cache_path is None or cache_path == "null":
         return None
```

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.69.0/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.69.0/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/hashing.py` & `lamindb_setup-0.69.0/lamindb_setup/core/hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/lamindb_setup/core/upath.py` & `lamindb_setup-0.69.0/lamindb_setup/core/upath.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,19 +180,19 @@
     if print_progress:
         if not os.path.isdir(path):
             cb = ProgressCallback("uploading")
         else:
             # todo: make proper progress bar for directories
             cb = fsspec.callbacks.NoOpCallback()
         kwargs["callback"] = cb
-    # this weird thing is to avoid triggering create_bucket in upload
+    # this weird thing is to avoid s3fs triggering create_bucket in upload
     # if dirs are present
     # it allows to avoid permission error
     destination = str(self)
-    if os.path.isfile(path):
+    if self.protocol != "s3" or os.path.isfile(path):
         cleanup_cache = False
     else:
         bucket = self._url.netloc
         if bucket not in self.fs.dircache:
             self.fs.dircache[bucket] = [{}]
             if not destination.endswith(TRAILING_SEP):  # type: ignore
                 destination += "/"
```

### Comparing `lamindb_setup-0.68.5/noxfile.py` & `lamindb_setup-0.69.0/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,19 @@
             env=env,
         )
         session.run(*f"pytest -s {COVERAGE_ARGS} ./docs/hub-cloud".split(), env=env)
 
 
 @nox.session
 def hub_local(session: nox.Session):
+    os.environ["AWS_SECRET_ACCESS_KEY_DEV_S3"] = os.environ["AWS_ACCESS_KEY_ID"]
     # the -n 1 is to ensure that supabase thread exits properly
-    session.run(*f"pytest -n 1 {COVERAGE_ARGS} ./tests/hub-local".split())
+    session.run(
+        *f"pytest -n 1 {COVERAGE_ARGS} ./tests/hub-local".split(), env=os.environ
+    )
 
 
 @nox.session
 def storage(session: nox.Session):
     # we need AWS to retrieve credentials for testuser1, but want to eliminate
     # them after that
     os.environ["AWS_ACCESS_KEY_ID"] = os.environ["TMP_AWS_ACCESS_KEY_ID"]
```

### Comparing `lamindb_setup-0.68.5/pyproject.toml` & `lamindb_setup-0.69.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.69.0/tests/hub-cloud/test_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.69.0/tests/hub-cloud/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/tests/hub-local/test_all.py` & `lamindb_setup-0.69.0/tests/hub-local/test_all.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.69.0/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/tests/hub-prod/test_upath.py` & `lamindb_setup-0.69.0/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/tests/storage/test_hashing.py` & `lamindb_setup-0.69.0/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/tests/storage/test_storage_access.py` & `lamindb_setup-0.69.0/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/tests/storage/test_storage_basis.py` & `lamindb_setup-0.69.0/tests/storage/test_storage_basis.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/tests/storage/test_storage_stats.py` & `lamindb_setup-0.69.0/tests/storage/test_storage_stats.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.5/PKG-INFO` & `lamindb_setup-0.69.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.68.5
+Version: 0.69.0
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```

