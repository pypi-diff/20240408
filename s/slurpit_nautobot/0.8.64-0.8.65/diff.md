# Comparing `tmp/slurpit_nautobot-0.8.64.tar.gz` & `tmp/slurpit_nautobot-0.8.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurpit_nautobot-0.8.64.tar", max compression
+gzip compressed data, was "slurpit_nautobot-0.8.65.tar", max compression
```

## Comparing `slurpit_nautobot-0.8.64.tar` & `slurpit_nautobot-0.8.65.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0     1064 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.64/LICENSE
--rw-r--r--   0        0        0       19 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.64/README.md
--rw-r--r--   0        0        0      559 2024-03-27 13:32:42.658329 slurpit_nautobot-0.8.64/pyproject.toml
--rw-r--r--   0        0        0     1262 2024-03-27 13:32:42.658329 slurpit_nautobot-0.8.64/src/slurpit_nautobot/__init__.py
--rw-r--r--   0        0        0       46 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/api/__init__.py
--rw-r--r--   0        0        0     1834 2024-03-17 15:46:59.051385 slurpit_nautobot-0.8.64/src/slurpit_nautobot/api/serializers.py
--rw-r--r--   0        0        0      484 2024-03-17 21:19:15.970312 slurpit_nautobot-0.8.64/src/slurpit_nautobot/api/urls.py
--rw-r--r--   0        0        0     9406 2024-03-27 01:08:33.602394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/api/views.py
--rw-r--r--   0        0        0     2547 2024-03-27 01:08:33.602394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/decorators.py
--rw-r--r--   0        0        0     2040 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/filtersets.py
--rw-r--r--   0        0        0     7715 2024-03-27 01:08:33.602394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/forms.py
--rw-r--r--   0        0        0    10458 2024-03-27 01:08:33.602394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/importer.py
--rw-r--r--   0        0        0        0 2024-03-27 13:32:42.698330 slurpit_nautobot-0.8.64/src/slurpit_nautobot/management/__init__.py
--rw-r--r--   0        0        0     1159 2024-03-27 01:08:33.602394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/management/choices.py
--rw-r--r--   0        0        0     9130 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/migrations/0001_initial.py
--rw-r--r--   0        0        0     1053 2024-03-17 14:29:31.470119 slurpit_nautobot-0.8.64/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py
--rw-r--r--   0        0        0      749 2024-03-27 01:08:33.606394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/migrations/0003_manufacturer.py
--rw-r--r--   0        0        0        0 2024-03-27 13:32:42.702330 slurpit_nautobot-0.8.64/src/slurpit_nautobot/migrations/__init__.py
--rw-r--r--   0        0        0     4912 2024-03-27 01:08:33.606394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/models/__init__.py
--rw-r--r--   0        0        0     2804 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/models/device.py
--rw-r--r--   0        0        0     1409 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/models/logs.py
--rw-r--r--   0        0        0      411 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/models/mapping.py
--rw-r--r--   0        0        0      762 2024-03-17 14:29:31.470119 slurpit_nautobot-0.8.64/src/slurpit_nautobot/models/planning.py
--rw-r--r--   0        0        0     1146 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/models/setting.py
--rw-r--r--   0        0        0     1975 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/navigation.py
--rw-r--r--   0        0        0      101 2024-03-27 01:08:33.606394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/references/__init__.py
--rw-r--r--   0        0        0     1888 2024-03-27 01:08:33.606394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/references/generic.py
--rw-r--r--   0        0        0      648 2024-03-27 01:08:33.606394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/references/imports.py
--rw-r--r--   0        0        0      286 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/search.py
--rw-r--r--   0        0        0      528 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/slurpitch.py
--rw-r--r--   0        0        0     4757 2024-03-27 01:08:33.606394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/tables.py
--rw-r--r--   0        0        0     1181 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/template_content.py
--rw-r--r--   0        0        0     2382 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html
--rw-r--r--   0        0        0     1623 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html
--rw-r--r--   0        0        0     3425 2024-03-27 10:33:21.020348 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html
--rw-r--r--   0        0        0    22100 2024-03-27 01:08:33.610394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html
--rw-r--r--   0        0        0      352 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/commingsoon.html
--rw-r--r--   0        0        0    17724 2024-03-27 01:08:33.610394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html
--rw-r--r--   0        0        0     3519 2024-03-27 01:08:33.610394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html
--rw-r--r--   0        0        0     3505 2024-03-27 01:08:33.610394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html
--rw-r--r--   0        0        0     6485 2024-03-27 01:08:33.610394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html
--rw-r--r--   0        0        0      475 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/onboarded_device_list.html
--rw-r--r--   0        0        0     3832 2024-03-27 10:33:21.020348 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html
--rw-r--r--   0        0        0     3880 2024-03-27 01:08:33.610394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html
--rw-r--r--   0        0        0     3177 2024-03-27 01:08:33.614394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html
--rw-r--r--   0        0        0     9226 2024-03-27 13:15:42.835761 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html
--rw-r--r--   0        0        0     2368 2024-03-27 10:33:21.020348 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html
--rw-r--r--   0        0        0     2644 2024-03-27 10:33:21.020348 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html
--rw-r--r--   0        0        0     2915 2024-03-27 01:08:33.614394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/table.html
--rw-r--r--   0        0        0      350 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/table1.html
--rw-r--r--   0        0        0     1162 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/urls.py
--rw-r--r--   0        0        0      459 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/utilities.py
--rw-r--r--   0        0        0     1490 2024-03-27 01:08:33.614394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/validator.py
--rw-r--r--   0        0        0      298 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/views/__init__.py
--rw-r--r--   0        0        0    10128 2024-03-27 01:08:33.614394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/views/datamapping.py
--rw-r--r--   0        0        0     1073 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/views/logging.py
--rw-r--r--   0        0        0    13967 2024-03-27 01:08:33.614394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/views/onboarding.py
--rw-r--r--   0        0        0      520 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.64/src/slurpit_nautobot/views/reconcile.py
--rw-r--r--   0        0        0    17695 2024-03-27 01:08:33.618394 slurpit_nautobot-0.8.64/src/slurpit_nautobot/views/setting.py
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 slurpit_nautobot-0.8.64/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.65/LICENSE
+-rw-r--r--   0        0        0       19 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.65/README.md
+-rw-r--r--   0        0        0      559 2024-04-08 13:55:12.915067 slurpit_nautobot-0.8.65/pyproject.toml
+-rw-r--r--   0        0        0     1262 2024-04-08 13:55:12.915067 slurpit_nautobot-0.8.65/src/slurpit_nautobot/__init__.py
+-rw-r--r--   0        0        0       46 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/api/__init__.py
+-rw-r--r--   0        0        0     1993 2024-04-08 11:09:53.805564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/api/serializers.py
+-rw-r--r--   0        0        0      484 2024-03-17 21:19:15.970312 slurpit_nautobot-0.8.65/src/slurpit_nautobot/api/urls.py
+-rw-r--r--   0        0        0     9406 2024-04-08 11:09:53.805564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/api/views.py
+-rw-r--r--   0        0        0     2547 2024-04-08 11:09:53.805564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/decorators.py
+-rw-r--r--   0        0        0     2040 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/filtersets.py
+-rw-r--r--   0        0        0     7715 2024-04-08 11:09:53.805564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/forms.py
+-rw-r--r--   0        0        0    10458 2024-04-08 11:09:53.809564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/importer.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:55:12.971067 slurpit_nautobot-0.8.65/src/slurpit_nautobot/management/__init__.py
+-rw-r--r--   0        0        0     1159 2024-04-08 11:09:53.809564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/management/choices.py
+-rw-r--r--   0        0        0     9130 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1053 2024-03-17 14:29:31.470119 slurpit_nautobot-0.8.65/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py
+-rw-r--r--   0        0        0      749 2024-04-08 11:09:53.809564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/migrations/0003_manufacturer.py
+-rw-r--r--   0        0        0      763 2024-04-08 11:09:53.809564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:55:12.971067 slurpit_nautobot-0.8.65/src/slurpit_nautobot/migrations/__init__.py
+-rw-r--r--   0        0        0     4984 2024-04-08 13:55:12.915067 slurpit_nautobot-0.8.65/src/slurpit_nautobot/models/__init__.py
+-rw-r--r--   0        0        0     3069 2024-04-08 11:09:53.809564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/models/device.py
+-rw-r--r--   0        0        0     1409 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/models/logs.py
+-rw-r--r--   0        0        0      411 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/models/mapping.py
+-rw-r--r--   0        0        0      844 2024-04-08 11:09:53.809564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/models/planning.py
+-rw-r--r--   0        0        0     1146 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/models/setting.py
+-rw-r--r--   0        0        0     1975 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/navigation.py
+-rw-r--r--   0        0        0      101 2024-04-08 11:09:53.809564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/references/__init__.py
+-rw-r--r--   0        0        0     1888 2024-04-08 11:09:53.809564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/references/generic.py
+-rw-r--r--   0        0        0      648 2024-04-08 11:09:53.813564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/references/imports.py
+-rw-r--r--   0        0        0      286 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/search.py
+-rw-r--r--   0        0        0      528 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/slurpitch.py
+-rw-r--r--   0        0        0     4757 2024-04-08 11:09:53.813564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/tables.py
+-rw-r--r--   0        0        0     1181 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/template_content.py
+-rw-r--r--   0        0        0     3832 2024-04-08 11:09:53.813564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html
+-rw-r--r--   0        0        0     1623 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html
+-rw-r--r--   0        0        0     3425 2024-04-08 11:09:53.813564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html
+-rw-r--r--   0        0        0    22100 2024-04-08 11:09:53.813564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html
+-rw-r--r--   0        0        0      352 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/commingsoon.html
+-rw-r--r--   0        0        0    17724 2024-04-08 11:09:53.813564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html
+-rw-r--r--   0        0        0     3547 2024-04-08 11:09:53.817564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html
+-rw-r--r--   0        0        0     3533 2024-04-08 11:09:53.817564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html
+-rw-r--r--   0        0        0     6485 2024-04-08 11:09:53.817564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html
+-rw-r--r--   0        0        0      475 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/onboarded_device_list.html
+-rw-r--r--   0        0        0     3549 2024-04-08 11:09:53.817564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html
+-rw-r--r--   0        0        0     4275 2024-04-08 11:09:53.817564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html
+-rw-r--r--   0        0        0     3177 2024-04-08 11:09:53.821564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html
+-rw-r--r--   0        0        0     9226 2024-04-08 11:09:53.821564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html
+-rw-r--r--   0        0        0     2368 2024-04-08 11:09:53.821564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html
+-rw-r--r--   0        0        0     2841 2024-04-08 11:09:53.821564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html
+-rw-r--r--   0        0        0     2915 2024-04-08 11:09:53.821564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/table.html
+-rw-r--r--   0        0        0      350 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/table1.html
+-rw-r--r--   0        0        0     1162 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/urls.py
+-rw-r--r--   0        0        0      459 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/utilities.py
+-rw-r--r--   0        0        0     1490 2024-04-08 11:09:53.821564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/validator.py
+-rw-r--r--   0        0        0      298 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/views/__init__.py
+-rw-r--r--   0        0        0    10130 2024-04-08 11:09:53.821564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/views/datamapping.py
+-rw-r--r--   0        0        0     1073 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/views/logging.py
+-rw-r--r--   0        0        0    13967 2024-04-08 11:09:53.825564 slurpit_nautobot-0.8.65/src/slurpit_nautobot/views/onboarding.py
+-rw-r--r--   0        0        0      520 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.65/src/slurpit_nautobot/views/reconcile.py
+-rw-r--r--   0        0        0    18125 2024-04-08 13:55:12.915067 slurpit_nautobot-0.8.65/src/slurpit_nautobot/views/setting.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 slurpit_nautobot-0.8.65/PKG-INFO
```

### Comparing `slurpit_nautobot-0.8.64/LICENSE` & `slurpit_nautobot-0.8.65/LICENSE`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/pyproject.toml` & `slurpit_nautobot-0.8.65/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slurpit_nautobot"
-version = "0.8.64"
+version = "0.8.65"
 description = ""
 authors = ["Pieter <pieter@slurpit.io>"]
 readme = "README.md"
 packages = [{include = "slurpit_nautobot", from = "src"}]
 
 
 [tool.poetry.dependencies]
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/__init__.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nautobot.apps import NautobotAppConfig
 from nautobot.apps import config as app_config
 
 class SlurpitConfig(NautobotAppConfig):
     name = "slurpit_nautobot"
     verbose_name = "Slurp'it Plugin"
     description = "Sync Slurp'it into Nautobot"
-    version = '0.8.64'
+    version = '0.8.65'
     base_url = "slurpit"   
     default_settings = {
         'DeviceType': {'model': "Slurp'it"},
         'Role': {'name': "Slurp'it"},
         'Location': {'name': 'Slurp\'it'},
         'LocationType': {'name': 'Slurp\'it'},
         'Region': {'name': 'Slurp\'it'},
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/api/serializers.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/api/serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,17 +17,18 @@
     comment = serializers.CharField(source='comments')
 
     class Meta:
         model = SlurpitPlanning
         fields = ['id', "name", "comment", "display"]
 
 class SlurpitStagedDeviceSerializer(NautobotModelSerializer):
+    id = serializers.IntegerField(source='slurpit_id')
     class Meta:
         model = SlurpitStagedDevice
-        fields = '__all__'
+        fields = ['id', 'disabled', 'hostname', 'fqdn', 'ipv4', 'device_os', 'device_type', 'brand', 'createddate', 'changeddate']
 
 class SlurpitSnapshotSerializer(NautobotModelSerializer):
     class Meta:
         model = SlurpitSnapshot
         fields = '__all__'
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/api/views.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/api/views.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/decorators.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/decorators.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/filtersets.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/filtersets.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/forms.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/forms.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/importer.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/importer.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/management/choices.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/management/choices.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/migrations/0001_initial.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/migrations/0003_manufacturer.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/migrations/0003_manufacturer.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/models/__init__.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,34 +91,39 @@
                 type=CustomFieldTypeChoices.TYPE_TEXT,
                 description="",
                 label='Ipv4',
                 grouping="Slurp'it",
                 )
     cf.content_types.set({device})
 
-
-def add_default_mandatory_objects(tags):
-    manu, _ = Manufacturer.objects.get_or_create(**get_config('Manufacturer'))
-    dtype, _ = DeviceType.objects.get_or_create(manufacturer=manu, **get_config('DeviceType'))
-    tenant, _ = Tenant.objects.get_or_create(**get_config('Tenant'))
-    location_type, _ = LocationType.objects.get_or_create(**get_config('LocationType'))
-    location_active_status = Status.objects.get_for_model(Location).all()[0]
-    location, _ = Location.objects.get_or_create(location_type=location_type, status=location_active_status, **get_config('Location'))
-    role, _ = Role.objects.get_or_create(**get_config('Role'))
+def create_default_data_mapping():
     SlurpitMapping.objects.all().delete()
 
     mappings = [
         {"source_field": "hostname", "target_field": "device|name", "mapping_type": "device"},
         {"source_field": "fqdn", "target_field": "device|primary_ip4", "mapping_type": "device"},
         {"source_field": "ipv4", "target_field": "device|primary_ip4", "mapping_type": "device"},
         {"source_field": "device_os", "target_field": "device|platform", "mapping_type": "device"},
         {"source_field": "device_type", "target_field": "device|device_type", "mapping_type": "device"},
     ]
     for mapping in mappings:
         SlurpitMapping.objects.get_or_create(**mapping)
 
 
+def add_default_mandatory_objects(tags):
+    manu, _ = Manufacturer.objects.get_or_create(**get_config('Manufacturer'))
+    dtype, _ = DeviceType.objects.get_or_create(manufacturer=manu, **get_config('DeviceType'))
+    tenant, _ = Tenant.objects.get_or_create(**get_config('Tenant'))
+    location_type, _ = LocationType.objects.get_or_create(**get_config('LocationType'))
+    location_active_status = Status.objects.get_for_model(Location).all()[0]
+    location, _ = Location.objects.get_or_create(location_type=location_type, status=location_active_status, **get_config('Location'))
+    role, _ = Role.objects.get_or_create(**get_config('Role'))
+
+    create_default_data_mapping()
+
+
+
 def post_migration(sender, **kwargs):
     create_custom_fields()
     tags = ensure_slurpit_tags()
     add_default_mandatory_objects(tags)
     pass
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/models/device.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/models/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,25 @@
     brand = models.CharField(max_length=255)
     createddate = models.DateTimeField()
     changeddate = models.DateTimeField()
 
     def __str__(self):
         return f"{self.hostname}"
     
+    def get_absolute_url(self):
+        return '/'
+    
+    class Meta:
+        ordering = ("hostname",)  # Name may be null
+        unique_together = (
+            ("hostname"),
+        )
+        verbose_name = "device"
+        verbose_name_plural = "device"
+    
     
 class SlurpitImportedDevice(PrimaryModel):
     slurpit_id = models.BigIntegerField(unique=True)
     disabled = models.BooleanField(default=False)
     hostname = models.CharField(max_length=255, unique=True)
     fqdn = models.CharField(max_length=128)
     ipv4 = models.CharField(max_length=23, null=True)
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/models/logs.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/models/logs.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/models/planning.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/models/planning.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,10 +14,11 @@
     def get_absolute_url(self):
         return reverse("plugins:slurpit_nautobot:slurpitplanning", args=[self.pk])
 
 class SlurpitSnapshot(PrimaryModel):
     hostname = models.CharField(max_length=255)
     planning_id = models.BigIntegerField()
     content = models.JSONField()
-
+    result_type = models.CharField(max_length=255, default="template_result")
+    
     def __str__(self):
         return f"{self.hostname}#{self.planning_id}"
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/models/setting.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/models/setting.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/navigation.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/navigation.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/references/generic.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/references/generic.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/references/imports.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/references/imports.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/slurpitch.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/slurpitch.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/tables.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/tables.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/template_content.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/template_content.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         <div class="card">
           <div class="card-body htmx-container table-responsive" id="object_list">
             <div class="col-md-12">
               <div class="pull-left noprint">
                 <div class="dropdown mb-3">
                   <button type="button" class="btn btn-success dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
-                    <i class="mdi mdi-check"></i>&nbsp;{% trans "Solve" %}
+                    <i class="mdi mdi-check"></i>&nbsp;{% trans "Solve" %} <span class="caret"></span>
                   </button>
                   {% block bulk_buttons %}
                   <ul class="dropdown-menu dropdown-menu-end">
                     <li>
                         <button type="submit" name="_rename" formaction="{% url 'plugins:slurpit_nautobot:onboard' %}?conflicted=create&return_url={% url 'plugins:slurpit_nautobot:importeddevice_list' %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn">
                           <i class="mdi mdi-plus" aria-hidden="true"></i> {% trans "Re-Create device" %}
                         </button>
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         <div class="card">
           <div class="card-body htmx-container table-responsive" id="object_list">
             <div class="col-md-12">
               <div class="pull-left noprint">
                 <div class="dropdown mb-3">
                   <button type="button" class="btn  btn-warning dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
-                    <i class="mdi mdi-refresh"></i>&nbsp;{% trans "Migrate" %}
+                    <i class="mdi mdi-refresh"></i>&nbsp;{% trans "Migrate" %} <span class="caret"></span>
                   </button>
                   {% block bulk_buttons %}
                   <ul class="dropdown-menu dropdown-menu-end">
                     <li>
                         <button type="submit" name="_rename" formaction="{% url 'plugins:slurpit_nautobot:onboard' %}?migrate=create&return_url={% url 'plugins:slurpit_nautobot:importeddevice_list' %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn">
                           <i class="mdi mdi-plus" aria-hidden="true"></i> {% trans "Re-Create device" %}
                         </button>
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html`

 * *Files 11% similar despite different names*

