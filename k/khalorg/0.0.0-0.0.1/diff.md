# Comparing `tmp/khalorg-0.0.0.tar.gz` & `tmp/khalorg-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khalorg-0.0.0.tar", last modified: Tue Jun 13 20:44:01 2023, max compression
+gzip compressed data, was "khalorg-0.0.1.tar", last modified: Mon Apr  8 19:33:19 2024, max compression
```

## Comparing `khalorg-0.0.0.tar` & `khalorg-0.0.1.tar`

### file list

```diff
@@ -1,112 +1,117 @@
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.429908 khalorg-0.0.0/
--rw-r--r--   0 barts     (1000) barts     (1000)       88 2023-06-10 08:37:21.000000 khalorg-0.0.0/.gitignore
--rw-r--r--   0 barts     (1000) barts     (1000)     1558 2023-06-09 18:01:22.000000 khalorg-0.0.0/CHANGELOG.md
--rw-r--r--   0 barts     (1000) barts     (1000)      983 2023-06-13 19:32:25.000000 khalorg-0.0.0/CONTRIBUTING.md
--rw-r--r--   0 barts     (1000) barts     (1000)     1064 2023-04-18 19:53:17.000000 khalorg-0.0.0/LICENCE
--rw-r--r--   0 barts     (1000) barts     (1000)    14461 2023-06-13 20:44:01.426574 khalorg-0.0.0/PKG-INFO
--rw-r--r--   0 barts     (1000) barts     (1000)    14036 2023-06-13 20:40:26.000000 khalorg-0.0.0/README.md
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.323242 khalorg-0.0.0/demo/
--rw-r--r--   0 barts     (1000) barts     (1000)   474334 2023-06-10 08:35:14.000000 khalorg-0.0.0/demo/delete.gif
--rw-r--r--   0 barts     (1000) barts     (1000)   814156 2023-06-10 08:31:21.000000 khalorg-0.0.0/demo/edit.gif
--rw-r--r--   0 barts     (1000) barts     (1000)   805028 2023-06-10 08:28:19.000000 khalorg-0.0.0/demo/list.gif
--rw-r--r--   0 barts     (1000) barts     (1000)      358 2023-06-10 07:57:04.000000 khalorg-0.0.0/demo/meeting.org
--rw-r--r--   0 barts     (1000) barts     (1000)   330668 2023-06-10 08:21:55.000000 khalorg-0.0.0/demo/new.gif
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.326575 khalorg-0.0.0/extras/
--rwxr-xr-x   0 barts     (1000) barts     (1000)     1900 2023-06-07 19:23:32.000000 khalorg-0.0.0/extras/calsync
--rwxr-xr-x   0 barts     (1000) barts     (1000)      285 2023-06-13 20:42:10.000000 khalorg-0.0.0/publish
--rw-r--r--   0 barts     (1000) barts     (1000)     1702 2023-06-13 20:40:44.000000 khalorg-0.0.0/pyproject.toml
--rw-r--r--   0 barts     (1000) barts     (1000)       38 2023-06-13 20:44:01.429908 khalorg-0.0.0/setup.cfg
--rw-r--r--   0 barts     (1000) barts     (1000)      141 2023-06-07 19:23:32.000000 khalorg-0.0.0/setup.py
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.303242 khalorg-0.0.0/src/
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.336575 khalorg-0.0.0/src/khalorg/
--rw-r--r--   0 barts     (1000) barts     (1000)      260 2023-06-13 20:15:09.000000 khalorg-0.0.0/src/khalorg/__init__.py
--rw-r--r--   0 barts     (1000) barts     (1000)       64 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/__main__.py
--rw-r--r--   0 barts     (1000) barts     (1000)     3476 2023-06-13 20:16:43.000000 khalorg-0.0.0/src/khalorg/cli.py
--rw-r--r--   0 barts     (1000) barts     (1000)     6303 2023-06-13 20:10:02.000000 khalorg-0.0.0/src/khalorg/commands.py
--rw-r--r--   0 barts     (1000) barts     (1000)      774 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/helpers.py
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.346575 khalorg-0.0.0/src/khalorg/khal/
--rw-r--r--   0 barts     (1000) barts     (1000)     7701 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/khal/args.py
--rw-r--r--   0 barts     (1000) barts     (1000)     9997 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/khal/calendar.py
--rw-r--r--   0 barts     (1000) barts     (1000)     4823 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/khal/checker.py
--rw-r--r--   0 barts     (1000) barts     (1000)     2418 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/khal/helpers.py
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.349908 khalorg-0.0.0/src/khalorg/org/
--rw-r--r--   0 barts     (1000) barts     (1000)    19368 2023-06-13 19:36:17.000000 khalorg-0.0.0/src/khalorg/org/agenda_items.py
--rw-r--r--   0 barts     (1000) barts     (1000)     2461 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/org/helpers.py
--rw-r--r--   0 barts     (1000) barts     (1000)      396 2023-06-09 17:59:06.000000 khalorg-0.0.0/src/khalorg/paths.py
--rw-r--r--   0 barts     (1000) barts     (1000)     8429 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/rrule.py
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.359908 khalorg-0.0.0/src/khalorg/static/
--rw-r--r--   0 barts     (1000) barts     (1000)        0 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/static/__init__.py
--rw-r--r--   0 barts     (1000) barts     (1000)      288 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/static/description_delete_command.txt
--rw-r--r--   0 barts     (1000) barts     (1000)       30 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/static/description_edit_command.txt
--rw-r--r--   0 barts     (1000) barts     (1000)      967 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/static/description_list_command.txt
--rw-r--r--   0 barts     (1000) barts     (1000)      381 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/static/description_new_command.txt
--rw-r--r--   0 barts     (1000) barts     (1000)      283 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/static/khal_format.txt
--rw-r--r--   0 barts     (1000) barts     (1000)      264 2023-06-07 19:23:32.000000 khalorg-0.0.0/src/khalorg/static/khalorg_format.txt
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.343242 khalorg-0.0.0/src/khalorg.egg-info/
--rw-r--r--   0 barts     (1000) barts     (1000)    14461 2023-06-13 20:44:01.000000 khalorg-0.0.0/src/khalorg.egg-info/PKG-INFO
--rw-r--r--   0 barts     (1000) barts     (1000)     3288 2023-06-13 20:44:01.000000 khalorg-0.0.0/src/khalorg.egg-info/SOURCES.txt
--rw-r--r--   0 barts     (1000) barts     (1000)        1 2023-06-13 20:44:01.000000 khalorg-0.0.0/src/khalorg.egg-info/dependency_links.txt
--rw-r--r--   0 barts     (1000) barts     (1000)       41 2023-06-13 20:44:01.000000 khalorg-0.0.0/src/khalorg.egg-info/entry_points.txt
--rw-r--r--   0 barts     (1000) barts     (1000)       89 2023-06-13 20:44:01.000000 khalorg-0.0.0/src/khalorg.egg-info/requires.txt
--rw-r--r--   0 barts     (1000) barts     (1000)        8 2023-06-13 20:44:01.000000 khalorg-0.0.0/src/khalorg.egg-info/top_level.txt
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.369908 khalorg-0.0.0/tests/
--rw-r--r--   0 barts     (1000) barts     (1000)        0 2023-06-07 19:38:51.000000 khalorg-0.0.0/tests/__init__.py
--rw-r--r--   0 barts     (1000) barts     (1000)     5000 2023-06-13 19:41:12.000000 khalorg-0.0.0/tests/agenda_items.py
--rw-r--r--   0 barts     (1000) barts     (1000)    12803 2023-06-09 17:59:06.000000 khalorg-0.0.0/tests/helpers.py
--rw-r--r--   0 barts     (1000) barts     (1000)      696 2023-06-13 20:15:18.000000 khalorg-0.0.0/tests/khalorg_tester
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.376575 khalorg-0.0.0/tests/static/
--rw-r--r--   0 barts     (1000) barts     (1000)        0 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/__init__.py
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.416575 khalorg-0.0.0/tests/static/agenda_items/
--rw-r--r--   0 barts     (1000) barts     (1000)      424 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/all_day.org
--rw-r--r--   0 barts     (1000) barts     (1000)      424 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/all_day_until_with_time.org
--rw-r--r--   0 barts     (1000) barts     (1000)      454 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/body_first.org
--rw-r--r--   0 barts     (1000) barts     (1000)      340 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/demo.org
--rw-r--r--   0 barts     (1000) barts     (1000)      838 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/duplicate.org
--rw-r--r--   0 barts     (1000) barts     (1000)      131 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/minimal.org
--rw-r--r--   0 barts     (1000) barts     (1000)      516 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/multiple_timestamps.org
--rw-r--r--   0 barts     (1000) barts     (1000)      516 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/multiple_timestamps_unsorted.org
--rw-r--r--   0 barts     (1000) barts     (1000)      330 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/no_heading.org
--rw-r--r--   0 barts     (1000) barts     (1000)      405 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/no_time_stamp.org
--rw-r--r--   0 barts     (1000) barts     (1000)      420 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/not_first_child.org
--rw-r--r--   0 barts     (1000) barts     (1000)      407 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/not_first_heading.org
--rw-r--r--   0 barts     (1000) barts     (1000)      454 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/not_first_level.org
--rw-r--r--   0 barts     (1000) barts     (1000)       60 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/past.org
--rw-r--r--   0 barts     (1000) barts     (1000)      387 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/recurring.org
--rw-r--r--   0 barts     (1000) barts     (1000)      375 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/recurring_allday.org
--rw-r--r--   0 barts     (1000) barts     (1000)      436 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/recurring_and_non_recurring.org
--rw-r--r--   0 barts     (1000) barts     (1000)     1237 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/recurring_first_item_moved.org
--rw-r--r--   0 barts     (1000) barts     (1000)      822 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/recurring_first_item_moved_expected.org
--rw-r--r--   0 barts     (1000) barts     (1000)      387 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/recurring_monthly.org
--rw-r--r--   0 barts     (1000) barts     (1000)      395 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/recurring_not_supported.org
--rw-r--r--   0 barts     (1000) barts     (1000)      527 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/rrule_recurring.org
--rw-r--r--   0 barts     (1000) barts     (1000)      498 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/rrule_recurring_1th.org
--rw-r--r--   0 barts     (1000) barts     (1000)      446 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/rrule_recurring_allday.org
--rw-r--r--   0 barts     (1000) barts     (1000)     1525 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/rrule_recurring_and_non_recurring.org
--rw-r--r--   0 barts     (1000) barts     (1000)     1587 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/rrule_recurring_duplicates.org
--rw-r--r--   0 barts     (1000) barts     (1000)      463 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/rrule_recurring_monthly.org
--rw-r--r--   0 barts     (1000) barts     (1000)      476 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/rrule_recurring_not_supported.org
--rw-r--r--   0 barts     (1000) barts     (1000)      480 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/scheduled_and_deadline.org
--rw-r--r--   0 barts     (1000) barts     (1000)      437 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/short_timestamp.org
--rw-r--r--   0 barts     (1000) barts     (1000)        0 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/timestamp_scheduled_deadline.org
--rw-r--r--   0 barts     (1000) barts     (1000)      837 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/two_items.org
--rw-r--r--   0 barts     (1000) barts     (1000)      467 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/two_timestamps.org
--rw-r--r--   0 barts     (1000) barts     (1000)      383 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/valid.org
--rw-r--r--   0 barts     (1000) barts     (1000)      361 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/agenda_items/valid_no_until.org
--rw-r--r--   0 barts     (1000) barts     (1000)      489 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/config_template.txt
--rw-r--r--   0 barts     (1000) barts     (1000)      282 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/khalorg_format_full.txt
--rw-r--r--   0 barts     (1000) barts     (1000)       60 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/test_config_combined.ini
--rw-r--r--   0 barts     (1000) barts     (1000)       41 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/test_config_default.ini
--rw-r--r--   0 barts     (1000) barts     (1000)      760 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/test_config_khal
--rw-r--r--   0 barts     (1000) barts     (1000)       41 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/static/test_config_user.ini
--rw-r--r--   0 barts     (1000) barts     (1000)     4160 2023-06-13 20:15:51.000000 khalorg-0.0.0/tests/test_cli.py
--rw-r--r--   0 barts     (1000) barts     (1000)     7658 2023-06-07 19:26:23.000000 khalorg-0.0.0/tests/test_commands.py
--rw-r--r--   0 barts     (1000) barts     (1000)      835 2023-06-09 17:59:06.000000 khalorg-0.0.0/tests/test_helpers.py
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.423241 khalorg-0.0.0/tests/test_khal/
--rw-r--r--   0 barts     (1000) barts     (1000)      328 2023-06-07 19:26:22.000000 khalorg-0.0.0/tests/test_khal/helpers.py
--rw-r--r--   0 barts     (1000) barts     (1000)     4987 2023-06-07 19:26:22.000000 khalorg-0.0.0/tests/test_khal/test_args.py
--rw-r--r--   0 barts     (1000) barts     (1000)     1433 2023-06-07 19:26:22.000000 khalorg-0.0.0/tests/test_khal/test_calendar.py
--rw-r--r--   0 barts     (1000) barts     (1000)     2123 2023-06-07 19:26:22.000000 khalorg-0.0.0/tests/test_khal/test_checker.py
-drwxr-xr-x   0 barts     (1000) barts     (1000)        0 2023-06-13 20:44:01.426574 khalorg-0.0.0/tests/test_org/
--rw-r--r--   0 barts     (1000) barts     (1000)     9637 2023-06-07 19:26:22.000000 khalorg-0.0.0/tests/test_org/test_agenda_items.py
--rw-r--r--   0 barts     (1000) barts     (1000)      740 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/test_org/test_helpers.py
--rw-r--r--   0 barts     (1000) barts     (1000)     1979 2023-06-07 19:23:32.000000 khalorg-0.0.0/tests/test_rrule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.214148 khalorg-0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.182148 khalorg-0.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.186148 khalorg-0.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-08 19:33:09.000000 khalorg-0.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-08 19:33:09.000000 khalorg-0.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-08 19:33:09.000000 khalorg-0.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-08 19:33:09.000000 khalorg-0.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 19:33:09.000000 khalorg-0.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 19:33:09.000000 khalorg-0.0.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-04-08 19:33:19.214148 khalorg-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-04-08 19:33:09.000000 khalorg-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.198148 khalorg-0.0.1/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)   474334 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/delete.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   814156 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/edit.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   805028 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/list.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40467 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/meeting.org
+-rw-r--r--   0 runner    (1001) docker     (127)  5848880 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/neovim-plugin.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   330668 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/new.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.198148 khalorg-0.0.1/extras/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4045 2024-04-08 19:33:09.000000 khalorg-0.0.1/extras/calsync
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-08 19:33:09.000000 khalorg-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:33:19.214148 khalorg-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 19:33:09.000000 khalorg-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.186148 khalorg-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.198148 khalorg-0.0.1/src/khalorg/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.202148 khalorg-0.0.1/src/khalorg/khal/
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/khal/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/khal/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/khal/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/khal/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.202148 khalorg-0.0.1/src/khalorg/org/
+-rw-r--r--   0 runner    (1001) docker     (127)    19368 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/org/agenda_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/org/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/rrule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.202148 khalorg-0.0.1/src/khalorg/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/description_delete_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/description_edit_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/description_list_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/description_new_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/khal_format.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/khalorg_format.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.214148 khalorg-0.0.1/src/khalorg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.202148 khalorg-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/agenda_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/khalorg_tester
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.206148 khalorg-0.0.1/tests/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.210148 khalorg-0.0.1/tests/static/agenda_items/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/all_day.org
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/all_day_until_with_time.org
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/body_first.org
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/demo.org
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/duplicate.org
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/minimal.org
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/multiple_timestamps.org
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/multiple_timestamps_unsorted.org
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/no_heading.org
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/no_time_stamp.org
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/not_first_child.org
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/not_first_heading.org
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/not_first_level.org
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/past.org
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_allday.org
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_and_non_recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_first_item_moved.org
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_first_item_moved_expected.org
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_monthly.org
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_not_supported.org
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_1th.org
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_allday.org
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_and_non_recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_duplicates.org
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_monthly.org
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_not_supported.org
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/scheduled_and_deadline.org
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/short_timestamp.org
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/timestamp_scheduled_deadline.org
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/two_items.org
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/two_timestamps.org
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/valid.org
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/valid_no_until.org
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/config_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/khalorg_format_full.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/test_config_combined.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/test_config_default.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/test_config_khal
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/test_config_user.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.210148 khalorg-0.0.1/tests/test_khal/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_khal/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_khal/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_khal/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_khal/test_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.214148 khalorg-0.0.1/tests/test_org/
+-rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_org/test_agenda_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_org/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_rrule.py
```

### Comparing `khalorg-0.0.0/CHANGELOG.md` & `khalorg-0.0.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/CONTRIBUTING.md` & `khalorg-0.0.1/CONTRIBUTING.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Contributing to khalorg
 
 Thank you for considering contributing to the `khalorg` project! We welcome contributions from everyone.
 
 ## Getting Started
 
 1. Fork the repository on GitHub.
