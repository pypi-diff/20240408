# Comparing `tmp/avtomat_aws-0.1.2.tar.gz` & `tmp/avtomat_aws-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avtomat_aws-0.1.2.tar", max compression
+gzip compressed data, was "avtomat_aws-0.1.3.tar", max compression
```

## Comparing `avtomat_aws-0.1.2.tar` & `avtomat_aws-0.1.3.tar`

### file list

```diff
@@ -1,117 +1,120 @@
--rw-r--r--   0        0        0      724 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0    18091 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/LICENSE
--rw-r--r--   0        0        0     3838 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/README.md
--rw-r--r--   0        0        0       69 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/backup/create_backups.py
--rw-r--r--   0        0        0      823 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/backup/delete_backups.py
--rw-r--r--   0        0        0      887 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     1115 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     1104 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1259 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/copy_snapshots.py
--rw-r--r--   0        0        0      670 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/create_snapshots.py
--rw-r--r--   0        0        0      814 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/delete_images.py
--rw-r--r--   0        0        0      677 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/delete_security_groups.py
--rw-r--r--   0        0        0      647 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/delete_snapshots.py
--rw-r--r--   0        0        0      793 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/delete_volumes.py
--rw-r--r--   0        0        0      472 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_active_regions.py
--rw-r--r--   0        0        0      451 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     1203 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_images.py
--rw-r--r--   0        0        0     1369 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_instances.py
--rw-r--r--   0        0        0      634 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     1401 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     1162 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_tags.py
--rw-r--r--   0        0        0      481 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     1348 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_volumes.py
--rw-r--r--   0        0        0      889 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0      813 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1175 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     1210 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/modify_tags.py
--rw-r--r--   0        0        0     1090 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/modify_volumes.py
--rw-r--r--   0        0        0      783 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/ec2/share_snapshots.py
--rw-r--r--   0        0        0      816 2024-04-07 16:44:46.757897 avtomat_aws-0.1.2/avtomat_aws/cli/general/get_date.py
--rw-r--r--   0        0        0      750 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0      740 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_inactive_users.py
--rw-r--r--   0        0        0      468 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0      691 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0      722 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_old_password_users.py
--rw-r--r--   0        0        0      725 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0      705 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     1221 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/iam/modify_access_keys.py
--rw-r--r--   0        0        0     1323 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/iam/modify_users_console_access.py
--rw-r--r--   0        0        0      583 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/iam/quarantine_user.py
--rw-r--r--   0        0        0     4721 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/main.py
--rw-r--r--   0        0        0     1201 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/s3/create_objects.py
--rw-r--r--   0        0        0      854 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/s3/delete_objects.py
--rw-r--r--   0        0        0     1184 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/s3/discover_objects.py
--rw-r--r--   0        0        0     1365 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/services.py
--rw-r--r--   0        0        0     1375 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/sts/create_session.py
--rw-r--r--   0        0        0      391 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/cli/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/decorators/__init__.py
--rw-r--r--   0        0        0      789 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/decorators/authenticate.py
--rw-r--r--   0        0        0      615 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/decorators/set_logger.py
--rw-r--r--   0        0        0      724 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/decorators/validate.py
--rw-r--r--   0        0        0        0 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/helpers/__init__.py
--rw-r--r--   0        0        0      288 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/helpers/set_defaults.py
--rw-r--r--   0        0        0      805 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/helpers/set_region.py
--rw-r--r--   0        0        0     2636 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/helpers/set_session.py
--rw-r--r--   0        0        0      728 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/helpers/set_session_objects.py
--rw-r--r--   0        0        0        0 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/loggers/__init__.py
--rw-r--r--   0        0        0      457 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/loggers/config.py
--rw-r--r--   0        0        0      138 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/loggers/set_logging.py
--rw-r--r--   0        0        0        0 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/__init__.py
--rw-r--r--   0        0        0       86 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/backup/__init__.py
--rw-r--r--   0        0        0     3810 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/backup/create_backups.py
--rw-r--r--   0        0        0     1629 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/backup/delete_backups.py
--rw-r--r--   0        0        0      163 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/cloudtrail/__init__.py
--rw-r--r--   0        0        0     2784 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     3383 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     3252 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1099 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/__init__.py
--rw-r--r--   0        0        0     2625 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/copy_snapshots.py
--rw-r--r--   0        0        0     1988 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/create_snapshots.py
--rw-r--r--   0        0        0     2264 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/delete_images.py
--rw-r--r--   0        0        0     1532 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/delete_security_groups.py
--rw-r--r--   0        0        0     1430 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/delete_snapshots.py
--rw-r--r--   0        0        0     2663 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/delete_volumes.py
--rw-r--r--   0        0        0      902 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_active_regions.py
--rw-r--r--   0        0        0     1346 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     2929 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_images.py
--rw-r--r--   0        0        0     3662 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_instances.py
--rw-r--r--   0        0        0     1800 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     3247 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     5192 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_tags.py
--rw-r--r--   0        0        0    16665 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     3322 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_volumes.py
--rw-r--r--   0        0        0     4757 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0     3973 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1853 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     4818 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/modify_tags.py
--rw-r--r--   0        0        0     2983 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/modify_volumes.py
--rw-r--r--   0        0        0     1819 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/ec2/share_snapshots.py
--rw-r--r--   0        0        0       31 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/general/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/general/get_date.py
--rw-r--r--   0        0        0      618 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/iam/__init__.py
--rw-r--r--   0        0        0     2674 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0     3228 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_inactive_users.py
--rw-r--r--   0        0        0     1538 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0     2138 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0     2026 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_old_password_users.py
--rw-r--r--   0        0        0     2808 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0     1945 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     2081 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/iam/modify_access_keys.py
--rw-r--r--   0        0        0     3175 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/iam/modify_users_console_access.py
--rw-r--r--   0        0        0     1719 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/iam/quarantine_user.py
--rw-r--r--   0        0        0      133 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/s3/__init__.py
--rw-r--r--   0        0        0     1908 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/s3/create_objects.py
--rw-r--r--   0        0        0     2141 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/s3/delete_objects.py
--rw-r--r--   0        0        0     2517 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/s3/discover_objects.py
--rw-r--r--   0        0        0       70 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/sts/__init__.py
--rw-r--r--   0        0        0      750 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/sts/create_session.py
--rw-r--r--   0        0        0      717 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/services/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/validations/__init__.py
--rw-r--r--   0        0        0      291 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/validations/config.py
--rw-r--r--   0        0        0     3423 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/validations/rules.py
--rw-r--r--   0        0        0      497 2024-04-07 16:44:46.761897 avtomat_aws-0.1.2/avtomat_aws/validations/validate.py
--rw-r--r--   0        0        0     1743 2024-04-07 16:44:46.765897 avtomat_aws-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 avtomat_aws-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      800 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0    18091 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3838 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/README.md
+-rw-r--r--   0        0        0       69 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/backup/create_backups.py
+-rw-r--r--   0        0        0      864 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/backup/delete_backups.py
+-rw-r--r--   0        0        0      928 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     1156 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     1145 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1300 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0      711 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/create_snapshots.py
+-rw-r--r--   0        0        0      855 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_images.py
+-rw-r--r--   0        0        0      718 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0      688 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0      834 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      513 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0      522 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1244 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_images.py
+-rw-r--r--   0        0        0     1410 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_instances.py
+-rw-r--r--   0        0        0      675 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     1442 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     1203 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_tags.py
+-rw-r--r--   0        0        0      522 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     1389 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_volumes.py
+-rw-r--r--   0        0        0      960 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0      884 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1175 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1251 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_tags.py
+-rw-r--r--   0        0        0     1131 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_volumes.py
+-rw-r--r--   0        0        0      824 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/share_snapshots.py
+-rw-r--r--   0        0        0      887 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/general/get_date.py
+-rw-r--r--   0        0        0      791 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0      781 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0      509 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0      732 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0      763 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0      766 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0      746 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     1262 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     1364 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0      583 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/quarantine_user.py
+-rw-r--r--   0        0        0     4829 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/main.py
+-rw-r--r--   0        0        0     1242 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/s3/create_objects.py
+-rw-r--r--   0        0        0      895 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/s3/delete_objects.py
+-rw-r--r--   0        0        0     1225 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/s3/discover_objects.py
+-rw-r--r--   0        0        0     1365 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/services.py
+-rw-r--r--   0        0        0     1375 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/sts/create_session.py
+-rw-r--r--   0        0        0      462 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/decorators/__init__.py
+-rw-r--r--   0        0        0      789 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/decorators/authenticate.py
+-rw-r--r--   0        0        0      615 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/decorators/set_logger.py
+-rw-r--r--   0        0        0      724 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/decorators/validate.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/cli/__init__.py
+-rw-r--r--   0        0        0      203 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/cli/set_output.py
+-rw-r--r--   0        0        0     2083 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/cli/table.py
+-rw-r--r--   0        0        0      288 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/set_defaults.py
+-rw-r--r--   0        0        0      805 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/set_region.py
+-rw-r--r--   0        0        0     2636 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/set_session.py
+-rw-r--r--   0        0        0      728 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/set_session_objects.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/loggers/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/loggers/config.py
+-rw-r--r--   0        0        0      138 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/loggers/set_logging.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/backup/__init__.py
+-rw-r--r--   0        0        0     3810 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/backup/create_backups.py
+-rw-r--r--   0        0        0     1629 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/backup/delete_backups.py
+-rw-r--r--   0        0        0      163 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/__init__.py
+-rw-r--r--   0        0        0     2784 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     3383 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     3252 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1099 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/__init__.py
+-rw-r--r--   0        0        0     2625 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0     1988 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/create_snapshots.py
+-rw-r--r--   0        0        0     2264 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_images.py
+-rw-r--r--   0        0        0     1532 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0     1430 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0     2663 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      902 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0     1346 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     2929 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_images.py
+-rw-r--r--   0        0        0     3662 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_instances.py
+-rw-r--r--   0        0        0     1800 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     3247 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     5192 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_tags.py
+-rw-r--r--   0        0        0    16665 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     3322 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_volumes.py
+-rw-r--r--   0        0        0     4757 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0     3973 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1853 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     4818 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_tags.py
+-rw-r--r--   0        0        0     2983 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_volumes.py
+-rw-r--r--   0        0        0     1819 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/share_snapshots.py
+-rw-r--r--   0        0        0       31 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/general/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/general/get_date.py
+-rw-r--r--   0        0        0      618 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/__init__.py
+-rw-r--r--   0        0        0     2674 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0     3228 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0     1538 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0     2138 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0     2026 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0     2808 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0     1945 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     2081 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     3175 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0     1719 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/quarantine_user.py
+-rw-r--r--   0        0        0      133 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/s3/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/s3/create_objects.py
+-rw-r--r--   0        0        0     2141 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/s3/delete_objects.py
+-rw-r--r--   0        0        0     2517 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/s3/discover_objects.py
+-rw-r--r--   0        0        0       70 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/sts/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/sts/create_session.py
+-rw-r--r--   0        0        0      717 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/validations/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/validations/config.py
+-rw-r--r--   0        0        0     3423 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/validations/rules.py
+-rw-r--r--   0        0        0      497 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/validations/validate.py
+-rw-r--r--   0        0        0     1743 2024-04-08 07:03:01.257117 avtomat_aws-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 avtomat_aws-0.1.3/PKG-INFO
```

### Comparing `avtomat_aws-0.1.2/CHANGELOG.md` & `avtomat_aws-0.1.3/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.1.3 (2024-04-08)
+
+### Fix
+
+- **cli**: Add option for tabulated output
+
 ## 0.1.2 (2024-04-07)
 
 ### Fix
 
 - **cli**: Add action descriptions to the parser
 
 ## 0.1.1 (2024-04-06)
