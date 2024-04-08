# Comparing `tmp/openstack-release-test-5.0.0.tar.gz` & `tmp/openstack-release-test-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstack-release-test-5.0.0.tar", last modified: Mon Oct  9 17:09:48 2023, max compression
+gzip compressed data, was "openstack-release-test-6.0.0.tar", last modified: Mon Apr  8 15:13:57 2024, max compression
```

## Comparing `openstack-release-test-5.0.0.tar` & `openstack-release-test-6.0.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.749589 openstack-release-test-5.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2023-10-09 17:09:48.000000 openstack-release-test-5.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      632 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2318 2023-10-09 17:09:48.000000 openstack-release-test-5.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2023-10-09 17:09:48.749589 openstack-release-test-5.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.741588 openstack-release-test-5.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.741588 openstack-release-test-5.0.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2469 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.741588 openstack-release-test-5.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1905 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/doc/source/usage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/log.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.745588 openstack-release-test-5.0.0/openstack_release_test.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2023-10-09 17:09:48.000000 openstack-release-test-5.0.0/openstack_release_test.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1639 2023-10-09 17:09:48.000000 openstack-release-test-5.0.0/openstack_release_test.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-10-09 17:09:48.000000 openstack-release-test-5.0.0/openstack_release_test.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-10-09 17:09:48.000000 openstack-release-test-5.0.0/openstack_release_test.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-10-09 17:09:48.000000 openstack-release-test-5.0.0/openstack_release_test.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-10-09 17:09:48.000000 openstack-release-test-5.0.0/openstack_release_test.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-10-09 17:09:48.000000 openstack-release-test-5.0.0/openstack_release_test.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.745588 openstack-release-test-5.0.0/release_test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/release_test/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.745588 openstack-release-test-5.0.0/release_test/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/release_test/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/release_test/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/release_test/tests/test_release_test.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.741588 openstack-release-test-5.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.745588 openstack-release-test-5.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/notes/add-reno-71dc832ce29b962f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/notes/faux-bug-1f38be77c952e9ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/notes/fix-readme-a83219eccffe7914.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/notes/launchpad-test-7d9df67df0ae43b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/notes/test-release-after-pypi-update-97153a13b68abaf7.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.745588 openstack-release-test-5.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/3.1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.745588 openstack-release-test-5.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:48.749589 openstack-release-test-5.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9124 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/meiji.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2023-10-09 17:09:48.749589 openstack-release-test-5.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1300 2023-10-09 17:09:22.000000 openstack-release-test-5.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.806307 openstack-release-test-6.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2024-04-08 15:13:57.000000 openstack-release-test-6.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      632 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2394 2024-04-08 15:13:57.000000 openstack-release-test-6.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2024-04-08 15:13:57.806307 openstack-release-test-6.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.798308 openstack-release-test-6.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.798308 openstack-release-test-6.0.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2469 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.798308 openstack-release-test-6.0.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1905 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/doc/source/usage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/log.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.798308 openstack-release-test-6.0.0/openstack_release_test.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2024-04-08 15:13:57.000000 openstack-release-test-6.0.0/openstack_release_test.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1670 2024-04-08 15:13:57.000000 openstack-release-test-6.0.0/openstack_release_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-08 15:13:57.000000 openstack-release-test-6.0.0/openstack_release_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-08 15:13:57.000000 openstack-release-test-6.0.0/openstack_release_test.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-08 15:13:57.000000 openstack-release-test-6.0.0/openstack_release_test.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-04-08 15:13:57.000000 openstack-release-test-6.0.0/openstack_release_test.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-04-08 15:13:57.000000 openstack-release-test-6.0.0/openstack_release_test.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.802307 openstack-release-test-6.0.0/release_test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/release_test/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.802307 openstack-release-test-6.0.0/release_test/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/release_test/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/release_test/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/release_test/tests/test_release_test.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.794308 openstack-release-test-6.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.802307 openstack-release-test-6.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/notes/add-reno-71dc832ce29b962f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/notes/faux-bug-1f38be77c952e9ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/notes/fix-readme-a83219eccffe7914.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/notes/launchpad-test-7d9df67df0ae43b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/notes/test-release-after-pypi-update-97153a13b68abaf7.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.806307 openstack-release-test-6.0.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/3.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.806307 openstack-release-test-6.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:13:57.806307 openstack-release-test-6.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9124 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/meiji.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2024-04-08 15:13:57.806307 openstack-release-test-6.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1300 2024-04-08 15:12:54.000000 openstack-release-test-6.0.0/tox.ini
```

### Comparing `openstack-release-test-5.0.0/AUTHORS` & `openstack-release-test-6.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/CONTRIBUTING.rst` & `openstack-release-test-6.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/ChangeLog` & `openstack-release-test-6.0.0/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+6.0.0
+-----
+
+* Update master for stable/2023.2
+
 5.0.0
 -----
 
 * Update setup.cfg with recent python versions
 
 4.1.0
 -----
