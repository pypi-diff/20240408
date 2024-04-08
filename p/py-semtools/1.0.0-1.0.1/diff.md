# Comparing `tmp/py_semtools-1.0.0.tar.gz` & `tmp/py_semtools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_semtools-1.0.0.tar", last modified: Mon Oct  9 14:02:26 2023, max compression
+gzip compressed data, was "py_semtools-1.0.1.tar", last modified: Mon Apr  8 10:01:55 2024, max compression
```

## Comparing `py_semtools-1.0.0.tar` & `py_semtools-1.0.1.tar`

### file list

```diff
@@ -1,68 +1,100 @@
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-09 14:02:26.809548 py_semtools-1.0.0/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      594 2023-10-06 13:24:19.000000 py_semtools-1.0.0/.coveragerc
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      566 2023-10-06 13:24:19.000000 py_semtools-1.0.0/.gitignore
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      530 2023-10-06 13:24:19.000000 py_semtools-1.0.0/.readthedocs.yml
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       82 2023-10-06 13:24:19.000000 py_semtools-1.0.0/AUTHORS.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      128 2023-10-06 13:24:19.000000 py_semtools-1.0.0/CHANGELOG.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    13866 2023-10-06 13:24:19.000000 py_semtools-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1079 2023-10-06 13:24:19.000000 py_semtools-1.0.0/LICENSE.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       49 2023-03-23 12:46:41.000000 py_semtools-1.0.0/MANIFEST.in
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2447 2023-10-09 14:02:26.809210 py_semtools-1.0.0/PKG-INFO
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        0 2023-02-21 11:12:17.000000 py_semtools-1.0.0/README.md
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1687 2023-10-06 13:24:19.000000 py_semtools-1.0.0/README.rst
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-09 14:02:26.750857 py_semtools-1.0.0/docs/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1154 2023-10-06 13:24:19.000000 py_semtools-1.0.0/docs/Makefile
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-09 14:02:26.751314 py_semtools-1.0.0/docs/_static/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       18 2023-10-06 13:24:19.000000 py_semtools-1.0.0/docs/_static/.gitignore
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       41 2023-10-06 13:24:19.000000 py_semtools-1.0.0/docs/authors.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       43 2023-10-06 13:24:19.000000 py_semtools-1.0.0/docs/changelog.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     9754 2023-10-06 13:24:19.000000 py_semtools-1.0.0/docs/conf.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       33 2023-10-06 13:24:19.000000 py_semtools-1.0.0/docs/contributing.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2329 2023-10-06 13:24:19.000000 py_semtools-1.0.0/docs/index.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       67 2023-10-06 13:24:19.000000 py_semtools-1.0.0/docs/license.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       39 2023-10-06 13:24:19.000000 py_semtools-1.0.0/docs/readme.rst
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      233 2023-10-06 13:24:19.000000 py_semtools-1.0.0/docs/requirements.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      346 2023-10-06 13:24:19.000000 py_semtools-1.0.0/pyproject.toml
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1344 2023-10-09 14:02:26.810867 py_semtools-1.0.0/setup.cfg
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      706 2023-10-06 13:24:19.000000 py_semtools-1.0.0/setup.py
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-09 14:02:26.739278 py_semtools-1.0.0/src/
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-09 14:02:26.754870 py_semtools-1.0.0/src/py_semtools/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      180 2023-10-06 13:24:19.000000 py_semtools-1.0.0/src/py_semtools/__init__.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    20107 2023-10-06 13:24:19.000000 py_semtools-1.0.0/src/py_semtools/cli_manager.py
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-09 14:02:26.758405 py_semtools-1.0.0/src/py_semtools/external_data/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      176 2023-10-06 13:24:19.000000 py_semtools-1.0.0/src/py_semtools/external_data/ontologies.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      849 2023-10-06 13:24:19.000000 py_semtools-1.0.0/src/py_semtools/file_parser.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1249 2023-10-06 13:24:19.000000 py_semtools-1.0.0/src/py_semtools/json_parser.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    21892 2023-10-06 13:24:19.000000 py_semtools-1.0.0/src/py_semtools/oboparser.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    63862 2023-10-06 13:24:19.000000 py_semtools-1.0.0/src/py_semtools/ontology.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     3875 2023-10-06 13:24:19.000000 py_semtools-1.0.0/src/py_semtools/sim_handler.py
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-09 14:02:26.757985 py_semtools-1.0.0/src/py_semtools.egg-info/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2447 2023-10-09 14:02:26.755470 py_semtools-1.0.0/src/py_semtools.egg-info/PKG-INFO
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1408 2023-10-09 14:02:26.755883 py_semtools-1.0.0/src/py_semtools.egg-info/SOURCES.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        1 2023-10-09 14:02:26.756329 py_semtools-1.0.0/src/py_semtools.egg-info/dependency_links.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      108 2023-10-09 14:02:26.756774 py_semtools-1.0.0/src/py_semtools.egg-info/entry_points.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        1 2023-10-06 10:22:03.000000 py_semtools-1.0.0/src/py_semtools.egg-info/not-zip-safe
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      119 2023-10-09 14:02:26.757688 py_semtools-1.0.0/src/py_semtools.egg-info/requires.txt
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       12 2023-10-09 14:02:26.758097 py_semtools-1.0.0/src/py_semtools.egg-info/top_level.txt
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-09 14:02:26.761720 py_semtools-1.0.0/tests/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/__init__.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      279 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/conftest.py
-drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-09 14:02:26.807536 py_semtools-1.0.0/tests/data/
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      169 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/circular_sample.obo
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      350 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/enrichment_ontology.obo
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      406 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/enrichment_ontology2.obo
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)  1562135 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/go-basic_sample.obo
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1737 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/go-onlyOne.obo
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      485 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/hierarchical_sample.obo
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       48 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/only_header_sample.obo
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126) 13759531 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/partial_go.json
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)  5318794 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/partial_go.obo
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      189 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/short_hierarchical_sample.obo
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      186 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/sparse2_sample.obo
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      172 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/data/sparse_sample.obo
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2182 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/test_go.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2108 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/test_jsonparser.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    13579 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/test_oboparser.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    41188 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/test_ontology.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     3838 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tests/test_similitudes.py
--rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2851 2023-10-06 13:24:19.000000 py_semtools-1.0.0/tox.ini
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.482644 py_semtools-1.0.1/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      594 2023-10-06 13:24:19.000000 py_semtools-1.0.1/.coveragerc
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      566 2023-10-06 13:24:19.000000 py_semtools-1.0.1/.gitignore
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      530 2023-10-06 13:24:19.000000 py_semtools-1.0.1/.readthedocs.yml
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       82 2023-10-06 13:24:19.000000 py_semtools-1.0.1/AUTHORS.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      128 2023-10-06 13:24:19.000000 py_semtools-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    13866 2023-10-06 13:24:19.000000 py_semtools-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1079 2023-10-06 13:24:19.000000 py_semtools-1.0.1/LICENSE.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       49 2023-03-23 12:46:41.000000 py_semtools-1.0.1/MANIFEST.in
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2586 2024-04-08 10:01:55.482080 py_semtools-1.0.1/PKG-INFO
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        0 2023-02-21 11:12:17.000000 py_semtools-1.0.1/README.md
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1687 2023-10-06 13:24:19.000000 py_semtools-1.0.1/README.rst
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.187769 py_semtools-1.0.1/docs/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1154 2023-10-06 13:24:19.000000 py_semtools-1.0.1/docs/Makefile
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.188946 py_semtools-1.0.1/docs/_static/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       18 2023-10-06 13:24:19.000000 py_semtools-1.0.1/docs/_static/.gitignore
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       41 2023-10-06 13:24:19.000000 py_semtools-1.0.1/docs/authors.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       43 2023-10-06 13:24:19.000000 py_semtools-1.0.1/docs/changelog.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     9754 2023-10-06 13:24:19.000000 py_semtools-1.0.1/docs/conf.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       33 2023-10-06 13:24:19.000000 py_semtools-1.0.1/docs/contributing.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2329 2023-10-06 13:24:19.000000 py_semtools-1.0.1/docs/index.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       67 2023-10-06 13:24:19.000000 py_semtools-1.0.1/docs/license.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       39 2023-10-06 13:24:19.000000 py_semtools-1.0.1/docs/readme.rst
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      233 2023-10-06 13:24:19.000000 py_semtools-1.0.1/docs/requirements.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      346 2023-10-06 13:24:19.000000 py_semtools-1.0.1/pyproject.toml
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1722 2024-04-08 10:01:55.484730 py_semtools-1.0.1/setup.cfg
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      706 2023-10-06 13:24:19.000000 py_semtools-1.0.1/setup.py
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.144779 py_semtools-1.0.1/src/
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.235796 py_semtools-1.0.1/src/py_semtools/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      218 2023-10-17 12:54:47.000000 py_semtools-1.0.1/src/py_semtools/__init__.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    56746 2024-04-04 13:13:08.000000 py_semtools-1.0.1/src/py_semtools/cli_manager.py
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.244865 py_semtools-1.0.1/src/py_semtools/external_data/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      176 2023-10-06 13:24:19.000000 py_semtools-1.0.1/src/py_semtools/external_data/ontologies.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      849 2023-10-06 13:24:19.000000 py_semtools-1.0.1/src/py_semtools/file_parser.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1249 2023-10-06 13:24:19.000000 py_semtools-1.0.1/src/py_semtools/json_parser.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    21874 2024-03-21 14:54:09.000000 py_semtools-1.0.1/src/py_semtools/oboparser.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    68611 2024-04-04 13:04:58.000000 py_semtools-1.0.1/src/py_semtools/ontology.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     3875 2023-10-06 13:24:19.000000 py_semtools-1.0.1/src/py_semtools/sim_handler.py
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.243647 py_semtools-1.0.1/src/py_semtools.egg-info/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2586 2024-04-08 10:01:54.000000 py_semtools-1.0.1/src/py_semtools.egg-info/PKG-INFO
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2789 2024-04-08 10:01:55.238246 py_semtools-1.0.1/src/py_semtools.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        1 2024-04-08 10:01:54.000000 py_semtools-1.0.1/src/py_semtools.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      344 2024-04-08 10:01:54.000000 py_semtools-1.0.1/src/py_semtools.egg-info/entry_points.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        1 2023-10-06 10:22:03.000000 py_semtools-1.0.1/src/py_semtools.egg-info/not-zip-safe
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      183 2024-04-08 10:01:54.000000 py_semtools-1.0.1/src/py_semtools.egg-info/requires.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       12 2024-04-08 10:01:54.000000 py_semtools-1.0.1/src/py_semtools.egg-info/top_level.txt
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.290351 py_semtools-1.0.1/tests/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)        0 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/__init__.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      279 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/conftest.py
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.447916 py_semtools-1.0.1/tests/data/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      169 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/data/circular_sample.obo
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      393 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/enrichment_ontology.obo
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      406 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/data/enrichment_ontology2.obo
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.145817 py_semtools-1.0.1/tests/data/get_sorted_suggestions/
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.454845 py_semtools-1.0.1/tests/data/get_sorted_suggestions/expected/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       73 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/get_sorted_suggestions/expected/filter_query_parentals.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       73 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/get_sorted_suggestions/expected/filter_target_and_query_parentals.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       90 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/get_sorted_suggestions/expected/filter_target_parentals.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       91 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/get_sorted_suggestions/expected/no_filter_limit_2.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      112 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/get_sorted_suggestions/expected/no_filter_no_limit.txt
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.458971 py_semtools-1.0.1/tests/data/get_sorted_suggestions/input_data/
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      472 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/get_sorted_suggestions/input_data/enrichment_ontology3.obo
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       53 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/get_sorted_suggestions/input_data/query_hps.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      196 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/get_sorted_suggestions/input_data/relations.txt
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)  1562135 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/data/go-basic_sample.obo
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     1737 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/data/go-onlyOne.obo
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      485 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/data/hierarchical_sample.obo
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.466418 py_semtools-1.0.1/tests/data/input_scripts/
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)      123 2023-10-17 12:54:47.000000 py_semtools-1.0.1/tests/data/input_scripts/profiles
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)      141 2023-10-17 12:54:47.000000 py_semtools-1.0.1/tests/data/input_scripts/profiles_2cols
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)       95 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/input_scripts/profiles_with_removedTerms
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)       47 2023-10-17 12:54:47.000000 py_semtools-1.0.1/tests/data/input_scripts/string_values
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)       27 2023-10-17 12:54:48.000000 py_semtools-1.0.1/tests/data/input_scripts/terms
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)       42 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/input_scripts/terms_for_xref
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)       48 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/data/only_header_sample.obo
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126) 13759531 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/data/partial_go.json
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)  5318794 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/data/partial_go.obo
+drwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)        0 2024-04-08 10:01:55.479739 py_semtools-1.0.1/tests/data/ref_output_scripts/
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)       84 2023-10-17 12:54:48.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/cleaned_profiles
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)       89 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/cleaned_profiles_2cols
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)      161 2023-10-17 12:54:48.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/expanded_profiles
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)      135 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/expected_IC_ont
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)       52 2023-10-17 12:54:48.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/parental_from_terms
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)      327 2023-10-17 12:54:48.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/profile_stats
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)      216 2023-10-17 12:54:48.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/profiles_IC_onto_freq
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)      275 2023-10-17 12:54:48.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/strsimnet
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)       87 2023-10-17 12:54:48.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/strsimnet_cutoff2
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)       94 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/terms_attr
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)       86 2023-10-17 12:54:48.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/translated_profiles_names
+-rwxr-xr-x   0 pedro     (6413) bio_267_uma  (3126)       68 2023-10-17 12:54:48.000000 py_semtools-1.0.1/tests/data/ref_output_scripts/translated_terms_codes
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      189 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/data/short_hierarchical_sample.obo
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      186 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/data/sparse2_sample.obo
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)      172 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/data/sparse_sample.obo
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    16830 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/test_cli_manager.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2182 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/test_go.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2108 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/test_jsonparser.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    13579 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/test_oboparser.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)    42606 2023-10-23 12:03:19.000000 py_semtools-1.0.1/tests/test_ontology.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     3838 2023-10-06 13:24:19.000000 py_semtools-1.0.1/tests/test_similitudes.py
+-rw-r--r--   0 pedro     (6413) bio_267_uma  (3126)     2952 2023-11-10 14:29:46.000000 py_semtools-1.0.1/tox.ini
```

### Comparing `py_semtools-1.0.0/.coveragerc` & `py_semtools-1.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/.gitignore` & `py_semtools-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/.readthedocs.yml` & `py_semtools-1.0.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/CONTRIBUTING.rst` & `py_semtools-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/LICENSE.txt` & `py_semtools-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/PKG-INFO` & `py_semtools-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: py_semtools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: seoanezonjic
 Author-email: darklordsone@hotmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: platformdirs
 Requires-Dist: numpy
 Requires-Dist: networkx