```diff
@@ -73,24 +73,15 @@
   <style>
     .footer {
       border-top-left-radius: 0px !important;
       border-top-right-radius: 0px !important;
       margin-left: 0px !important;
       margin-right: 0px !important;
     }
-    .dropdown-toggle:after { 
-      display: inline-block;
-      margin-left: 0.255em;
-      vertical-align: 0.255em;
-      content: "";
-      border-top: 0.3em solid;
-      border-right: 0.3em solid transparent;
-      border-bottom: 0;
-      border-left: 0.3em solid transparent;
-    }
+   
     .dropdown-menu .btn {
       background-color: transparent;
     }
 
   </style>
 {% endblock content %}
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html`

 * *Files 11% similar despite different names*

```diff
@@ -10,29 +10,29 @@
       <form action="" method="get" id="plan-form" class="form form-horizontal">
         <div>
           <div class="col-md-6 d-flex gap-2">
             <div class="w-50">
               {% render_form form %}
             </div>
             <div class="">
-              <button type="submit" class="btn btn-primary btn-sm">
+              <button type="submit" class="btn btn-primary planning-open">
                 Open
               </button>
             </div>
           </div>
           <input type="hidden" value="none" name="refresh" id="refreshInput"/>
           <input type="hidden" value="none" name="sync" id="syncInput"/>
           <div class="col-md-6 text-end" style="text-align: right;">
             <div class="btn-group btn-group-sm" role="group">
               <!-- {% if appliance_type == 'both' or appliance_type == 'pull'  %}
                 {% if connection_status == 'connected' %}
                   <a name="sync"  class="btn btn-orange btn-sm mx-2" id="sync">{% trans "Sync" %}</a>
                 {% endif %}
               {% endif %} -->
-              <select class="btn btn-sm btn-secondary result-type" id="result-type" name="result_type">
+              <select class="btn btn-secondary result-type" id="result-type" name="result_type">
                 <option value="planning" {% if "result_type" not in request.GET or request.GET.result_type == 'planning' %}selected="selected"{% else %} {% endif %}>{% trans "Planning Result" %}</option>
                 <option value="template" {% if request.GET.result_type == 'template' %}selected="selected"{% else %} {% endif %}>{% trans "Template Result" %}</option>
               </select>
             </div>
           </div>
          
         </div>
@@ -94,14 +94,23 @@
   }
   .d-flex {
     display: flex;
   }
   .col-md-9 {
     width: 95%;
   }
+  .planning-open {
+    line-height: 14px !important;
+  }
+
+  .btn-secondary {
+    background-color: #adb5bd;
+    color: #000 !important;
+  }
+
 </style>
 
 <script>
   var selectElement = document.getElementById('result-type');
   var form = document.getElementById('plan-form');
   // Add an event listener for the 'change' event
   selectElement.addEventListener('change', function(event) {
@@ -129,7 +138,18 @@
   });
 
  
 </script>
 
 {% endblock %}
 
+{% block javascript %}
+<script>
+  var form = document.getElementById('plan-form');
+  var refreshInput = document.getElementById('refreshInput');
+
+  $("#id_planning_id").on('select2:select', function(e){
+    form.submit();
+  });
+</script>
+{% endblock %}
+
```

