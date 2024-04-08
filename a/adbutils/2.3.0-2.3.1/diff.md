# Comparing `tmp/adbutils-2.3.0.tar.gz` & `tmp/adbutils-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbutils-2.3.0.tar", last modified: Sun Apr  7 12:31:00 2024, max compression
+gzip compressed data, was "adbutils-2.3.1.tar", last modified: Mon Apr  8 04:31:59 2024, max compression
```

## Comparing `adbutils-2.3.0.tar` & `adbutils-2.3.1.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.760258 adbutils-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-07 12:30:54.000000 adbutils-2.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.752258 adbutils-2.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-07 12:30:54.000000 adbutils-2.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.752258 adbutils-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-07 12:30:54.000000 adbutils-2.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-07 12:30:54.000000 adbutils-2.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-07 12:30:54.000000 adbutils-2.3.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 12:31:00.000000 adbutils-2.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-07 12:31:00.000000 adbutils-2.3.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-07 12:30:54.000000 adbutils-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-07 12:31:00.760258 adbutils-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-07 12:30:54.000000 adbutils-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/adbutils/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/adbutils/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/binaries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/pidcat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/screenrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/adbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.752258 adbutils-2.3.0/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-04-07 12:30:54.000000 adbutils-2.3.0/assets/images/pidcat.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-04-07 12:30:54.000000 adbutils-2.3.0/build_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 12:30:54.000000 adbutils-2.3.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-07 12:30:54.000000 adbutils-2.3.0/examples/reset-offline.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 12:30:54.000000 adbutils-2.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-07 12:30:54.000000 adbutils-2.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-07 12:31:00.760258 adbutils-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-07 12:30:54.000000 adbutils-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/test_real_device/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_forward_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.760258 adbutils-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-07 12:30:54.000000 adbutils-2.3.0/tests/adb_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-07 12:30:54.000000 adbutils-2.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-07 12:30:54.000000 adbutils-2.3.0/tests/test_adb_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-08 04:31:53.000000 adbutils-2.3.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.855289 adbutils-2.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 04:31:53.000000 adbutils-2.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.855289 adbutils-2.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-08 04:31:53.000000 adbutils-2.3.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-08 04:31:53.000000 adbutils-2.3.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-08 04:31:53.000000 adbutils-2.3.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 04:31:59.000000 adbutils-2.3.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 04:31:59.000000 adbutils-2.3.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 04:31:53.000000 adbutils-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-08 04:31:59.859289 adbutils-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-04-08 04:31:53.000000 adbutils-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.855289 adbutils-2.3.1/adbutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/adbutils/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/binaries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/pidcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/screenrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-08 04:31:53.000000 adbutils-2.3.1/adbutils/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.855289 adbutils-2.3.1/adbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 04:31:59.000000 adbutils-2.3.1/adbutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.851289 adbutils-2.3.1/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-04-08 04:31:53.000000 adbutils-2.3.1/assets/images/pidcat.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-04-08 04:31:53.000000 adbutils-2.3.1/build_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 04:31:53.000000 adbutils-2.3.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-08 04:31:53.000000 adbutils-2.3.1/examples/reset-offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 04:31:53.000000 adbutils-2.3.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 04:31:53.000000 adbutils-2.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 04:31:59.859289 adbutils-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-08 04:31:53.000000 adbutils-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/test_real_device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_forward_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-08 04:31:53.000000 adbutils-2.3.1/test_real_device/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:31:59.859289 adbutils-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-08 04:31:53.000000 adbutils-2.3.1/tests/adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 04:31:53.000000 adbutils-2.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-08 04:31:53.000000 adbutils-2.3.1/tests/test_adb_server.py
```

### Comparing `adbutils-2.3.0/.coveragerc` & `adbutils-2.3.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/.github/workflows/main.yml` & `adbutils-2.3.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/.github/workflows/publish-to-pypi.yml` & `adbutils-2.3.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/.travis.yml` & `adbutils-2.3.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/LICENSE` & `adbutils-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/PKG-INFO` & `adbutils-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.3.0
+Version: 2.3.1
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.3.0/README.md` & `adbutils-2.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,15 @@
 $ adb devices
 ```
 
 ## Changes from 1.x to 2.x
 
 ### Remove
 - current_app removed, use app_current instead
-- package_info removed, use app_info instead
+- package_info is going to remove, use app_info instead
 
 ### Add
 - add volume_up, volume_down, volume_mute
 
 ## Generate TOC
 ```bash
 gh-md-toc --insert README.md