+Requires-Dist: entrezpy
 Requires-Dist: scipy
+Requires-Dist: sentence_transformers
+Requires-Dist: requests
 Requires-Dist: py_exp_calc
+Requires-Dist: py_cmdtabs
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
```

### Comparing `py_semtools-1.0.0/README.rst` & `py_semtools-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/docs/Makefile` & `py_semtools-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/docs/conf.py` & `py_semtools-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/docs/index.rst` & `py_semtools-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/setup.cfg` & `py_semtools-1.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -19,34 +19,47 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
+	platformdirs
 	numpy
 	networkx
+	entrezpy
 	scipy
+	sentence_transformers
+	requests
 	py_exp_calc
+	py_cmdtabs
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
+[options.package_data]
+py_semtools.external_data = 
+	ontologies.txt
+
 [options.extras_require]
 testing = 
 	setuptools
 	pytest
 	pytest-cov
 
 [options.entry_points]
 console_scripts = 
 	semtools = py_semtools.cli_manager:semtools
 	strsimnet = py_semtools.cli_manager:strsimnet
+	get_sorted_suggestions = py_semtools.cli_manager:get_sorted_suggestions
+	remote_retriever = py_semtools.cli_manager:remote_retriever
+	stEngine = py_semtools.cli_manager:stEngine
+	get_pubmed_index = py_semtools.cli_manager:get_pubmed_index
 
 [tool:pytest]
 addopts = 
 	--cov py_semtools --cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
