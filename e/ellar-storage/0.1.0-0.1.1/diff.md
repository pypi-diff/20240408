# Comparing `tmp/ellar_storage-0.1.0.tar.gz` & `tmp/ellar_storage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar_storage-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ellar_storage-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ellar_storage-0.1.0.tar` & `ellar_storage-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0       65 2022-11-19 13:34:25.872132 ellar_storage-0.1.0/.dockerignore
--rw-r--r--   0        0        0      140 2023-08-08 12:55:09.403542 ellar_storage-0.1.0/.flake8
--rw-r--r--   0        0        0      205 2022-11-19 07:40:19.274325 ellar_storage-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      662 2024-04-07 17:21:21.279055 ellar_storage-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      535 2024-04-07 17:21:21.279408 ellar_storage-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1012 2024-03-29 12:25:18.413369 ellar_storage-0.1.0/.github/workflows/test_full.yml
--rw-r--r--   0        0        0     1892 2023-08-08 12:57:54.940044 ellar_storage-0.1.0/.gitignore
--rw-r--r--   0        0        0       53 2022-11-19 13:34:25.872663 ellar_storage-0.1.0/.isort.cfg
--rw-r--r--   0        0        0     1073 2023-02-09 07:38:33.894196 ellar_storage-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1083 2023-08-08 12:57:44.065537 ellar_storage-0.1.0/LICENSE
--rw-r--r--   0        0        0     1016 2024-03-29 12:25:18.418520 ellar_storage-0.1.0/Makefile
--rw-r--r--   0        0        0     7958 2024-04-07 17:47:04.210674 ellar_storage-0.1.0/README.md
--rw-r--r--   0        0        0      476 2024-04-04 07:01:50.448565 ellar_storage-0.1.0/ellar_storage/__init__.py
--rw-r--r--   0        0        0      103 2024-04-04 06:09:55.333199 ellar_storage-0.1.0/ellar_storage/constants.py
--rw-r--r--   0        0        0      889 2024-04-04 07:01:50.431750 ellar_storage-0.1.0/ellar_storage/exceptions.py
--rw-r--r--   0        0        0     1682 2024-04-07 17:47:27.076639 ellar_storage-0.1.0/ellar_storage/module.py
--rw-r--r--   0        0        0      110 2024-04-04 07:01:50.431614 ellar_storage-0.1.0/ellar_storage/providers.py
--rw-r--r--   0        0        0        0 2022-11-19 13:34:25.881062 ellar_storage-0.1.0/ellar_storage/py.typed
--rw-r--r--   0        0        0     1053 2024-04-04 07:01:50.448723 ellar_storage-0.1.0/ellar_storage/schemas.py
--rw-r--r--   0        0        0     6980 2024-04-04 08:59:36.731144 ellar_storage-0.1.0/ellar_storage/services.py
--rw-r--r--   0        0        0      273 2024-04-04 07:01:50.431958 ellar_storage-0.1.0/ellar_storage/storage.py
--rw-r--r--   0        0        0     3306 2024-04-04 08:47:11.454217 ellar_storage-0.1.0/ellar_storage/stored_file.py
--rw-r--r--   0        0        0      347 2024-04-01 20:27:54.462642 ellar_storage-0.1.0/ellar_storage/utils.py
--rw-r--r--   0        0        0     2546 2024-04-07 22:56:50.858652 ellar_storage-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      207 2022-11-19 13:34:25.883240 ellar_storage-0.1.0/pytest.ini
--rw-r--r--   0        0        0      165 2024-04-07 17:21:21.280824 ellar_storage-0.1.0/requirements-tests.txt
--rw-r--r--   0        0        0       43 2024-04-01 20:17:51.185948 ellar_storage-0.1.0/requirements.txt
--rw-r--r--   0        0        0      329 2024-04-07 17:21:21.281095 ellar_storage-0.1.0/samples/README.md
--rw-r--r--   0        0        0        0 2024-04-07 17:21:21.281139 ellar_storage-0.1.0/samples/ellar_storage_tut/__init__.py
--rw-r--r--   0        0        0     3305 2024-04-07 17:21:21.281462 ellar_storage-0.1.0/samples/ellar_storage_tut/config.py
--rw-r--r--   0        0        0     1548 2024-04-07 17:21:21.281933 ellar_storage-0.1.0/samples/ellar_storage_tut/controller.py
--rw-r--r--   0        0        0        0 2024-04-07 17:21:21.282012 ellar_storage-0.1.0/samples/ellar_storage_tut/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 17:21:21.282117 ellar_storage-0.1.0/samples/ellar_storage_tut/domain/__init__.py
--rw-r--r--   0        0        0       41 2024-04-07 17:21:21.282388 ellar_storage-0.1.0/samples/ellar_storage_tut/media/documents/docs.txt
--rw-r--r--   0        0        0       54 2024-04-07 17:21:21.282568 ellar_storage-0.1.0/samples/ellar_storage_tut/media/documents/docs.txt.metadata.json
--rw-r--r--   0        0        0       37 2024-04-07 17:21:21.282778 ellar_storage-0.1.0/samples/ellar_storage_tut/media/files/file.txt
--rw-r--r--   0        0        0       54 2024-04-07 17:21:21.282929 ellar_storage-0.1.0/samples/ellar_storage_tut/media/files/file.txt.metadata.json
--rw-r--r--   0        0        0       38 2024-04-07 17:21:21.283128 ellar_storage-0.1.0/samples/ellar_storage_tut/media/images/image.txt
--rw-r--r--   0        0        0       55 2024-04-07 17:21:21.283277 ellar_storage-0.1.0/samples/ellar_storage_tut/media/images/image.txt.metadata.json
--rw-r--r--   0        0        0      620 2024-04-07 17:21:21.283427 ellar_storage-0.1.0/samples/ellar_storage_tut/root_module.py
--rw-r--r--   0        0        0     2068 2024-04-07 17:21:21.283594 ellar_storage-0.1.0/samples/ellar_storage_tut/server.py
--rw-r--r--   0        0        0      413 2024-04-07 17:21:21.283749 ellar_storage-0.1.0/samples/manage.py
--rw-r--r--   0        0        0       23 2024-04-07 17:21:21.283889 ellar_storage-0.1.0/samples/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-07 17:21:21.283962 ellar_storage-0.1.0/samples/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-08-08 05:56:09.023147 ellar_storage-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      107 2024-04-07 17:21:21.284274 ellar_storage-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0       22 2024-04-04 04:01:00.311070 ellar_storage-0.1.0/tests/fixtures/test.txt
--rw-r--r--   0        0        0     2785 2024-04-04 08:47:11.469927 ellar_storage-0.1.0/tests/test_module.py
--rw-r--r--   0        0        0     2081 2024-04-04 07:01:50.448696 ellar_storage-0.1.0/tests/test_schema.py
--rw-r--r--   0        0        0     4609 2024-04-07 17:21:21.284685 ellar_storage-0.1.0/tests/test_service.py
--rw-r--r--   0        0        0     3270 2024-04-07 17:47:27.076684 ellar_storage-0.1.0/tests/test_service_async.py
--rw-r--r--   0        0        0      376 2024-04-07 17:21:21.285159 ellar_storage-0.1.0/tests/utils.py
--rw-r--r--   0        0        0     9611 1970-01-01 00:00:00.000000 ellar_storage-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2022-11-19 13:34:25.872132 ellar_storage-0.1.1/.dockerignore
+-rw-r--r--   0        0        0      140 2023-08-08 12:55:09.403542 ellar_storage-0.1.1/.flake8
+-rw-r--r--   0        0        0      205 2022-11-19 07:40:19.274325 ellar_storage-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      662 2024-04-07 17:21:21.279055 ellar_storage-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      535 2024-04-07 17:21:21.279408 ellar_storage-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1012 2024-03-29 12:25:18.413369 ellar_storage-0.1.1/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0     1892 2023-08-08 12:57:54.940044 ellar_storage-0.1.1/.gitignore
+-rw-r--r--   0        0        0       53 2022-11-19 13:34:25.872663 ellar_storage-0.1.1/.isort.cfg
+-rw-r--r--   0        0        0     1073 2023-02-09 07:38:33.894196 ellar_storage-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1083 2023-08-08 12:57:44.065537 ellar_storage-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1016 2024-03-29 12:25:18.418520 ellar_storage-0.1.1/Makefile
+-rw-r--r--   0        0        0     7960 2024-04-08 07:22:32.868533 ellar_storage-0.1.1/README.md
+-rw-r--r--   0        0        0      476 2024-04-08 07:22:43.331141 ellar_storage-0.1.1/ellar_storage/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-04 06:09:55.333199 ellar_storage-0.1.1/ellar_storage/constants.py
+-rw-r--r--   0        0        0      889 2024-04-04 07:01:50.431750 ellar_storage-0.1.1/ellar_storage/exceptions.py
+-rw-r--r--   0        0        0     1682 2024-04-07 17:47:27.076639 ellar_storage-0.1.1/ellar_storage/module.py
+-rw-r--r--   0        0        0      110 2024-04-04 07:01:50.431614 ellar_storage-0.1.1/ellar_storage/providers.py
+-rw-r--r--   0        0        0        0 2022-11-19 13:34:25.881062 ellar_storage-0.1.1/ellar_storage/py.typed
+-rw-r--r--   0        0        0     1053 2024-04-04 07:01:50.448723 ellar_storage-0.1.1/ellar_storage/schemas.py
+-rw-r--r--   0        0        0     6980 2024-04-04 08:59:36.731144 ellar_storage-0.1.1/ellar_storage/services.py
+-rw-r--r--   0        0        0      273 2024-04-04 07:01:50.431958 ellar_storage-0.1.1/ellar_storage/storage.py
+-rw-r--r--   0        0        0     3306 2024-04-04 08:47:11.454217 ellar_storage-0.1.1/ellar_storage/stored_file.py
+-rw-r--r--   0        0        0      347 2024-04-01 20:27:54.462642 ellar_storage-0.1.1/ellar_storage/utils.py
+-rw-r--r--   0        0        0     2545 2024-04-08 07:22:15.669806 ellar_storage-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      207 2022-11-19 13:34:25.883240 ellar_storage-0.1.1/pytest.ini
+-rw-r--r--   0        0        0      165 2024-04-07 17:21:21.280824 ellar_storage-0.1.1/requirements-tests.txt
+-rw-r--r--   0        0        0       43 2024-04-01 20:17:51.185948 ellar_storage-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      329 2024-04-07 17:21:21.281095 ellar_storage-0.1.1/samples/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 17:21:21.281139 ellar_storage-0.1.1/samples/ellar_storage_tut/__init__.py
+-rw-r--r--   0        0        0     3305 2024-04-07 17:21:21.281462 ellar_storage-0.1.1/samples/ellar_storage_tut/config.py
+-rw-r--r--   0        0        0     1548 2024-04-07 17:21:21.281933 ellar_storage-0.1.1/samples/ellar_storage_tut/controller.py
+-rw-r--r--   0        0        0        0 2024-04-07 17:21:21.282012 ellar_storage-0.1.1/samples/ellar_storage_tut/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 17:21:21.282117 ellar_storage-0.1.1/samples/ellar_storage_tut/domain/__init__.py
+-rw-r--r--   0        0        0       41 2024-04-07 17:21:21.282388 ellar_storage-0.1.1/samples/ellar_storage_tut/media/documents/docs.txt
+-rw-r--r--   0        0        0       54 2024-04-07 17:21:21.282568 ellar_storage-0.1.1/samples/ellar_storage_tut/media/documents/docs.txt.metadata.json
+-rw-r--r--   0        0        0       37 2024-04-07 17:21:21.282778 ellar_storage-0.1.1/samples/ellar_storage_tut/media/files/file.txt
+-rw-r--r--   0        0        0       54 2024-04-07 17:21:21.282929 ellar_storage-0.1.1/samples/ellar_storage_tut/media/files/file.txt.metadata.json
+-rw-r--r--   0        0        0       38 2024-04-07 17:21:21.283128 ellar_storage-0.1.1/samples/ellar_storage_tut/media/images/image.txt
+-rw-r--r--   0        0        0       55 2024-04-07 17:21:21.283277 ellar_storage-0.1.1/samples/ellar_storage_tut/media/images/image.txt.metadata.json
+-rw-r--r--   0        0        0      620 2024-04-07 17:21:21.283427 ellar_storage-0.1.1/samples/ellar_storage_tut/root_module.py
+-rw-r--r--   0        0        0     2068 2024-04-07 17:21:21.283594 ellar_storage-0.1.1/samples/ellar_storage_tut/server.py
+-rw-r--r--   0        0        0      413 2024-04-07 17:21:21.283749 ellar_storage-0.1.1/samples/manage.py
+-rw-r--r--   0        0        0       23 2024-04-07 17:21:21.283889 ellar_storage-0.1.1/samples/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-07 17:21:21.283962 ellar_storage-0.1.1/samples/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-08-08 05:56:09.023147 ellar_storage-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      107 2024-04-07 17:21:21.284274 ellar_storage-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0       22 2024-04-04 04:01:00.311070 ellar_storage-0.1.1/tests/fixtures/test.txt
+-rw-r--r--   0        0        0     2785 2024-04-04 08:47:11.469927 ellar_storage-0.1.1/tests/test_module.py
+-rw-r--r--   0        0        0     2081 2024-04-04 07:01:50.448696 ellar_storage-0.1.1/tests/test_schema.py
+-rw-r--r--   0        0        0     4609 2024-04-07 17:21:21.284685 ellar_storage-0.1.1/tests/test_service.py
+-rw-r--r--   0        0        0     3270 2024-04-07 17:47:27.076684 ellar_storage-0.1.1/tests/test_service_async.py
+-rw-r--r--   0        0        0      376 2024-04-07 17:21:21.285159 ellar_storage-0.1.1/tests/utils.py
+-rw-r--r--   0        0        0     9613 1970-01-01 00:00:00.000000 ellar_storage-0.1.1/PKG-INFO
```

### Comparing `ellar_storage-0.1.0/.github/workflows/publish.yml` & `ellar_storage-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/.github/workflows/test.yml` & `ellar_storage-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/.github/workflows/test_full.yml` & `ellar_storage-0.1.1/.github/workflows/test_full.yml`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/.gitignore` & `ellar_storage-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/.pre-commit-config.yaml` & `ellar_storage-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/LICENSE` & `ellar_storage-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/Makefile` & `ellar_storage-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/README.md` & `ellar_storage-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <p align="center">
   <a href="#" target="blank"><img src="https://python-ellar.github.io/ellar/img/EllarLogoB.png" width="200" alt="Ellar Logo" /></a>
 </p>
 
-![Test](https://github.com/eadwinCode/ellar-storage/actions/workflows/test_full.yml/badge.svg)
+![Test](https://github.com/python-ellar/ellar-storage/actions/workflows/test_full.yml/badge.svg)
 ![Coverage](https://img.shields.io/codecov/c/github/python-ellar/ellar-storage)
 [![PyPI version](https://badge.fury.io/py/ellar-storage.svg)](https://badge.fury.io/py/ellar-storage)
 [![PyPI version](https://img.shields.io/pypi/v/ellar-storage.svg)](https://pypi.python.org/pypi/ellar-storage)
 [![PyPI version](https://img.shields.io/pypi/pyversions/ellar-storage.svg)](https://pypi.python.org/pypi/ellar-storage)
 
 ## Introduction
 The EllarStorage Module enriches your Ellar application with robust support for managing both cloud and
```

