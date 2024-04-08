# Comparing `tmp/cads-api-client-0.9.1.tar.gz` & `tmp/cads-api-client-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cads-api-client-0.9.1.tar", last modified: Mon Mar 18 16:59:17 2024, max compression
+gzip compressed data, was "cads-api-client-0.9.2.tar", last modified: Wed Mar 20 18:16:39 2024, max compression
```

## Comparing `cads-api-client-0.9.1.tar` & `cads-api-client-0.9.2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:17.355065 cads-api-client-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:17.347065 cads-api-client-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:17.351065 cads-api-client-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-03-18 16:59:17.355065 cads-api-client-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:17.351065 cads-api-client-0.9.1/cads_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/cads_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/cads_api_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/cads_api_client/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/cads_api_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/cads_api_client/legacy_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/cads_api_client/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/cads_api_client/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/cads_api_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-18 16:59:17.000000 cads-api-client-0.9.1/cads_api_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:17.355065 cads-api-client-0.9.1/cads_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-03-18 16:59:17.000000 cads-api-client-0.9.1/cads_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-18 16:59:17.000000 cads-api-client-0.9.1/cads_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 16:59:17.000000 cads-api-client-0.9.1/cads_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-18 16:59:17.000000 cads-api-client-0.9.1/cads_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-18 16:59:17.000000 cads-api-client-0.9.1/cads_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:17.351065 cads-api-client-0.9.1/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:17.351065 cads-api-client-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:17.351065 cads-api-client-0.9.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:17.351065 cads-api-client-0.9.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:17.355065 cads-api-client-0.9.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/notebooks/cads_api_client_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/notebooks/cads_api_constraints_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/notebooks/cads_api_filters_and_pagination_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/notebooks/cads_api_licences_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 16:59:17.355065 cads-api-client-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:59:17.355065 cads-api-client-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/tests/integration_test_10_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/tests/integration_test_20_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/tests/integration_test_30_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/tests/integration_test_40_legacy_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/tests/test_10_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-03-18 16:59:08.000000 cads-api-client-0.9.1/tests/test_10_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.829143 cads-api-client-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.817142 cads-api-client-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.821143 cads-api-client-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-03-20 18:16:39.829143 cads-api-client-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.821143 cads-api-client-0.9.2/cads_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/legacy_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.829143 cads-api-client-0.9.2/cads_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/notebooks/cads_api_client_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/notebooks/cads_api_constraints_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/notebooks/cads_api_filters_and_pagination_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/notebooks/cads_api_licences_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 18:16:39.829143 cads-api-client-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/integration_test_10_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/integration_test_20_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/integration_test_30_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/integration_test_40_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/integration_test_50_legacy_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/test_10_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/test_10_processing.py
```

### Comparing `cads-api-client-0.9.1/.cruft.json` & `cads-api-client-0.9.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/.github/workflows/on-push.yml` & `cads-api-client-0.9.2/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/.gitignore` & `cads-api-client-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/.pre-commit-config.yaml` & `cads-api-client-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/LICENSE` & `cads-api-client-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/Makefile` & `cads-api-client-0.9.2/Makefile`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/PKG-INFO` & `cads-api-client-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-api-client
-Version: 0.9.1
+Version: 0.9.2
 Summary: CADS API Python client
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cads-api-client-0.9.1/README.md` & `cads-api-client-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/cads_api_client/__init__.py` & `cads-api-client-0.9.2/cads_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/cads_api_client/api_client.py` & `cads-api-client-0.9.2/cads_api_client/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,9 +101,9 @@
     def licences(self) -> Dict[str, Any]:
         return self.catalogue_api.licenses()
 
     @property
     def accepted_licences(self) -> Dict[str, Any]:
         return self.profile_api.accepted_licences()
 
-    def accept_licence(self, licence_id: str) -> Dict[str, Any]:
-        return self.profile_api.accept_licence(licence_id)
+    def accept_licence(self, licence_id: str, revision: int) -> Dict[str, Any]:
+        return self.profile_api.accept_licence(licence_id, revision=revision)
```

### Comparing `cads-api-client-0.9.1/cads_api_client/catalogue.py` & `cads-api-client-0.9.2/cads_api_client/catalogue.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/cads_api_client/config.py` & `cads-api-client-0.9.2/cads_api_client/config.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/cads_api_client/processing.py` & `cads-api-client-0.9.2/cads_api_client/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,19 +180,18 @@
         )
         requests_response.raise_for_status()
         json = requests_response.json()
         return json["status"]  # type: ignore
 
     def wait_on_result(self, retry_options: Dict[str, Any] = {}) -> None:
         sleep = 1.0
