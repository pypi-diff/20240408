# Comparing `tmp/backup_warden-1.0.6.tar.gz` & `tmp/backup_warden-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backup_warden-1.0.6.tar", max compression
+gzip compressed data, was "backup_warden-1.0.7.tar", max compression
```

## Comparing `backup_warden-1.0.6.tar` & `backup_warden-1.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-07-01 04:15:25.842306 backup_warden-1.0.6/LICENSE
--rw-r--r--   0        0        0    17412 2023-07-03 09:25:00.896237 backup_warden-1.0.6/README.md
--rw-r--r--   0        0        0    41618 2023-07-01 09:37:38.396113 backup_warden-1.0.6/backup_warden/__init__.py
--rw-r--r--   0        0        0    11707 2023-07-02 04:19:54.989560 backup_warden-1.0.6/backup_warden/app.py
--rw-r--r--   0        0        0      631 2023-07-03 09:25:33.871105 backup_warden-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    18380 1970-01-01 00:00:00.000000 backup_warden-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-01 04:15:25.842306 backup_warden-1.0.7/LICENSE
+-rw-r--r--   0        0        0    17764 2024-03-22 07:03:27.779145 backup_warden-1.0.7/README.md
+-rw-r--r--   0        0        0    42275 2024-03-22 06:41:38.090294 backup_warden-1.0.7/backup_warden/__init__.py
+-rw-r--r--   0        0        0    11966 2024-03-22 06:56:43.265625 backup_warden-1.0.7/backup_warden/app.py
+-rw-r--r--   0        0        0      630 2024-04-07 23:12:10.674668 backup_warden-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    18731 1970-01-01 00:00:00.000000 backup_warden-1.0.7/PKG-INFO
```

### Comparing `backup_warden-1.0.6/LICENSE` & `backup_warden-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `backup_warden-1.0.6/README.md` & `backup_warden-1.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Thanks to xolox for his work on [rotate-backups](https://github.com/xolox/python-rotate-backups) that gave me a lot of inspiration for this project!
 
 ## Usage
 
 | Option                      | Description                                                                                    | Default Value            |
 | --------------------------- | ---------------------------------------------------------------------------------------------- | ------------------------ |
+| `--minutely`                | Number of minutely backups to preserve                                                         | `0`                      |
 | `--hourly`                  | Number of hourly backups to preserve                                                           | `72`                     |
 | `--daily`                   | Number of daily backups to preserve                                                            | `7`                      |
 | `--weekly`                  | Number of weekly backups to preserve                                                           | `6`                      |
 | `--monthly`                 | Number of monthly backups to preserve                                                          | `12`                     |
 | `--yearly`                  | Number of yearly backups to preserve                                                           | `always`                 |
 | `-c`, `--config`            | Location of the config file                                                                    | `/etc/backup_warden.ini` |
 | `-s`, `--source`            | Source of where the backups are stored. Select from: `local`, `ssh`, `s3`                      | `local`                  |
@@ -23,25 +24,26 @@
 | `-I`, `--include`           | Include backups based on their directory path and/or filename (separated by comma)             |                          |
 | `-E`, `--exclude`           | Exclude backups based on their directory path and/or filename (separated by comma)             |                          |
 | `-H`, `--ssh-host`          | SSH host/alias to use                                                                          |                          |
 | `--ssh-sudo`                | Wrap SSH commands with sudo for escalated privileges                                           | `False`                  |
 | `--filestat`                | Use the file's last modified date instead of parsing timestamp from filename                   | `False`                  |
 | `--prefer-recent`           | Keep the most recent backup in each time slot instead of oldest                                | `False`                  |
 | `--relaxed`                 | Time windows are not enforced                                                                  | `False`                  |
+| `--utc`                     | Use UTC timezone instead of local machine's timezone for timestamps                            | `False`                  |
 | `--syslog`                  | Use syslog                                                                                     | `False`                  |
 | `--debug`                   | Log debug messages that can help troubleshoot                                                  | `False`                  |
 | `--delete`                  | Commit to deleting backups (DANGER ZONE)                                                       | `False`                  |
 | `-V`, `--version`           | Display version and exit                                                                       |                          |
 | `-h`, `--help`              | Show this help message and exit                                                                |                          |
 
 **Note**: Boolean options such as `--filestat` can be specified as `yes`/`no`, `true`/`false`, or `1`/`0` in the config
 
 ### Additional Information for Options
 
-#### Option: `hourly`, `daily`, `weekly`, `monthly`, `yearly`
+#### Option: `minutely`, `hourly`, `daily`, `weekly`, `monthly`, `yearly`
 
 - These options determine the number of backups to retain for each respective frequency
 - You have the flexibility to provide an expression that will be evaluated to calculate a value. For example, using `--hourly=5+2` would result in 7
 - Alternatively, you can specify "always" as the value to preserve all backups for that particular frequency
 
 #### Option: `source`
 There are currently three available sources, each functioning differently when scanning directories to find backups.
@@ -103,15 +105,15 @@
 
 In cases where your backup files do not contain a timestamp, you have the option to use the last modified time of the backup instead. However, it is important to note that when utilizing this parameter, you will also need to modify the `timestamp-pattern` to accurately identify which directories/files are considered backups. For example, if all of your backups have filenames starting with "backup-", you would change the `timestamp-pattern` to `backup-\S+`.
 
 If your backup file names are not standardized and do not follow a specific pattern, this feature is currently not supported.
 
 #### Option: `relaxed`
 
-Backup Warden offers the `--relaxed` option to modify its default rotation behavior. By default, Backup Warden enforces strict time windows for each rotation scheme. However, with the `--relaxed` option, you can relax this enforcement. Here's a clear explanation of the difference between strict and relaxed rotation:
+Backup Warden offers the `--relaxed` option to modify its default rotation behavior. By default, Backup Warden enforces strict time windows for each rotation scheme. However, with the `--relaxed` option, you can relax this enforcement. Here's a clear explanation/example of the difference between strict and relaxed rotation:
 
 - **Strict Rotation**: When the number of hourly backups to preserve is set to three, only backups created within the relevant time window (the hour of the most recent backup and the two hours leading up to it) will match the hourly frequency. Choose this option if your backups are created at regular intervals without any missed intervals
 
 - **Relaxed Rotation**: With the `--relaxed` option enabled, the three most recent backups will all match the hourly frequency and be preserved, regardless of the calculated time window. Choose this option if your backups are created at irregular intervals, as it allows for the preservation of more backups
 
 #### Option: `include-list`/`exclude-list`
 
@@ -177,20 +179,21 @@
 - `s3_endpoint_url`
 - `s3_access_key_id`
 - `s3_secret_access_key`
 - `slack_webhook`
 
 For each config `[path]` section, you can set the following options:
 
-- `hourly`, `daily`, `weekly`, `monthly`, `yearly`
+- `minutely`, `hourly`, `daily`, `weekly`, `monthly`, `yearly`
 - `timestamp_pattern`
 - `include_list`/`exclude_list`
 - `filestat`
 - `relaxed`
 - `prefer_recent`
+- `utc`
 
 You can also set the following options using environment variables, which will override the corresponding config values:
 
 - `S3_ENDPOINT_URL`
 - `AWS_ACCESS_KEY_ID`
 - `AWS_SECRET_ACCESS_KEY`
 - `SLACK_WEBHOOK`
```

