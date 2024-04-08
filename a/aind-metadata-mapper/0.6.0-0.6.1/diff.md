# Comparing `tmp/aind-metadata-mapper-0.6.0.tar.gz` & `tmp/aind-metadata-mapper-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-metadata-mapper-0.6.0.tar", last modified: Thu Mar  7 18:52:51 2024, max compression
+gzip compressed data, was "aind-metadata-mapper-0.6.1.tar", last modified: Mon Apr  8 17:53:02 2024, max compression
```

## Comparing `aind-metadata-mapper-0.6.0.tar` & `aind-metadata-mapper-0.6.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.932927 aind-metadata-mapper-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.916927 aind-metadata-mapper-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.920927 aind-metadata-mapper-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.920927 aind-metadata-mapper-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-03-07 18:52:51.932927 aind-metadata-mapper-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.920927 aind-metadata-mapper-0.6.0/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.920927 aind-metadata-mapper-0.6.0/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.924927 aind-metadata-mapper-0.6.0/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.924927 aind-metadata-mapper-0.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/examples/bergamo_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 18:52:51.932927 aind-metadata-mapper-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.916927 aind-metadata-mapper-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.924927 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.924927 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22822 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/bergamo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.924927 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/ephys/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.924927 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/fib/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/fib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/fib/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.924927 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/mesoscope/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.928927 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-03-07 18:52:51.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-07 18:52:51.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 18:52:51.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-07 18:52:51.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-07 18:52:51.000000 aind-metadata-mapper-0.6.0/src/aind_metadata_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.928927 aind-metadata-mapper-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.920927 aind-metadata-mapper-0.6.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.928927 aind-metadata-mapper-0.6.0/tests/resources/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/bergamo/cropped_neuron50_00001.tif
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/bergamo/example_description0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/bergamo/example_metadata.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/bergamo/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.928927 aind-metadata-mapper-0.6.0/tests/resources/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/ephys/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/ephys/newscale_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/ephys/newscale_surface_finding.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/ephys/settings_main.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/ephys/settings_surface_finding.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.928927 aind-metadata-mapper-0.6.0/tests/resources/fib/
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/fib/000000_ophys_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/fib/000000_ophys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/fib/example_from_teensy.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:52:51.928927 aind-metadata-mapper-0.6.0/tests/resources/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/mesoscope/example_extract.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/mesoscope/example_platform.json
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/resources/mesoscope/expected_session.json
--rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/test_bergamo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/test_ephys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/test_fib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/test_legacy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-03-07 18:52:43.000000 aind-metadata-mapper-0.6.0/tests/test_mesoscope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.326105 aind-metadata-mapper-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.314105 aind-metadata-mapper-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-08 17:53:02.326105 aind-metadata-mapper-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/examples/bergamo_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:53:02.326105 aind-metadata-mapper-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.314105 aind-metadata-mapper-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 17:52:51.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/bergamo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/ephys/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/fib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/fib/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/mesoscope/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.326105 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-08 17:53:02.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-08 17:53:02.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:53:02.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 17:53:02.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 17:53:02.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.314105 aind-metadata-mapper-0.6.1/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/tests/resources/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/bergamo/cropped_neuron50_00001.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/bergamo/example_description0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/bergamo/example_metadata.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/bergamo/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/tests/resources/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/ephys/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/ephys/newscale_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/ephys/newscale_surface_finding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/ephys/settings_main.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/ephys/settings_surface_finding.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/tests/resources/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/fib/000000_ophys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/fib/000000_ophys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/fib/example_from_teensy.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.326105 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/example_extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/example_platform.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/expected_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/test_bergamo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/test_ephys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/test_fib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/test_legacy_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/test_mesoscope.py
```

### Comparing `aind-metadata-mapper-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/.github/ISSUE_TEMPLATE/user-story.md` & `aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/.github/workflows/tag_and_publish.yml` & `aind-metadata-mapper-0.6.1/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/.github/workflows/test_and_lint.yml` & `aind-metadata-mapper-0.6.1/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/.gitignore` & `aind-metadata-mapper-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/LICENSE` & `aind-metadata-mapper-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/PKG-INFO` & `aind-metadata-mapper-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.6.0
+Version: 0.6.1
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aind-data-schema==0.26.5
+Requires-Dist: aind-data-schema==0.33.3
 Requires-Dist: scanimage-tiff-reader==1.4.1.4
 Requires-Dist: tifffile==2024.2.12
 Requires-Dist: pydantic-settings>=2.0
 Requires-Dist: pillow
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
```

### Comparing `aind-metadata-mapper-0.6.0/README.md` & `aind-metadata-mapper-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/doc_template/Makefile` & `aind-metadata-mapper-0.6.1/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/doc_template/make.bat` & `aind-metadata-mapper-0.6.1/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/doc_template/source/_static/dark-logo.svg` & `aind-metadata-mapper-0.6.1/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/doc_template/source/_static/favicon.ico` & `aind-metadata-mapper-0.6.1/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/doc_template/source/_static/light-logo.svg` & `aind-metadata-mapper-0.6.1/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/doc_template/source/conf.py` & `aind-metadata-mapper-0.6.1/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/examples/bergamo_session.py` & `aind-metadata-mapper-0.6.1/examples/bergamo_session.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/pyproject.toml` & `aind-metadata-mapper-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 readme = "README.md"
 dynamic = ["version"]
 
 dependencies = [
-    "aind-data-schema==0.26.5",
+    "aind-data-schema==0.33.3",
     "scanimage-tiff-reader==1.4.1.4",
     "tifffile==2024.2.12",
     "pydantic-settings>=2.0",
     "pillow"
 ]
 
 [project.optional-dependencies]
```

### Comparing `aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/bergamo/session.py` & `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/bergamo/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 import numpy as np
 from aind_data_schema.core.session import (
     DetectorConfig,
     FieldOfView,
     LaserConfig,
     Modality,
     Session,
+    StimulusEpoch,
+    StimulusModality,
     Stream,
 )
 from aind_data_schema.models.stimulus import (
     PhotoStimulation,
     PhotoStimulationGroup,
-    StimulusEpoch,
 )
 from aind_data_schema.models.units import PowerUnit, SizeUnit
 from pydantic import Field
 from pydantic_settings import BaseSettings
 from ScanImageTiffReader import ScanImageTiffReader
 
 from aind_metadata_mapper.core import GenericEtl, JobResponse
