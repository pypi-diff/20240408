# Comparing `tmp/datatrails-archivist-0.29.0a1.tar.gz` & `tmp/datatrails-archivist-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrails-archivist-0.29.0a1.tar", last modified: Tue Feb 27 10:51:22 2024, max compression
+gzip compressed data, was "datatrails-archivist-0.30.0.tar", last modified: Mon Apr  8 15:11:19 2024, max compression
```

## Comparing `datatrails-archivist-0.29.0a1.tar` & `datatrails-archivist-0.30.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:51:22.061844 datatrails-archivist-0.29.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-02-27 10:51:22.061844 datatrails-archivist-0.29.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12250 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:51:22.061844 datatrails-archivist-0.29.0a1/archivist/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-27 10:51:15.000000 datatrails-archivist-0.29.0a1/archivist/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/access_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/appidp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/archivist.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/archivistpublic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/assetattachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/attachments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:51:22.061844 datatrails-archivist-0.29.0a1/archivist/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:51:22.061844 datatrails-archivist-0.29.0a1/archivist/cmds/runner/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/cmds/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/cmds/runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/cmds/runner/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/cmds/runner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:51:22.061844 datatrails-archivist-0.29.0a1/archivist/cmds/template/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/cmds/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/cmds/template/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/cmds/template/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/cmds/template/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/compliance_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/compliance_policy_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/compliance_policy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/confirmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/dictmerge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/or_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/proof_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/retry429.py
--rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/sboms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/subjects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/subjects_confirmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/tenancies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/archivist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:51:22.061844 datatrails-archivist-0.29.0a1/datatrails_archivist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-02-27 10:51:22.000000 datatrails-archivist-0.29.0a1/datatrails_archivist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-27 10:51:22.000000 datatrails-archivist-0.29.0a1/datatrails_archivist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 10:51:22.000000 datatrails-archivist-0.29.0a1/datatrails_archivist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-27 10:51:22.000000 datatrails-archivist-0.29.0a1/datatrails_archivist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-27 10:51:22.000000 datatrails-archivist-0.29.0a1/datatrails_archivist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-27 10:51:22.000000 datatrails-archivist-0.29.0a1/datatrails_archivist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-27 10:49:18.000000 datatrails-archivist-0.29.0a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-27 10:51:22.061844 datatrails-archivist-0.29.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12250 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/archivist/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 15:11:16.000000 datatrails-archivist-0.30.0/archivist/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/access_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/appidp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/archivist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/archivistpublic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/assetattachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/attachments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/archivist/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/archivist/cmds/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/runner/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/runner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/archivist/cmds/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/template/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/template/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/template/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/compliance_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/compliance_policy_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/compliance_policy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/confirmation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/dictmerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/or_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/proof_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/retry429.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/sboms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/subjects_confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/tenancies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/setup.cfg
```

### Comparing `datatrails-archivist-0.29.0a1/LICENSE` & `datatrails-archivist-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/PKG-INFO` & `datatrails-archivist-0.30.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrails-archivist
-Version: 0.29.0a1
+Version: 0.30.0
 Summary: DataTrails API
 Home-page: https://github.com/datatrails/datatrails-python
 Author: DataTrails Inc.
 Author-email: support@datatrails.ai
 License: MIT
 Project-URL: Documentation, https://python.datatrails.ai
 Project-URL: Source, https://github.com/datatrails/datatrails-python
```

### Comparing `datatrails-archivist-0.29.0a1/README.rst` & `datatrails-archivist-0.30.0/README.rst`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/access_policies.py` & `datatrails-archivist-0.30.0/archivist/access_policies.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/appidp.py` & `datatrails-archivist-0.30.0/archivist/appidp.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/applications.py` & `datatrails-archivist-0.30.0/archivist/applications.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/archivist.py` & `datatrails-archivist-0.30.0/archivist/archivist.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/archivistpublic.py` & `datatrails-archivist-0.30.0/archivist/archivistpublic.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,15 +425,14 @@
             data = response.json()
 
             try:
                 records = data[field]
             except KeyError as ex:
                 raise ArchivistBadFieldError(f"No {field} found") from ex
 
-            for record in records:
-                yield record
+            yield from records
 
             page_token = data.get("next_page_token")
             if not page_token:
                 break
 
             params = {"page_token": page_token}
```