```

### Comparing `py_semtools-1.0.0/setup.py` & `py_semtools-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/src/py_semtools/file_parser.py` & `py_semtools-1.0.1/src/py_semtools/file_parser.py`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/src/py_semtools/json_parser.py` & `py_semtools-1.0.1/src/py_semtools/json_parser.py`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/src/py_semtools/oboparser.py` & `py_semtools-1.0.1/src/py_semtools/oboparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,21 +111,20 @@
     def process_entity(cls, header, infoType, stanzas, currInfo):
         info = cls.info2hash(currInfo)
         # Store current info
         if infoType == 'Header':
             header = info
         else:
             entity_id = info['id']
-            match infoType:
-                case 'Term':
-                    stanzas['terms'][entity_id] = info
-                case 'Typedef':
-                    stanzas['typedefs'][entity_id] = info
-                case 'Instance':
-                    stanzas['instances'][entity_id] = info
+            if infoType == 'Term':
+                stanzas['terms'][entity_id] = info
+            elif infoType == 'Typedef':
+                stanzas['typedefs'][entity_id] = info
+            elif infoType == 'Instance':
+                stanzas['instances'][entity_id] = info
         return header
 
     # Class method to transform string with <tag : info> into hash structure
     # ===== Parameters
     # +attributes+:: array tuples with info to be transformed into hash format
     # ===== Returns 
     # Attributes stored into hash structure
