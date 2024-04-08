# Comparing `tmp/reuse-3.0.1.tar.gz` & `tmp/reuse-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reuse-3.0.1.tar", max compression
+gzip compressed data, was "reuse-3.0.2.tar", max compression
```

## Comparing `reuse-3.0.1.tar` & `reuse-3.0.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     1154 2024-01-04 15:30:14.388230 reuse-3.0.1/.reuse/dep5
--rw-r--r--   0        0        0     1976 2024-01-16 15:40:22.239153 reuse-3.0.1/AUTHORS.rst
--rw-r--r--   0        0        0    35793 2024-01-19 12:33:53.876710 reuse-3.0.1/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2023-02-16 14:35:33.434942 reuse-3.0.1/LICENSES/
--rw-r--r--   0        0        0    11358 2022-01-24 22:16:23.685080 reuse-3.0.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    20131 2022-01-24 22:16:23.685080 reuse-3.0.1/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2022-01-24 22:16:23.686081 reuse-3.0.1/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0    35149 2022-01-24 22:16:23.686081 reuse-3.0.1/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     9960 2024-01-19 12:33:04.572494 reuse-3.0.1/README.md
--rw-r--r--   0        0        0     2173 2023-10-24 11:40:39.056621 reuse-3.0.1/_build.py
--rw-r--r--   0        0        0      712 2022-12-01 13:56:24.815249 reuse-3.0.1/docs/Makefile
--rw-r--r--   0        0        0        0 2022-01-24 22:16:23.686081 reuse-3.0.1/docs/_static/.gitkeep
--rw-r--r--   0        0        0      164 2022-01-24 22:16:23.686081 reuse-3.0.1/docs/authors.rst
--rw-r--r--   0        0        0     5990 2024-01-19 12:33:04.572494 reuse-3.0.1/docs/conf.py
--rw-r--r--   0        0        0      643 2023-05-21 13:26:14.034019 reuse-3.0.1/docs/index.rst
--rw-r--r--   0        0        0     2807 2023-11-09 08:52:59.359030 reuse-3.0.1/docs/requirements.txt
--rw-r--r--   0        0        0      124 2023-05-21 13:26:14.034019 reuse-3.0.1/docs/requirements.txt.license
--rw-r--r--   0        0        0     5608 2023-07-22 17:18:59.500349 reuse-3.0.1/docs/reuse-r-only.svg
--rw-r--r--   0        0        0      105 2023-07-22 17:18:59.500349 reuse-3.0.1/docs/reuse-r-only.svg.license
--rw-r--r--   0        0        0     5776 2022-12-01 14:07:09.243154 reuse-3.0.1/docs/scripts.rst
--rw-r--r--   0        0        0    12618 2024-01-04 15:30:14.392230 reuse-3.0.1/docs/usage.rst
--rw-r--r--   0        0        0      192 2022-01-24 22:16:23.687080 reuse-3.0.1/docs/usage.rst.license
--rw-r--r--   0        0        0      331 2024-01-04 15:30:14.392230 reuse-3.0.1/po/POTFILES.in
--rw-r--r--   0        0        0    33637 2024-01-19 12:33:00.320474 reuse-3.0.1/po/cs.po
--rw-r--r--   0        0        0    34682 2024-01-19 12:33:00.320474 reuse-3.0.1/po/de.po
--rw-r--r--   0        0        0    34960 2024-01-19 12:33:00.320474 reuse-3.0.1/po/eo.po
--rw-r--r--   0        0        0    42852 2024-01-19 12:33:00.320474 reuse-3.0.1/po/es.po
--rw-r--r--   0        0        0    35937 2024-01-19 12:33:00.320474 reuse-3.0.1/po/fr.po
--rw-r--r--   0        0        0    30278 2024-01-19 12:33:00.324474 reuse-3.0.1/po/gl.po
--rw-r--r--   0        0        0    30776 2024-01-19 12:33:00.324474 reuse-3.0.1/po/it.po
--rw-r--r--   0        0        0    35074 2024-01-19 12:33:00.324474 reuse-3.0.1/po/nl.po
--rw-r--r--   0        0        0    30884 2024-01-19 12:33:00.324474 reuse-3.0.1/po/pt.po
--rw-r--r--   0        0        0    20275 2024-01-19 12:33:00.324474 reuse-3.0.1/po/reuse.pot
--rw-r--r--   0        0        0      108 2023-05-21 13:26:14.040020 reuse-3.0.1/po/reuse.pot.license
--rw-r--r--   0        0        0    21560 2024-01-19 12:33:00.324474 reuse-3.0.1/po/sv.po
--rw-r--r--   0        0        0    34185 2024-01-19 12:33:00.324474 reuse-3.0.1/po/tr.po
--rw-r--r--   0        0        0    46172 2024-01-19 12:33:00.324474 reuse-3.0.1/po/uk.po
--rw-r--r--   0        0        0     3312 2024-01-19 12:33:04.572494 reuse-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     6181 2024-01-19 12:33:04.572494 reuse-3.0.1/src/reuse/__init__.py
--rw-r--r--   0        0        0      254 2023-10-24 14:05:05.807274 reuse-3.0.1/src/reuse/__main__.py
--rw-r--r--   0        0        0    17024 2023-11-28 08:02:43.136106 reuse-3.0.1/src/reuse/_annotate.py
--rw-r--r--   0        0        0     1358 2023-10-24 11:40:39.060621 reuse-3.0.1/src/reuse/_format.py
--rw-r--r--   0        0        0     2162 2024-01-17 13:04:07.431669 reuse-3.0.1/src/reuse/_licenses.py
--rw-r--r--   0        0        0    10568 2024-01-04 15:30:14.396230 reuse-3.0.1/src/reuse/_main.py
--rw-r--r--   0        0        0    20629 2024-01-19 12:33:00.324474 reuse-3.0.1/src/reuse/_util.py
--rw-r--r--   0        0        0    26990 2024-01-19 12:33:00.324474 reuse-3.0.1/src/reuse/comment.py
--rw-r--r--   0        0        0     6708 2023-10-24 20:07:13.217273 reuse-3.0.1/src/reuse/download.py
--rw-r--r--   0        0        0    10884 2023-10-24 20:07:13.217273 reuse-3.0.1/src/reuse/header.py
--rw-r--r--   0        0        0     4641 2023-10-24 20:07:13.217273 reuse-3.0.1/src/reuse/init.py
--rw-r--r--   0        0        0     9094 2024-01-04 15:30:14.396230 reuse-3.0.1/src/reuse/lint.py
--rw-r--r--   0        0        0    17355 2024-01-19 12:33:00.324474 reuse-3.0.1/src/reuse/project.py
--rw-r--r--   0        0        0      122 2023-10-24 11:40:39.060621 reuse-3.0.1/src/reuse/py.typed
--rw-r--r--   0        0        0    24819 2024-01-04 15:30:14.396230 reuse-3.0.1/src/reuse/report.py
--rw-r--r--   0        0        0    26498 2023-11-28 08:02:43.140106 reuse-3.0.1/src/reuse/resources/exceptions.json
--rw-r--r--   0        0        0      100 2022-01-24 22:16:23.695081 reuse-3.0.1/src/reuse/resources/exceptions.json.license
--rw-r--r--   0        0        0   270608 2023-11-28 08:02:43.140106 reuse-3.0.1/src/reuse/resources/licenses.json
--rw-r--r--   0        0        0      100 2022-01-24 22:16:23.697080 reuse-3.0.1/src/reuse/resources/licenses.json.license
--rw-r--r--   0        0        0     3132 2023-10-24 11:40:39.064621 reuse-3.0.1/src/reuse/spdx.py
--rw-r--r--   0        0        0     1040 2023-10-24 11:40:39.064621 reuse-3.0.1/src/reuse/supported_licenses.py
--rw-r--r--   0        0        0      281 2023-10-24 11:40:39.064621 reuse-3.0.1/src/reuse/templates/default_template.jinja2
--rw-r--r--   0        0        0      119 2022-01-24 22:16:23.697080 reuse-3.0.1/src/reuse/templates/default_template.jinja2.license
--rw-r--r--   0        0        0    10545 2023-11-28 08:02:43.140106 reuse-3.0.1/src/reuse/vcs.py
--rw-r--r--   0        0        0    12757 2024-01-04 15:30:14.396230 reuse-3.0.1/tests/conftest.py
--rw-r--r--   0        0        0      215 2024-01-04 15:30:14.400230 reuse-3.0.1/tests/resources/fake_repository/.reuse/dep5
--rw-r--r--   0        0        0       14 2023-07-22 17:18:59.516349 reuse-3.0.1/tests/resources/fake_repository/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0       14 2022-01-24 22:16:23.698080 reuse-3.0.1/tests/resources/fake_repository/LICENSES/Autoconf-exception-3.0.txt
--rw-r--r--   0        0        0       13 2022-01-24 22:16:23.698080 reuse-3.0.1/tests/resources/fake_repository/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0       13 2022-01-24 22:16:23.698080 reuse-3.0.1/tests/resources/fake_repository/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0        0 2022-01-24 22:16:23.698080 reuse-3.0.1/tests/resources/fake_repository/LICENSES/LicenseRef-custom.txt
--rw-r--r--   0        0        0       14 2024-01-04 15:30:14.400230 reuse-3.0.1/tests/resources/fake_repository/doc/index.rst
--rw-r--r--   0        0        0       58 2022-07-04 08:15:44.248468 reuse-3.0.1/tests/resources/fake_repository/src/custom.py
--rw-r--r--   0        0        0       58 2022-07-04 08:15:44.248468 reuse-3.0.1/tests/resources/fake_repository/src/exception.py
--rw-r--r--   0        0        0       59 2023-07-22 17:18:59.516349 reuse-3.0.1/tests/resources/fake_repository/src/multiple_licenses.rs
--rw-r--r--   0        0        0      156 2022-07-04 08:15:39.772434 reuse-3.0.1/tests/resources/fake_repository/src/source_code.c
--rw-r--r--   0        0        0      111 2022-07-04 08:15:44.249468 reuse-3.0.1/tests/resources/fake_repository/src/source_code.html
--rw-r--r--   0        0        0      109 2022-07-04 08:15:44.249468 reuse-3.0.1/tests/resources/fake_repository/src/source_code.jinja2
--rw-r--r--   0        0        0      166 2022-07-04 08:15:39.772434 reuse-3.0.1/tests/resources/fake_repository/src/source_code.py
--rw-r--r--   0        0        0     5450 2022-01-24 22:16:23.699081 reuse-3.0.1/tests/resources/fsfe.png
--rw-r--r--   0        0        0    14907 2024-01-17 13:04:07.431669 reuse-3.0.1/tests/test_comment.py
--rw-r--r--   0        0        0     3316 2023-10-24 11:40:39.064621 reuse-3.0.1/tests/test_core.py
--rw-r--r--   0        0        0     5308 2023-10-24 20:07:13.221273 reuse-3.0.1/tests/test_download.py
--rw-r--r--   0        0        0    10656 2023-10-24 11:40:39.064621 reuse-3.0.1/tests/test_header.py
--rw-r--r--   0        0        0     7577 2024-01-04 15:30:14.400230 reuse-3.0.1/tests/test_lint.py
--rw-r--r--   0        0        0    17257 2024-01-04 15:30:14.400230 reuse-3.0.1/tests/test_main.py
--rw-r--r--   0        0        0    37529 2024-01-17 13:04:07.431669 reuse-3.0.1/tests/test_main_annotate.py
--rw-r--r--   0        0        0     4597 2024-01-16 15:40:00.138913 reuse-3.0.1/tests/test_main_annotate_merge.py
--rw-r--r--   0        0        0    17237 2024-01-19 12:33:00.324474 reuse-3.0.1/tests/test_project.py
--rw-r--r--   0        0        0    15136 2024-01-04 15:30:14.400230 reuse-3.0.1/tests/test_report.py
--rw-r--r--   0        0        0    21824 2024-01-04 15:30:14.400230 reuse-3.0.1/tests/test_util.py
--rw-r--r--   0        0        0     1177 2023-11-28 08:02:43.144106 reuse-3.0.1/tests/test_vcs.py
--rw-r--r--   0        0        0    11450 1970-01-01 00:00:00.000000 reuse-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1154 2024-04-08 07:43:15.556065 reuse-3.0.2/.reuse/dep5
+-rw-r--r--   0        0        0     1976 2024-01-30 10:33:51.757472 reuse-3.0.2/AUTHORS.rst
+-rw-r--r--   0        0        0    35932 2024-04-08 07:56:57.875292 reuse-3.0.2/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2024-02-03 11:42:02.344180 reuse-3.0.2/LICENSES/
+-rw-r--r--   0        0        0    11358 2022-01-24 22:16:23.685080 reuse-3.0.2/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    20131 2022-01-24 22:16:23.685080 reuse-3.0.2/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2022-01-24 22:16:23.686081 reuse-3.0.2/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    35149 2022-01-24 22:16:23.686081 reuse-3.0.2/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     9960 2024-04-08 08:03:56.292397 reuse-3.0.2/README.md
+-rw-r--r--   0        0        0     2173 2024-01-30 10:33:51.761472 reuse-3.0.2/_build.py
+-rw-r--r--   0        0        0      712 2024-01-30 10:33:51.761472 reuse-3.0.2/docs/Makefile
+-rw-r--r--   0        0        0        0 2022-01-24 22:16:23.686081 reuse-3.0.2/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      164 2024-01-30 10:33:51.761472 reuse-3.0.2/docs/authors.rst
+-rw-r--r--   0        0        0     5990 2024-04-08 08:03:56.292397 reuse-3.0.2/docs/conf.py
+-rw-r--r--   0        0        0      643 2024-01-30 10:33:51.761472 reuse-3.0.2/docs/index.rst
+-rw-r--r--   0        0        0     2807 2023-11-09 08:52:59.359030 reuse-3.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0      124 2024-01-30 10:33:51.761472 reuse-3.0.2/docs/requirements.txt.license
+-rw-r--r--   0        0        0     5608 2023-07-22 17:18:59.500349 reuse-3.0.2/docs/reuse-r-only.svg
+-rw-r--r--   0        0        0      105 2024-01-30 10:33:51.761472 reuse-3.0.2/docs/reuse-r-only.svg.license
+-rw-r--r--   0        0        0     5776 2024-01-30 10:33:51.761472 reuse-3.0.2/docs/scripts.rst
+-rw-r--r--   0        0        0    12618 2024-04-08 07:43:15.556065 reuse-3.0.2/docs/usage.rst
+-rw-r--r--   0        0        0      192 2024-01-30 10:33:51.761472 reuse-3.0.2/docs/usage.rst.license
+-rw-r--r--   0        0        0      331 2024-04-08 07:43:15.556065 reuse-3.0.2/po/POTFILES.in
+-rw-r--r--   0        0        0    33637 2024-01-30 10:33:51.761472 reuse-3.0.2/po/cs.po
+-rw-r--r--   0        0        0    34682 2024-01-30 10:33:51.761472 reuse-3.0.2/po/de.po
+-rw-r--r--   0        0        0    34960 2024-01-30 10:33:51.761472 reuse-3.0.2/po/eo.po
+-rw-r--r--   0        0        0    42852 2024-04-08 07:52:23.411349 reuse-3.0.2/po/es.po
+-rw-r--r--   0        0        0    35937 2024-01-30 10:33:51.765472 reuse-3.0.2/po/fr.po
+-rw-r--r--   0        0        0    30278 2024-01-30 10:33:51.765472 reuse-3.0.2/po/gl.po
+-rw-r--r--   0        0        0    30776 2024-01-30 10:33:51.765472 reuse-3.0.2/po/it.po
+-rw-r--r--   0        0        0    35074 2024-01-30 10:33:51.765472 reuse-3.0.2/po/nl.po
+-rw-r--r--   0        0        0    30884 2024-01-30 10:33:51.765472 reuse-3.0.2/po/pt.po
+-rw-r--r--   0        0        0    20275 2024-01-19 13:14:00.612839 reuse-3.0.2/po/reuse.pot
+-rw-r--r--   0        0        0      108 2024-01-30 10:33:51.765472 reuse-3.0.2/po/reuse.pot.license
+-rw-r--r--   0        0        0    21560 2024-01-30 10:33:51.765472 reuse-3.0.2/po/sv.po
+-rw-r--r--   0        0        0    34185 2024-01-30 10:33:51.765472 reuse-3.0.2/po/tr.po
+-rw-r--r--   0        0        0    46172 2024-04-08 07:52:23.411349 reuse-3.0.2/po/uk.po
+-rw-r--r--   0        0        0     3312 2024-04-08 08:03:56.288397 reuse-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6181 2024-04-08 08:03:56.288397 reuse-3.0.2/src/reuse/__init__.py
+-rw-r--r--   0        0        0      254 2024-01-30 10:33:51.765472 reuse-3.0.2/src/reuse/__main__.py
+-rw-r--r--   0        0        0    17086 2024-04-08 07:52:38.225075 reuse-3.0.2/src/reuse/_annotate.py
+-rw-r--r--   0        0        0     1358 2024-01-30 10:33:51.769472 reuse-3.0.2/src/reuse/_format.py
+-rw-r--r--   0        0        0     2162 2024-01-30 10:33:51.769472 reuse-3.0.2/src/reuse/_licenses.py
+-rw-r--r--   0        0        0    10568 2024-04-08 07:43:15.560066 reuse-3.0.2/src/reuse/_main.py
+-rw-r--r--   0        0        0    20629 2024-04-08 07:43:15.560066 reuse-3.0.2/src/reuse/_util.py
+-rw-r--r--   0        0        0    26990 2024-02-14 07:45:39.082657 reuse-3.0.2/src/reuse/comment.py
+-rw-r--r--   0        0        0     6708 2024-01-30 10:33:51.769472 reuse-3.0.2/src/reuse/download.py
+-rw-r--r--   0        0        0    10884 2024-01-30 10:33:51.769472 reuse-3.0.2/src/reuse/header.py
+-rw-r--r--   0        0        0     4641 2024-01-30 10:33:51.769472 reuse-3.0.2/src/reuse/init.py
+-rw-r--r--   0        0        0     9094 2024-04-08 07:43:15.560066 reuse-3.0.2/src/reuse/lint.py
+-rw-r--r--   0        0        0    17355 2024-04-08 07:43:15.564066 reuse-3.0.2/src/reuse/project.py
+-rw-r--r--   0        0        0      122 2023-10-24 11:40:39.060621 reuse-3.0.2/src/reuse/py.typed
+-rw-r--r--   0        0        0    24819 2024-04-08 07:43:15.564066 reuse-3.0.2/src/reuse/report.py
+-rw-r--r--   0        0        0    26498 2024-04-08 07:45:27.461302 reuse-3.0.2/src/reuse/resources/exceptions.json
+-rw-r--r--   0        0        0      100 2024-01-30 10:33:51.769472 reuse-3.0.2/src/reuse/resources/exceptions.json.license
+-rw-r--r--   0        0        0   270608 2024-04-08 07:45:27.461302 reuse-3.0.2/src/reuse/resources/licenses.json
+-rw-r--r--   0        0        0      100 2024-01-30 10:33:51.769472 reuse-3.0.2/src/reuse/resources/licenses.json.license
+-rw-r--r--   0        0        0     3132 2024-01-30 10:33:51.769472 reuse-3.0.2/src/reuse/spdx.py
+-rw-r--r--   0        0        0     1040 2024-01-30 10:33:51.769472 reuse-3.0.2/src/reuse/supported_licenses.py
+-rw-r--r--   0        0        0      281 2023-10-24 11:40:39.064621 reuse-3.0.2/src/reuse/templates/default_template.jinja2
+-rw-r--r--   0        0        0      119 2024-01-30 10:33:51.769472 reuse-3.0.2/src/reuse/templates/default_template.jinja2.license
+-rw-r--r--   0        0        0    10545 2024-01-30 10:33:51.769472 reuse-3.0.2/src/reuse/vcs.py
+-rw-r--r--   0        0        0    12757 2024-04-08 07:43:15.564066 reuse-3.0.2/tests/conftest.py
+-rw-r--r--   0        0        0      215 2024-04-08 07:43:15.564066 reuse-3.0.2/tests/resources/fake_repository/.reuse/dep5
+-rw-r--r--   0        0        0       14 2023-07-22 17:18:59.516349 reuse-3.0.2/tests/resources/fake_repository/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0       14 2022-01-24 22:16:23.698080 reuse-3.0.2/tests/resources/fake_repository/LICENSES/Autoconf-exception-3.0.txt
+-rw-r--r--   0        0        0       13 2022-01-24 22:16:23.698080 reuse-3.0.2/tests/resources/fake_repository/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0       13 2022-01-24 22:16:23.698080 reuse-3.0.2/tests/resources/fake_repository/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0        0 2022-01-24 22:16:23.698080 reuse-3.0.2/tests/resources/fake_repository/LICENSES/LicenseRef-custom.txt
+-rw-r--r--   0        0        0       14 2024-04-08 07:43:15.568066 reuse-3.0.2/tests/resources/fake_repository/doc/index.rst
+-rw-r--r--   0        0        0       58 2024-01-30 10:33:51.769472 reuse-3.0.2/tests/resources/fake_repository/src/custom.py
+-rw-r--r--   0        0        0       58 2024-01-30 10:33:51.769472 reuse-3.0.2/tests/resources/fake_repository/src/exception.py
+-rw-r--r--   0        0        0       59 2024-01-30 10:33:51.769472 reuse-3.0.2/tests/resources/fake_repository/src/multiple_licenses.rs
+-rw-r--r--   0        0        0      156 2024-01-30 10:33:51.769472 reuse-3.0.2/tests/resources/fake_repository/src/source_code.c
+-rw-r--r--   0        0        0      111 2024-01-30 10:33:51.769472 reuse-3.0.2/tests/resources/fake_repository/src/source_code.html
+-rw-r--r--   0        0        0      109 2024-01-30 10:33:51.769472 reuse-3.0.2/tests/resources/fake_repository/src/source_code.jinja2
+-rw-r--r--   0        0        0      166 2024-01-30 10:33:51.769472 reuse-3.0.2/tests/resources/fake_repository/src/source_code.py
+-rw-r--r--   0        0        0     5450 2022-01-24 22:16:23.699081 reuse-3.0.2/tests/resources/fsfe.png
+-rw-r--r--   0        0        0    14907 2024-01-30 10:33:51.769472 reuse-3.0.2/tests/test_comment.py
+-rw-r--r--   0        0        0     3316 2024-04-08 07:43:15.568066 reuse-3.0.2/tests/test_core.py
+-rw-r--r--   0        0        0     5308 2024-01-30 10:33:51.769472 reuse-3.0.2/tests/test_download.py
+-rw-r--r--   0        0        0    10656 2024-01-30 10:33:51.773472 reuse-3.0.2/tests/test_header.py
+-rw-r--r--   0        0        0     7577 2024-04-08 07:43:15.568066 reuse-3.0.2/tests/test_lint.py
+-rw-r--r--   0        0        0    17257 2024-04-08 07:43:15.568066 reuse-3.0.2/tests/test_main.py
+-rw-r--r--   0        0        0    38105 2024-04-08 07:52:38.225075 reuse-3.0.2/tests/test_main_annotate.py
+-rw-r--r--   0        0        0     4597 2024-01-30 10:33:51.773472 reuse-3.0.2/tests/test_main_annotate_merge.py
+-rw-r--r--   0        0        0    17237 2024-04-08 07:43:15.568066 reuse-3.0.2/tests/test_project.py
+-rw-r--r--   0        0        0    15136 2024-04-08 07:43:15.568066 reuse-3.0.2/tests/test_report.py
+-rw-r--r--   0        0        0    21824 2024-04-08 07:43:15.572066 reuse-3.0.2/tests/test_util.py
+-rw-r--r--   0        0        0     1177 2024-01-30 10:33:51.773472 reuse-3.0.2/tests/test_vcs.py
+-rw-r--r--   0        0        0    11450 1970-01-01 00:00:00.000000 reuse-3.0.2/PKG-INFO
```

### Comparing `reuse-3.0.1/.reuse/dep5` & `reuse-3.0.2/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/AUTHORS.rst` & `reuse-3.0.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/CHANGELOG.md` & `reuse-3.0.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,21 @@
 ### Removed
 
 ### Fixed
 
 ### Security
 -->
 