#### html2text {}

```diff
@@ -5,8 +5,9 @@
 % if "result_type" not in request.GET or request.GET.result_type == 'planning'
 %}selected="selected"{% else %} {% endif %}>{% trans "Planning Result" %}
 % if request.GET.result_type == 'template' %}selected="selected"{% else %} {%
 endif %}>{% trans "Template Result" %}
 {{{{rreessuulltt__ssttaattuuss}}}} rreessuullttss {{%% iiff rreessuulltt__ssttaattuuss ==== ''CCaacchheedd'' %%}} -- RReeffrreesshh ddaattaa {{%%
 eennddiiff %%}} {{%% iiff rreessuulltt__ssttaattuuss ==== ''CCaacchheedd'' %%}} {{{{ ccaacchheedd__ttiimmee}}}} {{%% eennddiiff %%}}
 {% block table %} {% include "slurpit_nautobot/table1.html" %} {% endblock %}
+{% endblock %} {% block javascript %}
 {% endblock %}
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
               background-color: #007dff;
             }
           </style>
           {% if debug == True %}
           <div class="panel panel-default" style="margin-top: 10px;">
             <div class="panel-heading" style="display: flex; justify-content: space-between; align-items: center;">
                 <strong>Reset Plugin</strong>
-                <a class="btn btn-danger mx-3 px-3" data-bs-toggle="modal" data-bs-target="#resetModal">
+                <a class="btn btn-danger mx-3 px-3" data-toggle="modal" data-target="#resetModal">
                   {% trans "Reset" %}
                 </a>
             </div>
             <div class="panel-body">
               Remove all plugin data from the Slurp'it tables.
             </div>
           </div>
@@ -116,15 +116,15 @@
         <div class="col col-md-6">
           {% if appliance_type == 'both' or appliance_type == 'pull'  %}
             <div class="panel panel-default">
 
                 <div class="panel-heading" style="display: flex; justify-content: space-between; align-items: center;">
                     <strong>Slurp'it Server</strong>
                     <div>
-                        <button class="btn btn-primary mx-3" data-toggle="modal" data-target="#settingsEditModal">
+                        <button class="btn btn-warning mx-3" data-toggle="modal" data-target="#settingsEditModal">
                             {% trans "Edit" %}
                         </button>
                         <a name="Edit" class="btn btn-primary mx-3 px-3" href="{% url 'plugins:slurpit_nautobot:settings' %}?test=test"> {% trans "Test" %}</a>
                     </div>
                     
                 </div>
                 
@@ -204,21 +204,21 @@
 
 <div class="modal fade" tabindex="-1" id="resetModal">
   <div class="modal-dialog modal-lg">
     <div class="modal-content">
 
       <!-- Modal Header -->
       <div class="modal-header">
-        <h6 class="modal-title">Are you sure to reset the Slurp'it plugin?</h6>
-        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
+        <h3 class="modal-title">Are you sure to reset the Slurp'it plugin?</h3>
+        <!-- <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button> -->
       </div>
 
       <!-- Modal Footer -->
       <div class="modal-footer">
           <a class="btn btn-danger" id="" href="?reset=true" >{% trans "Reset" %}</a>
-          <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
+          <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
       </div>
 
       
     </div>
   </div>
 </div>
```