### Comparing `datatrails-archivist-0.29.0a1/archivist/asset.py` & `datatrails-archivist-0.30.0/archivist/asset.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/assetattachments.py` & `datatrails-archivist-0.30.0/archivist/assetattachments.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/assets.py` & `datatrails-archivist-0.30.0/archivist/assets.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/attachments.py` & `datatrails-archivist-0.30.0/archivist/attachments.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/cmds/runner/main.py` & `datatrails-archivist-0.30.0/archivist/cmds/runner/main.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/cmds/runner/run.py` & `datatrails-archivist-0.30.0/archivist/cmds/runner/run.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/cmds/template/main.py` & `datatrails-archivist-0.30.0/archivist/cmds/template/main.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/cmds/template/run.py` & `datatrails-archivist-0.30.0/archivist/cmds/template/run.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/compliance.py` & `datatrails-archivist-0.30.0/archivist/compliance.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/compliance_policies.py` & `datatrails-archivist-0.30.0/archivist/compliance_policies.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/compliance_policy_requests.py` & `datatrails-archivist-0.30.0/archivist/compliance_policy_requests.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/compliance_policy_type.py` & `datatrails-archivist-0.30.0/archivist/compliance_policy_type.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/composite.py` & `datatrails-archivist-0.30.0/archivist/composite.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/confirmer.py` & `datatrails-archivist-0.30.0/archivist/confirmer.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,24 +11,20 @@
     # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
     from backoff._typing import Details
 
     from .assets import Asset, _AssetsPublic, _AssetsRestricted
     from .events import Event, _EventsPublic, _EventsRestricted
 
 
-from .constants import (
-    CONFIRMATION_CONFIRMED,
-    CONFIRMATION_FAILED,
-    CONFIRMATION_PENDING,
-    CONFIRMATION_STATUS,
-)
+from .confirmation_status import ConfirmationStatus
+from .constants import CONFIRMATION_STATUS
 from .errors import ArchivistUnconfirmedError
 from .utils import backoff_handler
 
-MAX_TIME = 1200
+MAX_TIME = 300
 LOGGER = getLogger(__name__)
 
 # pylint: disable=protected-access
 PublicManagers = Union["_AssetsPublic", "_EventsPublic"]
 PrivateManagers = Union["_AssetsRestricted", "_EventsRestricted"]
 Managers = Union[PublicManagers, PrivateManagers]
 ReturnTypes = Union["Asset", "Event"]
@@ -50,38 +46,43 @@
 # an event will be returned. If self is Asset client then an asset will be
 # returned. Overloads are evaluated at startup but not at runtime, therefore
 # no test coverage be done directly.
 
 
 @overload
 def _wait_for_confirmation(
-    self: "_AssetsRestricted", identity: str
+    self: "_AssetsRestricted",
+    identity: str,
 ) -> "Asset": ...  # pragma: no cover
 
 
 @overload
 def _wait_for_confirmation(
-    self: "_AssetsPublic", identity: str
+    self: "_AssetsPublic",
+    identity: str,
 ) -> "Asset": ...  # pragma: no cover
 
 
 @overload
 def _wait_for_confirmation(
-    self: "_EventsRestricted", identity: str
+    self: "_EventsRestricted",
+    identity: str,
 ) -> "Event": ...  # pragma: no cover
 
 
 @overload
 def _wait_for_confirmation(
-    self: "_EventsPublic", identity: str
+    self: "_EventsPublic",
+    identity: str,
 ) -> "Event": ...  # pragma: no cover
 
 
 @backoff.on_predicate(
     backoff.expo,
+    max_value=30.0,
     logger=None,  # pyright: ignore
     max_time=__lookup_max_time,
     on_backoff=backoff_handler,
     on_giveup=__on_giveup_confirmation,
 )
 def _wait_for_confirmation(self: Managers, identity: str) -> ReturnTypes:
     """Return None until entity is confirmed"""
@@ -90,20 +91,26 @@
 
     LOGGER.debug("entity %s", entity)
     if CONFIRMATION_STATUS not in entity:
         raise ArchivistUnconfirmedError(
             f"cannot confirm {identity} as confirmation_status is not present"
         )
 