```

### Comparing `py_semtools-1.0.0/src/py_semtools/ontology.py` & `py_semtools-1.0.1/src/py_semtools/ontology.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import math
 import os
 import sys
+import time
 import copy
 import warnings
 import json
 import numpy as np
 from collections import defaultdict
 import networkx as nx
+import entrezpy.esearch.esearcher
 from concurrent.futures import ProcessPoolExecutor as PoolExecutor
 from functools import partial
-from collections import defaultdict
+from collections import defaultdict, deque
 import time
 import itertools
+import re
+import py_exp_calc.exp_calc as pxc
 
 from py_semtools import OboParser
 from py_semtools import JsonParser
 
 from py_exp_calc.exp_calc import intersection, union, diff
 
 class Ontology:
@@ -177,23 +181,22 @@
     # ===== Parameters
     # +term+:: which are requested
     # +relation+:: can be :ancestor or :descendant 
     # ===== Returns
     # Direct ancestors/descendants of given term or nil if any error occurs
     def get_direct_related(self, term, relation):
         target = None
-        match relation:
-            case 'ancestor':
-                target = 'byTerm'
-            case 'descendant':
-                target = 'byValue'
-            case _:
-                warnings.warn('Relation type not allowed. Returning None')
+        if relation == 'ancestor':
+            target = 'byTerm'
+        elif relation ==  'descendant':
+            target = 'byValue'
+        else:
+            warnings.warn('Relation type not allowed. Returning None')
         query = self.dicts['is_a'][target].get(term)
-        return query
+        return copy.deepcopy(query)
 
     # Return direct ancestors/descendants of a given term
     # Return direct ancestors of a given term
     # ===== Parameters
     # +term+:: which ancestors are requested
     # ===== Returns
     # Direct ancestors of given term or nil if any error occurs
@@ -210,37 +213,47 @@
 
     # Find ancestors/descendants of a given term
     # ===== Parameters
     # +term+:: to be checked
     # +return_ancestors+:: return ancestors if true or descendants if false
     # ===== Returns 
     # an array with all ancestors/descendants of given term or nil if parents are not available yet
-    def get_familiar(self, term, return_ancestors = True):
-        familiars = self.ancestors_index.get(term) if return_ancestors else self.descendants_index.get(term)
-        if familiars != None:
-            familiars = copy.copy(familiars)
-        else:
+    def get_familiar(self, term, return_ancestors = True, sorted_by_level = False):
+        if sorted_by_level:
             familiars = []
+            stack = deque(copy.deepcopy(self.get_direct_ancentors(term) if return_ancestors else self.get_direct_descendants(term)))
+            while len(stack) > 0:
+                next_term = stack.popleft()
+                familiars.append(next_term)
+                next_term_childs = self.get_direct_ancentors(next_term) if return_ancestors else self.get_direct_descendants(next_term) 
+                if next_term_childs != None: 
+                    for term in next_term_childs: stack.append(term)  
+        else:
+            familiars = self.ancestors_index.get(term) if return_ancestors else self.descendants_index.get(term)
+            if familiars != None:
+                familiars = copy.copy(familiars)
+            else:
+                familiars = []
         return familiars
 
     # Find ancestors of a given term
     # ===== Parameters
     # +term+:: to be checked
     # ===== Returns 
     # an array with all ancestors of given term or false if parents are not available yet
-    def get_ancestors(self, term):
-        return self.get_familiar(term, True)
+    def get_ancestors(self, term, sorted_by_level = False):
+        return self.get_familiar(term, True, sorted_by_level)
 
     # Find descendants of a given term
     # ===== Parameters
     # +term+:: to be checked
     # ===== Returns 
     # an array with all descendants of given term or false if parents are not available yet
-    def get_descendants(self, term):
-        return self.get_familiar(term, False)        
+    def get_descendants(self, term, sorted_by_level = False):
+        return self.get_familiar(term, False, sorted_by_level)        
 
     # Gets ontology level of a specific term
     # ===== Returns 
     # Term level
     def get_term_level(self, term):
         return self.dicts['level']['byValue'].get(term)
 
@@ -309,14 +322,36 @@
     # +id+:: to be translated
     # ===== Return
     # main name or nil if it's not included into this ontology
     def translate_id(self, t_id):
         name = self.translate(t_id, 'name', byValue = False)
         return None if name == None else name[0]
 
+    def get_synonims(self, t_id):
+        syns = self.dicts['synonym']['byTerm'].get(t_id)
+        if syns == None: syns = []
+        return syns
+
+
+    def filter_list(self, term_list, whitelist=[], blacklist=[]):
+        filt_list = []
+        for term_id in term_list:
+            keep = True
+            parentals = self.get_ancestors(term_id)
+            if len(whitelist) > 0:
+                wkeep = False
+                for wparental in whitelist:
+                    if wparental in parentals: wkeep = True; break
+                if not wkeep: keep = False # If there is white list but any parental is in the white list, remove the current term
+            for bparental in blacklist:
+                if bparental in parentals: keep = False; break
+            if keep: filt_list.append(term_id)
+        return filt_list
+
+
     # Get term frequency and information
     ####################################
 
     # One single term #
 
     # Get a term frequency
     # ===== Parameters