### Comparing `backup_warden-1.0.6/backup_warden/__init__.py` & `backup_warden-1.0.7/backup_warden/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Inspiration from https://github.com/xolox/python-rotate-backups
 
 import os
 import re
 import shutil
 from configparser import ConfigParser
 from dataclasses import dataclass, field
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from fnmatch import fnmatch
 from pathlib import Path
 from pprint import pformat
 from typing import List
 
 import boto3
 from botocore.exceptions import ClientError
@@ -38,14 +38,15 @@
 SOURCE_TYPES = [SOURCE_S3, SOURCE_LOCAL, SOURCE_SSH]
 
 """
 A dictionary with rotation frequency names (strings) as keys and
 :class:`~dateutil.relativedelta.relativedelta` objects as values.
 """
 SUPPORTED_FREQUENCIES = {
+    "minutely": relativedelta(minutes=1),
     "hourly": relativedelta(hours=1),
     "daily": relativedelta(days=1),
     "weekly": relativedelta(weeks=1),
     "monthly": relativedelta(months=1),
     "yearly": relativedelta(years=1),
 }
 
@@ -87,14 +88,15 @@
     rotation_scheme: dict
     timestamp_pattern: re.Pattern
     include_list: List[str] = field(default_factory=list)
     exclude_list: List[str] = field(default_factory=list)
     relaxed: bool = False
     filestat: bool = False
     prefer_recent: bool = False