@@ -12,15 +17,23 @@
 * Update master for stable/2023.1
 * Remove python-dev from bindep
 
 4.0.0
 -----
 
 * setup.cfg: Replace dashes with underscores
+
+3.9.0
+-----
+
 * remove unicode from code
+
+3.8.0
+-----
+
 * Fix formattiing of release list
 * [community goal] Update contributor documentation
 * Use py3 as the default runtime for tox
 * Add doc/requirements
 
 3.3.1
 -----
```

### Comparing `openstack-release-test-5.0.0/LICENSE` & `openstack-release-test-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/PKG-INFO` & `openstack-release-test-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: openstack-release-test
-Version: 5.0.0
+Version: 6.0.0
 Summary: Package for testing OpenStack release tools.
 Home-page: https://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==============
          release-test
```

### Comparing `openstack-release-test-5.0.0/bindep.txt` & `openstack-release-test-6.0.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/doc/source/conf.py` & `openstack-release-test-6.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/doc/source/contributor/contributing.rst` & `openstack-release-test-6.0.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/doc/source/index.rst` & `openstack-release-test-6.0.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/log.rst` & `openstack-release-test-6.0.0/log.rst`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/openstack_release_test.egg-info/PKG-INFO` & `openstack-release-test-6.0.0/openstack_release_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: openstack-release-test
-Version: 5.0.0
+Version: 6.0.0
 Summary: Package for testing OpenStack release tools.
 Home-page: https://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==============
          release-test
```

### Comparing `openstack-release-test-5.0.0/openstack_release_test.egg-info/SOURCES.txt` & `openstack-release-test-6.0.0/openstack_release_test.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 releasenotes/notes/.placeholder
 releasenotes/notes/add-reno-71dc832ce29b962f.yaml
 releasenotes/notes/faux-bug-1f38be77c952e9ec.yaml
 releasenotes/notes/fix-readme-a83219eccffe7914.yaml
 releasenotes/notes/launchpad-test-7d9df67df0ae43b4.yaml
 releasenotes/notes/test-release-after-pypi-update-97153a13b68abaf7.yaml
 releasenotes/source/2023.1.rst
+releasenotes/source/2023.2.rst
 releasenotes/source/3.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/meiji.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/pike.rst
```

### Comparing `openstack-release-test-5.0.0/release_test/__init__.py` & `openstack-release-test-6.0.0/release_test/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/release_test/tests/base.py` & `openstack-release-test-6.0.0/release_test/tests/base.py`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/release_test/tests/test_release_test.py` & `openstack-release-test-6.0.0/release_test/tests/test_release_test.py`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/releasenotes/source/conf.py` & `openstack-release-test-6.0.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/setup.cfg` & `openstack-release-test-6.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/setup.py` & `openstack-release-test-6.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `openstack-release-test-5.0.0/tox.ini` & `openstack-release-test-6.0.0/tox.ini`

 * *Files identical despite different names*

