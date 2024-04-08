# Comparing `tmp/avtomat_aws-0.1.3.tar.gz` & `tmp/avtomat_aws-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avtomat_aws-0.1.3.tar", max compression
+gzip compressed data, was "avtomat_aws-0.1.4.tar", max compression
```

## Comparing `avtomat_aws-0.1.3.tar` & `avtomat_aws-0.1.4.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0      800 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0    18091 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/LICENSE
--rw-r--r--   0        0        0     3838 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/README.md
--rw-r--r--   0        0        0       69 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/__init__.py
--rw-r--r--   0        0        0     1526 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/backup/create_backups.py
--rw-r--r--   0        0        0      864 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/backup/delete_backups.py
--rw-r--r--   0        0        0      928 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     1156 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     1145 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1300 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/copy_snapshots.py
--rw-r--r--   0        0        0      711 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/create_snapshots.py
--rw-r--r--   0        0        0      855 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_images.py
--rw-r--r--   0        0        0      718 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_security_groups.py
--rw-r--r--   0        0        0      688 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_snapshots.py
--rw-r--r--   0        0        0      834 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_volumes.py
--rw-r--r--   0        0        0      513 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_active_regions.py
--rw-r--r--   0        0        0      522 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     1244 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_images.py
--rw-r--r--   0        0        0     1410 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_instances.py
--rw-r--r--   0        0        0      675 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     1442 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     1203 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_tags.py
--rw-r--r--   0        0        0      522 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     1389 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_volumes.py
--rw-r--r--   0        0        0      960 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0      884 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1175 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     1251 2024-04-08 07:03:01.249117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_tags.py
--rw-r--r--   0        0        0     1131 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_volumes.py
--rw-r--r--   0        0        0      824 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/ec2/share_snapshots.py
--rw-r--r--   0        0        0      887 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/general/get_date.py
--rw-r--r--   0        0        0      791 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0      781 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_inactive_users.py
--rw-r--r--   0        0        0      509 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0      732 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0      763 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_old_password_users.py
--rw-r--r--   0        0        0      766 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0      746 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     1262 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/modify_access_keys.py
--rw-r--r--   0        0        0     1364 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/modify_users_console_access.py
--rw-r--r--   0        0        0      583 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/iam/quarantine_user.py
--rw-r--r--   0        0        0     4829 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/main.py
--rw-r--r--   0        0        0     1242 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/s3/create_objects.py
--rw-r--r--   0        0        0      895 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/s3/delete_objects.py
--rw-r--r--   0        0        0     1225 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/s3/discover_objects.py
--rw-r--r--   0        0        0     1365 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/services.py
--rw-r--r--   0        0        0     1375 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/sts/create_session.py
--rw-r--r--   0        0        0      462 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/cli/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/decorators/__init__.py
--rw-r--r--   0        0        0      789 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/decorators/authenticate.py
--rw-r--r--   0        0        0      615 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/decorators/set_logger.py
--rw-r--r--   0        0        0      724 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/decorators/validate.py
--rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/cli/__init__.py
--rw-r--r--   0        0        0      203 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/cli/set_output.py
--rw-r--r--   0        0        0     2083 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/cli/table.py
--rw-r--r--   0        0        0      288 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/set_defaults.py
--rw-r--r--   0        0        0      805 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/set_region.py
--rw-r--r--   0        0        0     2636 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/set_session.py
--rw-r--r--   0        0        0      728 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/helpers/set_session_objects.py
--rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/loggers/__init__.py
--rw-r--r--   0        0        0      457 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/loggers/config.py
--rw-r--r--   0        0        0      138 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/loggers/set_logging.py
--rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/__init__.py
--rw-r--r--   0        0        0       86 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/backup/__init__.py
--rw-r--r--   0        0        0     3810 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/backup/create_backups.py
--rw-r--r--   0        0        0     1629 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/backup/delete_backups.py
--rw-r--r--   0        0        0      163 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/__init__.py
--rw-r--r--   0        0        0     2784 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     3383 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     3252 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1099 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/__init__.py
--rw-r--r--   0        0        0     2625 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/copy_snapshots.py
--rw-r--r--   0        0        0     1988 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/create_snapshots.py
--rw-r--r--   0        0        0     2264 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_images.py
--rw-r--r--   0        0        0     1532 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_security_groups.py
--rw-r--r--   0        0        0     1430 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_snapshots.py
--rw-r--r--   0        0        0     2663 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_volumes.py
--rw-r--r--   0        0        0      902 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_active_regions.py
--rw-r--r--   0        0        0     1346 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     2929 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_images.py
--rw-r--r--   0        0        0     3662 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_instances.py
--rw-r--r--   0        0        0     1800 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     3247 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     5192 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_tags.py
--rw-r--r--   0        0        0    16665 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     3322 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_volumes.py
--rw-r--r--   0        0        0     4757 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0     3973 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1853 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     4818 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_tags.py
--rw-r--r--   0        0        0     2983 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_volumes.py
--rw-r--r--   0        0        0     1819 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/ec2/share_snapshots.py
--rw-r--r--   0        0        0       31 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/general/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/general/get_date.py
--rw-r--r--   0        0        0      618 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/__init__.py
--rw-r--r--   0        0        0     2674 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0     3228 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_inactive_users.py
--rw-r--r--   0        0        0     1538 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0     2138 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0     2026 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_old_password_users.py
--rw-r--r--   0        0        0     2808 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0     1945 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     2081 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/modify_access_keys.py
--rw-r--r--   0        0        0     3175 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/modify_users_console_access.py
--rw-r--r--   0        0        0     1719 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/iam/quarantine_user.py
--rw-r--r--   0        0        0      133 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/s3/__init__.py
--rw-r--r--   0        0        0     1908 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/s3/create_objects.py
--rw-r--r--   0        0        0     2141 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/s3/delete_objects.py
--rw-r--r--   0        0        0     2517 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/s3/discover_objects.py
--rw-r--r--   0        0        0       70 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/sts/__init__.py
--rw-r--r--   0        0        0      750 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/sts/create_session.py
--rw-r--r--   0        0        0      717 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/services/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/validations/__init__.py
--rw-r--r--   0        0        0      291 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/validations/config.py
--rw-r--r--   0        0        0     3423 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/validations/rules.py
--rw-r--r--   0        0        0      497 2024-04-08 07:03:01.253117 avtomat_aws-0.1.3/avtomat_aws/validations/validate.py
--rw-r--r--   0        0        0     1743 2024-04-08 07:03:01.257117 avtomat_aws-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 avtomat_aws-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1002 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0    18091 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3838 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/README.md
+-rw-r--r--   0        0        0       69 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/backup/create_backups.py
+-rw-r--r--   0        0        0      864 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/backup/delete_backups.py
+-rw-r--r--   0        0        0      928 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     1156 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     1145 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1300 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0      711 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/create_snapshots.py
+-rw-r--r--   0        0        0      855 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_images.py
+-rw-r--r--   0        0        0      718 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0      688 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0      834 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      513 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0      522 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1244 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_images.py
+-rw-r--r--   0        0        0     1410 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_instances.py
+-rw-r--r--   0        0        0      675 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     1442 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     1203 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_tags.py
+-rw-r--r--   0        0        0      522 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     1389 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_volumes.py
+-rw-r--r--   0        0        0      960 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0      884 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1175 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1251 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_tags.py
+-rw-r--r--   0        0        0     1131 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_volumes.py
+-rw-r--r--   0        0        0      824 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/share_snapshots.py
+-rw-r--r--   0        0        0      887 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/general/get_date.py
+-rw-r--r--   0        0        0      791 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0      781 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0      509 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0      732 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0      763 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0      766 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0      746 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     1262 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     1364 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0      583 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/quarantine_user.py
+-rw-r--r--   0        0        0     4829 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/main.py
+-rw-r--r--   0        0        0     1242 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/s3/create_objects.py
+-rw-r--r--   0        0        0      895 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/s3/delete_objects.py
+-rw-r--r--   0        0        0     1225 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/s3/discover_objects.py
+-rw-r--r--   0        0        0     1365 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/services.py
+-rw-r--r--   0        0        0     1375 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/sts/create_session.py
+-rw-r--r--   0        0        0      462 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/decorators/__init__.py
+-rw-r--r--   0        0        0      789 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/decorators/authenticate.py
+-rw-r--r--   0        0        0      615 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/decorators/set_logger.py
+-rw-r--r--   0        0        0      724 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/decorators/validate.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/cli/__init__.py
+-rw-r--r--   0        0        0      203 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/cli/set_output.py
+-rw-r--r--   0        0        0     2083 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/cli/table.py
+-rw-r--r--   0        0        0      288 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/set_defaults.py
+-rw-r--r--   0        0        0      805 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/set_region.py
+-rw-r--r--   0        0        0     2636 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/set_session.py
+-rw-r--r--   0        0        0      728 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/set_session_objects.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/loggers/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/loggers/config.py
+-rw-r--r--   0        0        0      138 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/loggers/set_logging.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/services/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/services/backup/__init__.py
+-rw-r--r--   0        0        0     3810 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/services/backup/create_backups.py
+-rw-r--r--   0        0        0     1629 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/services/backup/delete_backups.py
+-rw-r--r--   0        0        0      163 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/__init__.py
+-rw-r--r--   0        0        0     2821 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     3420 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     3289 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1099 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/__init__.py
+-rw-r--r--   0        0        0     2625 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0     1988 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/create_snapshots.py
+-rw-r--r--   0        0        0     2264 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_images.py
+-rw-r--r--   0        0        0     1532 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0     1430 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0     2663 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      902 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0     1346 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     3012 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_images.py
+-rw-r--r--   0        0        0     3662 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_instances.py
+-rw-r--r--   0        0        0     1800 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     3330 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     5192 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_tags.py
+-rw-r--r--   0        0        0    16665 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     3322 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_volumes.py
+-rw-r--r--   0        0        0     4757 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0     3973 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1853 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     4818 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_tags.py
+-rw-r--r--   0        0        0     2983 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_volumes.py
+-rw-r--r--   0        0        0     1819 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/share_snapshots.py
+-rw-r--r--   0        0        0       31 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/general/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/general/get_date.py
+-rw-r--r--   0        0        0      618 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/__init__.py
+-rw-r--r--   0        0        0     2674 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0     3228 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0     1538 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0     2138 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0     2026 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0     2808 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0     1945 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     2081 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     3175 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0     1719 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/quarantine_user.py
+-rw-r--r--   0        0        0      133 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/s3/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/s3/create_objects.py
+-rw-r--r--   0        0        0     2141 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/s3/delete_objects.py
+-rw-r--r--   0        0        0     2517 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/s3/discover_objects.py
+-rw-r--r--   0        0        0       70 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/sts/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/sts/create_session.py
+-rw-r--r--   0        0        0      717 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/validations/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/validations/config.py
+-rw-r--r--   0        0        0     3514 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/validations/rules.py
+-rw-r--r--   0        0        0      497 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/validations/validate.py
+-rw-r--r--   0        0        0     1743 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 avtomat_aws-0.1.4/PKG-INFO
```

### Comparing `avtomat_aws-0.1.3/CHANGELOG.md` & `avtomat_aws-0.1.4/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 0.1.4 (2024-04-08)
+
+### Fix
+
+- **date-handling**: Improve how discover_images and discover_snapshots handle dates
+- **validation-logic**: Fix cloudtrail validation logic to correctly evaluate dates
+
 ## 0.1.3 (2024-04-08)
 
 ### Fix
 
 - **cli**: Add option for tabulated output
 
 ## 0.1.2 (2024-04-07)