#### html2text {}

```diff
@@ -28,9 +28,9 @@
 Last Synced {{setting.last_synced}}
 {% endif %}
 ****** SSeettttiinnggss ******
 {% csrf_token %}
 Server URL[{{setting.server_url}}]
 API Key[{{setting.api_key}} ]
 {% trans "Save" %} Close
-** AArree yyoouu ssuurree ttoo rreesseett tthhee SSlluurrpp''iitt pplluuggiinn?? **
+******** AArree yyoouu ssuurree ttoo rreesseett tthhee SSlluurrpp''iitt pplluuggiinn?? ********
 _{_%_ _t_r_a_n_s_ _"_R_e_s_e_t_"_ _%_} Close
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/templates/slurpit_nautobot/table.html` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/templates/slurpit_nautobot/table.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/urls.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/urls.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/validator.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/validator.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/views/datamapping.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/views/datamapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                         'accept': 'application/json',
                         'Content-Type': 'application/json',
                     }
 
         uri_devices = f"{uri_base}/api/devices/sync"
         
         try:
-            row["ignore_plugin"] = str(1)
+            # row["ignore_plugin"] = str(1)
             r = requests.post(uri_devices, headers=headers, json=row, timeout=15, verify=False)
             r = r.json()
             r["item_name"] = item_name
             return r
         except Exception as e:
             return {"error": str(e), "device_name": item_name}