-        last_status = self._robust_status(retry_options=retry_options)
+        status = None
         while True:
-            status = self._robust_status(retry_options=retry_options)
-            if last_status != status:
-                logger.debug(f"status has been updated to {status}")
+            if status != (status := self._robust_status(retry_options=retry_options)):
+                logger.info(f"status has been updated to {status}")
             if status == "successful":
                 # workaround for the server-side 404 due to database replicas out od sync
                 time.sleep(1)
                 break
             elif status == "failed":
                 # workaround for the server-side 404 due to database replicas out od sync
                 time.sleep(1)
```

### Comparing `cads-api-client-0.9.1/cads_api_client/profile.py` & `cads-api-client-0.9.2/cads_api_client/profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,18 @@
         self.headers = headers
 
     def profile(self) -> Dict[str, Any]:
         url = f"{self.url}/account"
         response = processing.ApiResponse.from_request("get", url, headers=self.headers)
         return response.json
 
-    def accept_licence(self, licence_id: str) -> Dict[str, Any]:
+    def accept_licence(self, licence_id: str, revision: int) -> Dict[str, Any]:
         url = f"{self.url}/account/licences/{licence_id}"
-        response = processing.ApiResponse.from_request("put", url, headers=self.headers)
+        response = processing.ApiResponse.from_request(
+            "put", url, headers=self.headers, json={"revision": revision}
+        )
         return response.json
 
     def accepted_licences(self) -> Dict[str, Any]:
         url = f"{self.url}/account/licences"
         response = processing.ApiResponse.from_request("get", url, headers=self.headers)
         return response.json
```

### Comparing `cads-api-client-0.9.1/cads_api_client.egg-info/PKG-INFO` & `cads-api-client-0.9.2/cads_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-api-client
-Version: 0.9.1
+Version: 0.9.2
 Summary: CADS API Python client
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cads-api-client-0.9.1/cads_api_client.egg-info/SOURCES.txt` & `cads-api-client-0.9.2/cads_api_client.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,11 +35,12 @@
 notebooks/cads_api_constraints_test.ipynb
 notebooks/cads_api_filters_and_pagination_tests.ipynb
 notebooks/cads_api_licences_tests.ipynb
 tests/conftest.py
 tests/integration_test_10_catalogue.py
 tests/integration_test_20_processing.py
 tests/integration_test_30_remote.py
-tests/integration_test_40_legacy_api_client.py
+tests/integration_test_40_api_client.py
+tests/integration_test_50_legacy_api_client.py
 tests/test_00_version.py
 tests/test_10_config.py
 tests/test_10_processing.py
```

### Comparing `cads-api-client-0.9.1/docs/Makefile` & `cads-api-client-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/docs/conf.py` & `cads-api-client-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/docs/make.bat` & `cads-api-client-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/notebooks/cads_api_client_test.ipynb` & `cads-api-client-0.9.2/notebooks/cads_api_client_test.ipynb`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/notebooks/cads_api_constraints_test.ipynb` & `cads-api-client-0.9.2/notebooks/cads_api_constraints_test.ipynb`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/notebooks/cads_api_filters_and_pagination_tests.ipynb` & `cads-api-client-0.9.2/notebooks/cads_api_filters_and_pagination_tests.ipynb`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/notebooks/cads_api_licences_tests.ipynb` & `cads-api-client-0.9.2/notebooks/cads_api_licences_tests.ipynb`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/pyproject.toml` & `cads-api-client-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/tests/conftest.py` & `cads-api-client-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/tests/integration_test_10_catalogue.py` & `cads-api-client-0.9.2/tests/integration_test_10_catalogue.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/tests/integration_test_20_processing.py` & `cads-api-client-0.9.2/tests/integration_test_20_processing.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/tests/integration_test_30_remote.py` & `cads-api-client-0.9.2/tests/integration_test_30_remote.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/tests/test_10_config.py` & `cads-api-client-0.9.2/tests/test_10_config.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.1/tests/test_10_processing.py` & `cads-api-client-0.9.2/tests/test_10_processing.py`

 * *Files identical despite different names*

