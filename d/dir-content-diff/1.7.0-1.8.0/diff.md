# Comparing `tmp/dir-content-diff-1.7.0.tar.gz` & `tmp/dir-content-diff-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dir-content-diff-1.7.0.tar", last modified: Mon Feb  5 18:34:40 2024, max compression
+gzip compressed data, was "dir-content-diff-1.8.0.tar", last modified: Mon Apr  8 10:27:51 2024, max compression
```

## Comparing `dir-content-diff-1.7.0.tar` & `dir-content-diff-1.8.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:34:40.449624 dir-content-diff-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:34:40.441624 dir-content-diff-1.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:34:40.441624 dir-content-diff-1.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.github/ISSUE_TEMPLATE/how_to_use.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:34:40.441624 dir-content-diff-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.github/workflows/commitlint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.gitreview
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-02-05 18:34:40.449624 dir-content-diff-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:34:40.441624 dir-content-diff-1.7.0/dir_content_diff/
--rw-r--r--   0 runner    (1001) docker     (127)    14436 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/dir_content_diff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/dir_content_diff/base_comparators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/dir_content_diff/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/dir_content_diff/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/dir_content_diff/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:34:40.445624 dir-content-diff-1.7.0/dir_content_diff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-02-05 18:34:40.000000 dir-content-diff-1.7.0/dir_content_diff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-02-05 18:34:40.000000 dir-content-diff-1.7.0/dir_content_diff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 18:34:40.000000 dir-content-diff-1.7.0/dir_content_diff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-05 18:34:40.000000 dir-content-diff-1.7.0/dir_content_diff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-05 18:34:40.000000 dir-content-diff-1.7.0/dir_content_diff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 18:34:40.000000 dir-content-diff-1.7.0/dir_content_diff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:34:40.441624 dir-content-diff-1.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:34:40.445624 dir-content-diff-1.7.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/docs/source/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 18:34:40.449624 dir-content-diff-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:34:40.445624 dir-content-diff-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/tests/generate_test_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    42632 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12673 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-02-05 18:34:29.000000 dir-content-diff-1.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.801595 dir-content-diff-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.coveragerc_py38
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.793594 dir-content-diff-1.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.793594 dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/how_to_use.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.793594 dir-content-diff-1.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.gitreview
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-04-08 10:27:51.801595 dir-content-diff-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.797595 dir-content-diff-1.8.0/dir_content_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)    14436 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/dir_content_diff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/dir_content_diff/base_comparators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/dir_content_diff/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/dir_content_diff/pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/dir_content_diff/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.801595 dir-content-diff-1.8.0/dir_content_diff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.797595 dir-content-diff-1.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.797595 dir-content-diff-1.8.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:27:51.801595 dir-content-diff-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.801595 dir-content-diff-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/generate_test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42632 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tox.ini
```

### Comparing `dir-content-diff-1.7.0/.auto-changelog` & `dir-content-diff-1.8.0/.auto-changelog`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/.auto-changelog-template.hbs` & `dir-content-diff-1.8.0/.auto-changelog-template.hbs`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/.copier-answers.yml` & `dir-content-diff-1.8.0/.copier-answers.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changes here will be overwritten by Copier
 
-_commit: 0.1.53
+_commit: 0.1.54
 _src_path: git@bbpgitlab.epfl.ch:neuromath/python-template.git
 author_email: ''
 author_name: Blue Brain Project, EPFL
 copyright_license: Apache License 2.0
 copyright_year: '2023'
 distribution_name: dir-content-diff
 download_url: https://github.com/BlueBrain/dir-content-diff
```

### Comparing `dir-content-diff-1.7.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/.github/ISSUE_TEMPLATE/how_to_use.yaml` & `dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/how_to_use.yaml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/.github/dependabot.yml` & `dir-content-diff-1.8.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/.github/pull_request_template.md` & `dir-content-diff-1.8.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/.github/workflows/commitlint.yml` & `dir-content-diff-1.8.0/.github/workflows/commitlint.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,12 +8,12 @@
   check-pr-title:
     name: Check PR title
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-node@v4
         with:
-          node-version: '16'
+          node-version: '20'
       - run: npm install -g --force commitlint @commitlint/cli commitlint-plugin-cleanfeet
       - run: npm install conventional-changelog-conventionalcommits
       - run: touch .git/COMMIT_EDITMSG
       - run: echo "${{ github.event.pull_request.title }}" | commitlint
```

### Comparing `dir-content-diff-1.7.0/.github/workflows/publish-sdist.yml` & `dir-content-diff-1.8.0/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/.github/workflows/run-tox.yml` & `dir-content-diff-1.8.0/.github/workflows/run-tox.yml`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     - name: Upload to codecov
       uses: codecov/codecov-action@v4
       with:
         fail_ci_if_error: false
         directory: ./reports
         flags: pytest
         name: "dir-content-diff-py${{ matrix.python-version }}-${{ matrix.min_versions }}"
+        token: ${{ secrets.CODECOV_TOKEN }}
     - name: Upload test artifacts
       uses: actions/upload-artifact@v4
       if: always()
       with:
         name: tests-${{ matrix.python-version }}-${{ matrix.min_versions }}
         retention-days: 4
         path: |
```

### Comparing `dir-content-diff-1.7.0/.pre-commit-config.yaml` & `dir-content-diff-1.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/.pylintrc` & `dir-content-diff-1.8.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/CHANGELOG.md` & `dir-content-diff-1.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [1.8.0](https://github.com/BlueBrain/dir-content-diff/compare/1.7.0..1.8.0)
+
+> 8 April 2024
+
+### New Features
+
+- Add new comparators for Feather, Parquet and Stata files (Adrien Berchet - [#56](https://github.com/BlueBrain/dir-content-diff/pull/56))
+
 ## [1.7.0](https://github.com/BlueBrain/dir-content-diff/compare/1.6.0..1.7.0)
 
 > 5 February 2024
 
 ### New Features
 
 - Add 'replace_pattern' entry for DictComparator and several related save capabilities (Adrien Berchet - [#53](https://github.com/BlueBrain/dir-content-diff/pull/53))
```

### Comparing `dir-content-diff-1.7.0/CONTRIBUTING.md` & `dir-content-diff-1.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/LICENSE.txt` & `dir-content-diff-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/PKG-INFO` & `dir-content-diff-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir-content-diff
-Version: 1.7.0
+Version: 1.8.0
 Summary: Simple tool to compare directory contents.
 Home-page: https://dir-content-diff.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/dir-content-diff/issues
 Project-URL: Source, https://github.com/BlueBrain/dir-content-diff
 Classifier: Development Status :: 4 - Beta
@@ -24,29 +24,32 @@
 Requires-Dist: dictdiffer>=0.8
 Requires-Dist: dicttoxml>=1.7.12
 Requires-Dist: diff_pdf_visually>=1.7
 Requires-Dist: jsonpath-ng>=1.5
 Requires-Dist: PyYaml>=6
 Provides-Extra: pandas
 Requires-Dist: pandas>=1.4; extra == "pandas"
+Requires-Dist: pyarrow>=11; extra == "pandas"
 Requires-Dist: tables>=3.7; extra == "pandas"
 Provides-Extra: docs
 Requires-Dist: m2r2; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 Requires-Dist: pandas>=1.4; extra == "docs"
+Requires-Dist: pyarrow>=11; extra == "docs"
 Requires-Dist: tables>=3.7; extra == "docs"
 Provides-Extra: test
-Requires-Dist: coverage>=6; extra == "test"
+Requires-Dist: coverage>=7.2; extra == "test"
 Requires-Dist: dicttoxml>=1.7.16; extra == "test"
 Requires-Dist: matplotlib>=3; extra == "test"
 Requires-Dist: rst2pdf>=0.99; extra == "test"
 Requires-Dist: pytest>=6.2; extra == "test"
 Requires-Dist: pytest-html<4,>=2; extra == "test"
 Requires-Dist: pandas>=1.4; extra == "test"
+Requires-Dist: pyarrow>=11; extra == "test"
 Requires-Dist: tables>=3.7; extra == "test"
 
 [![Version](https://img.shields.io/pypi/v/dir-content-diff)](https://github.com/BlueBrain/dir-content-diff/releases)
 [![Build status](https://github.com/BlueBrain/dir-content-diff/actions/workflows/run-tox.yml/badge.svg?branch=main)](https://github.com/BlueBrain/dir-content-diff/actions)
 [![Coverage](https://codecov.io/github/BlueBrain/dir-content-diff/coverage.svg?branch=main)](https://codecov.io/github/BlueBrain/dir-content-diff?branch=main)
 [![License](https://img.shields.io/badge/License-Apache%202-blue)](https://github.com/BlueBrain/dir-content-diff/blob/main/LICENSE.txt)
 [![Documentation status](https://readthedocs.org/projects/dir-content-diff/badge/?version=latest)](https://dir-content-diff.readthedocs.io/)
```

### Comparing `dir-content-diff-1.7.0/README.md` & `dir-content-diff-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/commitlint.config.js` & `dir-content-diff-1.8.0/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/dir_content_diff/__init__.py` & `dir-content-diff-1.8.0/dir_content_diff/__init__.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/dir_content_diff/base_comparators.py` & `dir-content-diff-1.8.0/dir_content_diff/base_comparators.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/dir_content_diff/pandas.py` & `dir-content-diff-1.8.0/dir_content_diff/pandas.py`

 * *Files 16% similar despite different names*

```diff
@@ -143,16 +143,55 @@
     def save(self, data, path, **kwargs):
         """Save data to a HDF file."""
         index = kwargs.pop("index", False)
         key = kwargs.pop("key", "data")
         data.to_hdf(path, index=index, key=key, **kwargs)
 
 
+class FeatherComparator(DataframeComparator):
+    """Comparator for Feather files."""
+
+    def load(self, path, **kwargs):
+        """Load a Feather file into a :class:`pandas.DataFrame` object."""
+        return pd.read_feather(path, **kwargs)
+
+    def save(self, data, path, **kwargs):
+        """Save data to a Feather file."""
+        data.to_feather(path, **kwargs)
+
+
+class ParquetComparator(DataframeComparator):
+    """Comparator for Parquet files."""
+
+    def load(self, path, **kwargs):
+        """Load a Parquet file into a :class:`pandas.DataFrame` object."""
+        return pd.read_parquet(path, **kwargs)
+
+    def save(self, data, path, **kwargs):
+        """Save data to a Parquet file."""
+        data.to_parquet(path, **kwargs)
+
+
+class StataComparator(DataframeComparator):
+    """Comparator for Stata files."""
+
+    def load(self, path, **kwargs):
+        """Load a Stata file into a :class:`pandas.DataFrame` object."""
+        return pd.read_stata(path, **kwargs)
+
+    def save(self, data, path, **kwargs):
+        """Save data to a Stata file."""
+        data.to_stata(path, **kwargs)
+
+
 def register():
     """Register Pandas extensions."""
     register_comparator(".csv", CsvComparator())
     register_comparator(".tsv", CsvComparator())
     register_comparator(".h4", HdfComparator())
     register_comparator(".h5", HdfComparator())
     register_comparator(".hdf", HdfComparator())
     register_comparator(".hdf4", HdfComparator())
     register_comparator(".hdf5", HdfComparator())
+    register_comparator(".feather", FeatherComparator())
+    register_comparator(".parquet", ParquetComparator())
+    register_comparator(".dta", StataComparator())
```

### Comparing `dir-content-diff-1.7.0/dir_content_diff/pytest_plugin.py` & `dir-content-diff-1.8.0/dir_content_diff/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/dir_content_diff/util.py` & `dir-content-diff-1.8.0/dir_content_diff/util.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/dir_content_diff.egg-info/PKG-INFO` & `dir-content-diff-1.8.0/dir_content_diff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir-content-diff
-Version: 1.7.0
+Version: 1.8.0
 Summary: Simple tool to compare directory contents.
 Home-page: https://dir-content-diff.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/dir-content-diff/issues
 Project-URL: Source, https://github.com/BlueBrain/dir-content-diff
 Classifier: Development Status :: 4 - Beta
@@ -24,29 +24,32 @@
 Requires-Dist: dictdiffer>=0.8
 Requires-Dist: dicttoxml>=1.7.12
 Requires-Dist: diff_pdf_visually>=1.7
 Requires-Dist: jsonpath-ng>=1.5
 Requires-Dist: PyYaml>=6
 Provides-Extra: pandas
 Requires-Dist: pandas>=1.4; extra == "pandas"
+Requires-Dist: pyarrow>=11; extra == "pandas"
 Requires-Dist: tables>=3.7; extra == "pandas"
 Provides-Extra: docs
 Requires-Dist: m2r2; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 Requires-Dist: pandas>=1.4; extra == "docs"
+Requires-Dist: pyarrow>=11; extra == "docs"
 Requires-Dist: tables>=3.7; extra == "docs"
 Provides-Extra: test
-Requires-Dist: coverage>=6; extra == "test"
+Requires-Dist: coverage>=7.2; extra == "test"
 Requires-Dist: dicttoxml>=1.7.16; extra == "test"
 Requires-Dist: matplotlib>=3; extra == "test"
 Requires-Dist: rst2pdf>=0.99; extra == "test"
 Requires-Dist: pytest>=6.2; extra == "test"
 Requires-Dist: pytest-html<4,>=2; extra == "test"
 Requires-Dist: pandas>=1.4; extra == "test"
+Requires-Dist: pyarrow>=11; extra == "test"
 Requires-Dist: tables>=3.7; extra == "test"
 
 [![Version](https://img.shields.io/pypi/v/dir-content-diff)](https://github.com/BlueBrain/dir-content-diff/releases)
 [![Build status](https://github.com/BlueBrain/dir-content-diff/actions/workflows/run-tox.yml/badge.svg?branch=main)](https://github.com/BlueBrain/dir-content-diff/actions)
 [![Coverage](https://codecov.io/github/BlueBrain/dir-content-diff/coverage.svg?branch=main)](https://codecov.io/github/BlueBrain/dir-content-diff?branch=main)
 [![License](https://img.shields.io/badge/License-Apache%202-blue)](https://github.com/BlueBrain/dir-content-diff/blob/main/LICENSE.txt)
 [![Documentation status](https://readthedocs.org/projects/dir-content-diff/badge/?version=latest)](https://dir-content-diff.readthedocs.io/)
```

### Comparing `dir-content-diff-1.7.0/dir_content_diff.egg-info/SOURCES.txt` & `dir-content-diff-1.8.0/dir_content_diff.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .auto-changelog
 .auto-changelog-template.hbs
 .codespellignorelines
 .codespellrc
 .copier-answers.yml
 .coveragerc
+.coveragerc_py38
 .flake8
 .gitattributes
 .gitignore
 .gitreview
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yml
```

### Comparing `dir-content-diff-1.7.0/docs/Makefile` & `dir-content-diff-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/docs/source/conf.py` & `dir-content-diff-1.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/package.json` & `dir-content-diff-1.8.0/package.json`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/pyproject.toml` & `dir-content-diff-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/setup.py` & `dir-content-diff-1.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,20 @@
     "m2r2",
     "sphinx",
     "sphinx-bluebrain-theme",
 ]
 
 pandas_reqs = [
     "pandas>=1.4",
+    "pyarrow>=11",
     "tables>=3.7",
 ]
 
 test_reqs = [
-    "coverage>=6",
+    "coverage>=7.2",
     "dicttoxml>=1.7.16",
     "matplotlib>=3",
     "rst2pdf>=0.99",
     "pytest>=6.2",
     "pytest-html>=2,<4",
 ]
```

### Comparing `dir-content-diff-1.7.0/tests/conftest.py` & `dir-content-diff-1.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/tests/generate_test_files.py` & `dir-content-diff-1.8.0/tests/generate_test_files.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/tests/test_base.py` & `dir-content-diff-1.8.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/tests/test_pytest_plugin.py` & `dir-content-diff-1.8.0/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.7.0/tox.ini` & `dir-content-diff-1.8.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 [testenv]
 extras =
     pandas
     test
 setenv =
     COVERAGE_FILE = {env:COVERAGE_FILE:.coverage-{envname}}
+    py38,min_versions: COVERAGE_RCFILE=.coveragerc_py38
 deps =
     min_versions: Requirements-Builder
 commands =
     min_versions: requirements-builder --level=min --extras=pandas,test -o {envtmpdir}/requirements_min.txt setup.py
     min_versions: pip install -r {envtmpdir}/requirements_min.txt
     min_versions: pip freeze
     coverage run \
```