@@ -397,16 +398,14 @@
         """
         siHeader = self._parse_raw_image_info(extracted_source)
         photostim_groups = siHeader.metadata["json"]["RoiGroups"][
             "photostimRoiGroups"
         ]
 
         data_stream = Stream(
-            mouse_platform_name=self.job_settings.mouse_platform_name,
-            active_mouse_platform=self.job_settings.active_mouse_platform,
             stream_start_time=self.job_settings.stream_start_time,
             stream_end_time=self.job_settings.stream_end_time,
             stream_modalities=[Modality.POPHYS],
             camera_names=list(self.job_settings.camera_names),
             light_sources=[
                 LaserConfig(
                     name=self.job_settings.laser_a_name,
@@ -447,112 +446,120 @@
                     ),
                     frame_rate=float(
                         siHeader.metadata["hRoiManager"]["scanFrameRate"]
                     ),
                 ),
             ],
         )
+        stimulus_name = "PhotoStimulation"
+        photostim_interval = self.job_settings.photo_stim_inter_trial_interval
         return Session(
             experimenter_full_name=self.job_settings.experimenter_full_name,
             session_start_time=self.job_settings.session_start_time,
             session_end_time=self.job_settings.session_end_time,
             subject_id=self.job_settings.subject_id,
             session_type=self.job_settings.session_type,
             iacuc_protocol=self.job_settings.iacuc_protocol,
             rig_id=self.job_settings.rig_id,
             data_streams=[data_stream],
             stimulus_epochs=[
                 StimulusEpoch(
-                    stimulus=PhotoStimulation(
-                        stimulus_name="PhotoStimulation",
-                        number_groups=(
-                            self.job_settings.num_of_photo_stim_groups
-                        ),
-                        groups=[
-                            PhotoStimulationGroup(
-                                group_index=(
-                                    self.job_settings.photo_stim_groups[0][
-                                        "group_index"
-                                    ]
-                                ),
-                                number_of_neurons=int(
-                                    np.array(
+                    stimulus_name=stimulus_name,
+                    stimulus_modalities=[
+                        StimulusModality.OPTOGENETICS,
+                    ],
+                    stimulus_parameters=[
+                        PhotoStimulation(
+                            stimulus_name="PhotoStimulation",
+                            number_groups=(
+                                self.job_settings.num_of_photo_stim_groups
+                            ),
+                            groups=[
+                                PhotoStimulationGroup(
+                                    group_index=(
+                                        self.job_settings.photo_stim_groups[0][
+                                            "group_index"
+                                        ]
+                                    ),
+                                    number_of_neurons=int(
+                                        np.array(
+                                            photostim_groups[0]["rois"][1][
+                                                "scanfields"
+                                            ]["slmPattern"]
+                                        ).shape[0]
+                                    ),
+                                    stimulation_laser_power=int(
                                         photostim_groups[0]["rois"][1][
                                             "scanfields"
-                                        ]["slmPattern"]
-                                    ).shape[0]
-                                ),
-                                stimulation_laser_power=int(
-                                    photostim_groups[0]["rois"][1][
-                                        "scanfields"
-                                    ]["powers"]
-                                ),
-                                number_trials=(
-                                    self.job_settings.photo_stim_groups[0][
-                                        "number_trials"
-                                    ]
-                                ),
-                                number_spirals=int(
-                                    photostim_groups[0]["rois"][1][
-                                        "scanfields"
-                                    ]["repetitions"]
-                                ),
-                                spiral_duration=photostim_groups[0]["rois"][1][
-                                    "scanfields"
-                                ]["duration"],
-                                inter_spiral_interval=photostim_groups[0][
-                                    "rois"
-                                ][2]["scanfields"]["duration"],
-                            ),
-                            PhotoStimulationGroup(
-                                group_index=(
-                                    self.job_settings.photo_stim_groups[1][
-                                        "group_index"
-                                    ]
-                                ),
-                                number_of_neurons=int(
-                                    np.array(
+                                        ]["powers"]
+                                    ),
+                                    number_trials=(
+                                        self.job_settings.photo_stim_groups[0][
+                                            "number_trials"
+                                        ]
+                                    ),
+                                    number_spirals=int(
                                         photostim_groups[0]["rois"][1][
                                             "scanfields"
-                                        ]["slmPattern"]
-                                    ).shape[0]
-                                ),
-                                stimulation_laser_power=int(
-                                    photostim_groups[0]["rois"][1][
-                                        "scanfields"
-                                    ]["powers"]
-                                ),
-                                number_trials=(
-                                    self.job_settings.photo_stim_groups[1][
-                                        "number_trials"
-                                    ]
+                                        ]["repetitions"]
+                                    ),
+                                    spiral_duration=photostim_groups[0][
+                                        "rois"
+                                    ][1]["scanfields"]["duration"],
+                                    inter_spiral_interval=photostim_groups[0][
+                                        "rois"
+                                    ][2]["scanfields"]["duration"],
                                 ),
-                                number_spirals=int(
-                                    photostim_groups[0]["rois"][1][
-                                        "scanfields"
-                                    ]["repetitions"]
+                                PhotoStimulationGroup(
+                                    group_index=(
+                                        self.job_settings.photo_stim_groups[1][
+                                            "group_index"
+                                        ]
+                                    ),
+                                    number_of_neurons=int(
+                                        np.array(
+                                            photostim_groups[0]["rois"][1][
+                                                "scanfields"
+                                            ]["slmPattern"]
+                                        ).shape[0]
+                                    ),
+                                    stimulation_laser_power=int(
+                                        photostim_groups[0]["rois"][1][
+                                            "scanfields"
+                                        ]["powers"]
+                                    ),
+                                    number_trials=(
+                                        self.job_settings.photo_stim_groups[1][
+                                            "number_trials"
+                                        ]
+                                    ),
+                                    number_spirals=int(
+                                        photostim_groups[0]["rois"][1][
+                                            "scanfields"
+                                        ]["repetitions"]
+                                    ),
+                                    spiral_duration=photostim_groups[0][
+                                        "rois"
+                                    ][1]["scanfields"]["duration"],
+                                    inter_spiral_interval=photostim_groups[0][
+                                        "rois"
+                                    ][2]["scanfields"]["duration"],
                                 ),
-                                spiral_duration=photostim_groups[0]["rois"][1][
-                                    "scanfields"
-                                ]["duration"],
-                                inter_spiral_interval=photostim_groups[0][
-                                    "rois"
-                                ][2]["scanfields"]["duration"],
-                            ),
-                        ],
-                        inter_trial_interval=(
-                            self.job_settings.photo_stim_inter_trial_interval
-                        ),
-                    ),
+                            ],
+                            inter_trial_interval=(photostim_interval),
+                        )
+                    ],
                     stimulus_start_time=(
                         self.job_settings.stimulus_start_time
                     ),
                     stimulus_end_time=self.job_settings.stimulus_end_time,
                 )
             ],
+            mouse_platform_name=self.job_settings.mouse_platform_name,
+            active_mouse_platform=self.job_settings.active_mouse_platform,
         )
 
     def run_job(self) -> JobResponse:
         """Run the etl job and return a JobResponse."""
         extracted = self._extract()
         transformed = self._transform(extracted_source=extracted)
         job_response = self._load(
```

### Comparing `aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/core.py` & `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/core.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/ephys/session.py` & `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/ephys/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,20 +102,14 @@
             session_stream = {}
             session_stream["stream_start_time"] = datetime.strptime(
                 stage[0][0], "%Y/%m/%d %H:%M:%S.%f"
             )
             session_stream["stream_end_time"] = datetime.strptime(
                 stage[-1][0], "%Y/%m/%d %H:%M:%S.%f"
             )
-            session_stream["mouse_platform_name"] = data_stream[
-                "mouse_platform_name"
-            ]
-            session_stream["active_mouse_platform"] = data_stream[
-                "active_mouse_platform"
-            ]
             session_stream["stream_modalities"] = [Modality.ECEPHYS]
             session_stream["stick_microscopes"] = stick_microscopes
             session_stream["camera_names"] = camera_names
             session_stream["daq_names"] = [daqs]
             session_stream["ephys_modules"] = []
             stage_info = [
                 x for i, x in enumerate(stage) if x[1] != stage[i - 1][1]
@@ -130,14 +124,21 @@
                 }
                 ephys_module["ephys_probes"] = [{"name": probe}]
 
                 session_stream["ephys_modules"].append(ephys_module)
 
             ephys_session["data_streams"].append(session_stream)
 
+        ephys_session["mouse_platform_name"] = data_stream[
+            "mouse_platform_name"
+        ]
+        ephys_session["active_mouse_platform"] = data_stream[
+            "active_mouse_platform"
+        ]
+
         end_times = [
             datetime.strptime(x[-1][0], "%Y/%m/%d %H:%M:%S.%f")
             for x in stage_logs
         ]
         ephys_session["session_end_time"] = max(end_times)
         return Session(**ephys_session)
```

### Comparing `aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/fib/session.py` & `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/fib/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,20 @@
 from typing import List, Optional, Union
 
 from aind_data_schema.core.session import (
     DetectorConfig,
     FiberConnectionConfig,
     LightEmittingDiodeConfig,
     Session,
+    StimulusEpoch,
+    StimulusModality,
     Stream,
 )
 from aind_data_schema.models.modalities import Modality
-from aind_data_schema.models.stimulus import (
-    OptoStimulation,
-    PulseShape,
-    StimulusEpoch,
-)
+from aind_data_schema.models.stimulus import OptoStimulation, PulseShape
 from pydantic import Field
 from pydantic_settings import BaseSettings
 
 from aind_metadata_mapper.core import GenericEtl, JobResponse
 
 
 class JobSettings(BaseSettings):
@@ -144,32 +142,44 @@
         command = command_match.group(1)
         stimulus_name = self._dictionary_mapping.get(command, "")
 
         # create opto stim instance
         opto_stim = OptoStimulation(
             stimulus_name=stimulus_name,
             pulse_shape=PulseShape.SQUARE,
-            pulse_frequency=frequency,
-            number_pulse_trains=trial_num,
-            pulse_width=pulse_width,
-            pulse_train_duration=opto_duration,
+            pulse_frequency=[
+                frequency,
+            ],
+            number_pulse_trains=[
+                trial_num,
+            ],
+            pulse_width=[
+                pulse_width,
+            ],
+            pulse_train_duration=[
+                opto_duration,
+            ],
             pulse_train_interval=opto_interval,
             baseline_duration=opto_base,
             fixed_pulse_train_interval=True,  # TODO: Check this is right
         )
 
         # create stimulus presentation instance
         experiment_duration = (
             opto_base + opto_duration + (opto_interval * trial_num)
         )
         end_datetime = session_start_time + timedelta(
             seconds=experiment_duration
         )
         stimulus_epochs = StimulusEpoch(
-            stimulus=opto_stim,
+            stimulus_name=stimulus_name,
+            stimulus_modalities=[StimulusModality.OPTOGENETICS],
+            stimulus_parameters=[
+                opto_stim,
+            ],
             stimulus_start_time=session_start_time,
             stimulus_end_time=end_datetime,
         )
 
         # create light source instance
         light_source = []
         for ls in light_source_list:
@@ -189,16 +199,14 @@
             fiber_connections.append(cord)
         data_stream = [
             Stream(
                 stream_start_time=session_start_time,
                 stream_end_time=end_datetime,
                 light_sources=light_source,
                 stream_modalities=[Modality.FIB],
-                mouse_platform_name=mouse_platform_name,
-                active_mouse_platform=active_mouse_platform,
                 detectors=detectors,
                 fiber_connections=fiber_connections,
             )
         ]
         # and finally, create ophys session
         ophys_session = Session(
             stimulus_epochs=[stimulus_epochs],
@@ -207,14 +215,16 @@
             session_start_time=session_start_time,
             session_end_time=end_datetime,
             rig_id=rig_id,
             experimenter_full_name=experimenter_full_name,
             session_type=session_type,
             notes=notes,
             data_streams=data_stream,
+            mouse_platform_name=mouse_platform_name,
+            active_mouse_platform=active_mouse_platform,
         )
 
         return ophys_session
 
     def _extract(self) -> ParsedMetadata:
         """Extract metadata from fib session."""
```

### Comparing `aind-metadata-mapper-0.6.0/src/aind_metadata_mapper/mesoscope/session.py` & `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/mesoscope/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Mesoscope ETL"""
+
 import argparse
 import json
 import sys
 from datetime import datetime
 from pathlib import Path
 from typing import List, Union
 