+    utc: bool = False
 
     def __post_init__(self):
         self.timestamp_pattern = compile_timestamp_pattern(self.timestamp_pattern, self.filestat)
 
         if isinstance(self.include_list, str):
             self.include_list = split(self.include_list)
         if isinstance(self.exclude_list, str):
@@ -235,35 +237,40 @@
         :param backup_path: The backup path.
         :param config: The configuration for the path.
         :return: The extracted timestamp as a datetime object, or None if no timestamp is found.
         """
 
         backup_name = backup_path.name
 
+        if config.utc:
+            specified_timezone = timezone.utc
+        else:
+            specified_timezone = datetime.now().astimezone().tzinfo
+
         timestamp_extract = config.timestamp_pattern.search(backup_name)
         if timestamp_extract:
             unixtime = timestamp_extract.groupdict().get("unixtime")
             if unixtime:
                 unixtime = int(unixtime)
                 # Support seconds and milliseconds-precision timestamps
                 for time in (unixtime, unixtime / 1000):
                     try:
-                        return datetime.fromtimestamp(time)
+                        return datetime.fromtimestamp(time, tz=specified_timezone)
                     except ValueError:
                         pass
 
                 logger.debug(f"Unable to parse unix timestamp from {backup_path}")
             elif config.filestat:
                 if self.source in (SOURCE_LOCAL, SOURCE_SSH):
-                    return datetime.fromtimestamp(int(last_modified))
+                    return datetime.fromtimestamp(int(last_modified), tz=specified_timezone)
                 elif self.source == SOURCE_S3:
                     return last_modified.replace(tzinfo=None)
             else:
                 try:
-                    return datetime(*map(int, timestamp_extract.groups("0")))
+                    return datetime(*map(int, timestamp_extract.groups("0")), tzinfo=specified_timezone)
                 except ValueError:
                     pass
 
         # No timestamp or file match for filestat found, indicating no relevant timestamp
         return None
 
     def collect_backups(self):
@@ -526,27 +533,28 @@
                 frequencies ('hourly', 'daily', etc.) and whose values are
                 dictionaries. Each nested dictionary contains lists of
                 :class:`Backup` objects that are grouped together because
                 they belong into the same time unit for the corresponding
                 rotation frequency.
         """
         frequency_key_mapping = {
+            "minutely": lambda b: (b.year, b.month, b.day, b.hour, b.minute),
             "hourly": lambda b: (b.year, b.month, b.day, b.hour),
             "daily": lambda b: (b.year, b.month, b.day),
             "weekly": lambda b: (b.year, b.week),
             "monthly": lambda b: (b.year, b.month),
             "yearly": lambda b: b.year,
         }
 
         backups_by_frequency = {frequency: {} for frequency in SUPPORTED_FREQUENCIES}
 
         for b in backups:
             for frequency, key_mapping in frequency_key_mapping.items():
                 # If frequency is set to 0, don't add it