-2. Clone your forked repository (`git clone https://github.com/your_username/khalorg.git`).
+2. Clone your forked repository (`git clone https://github.com/BartSte/khalorg.git`).
 3. Create a new branch (`git checkout -b my_branch_name`).
 4. Make your changes.
 5. Commit your changes (`git commit -am "Add some feature"`).
 6. Push your changes to your forked repository (`git push origin my_branch_name`).
 7. Create a pull request on GitHub.
 
 ## Code of Conduct
 
 Please note that this project is released with a Contributor Code of Conduct. By participating in this project you agree to abide by its terms.
 
 ## Reporting Bugs
 
 If you encounter any bugs or issues, please report them on the issue tracker at:
 
-[Issues](https://github.com/username/khalorg/issues)
+[Issues](https://github.com/BartSte/khalorg/issues)
 
 ## License
 
 By contributing to this project, you agree that your contributions will be licensed under the MIT License.
```

### Comparing `khalorg-0.0.0/LICENCE` & `khalorg-0.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/PKG-INFO` & `khalorg-0.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,90 +1,117 @@
-Metadata-Version: 2.1
-Name: khalorg
-Version: 0.0.0
-Summary: An interface between Org mode and Khal cli calendar.
-Author: BartSte
-License: MIT License
-Keywords: khal,org mode,vdirsyncer,CalDav,agenda,emacs,neovim,orgmode-nvim
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: debug
-Provides-Extra: test
-Provides-Extra: build
-License-File: LICENCE
+# Khalorg
 
-[Click here for the GitHub page.](https://github.com/BartSte/khalorg) 
+[Click here for the GitHub page.](https://github.com/BartSte/khalorg)
 
-# Contents
+<img src="./demo/logo.jpg" width=50%>
+
+## Demo
+
+The demo below demonstrates the following features using the neovim plugin
+called [nvim-khalorg](https://github.com/BartSte/nvim-khalorg):
+
+- `khalorg new`: convert an org agenda item into a `khal` agenda item.
+- `khalorg list`: convert a `khal` agenda item into an org agenda item.
+- `khalorg edit`: edit an existing `khal` agenda item with org mode.
+- `khalorg delete`: delete an existing `khal` item.
+
+![neovim-plugin](https://github.com/BartSte/khalorg/blob/main/demo/neovim-plugin.gif?raw=true)
+
+## Contents
+
+<!--toc:start-->
+
+- [Demo](#demo)
+- [Contents](#contents)
 - [Introduction](#introduction)
+  - [Definitions](#definitions)
+  - [Motivation](#motivation)
+  - [Features](#features)
 - [Installation](#installation)
+  - [PyPi](#pypi)
+  - [From source](#from-source)
+  - [For development](#for-development)
 - [Usage](#usage)
+  - [List: from khal to org](#list-from-khal-to-org)
+    - [–format](#format)
+    - [Recurring items](#recurring-items)
+  - [New: from org to khal](#new-from-org-to-khal)
+    - [Recurring items](#recurring-items)
+    - [Attendees](#attendees)
+  - [Edit: from org to khal](#edit-from-org-to-khal)
+  - [Delete: from org to khal](#delete-from-org-to-khal)
+    - [Recurring items](#recurring-items)
 - [Neovim plugin](#neovim-plugin)
 - [Workflow for Office 365](#workflow-for-office-365)
 - [Troubleshooting](#troubleshooting)
 - [Contributing](#contributing)
 - [License](#license)
-- [Improvements](#improvements)
+- [Improvements:](#improvements)
+
+<!--toc:end-->
+
+## Introduction
 
-# Introduction
 `khalorg` is an interface between Org mode and Khal cli calendar.
 
-## Definitions
-- [CalDav](<https://en.wikipedia.org/wiki/CalDAV>): internet standard for client access to calendars
-- [Davmail](<https://davmail.sourceforge.net/e>): CalDav exchange gateway
-- [khal](<https://github.com/pimutils/khal>): command line calendar app 
-- [khalel](<https://gitlab.com/hperrey/khalel>): interface between emacs and khal
-- [nvim-orgmode](<https://github.com/nvim-orgmode/orgmode>): org mode for neovim
-- [org](<https://orgmode.org>): plain text system for keeping notes, agendas and more
-- [vdirsyncer](<https://github.com/pimutils/vdirsyncer>): synchronizes calendars and addressbooks between servers and the local file system
+### Definitions
+
+- [CalDav](https://en.wikipedia.org/wiki/CalDAV): internet standard for client access to calendars
+- [Davmail](https://davmail.sourceforge.net/e): CalDav exchange gateway
+- [khal](https://github.com/pimutils/khal): command line calendar app
+- [khalel](https://gitlab.com/hperrey/khalel): interface between emacs and khal
+- [nvim-orgmode](https://github.com/nvim-orgmode/orgmode): org mode for neovim
+- [org](https://orgmode.org): plain text system for keeping notes, agendas and more
+- [vdirsyncer](https://github.com/pimutils/vdirsyncer): synchronizes calendars and addressbooks between servers and the local file system
+
+### Motivation
 
-## Motivation
 I use org mode to manage my agenda and my notes. However, in a professional
 setting, you are often required to use proprietary software for your agenda,
 like Office 365. Luckily, programs exist that can synchronize agendas from
 different sources, by implementing the CalDav standard. Personally, I like to
 use `vdirsyncer` with `khal` to synchronize my agendas. To bridge the gap
 between `khal` and `org mode`, only 1 program exists called: `khalel`. However,
 this program is designed for `emacs`. Since there are also org mode users
 outside of `emacs` (e.g. `neovim`), `khalorg` aims to be a general interface
 between `vdirsyncer`/`khal` and `org mode`.
 
 Based on the above, the following workflow is desired:
 
-``` example
-┌──────┐     
-│CalDav│     
-└┬─────┘     
-┌▽─────────┐  
-│vdirsyncer│  
-└┬─────────┘  
-┌▽───┐        
-│khal│        
-└┬───┘        
+```example
+┌──────┐
+│CalDav│
+└┬─────┘
+┌▽─────────┐
+│vdirsyncer│
+└┬─────────┘
+┌▽───┐
+│khal│
+└┬───┘
 ┌▽───────┐
 │khalorg │
 └┬───────┘
-┌▽───────┐    
-│org mode│    
-└────────┘    
+┌▽───────┐
+│org mode│
+└────────┘
 ```
 
-## Features
+### Features
+
 - [x] Can be used by org mode for emacs, vim and neovim.
 - [x] Vdirsyncer calendars can be manipulated by using the cli of `khal`
-  as the interface.
+      as the interface.
 - [x] `khalorg new`: convert an org agenda item into a `khal` agenda
-  item.
+      item.
 - [x] `khalorg list`: convert a `khal` agenda item into an org agenda
-  item.
+      item.
 - [x] `khalorg edit`: edit an existing `khal` agenda item with org mode.
 - [x] `khalorg delete`: delete an existing `khal` item.
 - [x] Recurring items are supported by providing an org repeater in the
-  time stamp (e.g., `+1w`). The following is supported:
+      time stamp (e.g., `+1w`). The following is supported:
   - the follow org repeaters: `+{integer}{d,w,m,y}`
   - `khalorg new` and `khalorg edit --edit-dates` support 1 time stamp
     per org agenda item.
   - `khalorg list` concatenates timestamps that cannot be describes by
     an org repeater, resulting in an org agenda item with multiple
     timestamps.
   - Supports an `until` date for recurring items. The until date can be
@@ -92,82 +119,93 @@
 - [x] Has unittests
 - [x] Includes an Office 365 workflow with a bash script
 - [x] Semantic versioning
 - [x] Gifs with demos
 - [x] Neovim plugin
 - [x] Is available on PyPI
 
-# Installation
+## Installation
+
 For safety, always make a back-up of your calendar before installing software
 that is new to you.
 
 Make sure your `khal` date format is compatible with org, otherwise it
 will not work. When running `khal printformats` you should get:
-``` example
+
+```example
 longdatetimeformat: 2013-12-21 Sat 21:45
 datetimeformat: 2013-12-21 Sat 21:45
 longdateformat: 2013-12-21 Sat
 dateformat: 2013-12-21 Sat
 timeformat: 21:45
 ```
+
 If not, check the documentation of `khal` on how to change this.
 
-## PyPi
+### PyPi
+
 Install by running the following command:
-``` bash
+
+```bash
 pip install khalorg
 ```
 
-## From source
+### From source
+
 Set your current working directory to the root directory, i.e, the
 directory containing the `pyproject.toml` file. Next, run:
 
-``` bash
+```bash
 pip install .
 ```
+
 After this, the executable `khalorg` will be available.
 
-## For development
+### For development
+
 If you want to develop the code, debug it, and test it, run:
-``` bash
+
+```bash
 pip install -e '.[test,debug]'
 ```
 
-# Usage
+## Usage
+
 Use `khalorg --help` to get information about the cli of `khalorg`. The
 following section discuss the `khalorg` commands that are available.
 
-## List: from khal to org
+### List: from khal to org
 
 ![khalorg list demo](https://github.com/BartSte/khalorg/blob/main/demo/list.gif?raw=true)
 
 Agenda items from `khal` can be converted to org items using the
 `khalorg list` command. For examples:
 
-``` bash
-khalorg list my_calendar today 90d > my_calendar.org 
+```bash
+khalorg list my_calendar today 90d > my_calendar.org
 ```
 
 Here, the `khal` agenda items of the calendar `my_calendar` are
 converted to org format and written to a file called `my_calendar.org`.
 The range is specified from `today` till `90d` (90 days) in the future.
 For more information about the allowed date formats, check the
 `khal list` command, which is used for this functionality. It is assumed
 that the `khal` calendar called `my_calendar` exists. Make sure
 `my_calendar` is a calendar that exists on your local file system.
 
-### –format
+#### –format
+
 If `khalorg list --format` option is not defined, the default one is
 used which can be found at `./khalorg/static/khalorg_format.txt`. If you
 want to define your own format, you have 2 options: you can use the
 `khalorg list --format` option, or you can place your custom format at
 `$HOME/.config/khalorg/khalorg_format.txt` this format will then be used
 instead of the default one that is shown below.
 
-``` org
+```org
 * {title}
   {timestamps}
   :PROPERTIES:
   :ATTENDEES: {attendees}
   :CALENDAR: {calendar}
   :CATEGORIES: {categories}
   :LOCATION: {location}
@@ -176,14 +214,15 @@
   :UID: {uid}
   :URL: {url}
   :END:
   {description}
 ```
 
 the following keys are supported:
+
 - `{attendees}`: a comma separated list of email addresses of attendees
 - `{calendar}`: the name of the khal calendar
 - `{categories}`: the categories property of the item
 - `{description}`: the description of the item
 - `{location}`: the location of the item
 - `{organizer}`: the email of the organizer
 - `{status}`: the status of the item, e.g., TENTATIVE or ACCEPTED
@@ -195,137 +234,139 @@
 
 the following keys are supported but are typically reserved for internal use
 and are therefore less informative:
 
 - `{until}`: the until property value. Is empty when using `khalorg list`.
 - `{rrule}`: the ICal RRULE of the item.
 
-### Recurring items
+#### Recurring items
 
 The `khalorg list` command relies on the `khal list` command. Using this
 command the `RRULE` of each item is retrieved to created the correct org
 repeater. Only simple org repeaters are supported that have the
 following form: `+[number][h,w,m,y]`. Complex `RRULEs` are described by
 concatenating the corresponding timestamps within 1 agenda item,
 resulting in a list of items. For example, the agenda item below
 represents a weekly recurring event where the first meeting was moved to
 another date, resulting in a timestamp without a repeater, and one with
 a repeater.
 
-``` org
+```org
 * Meeting
   <2023-01-05 Thu 01:00-02:00>
   <2023-01-08 Sun 01:00-02:00 +1w>
   :PROPERTIES:
   :UID: 123
   :LOCATION: Somewhere
   :ORGANIZER: Someone (someone@outlook.com)
   :ATTENDEES: test@test.com, test2@test.com
   :URL: www.test.com
   :END:
   Hello,
-  
+
   Lets have a meeting.
-  
+
   Regards,
-  
-  
+
+
   Someone
 ```
 
-## New: from org to khal
+### New: from org to khal
 
 ![khalorg new demo](https://github.com/BartSte/khalorg/blob/main/demo/new.gif?raw=true)
 
 An org agenda item can be converted to a new `khal` agenda item by
 feeding the org item through stdin to `khalorg new` and specifying the
 khal calendar name as a positional argument. For example, the consider
 the org item below, which is saved as `meeting.org`.
 
-``` org
+```org
 * Meeting
   <2023-01-01 Sun 01:00-02:00 +1w>
   :PROPERTIES:
   :UID: 123
   :LOCATION: Somewhere
   :ORGANIZER: Someone (someone@outlook.com)
   :ATTENDEES: test@test.com, test2@test.com
   :URL: www.test.com
   :END:
   Hello,
-  
+
   Lets have a meeting.
-  
+
   Regards,
-  
-  
+
+
   Someone
 ```
 
 This item can be converted to the `khal` calendar called
 "my<sub>calendar</sub>" as follows:
 
-``` bash
+```bash
 cat meeting.org | khalorg new my_calendar
 ```
 
 It is assumed that the `khal` calendar called "my<sub>calendar</sub>"
 exists. Make sure "my<sub>calendar</sub>" is a calendar that exists on
 your local file system.
 
-### Recurring items
+#### Recurring items
+
 Only 1 timestamp per org item is supported. Note that the meeting above
 is repeated every week (`+1w`). Only simple org repeaters are supported
 that have the following form: `+[number][h,w,m,y]`. These events repeat
 forever, unless you specify an end date using the \`UNTIL\` property in
 the org file.
 
 Personally, when I need to create a complex repeat pattern (or when I
 need outlook specific items like a Teams invite), I create the event in
 outlook first. Next, I use `khalorg edit` to change the fields that need
 editing (e.g., the description).
 
-### Attendees
+#### Attendees
+
 Optionally, attendees can be added to the `ATTENDEES` property field.
 The attendees will be added to the `Attendees` field of `khal`. Once you
 synchronize `khal` with a server (e.g., outlook) an invitation will be
 send to the attendees.
 
-## Edit: from org to khal
+### Edit: from org to khal
 
 ![khalorg edit demo](https://github.com/BartSte/khalorg/blob/main/demo/edit.gif?raw=true)
 
 Existing `khal` events can be updates by feeding an org file with the
 corresponding UID through stdin to the `khalorg edit` command. For
 example, the org agenda item of <span class="spurious-link"
-target="New">*New*</span> can be altered and used as an input for
+target="New">_New_</span> can be altered and used as an input for
 `khalorg edit`, as long as the UID remains untouched.
 
-``` org
+```org
 * Edited meeting
   <2023-01-01 Sun 01:00-02:00 +1w>
   :PROPERTIES:
   :UID: 123
   :ORGANIZER: Someone (someone@outlook.com)
   :ATTENDEES: other@test.com
   :END:
   Hello,
-  
+
   I edited the meeting by removing the location and url. I also changed the
   title and the attendees field.
-  
+
   Regards,
-  
-  
+
+
   Someone
 ```
 
 Next, run the following command:
 
-``` bash
+```bash
 cat meeting.org | khalorg edit my_calendar
 ```
 
 When using `khalorg edit` please consider the following:
 
 - Editing an existing event is different from creating a new one as the
   original `icalendar` file is retained. Only parts of it are altered.
@@ -335,62 +376,67 @@
 - Only the PROTO event is edited, i.e., the whole series is altered not
   only the occurence.
 - `khal edit` will only update the dates + recurrence if the
   `--edit-dates` flag is passed. This avoids editing the start-stop date
   when editing an event that contains multiple timestamps (which are not
   supported).
 
-## Delete: from org to khal
- 
+### Delete: from org to khal
+
 ![khalorg deleted demo](https://github.com/BartSte/khalorg/blob/main/demo/delete.gif?raw=true)
 
 An event can be deleted from a khal calendar by feeding an org file to the
 `khalorg delete` command through stdin. The org file must contain an agenda
 item with a non-empty UID property. For example, the khal event that was
-created using the <span class="spurious-link" target="New">*New*</span> command
+created using the <span class="spurious-link" target="New">_New_</span> command
 above can be removed by feeding the same file to `khalorg delete`:
 
-``` bash
+```bash
 cat meeting.org | khalorg delete my_calendar
 ```
 
-### Recurring items
+#### Recurring items
+
 When deleting recurring items the whole series will be removed. Removing
 occurrences is not supported.
 
 ## Neovim plugin
-The neovim plugin can be found here: [nvim-khalorg](https://github.com/BartSte/nvim-khalorg).
 
-# Workflow for Office 365
+The neovim plugin can be found here:
+[nvim-khalorg](https://github.com/BartSte/nvim-khalorg). Check out the demo at
+the top of the [page](#demo).
+
+## Workflow for Office 365
+
 The diagram below illustrates the workflow than can be achieved when using
 `khalorg`. The folder `extras`, on the
 [GitHub](https://github.com/BartSte/khalorg) page, contains a `bash` script
 called `calsync`, that synchronizes `vdirsyncer` calendars and exports them as
 an org file using the `khalorg list` command. Davmail is used as the CalDav
 server in this specific example.
 
-``` example
-┌──────────┐  
-│Office 365│  
-└┬─────────┘  
-┌▽──────┐     
-│Davmail│     
-└┬──────┘     
-┌▽─────────┐  
-│vdirsyncer│  
-└┬─────────┘  
-┌▽───┐        
-│khal│        
-└┬───┘        
+```example
+┌──────────┐
+│Office 365│
+└┬─────────┘
+┌▽──────┐
+│Davmail│
+└┬──────┘
+┌▽─────────┐
+│vdirsyncer│
+└┬─────────┘
+┌▽───┐
+│khal│
+└┬───┘
 ┌▽───────┐
 │khalorg │
 └┬───────┘
-┌▽───────┐    
-│org mode│    
-└────────┘    
+┌▽───────┐
+│org mode│
+└────────┘
 ```
 
 ## Troubleshooting
 
 If you encounter any issues, please report them on the issue tracker at:
 [khalorg issues](https://github.com/BartSte/khalorg/issues)
 
@@ -399,24 +445,25 @@
 Contributions are welcome! Please see [CONTRIBUTING](./CONTRIBUTING.md) for
 more information.
 
 ## License
 
 Distributed under the [MIT License](./LICENCE).
 
-# Improvements:
+## Improvements:
+
 - [ ] Timezones are not yet supported, so `khalorg` will only work when
-  you agenda remain in the timezone that you specified within your
-  `khal` config.
+      you agenda remain in the timezone that you specified within your
+      `khal` config.
 - [ ] Running khal commands directly from a script in not
-  straightforward. Therefore, khal is executed as a subprocess, by using
-  its command line interface.
+      straightforward. Therefore, khal is executed as a subprocess, by using
+      its command line interface.
 - [ ] `khalorg new` and `khal edit` only support 1 timestamp per item.
-  However, it is desired that all timestamps within 1 org agenda item,
-  end up in 1 khal event, as is the case for the `orgagenda`. To achieve
-  this the following could be build:
+      However, it is desired that all timestamps within 1 org agenda item,
+      end up in 1 khal event, as is the case for the `orgagenda`. To achieve
+      this the following could be build:
   - [ ] When multiple timestamps without an org repeater are provided,
-    find the `RRULE` that describes them. Also, set the `UNTIL` date to
-    the last date. If no `RRULE` can be found, raise an error. Another
-    option could be to use the `RDATE` option of ICal.
+        find the `RRULE` that describes them. Also, set the `UNTIL` date to
+        the last date. If no `RRULE` can be found, raise an error. Another
+        option could be to use the `RDATE` option of ICal.
   - [ ] When multiple timestamps with an org repeater are presented, try
-    to find the `RRULE` that describes them.
+        to find the `RRULE` that describes them.
```

### Comparing `khalorg-0.0.0/README.md` & `khalorg-0.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,140 @@
-[Click here for the GitHub page.](https://github.com/BartSte/khalorg) 
+Metadata-Version: 2.1
+Name: khalorg
+Version: 0.0.1
+Summary: An interface between Org mode and Khal cli calendar.
+Author: BartSte
+License: MIT License
+Keywords: khal,org mode,vdirsyncer,CalDav,agenda,emacs,neovim,orgmode-nvim
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: khal>=0.11
+Requires-Dist: vdirsyncer
+Requires-Dist: orgparse
+Provides-Extra: debug
+Requires-Dist: ipdb; extra == "debug"
+Requires-Dist: ipython; extra == "debug"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Requires-Dist: twine; extra == "build"
+
+# Khalorg
+
+[Click here for the GitHub page.](https://github.com/BartSte/khalorg)
+
+<img src="./demo/logo.jpg" width=50%>
+
+## Demo
+
+The demo below demonstrates the following features using the neovim plugin
+called [nvim-khalorg](https://github.com/BartSte/nvim-khalorg):
+
+- `khalorg new`: convert an org agenda item into a `khal` agenda item.
+- `khalorg list`: convert a `khal` agenda item into an org agenda item.
+- `khalorg edit`: edit an existing `khal` agenda item with org mode.
+- `khalorg delete`: delete an existing `khal` item.
 
-# Contents
+![neovim-plugin](https://github.com/BartSte/khalorg/blob/main/demo/neovim-plugin.gif?raw=true)
+
+## Contents
+
+<!--toc:start-->
+
+- [Demo](#demo)
+- [Contents](#contents)
 - [Introduction](#introduction)
+  - [Definitions](#definitions)
+  - [Motivation](#motivation)
+  - [Features](#features)
 - [Installation](#installation)
+  - [PyPi](#pypi)
+  - [From source](#from-source)
+  - [For development](#for-development)
 - [Usage](#usage)
+  - [List: from khal to org](#list-from-khal-to-org)
+    - [–format](#format)
+    - [Recurring items](#recurring-items)
+  - [New: from org to khal](#new-from-org-to-khal)
+    - [Recurring items](#recurring-items)
+    - [Attendees](#attendees)
+  - [Edit: from org to khal](#edit-from-org-to-khal)
+  - [Delete: from org to khal](#delete-from-org-to-khal)
+    - [Recurring items](#recurring-items)
 - [Neovim plugin](#neovim-plugin)
 - [Workflow for Office 365](#workflow-for-office-365)
 - [Troubleshooting](#troubleshooting)
 - [Contributing](#contributing)
 - [License](#license)
-- [Improvements](#improvements)
+- [Improvements:](#improvements)
+
+<!--toc:end-->
+
+## Introduction
 
-# Introduction
 `khalorg` is an interface between Org mode and Khal cli calendar.
 
-## Definitions
-- [CalDav](<https://en.wikipedia.org/wiki/CalDAV>): internet standard for client access to calendars
-- [Davmail](<https://davmail.sourceforge.net/e>): CalDav exchange gateway
-- [khal](<https://github.com/pimutils/khal>): command line calendar app 
-- [khalel](<https://gitlab.com/hperrey/khalel>): interface between emacs and khal
-- [nvim-orgmode](<https://github.com/nvim-orgmode/orgmode>): org mode for neovim
-- [org](<https://orgmode.org>): plain text system for keeping notes, agendas and more
-- [vdirsyncer](<https://github.com/pimutils/vdirsyncer>): synchronizes calendars and addressbooks between servers and the local file system
+### Definitions
+
+- [CalDav](https://en.wikipedia.org/wiki/CalDAV): internet standard for client access to calendars
+- [Davmail](https://davmail.sourceforge.net/e): CalDav exchange gateway
+- [khal](https://github.com/pimutils/khal): command line calendar app
+- [khalel](https://gitlab.com/hperrey/khalel): interface between emacs and khal
+- [nvim-orgmode](https://github.com/nvim-orgmode/orgmode): org mode for neovim
+- [org](https://orgmode.org): plain text system for keeping notes, agendas and more
+- [vdirsyncer](https://github.com/pimutils/vdirsyncer): synchronizes calendars and addressbooks between servers and the local file system
+
+### Motivation
 
-## Motivation
 I use org mode to manage my agenda and my notes. However, in a professional
 setting, you are often required to use proprietary software for your agenda,
 like Office 365. Luckily, programs exist that can synchronize agendas from
 different sources, by implementing the CalDav standard. Personally, I like to
 use `vdirsyncer` with `khal` to synchronize my agendas. To bridge the gap
 between `khal` and `org mode`, only 1 program exists called: `khalel`. However,
 this program is designed for `emacs`. Since there are also org mode users
 outside of `emacs` (e.g. `neovim`), `khalorg` aims to be a general interface
 between `vdirsyncer`/`khal` and `org mode`.
 
 Based on the above, the following workflow is desired:
 
-``` example
-┌──────┐     
-│CalDav│     
-└┬─────┘     
-┌▽─────────┐  
-│vdirsyncer│  
-└┬─────────┘  
-┌▽───┐        
-│khal│        
-└┬───┘        
+```example
+┌──────┐
+│CalDav│
+└┬─────┘
+┌▽─────────┐
+│vdirsyncer│
+└┬─────────┘
+┌▽───┐
+│khal│
+└┬───┘
 ┌▽───────┐
 │khalorg │
 └┬───────┘
-┌▽───────┐    
-│org mode│    
-└────────┘    
+┌▽───────┐
+│org mode│
+└────────┘
 ```
 
-## Features
+### Features
+
 - [x] Can be used by org mode for emacs, vim and neovim.
 - [x] Vdirsyncer calendars can be manipulated by using the cli of `khal`
-  as the interface.
+      as the interface.
 - [x] `khalorg new`: convert an org agenda item into a `khal` agenda
-  item.
+      item.
 - [x] `khalorg list`: convert a `khal` agenda item into an org agenda
-  item.
+      item.
 - [x] `khalorg edit`: edit an existing `khal` agenda item with org mode.
 - [x] `khalorg delete`: delete an existing `khal` item.
 - [x] Recurring items are supported by providing an org repeater in the
-  time stamp (e.g., `+1w`). The following is supported:
+      time stamp (e.g., `+1w`). The following is supported:
   - the follow org repeaters: `+{integer}{d,w,m,y}`
   - `khalorg new` and `khalorg edit --edit-dates` support 1 time stamp
     per org agenda item.
   - `khalorg list` concatenates timestamps that cannot be describes by
     an org repeater, resulting in an org agenda item with multiple
     timestamps.
   - Supports an `until` date for recurring items. The until date can be
@@ -77,82 +142,93 @@
 - [x] Has unittests
 - [x] Includes an Office 365 workflow with a bash script
 - [x] Semantic versioning
 - [x] Gifs with demos
 - [x] Neovim plugin
 - [x] Is available on PyPI
 
-# Installation
+## Installation
+
 For safety, always make a back-up of your calendar before installing software
 that is new to you.
 
 Make sure your `khal` date format is compatible with org, otherwise it
 will not work. When running `khal printformats` you should get:
-``` example
+
+```example
 longdatetimeformat: 2013-12-21 Sat 21:45
 datetimeformat: 2013-12-21 Sat 21:45
 longdateformat: 2013-12-21 Sat
 dateformat: 2013-12-21 Sat
 timeformat: 21:45
 ```
+
 If not, check the documentation of `khal` on how to change this.
 
-## PyPi
+### PyPi
+
 Install by running the following command:
-``` bash
+
+```bash
 pip install khalorg
 ```
 
-## From source
+### From source
+
 Set your current working directory to the root directory, i.e, the
 directory containing the `pyproject.toml` file. Next, run:
 
-``` bash
+```bash
 pip install .
 ```
+
 After this, the executable `khalorg` will be available.
 
-## For development
+### For development
+
 If you want to develop the code, debug it, and test it, run:
-``` bash
+
+```bash
 pip install -e '.[test,debug]'
 ```
 
-# Usage
+## Usage
+
 Use `khalorg --help` to get information about the cli of `khalorg`. The
 following section discuss the `khalorg` commands that are available.
 
-## List: from khal to org
+### List: from khal to org
 
 ![khalorg list demo](https://github.com/BartSte/khalorg/blob/main/demo/list.gif?raw=true)
 
 Agenda items from `khal` can be converted to org items using the
 `khalorg list` command. For examples:
 
-``` bash
-khalorg list my_calendar today 90d > my_calendar.org 
+```bash
+khalorg list my_calendar today 90d > my_calendar.org
 ```
 
 Here, the `khal` agenda items of the calendar `my_calendar` are
 converted to org format and written to a file called `my_calendar.org`.
 The range is specified from `today` till `90d` (90 days) in the future.
 For more information about the allowed date formats, check the
 `khal list` command, which is used for this functionality. It is assumed
 that the `khal` calendar called `my_calendar` exists. Make sure
 `my_calendar` is a calendar that exists on your local file system.
 
-### –format
+#### –format
+
 If `khalorg list --format` option is not defined, the default one is
 used which can be found at `./khalorg/static/khalorg_format.txt`. If you
 want to define your own format, you have 2 options: you can use the
 `khalorg list --format` option, or you can place your custom format at
 `$HOME/.config/khalorg/khalorg_format.txt` this format will then be used
 instead of the default one that is shown below.
 
-``` org
+```org
 * {title}
   {timestamps}
   :PROPERTIES:
   :ATTENDEES: {attendees}
   :CALENDAR: {calendar}
   :CATEGORIES: {categories}
   :LOCATION: {location}
@@ -161,14 +237,15 @@
   :UID: {uid}
   :URL: {url}
   :END:
   {description}
 ```
 
 the following keys are supported:
+
 - `{attendees}`: a comma separated list of email addresses of attendees
 - `{calendar}`: the name of the khal calendar
 - `{categories}`: the categories property of the item
 - `{description}`: the description of the item
 - `{location}`: the location of the item
 - `{organizer}`: the email of the organizer
 - `{status}`: the status of the item, e.g., TENTATIVE or ACCEPTED
@@ -180,137 +257,139 @@
 
 the following keys are supported but are typically reserved for internal use
 and are therefore less informative:
 
 - `{until}`: the until property value. Is empty when using `khalorg list`.
 - `{rrule}`: the ICal RRULE of the item.
 
-### Recurring items
+#### Recurring items
 
 The `khalorg list` command relies on the `khal list` command. Using this
 command the `RRULE` of each item is retrieved to created the correct org
 repeater. Only simple org repeaters are supported that have the
 following form: `+[number][h,w,m,y]`. Complex `RRULEs` are described by
 concatenating the corresponding timestamps within 1 agenda item,
 resulting in a list of items. For example, the agenda item below
 represents a weekly recurring event where the first meeting was moved to
 another date, resulting in a timestamp without a repeater, and one with
 a repeater.
 
-``` org
+```org
 * Meeting
   <2023-01-05 Thu 01:00-02:00>
   <2023-01-08 Sun 01:00-02:00 +1w>
   :PROPERTIES:
   :UID: 123
   :LOCATION: Somewhere
   :ORGANIZER: Someone (someone@outlook.com)
   :ATTENDEES: test@test.com, test2@test.com
   :URL: www.test.com
   :END:
   Hello,
-  
+
   Lets have a meeting.
-  
+
   Regards,
-  
-  
+
+
   Someone
 ```
 
-## New: from org to khal
+### New: from org to khal
 
 ![khalorg new demo](https://github.com/BartSte/khalorg/blob/main/demo/new.gif?raw=true)
 
 An org agenda item can be converted to a new `khal` agenda item by
 feeding the org item through stdin to `khalorg new` and specifying the
 khal calendar name as a positional argument. For example, the consider
 the org item below, which is saved as `meeting.org`.
 
-``` org
+```org
 * Meeting
   <2023-01-01 Sun 01:00-02:00 +1w>
   :PROPERTIES:
   :UID: 123
   :LOCATION: Somewhere
   :ORGANIZER: Someone (someone@outlook.com)
   :ATTENDEES: test@test.com, test2@test.com
   :URL: www.test.com
   :END:
   Hello,
-  
+
   Lets have a meeting.
-  
+
   Regards,
-  
-  
+
+
   Someone
 ```
 
 This item can be converted to the `khal` calendar called
 "my<sub>calendar</sub>" as follows:
 
-``` bash
+```bash
 cat meeting.org | khalorg new my_calendar
 ```
 
 It is assumed that the `khal` calendar called "my<sub>calendar</sub>"
 exists. Make sure "my<sub>calendar</sub>" is a calendar that exists on
 your local file system.
 
-### Recurring items
+#### Recurring items
+
 Only 1 timestamp per org item is supported. Note that the meeting above
 is repeated every week (`+1w`). Only simple org repeaters are supported
 that have the following form: `+[number][h,w,m,y]`. These events repeat
 forever, unless you specify an end date using the \`UNTIL\` property in
 the org file.
 
 Personally, when I need to create a complex repeat pattern (or when I
 need outlook specific items like a Teams invite), I create the event in
 outlook first. Next, I use `khalorg edit` to change the fields that need
 editing (e.g., the description).
 
-### Attendees
+#### Attendees
+
 Optionally, attendees can be added to the `ATTENDEES` property field.
 The attendees will be added to the `Attendees` field of `khal`. Once you
 synchronize `khal` with a server (e.g., outlook) an invitation will be
 send to the attendees.
 
-## Edit: from org to khal
+### Edit: from org to khal
 
 ![khalorg edit demo](https://github.com/BartSte/khalorg/blob/main/demo/edit.gif?raw=true)
 
 Existing `khal` events can be updates by feeding an org file with the
 corresponding UID through stdin to the `khalorg edit` command. For
 example, the org agenda item of <span class="spurious-link"
-target="New">*New*</span> can be altered and used as an input for
+target="New">_New_</span> can be altered and used as an input for
 `khalorg edit`, as long as the UID remains untouched.
 
-``` org
+```org
 * Edited meeting
   <2023-01-01 Sun 01:00-02:00 +1w>
   :PROPERTIES:
   :UID: 123
   :ORGANIZER: Someone (someone@outlook.com)
   :ATTENDEES: other@test.com
   :END:
   Hello,
-  
+
   I edited the meeting by removing the location and url. I also changed the
   title and the attendees field.
-  
+
   Regards,
-  
-  
+
+
   Someone
 ```
 
 Next, run the following command:
 
-``` bash
+```bash
 cat meeting.org | khalorg edit my_calendar
 ```
 
 When using `khalorg edit` please consider the following:
 
 - Editing an existing event is different from creating a new one as the
   original `icalendar` file is retained. Only parts of it are altered.
@@ -320,62 +399,67 @@
 - Only the PROTO event is edited, i.e., the whole series is altered not
   only the occurence.
 - `khal edit` will only update the dates + recurrence if the
   `--edit-dates` flag is passed. This avoids editing the start-stop date
   when editing an event that contains multiple timestamps (which are not
   supported).
 
-## Delete: from org to khal
- 
+### Delete: from org to khal
+
 ![khalorg deleted demo](https://github.com/BartSte/khalorg/blob/main/demo/delete.gif?raw=true)
 
 An event can be deleted from a khal calendar by feeding an org file to the
 `khalorg delete` command through stdin. The org file must contain an agenda
 item with a non-empty UID property. For example, the khal event that was
-created using the <span class="spurious-link" target="New">*New*</span> command
+created using the <span class="spurious-link" target="New">_New_</span> command
 above can be removed by feeding the same file to `khalorg delete`:
 
-``` bash
+```bash
 cat meeting.org | khalorg delete my_calendar
 ```
 
-### Recurring items
+#### Recurring items
+
 When deleting recurring items the whole series will be removed. Removing
 occurrences is not supported.
 
 ## Neovim plugin
-The neovim plugin can be found here: [nvim-khalorg](https://github.com/BartSte/nvim-khalorg).
 
-# Workflow for Office 365
+The neovim plugin can be found here:
+[nvim-khalorg](https://github.com/BartSte/nvim-khalorg). Check out the demo at
+the top of the [page](#demo).
+
+## Workflow for Office 365
+
 The diagram below illustrates the workflow than can be achieved when using
 `khalorg`. The folder `extras`, on the
 [GitHub](https://github.com/BartSte/khalorg) page, contains a `bash` script
 called `calsync`, that synchronizes `vdirsyncer` calendars and exports them as
 an org file using the `khalorg list` command. Davmail is used as the CalDav
 server in this specific example.
 
-``` example
-┌──────────┐  
-│Office 365│  
-└┬─────────┘  
-┌▽──────┐     
-│Davmail│     
-└┬──────┘     
-┌▽─────────┐  
-│vdirsyncer│  
-└┬─────────┘  
-┌▽───┐        
-│khal│        
-└┬───┘        
+```example
+┌──────────┐
+│Office 365│
+└┬─────────┘
+┌▽──────┐
+│Davmail│
+└┬──────┘
+┌▽─────────┐
+│vdirsyncer│
+└┬─────────┘
+┌▽───┐
+│khal│
+└┬───┘
 ┌▽───────┐
 │khalorg │
 └┬───────┘
-┌▽───────┐    
-│org mode│    
-└────────┘    
+┌▽───────┐
+│org mode│
+└────────┘
 ```
 
 ## Troubleshooting
 
 If you encounter any issues, please report them on the issue tracker at:
 [khalorg issues](https://github.com/BartSte/khalorg/issues)
 
@@ -384,24 +468,25 @@
 Contributions are welcome! Please see [CONTRIBUTING](./CONTRIBUTING.md) for
 more information.
 
 ## License
 
 Distributed under the [MIT License](./LICENCE).
 
-# Improvements:
+## Improvements:
+
 - [ ] Timezones are not yet supported, so `khalorg` will only work when
-  you agenda remain in the timezone that you specified within your
-  `khal` config.
+      you agenda remain in the timezone that you specified within your
+      `khal` config.
 - [ ] Running khal commands directly from a script in not
-  straightforward. Therefore, khal is executed as a subprocess, by using
-  its command line interface.
+      straightforward. Therefore, khal is executed as a subprocess, by using
+      its command line interface.
 - [ ] `khalorg new` and `khal edit` only support 1 timestamp per item.
-  However, it is desired that all timestamps within 1 org agenda item,
-  end up in 1 khal event, as is the case for the `orgagenda`. To achieve
-  this the following could be build:
+      However, it is desired that all timestamps within 1 org agenda item,
+      end up in 1 khal event, as is the case for the `orgagenda`. To achieve
+      this the following could be build:
   - [ ] When multiple timestamps without an org repeater are provided,
-    find the `RRULE` that describes them. Also, set the `UNTIL` date to
-    the last date. If no `RRULE` can be found, raise an error. Another
-    option could be to use the `RDATE` option of ICal.
+        find the `RRULE` that describes them. Also, set the `UNTIL` date to
+        the last date. If no `RRULE` can be found, raise an error. Another
+        option could be to use the `RDATE` option of ICal.
   - [ ] When multiple timestamps with an org repeater are presented, try
-    to find the `RRULE` that describes them.
+        to find the `RRULE` that describes them.
```

### Comparing `khalorg-0.0.0/demo/delete.gif` & `khalorg-0.0.1/demo/delete.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/demo/edit.gif` & `khalorg-0.0.1/demo/edit.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/demo/list.gif` & `khalorg-0.0.1/demo/list.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/demo/new.gif` & `khalorg-0.0.1/demo/new.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/pyproject.toml` & `khalorg-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "khal>=0.11",
     "vdirsyncer",
     "orgparse"
 ]
-version = "0.0.0"
+version = "0.0.1"
 
 [project.optional-dependencies]
 debug = ["ipdb", "ipython"]
 test = ["pytest"]
 build = ["build", "twine"]
 
 [project.scripts]
```

### Comparing `khalorg-0.0.0/src/khalorg/cli.py` & `khalorg-0.0.1/src/khalorg/cli.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/src/khalorg/commands.py` & `khalorg-0.0.1/src/khalorg/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from khalorg.khal.checker import EventChecker, EventChecks
 from khalorg.khal.helpers import get_khal_format
 from khalorg.org.agenda_items import OrgAgendaFile, OrgAgendaItem
 
 
 def list_command(
         calendar: str,
-        khalorg_format: str = get_khalorg_format(),
+        khalorg_format: str | None  = None,
         start: str = 'today',
         stop: str = '1d',
         **_) -> str:
     """
     Lists khal agenda items to org format.
 
     Args:
@@ -27,14 +27,15 @@
         stop: end date (default: 1d)
 
     Returns
     -------
         stdout of the `khal list` command after post processing
 
     """
+    khalorg_format = khalorg_format or get_khalorg_format()
     args: KhalArgs = KhalArgs()
     args['-a'] = calendar
     args['-f'] = get_khal_format()
     args['start'] = start
     args['stop'] = stop
 
     khal_calendar: Calendar = Calendar(calendar)
```

### Comparing `khalorg-0.0.0/src/khalorg/helpers.py` & `khalorg-0.0.1/src/khalorg/helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/src/khalorg/khal/args.py` & `khalorg-0.0.1/src/khalorg/khal/args.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/src/khalorg/khal/calendar.py` & `khalorg-0.0.1/src/khalorg/khal/calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,16 @@
 
         Args:
         ----
             name: name of the khal calendar
         """
         path_config: Union[str, None] = find_configuration_file()
 
-        new_item_args: list = ['khal', 'new']
-        list_args: list = ['khal', 'list', '-df', '']
+        new_item_args: list = ["python3", "-m", "khal", "new"]
+        list_args: list = ["python3", "-m", "khal", "list", "-df", ""]
 
         self._collection: CalendarCollection
         self._new_item: Callable = subprocess_callback(new_item_args)
         self._list_command: Callable = subprocess_callback(list_args)
 
         self.name: str = name
         self.config: dict = get_config(path_config)
```

### Comparing `khalorg-0.0.0/src/khalorg/khal/checker.py` & `khalorg-0.0.1/src/khalorg/khal/checker.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/src/khalorg/khal/helpers.py` & `khalorg-0.0.1/src/khalorg/khal/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import sys
 from datetime import date, datetime
 from subprocess import STDOUT, CalledProcessError, check_output
 from typing import Callable
 
 from khalorg import paths
 
 Time = date | datetime
@@ -31,19 +32,25 @@
         timestamp: the time
 
     Returns:
     -------
         True if the `timestamp` is in the future
 
     """
+    logging.debug("Check if timestamp %s is in the future", timestamp)
     if isinstance(timestamp, datetime):
-        now: datetime = datetime.now(timestamp.tzinfo)
-        return timestamp >= now
+        logging.debug(
+            "Timestamp is a datetime object with tzinfo %s", timestamp.tzinfo
+        )
+        now = datetime.now(timestamp.tzinfo)
     else:
-        return timestamp >= datetime.now().date()
+        now = datetime.now().date()
+
+    logging.debug("Now is %s", now)
+    return timestamp >= now
 
 
 def subprocess_callback(cmd: list) -> Callable:
     """
     Returns a subprocess.check_output callback where the `cmd` is defined
     beforehand.
 
@@ -52,28 +59,30 @@
         cmd: the base command. For example: ['khal', 'new']
 
     Returns:
     -------
         callback function
 
     """
+
     def callback(args: list) -> str:
         return try_check_output([*cmd, *args]).decode()
 
     return callback
 
 
 def try_check_output(args: list) -> bytes:
     try:
-        return check_output(args, stderr=STDOUT)
+        return check_output(args, stderr=STDOUT, executable=sys.executable)
     except CalledProcessError as error:
         error_message: str = (
             f"The following arguments were sent to khal:\n\n{' '.join(args)}"
             "\n\nNext, the following error was received from khal:\n\n"
-            f"{error.output.decode()}\n\n")
+            f"{error.output.decode()}\n\n"
+        )
         logging.critical(error_message)
         raise Exception(error_message) from error
 
 
 def remove_tzinfo(time: Time) -> Time:
     """
     Remove tzinfo if possible.
```

### Comparing `khalorg-0.0.0/src/khalorg/org/agenda_items.py` & `khalorg-0.0.1/src/khalorg/org/agenda_items.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/src/khalorg/org/helpers.py` & `khalorg-0.0.1/src/khalorg/org/helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/src/khalorg/rrule.py` & `khalorg-0.0.1/src/khalorg/rrule.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/src/khalorg/static/description_list_command.txt` & `khalorg-0.0.1/src/khalorg/static/description_list_command.txt`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/src/khalorg.egg-info/PKG-INFO` & `khalorg-0.0.1/src/khalorg.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,140 @@
 Metadata-Version: 2.1
 Name: khalorg
-Version: 0.0.0
+Version: 0.0.1
 Summary: An interface between Org mode and Khal cli calendar.
 Author: BartSte
 License: MIT License
 Keywords: khal,org mode,vdirsyncer,CalDav,agenda,emacs,neovim,orgmode-nvim
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: khal>=0.11
+Requires-Dist: vdirsyncer
+Requires-Dist: orgparse
 Provides-Extra: debug
+Requires-Dist: ipdb; extra == "debug"
+Requires-Dist: ipython; extra == "debug"
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 Provides-Extra: build
-License-File: LICENCE
+Requires-Dist: build; extra == "build"
+Requires-Dist: twine; extra == "build"
+
+# Khalorg
+
+[Click here for the GitHub page.](https://github.com/BartSte/khalorg)
+
+<img src="./demo/logo.jpg" width=50%>
+
+## Demo
 
-[Click here for the GitHub page.](https://github.com/BartSte/khalorg) 
+The demo below demonstrates the following features using the neovim plugin
+called [nvim-khalorg](https://github.com/BartSte/nvim-khalorg):
 
-# Contents
+- `khalorg new`: convert an org agenda item into a `khal` agenda item.
+- `khalorg list`: convert a `khal` agenda item into an org agenda item.
+- `khalorg edit`: edit an existing `khal` agenda item with org mode.
+- `khalorg delete`: delete an existing `khal` item.
+
+![neovim-plugin](https://github.com/BartSte/khalorg/blob/main/demo/neovim-plugin.gif?raw=true)
+
+## Contents
+
+<!--toc:start-->
+
+- [Demo](#demo)
+- [Contents](#contents)
 - [Introduction](#introduction)
+  - [Definitions](#definitions)
+  - [Motivation](#motivation)
+  - [Features](#features)
 - [Installation](#installation)
+  - [PyPi](#pypi)
+  - [From source](#from-source)
+  - [For development](#for-development)
 - [Usage](#usage)
+  - [List: from khal to org](#list-from-khal-to-org)
+    - [–format](#format)
+    - [Recurring items](#recurring-items)
+  - [New: from org to khal](#new-from-org-to-khal)
+    - [Recurring items](#recurring-items)
+    - [Attendees](#attendees)
+  - [Edit: from org to khal](#edit-from-org-to-khal)
+  - [Delete: from org to khal](#delete-from-org-to-khal)
+    - [Recurring items](#recurring-items)
 - [Neovim plugin](#neovim-plugin)
 - [Workflow for Office 365](#workflow-for-office-365)
 - [Troubleshooting](#troubleshooting)
 - [Contributing](#contributing)
 - [License](#license)
-- [Improvements](#improvements)
+- [Improvements:](#improvements)
+
+<!--toc:end-->
+
+## Introduction
 
-# Introduction
 `khalorg` is an interface between Org mode and Khal cli calendar.
 
-## Definitions
-- [CalDav](<https://en.wikipedia.org/wiki/CalDAV>): internet standard for client access to calendars
-- [Davmail](<https://davmail.sourceforge.net/e>): CalDav exchange gateway
-- [khal](<https://github.com/pimutils/khal>): command line calendar app 
-- [khalel](<https://gitlab.com/hperrey/khalel>): interface between emacs and khal
-- [nvim-orgmode](<https://github.com/nvim-orgmode/orgmode>): org mode for neovim
-- [org](<https://orgmode.org>): plain text system for keeping notes, agendas and more
-- [vdirsyncer](<https://github.com/pimutils/vdirsyncer>): synchronizes calendars and addressbooks between servers and the local file system
+### Definitions
+
+- [CalDav](https://en.wikipedia.org/wiki/CalDAV): internet standard for client access to calendars
+- [Davmail](https://davmail.sourceforge.net/e): CalDav exchange gateway
+- [khal](https://github.com/pimutils/khal): command line calendar app
+- [khalel](https://gitlab.com/hperrey/khalel): interface between emacs and khal
+- [nvim-orgmode](https://github.com/nvim-orgmode/orgmode): org mode for neovim
+- [org](https://orgmode.org): plain text system for keeping notes, agendas and more
+- [vdirsyncer](https://github.com/pimutils/vdirsyncer): synchronizes calendars and addressbooks between servers and the local file system
+
+### Motivation
 
-## Motivation
 I use org mode to manage my agenda and my notes. However, in a professional
 setting, you are often required to use proprietary software for your agenda,
 like Office 365. Luckily, programs exist that can synchronize agendas from
 different sources, by implementing the CalDav standard. Personally, I like to
 use `vdirsyncer` with `khal` to synchronize my agendas. To bridge the gap
 between `khal` and `org mode`, only 1 program exists called: `khalel`. However,
 this program is designed for `emacs`. Since there are also org mode users
 outside of `emacs` (e.g. `neovim`), `khalorg` aims to be a general interface
 between `vdirsyncer`/`khal` and `org mode`.
 
 Based on the above, the following workflow is desired:
 
-``` example
-┌──────┐     
-│CalDav│     
-└┬─────┘     
-┌▽─────────┐  
-│vdirsyncer│  
-└┬─────────┘  
-┌▽───┐        
-│khal│        
-└┬───┘        
+```example
+┌──────┐
+│CalDav│
+└┬─────┘
+┌▽─────────┐
+│vdirsyncer│
+└┬─────────┘
+┌▽───┐
+│khal│
+└┬───┘
 ┌▽───────┐
 │khalorg │
 └┬───────┘
-┌▽───────┐    
-│org mode│    
-└────────┘    
+┌▽───────┐
+│org mode│
+└────────┘
 ```
 
-## Features
+### Features
+
 - [x] Can be used by org mode for emacs, vim and neovim.
 - [x] Vdirsyncer calendars can be manipulated by using the cli of `khal`
-  as the interface.
+      as the interface.
 - [x] `khalorg new`: convert an org agenda item into a `khal` agenda
-  item.
+      item.
 - [x] `khalorg list`: convert a `khal` agenda item into an org agenda
-  item.
+      item.
 - [x] `khalorg edit`: edit an existing `khal` agenda item with org mode.
 - [x] `khalorg delete`: delete an existing `khal` item.
 - [x] Recurring items are supported by providing an org repeater in the
-  time stamp (e.g., `+1w`). The following is supported:
+      time stamp (e.g., `+1w`). The following is supported:
   - the follow org repeaters: `+{integer}{d,w,m,y}`
   - `khalorg new` and `khalorg edit --edit-dates` support 1 time stamp
     per org agenda item.
   - `khalorg list` concatenates timestamps that cannot be describes by
     an org repeater, resulting in an org agenda item with multiple
     timestamps.
   - Supports an `until` date for recurring items. The until date can be
@@ -92,82 +142,93 @@
 - [x] Has unittests
 - [x] Includes an Office 365 workflow with a bash script
 - [x] Semantic versioning
 - [x] Gifs with demos
 - [x] Neovim plugin
 - [x] Is available on PyPI
 
-# Installation
+## Installation
+
 For safety, always make a back-up of your calendar before installing software
 that is new to you.
 
 Make sure your `khal` date format is compatible with org, otherwise it
 will not work. When running `khal printformats` you should get:
-``` example
+
+```example
 longdatetimeformat: 2013-12-21 Sat 21:45
 datetimeformat: 2013-12-21 Sat 21:45
 longdateformat: 2013-12-21 Sat
 dateformat: 2013-12-21 Sat
 timeformat: 21:45
 ```
+
 If not, check the documentation of `khal` on how to change this.
 
-## PyPi
+### PyPi
+
 Install by running the following command:
-``` bash
+
+```bash
 pip install khalorg
 ```
 
-## From source
+### From source
+
 Set your current working directory to the root directory, i.e, the
 directory containing the `pyproject.toml` file. Next, run:
 
-``` bash
+```bash
 pip install .
 ```
+
 After this, the executable `khalorg` will be available.
 
-## For development
+### For development
+
 If you want to develop the code, debug it, and test it, run:
-``` bash
+
+```bash
 pip install -e '.[test,debug]'
 ```
 
-# Usage
+## Usage
+
 Use `khalorg --help` to get information about the cli of `khalorg`. The
 following section discuss the `khalorg` commands that are available.
 
-## List: from khal to org
+### List: from khal to org
 
 ![khalorg list demo](https://github.com/BartSte/khalorg/blob/main/demo/list.gif?raw=true)
 
 Agenda items from `khal` can be converted to org items using the
 `khalorg list` command. For examples:
 
-``` bash
-khalorg list my_calendar today 90d > my_calendar.org 
+```bash
+khalorg list my_calendar today 90d > my_calendar.org
 ```
 
 Here, the `khal` agenda items of the calendar `my_calendar` are
 converted to org format and written to a file called `my_calendar.org`.
 The range is specified from `today` till `90d` (90 days) in the future.
 For more information about the allowed date formats, check the
 `khal list` command, which is used for this functionality. It is assumed
 that the `khal` calendar called `my_calendar` exists. Make sure
 `my_calendar` is a calendar that exists on your local file system.
 
-### –format
+#### –format
+
 If `khalorg list --format` option is not defined, the default one is
 used which can be found at `./khalorg/static/khalorg_format.txt`. If you
 want to define your own format, you have 2 options: you can use the
 `khalorg list --format` option, or you can place your custom format at
 `$HOME/.config/khalorg/khalorg_format.txt` this format will then be used
 instead of the default one that is shown below.
 
-``` org
+```org
 * {title}
   {timestamps}
   :PROPERTIES:
   :ATTENDEES: {attendees}
   :CALENDAR: {calendar}
   :CATEGORIES: {categories}
   :LOCATION: {location}
@@ -176,14 +237,15 @@
   :UID: {uid}
   :URL: {url}
   :END:
   {description}
 ```
 
 the following keys are supported:
+
 - `{attendees}`: a comma separated list of email addresses of attendees
 - `{calendar}`: the name of the khal calendar
 - `{categories}`: the categories property of the item
 - `{description}`: the description of the item
 - `{location}`: the location of the item
 - `{organizer}`: the email of the organizer
 - `{status}`: the status of the item, e.g., TENTATIVE or ACCEPTED
@@ -195,137 +257,139 @@
 
 the following keys are supported but are typically reserved for internal use
 and are therefore less informative:
 
 - `{until}`: the until property value. Is empty when using `khalorg list`.
 - `{rrule}`: the ICal RRULE of the item.
 
-### Recurring items
+#### Recurring items
 
 The `khalorg list` command relies on the `khal list` command. Using this
 command the `RRULE` of each item is retrieved to created the correct org
 repeater. Only simple org repeaters are supported that have the
 following form: `+[number][h,w,m,y]`. Complex `RRULEs` are described by
 concatenating the corresponding timestamps within 1 agenda item,
 resulting in a list of items. For example, the agenda item below
 represents a weekly recurring event where the first meeting was moved to
 another date, resulting in a timestamp without a repeater, and one with
 a repeater.
 
-``` org
+```org
 * Meeting
   <2023-01-05 Thu 01:00-02:00>
   <2023-01-08 Sun 01:00-02:00 +1w>
   :PROPERTIES:
   :UID: 123
   :LOCATION: Somewhere
   :ORGANIZER: Someone (someone@outlook.com)
   :ATTENDEES: test@test.com, test2@test.com
   :URL: www.test.com
   :END:
   Hello,
-  
+
   Lets have a meeting.
-  
+
   Regards,
-  
-  
+
+
   Someone
 ```
 
-## New: from org to khal
+### New: from org to khal
 
 ![khalorg new demo](https://github.com/BartSte/khalorg/blob/main/demo/new.gif?raw=true)
 
 An org agenda item can be converted to a new `khal` agenda item by
 feeding the org item through stdin to `khalorg new` and specifying the
 khal calendar name as a positional argument. For example, the consider
 the org item below, which is saved as `meeting.org`.
 
-``` org
+```org
 * Meeting
   <2023-01-01 Sun 01:00-02:00 +1w>
   :PROPERTIES:
   :UID: 123
   :LOCATION: Somewhere
   :ORGANIZER: Someone (someone@outlook.com)
   :ATTENDEES: test@test.com, test2@test.com
   :URL: www.test.com
   :END:
   Hello,
-  
+
   Lets have a meeting.
-  
+
   Regards,
-  
-  
+
+
   Someone
 ```
 
 This item can be converted to the `khal` calendar called
 "my<sub>calendar</sub>" as follows:
 
-``` bash
+```bash
 cat meeting.org | khalorg new my_calendar
 ```
 
 It is assumed that the `khal` calendar called "my<sub>calendar</sub>"
 exists. Make sure "my<sub>calendar</sub>" is a calendar that exists on
 your local file system.
 
-### Recurring items
+#### Recurring items
+
 Only 1 timestamp per org item is supported. Note that the meeting above
 is repeated every week (`+1w`). Only simple org repeaters are supported
 that have the following form: `+[number][h,w,m,y]`. These events repeat
 forever, unless you specify an end date using the \`UNTIL\` property in
 the org file.
 
 Personally, when I need to create a complex repeat pattern (or when I
 need outlook specific items like a Teams invite), I create the event in
 outlook first. Next, I use `khalorg edit` to change the fields that need
 editing (e.g., the description).
 
-### Attendees
+#### Attendees
+
 Optionally, attendees can be added to the `ATTENDEES` property field.
 The attendees will be added to the `Attendees` field of `khal`. Once you
 synchronize `khal` with a server (e.g., outlook) an invitation will be
 send to the attendees.
 
-## Edit: from org to khal
+### Edit: from org to khal
 
 ![khalorg edit demo](https://github.com/BartSte/khalorg/blob/main/demo/edit.gif?raw=true)
 
 Existing `khal` events can be updates by feeding an org file with the
 corresponding UID through stdin to the `khalorg edit` command. For
 example, the org agenda item of <span class="spurious-link"
-target="New">*New*</span> can be altered and used as an input for
+target="New">_New_</span> can be altered and used as an input for
 `khalorg edit`, as long as the UID remains untouched.
 
-``` org
+```org
 * Edited meeting
   <2023-01-01 Sun 01:00-02:00 +1w>
   :PROPERTIES:
   :UID: 123
   :ORGANIZER: Someone (someone@outlook.com)
   :ATTENDEES: other@test.com
   :END:
   Hello,
-  
+
   I edited the meeting by removing the location and url. I also changed the
   title and the attendees field.
-  
+
   Regards,
-  
-  
+
+
   Someone
 ```
 
 Next, run the following command:
 
-``` bash
+```bash
 cat meeting.org | khalorg edit my_calendar
 ```
 
 When using `khalorg edit` please consider the following:
 
 - Editing an existing event is different from creating a new one as the
   original `icalendar` file is retained. Only parts of it are altered.
@@ -335,62 +399,67 @@
 - Only the PROTO event is edited, i.e., the whole series is altered not
   only the occurence.
 - `khal edit` will only update the dates + recurrence if the
   `--edit-dates` flag is passed. This avoids editing the start-stop date
   when editing an event that contains multiple timestamps (which are not
   supported).
 
-## Delete: from org to khal
- 
+### Delete: from org to khal
+
 ![khalorg deleted demo](https://github.com/BartSte/khalorg/blob/main/demo/delete.gif?raw=true)
 
 An event can be deleted from a khal calendar by feeding an org file to the
 `khalorg delete` command through stdin. The org file must contain an agenda
 item with a non-empty UID property. For example, the khal event that was
-created using the <span class="spurious-link" target="New">*New*</span> command
+created using the <span class="spurious-link" target="New">_New_</span> command
 above can be removed by feeding the same file to `khalorg delete`:
 
-``` bash
+```bash
 cat meeting.org | khalorg delete my_calendar
 ```
 
-### Recurring items
+#### Recurring items
+
 When deleting recurring items the whole series will be removed. Removing
 occurrences is not supported.
 
 ## Neovim plugin
-The neovim plugin can be found here: [nvim-khalorg](https://github.com/BartSte/nvim-khalorg).
 
-# Workflow for Office 365
+The neovim plugin can be found here:
+[nvim-khalorg](https://github.com/BartSte/nvim-khalorg). Check out the demo at
+the top of the [page](#demo).
+
+## Workflow for Office 365
+
 The diagram below illustrates the workflow than can be achieved when using
 `khalorg`. The folder `extras`, on the
 [GitHub](https://github.com/BartSte/khalorg) page, contains a `bash` script
 called `calsync`, that synchronizes `vdirsyncer` calendars and exports them as
 an org file using the `khalorg list` command. Davmail is used as the CalDav
 server in this specific example.
 
-``` example
-┌──────────┐  
-│Office 365│  
-└┬─────────┘  
-┌▽──────┐     
-│Davmail│     
-└┬──────┘     
-┌▽─────────┐  
-│vdirsyncer│  
-└┬─────────┘  
-┌▽───┐        
-│khal│        
-└┬───┘        
+```example
+┌──────────┐
+│Office 365│
+└┬─────────┘
+┌▽──────┐
+│Davmail│
+└┬──────┘
+┌▽─────────┐
+│vdirsyncer│
+└┬─────────┘
+┌▽───┐
+│khal│
+└┬───┘
 ┌▽───────┐
 │khalorg │
 └┬───────┘
-┌▽───────┐    
-│org mode│    
-└────────┘    
+┌▽───────┐
+│org mode│
+└────────┘
 ```
 
 ## Troubleshooting
 
 If you encounter any issues, please report them on the issue tracker at:
 [khalorg issues](https://github.com/BartSte/khalorg/issues)
 
@@ -399,24 +468,25 @@
 Contributions are welcome! Please see [CONTRIBUTING](./CONTRIBUTING.md) for
 more information.
 
 ## License
 
 Distributed under the [MIT License](./LICENCE).
 
-# Improvements:
+## Improvements:
+
 - [ ] Timezones are not yet supported, so `khalorg` will only work when
-  you agenda remain in the timezone that you specified within your
-  `khal` config.
+      you agenda remain in the timezone that you specified within your
+      `khal` config.
 - [ ] Running khal commands directly from a script in not
-  straightforward. Therefore, khal is executed as a subprocess, by using
-  its command line interface.
+      straightforward. Therefore, khal is executed as a subprocess, by using
+      its command line interface.
 - [ ] `khalorg new` and `khal edit` only support 1 timestamp per item.
-  However, it is desired that all timestamps within 1 org agenda item,
-  end up in 1 khal event, as is the case for the `orgagenda`. To achieve
-  this the following could be build:
+      However, it is desired that all timestamps within 1 org agenda item,
+      end up in 1 khal event, as is the case for the `orgagenda`. To achieve
+      this the following could be build:
   - [ ] When multiple timestamps without an org repeater are provided,
-    find the `RRULE` that describes them. Also, set the `UNTIL` date to
-    the last date. If no `RRULE` can be found, raise an error. Another
-    option could be to use the `RDATE` option of ICal.
+        find the `RRULE` that describes them. Also, set the `UNTIL` date to
+        the last date. If no `RRULE` can be found, raise an error. Another
+        option could be to use the `RDATE` option of ICal.
   - [ ] When multiple timestamps with an org repeater are presented, try
-    to find the `RRULE` that describes them.
+        to find the `RRULE` that describes them.
```

### Comparing `khalorg-0.0.0/src/khalorg.egg-info/SOURCES.txt` & `khalorg-0.0.1/src/khalorg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 .gitignore
 CHANGELOG.md
 CONTRIBUTING.md
 LICENCE
 README.md
-publish
 pyproject.toml
 setup.py
+.github/workflows/release.yml
+.github/workflows/test.yml
 demo/delete.gif
 demo/edit.gif
 demo/list.gif
+demo/logo.jpg
 demo/meeting.org
+demo/neovim-plugin.gif
 demo/new.gif
 extras/calsync
 src/khalorg/__init__.py
 src/khalorg/__main__.py
 src/khalorg/cli.py
 src/khalorg/commands.py
 src/khalorg/helpers.py
```

### Comparing `khalorg-0.0.0/tests/agenda_items.py` & `khalorg-0.0.1/tests/agenda_items.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/helpers.py` & `khalorg-0.0.1/tests/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
 
     Returns
     -------
         the start and end times when planning an even now.
 
     """
     # must be in the future
-    start: datetime = datetime.now() + timedelta(minutes=1)
+    start: datetime = datetime.now() + timedelta(minutes=2)
     end: datetime = start + delta
 
     if all_day:
         return datetime.date(start), datetime.date(end)
     else:
         start = start.replace(second=0, microsecond=0)
         end = end.replace(second=0, microsecond=0)
```

### Comparing `khalorg-0.0.0/tests/khalorg_tester` & `khalorg-0.0.1/tests/khalorg_tester`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/static/agenda_items/duplicate.org` & `khalorg-0.0.1/tests/static/agenda_items/duplicate.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/static/agenda_items/multiple_timestamps.org` & `khalorg-0.0.1/tests/static/agenda_items/multiple_timestamps.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/static/agenda_items/multiple_timestamps_unsorted.org` & `khalorg-0.0.1/tests/static/agenda_items/multiple_timestamps_unsorted.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/static/agenda_items/recurring_first_item_moved.org` & `khalorg-0.0.1/tests/static/agenda_items/recurring_first_item_moved.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/static/agenda_items/recurring_first_item_moved_expected.org` & `khalorg-0.0.1/tests/static/agenda_items/recurring_first_item_moved_expected.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/static/agenda_items/rrule_recurring.org` & `khalorg-0.0.1/tests/static/agenda_items/rrule_recurring.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/static/agenda_items/rrule_recurring_and_non_recurring.org` & `khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_and_non_recurring.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/static/agenda_items/rrule_recurring_duplicates.org` & `khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_duplicates.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/static/agenda_items/two_items.org` & `khalorg-0.0.1/tests/static/agenda_items/two_items.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/static/test_config_khal` & `khalorg-0.0.1/tests/static/test_config_khal`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/test_cli.py` & `khalorg-0.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/test_commands.py` & `khalorg-0.0.1/tests/test_commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import date, datetime, timedelta
+import logging
 from os.path import join
 from tests import static
 from tests.helpers import (
     assert_event_created,
     assert_event_deleted,
     assert_event_edited,
     get_module_path,
@@ -80,16 +81,20 @@
     stdout: str = list_command('one', khalorg_format)
     actual.load_from_str(stdout)
 
     # UID and CALENDAR are changed in the process.
     expected.properties['UID'] = actual.properties['UID']
     expected.properties['CALENDAR'] = actual.properties['CALENDAR']
     expected.properties['RRULE'] = actual.properties['RRULE']
-    assert str(expected) == str(actual), f'Org item: {expected}'
 
+    logging.debug("khalorg_format: %s", khalorg_format)
+    logging.debug("Stdout: %s", stdout)
+    logging.debug("Expected: %s", expected)
+    logging.debug("Actual: %s", actual)
+    assert str(expected) == str(actual)
     # A recurring item should have a non empty rrule
     assert bool(actual.properties['RRULE']) == bool(expected.first_timestamp._repeater)  # noqa
 
 
 def test_list_recurring(runner):
     """ List supported recurring items. """
     daily = [(1, 'd'), (2, 'd')]
```

### Comparing `khalorg-0.0.0/tests/test_helpers.py` & `khalorg-0.0.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/test_khal/test_args.py` & `khalorg-0.0.1/tests/test_khal/test_args.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 from datetime import datetime
-from tests.agenda_items import AllDay, Recurring, Valid
-from tests.helpers import (
-    read_org_test_file,
-)
-from tests.test_khal.helpers import Mixin
+from os.path import join
 from unittest import TestCase
+from unittest.mock import patch
 
 from khalorg.khal.args import EditArgs, NewArgs
 from khalorg.khal.helpers import set_tzinfo
 from khalorg.org.agenda_items import OrgAgendaItem
 
+from tests import static
+from tests.agenda_items import AllDay, Recurring, Valid
+from tests.helpers import (
+    get_module_path,
+    read_org_test_file,
+)
+from tests.test_khal.helpers import Mixin
+
 FORMAT = '%Y-%m-%d %a %H:%M'
 
 
+def test_config_khal():
+    return join(get_module_path(static), 'test_config_khal')
+
+
+@patch('khalorg.khal.args.find_configuration_file', new=test_config_khal)
 class TestArgs(Mixin, TestCase):
 
     def test_load_from_org(self):
         """
         When loaded from the org file valid.org, the resulting cli
         args must be the same as: Valid.command_line_args
         .
@@ -102,14 +112,15 @@
             '2024-01-01 Mon 01:00',
             '2023-01-01 Sun 00:00']
 
         actual: list = args.as_list()
         self.assertEqual(actual, expected)
 
 
+@patch('khalorg.khal.args.find_configuration_file', new=test_config_khal)
 class TestEditArgs(Mixin, TestCase):
 
     def test(self):
         """
         For the agenda item `/test/static/agenda_items/recurring.org` the
         EditArgs should be equal to `expected`.
         """
```

### Comparing `khalorg-0.0.0/tests/test_khal/test_calendar.py` & `khalorg-0.0.1/tests/test_khal/test_calendar.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/test_khal/test_checker.py` & `khalorg-0.0.1/tests/test_khal/test_checker.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/test_org/test_agenda_items.py` & `khalorg-0.0.1/tests/test_org/test_agenda_items.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/test_org/test_helpers.py` & `khalorg-0.0.1/tests/test_org/test_helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.0/tests/test_rrule.py` & `khalorg-0.0.1/tests/test_rrule.py`

 * *Files identical despite different names*