+## 3.0.2 - 2024-04-08
+
+### Fixed
+
+- `annotate`'s '`--style` now works again when used for a file with an
+  unrecognised extension. (#909)
+
 ## 3.0.1 - 2024-01-19
 
 ### Fixed
 
 - `.qrc` and `.ui` now have the HTML comment style instead of being marked
   uncommentable. (#896)
 - This reverts behaviour introduced in v3.0.0: the contents of uncommentable
```

### Comparing `reuse-3.0.1/LICENSES/Apache-2.0.txt` & `reuse-3.0.2/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/LICENSES/CC-BY-SA-4.0.txt` & `reuse-3.0.2/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/LICENSES/CC0-1.0.txt` & `reuse-3.0.2/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/LICENSES/GPL-3.0-or-later.txt` & `reuse-3.0.2/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/README.md` & `reuse-3.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 Git. This uses [pre-commit](https://pre-commit.com/). Once you
 [have it installed](https://pre-commit.com/#install), add this to the
 `.pre-commit-config.yaml` in your repository:
 
 ```yaml
 repos:
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v3.0.1
+    rev: v3.0.2
     hooks:
       - id: reuse
 ```
 
 Then run `pre-commit install`. Now, every time you commit, `reuse lint` is run
 in the background, and will prevent your commit from going through if there was
 an error.
```

### Comparing `reuse-3.0.1/_build.py` & `reuse-3.0.2/_build.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/docs/Makefile` & `reuse-3.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/docs/conf.py` & `reuse-3.0.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
 try:
     # The full version, including alpha/beta/rc tags.
     release = get_version("reuse")
 except PackageNotFoundError:
-    release = "3.0.1"
+    release = "3.0.2"
 
 # The short X.Y.Z version.
 version = ".".join(release.split(".")[:3])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
```

### Comparing `reuse-3.0.1/docs/index.rst` & `reuse-3.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/docs/requirements.txt` & `reuse-3.0.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/docs/reuse-r-only.svg` & `reuse-3.0.2/docs/reuse-r-only.svg`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/docs/scripts.rst` & `reuse-3.0.2/docs/scripts.rst`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/docs/usage.rst` & `reuse-3.0.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/cs.po` & `reuse-3.0.2/po/cs.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/de.po` & `reuse-3.0.2/po/de.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/eo.po` & `reuse-3.0.2/po/eo.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/es.po` & `reuse-3.0.2/po/es.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/fr.po` & `reuse-3.0.2/po/fr.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/gl.po` & `reuse-3.0.2/po/gl.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/it.po` & `reuse-3.0.2/po/it.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/nl.po` & `reuse-3.0.2/po/nl.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/pt.po` & `reuse-3.0.2/po/pt.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/reuse.pot` & `reuse-3.0.2/po/reuse.pot`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/sv.po` & `reuse-3.0.2/po/sv.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/tr.po` & `reuse-3.0.2/po/tr.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/po/uk.po` & `reuse-3.0.2/po/uk.po`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/pyproject.toml` & `reuse-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-FileCopyrightText: 2022 Carmen Bianca Bakker <carmenbianca@fsfe.org>
 # SPDX-FileCopyrightText: 2023 DB Systel GmbH
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [tool.poetry]
 name = "reuse"
-version = "3.0.1"
+version = "3.0.2"
 description = "reuse is a tool for compliance with the REUSE recommendations."
 authors = [
     "Free Software Foundation Europe <contact@fsfe.org>",
 ]
 maintainers = [
     "Carmen Bianca Bakker <carmenbianca@fsfe.org>",
     "Max Mehl <max.mehl@fsfe.org>",
```

### Comparing `reuse-3.0.1/src/reuse/__init__.py` & `reuse-3.0.2/src/reuse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from boolean.boolean import Expression
 
 try:
     __version__ = version("reuse")
 except PackageNotFoundError:
     # package is not installed
-    __version__ = "3.0.1"
+    __version__ = "3.0.2"
 
 __author__ = "Carmen Bianca Bakker"
 __email__ = "carmenbianca@fsfe.org"
 __license__ = "Apache-2.0 AND CC0-1.0 AND CC-BY-SA-4.0 AND GPL-3.0-or-later"
 __REUSE_version__ = "3.0"
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `reuse-3.0.1/src/reuse/_annotate.py` & `reuse-3.0.2/src/reuse/_annotate.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,19 +338,21 @@
     if not_writeable:
         parser.error(
             _("can't write to '{}'").format("', '".join(not_writeable))
         )
 
 
 def verify_paths_comment_style(args: Namespace, paths: Iterable[Path]) -> None:
-    """Exit if --fallback-dot-license or --skip-unrecognised is not enabled and
-    one of the paths has an unrecognised style.
+    """Exit if --style, --force-dot-license, --fallback-dot-license,
+    or --skip-unrecognised is not enabled and one of the paths has an
+    unrecognised style.
     """
     if (
-        not args.fallback_dot_license
+        not args.style
+        and not args.fallback_dot_license
         and not args.skip_unrecognised
         and not args.force_dot_license
     ):
         unrecognised_files = []
 
         for path in paths:
             if not _has_style(path):
```

### Comparing `reuse-3.0.1/src/reuse/_format.py` & `reuse-3.0.2/src/reuse/_format.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/_licenses.py` & `reuse-3.0.2/src/reuse/_licenses.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/_main.py` & `reuse-3.0.2/src/reuse/_main.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/_util.py` & `reuse-3.0.2/src/reuse/_util.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/comment.py` & `reuse-3.0.2/src/reuse/comment.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/download.py` & `reuse-3.0.2/src/reuse/download.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/header.py` & `reuse-3.0.2/src/reuse/header.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/init.py` & `reuse-3.0.2/src/reuse/init.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/lint.py` & `reuse-3.0.2/src/reuse/lint.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/project.py` & `reuse-3.0.2/src/reuse/project.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/report.py` & `reuse-3.0.2/src/reuse/report.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/resources/exceptions.json` & `reuse-3.0.2/src/reuse/resources/exceptions.json`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/resources/licenses.json` & `reuse-3.0.2/src/reuse/resources/licenses.json`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/spdx.py` & `reuse-3.0.2/src/reuse/spdx.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/supported_licenses.py` & `reuse-3.0.2/src/reuse/supported_licenses.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/src/reuse/vcs.py` & `reuse-3.0.2/src/reuse/vcs.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/conftest.py` & `reuse-3.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/resources/fsfe.png` & `reuse-3.0.2/tests/resources/fsfe.png`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/test_comment.py` & `reuse-3.0.2/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/test_core.py` & `reuse-3.0.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/test_download.py` & `reuse-3.0.2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/test_header.py` & `reuse-3.0.2/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/test_lint.py` & `reuse-3.0.2/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/test_main.py` & `reuse-3.0.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/test_main_annotate.py` & `reuse-3.0.2/tests/test_main_annotate.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,14 +448,39 @@
         out=stringio,
     )
 
     assert result == 0
     assert simple_file.read_text() == expected
 
 
+def test_annotate_specify_style_unrecognised(
+    fake_repository, stringio, mock_date_today
+):
+    """Add a header to a file that is unrecognised."""
+
+    simple_file = fake_repository / "hello.foo"
+    simple_file.touch()
+    expected = "# SPDX-FileCopyrightText: 2018 Jane Doe"
+
+    result = main(
+        [
+            "annotate",
+            "--copyright",
+            "Jane Doe",
+            "--style",
+            "python",
+            "hello.foo",
+        ],
+        out=stringio,
+    )
+
+    assert result == 0
+    assert simple_file.read_text().strip() == expected
+
+
 def test_annotate_implicit_style(fake_repository, stringio, mock_date_today):
     """Add a header to a file that has a recognised extension."""
     simple_file = fake_repository / "foo.js"
     simple_file.write_text("pass")
     expected = cleandoc(
         """
         // SPDX-FileCopyrightText: 2018 Jane Doe
```

### Comparing `reuse-3.0.1/tests/test_main_annotate_merge.py` & `reuse-3.0.2/tests/test_main_annotate_merge.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/test_project.py` & `reuse-3.0.2/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/test_report.py` & `reuse-3.0.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/test_util.py` & `reuse-3.0.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/tests/test_vcs.py` & `reuse-3.0.2/tests/test_vcs.py`

 * *Files identical despite different names*

### Comparing `reuse-3.0.1/PKG-INFO` & `reuse-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reuse
-Version: 3.0.1
+Version: 3.0.2
 Summary: reuse is a tool for compliance with the REUSE recommendations.
 Home-page: https://reuse.software/
 License: Apache-2.0 AND CC0-1.0 AND CC-BY-SA-4.0 AND GPL-3.0-or-later
 Author: Free Software Foundation Europe
 Author-email: contact@fsfe.org
 Maintainer: Carmen Bianca Bakker
 Maintainer-email: carmenbianca@fsfe.org
@@ -275,15 +275,15 @@
 Git. This uses [pre-commit](https://pre-commit.com/). Once you
 [have it installed](https://pre-commit.com/#install), add this to the
 `.pre-commit-config.yaml` in your repository:
 
 ```yaml
 repos:
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v3.0.1
+    rev: v3.0.2
     hooks:
       - id: reuse
 ```
 
 Then run `pre-commit install`. Now, every time you commit, `reuse lint` is run
 in the background, and will prevent your commit from going through if there was
 an error.
```