@@ -355,57 +390,57 @@
     def get_IC(self, term, ic_type = 'resnik', force = False, zhou_k = 0.5):
         curr_ics = self.ics[ic_type]
         if ic_type not in self.allowed_calcs['ics']: raise Exception(f"IC type specified ({ic_type}) is not allowed") 
         if term in curr_ics and not force: return curr_ics[term]  # Check if it's already calculated
         # Calculate
         ic = - 1
         term_meta = self.meta[term]
-        match ic_type: # https://arxiv.org/ftp/arxiv/papers/1310/1310.8059.pdf  |||  https://sci-hub.st/https://doi.org/10.1016/j.eswa.2012.01.082
-            ###########################################
-            #### STRUCTURE BASED METRICS
-            ###########################################
-            # Shortest path
-            # Weighted Link
-            # Hirst and St-Onge Measure
-            # Wu and Palmer
-            # Slimani
-            # Li
-            # Leacock and Chodorow
-            ###########################################
-            #### INFORMATION CONTENT METRICS
-            ###########################################
-            case 'resnik': # Resnik P: Using Information Content to Evaluate Semantic Similarity in a Taxonomy
-                # -log(Freq(x) / Max_Freq)
-                ic = -math.log10(term_meta['struct_freq'] / self.max_freqs['struct_freq'])
-            case 'resnik_observed':
-                # -log(Freq(x) / Max_Freq)
-                ic = -math.log10(term_meta['observed_freq'] / self.max_freqs['observed_freq'])
-            # Lin
-            # Jiang & Conrath
-
-            ###########################################
-            #### FEATURE-BASED METRICS
-            ###########################################
-            # Tversky
-            # x-similarity
-            # Rodirguez
-
-            ###########################################
-            #### HYBRID METRICS
-            ###########################################
-            case 'seco' | 'zhou': # SECO:: An intrinsic information content metric for semantic similarity in WordNet
-                #  1 - ( log(hypo(x) + 1) / log(max_nodes) )
-                ic = 1 - math.log10(term_meta['struct_freq']) / math.log10(len(self.terms))
-                if 'zhou': # New Model of Semantic Similarity Measuring in Wordnet                
-                    # k*(IC_Seco(x)) + (1-k)*(log(depth(x))/log(max_depth))
-                    self.ics['seco'][term] = ic # Special store
-                    ic = zhou_k * ic + (1.0 - zhou_k) * (math.log10(term_meta['descendants']) / math.log10(self.max_freqs['max_depth']))
-            case 'sanchez': # Semantic similarity estimation in the biomedical domain: An ontology-basedinformation-theoretic perspective
-                ic = -math.log10((term_meta['descendants'] / term_meta['ancestors'] + 1.0) / (self.max_freqs['max_depth'] + 1.0))
-            # Knappe
+        # https://arxiv.org/ftp/arxiv/papers/1310/1310.8059.pdf  |||  https://sci-hub.st/https://doi.org/10.1016/j.eswa.2012.01.082
+        ###########################################
+        #### STRUCTURE BASED METRICS
+        ###########################################
+        # Shortest path
+        # Weighted Link
+        # Hirst and St-Onge Measure
+        # Wu and Palmer
+        # Slimani
+        # Li
+        # Leacock and Chodorow
+        ###########################################
+        #### INFORMATION CONTENT METRICS
+        ###########################################
+        if ic_type == 'resnik': # Resnik P: Using Information Content to Evaluate Semantic Similarity in a Taxonomy
+            # -log(Freq(x) / Max_Freq)
+            ic = -math.log10(term_meta['struct_freq'] / self.max_freqs['struct_freq'])
+        elif ic_type == 'resnik_observed':
+            # -log(Freq(x) / Max_Freq)
+            ic = -math.log10(term_meta['observed_freq'] / self.max_freqs['observed_freq'])
+        # Lin
+        # Jiang & Conrath
+
+        ###########################################
+        #### FEATURE-BASED METRICS
+        ###########################################
+        # Tversky
+        # x-similarity
+        # Rodirguez
+
+        ###########################################
+        #### HYBRID METRICS
+        ###########################################
+        elif ic_type == 'seco' or ic_type == 'zhou': # SECO:: An intrinsic information content metric for semantic similarity in WordNet
+            #  1 - ( log(hypo(x) + 1) / log(max_nodes) )
+            ic = 1 - math.log10(term_meta['struct_freq']) / math.log10(len(self.terms))
+            if 'zhou': # New Model of Semantic Similarity Measuring in Wordnet                
+                # k*(IC_Seco(x)) + (1-k)*(log(depth(x))/log(max_depth))
+                self.ics['seco'][term] = ic # Special store
+                ic = zhou_k * ic + (1.0 - zhou_k) * (math.log10(term_meta['descendants']) / math.log10(self.max_freqs['max_depth']))
+        elif ic_type == 'sanchez': # Semantic similarity estimation in the biomedical domain: An ontology-basedinformation-theoretic perspective
+            ic = -math.log10((term_meta['descendants'] / term_meta['ancestors'] + 1.0) / (self.max_freqs['max_depth'] + 1.0))
+        # Knappe
         curr_ics[term] = ic
         return ic
 
     # Term vs Term #
 
     def get_LCA(self, termA, termB, lca_index = False):
         lca = []
@@ -478,24 +513,23 @@
     # ===== Returns 
     # the similarity between both sets or false if frequencies are not available yet
     def get_similarity(self, termA, termB, sim_type = 'resnik', ic_type = 'resnik', mica_index = False):
         if sim_type not in self.allowed_calcs['sims']: raise Exception(f"SIM type specified ({sim_type}) is not allowed") 
         sim = None
         mica, sim_res = self.get_MICA(termA, termB, ic_type, mica_index)
         if mica != None:
-            match sim_type:
-                case 'resnik':
-                    sim = sim_res
-                case 'lin':
-                    if termA == termB:
-                        sim = 1.0
-                    else:
-                        sim = (2.0 * sim_res) / (self.get_IC(termA, ic_type=ic_type) + self.get_IC(termB, ic_type=ic_type))
-                case 'jiang_conrath': # This is not a similarity, this is a disimilarity (distance)
-                    sim = (self.get_IC(termA, ic_type=ic_type) + self.get_IC(termB, ic_type=ic_type)) - (2.0 * sim_res)
+            if sim_type == 'resnik':
+                sim = sim_res
+            elif sim_type == 'lin':
+                if termA == termB:
+                    sim = 1.0
+                else:
+                    sim = (2.0 * sim_res) / (self.get_IC(termA, ic_type=ic_type) + self.get_IC(termB, ic_type=ic_type))
+            elif sim_type == 'jiang_conrath': # This is not a similarity, this is a disimilarity (distance)
+                sim = (self.get_IC(termA, ic_type=ic_type) + self.get_IC(termB, ic_type=ic_type)) - (2.0 * sim_res)
         return sim
 
     # Checking valid terms
     ####################################
 
     def term_exist(self, t_id):
         return t_id in self.terms
@@ -684,15 +718,15 @@
         if remove_alternatives: terms_without_ancestors, _ = self.remove_alternatives_from_profile(terms_without_ancestors) 
         return terms_without_ancestors
 
     def clean_profile_hard(self, profile, options = {}, remove_alternatives = True):
         profile, _ = self.check_ids(profile)
         profile = [ t for t in profile if not self.is_obsolete(t)] 
         if options.get('term_filter') != None: profile = [ term for term in profile if options['term_filter'] in self.get_ancestors(term) ] # keep terms with parents in term filter
-        profile = self.clean_profile(list(set(profile)), remove_alternatives)
+        profile = self.clean_profile(pxc.uniq(profile), remove_alternatives)
         return profile
 
     # Remove terms from a given profile using hierarchical info and scores set given  
     # ===== Parameters
     # +profile+:: profile to be cleaned
     # +scores+:: hash with terms by keys and numerical values (scores)
     # +byMax+:: if true, maximum scored term will be keeped, if false, minimum will be keeped
@@ -852,14 +886,27 @@
         if bidirectional:
             means_simA = means_sim * len(micasA)
             means_simB = self.compare(termsB, termsA, sim_type = sim_type, ic_type = ic_type, bidirectional = False, store_mica = store_mica) * len(termsB)
             means_sim = (means_simA + means_simB) / (len(termsA) + len(termsB))
         # Return
         return means_sim
 
+    def get_profile_similarities(self, terms, sim_type = 'resnik', ic_type = 'resnik', store_mica = False):
+        all_terms = copy.copy(terms)
+        sims = []
+        while len(all_terms) > 1:
+            t1 = all_terms.pop()
+            for t2 in all_terms:
+                if store_mica:
+                    value = self.sim_index[t1][t2]
+                else:
+                    value = self.get_similarity(t1, t2, sim_type = sim_type, ic_type = ic_type)
+                if type(value) is float: sims.append(value)
+        return np.mean(sims)
+
 
     #############################################
     # PROFILE INTERNAL METHODS 
     #############################################
 
     # I/O profiles
     ####################################
@@ -888,17 +935,21 @@
         if calc_metadata: self.get_items_from_profiles()
 
     # Stores a given profile with an specific ID. If ID is already assigend to a profile, it will be replaced
     # ===== Parameters
     # +id+:: assigned to profile
     # +terms+:: array of terms
     # +substitute+:: subsstitute flag from check_ids
-    def add_profile(self, pr_id, terms, substitute = True): # FRED: Talk with PSZ about the uniqness of IDs translated
-        if pr_id in self.profiles: warnings.warn(f"Profile assigned to ID ({pr_id}) is going to be replaced") 
-        correct_terms, rejected_terms = self.check_ids(terms, substitute = substitute)
+    def add_profile(self, pr_id, terms, substitute = True, clean_hard=False, options={}): # FRED: Talk with PSZ about the uniqness of IDs translated
+        if pr_id in self.profiles: warnings.warn(f"Profile assigned to ID ({pr_id}) is going to be replaced")
+        if clean_hard:
+            correct_terms = self.clean_profile_hard(terms, options=options)
+            rejected_terms = []
+        else:
+            correct_terms, rejected_terms = self.check_ids(terms, substitute = substitute)
         if len(rejected_terms) > 0: warnings.warn(f"Given terms contains erroneus IDs: {','.join(rejected_terms)}. These IDs will be removed")
         self.profiles[pr_id] = correct_terms              
 
 
     # Includes as "observed_terms" all terms included into stored profiles
     # ===== Parameters
     # +reset+:: if true, reset observed freqs alreeady stored befor re-calculate
@@ -971,27 +1022,15 @@
             profs_names[pr_id] = names
         return  list(profs_names.values()) if asArray else profs_names
 
     # Description of profile size
     ####################################
 
     def profile_stats(self):
-        stats = {}
-        data = np.array(self.get_profiles_sizes())
-        stats["average"] = np.mean(data)
-        stats["variance"] = np.var(data)
-        stats["standardDeviation"] = np.std(data)
-        stats["max"] = data.max()
-        stats["min"] = data.min()
-        stats["count"] = len(data)
-        stats["countNonZero"] = len([non_zero_element for non_zero_element in data if non_zero_element != 0])
-        stats["q1"] = np.quantile(data, 0.25)
-        stats["median"] = np.quantile(data, 0.5)
-        stats["q3"] = np.quantile(data, 0.75)
-        return stats
+        return list(pxc.get_stats_from_list(self.get_profiles_sizes()))
 
     # ===== Returns 
     # mean size of stored profiles
     # ===== Parameters
     # +round_digits+:: number of digits to round result. Default: 4
     # ===== Returns 
     # mean size of stored profiles