@@ -95,15 +96,16 @@
         """
         # The pydantic models will validate that the user inputs a Path.
         # We can add validators there if we want to coerce strings to Paths.
         input_source = self.job_settings.input_source
         behavior_source = self.job_settings.behavior_source
         session_metadata = {}
         if behavior_source.is_dir():
-            for ftype in behavior_source.glob("*json"):
+            # deterministic order
+            for ftype in sorted(list(behavior_source.glob("*json"))):
                 if (
                     "Behavior" in ftype.stem
                     or "Eye" in ftype.stem
                     or "Face" in ftype.stem
                 ):
                     with open(ftype, "r") as f:
                         session_metadata[ftype.stem] = json.load(f)
@@ -163,16 +165,14 @@
                 fovs.append(fov)
         data_streams.append(
             Stream(
                 camera_names=["Mesoscope"],
                 stream_start_time=self.job_settings.session_start_time,
                 stream_end_time=self.job_settings.session_end_time,
                 ophys_fovs=fovs,
-                mouse_platform_name=self.job_settings.mouse_platform_name,
-                active_mouse_platform=True,
                 stream_modalities=[Modality.POPHYS],
             )
         )
         for camera in extracted_source.keys():
             if camera != "platform":
                 start_time = datetime.strptime(
                     extracted_source[camera]["RecordingReport"]["TimeStart"],
@@ -184,18 +184,14 @@
                 )
                 camera_name = camera.split("_")[1]
                 data_streams.append(
                     Stream(
                         camera_names=[camera_name],
                         stream_start_time=start_time,
                         stream_end_time=end_time,
-                        mouse_platform_name=(
-                            self.job_settings.mouse_platform_name
-                        ),
-                        active_mouse_platform=True,
                         stream_modalities=[Modality.BEHAVIOR_VIDEOS],
                     )
                 )
         vasculature_fp = next(
             self.job_settings.input_source.glob("*vasculature*.tif"), ""
         )
         # Pull datetime from vasculature.
@@ -212,30 +208,30 @@
             vasculature_dt[0], "%Y:%m:%d %H:%M:%S"
         )
         data_streams.append(
             Stream(
                 camera_names=["Vasculature"],
                 stream_start_time=vasculature_dt,
                 stream_end_time=vasculature_dt,
-                mouse_platform_name=self.job_settings.mouse_platform_name,
-                active_mouse_platform=True,
                 stream_modalities=[
                     Modality.CONFOCAL
                 ],  # TODO: ask Saskia about this
             )
         )
         return Session(
             experimenter_full_name=self.job_settings.experimenter_full_name,
             session_type="Mesoscope",
             subject_id=self.job_settings.subject_id,
             iacuc_protocol=self.job_settings.iacuc_protocol,
             session_start_time=self.job_settings.session_start_time,
             session_end_time=self.job_settings.session_end_time,
             rig_id=extracted_source["platform"]["rig_id"],
             data_streams=data_streams,
+            mouse_platform_name=self.job_settings.mouse_platform_name,
+            active_mouse_platform=True,
         )
 
     def run_job(self) -> None:
         """
         Run the etl job
         Returns
         -------
