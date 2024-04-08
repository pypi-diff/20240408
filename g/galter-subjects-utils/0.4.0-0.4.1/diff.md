# Comparing `tmp/galter-subjects-utils-0.4.0.tar.gz` & `tmp/galter-subjects-utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galter-subjects-utils-0.4.0.tar", last modified: Fri Apr  5 12:48:52 2024, max compression
+gzip compressed data, was "galter-subjects-utils-0.4.1.tar", last modified: Mon Apr  8 20:29:29 2024, max compression
```

## Comparing `galter-subjects-utils-0.4.0.tar` & `galter-subjects-utils-0.4.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.210984 galter-subjects-utils-0.4.0/galter_subjects_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.210984 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.214984 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.214984 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/deltor.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/keeptrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/types_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.214984 galter-subjects-utils-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.206984 galter-subjects-utils-0.4.0/tests/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/tests/contrib/lcsh/
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/contrib/lcsh/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/contrib/lcsh/test_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/tests/contrib/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/contrib/mesh/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/contrib/mesh/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/contrib/mesh/test_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/tests/downloads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/downloads/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/test_deltor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/test_keeptrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/test_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.606305 galter-subjects-utils-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-08 20:29:29.606305 galter-subjects-utils-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.598306 galter-subjects-utils-0.4.1/galter_subjects_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.598306 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/deltor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/keeptrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/types_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:29:29.606305 galter-subjects-utils-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.594306 galter-subjects-utils-0.4.1/tests/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/tests/contrib/lcsh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/contrib/lcsh/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/contrib/lcsh/test_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/tests/contrib/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/contrib/mesh/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/contrib/mesh/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/contrib/mesh/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/tests/downloads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/downloads/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/test_deltor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/test_keeptrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/test_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/test_writer.py
```

### Comparing `galter-subjects-utils-0.4.0/LICENSE` & `galter-subjects-utils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/MANIFEST.in` & `galter-subjects-utils-0.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/PKG-INFO` & `galter-subjects-utils-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galter-subjects-utils
-Version: 0.4.0
+Version: 0.4.1
 Summary: Subject terms tooling for InvenioRDM
 Author-email: Northwestern University <DL_FSM_GDS@e.northwestern.edu>
 License: MIT License
         
         Copyright (C) 2021-2023 Northwestern University.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Repository, https://github.com/galterlibrary/galter-subjects-utils
-Keywords: invenio,inveniordm,subjects,MeSH
+Keywords: invenio,inveniordm,subjects
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -78,17 +78,18 @@
 pip install galter-subjects-utils
 ```
 
 ### Versions
 
 This repository follows [semantic versioning](https://semver.org/) indexed on invenio-app-rdm compatibility according to the table below:
 
-| This Version | invenio-app-rdm version |
-| ------------ | ----------------------- |
-| 0.3.X        | 11.X                    |
+| galter-subjects-utils | invenio-app-rdm version |
+| --------------------- | ----------------------- |
+| 0.3.X                 | 11.X                    |
+| 0.4.X                 | 11.X                    |
 
 This just means for example that version 0.3 guarantees generation of subjects files and subject manipulation compatible with invenio-app-rdm v11. When there is a break in subjects format, this tool will bump its major version.
 
 ## Usage
 
 ```bash
 pipenv run invenio galter-subjects --help
```

### Comparing `galter-subjects-utils-0.4.0/README.md` & `galter-subjects-utils-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 pip install galter-subjects-utils
 ```
 
 ### Versions
 
 This repository follows [semantic versioning](https://semver.org/) indexed on invenio-app-rdm compatibility according to the table below:
 
-| This Version | invenio-app-rdm version |
-| ------------ | ----------------------- |
-| 0.3.X        | 11.X                    |
+| galter-subjects-utils | invenio-app-rdm version |
+| --------------------- | ----------------------- |
+| 0.3.X                 | 11.X                    |
+| 0.4.X                 | 11.X                    |
 
 This just means for example that version 0.3 guarantees generation of subjects files and subject manipulation compatible with invenio-app-rdm v11. When there is a break in subjects format, this tool will bump its major version.
 
 ## Usage
 
 ```bash
 pipenv run invenio galter-subjects --help