@@ -1179,14 +1218,25 @@
             for curr_id, current_profile in main_profiles.items():
                 for t_id, profile in comp_profiles.items():
                     value = self.compare(current_profile, profile, sim_type = sim_type, ic_type = ic_type, bidirectional = bidirectional, store_mica = True)
                     self.add2nestHash(profiles_similarity, curr_id, t_id, value)
         #print(f"similarity: {time.time() - start}")
         return profiles_similarity
 
+    def get_profile_similarities_from_profiles(self, sim_type = 'resnik', ic_type = 'resnik'):
+        profiles_similarity = {}
+        pair_index = self.get_pair_index(self.profiles, self.profiles, same_profiles=True)
+        self.mica_index = defaultdict(lambda: dict())
+        self.sim_index = defaultdict(lambda: dict())
+        self.get_mica_index_from_profiles(pair_index, ic_type = ic_type, sim_type=sim_type)
+        for t_id, prof in self.profiles.items():
+            sim = self.get_profile_similarities(prof, sim_type = sim_type, ic_type = ic_type, store_mica = True)
+            profiles_similarity[t_id] = 1 if (np.isnan(sim) and len(prof) == 1) else sim
+        return profiles_similarity
+
     # specifity_index related methods
     ####################################
 
     # Return ontology levels from profile terms
     # ===== Returns 
     # hash of term levels (Key: level; Value: array of term IDs)
     def get_ontology_levels_from_profiles(self, uniq = True):
@@ -1268,15 +1318,45 @@
         if len(highSection) == 0:
             dsi = 0
         else:
             hss = self.get_weigthed_level_contribution(highSection, maxL, len(ontology_levels) - maxL)
             lss = self.get_weigthed_level_contribution(lowSection, maxL, maxL)
             dsi = hss / lss
         return dsi
- 
+
+    ########################################
+    ## INTERNET QUERY METHODS
+    ######################################## 
+    def query_ncbi(self, db): # Due a hardcoded limit in NCBI API we only can retrieve 10000 records. To download the complete dataset, we need the E-Direct tools. Install from https://www.ncbi.nlm.nih.gov/books/NBK179288/ and add detection and implementation
+        #import entrezpy.log.logger
+        #entrezpy.log.logger.set_level('DEBUG')
+        count = 0
+        ont_term_res = {}
+        for t_id, tags in self.each(att = True):
+            if count == 1000: break
+            name = tags['name']
+            syns = self.get_synonims(t_id)
+            strings = [name]
+            if len(syns) > 0:
+                strings.extend(syns)
+                strings = list(set(strings))
+            query = ' OR '.join(strings)
+            es = entrezpy.esearch.esearcher.Esearcher('esearcher', 'mail', threads=1)
+            #es.requests_per_sec = 2
+            es.num_threads = 1
+            a = es.inquire({'db': db,'term':query, 'retmax': 10000, 'rettype': 'uilist'})
+            count += 1
+            if a != None: 
+                result = a.get_result().uids
+                a.result = None # This resets class/object to avoid the bug of result aggregation from one query to other
+                print(f"{t_id} => {len(result)}")
+                if len(result) > 0 : ont_term_res[t_id] = [strings, result]
+        return ont_term_res
+
+
     ########################################
     ## GENERAL ONTOLOGY METHODS
     ########################################
     def __eq__(self, other):
         if isinstance(other, Ontology):
             res = self.terms == other.terms and \
                 self.ancestors_index == other.ancestors_index and \
@@ -1341,14 +1421,34 @@
         roots = [ term for term in self.each() if self.ancestors_index.get(term) == None]
         return roots
 
     def list_term_attributes(self):
         terms = [ [term, self.translate_id(term), self.get_term_level(term)] for term in self.each()]
         return terms
 
+    def return_terms_by_keyword_match(self, keyword, fields = ['name', 'synonym', 'def']):
+        terms = []
+        query_kwd = re.compile(keyword, re.IGNORECASE)
+        for term, attrs in self.each(att=True):
+            breakit = False
+            for field in fields:
+                if breakit == True: break
+                if attrs.get(field):
+                    if type(attrs[field]) == str:
+                        if re.search(query_kwd, attrs[field]):
+                            terms.append(term)
+                            break
+                    elif type(attrs[field]) == list:
+                        for subfield in attrs[field]:
+                            if re.search(query_kwd, subfield):
+                                terms.append(term)
+                                breakit = True
+                                break
+        return terms
+    
     # Gets ontology levels calculated
     # ===== Returns 
     # ontology levels calculated
     def get_ontology_levels(self):
         return copy.copy(self.dicts['level']['byTerm']) # By term, in this case, is Key::Level, Value::Terms
 
     ########################################
```

### Comparing `py_semtools-1.0.0/src/py_semtools/sim_handler.py` & `py_semtools-1.0.1/src/py_semtools/sim_handler.py`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/src/py_semtools.egg-info/PKG-INFO` & `py_semtools-1.0.1/src/py_semtools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
-Name: py-semtools
-Version: 1.0.0
+Name: py_semtools
+Version: 1.0.1
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: seoanezonjic
 Author-email: darklordsone@hotmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: platformdirs
 Requires-Dist: numpy
 Requires-Dist: networkx
+Requires-Dist: entrezpy
 Requires-Dist: scipy
+Requires-Dist: sentence_transformers
+Requires-Dist: requests
 Requires-Dist: py_exp_calc
+Requires-Dist: py_cmdtabs
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
```