```

### Comparing `aind-metadata-mapper-0.6.0/src/aind_metadata_mapper.egg-info/PKG-INFO` & `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.6.0
+Version: 0.6.1
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aind-data-schema==0.26.5
+Requires-Dist: aind-data-schema==0.33.3
 Requires-Dist: scanimage-tiff-reader==1.4.1.4
 Requires-Dist: tifffile==2024.2.12
 Requires-Dist: pydantic-settings>=2.0
 Requires-Dist: pillow
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
```

### Comparing `aind-metadata-mapper-0.6.0/src/aind_metadata_mapper.egg-info/SOURCES.txt` & `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/bergamo/cropped_neuron50_00001.tif` & `aind-metadata-mapper-0.6.1/tests/resources/bergamo/cropped_neuron50_00001.tif`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/bergamo/example_description0.txt` & `aind-metadata-mapper-0.6.1/tests/resources/bergamo/example_description0.txt`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/bergamo/example_metadata.txt.gz` & `aind-metadata-mapper-0.6.1/tests/resources/bergamo/example_metadata.txt.gz`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/bergamo/expected_session.json` & `aind-metadata-mapper-0.6.1/tests/resources/bergamo/expected_session.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8225052233608596%*

 * *Differences: {"'active_mouse_platform'": 'True',*

 * * "'data_streams'": "{0: {'stream_start_time': '2023-10-10T15:00:00Z', 'stream_end_time': "*

 * *                   "'2023-10-10T16:00:00Z', 'ophys_fovs': {0: {'power': None, 'power_unit': "*

 * *                   "'percent', 'scanfield_z': None, 'scanfield_z_unit': 'micrometer', "*

 * *                   "'scanimage_roi_index': None, 'notes': None}}, delete: "*

 * *                   "['stimulus_device_names', 'mouse_platform_name', 'active_mouse_platform']}}",*

 * * "'mouse_platform_name'": "'s […]*

```diff
@@ -1,14 +1,14 @@
 {
+    "active_mouse_platform": true,
     "animal_weight_post": null,
     "animal_weight_prior": null,
     "calibrations": [],
     "data_streams": [
         {
-            "active_mouse_platform": true,
             "camera_names": [
                 "Side Camera"
             ],
             "daq_names": [],
             "detectors": [
                 {
                     "exposure_time": "0.1",
@@ -27,15 +27,14 @@
                     "excitation_power_unit": "percent",
                     "name": "Laser A",
                     "wavelength": 920,
                     "wavelength_unit": "nanometer"
                 }
             ],
             "manipulator_modules": [],
-            "mouse_platform_name": "some_mouse_platform_name",
             "notes": null,
             "ophys_fovs": [
                 {
                     "coupled_fov_index": null,
                     "fov_coordinate_ap": "1.5",
                     "fov_coordinate_ml": "1.5",
                     "fov_coordinate_unit": "micrometer",
@@ -47,89 +46,114 @@
                     "fov_width": 512,
                     "frame_rate": "30.0119",
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 150,
                     "imaging_depth_unit": "micrometer",
                     "index": 0,
                     "magnification": "16x",
+                    "notes": null,
+                    "power": null,
+                    "power_unit": "percent",
+                    "scanfield_z": null,
+                    "scanfield_z_unit": "micrometer",
+                    "scanimage_roi_index": null,
                     "targeted_structure": "M1"
                 }
             ],
             "slap_fovs": null,
             "stack_parameters": null,
             "stick_microscopes": [],
-            "stimulus_device_names": [],
-            "stream_end_time": "2023-10-10T16:00:00",
+            "stream_end_time": "2023-10-10T16:00:00Z",
             "stream_modalities": [
                 {
                     "abbreviation": "ophys",
                     "name": "Planar optical physiology"
                 }
             ],
-            "stream_start_time": "2023-10-10T15:00:00"
+            "stream_start_time": "2023-10-10T15:00:00Z"
         }
     ],
     "describedBy": "https://raw.githubusercontent.com/AllenNeuralDynamics/aind-data-schema/main/src/aind_data_schema/core/session.py",
     "experimenter_full_name": [
         "John Smith",
         "Jane Smith"
     ],
     "iacuc_protocol": "2115",
     "maintenance": [],
+    "mouse_platform_name": "some_mouse_platform_name",
     "notes": null,
     "protocol_id": [],
     "reward_consumed_total": null,
     "reward_consumed_unit": "microliter",
     "reward_delivery": null,
     "rig_id": "Bergamo photostim.",
-    "schema_version": "0.1.4",
-    "session_end_time": "2023-10-10T17:00:00",
-    "session_start_time": "2023-10-10T14:00:00",
+    "schema_version": "0.2.1",
+    "session_end_time": "2023-10-10T17:00:00Z",
+    "session_start_time": "2023-10-10T14:00:00Z",
     "session_type": "BCI",
     "stimulus_epochs": [
         {
-            "stimulus": {
-                "groups": [
-                    {
-                        "group_index": 0,
-                        "inter_spiral_interval": "0.001",
-                        "inter_spiral_interval_unit": "second",
-                        "notes": null,
-                        "number_of_neurons": 10,
-                        "number_spirals": 10,
-                        "number_trials": 5,
-                        "other_parameters": {},
-                        "spiral_duration": "0.01",
-                        "spiral_duration_unit": "second",
-                        "stimulation_laser_power": "20",
-                        "stimulation_laser_power_unit": "milliwatt"
-                    },
-                    {
-                        "group_index": 0,
-                        "inter_spiral_interval": "0.001",
-                        "inter_spiral_interval_unit": "second",
-                        "notes": null,
-                        "number_of_neurons": 10,
-                        "number_spirals": 10,
-                        "number_trials": 5,
-                        "other_parameters": {},
-                        "spiral_duration": "0.01",
-                        "spiral_duration_unit": "second",
-                        "stimulation_laser_power": "20",
-                        "stimulation_laser_power_unit": "milliwatt"
-                    }
-                ],
-                "inter_trial_interval": "10",
-                "inter_trial_interval_unit": "second",
-                "notes": null,
-                "number_groups": 2,
-                "other_parameters": {},
-                "stimulus_name": "PhotoStimulation",
-                "stimulus_type": "Photo Stimulation"
-            },
-            "stimulus_end_time": "2023-10-10T15:45:00",
-            "stimulus_start_time": "2023-10-10T15:15:00"
+            "light_source_config": null,
+            "notes": null,
+            "output_parameters": {},
+            "reward_consumed_during_epoch": null,
+            "reward_consumed_unit": "microliter",
+            "script": null,
+            "session_number": null,
+            "software": [],
+            "speaker_config": null,
+            "stimulus_device_names": [],
+            "stimulus_end_time": "2023-10-10T15:45:00Z",
+            "stimulus_modalities": [
+                "Optogenetics"
+            ],
+            "stimulus_name": "PhotoStimulation",
+            "stimulus_parameters": [
+                {
+                    "groups": [
+                        {
+                            "group_index": 0,
+                            "inter_spiral_interval": "0.001",
+                            "inter_spiral_interval_unit": "second",
+                            "notes": null,
+                            "number_of_neurons": 10,
+                            "number_spirals": 10,
+                            "number_trials": 5,
+                            "other_parameters": {},
+                            "spiral_duration": "0.01",
+                            "spiral_duration_unit": "second",
+                            "stimulation_laser_power": "20",
+                            "stimulation_laser_power_unit": "milliwatt"
+                        },
+                        {
+                            "group_index": 0,
+                            "inter_spiral_interval": "0.001",
+                            "inter_spiral_interval_unit": "second",
+                            "notes": null,
+                            "number_of_neurons": 10,
+                            "number_spirals": 10,
+                            "number_trials": 5,
+                            "other_parameters": {},
+                            "spiral_duration": "0.01",
+                            "spiral_duration_unit": "second",
+                            "stimulation_laser_power": "20",
+                            "stimulation_laser_power_unit": "milliwatt"
+                        }
+                    ],
+                    "inter_trial_interval": "10",
+                    "inter_trial_interval_unit": "second",
+                    "notes": null,
+                    "number_groups": 2,
+                    "other_parameters": {},
+                    "stimulus_name": "PhotoStimulation",
+                    "stimulus_type": "Photo Stimulation"
+                }
+            ],
+            "stimulus_start_time": "2023-10-10T15:15:00Z",
+            "trials_finished": null,
+            "trials_rewarded": null,
+            "trials_total": null
         }
     ],
     "subject_id": "12345",
     "weight_unit": "gram"
 }