-    if entity[CONFIRMATION_STATUS] == CONFIRMATION_FAILED:
+    status = entity[CONFIRMATION_STATUS]
+    if status == ConfirmationStatus.FAILED.name:
         raise ArchivistUnconfirmedError(
             f"confirmation for {identity} FAILED - this is unusable"
         )
 
-    if entity[CONFIRMATION_STATUS] == CONFIRMATION_CONFIRMED:
+    # Simple hash and merkleLog
+    if status in (
+        ConfirmationStatus.CONFIRMED.name,
+        ConfirmationStatus.COMMITTED.name,
+        ConfirmationStatus.UNEQUIVOCAL.name,
+    ):
         return entity
 
     return None  # pyright: ignore
 
 
 def __on_giveup_confirmed(details: "Details"):
     self: PrivateManagers = details["args"][0]
@@ -112,35 +119,46 @@
     raise ArchivistUnconfirmedError(
         f"{count} pending assets still present after {elapsed} seconds"
     )
 
 
 @backoff.on_predicate(
     backoff.expo,
+    max_value=30.0,
     logger=None,  # pyright: ignore
     max_time=__lookup_max_time,
     on_backoff=backoff_handler,
     on_giveup=__on_giveup_confirmed,
 )
 def _wait_for_confirmed(
-    self: PrivateManagers, *, props: "dict[str, Any]|None" = None, **kwargs: Any
+    self: PrivateManagers,
+    *,
+    props: "dict[str, Any]|None" = None,
+    **kwargs: Any,
 ) -> bool:
     """Return False until all entities are confirmed"""
 
-    # look for unconfirmed entities
+    # look for pending entities
+    newprops = deepcopy(props) if props else {}
+    newprops[CONFIRMATION_STATUS] = ConfirmationStatus.PENDING.name
+    LOGGER.debug("Count pending entities %s", newprops)
+    pending_count = self.count(props=newprops, **kwargs)
+
+    # look for stored entities
     newprops = deepcopy(props) if props else {}
-    newprops[CONFIRMATION_STATUS] = CONFIRMATION_PENDING
+    newprops[CONFIRMATION_STATUS] = ConfirmationStatus.STORED.name
+    LOGGER.debug("Count stored entities %s", newprops)
+    stored_count = self.count(props=newprops, **kwargs)
 
-    LOGGER.debug("Count unconfirmed entities %s", newprops)
-    count = self.count(props=newprops, **kwargs)
+    count = pending_count + stored_count
 
     if count == 0:
         # did any fail
         newprops = deepcopy(props) if props else {}
-        newprops[CONFIRMATION_STATUS] = CONFIRMATION_FAILED
+        newprops[CONFIRMATION_STATUS] = ConfirmationStatus.FAILED.name
         count = self.count(props=newprops, **kwargs)
         if count > 0:
             raise ArchivistUnconfirmedError(f"There are {count} FAILED entities")
 
         return True
 
     self.pending_count = count
```

### Comparing `datatrails-archivist-0.29.0a1/archivist/constants.py` & `datatrails-archivist-0.30.0/archivist/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 ]
 
 # define in MIME canonical form
 HEADERS_REQUEST_TOTAL_COUNT = "X-Request-Total-Count"
 HEADERS_TOTAL_COUNT = "X-Total-Count"
 HEADERS_RETRY_AFTER = "Archivist-Rate-Limit-Reset"
 
+PROOF_MECHANISM = "proof_mechanism"
+
 CONFIRMATION_STATUS = "confirmation_status"
-CONFIRMATION_PENDING = "PENDING"
-CONFIRMATION_FAILED = "FAILED"
-CONFIRMATION_CONFIRMED = "CONFIRMED"
 
 APPIDP_SUBPATH = "iam/v1"
 APPIDP_LABEL = "appidp"
 APPIDP_TOKEN = "token"
 
 APPLICATIONS_SUBPATH = "iam/v1"
 APPLICATIONS_LABEL = "applications"