-                if self.config.rotation_scheme[frequency] != 0:
+                if self.config.rotation_scheme.get(frequency) != 0:
                     key = key_mapping(b)
                     backups_by_frequency[frequency].setdefault(key, []).append(b)
 
         return backups_by_frequency
 
     def apply_rotation_scheme(self, backups_by_frequency, most_recent_backup):
         """
@@ -579,22 +587,24 @@
                     selected_backup = list(backups_in_period)[index]
                     backups[period] = [selected_backup]
 
                 # Check if we need to rotate away backups in old periods.
                 retention_period = rotation_scheme[frequency]
 
                 if retention_period != "always":
+                    # Remove backups created before the minimum date of this
+                    # rotation frequency? (relative to the most recent backup)
                     if not self.config.relaxed:
                         minimum_date = most_recent_backup - SUPPORTED_FREQUENCIES[frequency] * retention_period
-                        for period, backups_in_period in list(backups.items()):
+                        for backup, backups_in_period in list(backups.items()):
                             backups_in_period[:] = [
                                 backup for backup in backups_in_period if backup.timestamp >= minimum_date
                             ]
                             if not backups_in_period:
-                                backups.pop(period)
+                                backups.pop(backup)
 
                     # If there are more periods remaining than the user
                     # requested to be preserved we delete the oldest one(s).
                     items_to_preserve = list(backups.items())[-retention_period:]
                     backups_by_frequency[frequency] = dict(items_to_preserve)
 
     def find_preservation_criteria(self, backups_by_frequency):
@@ -651,15 +661,15 @@
             backups = sorted(warden_backups.backups, key=lambda b: b.timestamp)
             if backups:
                 most_recent_backup: Backup = backups[-1]
                 backups_by_frequency = self.group_backups(backups)
                 self.apply_rotation_scheme(backups_by_frequency, most_recent_backup.timestamp)
                 backups_to_preserve = self.find_preservation_criteria(backups_by_frequency)
 
-                if most_recent_backup.timestamp < (datetime.utcnow() - timedelta(1)):
+                if most_recent_backup.timestamp < (datetime.now(timezone.utc) - timedelta(1)):
                     no_backups_24hrs.append(path_name)
                     warning_message = (
                         f"No backup taken for path {path_name} in the past 24 hours! Most recent backup:"
                         f" {most_recent_backup.timestamp}"
                     )
                     logger.error(warning_message)
                     slack_notify(
@@ -756,23 +766,25 @@
             if path_backup_files_count:
                 self.tabulate_rows.append(["", "", "", ""])
                 self.tabulate_rows.append(
                     [
                         f"Total: {path_backup_files_count}",
                         "",
                         convert_bytes(path_backup_size),
-                        "All backups preserved"
-                        if not path_backup_deleted_files_count
-                        else (
-                            f"Deleted {path_backup_deleted_files_count} backups totaling"
-                            f" {convert_bytes(path_backup_deleted_size)}"
-                            if self.delete
+                        (
+                            "All backups preserved"
+                            if not path_backup_deleted_files_count
                             else (
                                 f"Deleted {path_backup_deleted_files_count} backups totaling"
-                                f" {convert_bytes(path_backup_deleted_size)} (skipped)"
+                                f" {convert_bytes(path_backup_deleted_size)}"
+                                if self.delete
+                                else (
+                                    f"Deleted {path_backup_deleted_files_count} backups totaling"
+                                    f" {convert_bytes(path_backup_deleted_size)} (skipped)"
+                                )
                             )
                         ),
                     ]
                 )
                 self.print_tabulate()
             else:
                 print()
@@ -882,15 +894,15 @@
                         config_value = config.get(section, option, fallback=None)
 
                     config_data[option] = config_value
         elif not app_config and section != "main":
             rotation_scheme = {
                 name: parse_timestamp_frequency(config.get(section, name, fallback=""))
                 for name in SUPPORTED_FREQUENCIES
-                if config.get(section, name)
+                if config.get(section, name, fallback=None)
             }
 
             config_options = {"config_name": section, "rotation_scheme": rotation_scheme}
 
             # We create a config section based off of the keys in Warden_Config object
             for option, data_type in Warden_Config.__annotations__.items():
                 # These options won't be in the config file
```

### Comparing `backup_warden-1.0.6/backup_warden/app.py` & `backup_warden-1.0.7/backup_warden/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,26 +108,27 @@
 
     try:
         check_for_update()
 
         # Create rotation scheme and remove from options so they don't get sent to BackupWarden
         rotation_scheme = {
             frequency: parse_timestamp_frequency(options.pop(frequency, None))
-            for frequency in ("hourly", "daily", "weekly", "monthly", "yearly")
+            for frequency in ("minutely", "hourly", "daily", "weekly", "monthly", "yearly")
         }
 
         # Create our parameter config as a default
         config = Warden_Config(
             config_name="parameters",
             rotation_scheme=rotation_scheme,
             timestamp_pattern=options.pop("timestamp_pattern"),
             filestat=options.pop("filestat"),
             include_list=options.pop("include_list"),
             exclude_list=options.pop("exclude_list"),
             relaxed=options.pop("relaxed"),
+            utc=options.pop("utc"),
             prefer_recent=options.pop("prefer_recent"),
         )
 
         # Remove syslog from options so it isn't sent to BackupWarden since it's only used here
         options.pop("syslog")
 
         backup_warden = BackupWarden(config=config, **options)
@@ -250,14 +251,17 @@
     )
     parser.add_argument(
         "--relaxed",
         action="store_true",
         help="Time windows are not enforced (see documentation for more information)",
     )
     parser.add_argument(
+        "--utc", action="store_true", help="Use UTC timezone instead of local machine's timezone for timestamps"
+    )
+    parser.add_argument(
         "--syslog",
         dest="syslog",
         action="store_true",
         help="Use syslog",
     )
     parser.add_argument(
         "--debug",
@@ -269,14 +273,15 @@
         action="store_true",
         help="Commit to deleting backups (DANGER ZONE)",
     )
     parser.add_argument("-V", "--version", action="version", version=__version__, help="Display version and exit")
 
     retention_group = parser.add_argument_group("Retention options")
     retention_options = [
+        ("minutely", "Number of minutely backups to preserve", 0),
         ("hourly", "Number of hourly backups to preserve", 72),
         ("daily", "Number of daily backups to preserve", 7),
         ("weekly", "Number of weekly backups to preserve", 6),
         ("monthly", "Number of monthly backups to preserve", 12),
         ("yearly", "Number of yearly backups to preserve", "always"),
     ]
     for option_name, option_help, option_default in retention_options:
```

### Comparing `backup_warden-1.0.6/pyproject.toml` & `backup_warden-1.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "backup_warden"
-version = "1.0.6"
+version = "1.0.7"
 description = "Streamline your backup management with ease and simplicity"
 authors = ["Charles Thompson <01charles.t@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-boto3 = "^1.26.146"
+boto3 = "^1.34.79"
 tabulate = "^0.9.0"
-slack-sdk = "^3.21.3"
-loguru = "^0.7.0"
-configparser = "^5.3.0"
+slack-sdk = "^3.27.1"
+loguru = "^0.7.2"
+configparser = "^6.0.1"
 property-manager = "^3.0"
-paramiko = "^3.2.0"
-fabric = "^3.1.0"
+paramiko = "^3.4.0"
+fabric = "^3.2.2"
 simpleeval = "^0.9.13"
 requests = "^2.31.0"
-packaging = "^23.1"
+packaging = "^24.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 backup-warden = "backup_warden.app:main"
```

### Comparing `backup_warden-1.0.6/PKG-INFO` & `backup_warden-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
-Name: backup-warden
-Version: 1.0.6
+Name: backup_warden
+Version: 1.0.7
 Summary: Streamline your backup management with ease and simplicity
 Author: Charles Thompson
 Author-email: 01charles.t@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: boto3 (>=1.26.146,<2.0.0)
-Requires-Dist: configparser (>=5.3.0,<6.0.0)
-Requires-Dist: fabric (>=3.1.0,<4.0.0)
-Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: packaging (>=23.1,<24.0)
-Requires-Dist: paramiko (>=3.2.0,<4.0.0)
+Requires-Dist: boto3 (>=1.34.79,<2.0.0)
+Requires-Dist: configparser (>=6.0.1,<7.0.0)
+Requires-Dist: fabric (>=3.2.2,<4.0.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: packaging (>=24.0,<25.0)
+Requires-Dist: paramiko (>=3.4.0,<4.0.0)
 Requires-Dist: property-manager (>=3.0,<4.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: simpleeval (>=0.9.13,<0.10.0)
-Requires-Dist: slack-sdk (>=3.21.3,<4.0.0)
+Requires-Dist: slack-sdk (>=3.27.1,<4.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Backup Warden
 
 In today's digital landscape, every business is taking backups of their data (hopefully). These backups can be challenging as they often require substantial disk space and/or cloud storage that can lead to significant financial expenses. If you're in search of a solution to handle your backups and retain only the necessary ones according to your retention policies, look no further! With Backup Warden, it will supervise and maintain your backups simplifying your overall data life cycle and enabling you to have smarter resource utilization.
 
 Thanks to xolox for his work on [rotate-backups](https://github.com/xolox/python-rotate-backups) that gave me a lot of inspiration for this project!
 
 ## Usage
 
 | Option                      | Description                                                                                    | Default Value            |
 | --------------------------- | ---------------------------------------------------------------------------------------------- | ------------------------ |
+| `--minutely`                | Number of minutely backups to preserve                                                         | `0`                      |
 | `--hourly`                  | Number of hourly backups to preserve                                                           | `72`                     |
 | `--daily`                   | Number of daily backups to preserve                                                            | `7`                      |
 | `--weekly`                  | Number of weekly backups to preserve                                                           | `6`                      |
 | `--monthly`                 | Number of monthly backups to preserve                                                          | `12`                     |
 | `--yearly`                  | Number of yearly backups to preserve                                                           | `always`                 |
 | `-c`, `--config`            | Location of the config file                                                                    | `/etc/backup_warden.ini` |
 | `-s`, `--source`            | Source of where the backups are stored. Select from: `local`, `ssh`, `s3`                      | `local`                  |
@@ -48,25 +49,26 @@
 | `-I`, `--include`           | Include backups based on their directory path and/or filename (separated by comma)             |                          |
 | `-E`, `--exclude`           | Exclude backups based on their directory path and/or filename (separated by comma)             |                          |
 | `-H`, `--ssh-host`          | SSH host/alias to use                                                                          |                          |
 | `--ssh-sudo`                | Wrap SSH commands with sudo for escalated privileges                                           | `False`                  |
 | `--filestat`                | Use the file's last modified date instead of parsing timestamp from filename                   | `False`                  |
 | `--prefer-recent`           | Keep the most recent backup in each time slot instead of oldest                                | `False`                  |
 | `--relaxed`                 | Time windows are not enforced                                                                  | `False`                  |
+| `--utc`                     | Use UTC timezone instead of local machine's timezone for timestamps                            | `False`                  |
 | `--syslog`                  | Use syslog                                                                                     | `False`                  |
 | `--debug`                   | Log debug messages that can help troubleshoot                                                  | `False`                  |
 | `--delete`                  | Commit to deleting backups (DANGER ZONE)                                                       | `False`                  |
 | `-V`, `--version`           | Display version and exit                                                                       |                          |
 | `-h`, `--help`              | Show this help message and exit                                                                |                          |
 
 **Note**: Boolean options such as `--filestat` can be specified as `yes`/`no`, `true`/`false`, or `1`/`0` in the config
 
 ### Additional Information for Options
 
-#### Option: `hourly`, `daily`, `weekly`, `monthly`, `yearly`
+#### Option: `minutely`, `hourly`, `daily`, `weekly`, `monthly`, `yearly`
 
 - These options determine the number of backups to retain for each respective frequency
 - You have the flexibility to provide an expression that will be evaluated to calculate a value. For example, using `--hourly=5+2` would result in 7
 - Alternatively, you can specify "always" as the value to preserve all backups for that particular frequency
 
 #### Option: `source`
 There are currently three available sources, each functioning differently when scanning directories to find backups.
@@ -128,15 +130,15 @@
 
 In cases where your backup files do not contain a timestamp, you have the option to use the last modified time of the backup instead. However, it is important to note that when utilizing this parameter, you will also need to modify the `timestamp-pattern` to accurately identify which directories/files are considered backups. For example, if all of your backups have filenames starting with "backup-", you would change the `timestamp-pattern` to `backup-\S+`.
 
 If your backup file names are not standardized and do not follow a specific pattern, this feature is currently not supported.
 
 #### Option: `relaxed`
 
-Backup Warden offers the `--relaxed` option to modify its default rotation behavior. By default, Backup Warden enforces strict time windows for each rotation scheme. However, with the `--relaxed` option, you can relax this enforcement. Here's a clear explanation of the difference between strict and relaxed rotation:
+Backup Warden offers the `--relaxed` option to modify its default rotation behavior. By default, Backup Warden enforces strict time windows for each rotation scheme. However, with the `--relaxed` option, you can relax this enforcement. Here's a clear explanation/example of the difference between strict and relaxed rotation:
 
 - **Strict Rotation**: When the number of hourly backups to preserve is set to three, only backups created within the relevant time window (the hour of the most recent backup and the two hours leading up to it) will match the hourly frequency. Choose this option if your backups are created at regular intervals without any missed intervals
 
 - **Relaxed Rotation**: With the `--relaxed` option enabled, the three most recent backups will all match the hourly frequency and be preserved, regardless of the calculated time window. Choose this option if your backups are created at irregular intervals, as it allows for the preservation of more backups
 
 #### Option: `include-list`/`exclude-list`
 
@@ -202,20 +204,21 @@
 - `s3_endpoint_url`
 - `s3_access_key_id`
 - `s3_secret_access_key`
 - `slack_webhook`
 
 For each config `[path]` section, you can set the following options:
 
-- `hourly`, `daily`, `weekly`, `monthly`, `yearly`
+- `minutely`, `hourly`, `daily`, `weekly`, `monthly`, `yearly`
 - `timestamp_pattern`
 - `include_list`/`exclude_list`
 - `filestat`
 - `relaxed`
 - `prefer_recent`
+- `utc`
 
 You can also set the following options using environment variables, which will override the corresponding config values:
 
 - `S3_ENDPOINT_URL`
 - `AWS_ACCESS_KEY_ID`
 - `AWS_SECRET_ACCESS_KEY`
 - `SLACK_WEBHOOK`
```