```

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/ephys/ephys_session.json` & `aind-metadata-mapper-0.6.1/tests/resources/ephys/ephys_session.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7997271607111422%*

 * *Differences: {"'active_mouse_platform'": 'False',*

 * * "'data_streams'": "{0: {'stream_start_time': '2023-04-04T10:37:28.815000Z', 'stream_end_time': "*

 * *                   "'2023-04-06T11:47:57.558000Z', 'ephys_modules': {0: {'implant_hole_number': "*

 * *                   "None}, 1: {'implant_hole_number': None}}, delete: ['stimulus_device_names', "*

 * *                   "'mouse_platform_name', 'active_mouse_platform']}, 1: {'stream_start_time': "*

 * *                   "'2023-04-04T12:37:28.815000Z', 'stream_end_time': "*

 * *             […]*

```diff
@@ -1,14 +1,14 @@
 {
+    "active_mouse_platform": false,
     "animal_weight_post": null,
     "animal_weight_prior": null,
     "calibrations": [],
     "data_streams": [
         {
-            "active_mouse_platform": false,
             "camera_names": [],
             "daq_names": [
                 "Basestation"
             ],
             "detectors": [],
             "ephys_modules": [
                 {
@@ -19,14 +19,15 @@
                     "coordinate_transform": "behavior/calibration_info_np2_2024_01_17T15_04_00.npy",
                     "ephys_probes": [
                         {
                             "name": "46121",
                             "other_targeted_structures": []
                         }
                     ],
+                    "implant_hole_number": null,
                     "manipulator_coordinates": {
                         "unit": "micrometer",
                         "x": "7520.0",
                         "y": "7505.0",
                         "z": "7493.0"
                     },
                     "module_angle": "-27.1",
@@ -51,14 +52,15 @@
                     "coordinate_transform": "behavior/calibration_info_np2_2024_01_17T15_04_00.npy",
                     "ephys_probes": [
                         {
                             "name": "46118",
                             "other_targeted_structures": []
                         }
                     ],
+                    "implant_hole_number": null,
                     "manipulator_coordinates": {
                         "unit": "micrometer",
                         "x": "7500.0",
                         "y": "7499.5",
                         "z": "7600.0"
                     },
                     "module_angle": "20",
@@ -76,15 +78,14 @@
                     ]
                 }
             ],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
-            "mouse_platform_name": "Running Wheel",
             "notes": null,
             "ophys_fovs": [],
             "slap_fovs": null,
             "stack_parameters": null,
             "stick_microscopes": [
                 {
                     "angle_unit": "degrees",
@@ -123,26 +124,24 @@
                     "calibration_date": null,
                     "coordinate_transform": null,
                     "module_angle": "-180.0",
                     "notes": "Did not record arc or module angles, did not calibrate",
                     "rotation_angle": null
                 }
             ],
-            "stimulus_device_names": [],
-            "stream_end_time": "2023-04-06T11:47:57.558000",
+            "stream_end_time": "2023-04-06T11:47:57.558000Z",
             "stream_modalities": [
                 {
                     "abbreviation": "ecephys",
                     "name": "Extracellular electrophysiology"
                 }
             ],
-            "stream_start_time": "2023-04-04T10:37:28.815000"
+            "stream_start_time": "2023-04-04T10:37:28.815000Z"
         },
         {
-            "active_mouse_platform": false,
             "camera_names": [],
             "daq_names": [
                 "Basestation"
             ],
             "detectors": [],
             "ephys_modules": [
                 {
@@ -153,14 +152,15 @@
                     "coordinate_transform": "behavior/calibration_info_np2_2024_01_17T15_04_00.npy",
                     "ephys_probes": [
                         {
                             "name": "46121",
                             "other_targeted_structures": []
                         }
                     ],
+                    "implant_hole_number": null,
                     "manipulator_coordinates": {
                         "unit": "micrometer",
                         "x": "7520.0",
                         "y": "7505.0",
                         "z": "7493.0"
                     },
                     "module_angle": "-27.1",
@@ -185,14 +185,15 @@
                     "coordinate_transform": "behavior/calibration_info_np2_2024_01_17T15_04_00.npy",
                     "ephys_probes": [
                         {
                             "name": "46118",
                             "other_targeted_structures": []
                         }
                     ],
+                    "implant_hole_number": null,
                     "manipulator_coordinates": {
                         "unit": "micrometer",
                         "x": "7500.0",
                         "y": "7499.5",
                         "z": "7600.0"
                     },
                     "module_angle": "20",
@@ -210,15 +211,14 @@
                     ]
                 }
             ],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
-            "mouse_platform_name": "Running Wheel",
             "notes": null,
             "ophys_fovs": [],
             "slap_fovs": null,
             "stack_parameters": null,
             "stick_microscopes": [
                 {
                     "angle_unit": "degrees",
@@ -257,37 +257,38 @@
                     "calibration_date": null,
                     "coordinate_transform": null,
                     "module_angle": "-180.0",
                     "notes": "Did not record arc or module angles, did not calibrate",
                     "rotation_angle": null
                 }
             ],
-            "stimulus_device_names": [],
-            "stream_end_time": "2023-04-06T13:47:57.558000",
+            "stream_end_time": "2023-04-06T13:47:57.558000Z",
             "stream_modalities": [
                 {
                     "abbreviation": "ecephys",
                     "name": "Extracellular electrophysiology"
                 }
             ],
-            "stream_start_time": "2023-04-04T12:37:28.815000"
+            "stream_start_time": "2023-04-04T12:37:28.815000Z"
         }
     ],
     "describedBy": "https://raw.githubusercontent.com/AllenNeuralDynamics/aind-data-schema/main/src/aind_data_schema/core/session.py",
     "experimenter_full_name": [
         "Al Dente"
     ],
     "iacuc_protocol": "2109",
     "maintenance": [],
+    "mouse_platform_name": "Running Wheel",
     "notes": null,
+    "protocol_id": [],
     "reward_consumed_total": null,
     "reward_consumed_unit": "microliter",
     "reward_delivery": null,
     "rig_id": "323_EPHYS2-RF_2024-01-18_01",
-    "schema_version": "0.1.4",
-    "session_end_time": "2023-04-06T13:47:57.558000",
-    "session_start_time": "2023-04-04T10:37:28",
+    "schema_version": "0.2.1",
+    "session_end_time": "2023-04-06T13:47:57.558000Z",
+    "session_start_time": "2023-04-04T10:37:28Z",
     "session_type": "Receptive field mapping",
     "stimulus_epochs": [],
     "subject_id": "699889",
     "weight_unit": "gram"
 }
```

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/ephys/newscale_main.csv` & `aind-metadata-mapper-0.6.1/tests/resources/ephys/newscale_main.csv`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/ephys/newscale_surface_finding.csv` & `aind-metadata-mapper-0.6.1/tests/resources/ephys/newscale_surface_finding.csv`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/ephys/settings_main.xml` & `aind-metadata-mapper-0.6.1/tests/resources/ephys/settings_main.xml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/ephys/settings_surface_finding.xml` & `aind-metadata-mapper-0.6.1/tests/resources/ephys/settings_surface_finding.xml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/fib/000000_ophys_rig.json` & `aind-metadata-mapper-0.6.1/tests/resources/fib/000000_ophys_rig.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/fib/000000_ophys_session.json` & `aind-metadata-mapper-0.6.1/tests/resources/fib/000000_ophys_session.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.822654462242563%*

 * *Differences: {"'active_mouse_platform'": 'False',*

 * * "'data_streams'": "{0: {'stream_start_time': '1999-10-04T00:00:00Z', 'stream_end_time': "*

 * *                   "'1999-10-04T00:00:48Z', delete: ['stimulus_device_names', "*

 * *                   "'mouse_platform_name', 'active_mouse_platform']}}",*

 * * "'mouse_platform_name'": "'Disc'",*

 * * "'schema_version'": "'0.2.1'",*

 * * "'session_end_time'": "'1999-10-04T00:00:48Z'",*

 * * "'session_start_time'": "'1999-10-04T00:00:00Z'",*

 * * "'stimulus_epochs'": "{0: {'stimulus_start_time': '1999-10-04T0 […]*

```diff
@@ -1,14 +1,14 @@
 {
+    "active_mouse_platform": false,
     "animal_weight_post": null,
     "animal_weight_prior": null,
     "calibrations": [],
     "data_streams": [
         {
-            "active_mouse_platform": false,
             "camera_names": [],
             "daq_names": [],
             "detectors": [
                 {
                     "exposure_time": "10",
                     "exposure_time_unit": "millisecond",
                     "name": "Hamamatsu Camera",
@@ -42,68 +42,94 @@
                     "device_type": "LightEmittingDiode",
                     "excitation_power": "0.02",
                     "excitation_power_unit": "milliwatt",
                     "name": "565nm LED"
                 }
             ],
             "manipulator_modules": [],
-            "mouse_platform_name": "Disc",
             "notes": null,
             "ophys_fovs": [],
             "slap_fovs": null,
             "stack_parameters": null,
             "stick_microscopes": [],
-            "stimulus_device_names": [],
-            "stream_end_time": "1999-10-04T00:00:48",
+            "stream_end_time": "1999-10-04T00:00:48Z",
             "stream_modalities": [
                 {
                     "abbreviation": "fib",
                     "name": "Fiber photometry"
                 }
             ],
-            "stream_start_time": "1999-10-04T00:00:00"
+            "stream_start_time": "1999-10-04T00:00:00Z"
         }
     ],
     "describedBy": "https://raw.githubusercontent.com/AllenNeuralDynamics/aind-data-schema/main/src/aind_data_schema/core/session.py",
     "experimenter_full_name": [
         "Don Key"
     ],
     "iacuc_protocol": "2115",
     "maintenance": [],
+    "mouse_platform_name": "Disc",
     "notes": "brabrabrabra....",
     "protocol_id": [],
     "reward_consumed_total": null,
     "reward_consumed_unit": "microliter",
     "reward_delivery": null,
     "rig_id": "ophys_rig",
-    "schema_version": "0.1.4",
-    "session_end_time": "1999-10-04T00:00:48",
-    "session_start_time": "1999-10-04T00:00:00",
+    "schema_version": "0.2.1",
+    "session_end_time": "1999-10-04T00:00:48Z",
+    "session_start_time": "1999-10-04T00:00:00Z",
     "session_type": "Foraging_Photometry",
     "stimulus_epochs": [
         {
-            "stimulus": {
-                "baseline_duration": "10.0",
-                "baseline_duration_unit": "second",
-                "fixed_pulse_train_interval": true,
-                "notes": null,
-                "number_pulse_trains": 2,
-                "other_parameters": {},
-                "pulse_frequency": 10,
-                "pulse_frequency_unit": "hertz",
-                "pulse_shape": "Square",
-                "pulse_train_duration": "2.0",
-                "pulse_train_duration_unit": "second",
-                "pulse_train_interval": "18.0",
-                "pulse_train_interval_unit": "second",
-                "pulse_width": 5000,
-                "pulse_width_unit": "millisecond",
-                "stimulus_name": "OptoStim10Hz",
-                "stimulus_type": "Opto Stimulation"
-            },
-            "stimulus_end_time": "1999-10-04T00:00:48",
-            "stimulus_start_time": "1999-10-04T00:00:00"
+            "light_source_config": null,
+            "notes": null,
+            "output_parameters": {},
+            "reward_consumed_during_epoch": null,
+            "reward_consumed_unit": "microliter",
+            "script": null,
+            "session_number": null,
+            "software": [],
+            "speaker_config": null,
+            "stimulus_device_names": [],
+            "stimulus_end_time": "1999-10-04T00:00:48Z",
+            "stimulus_modalities": [
+                "Optogenetics"
+            ],
+            "stimulus_name": "OptoStim10Hz",
+            "stimulus_parameters": [
+                {
+                    "baseline_duration": "10.0",
+                    "baseline_duration_unit": "second",
+                    "fixed_pulse_train_interval": true,
+                    "notes": null,
+                    "number_pulse_trains": [
+                        2
+                    ],
+                    "other_parameters": {},
+                    "pulse_frequency": [
+                        "10"
+                    ],
+                    "pulse_frequency_unit": "hertz",
+                    "pulse_shape": "Square",
+                    "pulse_train_duration": [
+                        "2.0"
+                    ],
+                    "pulse_train_duration_unit": "second",
+                    "pulse_train_interval": "18.0",
+                    "pulse_train_interval_unit": "second",
+                    "pulse_width": [
+                        5000
+                    ],
+                    "pulse_width_unit": "millisecond",
+                    "stimulus_name": "OptoStim10Hz",
+                    "stimulus_type": "Opto Stimulation"
+                }
+            ],
+            "stimulus_start_time": "1999-10-04T00:00:00Z",
+            "trials_finished": null,
+            "trials_rewarded": null,
+            "trials_total": null
         }
     ],
     "subject_id": "000000",
     "weight_unit": "gram"
 }