```

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/views/logging.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/views/logging.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/views/onboarding.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/views/onboarding.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/views/reconcile.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/views/reconcile.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.64/src/slurpit_nautobot/views/setting.py` & `slurpit_nautobot-0.8.65/src/slurpit_nautobot/views/setting.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from nautobot.core.views import generic
 from nautobot.users.models import Token
 from nautobot.dcim.models import Device
 from nautobot.core.views.paginator import get_paginate_count, EnhancedPaginator
 
 from ..forms import SlurpitPlanningTableForm, SlurpitApplianceTypeForm
-from ..models import SlurpitSetting, SlurpitLog, SlurpitPlanning, SlurpitSnapshot, SlurpitImportedDevice, SlurpitStagedDevice
+from ..models import create_default_data_mapping, SlurpitSetting, SlurpitLog, SlurpitPlanning, SlurpitSnapshot, SlurpitImportedDevice, SlurpitStagedDevice
 from ..tables import SlurpitPlanningTable
 from ..management.choices import *
 from ..decorators import slurpit_plugin_registered
 from ..importer import get_latest_data_on_planning, import_plannings
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 from ..filtersets import SlurpitPlanningFilterSet
 
@@ -37,19 +37,21 @@
     app_label = "dcim"
     model_name = "device"
     
     def get(self, request):
         reset_param = request.GET.get('reset', None)
         if reset_param:
             SlurpitImportedDevice.objects.all().delete()
-            SlurpitStagedDevice.objects.all().delete()
             SlurpitSnapshot.objects.all().delete()
             SlurpitLog.objects.all().delete()
             SlurpitSetting.objects.all().delete()
             SlurpitPlanning.objects.all().delete()
+            SlurpitStagedDevice.objects.all().delete()
+            
+            create_default_data_mapping()
 
             return HttpResponseRedirect(reverse("plugins:slurpit_nautobot:settings"))
         
         appliance_type = ''
         try:
             setting = SlurpitSetting.objects.get()
             server_url = setting.server_url
@@ -298,15 +300,15 @@
         return None
 
 def get_refresh_url(request, pk):
     get_params = request.GET.copy()
     get_params['refresh'] = 'none'
     get_params['sync'] = 'none'
 
-    path = f"/dcim/devices/{pk}/Slurpit/"
+    path = f"/plugins/slurpit/devices/{pk}/slurpit_planning/"
     query_string = get_params.urlencode()
     url_no_refresh = f"{path}?{query_string}" if query_string else path
 
     return url_no_refresh
 
 
 class SlurpitPlanningning(ObjectView):
@@ -361,27 +363,28 @@
             cached_time, data = cache.get(cache_key, (None, None))
             if cached_time:
                 result_status = "Cached"
                 
             if not data:
                 data = []
                 try: 
-                    temp = SlurpitSnapshot.objects.filter(hostname=device.name, planning_id=planning.planning_id)
                     result_key = f"{result_type}_result"
+                    temp = SlurpitSnapshot.objects.filter(hostname=device.name, planning_id=planning.planning_id, result_type=result_key)
+                    
                     
                     # Empty case
                     if temp.count() == 0:
                         if appliance_type != "cloud":
                             sync_snapshot(cache_key, device.name, planning)
-                        temp = SlurpitSnapshot.objects.filter(hostname=device.name, planning_id=planning.planning_id)
+                        temp = SlurpitSnapshot.objects.filter(hostname=device.name, planning_id=planning.planning_id, result_type=result_key)
 
                     for r in temp:
                         r = r.content
-                        raw = r[result_key]
-                        data.append({**raw})
+                        # raw = r[result_key]
+                        data.append({**r})
                     result_status = "Live"
                     cache.set(cache_key, (datetime.now(), data), 60 * 60 * 8)
                     
                 except Exception as e:
                     messages.error(request, e)
 
         if refresh == "refresh":
@@ -421,23 +424,28 @@
                 "connection_status": connection_status,
                 "verbose_name": "Device"
             },
         )
 
 def sync_snapshot(cache_key, device_name, plan):
     cache.delete(cache_key)
-    temp = get_latest_data_on_planning(device_name, plan.planning_id)
-    temp = temp[plan.name]["data"]
 
     count = SlurpitSnapshot.objects.filter(hostname=device_name, planning_id=plan.planning_id).delete()[0]
     SlurpitLog.info(category=LogCategoryChoices.PLANNING, message=f"Sync deleted {count} snapshots for planning {plan.name}")
 
+    data = get_latest_data_on_planning(device_name, plan.planning_id)
     new_items = []
+
+    temp = data[plan.name]["planning_results"]
+    for item in temp:
+        new_items.append(SlurpitSnapshot(hostname=device_name, planning_id=plan.planning_id, content=item, result_type="planning_result"))
+    
+    temp = data[plan.name]["template_results"]
     for item in temp:
-        new_items.append(SlurpitSnapshot(hostname=device_name, planning_id=plan.planning_id, content=item))
+        new_items.append(SlurpitSnapshot(hostname=device_name, planning_id=plan.planning_id, content=item, result_type="template_result"))
     
     SlurpitSnapshot.objects.bulk_create(new_items, batch_size=BATCH_SIZE, ignore_conflicts=True)
     SlurpitLog.info(category=LogCategoryChoices.PLANNING, message=f"Sync imported {len(new_items)} snapshots for planning {plan.name}")
 
 class SlurpitPlanningListView(generic.ObjectListView):
     queryset = SlurpitPlanning.objects.all()
     filterset = SlurpitPlanningFilterSet
```