```

### Comparing `avtomat_aws-0.1.3/LICENSE` & `avtomat_aws-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/README.md` & `avtomat_aws-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/backup/create_backups.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/backup/delete_backups.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_events.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/cloudtrail/discover_user_events.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/copy_snapshots.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/create_snapshots.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/create_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_images.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_security_groups.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_snapshots.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/delete_volumes.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_active_regions.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_active_regions.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_images.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_instances.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_snapshots.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_tags.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_unused_security_groups.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_unused_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/discover_volumes.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/encrypt_volume.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_tags.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/modify_volumes.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/ec2/share_snapshots.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/general/get_date.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_inactive_console_users.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_inactive_users.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_old_access_keys.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_old_password_users.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_unused_access_keys.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/iam/discover_unused_roles.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/iam/modify_access_keys.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/iam/modify_users_console_access.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/iam/quarantine_user.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/main.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/main.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/s3/create_objects.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/s3/delete_objects.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/s3/discover_objects.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/services.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/services.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/cli/sts/create_session.py` & `avtomat_aws-0.1.4/avtomat_aws/cli/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/decorators/authenticate.py` & `avtomat_aws-0.1.4/avtomat_aws/decorators/authenticate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/decorators/set_logger.py` & `avtomat_aws-0.1.4/avtomat_aws/decorators/set_logger.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/decorators/validate.py` & `avtomat_aws-0.1.4/avtomat_aws/decorators/validate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/helpers/cli/table.py` & `avtomat_aws-0.1.4/avtomat_aws/helpers/cli/table.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/helpers/set_region.py` & `avtomat_aws-0.1.4/avtomat_aws/helpers/set_region.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/helpers/set_session.py` & `avtomat_aws-0.1.4/avtomat_aws/helpers/set_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/helpers/set_session_objects.py` & `avtomat_aws-0.1.4/avtomat_aws/helpers/set_session_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/backup/create_backups.py` & `avtomat_aws-0.1.4/avtomat_aws/services/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/backup/delete_backups.py` & `avtomat_aws-0.1.4/avtomat_aws/services/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_events.py` & `avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_events.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from avtomat_aws.decorators.set_logger import set_logger
 from avtomat_aws.decorators.validate import validate
 from avtomat_aws.helpers.set_session_objects import set_session_objects
 
 logger = logging.getLogger(__name__)
 
 DEFAULTS = {
-    "created_after": (datetime.now() - timedelta(days=90)).strftime("%Y/%m/%d"),
-    "created_before": (datetime.now()).strftime("%Y/%m/%d"),
+    "created_after": datetime.now() - timedelta(days=90),
+    "created_before": datetime.now(),
     "region": None,
     "debug": False,
     "silent": False,
 }
 RULES = [
     {"required": ["event"]},
     {"date_yymmdd": ["created_after", "created_before"]},
@@ -27,17 +27,17 @@
 @authenticate()
 def discover_events(**kwargs):
     """Discover events by name"""
 
     # Required parameters
     event = kwargs.pop("event")
 
-    if kwargs.get("created_after"):
+    if kwargs.get("created_after") and type(kwargs["created_after"]) is str:
         kwargs["created_after"] = datetime.strptime(kwargs["created_after"], "%Y/%m/%d")
-    if kwargs.get("created_before"):
+    if kwargs.get("created_before") and type(kwargs["created_before"]) is str:
         kwargs["created_before"] = datetime.strptime(
             kwargs["created_before"], "%Y/%m/%d"
         )
 
     logger.info(f"Discovering CloudTrail events for '{event}'")
 
     events = search_events(event, **kwargs)
```

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_resource_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from avtomat_aws.decorators.validate import validate
 from avtomat_aws.helpers.set_session_objects import set_session_objects
 
 logger = logging.getLogger(__name__)
 
 DEFAULTS = {
     "events": [],
-    "created_after": (datetime.now() - timedelta(days=90)).strftime("%Y/%m/%d"),
-    "created_before": (datetime.now()).strftime("%Y/%m/%d"),
+    "created_after": datetime.now() - timedelta(days=90),
+    "created_before": datetime.now(),
     "region": None,
     "debug": False,
     "silent": False,
 }
 RULES = [
     {"required": ["resource_id"]},
     {"date_yymmdd": ["created_after", "created_before"]},
@@ -28,17 +28,17 @@
 @authenticate()
 def discover_resource_events(**kwargs):
     """Discover events for a specific resource"""
 
     # Required parameters
     resource_id = kwargs.pop("resource_id")
 
-    if kwargs.get("created_after"):
+    if kwargs.get("created_after") and type(kwargs["created_after"]) is str:
         kwargs["created_after"] = datetime.strptime(kwargs["created_after"], "%Y/%m/%d")
-    if kwargs.get("created_before"):
+    if kwargs.get("created_before") and type(kwargs["created_before"]) is str:
         kwargs["created_before"] = datetime.strptime(
             kwargs["created_before"], "%Y/%m/%d"
         )
 
     logger.info(f"Discovering CloudTrail events for resource '{resource_id}'")
 
     unfiltered_events = search_events(resource_id, **kwargs)
```

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/cloudtrail/discover_user_events.py` & `avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_user_events.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from avtomat_aws.decorators.validate import validate
 from avtomat_aws.helpers.set_session_objects import set_session_objects
 
 logger = logging.getLogger(__name__)
 
 DEFAULTS = {
     "events": [],
-    "created_after": (datetime.now() - timedelta(days=90)).strftime("%Y/%m/%d"),
-    "created_before": (datetime.now()).strftime("%Y/%m/%d"),
+    "created_after": datetime.now() - timedelta(days=90),
+    "created_before": datetime.now(),
     "region": None,
     "debug": False,
     "silent": False,
 }
 RULES = [
     {"required": ["user"]},
     {"date_yymmdd": ["created_after", "created_before"]},
@@ -28,17 +28,17 @@
 @authenticate()
 def discover_user_events(**kwargs):
     """Discover events created by specific user"""
 
     # Required parameters
     user = kwargs.pop("user")
 
-    if kwargs.get("created_after"):
+    if kwargs.get("created_after") and type(kwargs["created_after"]) is str:
         kwargs["created_after"] = datetime.strptime(kwargs["created_after"], "%Y/%m/%d")
-    if kwargs.get("created_before"):
+    if kwargs.get("created_before") and type(kwargs["created_before"]) is str:
         kwargs["created_before"] = datetime.strptime(
             kwargs["created_before"], "%Y/%m/%d"
         )
 
     logger.info(f"Discovering CloudTrail events for user '{user}'")
 
     unfiltered_events = search_events(user, **kwargs)
```

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/__init__.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/copy_snapshots.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/create_snapshots.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/create_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_images.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_security_groups.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_snapshots.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/delete_volumes.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_active_regions.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_active_regions.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_default_ebs_encryption.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_images.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_images.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
 @validate(DEFAULTS, RULES)
 @set_logger()
 @authenticate()
 def discover_images(**kwargs):
     """Discover images based on provided criteria"""
 
-    if kwargs.get("created_before"):
+    if kwargs.get("created_after") and type(kwargs["created_after"]) is str:
+        kwargs["created_after"] = datetime.strptime(kwargs["created_after"], "%Y/%m/%d")
+    if kwargs.get("created_before") and type(kwargs["created_before"]) is str:
         kwargs["created_before"] = datetime.strptime(
             kwargs["created_before"], "%Y/%m/%d"
         )
-    if kwargs.get("created_after"):
-        kwargs["created_after"] = datetime.strptime(kwargs["created_after"], "%Y/%m/%d")
 
     logger.info("Discovering images")
 
     filters = build_filters(**kwargs)
     images = search_images(filters, **kwargs)
 
     logger.info(f"{len(images)} images found")
```

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_instances.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_snapshots.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_snapshots.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 
 @validate(DEFAULTS, RULES)
 @set_logger()
 @authenticate()
 def discover_snapshots(**kwargs):
     """Discover snapshots based on provided criteria"""
 
-    if kwargs.get("created_before"):
+    if kwargs.get("created_after") and type(kwargs["created_after"]) is str:
+        kwargs["created_after"] = datetime.strptime(kwargs["created_after"], "%Y/%m/%d")
+    if kwargs.get("created_before") and type(kwargs["created_before"]) is str:
         kwargs["created_before"] = datetime.strptime(
             kwargs["created_before"], "%Y/%m/%d"
         )
-    if kwargs.get("created_after"):
-        kwargs["created_after"] = datetime.strptime(kwargs["created_after"], "%Y/%m/%d")
 
     logger.info("Discovering snapshots")
 
     filters = build_filters(**kwargs)
     snapshots = search_snapshots(filters, **kwargs)
 
     logger.info(f"{len(snapshots)} snapshots found")
```

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_tags.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_unused_security_groups.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_unused_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/discover_volumes.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/encrypt_volume.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_tags.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/modify_volumes.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/ec2/share_snapshots.py` & `avtomat_aws-0.1.4/avtomat_aws/services/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/general/get_date.py` & `avtomat_aws-0.1.4/avtomat_aws/services/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/iam/__init__.py` & `avtomat_aws-0.1.4/avtomat_aws/services/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_inactive_console_users.py` & `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_inactive_users.py` & `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_no_mfa_users.py` & `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_no_mfa_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_old_access_keys.py` & `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_old_password_users.py` & `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_unused_access_keys.py` & `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/iam/discover_unused_roles.py` & `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/iam/modify_access_keys.py` & `avtomat_aws-0.1.4/avtomat_aws/services/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/iam/modify_users_console_access.py` & `avtomat_aws-0.1.4/avtomat_aws/services/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/iam/quarantine_user.py` & `avtomat_aws-0.1.4/avtomat_aws/services/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/s3/create_objects.py` & `avtomat_aws-0.1.4/avtomat_aws/services/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/s3/delete_objects.py` & `avtomat_aws-0.1.4/avtomat_aws/services/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/s3/discover_objects.py` & `avtomat_aws-0.1.4/avtomat_aws/services/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/sts/create_session.py` & `avtomat_aws-0.1.4/avtomat_aws/services/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/services/sts/whoami.py` & `avtomat_aws-0.1.4/avtomat_aws/services/sts/whoami.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.3/avtomat_aws/validations/rules.py` & `avtomat_aws-0.1.4/avtomat_aws/validations/rules.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timedelta
 
 
 def required_rule(kwargs, params):
     """Validates that required parameters are provided."""
 
     for param in params:
         if param not in kwargs or kwargs[param] is None:
@@ -41,15 +41,15 @@
 
 def at_most_one_rule(kwargs, params):
     """Validates that at most one of the parameters is provided."""
 
     if len(params) < 2:
         raise ValueError("Rule 'at_most_one' requires at least two parameters")
 
-    params_defined = sum(kwargs.get(param) not in (None, []) for param in params)
+    params_defined = sum(kwargs.get(param) not in (None, [], False) for param in params)
     if params_defined > 1:
         raise ValueError(
             f"The following parameters cannot be used together, select only one: {params}"
         )
 
 
 def at_least_one_rule(kwargs, params):
@@ -68,27 +68,31 @@
         raise ValueError("Cannot set both 'debug' and 'silent' log levels")
 
 
 def date_yymmdd_rule(kwargs, params):
     """Validates that date parameters are in the correct format (YYYY/MM/DD)."""
 
     for param in params:
-        if kwargs.get(param):
+        if kwargs.get(param) and type(kwargs[param]) is str:
             try:
-                kwargs[param] = datetime.strptime(kwargs[param], "%Y/%m/%d")
+                datetime.strptime(kwargs[param], "%Y/%m/%d")
             except ValueError:
                 raise ValueError(
                     f"'{param}' '{kwargs[param]}' does not match the format YYYY/MM/DD"
                 )
 
 
 def cloudtrail_rule(kwargs, params):
     """Validates that a date is not in the future or not more than 90 days in the past."""
 
     for param in params:
-        if kwargs.get(param):
-            if kwargs[param] < datetime.now(timezone.utc) - timedelta(days=90):
-                raise ValueError(
-                    f"'{param}' '{kwargs[param]}' cannot be more than 90 days in the past"
-                )
-            if kwargs[param] > datetime.now(timezone.utc):
-                raise ValueError(f"'{param}' '{kwargs[param]}' cannot be in the future")
+        if type(kwargs[param]) is str:
+            param_date = datetime.strptime(kwargs[param], "%Y/%m/%d")
+        else:
+            param_date = kwargs[param]
+
+        if param_date < datetime.now() - timedelta(days=90):
+            raise ValueError(
+                f"'{param}' '{kwargs[param]}' cannot be more than 90 days in the past"
+            )
+        if param_date > datetime.now():
+            raise ValueError(f"'{param}' '{kwargs[param]}' cannot be in the future")
```

### Comparing `avtomat_aws-0.1.3/pyproject.toml` & `avtomat_aws-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avtomat-aws"
-version = "0.1.3"
+version = "0.1.4"
 description = "A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations."
 authors = ["Dimitar Atanasov <dimitar@avtomat.io>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://avtomat.io"
 documentation = "https://docs.avtomat.io/aws/get_started"
 keywords = ["aws", "cloud", "automation", "cli", "python", "boto3"]
```

### Comparing `avtomat_aws-0.1.3/PKG-INFO` & `avtomat_aws-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avtomat-aws
-Version: 0.1.3
+Version: 0.1.4
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
-Metadata-Version: 2.1 Name: avtomat-aws Version: 0.1.3 Summary: A collection of
+Metadata-Version: 2.1 Name: avtomat-aws Version: 0.1.4 Summary: A collection of
 reusable Amazon Web Services actions, bringing speed and certainty to cloud
 operations. Home-page: https://avtomat.io License: GPL-2.0-only Keywords:
 aws,cloud,automation,cli,python,boto3 Author: Dimitar Atanasov Author-email:
 dimitar@avtomat.io Requires-Python: >=3.9,<4.0 Classifier: Development Status
 :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