```

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/adapter.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/adapter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/cli.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/cli.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/adapter.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/adapter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/cli.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,19 +99,22 @@
     downloader_kwargs = to_lcsh_downloader_kwargs(parameters)
     downloader = LCSHDownloader(**downloader_kwargs)
     downloader.download()
 
     # Convert
     converter_kwargs = to_lcsh_converter_kwargs(downloader)
     converter = LCSHRDMConverter(**converter_kwargs)
+    converted = converter.convert(),
+    # Exclude special automated geographic terms
+    converted_filtered = (s for s in converted if not s["id"].endswith("-781"))
 
     # Write
     header = ["id", "scheme", "subject"]
     filepath = write_csv(
-        converter.convert(),
+        converted_filtered,
         parameters["output_file"],
         writer_kwargs={
             "fieldnames": header
         }
     )
 
     print(f"LCSH terms written here {filepath}")
```

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/converter.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/converter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/downloader.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/scheme.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/scheme.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/adapter.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/adapter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/cli.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/cli.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/converter.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/converter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/downloader.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/reader.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/scheme.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/scheme.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/deltor.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/deltor.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/downloader.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/keeptrace.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/keeptrace.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/reader.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/scheme.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/scheme.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/updater.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/updater.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils/writer.py` & `galter-subjects-utils-0.4.1/galter_subjects_utils/writer.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/PKG-INFO` & `galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galter-subjects-utils
-Version: 0.4.0
+Version: 0.4.1
 Summary: Subject terms tooling for InvenioRDM
 Author-email: Northwestern University <DL_FSM_GDS@e.northwestern.edu>
 License: MIT License
         
         Copyright (C) 2021-2023 Northwestern University.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Repository, https://github.com/galterlibrary/galter-subjects-utils
-Keywords: invenio,inveniordm,subjects,MeSH
+Keywords: invenio,inveniordm,subjects
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -78,17 +78,18 @@
 pip install galter-subjects-utils
 ```
 
 ### Versions
 
 This repository follows [semantic versioning](https://semver.org/) indexed on invenio-app-rdm compatibility according to the table below:
 
-| This Version | invenio-app-rdm version |
-| ------------ | ----------------------- |
-| 0.3.X        | 11.X                    |
+| galter-subjects-utils | invenio-app-rdm version |
+| --------------------- | ----------------------- |
+| 0.3.X                 | 11.X                    |
+| 0.4.X                 | 11.X                    |
 
 This just means for example that version 0.3 guarantees generation of subjects files and subject manipulation compatible with invenio-app-rdm v11. When there is a break in subjects format, this tool will bump its major version.
 
 ## Usage
 
 ```bash
 pipenv run invenio galter-subjects --help
```

### Comparing `galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/SOURCES.txt` & `galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/pyproject.toml` & `galter-subjects-utils-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     "invenio_rdm_records",
     "invenio_records_resources",
     "invenio_vocabularies",
     "requests",
     "sqlalchemy",
 ]
 description = "Subject terms tooling for InvenioRDM"
-keywords = ["invenio", "inveniordm", "subjects", "MeSH"]
+keywords = ["invenio", "inveniordm", "subjects"]
 license = {file = "LICENSE"}
 name = "galter-subjects-utils"
 readme = "README.md"
 requires-python = ">=3.8"
 scripts = {galter-subjects-utils = "galter_subjects_utils.cli:main"}
 urls = {Repository = "https://github.com/galterlibrary/galter-subjects-utils"}
-version = "0.4.0"
+version = "0.4.1"
 
 [project.optional-dependencies]
 dev = [
     "check-manifest>=0.49",
     "invenio-search[opensearch2]>=2.1.0,<3.0.0",  # Needs to be specified separately as it's up to instance
     "invoke>=2.2,<3.0",
     "pytest-invenio>=2.1.1,<3.0.0",
```

### Comparing `galter-subjects-utils-0.4.0/tests/conftest.py` & `galter-subjects-utils-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/tests/contrib/lcsh/test_converter.py` & `galter-subjects-utils-0.4.1/tests/contrib/lcsh/test_converter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/tests/contrib/lcsh/test_downloader.py` & `galter-subjects-utils-0.4.1/tests/contrib/lcsh/test_downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/tests/contrib/mesh/test_converter.py` & `galter-subjects-utils-0.4.1/tests/contrib/mesh/test_converter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/tests/contrib/mesh/test_downloader.py` & `galter-subjects-utils-0.4.1/tests/contrib/mesh/test_downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/tests/contrib/mesh/test_reader.py` & `galter-subjects-utils-0.4.1/tests/contrib/mesh/test_reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/tests/test_deltor.py` & `galter-subjects-utils-0.4.1/tests/test_deltor.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/tests/test_keeptrace.py` & `galter-subjects-utils-0.4.1/tests/test_keeptrace.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/tests/test_reader.py` & `galter-subjects-utils-0.4.1/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/tests/test_updater.py` & `galter-subjects-utils-0.4.1/tests/test_updater.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.0/tests/test_writer.py` & `galter-subjects-utils-0.4.1/tests/test_writer.py`

 * *Files identical despite different names*