```

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json` & `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json` & `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json` & `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Face_20240212T091444.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/mesoscope/example_extract.json` & `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/example_extract.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/mesoscope/example_platform.json` & `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/example_platform.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/resources/mesoscope/expected_session.json` & `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/expected_session.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8432195801412795%*

 * *Differences: {"'active_mouse_platform'": 'True',*

 * * "'data_streams'": "{0: {'stream_start_time': '2024-02-22T15:30:00Z', 'stream_end_time': "*

 * *                   "'2024-02-22T17:30:00Z', 'ophys_fovs': {0: {'power': None, 'power_unit': "*

 * *                   "'percent', 'scanfield_z': None, 'scanfield_z_unit': 'micrometer', "*

 * *                   "'scanimage_roi_index': None, 'notes': None}, 1: {'power': None, 'power_unit': "*

 * *                   "'percent', 'scanfield_z': None, 'scanfield_z_unit': 'micrometer', "*

 * *                […]*

```diff
@@ -1,25 +1,24 @@
 {
+    "active_mouse_platform": true,
     "animal_weight_post": null,
     "animal_weight_prior": null,
     "calibrations": [],
     "data_streams": [
         {
-            "active_mouse_platform": true,
             "camera_names": [
                 "Mesoscope"
             ],
             "daq_names": [],
             "detectors": [],
             "ephys_modules": [],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
-            "mouse_platform_name": "disc",
             "notes": null,
             "ophys_fovs": [
                 {
                     "coupled_fov_index": null,
                     "fov_coordinate_ap": "1.5",
                     "fov_coordinate_ml": "1.5",
                     "fov_coordinate_unit": "micrometer",
@@ -31,14 +30,20 @@
                     "fov_width": 512,
                     "frame_rate": "9.48",
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 190,
                     "imaging_depth_unit": "micrometer",
                     "index": 0,
                     "magnification": "16x",
+                    "notes": null,
+                    "power": null,
+                    "power_unit": "percent",
+                    "scanfield_z": null,
+                    "scanfield_z_unit": "micrometer",
+                    "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
                     "coupled_fov_index": null,
                     "fov_coordinate_ap": "1.5",
                     "fov_coordinate_ml": "1.5",
                     "fov_coordinate_unit": "micrometer",
@@ -50,14 +55,20 @@
                     "fov_width": 512,
                     "frame_rate": "9.48",
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 232,
                     "imaging_depth_unit": "micrometer",
                     "index": 0,
                     "magnification": "16x",
+                    "notes": null,
+                    "power": null,
+                    "power_unit": "percent",
+                    "scanfield_z": null,
+                    "scanfield_z_unit": "micrometer",
+                    "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
                     "coupled_fov_index": null,
                     "fov_coordinate_ap": "1.5",
                     "fov_coordinate_ml": "1.5",
                     "fov_coordinate_unit": "micrometer",
@@ -69,14 +80,20 @@
                     "fov_width": 512,
                     "frame_rate": "9.48",
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 136,
                     "imaging_depth_unit": "micrometer",
                     "index": 1,
                     "magnification": "16x",
+                    "notes": null,
+                    "power": null,
+                    "power_unit": "percent",
+                    "scanfield_z": null,
+                    "scanfield_z_unit": "micrometer",
+                    "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
                     "coupled_fov_index": null,
                     "fov_coordinate_ap": "1.5",
                     "fov_coordinate_ml": "1.5",
                     "fov_coordinate_unit": "micrometer",
@@ -88,14 +105,20 @@
                     "fov_width": 512,
                     "frame_rate": "9.48",
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 282,
                     "imaging_depth_unit": "micrometer",
                     "index": 1,
                     "magnification": "16x",
+                    "notes": null,
+                    "power": null,
+                    "power_unit": "percent",
+                    "scanfield_z": null,
+                    "scanfield_z_unit": "micrometer",
+                    "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
                     "coupled_fov_index": null,
                     "fov_coordinate_ap": "1.5",
                     "fov_coordinate_ml": "1.5",
                     "fov_coordinate_unit": "micrometer",
@@ -107,14 +130,20 @@
                     "fov_width": 512,
                     "frame_rate": "9.48",
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 72,
                     "imaging_depth_unit": "micrometer",
                     "index": 2,
                     "magnification": "16x",
+                    "notes": null,
+                    "power": null,
+                    "power_unit": "percent",
+                    "scanfield_z": null,
+                    "scanfield_z_unit": "micrometer",
+                    "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
                     "coupled_fov_index": null,
                     "fov_coordinate_ap": "1.5",
                     "fov_coordinate_ml": "1.5",
                     "fov_coordinate_unit": "micrometer",
@@ -126,14 +155,20 @@
                     "fov_width": 512,
                     "frame_rate": "9.48",
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 326,
                     "imaging_depth_unit": "micrometer",
                     "index": 2,
                     "magnification": "16x",
+                    "notes": null,
+                    "power": null,
+                    "power_unit": "percent",
+                    "scanfield_z": null,
+                    "scanfield_z_unit": "micrometer",
+                    "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
                     "coupled_fov_index": null,
                     "fov_coordinate_ap": "1.5",
                     "fov_coordinate_ml": "1.5",
                     "fov_coordinate_unit": "micrometer",
@@ -145,14 +180,20 @@
                     "fov_width": 512,
                     "frame_rate": "9.48",
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 30,
                     "imaging_depth_unit": "micrometer",
                     "index": 3,
                     "magnification": "16x",
+                    "notes": null,
+                    "power": null,
+                    "power_unit": "percent",
+                    "scanfield_z": null,
+                    "scanfield_z_unit": "micrometer",
+                    "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
                     "coupled_fov_index": null,
                     "fov_coordinate_ap": "1.5",
                     "fov_coordinate_ml": "1.5",
                     "fov_coordinate_unit": "micrometer",
@@ -164,156 +205,150 @@
                     "fov_width": 512,
                     "frame_rate": "9.48",
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 364,
                     "imaging_depth_unit": "micrometer",
                     "index": 3,
                     "magnification": "16x",
+                    "notes": null,
+                    "power": null,
+                    "power_unit": "percent",
+                    "scanfield_z": null,
+                    "scanfield_z_unit": "micrometer",
+                    "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 }
             ],
             "slap_fovs": null,
             "stack_parameters": null,
             "stick_microscopes": [],
-            "stimulus_device_names": [],
-            "stream_end_time": "2024-02-22T17:30:00",
+            "stream_end_time": "2024-02-22T17:30:00Z",
             "stream_modalities": [
                 {
                     "abbreviation": "ophys",
                     "name": "Planar optical physiology"
                 }
             ],
-            "stream_start_time": "2024-02-22T15:30:00"
+            "stream_start_time": "2024-02-22T15:30:00Z"
         },
         {
-            "active_mouse_platform": true,
             "camera_names": [
                 "Behavior"
             ],
             "daq_names": [],
             "detectors": [],
             "ephys_modules": [],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
-            "mouse_platform_name": "disc",
             "notes": null,
             "ophys_fovs": [],
             "slap_fovs": null,
             "stack_parameters": null,
             "stick_microscopes": [],
-            "stimulus_device_names": [],
-            "stream_end_time": "2024-02-12T10:30:54",
+            "stream_end_time": "2024-02-12T10:30:54Z",
             "stream_modalities": [
                 {
                     "abbreviation": "behavior-videos",
                     "name": "Behavior videos"
                 }
             ],
-            "stream_start_time": "2024-02-12T09:14:43"
+            "stream_start_time": "2024-02-12T09:14:43Z"
         },
         {
-            "active_mouse_platform": true,
             "camera_names": [
                 "Eye"
             ],
             "daq_names": [],
             "detectors": [],
             "ephys_modules": [],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
-            "mouse_platform_name": "disc",
             "notes": null,
             "ophys_fovs": [],
             "slap_fovs": null,
             "stack_parameters": null,
             "stick_microscopes": [],
-            "stimulus_device_names": [],
-            "stream_end_time": "2024-02-12T10:30:55",
+            "stream_end_time": "2024-02-12T10:30:55Z",
             "stream_modalities": [
                 {
                     "abbreviation": "behavior-videos",
                     "name": "Behavior videos"
                 }
             ],
-            "stream_start_time": "2024-02-12T09:14:44"
+            "stream_start_time": "2024-02-12T09:14:44Z"
         },
         {
-            "active_mouse_platform": true,
             "camera_names": [
                 "Face"
             ],
             "daq_names": [],
             "detectors": [],
             "ephys_modules": [],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
-            "mouse_platform_name": "disc",
             "notes": null,
             "ophys_fovs": [],
             "slap_fovs": null,
             "stack_parameters": null,
             "stick_microscopes": [],
-            "stimulus_device_names": [],
-            "stream_end_time": "2024-02-12T10:30:55",
+            "stream_end_time": "2024-02-12T10:30:55Z",
             "stream_modalities": [
                 {
                     "abbreviation": "behavior-videos",
                     "name": "Behavior videos"
                 }
             ],
-            "stream_start_time": "2024-02-12T09:14:44"
+            "stream_start_time": "2024-02-12T09:14:44Z"
         },
         {
-            "active_mouse_platform": true,
             "camera_names": [
                 "Vasculature"
             ],
             "daq_names": [],
             "detectors": [],
             "ephys_modules": [],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
-            "mouse_platform_name": "disc",
             "notes": null,
             "ophys_fovs": [],
             "slap_fovs": null,
             "stack_parameters": null,
             "stick_microscopes": [],
-            "stimulus_device_names": [],
-            "stream_end_time": "2024-02-12T11:02:22",
+            "stream_end_time": "2024-02-12T11:02:22Z",
             "stream_modalities": [
                 {
                     "abbreviation": "confocal",
                     "name": "Confocal microscopy"
                 }
             ],
-            "stream_start_time": "2024-02-12T11:02:22"
+            "stream_start_time": "2024-02-12T11:02:22Z"
         }
     ],
     "describedBy": "https://raw.githubusercontent.com/AllenNeuralDynamics/aind-data-schema/main/src/aind_data_schema/core/session.py",
     "experimenter_full_name": [
         "John Doe"
     ],
     "iacuc_protocol": "12345",
     "maintenance": [],
+    "mouse_platform_name": "disc",
     "notes": null,
     "protocol_id": [],
     "reward_consumed_total": null,
     "reward_consumed_unit": "microliter",
     "reward_delivery": null,
     "rig_id": "MESO.1",
-    "schema_version": "0.1.4",
-    "session_end_time": "2024-02-22T17:30:00",
-    "session_start_time": "2024-02-22T15:30:00",
+    "schema_version": "0.2.1",
+    "session_end_time": "2024-02-22T17:30:00Z",
+    "session_start_time": "2024-02-22T15:30:00Z",
     "session_type": "Mesoscope",
     "stimulus_epochs": [],
     "subject_id": "12345",
     "weight_unit": "gram"
 }
```

### Comparing `aind-metadata-mapper-0.6.0/tests/test_bergamo.py` & `aind-metadata-mapper-0.6.1/tests/test_bergamo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests parsing of session information from bergamo rig."""
 
 import gzip
 import json
 import os
 import unittest
-from datetime import datetime
+from datetime import datetime, timezone
 from pathlib import Path
 from unittest.mock import MagicMock, call, patch
 
 from aind_data_schema.core.session import Session
 
 from aind_metadata_mapper.bergamo.session import (
     BergamoEtl,
@@ -42,20 +42,32 @@
         cls.example_shape = [347, 512, 512]
         cls.example_job_settings = JobSettings(
             input_source=RESOURCES_DIR,
             mouse_platform_name="some_mouse_platform_name",
             active_mouse_platform=True,
             experimenter_full_name=["John Smith", "Jane Smith"],
             subject_id="12345",
-            session_start_time=datetime(2023, 10, 10, 14, 0, 0),
-            session_end_time=datetime(2023, 10, 10, 17, 0, 0),
-            stream_start_time=datetime(2023, 10, 10, 15, 0, 0),
-            stream_end_time=datetime(2023, 10, 10, 16, 0, 0),
-            stimulus_start_time=datetime(2023, 10, 10, 15, 15, 0),
-            stimulus_end_time=datetime(2023, 10, 10, 15, 45, 0),
+            session_start_time=datetime(
+                2023, 10, 10, 14, 0, 0, tzinfo=timezone.utc
+            ),
+            session_end_time=datetime(
+                2023, 10, 10, 17, 0, 0, tzinfo=timezone.utc
+            ),
+            stream_start_time=datetime(
+                2023, 10, 10, 15, 0, 0, tzinfo=timezone.utc
+            ),
+            stream_end_time=datetime(
+                2023, 10, 10, 16, 0, 0, tzinfo=timezone.utc
+            ),
+            stimulus_start_time=datetime(
+                2023, 10, 10, 15, 15, 0, tzinfo=timezone.utc
+            ),
+            stimulus_end_time=datetime(
+                2023, 10, 10, 15, 45, 0, tzinfo=timezone.utc
+            ),
         )
         cls.expected_session = expected_session_contents
 
     def test_class_constructor(self):
         """Tests that the class can be constructed from a json string"""
         settings1 = self.example_job_settings.model_copy(deep=True)
         json_str = settings1.model_dump_json()
```

### Comparing `aind-metadata-mapper-0.6.0/tests/test_ephys.py` & `aind-metadata-mapper-0.6.1/tests/test_ephys.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tests parsing of session information from ephys rig."""
 
 import csv
 import json
 import os
 import unittest
+import zoneinfo
 from pathlib import Path
 from xml.dom import minidom
 
 from aind_data_schema.core.session import Session
 
 from aind_metadata_mapper.ephys.session import EphysEtl
 
@@ -25,14 +26,16 @@
 
 EXPECTED_SESSION = RESOURCES_DIR / "ephys_session.json"
 
 
 class TestSchemaWriter(unittest.TestCase):
     """Test methods in SchemaWriter class."""
 
+    maxDiff = None  # show full diff without truncation
+
     @classmethod
     def setUpClass(cls):
         """Load record object and user settings before running tests."""
         # TODO: Add visual stimulus
         cls.experiment_data = {
             "experimenter_full_name": ["Al Dente"],
             "subject_id": "699889",
@@ -214,12 +217,32 @@
             output_directory=RESOURCES_DIR,
             stage_logs=self.stage_logs,
             openephys_logs=self.openephys_logs,
             experiment_data=self.experiment_data,
         )
         parsed_info = etl_job1._extract()
         actual_session = etl_job1._transform(parsed_info)
-        self.assertEqual(self.expected_session, actual_session)
+        actual_session.session_start_time = (
+            actual_session.session_start_time.replace(
+                tzinfo=zoneinfo.ZoneInfo("UTC")
+            )
+        )
+        actual_session.session_end_time = (
+            actual_session.session_end_time.replace(
+                tzinfo=zoneinfo.ZoneInfo("UTC")
+            )
+        )
+        for stream in actual_session.data_streams:
+            stream.stream_start_time = stream.stream_start_time.replace(
+                tzinfo=zoneinfo.ZoneInfo("UTC")
+            )
+            stream.stream_end_time = stream.stream_end_time.replace(
+                tzinfo=zoneinfo.ZoneInfo("UTC")
+            )
+        self.assertEqual(
+            self.expected_session.model_dump(),
+            actual_session.model_dump(),
+        )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aind-metadata-mapper-0.6.0/tests/test_fib.py` & `aind-metadata-mapper-0.6.1/tests/test_fib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests parsing of session information from fib rig."""
 
 import json
 import os
 import unittest
+import zoneinfo
 from datetime import datetime
 from pathlib import Path
 
 from aind_data_schema.core.session import Session
 
 from aind_metadata_mapper.fib.session import FIBEtl, JobSettings
 
@@ -28,15 +29,17 @@
             raw_md_contents = f.read()
         with open(EXPECTED_SESSION, "r") as f:
             expected_session_contents = Session(**json.load(f))
 
         cls.example_job_settings = JobSettings(
             string_to_parse=raw_md_contents,
             experimenter_full_name=["Don Key"],
-            session_start_time=datetime(1999, 10, 4),
+            session_start_time=datetime(
+                1999, 10, 4, tzinfo=zoneinfo.ZoneInfo("UTC")
+            ),
             notes="brabrabrabra....",
             labtracks_id="000000",
             iacuc_protocol="2115",
             light_source_list=[
                 {
                     "name": "470nm LED",
                     "excitation_power": 0.020,
@@ -93,15 +96,16 @@
 
         etl_job1 = FIBEtl(job_settings=self.example_job_settings)
         parsed_info = etl_job1._extract()
         self.assertEqual(
             self.example_job_settings.string_to_parse, parsed_info.teensy_str
         )
         self.assertEqual(
-            datetime(1999, 10, 4), self.example_job_settings.session_start_time
+            datetime(1999, 10, 4, tzinfo=zoneinfo.ZoneInfo("UTC")),
+            self.example_job_settings.session_start_time,
         )
 
     def test_transform(self):
         """Tests that the teensy response maps correctly to ophys session."""
 
         etl_job1 = FIBEtl(job_settings=self.example_job_settings)
         parsed_info = etl_job1._extract()
```

### Comparing `aind-metadata-mapper-0.6.0/tests/test_legacy_core.py` & `aind-metadata-mapper-0.6.1/tests/test_legacy_core.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.0/tests/test_mesoscope.py` & `aind-metadata-mapper-0.6.1/tests/test_mesoscope.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Unit tests for mesoscope etl package"""
 
 import json
 import os
 import unittest
+import zoneinfo
 from datetime import datetime
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 from aind_data_schema.core.session import Session
 from PIL import Image
 
@@ -23,14 +24,16 @@
 EXAMPLE_PLATFORM = RESOURCES_DIR / "example_platform.json"
 EXAMPLE_IMAGE = RESOURCES_DIR / "test.tiff"
 
 
 class TestMesoscope(unittest.TestCase):
     """Tests methods in MesoscopeEtl class"""
 
+    maxDiff = None  # show full diff without truncation
+
     @classmethod
     def setUpClass(cls) -> None:
         """Set up the test suite"""
         with open(EXAMPLE_EXTRACT, "r") as f:
             cls.example_extract = json.load(f)
         with open(EXAMPLE_SESSION, "r") as f:
             cls.example_session = json.load(f)
@@ -40,16 +43,20 @@
             "fov_scale_factor": 1.0,
         }
         cls.example_job_settings = JobSettings(
             input_source=EXAMPLE_PLATFORM,
             behavior_source=RESOURCES_DIR,
             output_directory=RESOURCES_DIR,
             subject_id="12345",
-            session_start_time=datetime(2024, 2, 22, 15, 30, 0),
-            session_end_time=datetime(2024, 2, 22, 17, 30, 0),
+            session_start_time=datetime(
+                2024, 2, 22, 15, 30, 0, tzinfo=zoneinfo.ZoneInfo("UTC")
+            ),
+            session_end_time=datetime(
+                2024, 2, 22, 17, 30, 0, tzinfo=zoneinfo.ZoneInfo("UTC")
+            ),
             project="some_project",
             experimenter_full_name=["John Doe"],
             magnification="16x",
             fov_coordinate_ap=1.5,
             fov_coordinate_ml=1.5,
             fov_reference="Bregma",
             iacuc_protocol="12345",
@@ -154,14 +161,15 @@
     @patch(
         "aind_metadata_mapper.mesoscope.session.MesoscopeEtl._read_metadata"
     )
     @patch("PIL.Image.open")
     def test_transform(self, mock_open, mock_scanimage) -> None:
         """Tests that the platform json is extracted and transfromed into a
         session object correctly"""
+
         etl = MesoscopeEtl(
             job_settings=self.example_job_settings,
         )
         # mock vasculature image
         mock_image = Image.new("RGB", (100, 100))
         mock_image.tag = {306: ("2024:02:12 11:02:22",)}
         mock_open.return_value = mock_image
@@ -177,15 +185,21 @@
         mock_meta[0][
             "SI.hRoiManager.scanZoomFactor"
         ] = self.example_scanimage_meta["fov_scale_factor"]
         mock_scanimage.return_value = mock_meta
 
         extract = etl._extract()
         transformed_session = etl._transform(extract)
-
+        for stream in transformed_session.data_streams:
+            stream.stream_start_time = stream.stream_start_time.replace(
+                tzinfo=zoneinfo.ZoneInfo("UTC")
+            )
+            stream.stream_end_time = stream.stream_end_time.replace(
+                tzinfo=zoneinfo.ZoneInfo("UTC")
+            )
         self.assertEqual(
             self.example_session,
             json.loads(transformed_session.model_dump_json()),
         )
 
     @patch("aind_metadata_mapper.mesoscope.session.MesoscopeEtl._extract")
     @patch("aind_metadata_mapper.mesoscope.session.MesoscopeEtl._transform")
```