### Comparing `py_semtools-1.0.0/tests/data/go-basic_sample.obo` & `py_semtools-1.0.1/tests/data/go-basic_sample.obo`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/tests/data/go-onlyOne.obo` & `py_semtools-1.0.1/tests/data/go-onlyOne.obo`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/tests/data/partial_go.json` & `py_semtools-1.0.1/tests/data/partial_go.json`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/tests/data/partial_go.obo` & `py_semtools-1.0.1/tests/data/partial_go.obo`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/tests/test_go.py` & `py_semtools-1.0.1/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/tests/test_jsonparser.py` & `py_semtools-1.0.1/tests/test_jsonparser.py`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/tests/test_oboparser.py` & `py_semtools-1.0.1/tests/test_oboparser.py`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/tests/test_ontology.py` & `py_semtools-1.0.1/tests/test_ontology.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,23 +441,24 @@
     ####################################
     
     def test_description_profile_size(self):
         self.hierarchical.add_profile("A", ["Child2", "Parental"], substitute= False) # Add profiles
         self.hierarchical.add_profile("B", ["Child2", "Parental", "FakeID"], substitute= False)
         self.hierarchical.add_profile("C", ["Child2", "Parental"], substitute= False)
         self.hierarchical.add_profile("D", ["Parental"], substitute= False)
-
+        expected_stats = [['Elements', '4'], ['Elements Non Zero', '4'], ['Non Zero Density', '1.0'], 
+         ['Max', '2'], ['Min', '1'], ['Average', '1.75'], 
+         ['Variance', '0.1875'], ['Standard Deviation', '0.4330127018922193'], ['Q1', '1.75'], 
+         ['Median', '2.0'], ['Q3', '2.0'], ['Min Non Zero', '1'],
+         ['Average Non Zero', '1.75'], ['Variance Non Zero', '0.1875'], ['Standard Deviation Non Zero', '0.4330127018922193'],
+         ['Q1 Non Zero', '1.75'], ['Median Non Zero', '2.0'], ['Q3 Non Zero', '2.0']]
         # Getiings
         self.assertEqual([2, 2, 2, 1], self.hierarchical.get_profiles_sizes()) # Check metadata
         self.assertEqual(round(7 /4.0, 4), self.hierarchical.get_profiles_mean_size())
-        self.assertEqual({"average": 1.75, 
-                      "variance": 0.1875,
-                      "standardDeviation": math.sqrt(0.1875), 
-                      "max": 2, "min": 1, "count": 4, "countNonZero": 4, 
-                      "q1": 1.75, "median": 2.0, "q3": 2.0}, self.hierarchical.profile_stats())
+        self.assertEqual(expected_stats, self.hierarchical.profile_stats())
         self.assertEqual(1, self.hierarchical.get_profile_length_at_percentile(0, increasing_sort= True))
         self.assertEqual(2, self.hierarchical.get_profile_length_at_percentile(2.0 / (4 - 1) * 100, increasing_sort= True))
         self.assertEqual(2, self.hierarchical.get_profile_length_at_percentile(3.0 / (4 - 1) * 100, increasing_sort= True))
         self.assertEqual(1, self.hierarchical.get_profile_length_at_percentile(4.0 / (5 - 1) * 100, increasing_sort= False))
 
     def test_parentals_per_profile(self):
         self.sparse.precompute()
@@ -629,15 +630,31 @@
         ###########################
         ## NOW INCLUDING NOT STORED TERMS
         ###########################
         initial_items = {"Child1": ["branchAChild1"], "Child2": ["branchAChild2", "branchB"]}
         onto_notroot_items = {"root": ["branchA"], "Child1": ["branchAChild1"], "Child2": ["branchAChild2", "branchB"]}
         self.short_hierarchical.load_item_relations_to_terms(initial_items, True)
         self.short_hierarchical.expand_items_to_parentals(ontology= self.enrichment_hierarchical, clean_profiles= False)
-        self.assertEqual(onto_notroot_items, self.short_hierarchical.items)		
+        self.assertEqual(onto_notroot_items, self.short_hierarchical.items)
+
+    def test_return_terms_by_keyword_match(self):
+        expected = ["Child2"]
+        returned = self.hierarchical.return_terms_by_keyword_match("Child", fields = ['name'])
+        returned2 = self.hierarchical.return_terms_by_keyword_match("Child", fields = ['name', 'name']) #Checking that no duplicated terms are returned even if the fields parameter is duplicated
+        returned3 = self.hierarchical.return_terms_by_keyword_match("mannosyltransferase", fields = ['name', 'synonym'])
+        returned4 = self.hierarchical.return_terms_by_keyword_match("mannosyltransferase", fields = ['name', 'synonym', 'synonym']) #Checking that no duplicated terms are returned even if the fields parameter is duplicated
+        self.assertEqual(expected, returned)
+        self.assertEqual(expected, returned2)
+        self.assertEqual(expected, returned3)
+        self.assertEqual(expected, returned4)
+
+        expected = ["branchA", "branchAChild1", "branchAChild2", "branchB"]
+        returned = self.enrichment_hierarchical.return_terms_by_keyword_match("Child", fields = ['name'])
+        self.assertEqual(expected, returned)
+
 
     #################################
     # AUXILIAR METHODS
     #################################
 
     def test_auxiliar_methods(self):
         self.hierarchical.precompute()
```

### Comparing `py_semtools-1.0.0/tests/test_similitudes.py` & `py_semtools-1.0.1/tests/test_similitudes.py`

 * *Files identical despite different names*

### Comparing `py_semtools-1.0.0/tox.ini` & `py_semtools-1.0.1/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 [tox]
 minversion = 3.24
 envlist = default
 isolated_build = True
 
 
 [testenv]
+sitepackages = True
 description = Invoke pytest to run automated tests
 setenv =
     TOXINIDIR = {toxinidir}
 passenv =
     HOME
     SETUPTOOLS_*
+allowlist_externals = 
+    rm
 extras =
     testing
 commands =
-    pytest {posargs}
-
+    python -m pytest {posargs}
+    rm -rf {toxinidir}/.tox/.tmp/package/
 
 # # To run `tox -e lint` you need to make sure you have a
 # # `.pre-commit-config.yaml` file. See https://pre-commit.com
 # [testenv:lint]
 # description = Perform static analysis and style checks
 # skip_install = True
 # deps = pre-commit
```