```

### Comparing `avtomat_aws-0.1.2/LICENSE` & `avtomat_aws-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/README.md` & `avtomat_aws-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/backup/create_backups.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/backup/create_backups.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.backup import create_backups
 
 ACTION_DESCRIPTION = "Start an on-demand backup job for the specified resources."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -45,12 +46,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = create_backups(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/backup/delete_backups.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_security_groups.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-from avtomat_aws.services.backup import delete_backups
+from avtomat_aws.helpers.cli.set_output import set_output
+from avtomat_aws.services.ec2 import delete_security_groups
 
-ACTION_DESCRIPTION = "Delete backup recovery points."
+ACTION_DESCRIPTION = "Delete EC2 security groups."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
     required = parser.add_argument_group("required")
 
     required.add_argument(
-        "--backup_vault_name",
-        help="Backup vault from which to delete recovery points.",
-        required=True,
-    )
-    required.add_argument(
-        "--recovery_point_arns",
+        "--security_group_ids",
         nargs="+",
-        help="Recovery point ARNs to delete, separated by space.",
+        help="Security Group IDs to delete, separated by space.",
         required=True,
     )
 
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = delete_backups(**inputs)
-        for item in result:
-            print(item)
+        result = delete_security_groups(**inputs)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/cloudtrail/discover_events.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_user_events.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,27 @@
-from avtomat_aws.services.cloudtrail import discover_events
+from avtomat_aws.helpers.cli.set_output import set_output
+from avtomat_aws.services.cloudtrail import discover_user_events
 
-ACTION_DESCRIPTION = "Discover events by name."
+ACTION_DESCRIPTION = "Discover events created by specific user."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
     required = parser.add_argument_group("required")
 
-    required.add_argument("--event", help="Search for this event.", required=True)
+    required.add_argument(
+        "--user", help="Search events originating from this user.", required=True
+    )
+    parser.add_argument(
+        "--events",
+        nargs="+",
+        help="Search for specific events, separated by space.",
+        required=False,
+    )
     parser.add_argument(
         "--created_after",
         help="Search for events created after this time. (YYYY/MM/DD)",
         required=False,
     )
     parser.add_argument(
         "--created_before",
@@ -23,13 +32,12 @@
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = discover_events(**inputs)
-        for item in result:
-            print(item)
+        result = discover_user_events(**inputs)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_resource_events.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.cloudtrail import discover_resource_events
 
 ACTION_DESCRIPTION = "Discover events for a specific resource."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -32,12 +33,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = discover_resource_events(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/cloudtrail/discover_user_events.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_events.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-from avtomat_aws.services.cloudtrail import discover_user_events
+from avtomat_aws.helpers.cli.set_output import set_output
+from avtomat_aws.services.cloudtrail import discover_events
 
-ACTION_DESCRIPTION = "Discover events created by specific user."
+ACTION_DESCRIPTION = "Discover events by name."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
     required = parser.add_argument_group("required")
 
-    required.add_argument(
-        "--user", help="Search events originating from this user.", required=True
-    )
-    parser.add_argument(
-        "--events",
-        nargs="+",
-        help="Search for specific events, separated by space.",
-        required=False,
-    )
+    required.add_argument("--event", help="Search for this event.", required=True)
     parser.add_argument(
         "--created_after",
         help="Search for events created after this time. (YYYY/MM/DD)",
         required=False,
     )
     parser.add_argument(
         "--created_before",
@@ -31,13 +24,12 @@
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = discover_user_events(**inputs)
-        for item in result:
-            print(item)
+        result = discover_events(**inputs)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/copy_snapshots.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/copy_snapshots.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import copy_snapshots
 
 ACTION_DESCRIPTION = "Move EC2 snapshots between regions or accounts."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -39,12 +40,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = copy_snapshots(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/create_snapshots.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/create_snapshots.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import create_snapshots
 
 ACTION_DESCRIPTION = "Create EBS snapshots from volumes."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -19,12 +20,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = create_snapshots(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/delete_images.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_images.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import delete_images
 
 ACTION_DESCRIPTION = "Delete EC2 images (AMI)."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -25,12 +26,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = delete_images(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/delete_snapshots.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_snapshots.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import delete_snapshots
 
 ACTION_DESCRIPTION = "Delete EBS snapshots."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -19,12 +20,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = delete_snapshots(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/delete_volumes.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_volumes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import delete_volumes
 
 ACTION_DESCRIPTION = "Delete EBS volumes."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -25,12 +26,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = delete_volumes(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_images.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_images.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import discover_images
 
 ACTION_DESCRIPTION = "Discover AWS images (AMI)."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -39,12 +40,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = discover_images(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_instances.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_instances.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import discover_instances
 
 ACTION_DESCRIPTION = "Discover instances."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -44,12 +45,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = discover_instances(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_no_ssm_instances.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import discover_no_ssm_instances
 
 ACTION_DESCRIPTION = "Discover EC2 instances without SSM enabled."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -17,12 +18,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = discover_no_ssm_instances(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_snapshots.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_volumes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,58 @@
-from avtomat_aws.services.ec2 import discover_snapshots
+from avtomat_aws.helpers.cli.set_output import set_output
+from avtomat_aws.services.ec2 import discover_volumes
 
-ACTION_DESCRIPTION = "Discover snapshots of EBS volumes."
+ACTION_DESCRIPTION = "Discover EBS volumes."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
     parser.add_argument(
-        "--volume_ids",
+        "--instance_ids",
         nargs="+",
-        help="Get snapshots that originate from specific volumes.",
+        help="Get volumes attached to specified instances.",
         required=False,
     )
     parser.add_argument(
-        "--snapshot_ids",
+        "--volume_ids",
         nargs="+",
-        help="Snapshot IDs to focus on, separated by space.",
+        help="Volume IDs to focus on, separated by space.",
         required=False,
     )
     parser.add_argument(
         "--unencrypted",
         action="store_true",
-        help="Get only unencrypted snapshots.",
+        help="Get only unencrypted volumes.",
         required=False,
     )
     parser.add_argument(
-        "--exclude_aws_backup",
+        "--detached",
         action="store_true",
-        help="Exclude snapshots managed by AWS Backup.",
+        help="Get only detached volumes.",
         required=False,
     )
     parser.add_argument(
-        "--created_before",
-        help="Get snapshots created before date (YYYY/MM//DD).",
+        "--types",
+        nargs="+",
+        help="Volume types to check, separated by space.",
         required=False,
     )
     parser.add_argument(
-        "--created_after",
-        help="Get snapshots created after date (YYYY/MM//DD).",
+        "--root",
+        action="store_true",
+        help="Get only root volumes.",
         required=False,
     )
 
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = discover_snapshots(**inputs)
-        for item in result:
-            print(item)
+        result = discover_volumes(**inputs)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_tags.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_tags.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import discover_tags
 
 ACTION_DESCRIPTION = "Find existing or missing tags on EC2 resources."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -37,12 +38,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = discover_tags(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/discover_volumes.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,47 @@
-from avtomat_aws.services.ec2 import discover_volumes
+from avtomat_aws.services.ec2 import modify_default_ebs_encryption
 
-ACTION_DESCRIPTION = "Discover EBS volumes."
+ACTION_DESCRIPTION = "Modify default EBS encryption."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
     parser.add_argument(
-        "--instance_ids",
-        nargs="+",
-        help="Get volumes attached to specified instances.",
-        required=False,
-    )
-    parser.add_argument(
-        "--volume_ids",
-        nargs="+",
-        help="Volume IDs to focus on, separated by space.",
+        "--enable",
+        action="store_true",
+        help="Enable default EBS encryption.",
         required=False,
     )
     parser.add_argument(
-        "--unencrypted",
+        "--disable",
         action="store_true",
-        help="Get only unencrypted volumes.",
+        help="Disable default EBS encryption.",
         required=False,
     )
     parser.add_argument(
-        "--detached",
+        "--change_kms_key",
         action="store_true",
-        help="Get only detached volumes.",
+        help="Change the KMS Key used for encryption.",
         required=False,
     )
     parser.add_argument(
-        "--types",
-        nargs="+",
-        help="Volume types to check, separated by space.",
-        required=False,
+        "--kms_key_id", help="KMS Key ID to use for encryption.", required=False
     )
     parser.add_argument(
-        "--root",
+        "--reset_kms_key",
         action="store_true",
-        help="Get only root volumes.",
+        help="Reset the KMS Key used for encryption to AWS EBS default.",
         required=False,
     )
 
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = discover_volumes(**inputs)
-        for item in result:
-            print(item)
+        modify_default_ebs_encryption(**inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/encrypt_instance_volumes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import encrypt_instance_volumes
 
 ACTION_DESCRIPTION = "Encrypt all EBS volumes attached to an instance."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -25,11 +26,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = encrypt_instance_volumes(**inputs)
-        print(result)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/encrypt_volume.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/encrypt_volume.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import encrypt_volume
 
 ACTION_DESCRIPTION = "Encrypt an EBS volume."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -23,11 +24,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = encrypt_volume(**inputs)
-        print(result)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/modify_tags.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_tags.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import modify_tags
 
 ACTION_DESCRIPTION = "Modify EC2 resource tags."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -37,12 +38,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = modify_tags(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/ec2/modify_volumes.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_volumes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.ec2 import modify_volumes
 
 ACTION_DESCRIPTION = "Modify EBS volumes."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -32,12 +33,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = modify_volumes(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/general/get_date.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_old_password_users.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-from avtomat_aws.services.general import get_date
+from avtomat_aws.helpers.cli.set_output import set_output
+from avtomat_aws.services.iam import discover_old_password_users
 
-ACTION_DESCRIPTION = "Return a date in the requested format."
+ACTION_DESCRIPTION = "Discover IAM users with passwords older than a certain age."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
-    parser.add_argument(
-        "--after",
-        type=int,
-        help="Return a date number of days in the future.",
-        required=False,
-    )
-    parser.add_argument(
-        "--before",
+    required = parser.add_argument_group("required")
+
+    required.add_argument(
+        "--threshold_days",
         type=int,
-        help="Return a date number of days in the past.",
-        required=False,
-    )
-    parser.add_argument(
-        "--format", help="Return the date in this format.", required=False
+        help="Get users with a password older than this number of days.",
+        required=True,
     )
 
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = get_date(**inputs)
-        print(result)
+        result = discover_old_password_users(**inputs)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_inactive_console_users.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_inactive_console_users.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.iam import discover_inactive_console_users
 
 ACTION_DESCRIPTION = (
     "Discover IAM users with last console sign-in over a certain period."
 )
 
 
@@ -21,12 +22,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = discover_inactive_console_users(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_inactive_users.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_old_access_keys.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from avtomat_aws.services.iam import discover_inactive_users
+from avtomat_aws.helpers.cli.set_output import set_output
+from avtomat_aws.services.iam import discover_old_access_keys
 
-ACTION_DESCRIPTION = "Discover IAM users who haven't used the console and any access keys over a certain period."
+ACTION_DESCRIPTION = "Discover IAM access keys over a certain age."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
     required = parser.add_argument_group("required")
 
     required.add_argument(
         "--threshold_days",
         type=int,
-        help="Get users with no activity over this number of days.",
+        help="Get access keys older than this number of days.",
         required=True,
     )
 
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = discover_inactive_users(**inputs)
-        for item in result:
-            print(item)
+        result = discover_old_access_keys(**inputs)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_old_access_keys.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_unused_roles.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from avtomat_aws.services.iam import discover_old_access_keys
+from avtomat_aws.helpers.cli.set_output import set_output
+from avtomat_aws.services.iam import discover_unused_roles
 
-ACTION_DESCRIPTION = "Discover IAM access keys over a certain age."
+ACTION_DESCRIPTION = "Discover IAM roles not used over a certain amount of days."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
     required = parser.add_argument_group("required")
 
     required.add_argument(
         "--threshold_days",
         type=int,
-        help="Get access keys older than this number of days.",
+        help="Get roles not used for more than this number of days.",
         required=True,
     )
 
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = discover_old_access_keys(**inputs)
-        for item in result:
-            print(item)
+        result = discover_unused_roles(**inputs)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_unused_access_keys.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_unused_access_keys.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.iam import discover_unused_access_keys
 
 ACTION_DESCRIPTION = "Discover IAM access keys not used for over a number of days."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -19,12 +20,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = discover_unused_access_keys(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/iam/discover_unused_roles.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/s3/delete_objects.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-from avtomat_aws.services.iam import discover_unused_roles
+from avtomat_aws.helpers.cli.set_output import set_output
+from avtomat_aws.services.s3 import delete_objects
 
-ACTION_DESCRIPTION = "Discover IAM roles not used over a certain amount of days."
+ACTION_DESCRIPTION = "Delete objects from an S3 bucket."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
     required = parser.add_argument_group("required")
 
     required.add_argument(
-        "--threshold_days",
-        type=int,
-        help="Get roles not used for more than this number of days.",
+        "--bucket", help="Name of the S3 bucket to delete objects from.", required=True
+    )
+    required.add_argument(
+        "--objects",
+        nargs="+",
+        help="Objects to delete, separated by space.",
         required=True,
     )
+    parser.add_argument("--prefix", help="Prefix to filter objects by.", required=False)
 
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = discover_unused_roles(**inputs)
-        for item in result:
-            print(item)
+        result = delete_objects(**inputs)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/iam/modify_access_keys.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/iam/modify_access_keys.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.iam import modify_access_keys
 
 ACTION_DESCRIPTION = "Enable or disable an IAM access key."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -36,12 +37,11 @@
         "region": args.region,
         "debug": args.debug,
         "silent": args.silent,
     }
 
     try:
         result = modify_access_keys(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/iam/modify_users_console_access.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/iam/modify_users_console_access.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.iam import modify_users_console_access
 
 ACTION_DESCRIPTION = "Enable or disable AWS Management Console access for an IAM user."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -38,12 +39,11 @@
         "region": args.region,
         "debug": args.debug,
         "silent": args.silent,
     }
 
     try:
         result = modify_users_console_access(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/iam/quarantine_user.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/main.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,17 @@
     )
     parser.add_argument(
         "--debug", action="store_true", help="Increase log verbosity.", required=False
     )
     parser.add_argument(
         "--silent", action="store_true", help="Decrease log verbosity.", required=False
     )
+    parser.add_argument(
+        "--output", help="Output format.", choices=["table"], required=False
+    )
 
     # Use the imported module's function to add its arguments to the parser
     if hasattr(module, "add_cli_arguments"):
         module.add_cli_arguments(parser)
         parser.set_defaults(func=module.cli)
     else:
         print("No arguments defined for this action.")
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/s3/create_objects.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/s3/create_objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.s3 import create_objects
 
 ACTION_DESCRIPTION = "Create objects in an S3 bucket."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -36,12 +37,11 @@
         "region": args.region,
         "debug": args.debug,
         "silent": args.silent,
     }
 
     try:
         result = create_objects(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/s3/discover_objects.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/s3/discover_objects.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from avtomat_aws.helpers.cli.set_output import set_output
 from avtomat_aws.services.s3 import discover_objects
 
 ACTION_DESCRIPTION = "Discover objects in an S3 bucket."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
@@ -33,12 +34,11 @@
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
         result = discover_objects(**inputs)
-        for item in result:
-            print(item)
+        set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/services.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/services.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/cli/sts/create_session.py` & `avtomat_aws-0.1.3/avtomat_aws/cli/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/decorators/authenticate.py` & `avtomat_aws-0.1.3/avtomat_aws/decorators/authenticate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/decorators/set_logger.py` & `avtomat_aws-0.1.3/avtomat_aws/decorators/set_logger.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/decorators/validate.py` & `avtomat_aws-0.1.3/avtomat_aws/decorators/validate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/helpers/set_region.py` & `avtomat_aws-0.1.3/avtomat_aws/helpers/set_region.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/helpers/set_session.py` & `avtomat_aws-0.1.3/avtomat_aws/helpers/set_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/helpers/set_session_objects.py` & `avtomat_aws-0.1.3/avtomat_aws/helpers/set_session_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/backup/create_backups.py` & `avtomat_aws-0.1.3/avtomat_aws/services/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/backup/delete_backups.py` & `avtomat_aws-0.1.3/avtomat_aws/services/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/cloudtrail/discover_events.py` & `avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/cloudtrail/discover_user_events.py` & `avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/__init__.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/copy_snapshots.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/create_snapshots.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/create_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/delete_images.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/delete_security_groups.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/delete_snapshots.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/delete_volumes.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_active_regions.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_active_regions.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_default_ebs_encryption.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_images.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_instances.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_snapshots.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_tags.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_unused_security_groups.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_unused_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/discover_volumes.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/encrypt_volume.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/modify_tags.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/modify_volumes.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/ec2/share_snapshots.py` & `avtomat_aws-0.1.3/avtomat_aws/services/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/general/get_date.py` & `avtomat_aws-0.1.3/avtomat_aws/services/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/iam/__init__.py` & `avtomat_aws-0.1.3/avtomat_aws/services/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_inactive_console_users.py` & `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_inactive_users.py` & `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_no_mfa_users.py` & `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_no_mfa_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_old_access_keys.py` & `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_old_password_users.py` & `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_unused_access_keys.py` & `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/iam/discover_unused_roles.py` & `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/iam/modify_access_keys.py` & `avtomat_aws-0.1.3/avtomat_aws/services/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/iam/modify_users_console_access.py` & `avtomat_aws-0.1.3/avtomat_aws/services/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/iam/quarantine_user.py` & `avtomat_aws-0.1.3/avtomat_aws/services/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/s3/create_objects.py` & `avtomat_aws-0.1.3/avtomat_aws/services/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/s3/delete_objects.py` & `avtomat_aws-0.1.3/avtomat_aws/services/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/s3/discover_objects.py` & `avtomat_aws-0.1.3/avtomat_aws/services/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/sts/create_session.py` & `avtomat_aws-0.1.3/avtomat_aws/services/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/services/sts/whoami.py` & `avtomat_aws-0.1.3/avtomat_aws/services/sts/whoami.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/avtomat_aws/validations/rules.py` & `avtomat_aws-0.1.3/avtomat_aws/validations/rules.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.2/pyproject.toml` & `avtomat_aws-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avtomat-aws"
-version = "0.1.2"
+version = "0.1.3"
 description = "A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations."
 authors = ["Dimitar Atanasov <dimitar@avtomat.io>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://avtomat.io"
 documentation = "https://docs.avtomat.io/aws/get_started"
 keywords = ["aws", "cloud", "automation", "cli", "python", "boto3"]
```

### Comparing `avtomat_aws-0.1.2/PKG-INFO` & `avtomat_aws-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avtomat-aws
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations.
 Home-page: https://avtomat.io
 License: GPL-2.0-only
 Keywords: aws,cloud,automation,cli,python,boto3
 Author: Dimitar Atanasov
 Author-email: dimitar@avtomat.io
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: avtomat-aws Version: 0.1.2 Summary: A collection of
+Metadata-Version: 2.1 Name: avtomat-aws Version: 0.1.3 Summary: A collection of
 reusable Amazon Web Services actions, bringing speed and certainty to cloud
 operations. Home-page: https://avtomat.io License: GPL-2.0-only Keywords:
 aws,cloud,automation,cli,python,boto3 Author: Dimitar Atanasov Author-email:
 dimitar@avtomat.io Requires-Python: >=3.9,<4.0 Classifier: Development Status
 :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