```

### Comparing `adbutils-2.3.0/adbutils/__init__.py` & `adbutils-2.3.1/adbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/adbutils/__main__.py` & `adbutils-2.3.1/adbutils/__main__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/adbutils/_adb.py` & `adbutils-2.3.1/adbutils/_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/adbutils/_device.py` & `adbutils-2.3.1/adbutils/_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import socket
 import subprocess
 import threading
 import typing
 from typing import Optional, Union
 
 
+from adbutils._deprecated import DeprecatedExtension
 from adbutils.install import InstallExtension
 from adbutils.screenrecord import ScreenrecordExtension
 from adbutils.screenshot import ScreenshotExtesion
 
 from adbutils._adb import AdbConnection, BaseClient
 from adbutils._proto import *
 from adbutils._proto import StrOrPathLike
@@ -446,14 +447,15 @@
 
 class AdbDevice(
     BaseDevice,
     ShellExtension,
     ScreenrecordExtension,
     ScreenshotExtesion,
     InstallExtension,
+    DeprecatedExtension,
 ):
     """provide custom functions for some complex operations"""
 
     def __init__(
         self, client: BaseClient, serial: str = None, transport_id: int = None
     ):
         BaseDevice.__init__(self, client, serial, transport_id)
```

### Comparing `adbutils-2.3.0/adbutils/_proto.py` & `adbutils-2.3.1/adbutils/_proto.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/adbutils/_utils.py` & `adbutils-2.3.1/adbutils/_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/adbutils/errors.py` & `adbutils-2.3.1/adbutils/errors.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/adbutils/install.py` & `adbutils-2.3.1/adbutils/install.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/adbutils/pidcat.py` & `adbutils-2.3.1/adbutils/pidcat.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/adbutils/screenrecord.py` & `adbutils-2.3.1/adbutils/screenrecord.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/adbutils/screenshot.py` & `adbutils-2.3.1/adbutils/screenshot.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/adbutils/shell.py` & `adbutils-2.3.1/adbutils/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
 
     def app_stop(self, package_name: str):
         """stop app with "am force-stop" """
         self.shell(["am", "force-stop", package_name])
 
     def app_clear(self, package_name: str):
         self.shell(["pm", "clear", package_name])
-
+    
     def app_info(self, package_name: str) -> Optional[AppInfo]:
         """
         Get app info
 
         Returns:
             None or AppInfo
         """
```

### Comparing `adbutils-2.3.0/adbutils/sync.py` & `adbutils-2.3.1/adbutils/sync.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/adbutils.egg-info/PKG-INFO` & `adbutils-2.3.1/adbutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.3.0
+Version: 2.3.1
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.3.0/adbutils.egg-info/SOURCES.txt` & `adbutils-2.3.1/adbutils.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 setup.py
 .github/dependabot.yml
 .github/workflows/main.yml
 .github/workflows/publish-to-pypi.yml
 adbutils/__init__.py
 adbutils/__main__.py
 adbutils/_adb.py
+adbutils/_deprecated.py
 adbutils/_device.py
 adbutils/_proto.py
 adbutils/_utils.py
 adbutils/_version.py
 adbutils/errors.py
 adbutils/install.py
 adbutils/pidcat.py
```

### Comparing `adbutils-2.3.0/assets/images/pidcat.png` & `adbutils-2.3.1/assets/images/pidcat.png`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/build_wheel.py` & `adbutils-2.3.1/build_wheel.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/examples/reset-offline.py` & `adbutils-2.3.1/examples/reset-offline.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/setup.cfg` & `adbutils-2.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/test_real_device/conftest.py` & `adbutils-2.3.1/test_real_device/conftest.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/test_real_device/test_adb.py` & `adbutils-2.3.1/test_real_device/test_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/test_real_device/test_deprecated.py` & `adbutils-2.3.1/test_real_device/test_deprecated.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """Created on Mon May 09 2022 17:31:25 by codeskyblue
 """
 
 import pytest
 from adbutils import AdbDevice, adb
 
 
-@pytest.mark.skip("package_info is removed")
 def test_package_info(device: AdbDevice):
     pinfo = device.app_current()
     pinfo = device.package_info(pinfo.package)
     assert 'version_name' in pinfo
 
 
 @pytest.mark.skip("current_app is removed")
```

### Comparing `adbutils-2.3.0/test_real_device/test_device.py` & `adbutils-2.3.1/test_real_device/test_device.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/test_real_device/test_forward_reverse.py` & `adbutils-2.3.1/test_real_device/test_forward_reverse.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/test_real_device/test_utils.py` & `adbutils-2.3.1/test_real_device/test_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/tests/adb_server.py` & `adbutils-2.3.1/tests/adb_server.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.3.0/tests/conftest.py` & `adbutils-2.3.1/tests/conftest.py`

 * *Files identical despite different names*