```

### Comparing `datatrails-archivist-0.29.0a1/archivist/dictmerge.py` & `datatrails-archivist-0.30.0/archivist/dictmerge.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/errors.py` & `datatrails-archivist-0.30.0/archivist/errors.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/events.py` & `datatrails-archivist-0.30.0/archivist/events.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/locations.py` & `datatrails-archivist-0.30.0/archivist/locations.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/logger.py` & `datatrails-archivist-0.30.0/archivist/logger.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/parser.py` & `datatrails-archivist-0.30.0/archivist/parser.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/proof_mechanism.py` & `datatrails-archivist-0.30.0/archivist/proof_mechanism.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/retry429.py` & `datatrails-archivist-0.30.0/archivist/retry429.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/runner.py` & `datatrails-archivist-0.30.0/archivist/runner.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/sboms.py` & `datatrails-archivist-0.30.0/archivist/sboms.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/subjects.py` & `datatrails-archivist-0.30.0/archivist/subjects.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/subjects_confirmer.py` & `datatrails-archivist-0.30.0/archivist/subjects_confirmer.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from typing import TYPE_CHECKING
 
 import backoff
 
 if TYPE_CHECKING:
     from .subjects import Subject, _SubjectsClient
 
+from .confirmation_status import ConfirmationStatus
 from .constants import (
-    CONFIRMATION_CONFIRMED,
     CONFIRMATION_STATUS,
 )
 from .errors import ArchivistUnconfirmedError
 
 # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
 from .utils import backoff_handler
 
-MAX_TIME = 1200
+MAX_TIME = 300
 
 LOGGER = getLogger(__name__)
 
 
 def __lookup_max_time():
     return MAX_TIME
 
@@ -33,22 +33,23 @@
     raise ArchivistUnconfirmedError(
         f"confirmation for {identity} timed out after {elapsed} seconds"
     )
 
 
 @backoff.on_predicate(
     backoff.expo,
+    max_value=30.0,
     logger=None,  # pyright: ignore
     max_time=__lookup_max_time,
     on_backoff=backoff_handler,
     on_giveup=__on_giveup_confirmation,
 )
 def _wait_for_confirmation(self: "_SubjectsClient", identity: str) -> "Subject":
     """Return None until subjects is confirmed"""
     subject = self.read(identity)
     if CONFIRMATION_STATUS not in subject:
         return None  # pyright: ignore
 
-    if subject[CONFIRMATION_STATUS] == CONFIRMATION_CONFIRMED:
+    if subject[CONFIRMATION_STATUS] == ConfirmationStatus.CONFIRMED.name:
         return subject
 
     return None  # pyright: ignore
```

### Comparing `datatrails-archivist-0.29.0a1/archivist/tenancies.py` & `datatrails-archivist-0.30.0/archivist/tenancies.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/timestamp.py` & `datatrails-archivist-0.30.0/archivist/timestamp.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/archivist/utils.py` & `datatrails-archivist-0.30.0/archivist/utils.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/datatrails_archivist.egg-info/PKG-INFO` & `datatrails-archivist-0.30.0/datatrails_archivist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrails-archivist
-Version: 0.29.0a1
+Version: 0.30.0
 Summary: DataTrails API
 Home-page: https://github.com/datatrails/datatrails-python
 Author: DataTrails Inc.
 Author-email: support@datatrails.ai
 License: MIT
 Project-URL: Documentation, https://python.datatrails.ai
 Project-URL: Source, https://github.com/datatrails/datatrails-python
```

### Comparing `datatrails-archivist-0.29.0a1/datatrails_archivist.egg-info/SOURCES.txt` & `datatrails-archivist-0.30.0/datatrails_archivist.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 archivist/assets.py
 archivist/attachments.py
 archivist/compliance.py
 archivist/compliance_policies.py
 archivist/compliance_policy_requests.py
 archivist/compliance_policy_type.py
 archivist/composite.py
+archivist/confirmation_status.py
 archivist/confirmer.py
 archivist/constants.py
 archivist/dictmerge.py
 archivist/errors.py
 archivist/events.py
 archivist/headers.py
 archivist/locations.py
```

### Comparing `datatrails-archivist-0.29.0a1/pyproject.toml` & `datatrails-archivist-0.30.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.29.0a1/setup.cfg` & `datatrails-archivist-0.30.0/setup.cfg`

 * *Files identical despite different names*