### Comparing `ellar_storage-0.1.0/ellar_storage/exceptions.py` & `ellar_storage-0.1.1/ellar_storage/exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/ellar_storage/module.py` & `ellar_storage-0.1.1/ellar_storage/module.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/ellar_storage/schemas.py` & `ellar_storage-0.1.1/ellar_storage/schemas.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/ellar_storage/services.py` & `ellar_storage-0.1.1/ellar_storage/services.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/ellar_storage/stored_file.py` & `ellar_storage-0.1.1/ellar_storage/stored_file.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/pyproject.toml` & `ellar_storage-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -90,8 +90,7 @@
 warn_no_return = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 disallow_untyped_defs = true
 check_untyped_defs = true
 implicit_reexport = false
-
```

### Comparing `ellar_storage-0.1.0/samples/ellar_storage_tut/config.py` & `ellar_storage-0.1.1/samples/ellar_storage_tut/config.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/samples/ellar_storage_tut/controller.py` & `ellar_storage-0.1.1/samples/ellar_storage_tut/controller.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/samples/ellar_storage_tut/root_module.py` & `ellar_storage-0.1.1/samples/ellar_storage_tut/root_module.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/samples/ellar_storage_tut/server.py` & `ellar_storage-0.1.1/samples/ellar_storage_tut/server.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/tests/test_module.py` & `ellar_storage-0.1.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/tests/test_schema.py` & `ellar_storage-0.1.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/tests/test_service.py` & `ellar_storage-0.1.1/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/tests/test_service_async.py` & `ellar_storage-0.1.1/tests/test_service_async.py`

 * *Files identical despite different names*

### Comparing `ellar_storage-0.1.0/PKG-INFO` & `ellar_storage-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellar-storage
-Version: 0.1.0
+Version: 0.1.1
 Summary: Storage Module for Ellar
 Author-email: Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 Project-URL: Source, https://github.com/python-ellar/ellar-storage
 Provides-Extra: crypto
 
 <p align="center">
   <a href="#" target="blank"><img src="https://python-ellar.github.io/ellar/img/EllarLogoB.png" width="200" alt="Ellar Logo" /></a>
 </p>
 
-![Test](https://github.com/eadwinCode/ellar-storage/actions/workflows/test_full.yml/badge.svg)
+![Test](https://github.com/python-ellar/ellar-storage/actions/workflows/test_full.yml/badge.svg)
 ![Coverage](https://img.shields.io/codecov/c/github/python-ellar/ellar-storage)
 [![PyPI version](https://badge.fury.io/py/ellar-storage.svg)](https://badge.fury.io/py/ellar-storage)
 [![PyPI version](https://img.shields.io/pypi/v/ellar-storage.svg)](https://pypi.python.org/pypi/ellar-storage)
 [![PyPI version](https://img.shields.io/pypi/pyversions/ellar-storage.svg)](https://pypi.python.org/pypi/ellar-storage)
 
 ## Introduction
 The EllarStorage Module enriches your Ellar application with robust support for managing both cloud and
```

