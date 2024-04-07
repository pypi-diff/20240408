# Comparing `tmp/interrogate-1.6.0.tar.gz` & `tmp/interrogate-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interrogate-1.6.0.tar", last modified: Sat Apr  6 23:29:20 2024, max compression
+gzip compressed data, was "interrogate-1.7.0.tar", last modified: Sun Apr  7 22:30:02 2024, max compression
```

## Comparing `interrogate-1.6.0.tar` & `interrogate-1.7.0.tar`

### file list

```diff
@@ -1,183 +1,184 @@
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.848620 interrogate-1.6.0/
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.806166 interrogate-1.6.0/.github/
--rw-r--r--   0 lynn       (501) staff       (20)      110 2023-01-07 16:39:14.000000 interrogate-1.6.0/.github/FUNDING.yml
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.806492 interrogate-1.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 lynn       (501) staff       (20)      774 2023-01-07 16:39:14.000000 interrogate-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 lynn       (501) staff       (20)      801 2023-01-07 16:39:14.000000 interrogate-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 lynn       (501) staff       (20)      183 2023-01-07 16:39:14.000000 interrogate-1.6.0/.github/dependabot.yml
--rw-r--r--   0 lynn       (501) staff       (20)     2075 2023-01-07 16:39:14.000000 interrogate-1.6.0/.github/pull_request_template.md
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.807309 interrogate-1.6.0/.github/workflows/
--rw-r--r--   0 lynn       (501) staff       (20)     4477 2024-04-06 18:03:19.000000 interrogate-1.6.0/.github/workflows/main.yml
--rw-r--r--   0 lynn       (501) staff       (20)        0 2024-04-06 23:26:56.000000 interrogate-1.6.0/.github/workflows/pypi.yml
--rw-r--r--   0 lynn       (501) staff       (20)     2159 2024-04-06 18:03:19.000000 interrogate-1.6.0/.github/workflows/sanity.yml
--rw-r--r--   0 lynn       (501) staff       (20)      779 2024-04-06 18:03:19.000000 interrogate-1.6.0/.github/workflows/windows.yml
--rw-r--r--   0 lynn       (501) staff       (20)      947 2024-04-06 21:44:22.000000 interrogate-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0 lynn       (501) staff       (20)      214 2023-01-07 16:39:14.000000 interrogate-1.6.0/.pre-commit-hooks.yaml
--rw-r--r--   0 lynn       (501) staff       (20)      225 2024-04-06 18:03:19.000000 interrogate-1.6.0/.readthedocs.yaml
--rw-r--r--   0 lynn       (501) staff       (20)     1076 2023-01-07 16:39:14.000000 interrogate-1.6.0/LICENSE
--rw-r--r--   0 lynn       (501) staff       (20)      533 2024-04-06 18:03:07.000000 interrogate-1.6.0/MANIFEST.in
--rw-r--r--   0 lynn       (501) staff       (20)    35835 2024-04-06 23:29:20.848387 interrogate-1.6.0/PKG-INFO
--rw-r--r--   0 lynn       (501) staff       (20)    33051 2024-04-06 23:21:11.000000 interrogate-1.6.0/README.rst
--rw-r--r--   0 lynn       (501) staff       (20)      173 2023-01-07 16:39:14.000000 interrogate-1.6.0/codecov.yml
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.808221 interrogate-1.6.0/docs/
--rw-r--r--   0 lynn       (501) staff       (20)     1179 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/Makefile
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.809072 interrogate-1.6.0/docs/_static/
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.809991 interrogate-1.6.0/docs/_static/badge_examples/
--rw-r--r--   0 lynn       (501) staff       (20)    11389 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_f.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5733 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_fs.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11873 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_fsm.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5771 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_ftb.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11511 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_p.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6724 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_s.svg
--rw-r--r--   0 lynn       (501) staff       (20)      456 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/custom.css
--rw-r--r--   0 lynn       (501) staff       (20)     4791 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/favicon.png
--rw-r--r--   0 lynn       (501) staff       (20)    11873 2024-04-06 18:03:19.000000 interrogate-1.6.0/docs/_static/interrogate_badge.svg
--rw-r--r--   0 lynn       (501) staff       (20)    12422 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/logo_pink.png
--rw-r--r--   0 lynn       (501) staff       (20)     1079 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/logo_smol.png
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.810146 interrogate-1.6.0/docs/_templates/
--rw-r--r--   0 lynn       (501) staff       (20)      292 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_templates/navigation.html
--rw-r--r--   0 lynn       (501) staff       (20)     5630 2024-04-06 23:21:43.000000 interrogate-1.6.0/docs/changelog.rst
--rw-r--r--   0 lynn       (501) staff       (20)     3091 2024-04-06 18:03:19.000000 interrogate-1.6.0/docs/conf.py
--rw-r--r--   0 lynn       (501) staff       (20)       53 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/docutils.conf
--rw-r--r--   0 lynn       (501) staff       (20)     4391 2024-04-06 21:44:22.000000 interrogate-1.6.0/docs/index.rst
--rw-r--r--   0 lynn       (501) staff       (20)     1173 2024-04-06 23:03:15.000000 interrogate-1.6.0/pyproject.toml
--rw-r--r--   0 lynn       (501) staff       (20)       38 2024-04-06 23:29:20.848657 interrogate-1.6.0/setup.cfg
--rw-r--r--   0 lynn       (501) staff       (20)     3445 2024-04-06 23:23:17.000000 interrogate-1.6.0/setup.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.802338 interrogate-1.6.0/src/
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.811830 interrogate-1.6.0/src/interrogate/
--rw-r--r--   0 lynn       (501) staff       (20)      296 2024-04-06 23:18:55.000000 interrogate-1.6.0/src/interrogate/__init__.py
--rw-r--r--   0 lynn       (501) staff       (20)      129 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/__main__.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.813907 interrogate-1.6.0/src/interrogate/badge/
--rw-r--r--   0 lynn       (501) staff       (20)    11935 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/flat-square-modified-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5815 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/flat-square-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11460 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/flat-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5824 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/for-the-badge-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11648 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/plastic-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6812 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/social-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)     8243 2024-04-06 22:07:45.000000 interrogate-1.6.0/src/interrogate/badge_gen.py
--rw-r--r--   0 lynn       (501) staff       (20)    10587 2024-04-06 21:44:22.000000 interrogate-1.6.0/src/interrogate/cli.py
--rw-r--r--   0 lynn       (501) staff       (20)     8003 2024-04-06 23:05:46.000000 interrogate-1.6.0/src/interrogate/config.py
--rw-r--r--   0 lynn       (501) staff       (20)    17660 2024-04-06 23:16:35.000000 interrogate-1.6.0/src/interrogate/coverage.py
--rw-r--r--   0 lynn       (501) staff       (20)     8013 2024-04-06 18:03:19.000000 interrogate-1.6.0/src/interrogate/utils.py
--rw-r--r--   0 lynn       (501) staff       (20)     8276 2024-04-06 21:44:22.000000 interrogate-1.6.0/src/interrogate/visit.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.847423 interrogate-1.6.0/src/interrogate.egg-info/
--rw-r--r--   0 lynn       (501) staff       (20)    35835 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/PKG-INFO
--rw-r--r--   0 lynn       (501) staff       (20)     5838 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/SOURCES.txt
--rw-r--r--   0 lynn       (501) staff       (20)        1 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/dependency_links.txt
--rw-r--r--   0 lynn       (501) staff       (20)       53 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/entry_points.txt
--rw-r--r--   0 lynn       (501) staff       (20)        1 2023-01-07 17:13:34.000000 interrogate-1.6.0/src/interrogate.egg-info/not-zip-safe
--rw-r--r--   0 lynn       (501) staff       (20)      247 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/requires.txt
--rw-r--r--   0 lynn       (501) staff       (20)       12 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/top_level.txt
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.802814 interrogate-1.6.0/tests/
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.814436 interrogate-1.6.0/tests/functional/
--rw-r--r--   0 lynn       (501) staff       (20)       87 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/functional/__init__.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.816230 interrogate-1.6.0/tests/functional/fixtures/
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_badge.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6237 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_detailed.txt
--rw-r--r--   0 lynn       (501) staff       (20)     5751 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_detailed_no_module.txt
--rw-r--r--   0 lynn       (501) staff       (20)     2836 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_detailed_single_file.txt
--rw-r--r--   0 lynn       (501) staff       (20)     4050 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_detailed_skip_covered.txt
--rw-r--r--   0 lynn       (501) staff       (20)       47 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_no_verbosity.txt
--rw-r--r--   0 lynn       (501) staff       (20)      810 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_summary.txt
--rw-r--r--   0 lynn       (501) staff       (20)      729 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_summary_no_module.txt
--rw-r--r--   0 lynn       (501) staff       (20)      810 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_summary_skip_covered.txt
--rw-r--r--   0 lynn       (501) staff       (20)      405 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_summary_skip_covered_all.txt
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.817534 interrogate-1.6.0/tests/functional/fixtures/windows/
--rw-r--r--   0 lynn       (501) staff       (20)     6160 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed.txt
--rw-r--r--   0 lynn       (501) staff       (20)     6401 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed_no_module.txt
--rw-r--r--   0 lynn       (501) staff       (20)     2801 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed_single_file.txt
--rw-r--r--   0 lynn       (501) staff       (20)     4000 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed_skip_covered.txt
--rw-r--r--   0 lynn       (501) staff       (20)       47 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_no_verbosity.txt
--rw-r--r--   0 lynn       (501) staff       (20)      800 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary.txt
--rw-r--r--   0 lynn       (501) staff       (20)      560 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary_no_module.txt
--rw-r--r--   0 lynn       (501) staff       (20)      640 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary_skip_covered.txt
--rw-r--r--   0 lynn       (501) staff       (20)      560 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary_skip_covered_all.txt
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.818459 interrogate-1.6.0/tests/functional/sample/
--rw-r--r--   0 lynn       (501) staff       (20)       55 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/functional/sample/__init__.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.818820 interrogate-1.6.0/tests/functional/sample/child_sample/
--rw-r--r--   0 lynn       (501) staff       (20)       62 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/functional/sample/child_sample/__init__.py
--rw-r--r--   0 lynn       (501) staff       (20)      488 2024-04-06 18:03:19.000000 interrogate-1.6.0/tests/functional/sample/child_sample/child_sample_module.py
--rw-r--r--   0 lynn       (501) staff       (20)       33 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/functional/sample/empty.py
--rw-r--r--   0 lynn       (501) staff       (20)     1893 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/sample/full.py
--rw-r--r--   0 lynn       (501) staff       (20)       43 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/functional/sample/ignoreme.txt
--rw-r--r--   0 lynn       (501) staff       (20)     1582 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/sample/partial.py
--rw-r--r--   0 lynn       (501) staff       (20)     6097 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/test_cli.py
--rw-r--r--   0 lynn       (501) staff       (20)     9467 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/test_coverage.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.819533 interrogate-1.6.0/tests/unit/
--rw-r--r--   0 lynn       (501) staff       (20)       81 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/__init__.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.803267 interrogate-1.6.0/tests/unit/fixtures/
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.821007 interrogate-1.6.0/tests/unit/fixtures/default-style/
--rw-r--r--   0 lynn       (501) staff       (20)    11876 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11873 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6720 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/99.png
--rw-r--r--   0 lynn       (501) staff       (20)    11876 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/default.svg
--rw-r--r--   0 lynn       (501) staff       (20)     1685 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/no_logo.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.838644 interrogate-1.6.0/tests/unit/fixtures/flat/
--rw-r--r--   0 lynn       (501) staff       (20)    11392 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11389 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11396 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11396 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11396 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11396 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     7766 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/99.png
--rw-r--r--   0 lynn       (501) staff       (20)    11393 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11396 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/default.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.839985 interrogate-1.6.0/tests/unit/fixtures/flat-square/
--rw-r--r--   0 lynn       (501) staff       (20)     5736 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5733 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5739 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5739 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5739 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5739 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5583 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/99.png
--rw-r--r--   0 lynn       (501) staff       (20)     5736 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5739 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/default.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.841364 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/
--rw-r--r--   0 lynn       (501) staff       (20)    11876 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11873 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6720 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/99.png
--rw-r--r--   0 lynn       (501) staff       (20)    11876 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/default.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.842687 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/
--rw-r--r--   0 lynn       (501) staff       (20)     5774 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5771 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5779 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5779 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5779 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5779 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5803 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/99.png
--rw-r--r--   0 lynn       (501) staff       (20)     5776 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5777 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/default.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.845958 interrogate-1.6.0/tests/unit/fixtures/plastic/
--rw-r--r--   0 lynn       (501) staff       (20)    11514 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11511 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11518 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11518 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11518 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11518 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     8002 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/99.png
--rw-r--r--   0 lynn       (501) staff       (20)    11515 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11518 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/default.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.847209 interrogate-1.6.0/tests/unit/fixtures/social/
--rw-r--r--   0 lynn       (501) staff       (20)     6724 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6724 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     7102 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/99.png
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/default.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6426 2024-04-06 18:03:19.000000 interrogate-1.6.0/tests/unit/test_badge_gen.py
--rw-r--r--   0 lynn       (501) staff       (20)     7511 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/test_config.py
--rw-r--r--   0 lynn       (501) staff       (20)    10955 2024-04-06 18:03:20.000000 interrogate-1.6.0/tests/unit/test_utils.py
--rw-r--r--   0 lynn       (501) staff       (20)     1312 2024-04-06 21:32:01.000000 interrogate-1.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.736577 interrogate-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.708576 interrogate-1.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 22:29:57.000000 interrogate-1.7.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.708576 interrogate-1.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-07 22:29:57.000000 interrogate-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-07 22:29:57.000000 interrogate-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 22:29:57.000000 interrogate-1.7.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-07 22:29:57.000000 interrogate-1.7.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.712576 interrogate-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-07 22:29:57.000000 interrogate-1.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-07 22:29:57.000000 interrogate-1.7.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-07 22:29:57.000000 interrogate-1.7.0/.github/workflows/sanity.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-07 22:29:57.000000 interrogate-1.7.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-07 22:29:57.000000 interrogate-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-07 22:29:57.000000 interrogate-1.7.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-07 22:29:57.000000 interrogate-1.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-07 22:29:57.000000 interrogate-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-07 22:29:57.000000 interrogate-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    37451 2024-04-07 22:30:02.736577 interrogate-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34234 2024-04-07 22:29:57.000000 interrogate-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-07 22:29:57.000000 interrogate-1.7.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.712576 interrogate-1.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.712576 interrogate-1.7.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.712576 interrogate-1.7.0/docs/_static/badge_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_f.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_fs.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_fsm.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_ftb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11511 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_p.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_s.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_static/interrogate_badge.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12422 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_static/logo_pink.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_static/logo_smol.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.712576 interrogate-1.7.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/_templates/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-07 22:29:57.000000 interrogate-1.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-07 22:29:57.000000 interrogate-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:30:02.736577 interrogate-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-07 22:29:57.000000 interrogate-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.704576 interrogate-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.716576 interrogate-1.7.0/src/interrogate/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.716576 interrogate-1.7.0/src/interrogate/badge/
+-rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/badge/flat-square-modified-style.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/badge/flat-square-style.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/badge/flat-style.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/badge/for-the-badge-style.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/badge/plastic-style.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/badge/social-style.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/badge_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-07 22:29:57.000000 interrogate-1.7.0/src/interrogate/visit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.736577 interrogate-1.7.0/src/interrogate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    37451 2024-04-07 22:30:02.000000 interrogate-1.7.0/src/interrogate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-07 22:30:02.000000 interrogate-1.7.0/src/interrogate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:30:02.000000 interrogate-1.7.0/src/interrogate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-07 22:30:02.000000 interrogate-1.7.0/src/interrogate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:30:02.000000 interrogate-1.7.0/src/interrogate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-07 22:30:02.000000 interrogate-1.7.0/src/interrogate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 22:30:02.000000 interrogate-1.7.0/src/interrogate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.704576 interrogate-1.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.716576 interrogate-1.7.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.720576 interrogate-1.7.0/tests/functional/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/expected_badge.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/expected_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/expected_detailed_no_module.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/expected_detailed_single_file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/expected_detailed_skip_covered.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/expected_no_verbosity.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/expected_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/expected_summary_no_module.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/expected_summary_skip_covered.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/expected_summary_skip_covered_all.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.720576 interrogate-1.7.0/tests/functional/fixtures/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/windows/expected_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/windows/expected_detailed_no_module.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/windows/expected_detailed_single_file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/windows/expected_detailed_skip_covered.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/windows/expected_no_verbosity.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/windows/expected_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/windows/expected_summary_no_module.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/windows/expected_summary_skip_covered.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/fixtures/windows/expected_summary_skip_covered_all.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.720576 interrogate-1.7.0/tests/functional/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/sample/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.724576 interrogate-1.7.0/tests/functional/sample/child_sample/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/sample/child_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/sample/child_sample/child_sample_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/sample/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/sample/full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/sample/full.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/sample/ignoreme.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/sample/partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/functional/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.724576 interrogate-1.7.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.708576 interrogate-1.7.0/tests/unit/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.724576 interrogate-1.7.0/tests/unit/fixtures/default-style/
+-rw-r--r--   0 runner    (1001) docker     (127)    11876 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/default-style/0.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/default-style/100.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/default-style/45.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/default-style/60.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/default-style/89.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/default-style/90.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/default-style/99.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11876 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/default-style/99.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/default-style/default.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/default-style/no_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.728577 interrogate-1.7.0/tests/unit/fixtures/flat/
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat/0.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat/100.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat/45.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat/60.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat/89.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat/90.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat/99.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat/99.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat/default.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.728577 interrogate-1.7.0/tests/unit/fixtures/flat-square/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square/0.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square/100.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square/45.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square/60.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square/89.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square/90.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square/99.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square/99.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square/default.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.728577 interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/
+-rw-r--r--   0 runner    (1001) docker     (127)    11876 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/0.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/100.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/45.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/60.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/89.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/90.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/99.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11876 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/99.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/default.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.732576 interrogate-1.7.0/tests/unit/fixtures/for-the-badge/
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/for-the-badge/0.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/for-the-badge/100.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/for-the-badge/45.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/for-the-badge/60.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/for-the-badge/89.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/for-the-badge/90.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/for-the-badge/99.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/for-the-badge/99.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/for-the-badge/default.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.732576 interrogate-1.7.0/tests/unit/fixtures/plastic/
+-rw-r--r--   0 runner    (1001) docker     (127)    11514 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/plastic/0.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11511 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/plastic/100.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/plastic/45.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/plastic/60.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/plastic/89.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/plastic/90.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/plastic/99.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/plastic/99.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/plastic/default.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:02.736577 interrogate-1.7.0/tests/unit/fixtures/social/
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/social/0.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/social/100.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/social/45.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/social/60.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/social/89.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/social/90.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/social/99.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/social/99.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/fixtures/social/default.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/test_badge_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-04-07 22:29:57.000000 interrogate-1.7.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-07 22:29:57.000000 interrogate-1.7.0/tox.ini
```

### Comparing `interrogate-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `interrogate-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `interrogate-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/.github/pull_request_template.md` & `interrogate-1.7.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/.github/workflows/main.yml` & `interrogate-1.7.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/.github/workflows/sanity.yml` & `interrogate-1.7.0/.github/workflows/sanity.yml`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/.github/workflows/windows.yml` & `interrogate-1.7.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/.pre-commit-config.yaml` & `interrogate-1.7.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 ---
 ci:
   autoupdate_schedule: monthly
 
 repos:
   - repo: https://github.com/econchick/interrogate
-    rev: 1.5.0
+    rev: 1.6.0
     hooks:
       - id: interrogate
         exclude: ^(docs/conf.py|setup.py|tests/functional/sample)
         args: [--config=pyproject.toml]
 
   - repo: https://github.com/psf/black
     rev: 24.3.0
     hooks:
       - id: black
+        exclude: ^(tests/functional/sample/full.pyi)
 
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
```

### Comparing `interrogate-1.6.0/LICENSE` & `interrogate-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/MANIFEST.in` & `interrogate-1.7.0/MANIFEST.in`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 include LICENSE *.rst *.toml *.yml *.yaml *.ini
 include src/interrogate/badge/*.svg
 graft .github
 
 # Tests
 include tox.ini conftest.py
-recursive-include tests *.py
+recursive-include tests *.py *.pyi
 recursive-include tests *.svg *.png
 recursive-include tests *.txt
 
 # Documentation
 include docs/Makefile docs/docutils.conf
 recursive-include docs *.png
 recursive-include docs *.svg
```

### Comparing `interrogate-1.6.0/PKG-INFO` & `interrogate-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interrogate
-Version: 1.6.0
+Version: 1.7.0
 Summary: Interrogate a codebase for docstring coverage.
 Home-page: https://interrogate.readthedocs.io
 Author: Lynn Root
 Author-email: lynn@lynnroot.com
 Maintainer: Lynn Root
 Maintainer-email: lynn@lynnroot.com
 Project-URL: Documentation, https://interrogate.readthedocs.io
@@ -28,15 +28,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: click>=7.1
 Requires-Dist: colorama
 Requires-Dist: py
 Requires-Dist: tabulate
-Requires-Dist: toml
+Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: png
 Requires-Dist: cairosvg; extra == "png"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-autobuild; extra == "docs"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
@@ -370,15 +370,15 @@
 
 Or use it with `pre-commit <https://pre-commit.com/>`_:
 
 .. code-block:: yaml
 
     repos:
       - repo: https://github.com/econchick/interrogate
-        rev: 1.6.0  # or master if you're bold
+        rev: 1.7.0  # or master if you're bold
         hooks:
           - id: interrogate
             args: [--quiet, --fail-under=95]
             pass_filenames: false  # needed if excluding files with pyproject.toml or setup.cfg
 
 Use it within your code directly:
 
@@ -389,14 +389,15 @@
     >>> results = cov.get_coverage()
     >>> results
     InterrogateResults(total=68, covered=65, missing=3)
 
 
 Use ``interrogate`` with `GitHub Actions <https://github.com/features/actions>`_. Check out the `action <https://github.com/marketplace/actions/python-interrogate-check>`_ written & maintained by `Jack McKew <https://github.com/JackMcKew>`_ (thank you, Jack!).
 
+Or use ``interrogate`` in VSCode with the `interrogate extension <https://marketplace.visualstudio.com/items?itemName=kennethlove.interrogate>`_ written & maintained by `Kenneth Love <https://thekennethlove.com/>`_ (thank you, Kenneth!).
 
 Configuration
 =============
 
 Configure within your ``pyproject.toml`` (``interrogate`` will automatically detect a ``pyproject.toml`` file and pick up default values for the command line options):
 
 .. code-block:: console
@@ -416,14 +417,17 @@
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
     ignore-overloaded-functions = false
     fail-under = 95
     exclude = ["setup.py", "docs", "build"]
     ignore-regex = ["^get$", "^mock_.*", ".*BaseClass.*"]
+    ext = []
+    # possible values: sphinx (default), google
+    style = sphinx
     # possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex = []
     color = true
     omit-covered-files = false
     generate-badge = "."
@@ -449,14 +453,17 @@
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
     ignore-overloaded-functions = false
     fail-under = 95
     exclude = setup.py,docs,build
     ignore-regex = ^get$,^mock_.*,.*BaseClass.*
+    ext = []
+    ; possible values: sphinx (default), google
+    style = sphinx
     ; possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex =
     color = true
     omit-covered-files = false
     generate-badge = .
@@ -566,33 +573,45 @@
                                       [default: False]
 
                                       NOTE: This does not include magic methods;
                                       use `--ignore-magic` and/or `--ignore-init-
                                       method` instead.
 
       -P, --ignore-property-decorators
-                                      Ignore methods with property setter/getter
+                                      Ignore methods with property setter/getter/deleter
                                       decorators.  [default: False]
 
       -S, --ignore-setters            Ignore methods with property setter
                                       decorators.  [default: False]
 
       -s, --ignore-semiprivate        Ignore semiprivate classes, methods, and
                                       functions starting with a single underscore.
                                       [default: False]
 
       -r, --ignore-regex STR          Regex identifying class, method, and
                                       function names to ignore. Multiple
                                       `-r/--ignore-regex` invocations supported.
 
+      --ext                           Include Python-like files with the given
+                                      extension (supported: ``pyi``). Multiple
+                                      `--ext` invocations supported.
+
       -w, --whitelist-regex STR       Regex identifying class, method, and
                                       function names to include. Multiple
                                       `-w/--whitelist-regex` invocations
                                       supported.
 
+      --style [sphinx|google]         Style of docstrings to honor. Using `google`
+                                      will consider a class and its `__init__`
+                                      method both covered if there is either a
+                                      class-level docstring, or an `__init__`
+                                      method docstring, instead of enforcing both.
+                                      Mutually exclusive with `-i`/`--ignore-init`
+                                      flag.  [default: sphinx]
+
       -o, --output FILE               Write output to a given FILE.  [default:
                                       stdout]
 
       --color / --no-color            Toggle color output on/off when printing to
                                       stdout.  [default: True]
 
       --omit-covered-files            Omit reporting files that have 100%
@@ -668,23 +687,30 @@
 .. _docstring-coverage: https://bitbucket.org/DataGreed/docstring-coverage
 
 .. end-credits
 
 Release Information
 ===================
 
-1.6.0 (2024-04-06)
+1.7.0 (2024-04-07)
 ------------------
 
 Added
 ^^^^^
 
-* Add ``--ignore-overloaded-functions`` flag to ignore overload decorators (`#97 <https://github.com/econchick/interrogate/issues/97>`_) – thank you `ErwinJunge <https://github.com/econchick/interrogate/pull/98>`_ (via `#167 <https://github.com/econchick/interrogate/pull/167>`_) and `zackyancey <https://github.com/econchick/interrogate/pull/160>`_.
-* Support for Python 3.11 & 3.12.
+* `tomli` dependency for Python versions < 3.11, making use of `tomllib` in the standard library with 3.11+ (`#150 <https://github.com/econchick/interrogate/issues/150>`_).
+* Support for ``pyi`` file extensions (and leave room for other file extensions to be added, like maybe ``ipynb``).
+* Support for Google-style docstrings for class ``__init__`` methods with new ``--style [sphinx|google]`` flag (`#128 <https://github.com/econchick/interrogate/issues/128>`_).
+
+Fixed
+^^^^^
+
+* Include support for deleters when ignoring property decorators (`#126 <https://github.com/econchick/interrogate/issues/126>_`).
+* Support floats for `--fail-under` values (`#114 <https://github.com/econchick/interrogate/issues/114>`_).
 
 Removed
 ^^^^^^^
 
-* Support for Python 3.6 & 3.7.
+* `toml` dependency for all Python versions (`#150 <https://github.com/econchick/interrogate/issues/150>`_).
 
 
 `Full changelog <https://interrogate.readthedocs.io/en/latest/#changelog>`_.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `interrogate-1.6.0/README.rst` & `interrogate-1.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -314,15 +314,15 @@
 
 Or use it with `pre-commit <https://pre-commit.com/>`_:
 
 .. code-block:: yaml
 
     repos:
       - repo: https://github.com/econchick/interrogate
-        rev: 1.6.0  # or master if you're bold
+        rev: 1.7.0  # or master if you're bold
         hooks:
           - id: interrogate
             args: [--quiet, --fail-under=95]
             pass_filenames: false  # needed if excluding files with pyproject.toml or setup.cfg
 
 Use it within your code directly:
 
@@ -333,14 +333,15 @@
     >>> results = cov.get_coverage()
     >>> results
     InterrogateResults(total=68, covered=65, missing=3)
 
 
 Use ``interrogate`` with `GitHub Actions <https://github.com/features/actions>`_. Check out the `action <https://github.com/marketplace/actions/python-interrogate-check>`_ written & maintained by `Jack McKew <https://github.com/JackMcKew>`_ (thank you, Jack!).
 
+Or use ``interrogate`` in VSCode with the `interrogate extension <https://marketplace.visualstudio.com/items?itemName=kennethlove.interrogate>`_ written & maintained by `Kenneth Love <https://thekennethlove.com/>`_ (thank you, Kenneth!).
 
 Configuration
 =============
 
 Configure within your ``pyproject.toml`` (``interrogate`` will automatically detect a ``pyproject.toml`` file and pick up default values for the command line options):
 
 .. code-block:: console
@@ -360,14 +361,17 @@
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
     ignore-overloaded-functions = false
     fail-under = 95
     exclude = ["setup.py", "docs", "build"]
     ignore-regex = ["^get$", "^mock_.*", ".*BaseClass.*"]
+    ext = []
+    # possible values: sphinx (default), google
+    style = sphinx
     # possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex = []
     color = true
     omit-covered-files = false
     generate-badge = "."
@@ -393,14 +397,17 @@
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
     ignore-overloaded-functions = false
     fail-under = 95
     exclude = setup.py,docs,build
     ignore-regex = ^get$,^mock_.*,.*BaseClass.*
+    ext = []
+    ; possible values: sphinx (default), google
+    style = sphinx
     ; possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex =
     color = true
     omit-covered-files = false
     generate-badge = .
@@ -510,33 +517,45 @@
                                       [default: False]
 
                                       NOTE: This does not include magic methods;
                                       use `--ignore-magic` and/or `--ignore-init-
                                       method` instead.
 
       -P, --ignore-property-decorators
-                                      Ignore methods with property setter/getter
+                                      Ignore methods with property setter/getter/deleter
                                       decorators.  [default: False]
 
       -S, --ignore-setters            Ignore methods with property setter
                                       decorators.  [default: False]
 
       -s, --ignore-semiprivate        Ignore semiprivate classes, methods, and
                                       functions starting with a single underscore.
                                       [default: False]
 
       -r, --ignore-regex STR          Regex identifying class, method, and
                                       function names to ignore. Multiple
                                       `-r/--ignore-regex` invocations supported.
 
+      --ext                           Include Python-like files with the given
+                                      extension (supported: ``pyi``). Multiple
+                                      `--ext` invocations supported.
+
       -w, --whitelist-regex STR       Regex identifying class, method, and
                                       function names to include. Multiple
                                       `-w/--whitelist-regex` invocations
                                       supported.
 
+      --style [sphinx|google]         Style of docstrings to honor. Using `google`
+                                      will consider a class and its `__init__`
+                                      method both covered if there is either a
+                                      class-level docstring, or an `__init__`
+                                      method docstring, instead of enforcing both.
+                                      Mutually exclusive with `-i`/`--ignore-init`
+                                      flag.  [default: sphinx]
+
       -o, --output FILE               Write output to a given FILE.  [default:
                                       stdout]
 
       --color / --no-color            Toggle color output on/off when printing to
                                       stdout.  [default: True]
 
       --omit-covered-files            Omit reporting files that have 100%
```

### Comparing `interrogate-1.6.0/docs/Makefile` & `interrogate-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_f.svg` & `interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_f.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_fs.svg` & `interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_fs.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_fsm.svg` & `interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_fsm.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_ftb.svg` & `interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_ftb.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_p.svg` & `interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_p.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_s.svg` & `interrogate-1.7.0/docs/_static/badge_examples/interrogate_badge_s.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/_static/favicon.png` & `interrogate-1.7.0/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/_static/interrogate_badge.svg` & `interrogate-1.7.0/docs/_static/interrogate_badge.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/_static/logo_pink.png` & `interrogate-1.7.0/docs/_static/logo_pink.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/_static/logo_smol.png` & `interrogate-1.7.0/docs/_static/logo_smol.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/changelog.rst` & `interrogate-1.7.0/docs/changelog.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 Changelog
 =========
 
 .. short-log
 
+1.7.0 (2024-04-07)
+------------------
+
+Added
+^^^^^
+
+* `tomli` dependency for Python versions < 3.11, making use of `tomllib` in the standard library with 3.11+ (`#150 <https://github.com/econchick/interrogate/issues/150>`_).
+* Support for ``pyi`` file extensions (and leave room for other file extensions to be added, like maybe ``ipynb``).
+* Support for Google-style docstrings for class ``__init__`` methods with new ``--style [sphinx|google]`` flag (`#128 <https://github.com/econchick/interrogate/issues/128>`_).
+
+Fixed
+^^^^^
+
+* Include support for deleters when ignoring property decorators (`#126 <https://github.com/econchick/interrogate/issues/126>_`).
+* Support floats for `--fail-under` values (`#114 <https://github.com/econchick/interrogate/issues/114>`_).
+
+Removed
+^^^^^^^
+
+* `toml` dependency for all Python versions (`#150 <https://github.com/econchick/interrogate/issues/150>`_).
+
+.. short-log
+
 1.6.0 (2024-04-06)
 ------------------
 
 Added
 ^^^^^
 
 * Add ``--ignore-overloaded-functions`` flag to ignore overload decorators (`#97 <https://github.com/econchick/interrogate/issues/97>`_) – thank you `ErwinJunge <https://github.com/econchick/interrogate/pull/98>`_ (via `#167 <https://github.com/econchick/interrogate/pull/167>`_) and `zackyancey <https://github.com/econchick/interrogate/pull/160>`_.
 * Support for Python 3.11 & 3.12.
 
 Removed
 ^^^^^^^
 
 * Support for Python 3.6 & 3.7.
 
-.. short-log
 
 1.5.0 (2021-09-10)
 ------------------
 
 Added
 ^^^^^
```

### Comparing `interrogate-1.6.0/docs/conf.py` & `interrogate-1.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/docs/index.rst` & `interrogate-1.7.0/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -76,32 +76,43 @@
 
     Ignore private classes, methods, and functions starting with two underscores.  [default: ``False``]
 
     NOTE: This does not include magic methods; use ``--ignore-magic`` and/or ``--ignore-init-method`` instead.
 
 .. option:: -P, --ignore-property-decorators
 
-    Ignore methods with property setter/getter decorators.  [default: ``False``]
+    Ignore methods with property setter/getter/deleter decorators.  [default: ``False``]
 
 .. option:: -S, --ignore-setters
 
     Ignore methods with property setter decorators.  [default: ``False``]
 
 .. option:: -s, --ignore-semiprivate
 
     Ignore semiprivate classes, methods, and functions starting with a single underscore. [default: ``False``]
 
 .. option:: -r, --ignore-regex STR
 
     Regex identifying class, method, and function names to ignore. Multiple ``-r/--ignore-regex`` invocations supported.
 
+.. option:: --ext STR
+
+    Include Python-like files with the given extension (supported: ``pyi``). Multiple ``--ext`` invocations supported.
+
 .. option:: -w, --whitelist-regex STR
 
     Regex identifying class, method, and function names to include. Multiple ``-r/--ignore-regex`` invocations supported.
 
+.. option:: --style [sphinx|google]
+
+    Style of docstrings to honor. Using ``google`` will consider a class and its ``__init__`` method
+    both covered if there is either a class-level docstring, or an ``__init__`` method docstring,
+    instead of enforcing both. Mutually exclusive with ``-i/--ignore-init`` flag.
+    [default: ``sphinx``]
+
 .. option:: -o, --output FILE
 
     Write output to a given ``FILE``.  [default: ``stdout``]
 
 .. option:: -c, --config FILE
 
     Read configuration from ``pyproject.toml`` or ``setup.cfg``.
```

### Comparing `interrogate-1.6.0/pyproject.toml` & `interrogate-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/setup.py` & `interrogate-1.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 ]
 INSTALL_REQUIRES = [
     "attrs",
     "click>=7.1",
     "colorama",
     "py",
     "tabulate",
-    "toml",
+    "tomli; python_version < '3.11'",
 ]
 EXTRAS_REQUIRE = {
     "png": ["cairosvg"],
     "docs": ["sphinx", "sphinx-autobuild"],
     "tests": ["pytest", "pytest-cov", "pytest-mock", "coverage[toml]"],
 }
 EXTRAS_REQUIRE["dev"] = (
```

### Comparing `interrogate-1.6.0/src/interrogate/badge/flat-square-modified-style.svg` & `interrogate-1.7.0/src/interrogate/badge/flat-square-modified-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/src/interrogate/badge/flat-square-style.svg` & `interrogate-1.7.0/src/interrogate/badge/flat-square-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/src/interrogate/badge/flat-style.svg` & `interrogate-1.7.0/src/interrogate/badge/flat-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/src/interrogate/badge/for-the-badge-style.svg` & `interrogate-1.7.0/src/interrogate/badge/for-the-badge-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/src/interrogate/badge/plastic-style.svg` & `interrogate-1.7.0/src/interrogate/badge/plastic-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/src/interrogate/badge/social-style.svg` & `interrogate-1.7.0/src/interrogate/badge/social-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/src/interrogate/badge_gen.py` & `interrogate-1.7.0/src/interrogate/badge_gen.py`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/src/interrogate/cli.py` & `interrogate-1.7.0/src/interrogate/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 )
 @click.option(
     "-P",
     "--ignore-property-decorators",
     is_flag=True,
     default=False,
     show_default=True,
-    help="Ignore methods with property setter/getter decorators.",
+    help="Ignore methods with property setter/getter/deleter decorators.",
 )
 @click.option(
     "-S",
     "--ignore-setters",
     is_flag=True,
     default=False,
     show_default=True,
@@ -174,27 +174,51 @@
     callback=utils.parse_regex,
     help=(
         "Regex identifying class, method, and function names to ignore. "
         "Multiple `-r/--ignore-regex` invocations supported."
     ),
 )
 @click.option(
+    "--ext",
+    default=(),
+    multiple=True,
+    metavar="STR",
+    type=click.Choice(["pyi"], case_sensitive=False),
+    help=(
+        "Include Python-like files with the given extension "
+        "(supported: ``pyi``). Multiple ``--ext`` invocations supported. "
+        "``.py`` files included by default unless excluded in ``--exclude``."
+    ),
+)
+@click.option(
     "-w",
     "--whitelist-regex",
     type=str,
     default=(),
     multiple=True,
     metavar="STR",
     callback=utils.parse_regex,
     help=(
         "Regex identifying class, method, and function names to include. "
         "Multiple `-w/--whitelist-regex` invocations supported."
     ),
 )
 @click.option(
+    "--style",
+    type=click.Choice(["sphinx", "google"]),
+    default="sphinx",
+    show_default=True,
+    help=(
+        "Style of docstrings to honor.\nUsing `google` will consider a class "
+        "and its `__init__` method both covered if there is either a class-"
+        "level docstring, or an `__init__` method docstring, instead of "
+        "enforcing both. Mutually exclusive with `-i`/`--ignore-init` flag."
+    ),
+)
+@click.option(
     "-o",
     "--output",
     default=None,
     metavar="FILE",
     help="Write output to a given FILE.  [default: stdout]",
 )
 @click.option(
@@ -306,42 +330,55 @@
     .. versionadded:: 1.3.0 config parsing support for setup.cfg
     .. versionadded:: 1.4.0 ``--badge-format``
     .. versionadded:: 1.4.0 ``--ignore-nested-classes``
     .. versionadded:: 1.4.0 ``--ignore-setters``
     .. versionadded:: 1.5.0 ``--omit-covered-files``
     .. versionadded:: 1.5.0 ``--badge-style``
     .. versionadded:: 1.6.0 ``--ignore-overloaded-functions``
+    .. verisonadded:: 1.7.0 ``--ext``
+    .. versionadded:: 1.7.0 ``--style=sphinx|google``
 
     .. versionchanged:: 1.3.1 only generate badge if results change from
         an existing badge.
+    .. versionchanged:: 1.7.0 include property deleters when ignoring all
+        property decorators (--ignore-property-decorators)
     """
     gen_badge = kwargs["generate_badge"]
     if kwargs["badge_format"] is not None and gen_badge is None:
         raise click.BadParameter(
             "The `--badge-format` option must be used along with the `-g/"
             "--generate-badge option."
         )
     if kwargs["badge_style"] is not None and gen_badge is None:
         raise click.BadParameter(
             "The `--badge-style` option must be used along with the `-g/"
             "--generate-badge option."
         )
+    if kwargs["style"] == "google" and kwargs["ignore_init_method"]:
+        raise click.BadOptionUsage(
+            option_name="style",
+            message=(
+                "The `--ignore-init-method` flag is mutually exclusive with "
+                "`--style google`."
+            ),
+        )
     if not paths:
         paths = (os.path.abspath(os.getcwd()),)
 
     # NOTE: this will need to be fixed if we want to start supporting
     #       --whitelist-regex on filenames. This otherwise assumes you
     #       want to ignore module-level docs when only white listing
     #       items (visit.py will also need to be addressed since white/
     #       black listing only looks at classes & funcs, not modules).
     if kwargs["whitelist_regex"]:
         kwargs["ignore_module"] = True
 
     conf = config.InterrogateConfig(
         color=kwargs["color"],
+        docstring_style=kwargs["style"],
         fail_under=kwargs["fail_under"],
         ignore_regex=kwargs["ignore_regex"],
         ignore_magic=kwargs["ignore_magic"],
         ignore_module=kwargs["ignore_module"],
         ignore_private=kwargs["ignore_private"],
         ignore_semiprivate=kwargs["ignore_semiprivate"],
         ignore_init_method=kwargs["ignore_init_method"],
@@ -354,14 +391,15 @@
         include_regex=kwargs["whitelist_regex"],
         omit_covered_files=kwargs["omit_covered_files"],
     )
     interrogate_coverage = coverage.InterrogateCoverage(
         paths=paths,
         conf=conf,
         excluded=kwargs["exclude"],
+        extensions=kwargs["ext"],
     )
     results = interrogate_coverage.get_coverage()
 
     is_quiet = kwargs["quiet"]
     if not is_quiet:
         colorama.init()  # needed for Windows
         interrogate_coverage.print_results(
```

### Comparing `interrogate-1.6.0/src/interrogate/config.py` & `interrogate-1.7.0/src/interrogate/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,31 @@
 
 import configparser
 import os
 import pathlib
 
 import attr
 import click
-import toml
+
+
+try:
+    import tomllib
+except ImportError:
+    import tomli as tomllib
 
 
 # TODO: idea: break out InterrogateConfig into two classes: one for
 # running the tool, one for reporting the results
 @attr.s
 class InterrogateConfig:
     """Configuration related to interrogating a given codebase.
 
     :param bool color: Highlight verbose output with color.
+    :param str docstring_style: Style of docstrings to follow. Choices:
+        "sphinx" (default), "google".
     :param fail_under: Fail when coverage % is less than a given amount.
     :type fail_under: `int` or `float`
     :param str ignore_regex: Regex identifying class, method, and
         function names to ignore.
     :param bool ignore_magic: Ignore all magic methods of classes.
     :param bool ignore_module: Ignore module-level docstrings.
     :param bool ignore_private: Ignore private classes, methods, and
@@ -39,15 +46,18 @@
         function names to include.
     :param bool omit_covered_files: Omit reporting files that have 100%
         documentation coverage.
     :param bool ignore_overloaded_functions: Ignore `@typing.overload`-decorated
         functions.
     """
 
+    VALID_STYLES = ("sphinx", "google")
+
     color = attr.ib(default=False)
+    docstring_style = attr.ib(default="sphinx")
     fail_under = attr.ib(default=80.0)
     ignore_regex = attr.ib(default=False)
     ignore_magic = attr.ib(default=False)
     ignore_module = attr.ib(default=False)
     ignore_private = attr.ib(default=False)
     ignore_semiprivate = attr.ib(default=False)
     ignore_init_method = attr.ib(default=False)
@@ -56,14 +66,23 @@
     ignore_nested_functions = attr.ib(default=False)
     ignore_property_setters = attr.ib(default=False)
     ignore_property_decorators = attr.ib(default=False)
     ignore_overloaded_functions = attr.ib(default=False)
     include_regex = attr.ib(default=False)
     omit_covered_files = attr.ib(default=False)
 
+    @docstring_style.validator
+    def _check_style(self, attribute, value):
+        """Validate selected choice for docstring style"""
+        if value not in self.VALID_STYLES:
+            raise ValueError(
+                f"Invalid `docstring_style` '{value}'. Valid values: "
+                f"{', '.join(self.VALID_STYLES)}"
+            )
+
 
 def find_project_root(srcs):
     """Return a directory containing .git, .hg, or pyproject.toml.
     That directory can be one of the directories passed in `srcs` or their
     common parent.
     If no directory in the tree contains a marker that would specify it's the
     project root, the root of the file system is returned.
@@ -103,17 +122,18 @@
 def parse_pyproject_toml(path_config):
     """Parse ``pyproject.toml`` file and return relevant parts for Interrogate.
 
     :param str path_config: Path to ``pyproject.toml`` file.
     :return: Dictionary representing configuration for Interrogate.
     :rtype: dict
     :raise OSError: an I/O-related error when opening ``pyproject.toml``.
-    :raise toml.TomlDecodeError: unable to load ``pyproject.toml``.
+    :raise toml.TOMLDecodeError: unable to load ``pyproject.toml``.
     """
-    pyproject_toml = toml.load(path_config)
+    with open(path_config, "rb") as f:
+        pyproject_toml = tomllib.load(f)
     config = pyproject_toml.get("tool", {}).get("interrogate", {})
     return {
         k.replace("--", "").replace("-", "_"): v for k, v in config.items()
     }
 
 
 def sanitize_list_values(value):
@@ -198,15 +218,15 @@
         if value is None:
             return None
 
     config = None
     if value.endswith(".toml"):
         try:
             config = parse_pyproject_toml(value)
-        except (toml.TomlDecodeError, OSError) as e:
+        except (tomllib.TOMLDecodeError, OSError) as e:
             raise click.FileError(
                 filename=value,
                 hint=f"Error reading configuration file: {e}",
             )
 
     elif value.endswith(".cfg"):
         try:
```

### Comparing `interrogate-1.6.0/src/interrogate/coverage.py` & `interrogate-1.7.0/src/interrogate/coverage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright 2020 Lynn Root
 """Measure and report on documentation coverage in Python modules."""
 import ast
+import decimal
 import os
 import pathlib
 import sys
 
 from fnmatch import fnmatch
 
 import attr
@@ -104,17 +105,20 @@
     :param list(str) paths: list of paths to interrogate.
     :param config.InterrogateConfig conf: interrogation configuration.
     :param tuple(str) excluded: tuple of files and directories to exclude
         in assessing coverage.
     """
 
     COMMON_EXCLUDE = [".tox", ".venv", "venv", ".git", ".hg"]
+    VALID_EXT = [".py", ".pyi"]  # someday in the future: .ipynb
 
-    def __init__(self, paths, conf=None, excluded=None):
+    def __init__(self, paths, conf=None, excluded=None, extensions=None):
         self.paths = paths
+        self.extensions = set(extensions or set())
+        self.extensions.add(".py")
         self.config = conf or config.InterrogateConfig()
         self.excluded = excluded or ()
         self.common_base = pathlib.Path("/")
         self.output_formatter = None
         self._add_common_exclude()
         self.skipped_file_count = 0
 
@@ -124,45 +128,53 @@
             self.excluded = self.excluded + tuple(
                 os.path.join(path, i) for i in self.COMMON_EXCLUDE
             )
 
     def _filter_files(self, files):
         """Filter files that are explicitly excluded."""
         for f in files:
-            if not f.endswith(".py"):
+            has_valid_ext = any([f.endswith(ext) for ext in self.extensions])
+            if not has_valid_ext:
                 continue
             if self.config.ignore_init_module:
                 basename = os.path.basename(f)
                 if basename == "__init__.py":
                     continue
             if any(fnmatch(f, exc + "*") for exc in self.excluded):
                 continue
             yield f
 
     def get_filenames_from_paths(self):
         """Find all files to measure for docstring coverage."""
         filenames = []
         for path in self.paths:
             if os.path.isfile(path):
-                if not path.endswith(".py") and not path.endswith(".pyi"):
+                has_valid_ext = any(
+                    [path.endswith(ext) for ext in self.VALID_EXT]
+                )
+                if not has_valid_ext:
                     msg = (
-                        "E: Invalid file '{}'. Unable to interrogate non-Python"
-                        " files.".format(path)
+                        f"E: Invalid file '{path}'. Unable to interrogate "
+                        "non-Python or Python-like files. "
+                        f"Valid file extensions: {', '.join(self.VALID_EXT)}"
                     )
                     click.echo(msg, err=True)
                     return sys.exit(1)
                 filenames.append(path)
                 continue
             for root, dirs, fs in os.walk(path):
                 full_paths = [os.path.join(root, f) for f in fs]
                 filenames.extend(self._filter_files(full_paths))
 
         if not filenames:
             p = ", ".join(self.paths)
-            msg = f"E: No Python files found to interrogate in '{p}'."
+            msg = (
+                f"E: No Python or Python-like files found to interrogate in "
+                f"'{p}'."
+            )
             click.echo(msg, err=True)
             return sys.exit(1)
 
         self.common_base = utils.get_common_base(filenames)
         return filenames
 
     def _filter_nodes(self, nodes):
@@ -196,14 +208,31 @@
         nested_cls = [n for n in nodes if n.is_nested_cls]
         inner_nested_nodes = [n for n in nodes if n.parent in nested_cls]
 
         filtered_nodes = [n for n in nodes if n not in inner_nested_nodes]
         filtered_nodes = [n for n in filtered_nodes if n not in nested_cls]
         return filtered_nodes
 
+    def _set_google_style(self, nodes):
+        """Apply Google-style docstrings for class coverage.
+
+        Update coverage of a class node if its `__init__` method has a
+        docstring, or an `__init__` method if its class has a docstring.
+
+        A class and its `__init__` method are considered covered if either one
+        contains a docstring. See <https://sphinxcontrib-napoleon.readthedocs.
+        io/en/latest/example_google.html>`_ for more info and an example.
+        """
+        for node in nodes:
+            if node.node_type == "FunctionDef" and node.name == "__init__":
+                if not node.covered and node.parent.covered:
+                    setattr(node, "covered", True)
+                elif node.covered and not node.parent.covered:
+                    setattr(node.parent, "covered", True)
+
     def _get_file_coverage(self, filename):
         """Get coverage results for a particular file."""
         with open(filename, encoding="utf-8") as f:
             source_tree = f.read()
 
         parsed_tree = ast.parse(source_tree)
         visitor = visit.CoverageVisitor(filename=filename, config=self.config)
@@ -216,14 +245,17 @@
         if self.config.ignore_nested_functions:
             filtered_nodes = [
                 n for n in filtered_nodes if not n.is_nested_func
             ]
         if self.config.ignore_nested_classes:
             filtered_nodes = self._filter_inner_nested(filtered_nodes)
 
+        if self.config.docstring_style == "google":
+            self._set_google_style(filtered_nodes)
+
         results = InterrogateFileResult(
             filename=filename,
             ignore_module=self.config.ignore_module,
             nodes=filtered_nodes,
         )
         results.combine()
         return results
@@ -236,15 +268,18 @@
             result = self._get_file_coverage(f)
             if result:
                 file_results.append(result)
         results.file_results = file_results
 
         results.combine()
 
-        if self.config.fail_under > results.perc_covered:
+        fail_under_str = str(self.config.fail_under)
+        round_to = -decimal.Decimal(fail_under_str).as_tuple().exponent
+
+        if self.config.fail_under > round(results.perc_covered, round_to):
             results.ret_code = 1
 
         return results
 
     def get_coverage(self):
         """Get coverage results from files."""
         filenames = self.get_filenames_from_paths()
```

### Comparing `interrogate-1.6.0/src/interrogate/utils.py` & `interrogate-1.7.0/src/interrogate/utils.py`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/src/interrogate/visit.py` & `interrogate-1.7.0/src/interrogate/visit.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,25 +152,27 @@
             for regexp in self.config.ignore_regex:
                 regex_result = regexp.match(node.name)
                 if regex_result:
                     return True
         return False
 
     def _has_property_decorators(self, node):
-        """Detect if node has property get/setter decorators."""
+        """Detect if node has property get/setter/deleter decorators."""
         if not hasattr(node, "decorator_list"):
             return False
 
         for dec in node.decorator_list:
             if hasattr(dec, "id"):
                 if dec.id == "property":
                     return True
             if hasattr(dec, "attr"):
                 if dec.attr == "setter":
                     return True
+                if dec.attr == "deleter":
+                    return True
         return False
 
     def _has_setters(self, node):
         """Detect if node has property get/setter decorators."""
         if not hasattr(node, "decorator_list"):
             return False
```

### Comparing `interrogate-1.6.0/src/interrogate.egg-info/PKG-INFO` & `interrogate-1.7.0/src/interrogate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interrogate
-Version: 1.6.0
+Version: 1.7.0
 Summary: Interrogate a codebase for docstring coverage.
 Home-page: https://interrogate.readthedocs.io
 Author: Lynn Root
 Author-email: lynn@lynnroot.com
 Maintainer: Lynn Root
 Maintainer-email: lynn@lynnroot.com
 Project-URL: Documentation, https://interrogate.readthedocs.io
@@ -28,15 +28,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: click>=7.1
 Requires-Dist: colorama
 Requires-Dist: py
 Requires-Dist: tabulate
-Requires-Dist: toml
+Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: png
 Requires-Dist: cairosvg; extra == "png"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-autobuild; extra == "docs"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
@@ -370,15 +370,15 @@
 
 Or use it with `pre-commit <https://pre-commit.com/>`_:
 
 .. code-block:: yaml
 
     repos:
       - repo: https://github.com/econchick/interrogate
-        rev: 1.6.0  # or master if you're bold
+        rev: 1.7.0  # or master if you're bold
         hooks:
           - id: interrogate
             args: [--quiet, --fail-under=95]
             pass_filenames: false  # needed if excluding files with pyproject.toml or setup.cfg
 
 Use it within your code directly:
 
@@ -389,14 +389,15 @@
     >>> results = cov.get_coverage()
     >>> results
     InterrogateResults(total=68, covered=65, missing=3)
 
 
 Use ``interrogate`` with `GitHub Actions <https://github.com/features/actions>`_. Check out the `action <https://github.com/marketplace/actions/python-interrogate-check>`_ written & maintained by `Jack McKew <https://github.com/JackMcKew>`_ (thank you, Jack!).
 
+Or use ``interrogate`` in VSCode with the `interrogate extension <https://marketplace.visualstudio.com/items?itemName=kennethlove.interrogate>`_ written & maintained by `Kenneth Love <https://thekennethlove.com/>`_ (thank you, Kenneth!).
 
 Configuration
 =============
 
 Configure within your ``pyproject.toml`` (``interrogate`` will automatically detect a ``pyproject.toml`` file and pick up default values for the command line options):
 
 .. code-block:: console
@@ -416,14 +417,17 @@
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
     ignore-overloaded-functions = false
     fail-under = 95
     exclude = ["setup.py", "docs", "build"]
     ignore-regex = ["^get$", "^mock_.*", ".*BaseClass.*"]
+    ext = []
+    # possible values: sphinx (default), google
+    style = sphinx
     # possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex = []
     color = true
     omit-covered-files = false
     generate-badge = "."
@@ -449,14 +453,17 @@
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
     ignore-overloaded-functions = false
     fail-under = 95
     exclude = setup.py,docs,build
     ignore-regex = ^get$,^mock_.*,.*BaseClass.*
+    ext = []
+    ; possible values: sphinx (default), google
+    style = sphinx
     ; possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex =
     color = true
     omit-covered-files = false
     generate-badge = .
@@ -566,33 +573,45 @@
                                       [default: False]
 
                                       NOTE: This does not include magic methods;
                                       use `--ignore-magic` and/or `--ignore-init-
                                       method` instead.
 
       -P, --ignore-property-decorators
-                                      Ignore methods with property setter/getter
+                                      Ignore methods with property setter/getter/deleter
                                       decorators.  [default: False]
 
       -S, --ignore-setters            Ignore methods with property setter
                                       decorators.  [default: False]
 
       -s, --ignore-semiprivate        Ignore semiprivate classes, methods, and
                                       functions starting with a single underscore.
                                       [default: False]
 
       -r, --ignore-regex STR          Regex identifying class, method, and
                                       function names to ignore. Multiple
                                       `-r/--ignore-regex` invocations supported.
 
+      --ext                           Include Python-like files with the given
+                                      extension (supported: ``pyi``). Multiple
+                                      `--ext` invocations supported.
+
       -w, --whitelist-regex STR       Regex identifying class, method, and
                                       function names to include. Multiple
                                       `-w/--whitelist-regex` invocations
                                       supported.
 
+      --style [sphinx|google]         Style of docstrings to honor. Using `google`
+                                      will consider a class and its `__init__`
+                                      method both covered if there is either a
+                                      class-level docstring, or an `__init__`
+                                      method docstring, instead of enforcing both.
+                                      Mutually exclusive with `-i`/`--ignore-init`
+                                      flag.  [default: sphinx]
+
       -o, --output FILE               Write output to a given FILE.  [default:
                                       stdout]
 
       --color / --no-color            Toggle color output on/off when printing to
                                       stdout.  [default: True]
 
       --omit-covered-files            Omit reporting files that have 100%
@@ -668,23 +687,30 @@
 .. _docstring-coverage: https://bitbucket.org/DataGreed/docstring-coverage
 
 .. end-credits
 
 Release Information
 ===================
 
-1.6.0 (2024-04-06)
+1.7.0 (2024-04-07)
 ------------------
 
 Added
 ^^^^^
 
-* Add ``--ignore-overloaded-functions`` flag to ignore overload decorators (`#97 <https://github.com/econchick/interrogate/issues/97>`_) – thank you `ErwinJunge <https://github.com/econchick/interrogate/pull/98>`_ (via `#167 <https://github.com/econchick/interrogate/pull/167>`_) and `zackyancey <https://github.com/econchick/interrogate/pull/160>`_.
-* Support for Python 3.11 & 3.12.
+* `tomli` dependency for Python versions < 3.11, making use of `tomllib` in the standard library with 3.11+ (`#150 <https://github.com/econchick/interrogate/issues/150>`_).
+* Support for ``pyi`` file extensions (and leave room for other file extensions to be added, like maybe ``ipynb``).
+* Support for Google-style docstrings for class ``__init__`` methods with new ``--style [sphinx|google]`` flag (`#128 <https://github.com/econchick/interrogate/issues/128>`_).
+
+Fixed
+^^^^^
+
+* Include support for deleters when ignoring property decorators (`#126 <https://github.com/econchick/interrogate/issues/126>_`).
+* Support floats for `--fail-under` values (`#114 <https://github.com/econchick/interrogate/issues/114>`_).
 
 Removed
 ^^^^^^^
 
-* Support for Python 3.6 & 3.7.
+* `toml` dependency for all Python versions (`#150 <https://github.com/econchick/interrogate/issues/150>`_).
 
 
 `Full changelog <https://interrogate.readthedocs.io/en/latest/#changelog>`_.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `interrogate-1.6.0/src/interrogate.egg-info/SOURCES.txt` & `interrogate-1.7.0/src/interrogate.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 tests/functional/fixtures/windows/expected_summary.txt
 tests/functional/fixtures/windows/expected_summary_no_module.txt
 tests/functional/fixtures/windows/expected_summary_skip_covered.txt
 tests/functional/fixtures/windows/expected_summary_skip_covered_all.txt
 tests/functional/sample/__init__.py
 tests/functional/sample/empty.py
 tests/functional/sample/full.py
+tests/functional/sample/full.pyi
 tests/functional/sample/ignoreme.txt
 tests/functional/sample/partial.py
 tests/functional/sample/child_sample/__init__.py
 tests/functional/sample/child_sample/child_sample_module.py
 tests/unit/__init__.py
 tests/unit/test_badge_gen.py
 tests/unit/test_config.py
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/expected_badge.svg` & `interrogate-1.7.0/tests/unit/fixtures/default-style/90.svg`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 2e63 6f6d 2f22 2073 7479 6c65 3d22 6669  .com/" style="fi
 000000d0: 6c6c 2d72 756c 653a 6576 656e 6f64 643b  ll-rule:evenodd;
 000000e0: 636c 6970 2d72 756c 653a 6576 656e 6f64  clip-rule:evenod
 000000f0: 643b 7374 726f 6b65 2d6c 696e 656a 6f69  d;stroke-linejoi
 00000100: 6e3a 726f 756e 643b 7374 726f 6b65 2d6d  n:round;stroke-m
 00000110: 6974 6572 6c69 6d69 743a 323b 223e 0a20  iterlimit:2;">. 
 00000120: 2020 203c 7469 746c 653e 696e 7465 7272     <title>interr
-00000130: 6f67 6174 653a 2035 302e 3025 3c2f 7469  ogate: 50.0%</ti
+00000130: 6f67 6174 653a 2039 302e 3025 3c2f 7469  ogate: 90.0%</ti
 00000140: 746c 653e 0a20 2020 203c 6720 7472 616e  tle>.    <g tran
 00000150: 7366 6f72 6d3d 226d 6174 7269 7828 312c  sform="matrix(1,
 00000160: 302c 302c 312c 3232 2c30 2922 3e0a 2020  0,0,1,22,0)">.  
 00000170: 2020 2020 2020 3c67 2069 643d 2262 6163        <g id="bac
 00000180: 6b67 726f 756e 6473 2220 7472 616e 7366  kgrounds" transf
 00000190: 6f72 6d3d 226d 6174 7269 7828 312e 3332  orm="matrix(1.32
 000001a0: 3738 392c 302c 302c 312c 2d32 322e 3338  789,0,0,1,-22.38
@@ -33,15 +33,15 @@
 00000200: 3835 2c38 3529 3b22 2f3e 0a20 2020 2020  85,85);"/>.     
 00000210: 2020 203c 2f67 3e0a 2020 2020 2020 2020     </g>.        
 00000220: 3c72 6563 7420 783d 2237 3122 2079 3d22  <rect x="71" y="
 00000230: 3022 2077 6964 7468 3d22 3437 2220 6865  0" width="47" he
 00000240: 6967 6874 3d22 3230 2220 6461 7461 2d69  ight="20" data-i
 00000250: 6e74 6572 726f 6761 7465 3d22 636f 6c6f  nterrogate="colo
 00000260: 7222 2073 7479 6c65 3d22 6669 6c6c 3a23  r" style="fill:#
-00000270: 6665 3764 3337 222f 3e0a 2020 2020 2020  fe7d37"/>.      
+00000270: 3937 4341 3030 222f 3e0a 2020 2020 2020  97CA00"/>.      
 00000280: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
 00000290: 6d61 7472 6978 2831 2e31 3937 3436 2c30  matrix(1.19746,0
 000002a0: 2c30 2c31 2c2d 3232 2e33 3734 342c 2d34  ,0,1,-22.3744,-4
 000002b0: 2e38 3537 3233 652d 3136 2922 3e0a 2020  .85723e-16)">.  
 000002c0: 2020 2020 2020 2020 2020 3c72 6563 7420            <rect 
 000002d0: 783d 2230 2220 793d 2230 2220 7769 6474  x="0" y="0" widt
 000002e0: 683d 2231 3138 2220 6865 6967 6874 3d22  h="118" height="
@@ -72,22 +72,22 @@
 00000470: 7465 7874 2078 3d22 3131 3630 2220 793d  text x="1160" y=
 00000480: 2231 3530 2220 6669 6c6c 3d22 2330 3130  "150" fill="#010
 00000490: 3130 3122 2066 696c 6c2d 6f70 6163 6974  101" fill-opacit
 000004a0: 793d 222e 3322 2074 7261 6e73 666f 726d  y=".3" transform
 000004b0: 3d22 7363 616c 6528 2e31 2922 2074 6578  ="scale(.1)" tex
 000004c0: 744c 656e 6774 683d 2233 3730 2220 6461  tLength="370" da
 000004d0: 7461 2d69 6e74 6572 726f 6761 7465 3d22  ta-interrogate="
-000004e0: 7265 7375 6c74 223e 3530 2e30 253c 2f74  result">50.0%</t
+000004e0: 7265 7375 6c74 223e 3930 2e30 253c 2f74  result">90.0%</t
 000004f0: 6578 743e 0a20 2020 2020 2020 203c 7465  ext>.        <te
 00000500: 7874 2078 3d22 3131 3630 2220 793d 2231  xt x="1160" y="1
 00000510: 3430 2220 7472 616e 7366 6f72 6d3d 2273  40" transform="s
 00000520: 6361 6c65 282e 3129 2220 7465 7874 4c65  cale(.1)" textLe
 00000530: 6e67 7468 3d22 3337 3022 2064 6174 612d  ngth="370" data-
 00000540: 696e 7465 7272 6f67 6174 653d 2272 6573  interrogate="res
-00000550: 756c 7422 3e35 302e 3025 3c2f 7465 7874  ult">50.0%</text
+00000550: 756c 7422 3e39 302e 3025 3c2f 7465 7874  ult">90.0%</text
 00000560: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
 00000570: 6720 6964 3d22 6c6f 676f 2d73 6861 646f  g id="logo-shado
 00000580: 7722 2073 6572 6966 3a69 643d 226c 6f67  w" serif:id="log
 00000590: 6f20 7368 6164 6f77 2220 7472 616e 7366  o shadow" transf
 000005a0: 6f72 6d3d 226d 6174 7269 7828 302e 3835  orm="matrix(0.85
 000005b0: 3438 3736 2c30 2c30 2c30 2e38 3534 3837  4876,0,0,0.85487
 000005c0: 362c 2d36 2e37 3335 3134 2c31 2e37 3332  6,-6.73514,1.732
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/expected_detailed.txt` & `interrogate-1.7.0/tests/functional/fixtures/windows/expected_detailed.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,83 @@
------------------------------- Detailed Coverage -------------------------------
-| Name                                                             |    Status |
-|------------------------------------------------------------------|-----------|
-| __init__.py (module)                                             |   COVERED |
-|------------------------------------------------------------------|-----------|
-| empty.py (module)                                                |    MISSED |
-|------------------------------------------------------------------|-----------|
-| full.py (module)                                                 |   COVERED |
-|   Foo (L8)                                                       |   COVERED |
-|     Foo.__init__ (L11)                                           |   COVERED |
-|     Foo.__str__ (L15)                                            |   COVERED |
-|     Foo._semiprivate (L19)                                       |   COVERED |
-|     Foo.__private (L23)                                          |   COVERED |
-|     Foo.method_foo (L27)                                         |   COVERED |
-|     Foo.get (L31)                                                |   COVERED |
-|     Foo.get (L35)                                                |   COVERED |
-|     Foo.prop (L40)                                               |   COVERED |
-|     Foo.prop (L45)                                               |   COVERED |
-|     Foo.module_overload (L50)                                    |   COVERED |
-|     Foo.module_overload (L55)                                    |   COVERED |
-|     Foo.module_overload (L59)                                    |   COVERED |
-|     Foo.simple_overload (L64)                                    |   COVERED |
-|     Foo.simple_overload (L69)                                    |   COVERED |
-|     Foo.simple_overload (L73)                                    |   COVERED |
-|   top_level_func (L78)                                           |   COVERED |
-|     top_level_func.inner_func (L81)                              |   COVERED |
-|   Bar (L86)                                                      |   COVERED |
-|     Bar.method_bar (L89)                                         |   COVERED |
-|       Bar.method_bar.InnerBar (L92)                              |   COVERED |
-|   _SemiprivateClass (L98)                                        |   COVERED |
-|   __PrivateClass (L104)                                          |   COVERED |
-|------------------------------------------------------------------|-----------|
-| partial.py (module)                                              |   COVERED |
-|   Foo (L8)                                                       |   COVERED |
-|     Foo.__init__ (L11)                                           |   COVERED |
-|     Foo.__str__ (L15)                                            |   COVERED |
-|     Foo.__repr__ (L19)                                           |    MISSED |
-|     Foo._semiprivate_documented (L22)                            |   COVERED |
-|     Foo._semiprivate_undocumented (L26)                          |    MISSED |
-|     Foo.__private (L29)                                          |    MISSED |
-|     Foo.method_foo (L32)                                         |    MISSED |
-|     Foo.get (L35)                                                |    MISSED |
-|     Foo.get (L38)                                                |    MISSED |
-|     Foo.a_prop (L42)                                             |    MISSED |
-|     Foo.a_prop (L46)                                             |    MISSED |
-|     Foo.module_overload (L50)                                    |    MISSED |
-|     Foo.module_overload (L53)                                    |    MISSED |
-|     Foo.module_overload (L55)                                    |   COVERED |
-|     Foo.simple_overload (L60)                                    |    MISSED |
-|     Foo.simple_overload (L63)                                    |    MISSED |
-|     Foo.simple_overload (L65)                                    |   COVERED |
-|   documented_top_level_func (L70)                                |   COVERED |
-|     documented_top_level_func.documented_inner_func (L73)        |   COVERED |
-|   undocumented_top_level_func (L78)                              |    MISSED |
-|     undocumented_top_level_func.undocumented_inner_func (L79)    |    MISSED |
-|   Bar (L83)                                                      |    MISSED |
-|     Bar.method_bar (L84)                                         |    MISSED |
-|       Bar.method_bar.InnerBar (L85)                              |    MISSED |
-|   _SemiprivateClass (L89)                                        |    MISSED |
-|   __PrivateClass (L93)                                           |    MISSED |
-|------------------------------------------------------------------|-----------|
-| child_sample/__init__.py (module)                                |    MISSED |
-|------------------------------------------------------------------|-----------|
-| child_sample/child_sample_module.py (module)                     |    MISSED |
-|   ChildFoo (L5)                                                  |    MISSED |
-|     ChildFoo.__init__ (L6)                                       |    MISSED |
-|     ChildFoo.__str__ (L9)                                        |    MISSED |
-|     ChildFoo._ignore_me (L12)                                    |    MISSED |
-|     ChildFoo.__ignore_me_too (L15)                               |    MISSED |
-|     ChildFoo.method_foo (L18)                                    |    MISSED |
-|   a_child_func (L22)                                             |    MISSED |
-|   ChildBar (L26)                                                 |    MISSED |
-|     ChildBar.method_bar (L27)                                    |    MISSED |
-|       ChildBar.method_bar.InnerBar (L28)                         |    MISSED |
-|   _ChildBaz (L34)                                                |    MISSED |
-|   __ChildBla (L38)                                               |    MISSED |
-|------------------------------------------------------------------|-----------|
+------------------------------ Detailed Coverage ------------------------------
+| Name                                                            |    Status |
+|-----------------------------------------------------------------|-----------|
+| __init__.py (module)                                            |   COVERED |
+|-----------------------------------------------------------------|-----------|
+| empty.py (module)                                               |    MISSED |
+|-----------------------------------------------------------------|-----------|
+| full.py (module)                                                |   COVERED |
+|   Foo (L8)                                                      |   COVERED |
+|     Foo.__init__ (L11)                                          |   COVERED |
+|     Foo.__str__ (L15)                                           |   COVERED |
+|     Foo._semiprivate (L19)                                      |   COVERED |
+|     Foo.__private (L23)                                         |   COVERED |
+|     Foo.method_foo (L27)                                        |   COVERED |
+|     Foo.get (L31)                                               |   COVERED |
+|     Foo.get (L35)                                               |   COVERED |
+|     Foo.prop (L40)                                              |   COVERED |
+|     Foo.prop (L45)                                              |   COVERED |
+|     Foo.prop (L50)                                              |   COVERED |
+|     Foo.module_overload (L55)                                   |   COVERED |
+|     Foo.module_overload (L60)                                   |   COVERED |
+|     Foo.module_overload (L64)                                   |   COVERED |
+|     Foo.simple_overload (L69)                                   |   COVERED |
+|     Foo.simple_overload (L74)                                   |   COVERED |
+|     Foo.simple_overload (L78)                                   |   COVERED |
+|   top_level_func (L83)                                          |   COVERED |
+|     top_level_func.inner_func (L86)                             |   COVERED |
+|   Bar (L91)                                                     |   COVERED |
+|     Bar.method_bar (L94)                                        |   COVERED |
+|       Bar.method_bar.InnerBar (L97)                             |   COVERED |
+|   _SemiprivateClass (L103)                                      |   COVERED |
+|   __PrivateClass (L109)                                         |   COVERED |
+|   InitDocs (L116)                                               |   COVERED |
+|     InitDocs.__init__ (L117)                                    |   COVERED |
+|   ClassDocs (L123)                                              |   COVERED |
+|     ClassDocs.__init__ (L126)                                   |   COVERED |
+|-----------------------------------------------------------------|-----------|
+| partial.py (module)                                             |   COVERED |
+|   Foo (L8)                                                      |   COVERED |
+|     Foo.__init__ (L11)                                          |   COVERED |
+|     Foo.__str__ (L15)                                           |   COVERED |
+|     Foo.__repr__ (L19)                                          |    MISSED |
+|     Foo._semiprivate_documented (L22)                           |   COVERED |
+|     Foo._semiprivate_undocumented (L26)                         |    MISSED |
+|     Foo.__private (L29)                                         |    MISSED |
+|     Foo.method_foo (L32)                                        |    MISSED |
+|     Foo.get (L35)                                               |    MISSED |
+|     Foo.get (L38)                                               |    MISSED |
+|     Foo.a_prop (L42)                                            |    MISSED |
+|     Foo.a_prop (L46)                                            |    MISSED |
+|     Foo.a_prop (L50)                                            |   COVERED |
+|     Foo.module_overload (L54)                                   |    MISSED |
+|     Foo.module_overload (L57)                                   |    MISSED |
+|     Foo.module_overload (L59)                                   |   COVERED |
+|     Foo.simple_overload (L64)                                   |    MISSED |
+|     Foo.simple_overload (L67)                                   |    MISSED |
+|     Foo.simple_overload (L69)                                   |   COVERED |
+|   documented_top_level_func (L74)                               |   COVERED |
+|     documented_top_level_func.documented_inner_func (L77)       |   COVERED |
+|   undocumented_top_level_func (L82)                             |    MISSED |
+|     undocumented_top_level_func.undocumented_inner_func (L83)   |    MISSED |
+|   Bar (L87)                                                     |    MISSED |
+|     Bar.method_bar (L88)                                        |    MISSED |
+|       Bar.method_bar.InnerBar (L89)                             |    MISSED |
+|   _SemiprivateClass (L93)                                       |    MISSED |
+|   __PrivateClass (L97)                                          |    MISSED |
+|-----------------------------------------------------------------|-----------|
+| child_sample\__init__.py (module)                               |    MISSED |
+|-----------------------------------------------------------------|-----------|
+| child_sample\child_sample_module.py (module)                    |    MISSED |
+|   ChildFoo (L5)                                                 |    MISSED |
+|     ChildFoo.__init__ (L6)                                      |    MISSED |
+|     ChildFoo.__str__ (L9)                                       |    MISSED |
+|     ChildFoo._ignore_me (L12)                                   |    MISSED |
+|     ChildFoo.__ignore_me_too (L15)                              |    MISSED |
+|     ChildFoo.method_foo (L18)                                   |    MISSED |
+|   a_child_func (L22)                                            |    MISSED |
+|   ChildBar (L26)                                                |    MISSED |
+|     ChildBar.method_bar (L27)                                   |    MISSED |
+|       ChildBar.method_bar.InnerBar (L28)                        |    MISSED |
+|   _ChildBaz (L34)                                               |    MISSED |
+|   __ChildBla (L38)                                              |    MISSED |
+|-----------------------------------------------------------------|-----------|
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/expected_detailed_no_module.txt` & `interrogate-1.7.0/tests/functional/fixtures/expected_detailed_no_module.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,56 +8,62 @@
 |     Foo._semiprivate (L19)                                       |   COVERED |
 |     Foo.__private (L23)                                          |   COVERED |
 |     Foo.method_foo (L27)                                         |   COVERED |
 |     Foo.get (L31)                                                |   COVERED |
 |     Foo.get (L35)                                                |   COVERED |
 |     Foo.prop (L40)                                               |   COVERED |
 |     Foo.prop (L45)                                               |   COVERED |
-|     Foo.module_overload (L50)                                    |   COVERED |
+|     Foo.prop (L50)                                               |   COVERED |
 |     Foo.module_overload (L55)                                    |   COVERED |
-|     Foo.module_overload (L59)                                    |   COVERED |
-|     Foo.simple_overload (L64)                                    |   COVERED |
+|     Foo.module_overload (L60)                                    |   COVERED |
+|     Foo.module_overload (L64)                                    |   COVERED |
 |     Foo.simple_overload (L69)                                    |   COVERED |
-|     Foo.simple_overload (L73)                                    |   COVERED |
-|   top_level_func (L78)                                           |   COVERED |
-|     top_level_func.inner_func (L81)                              |   COVERED |
-|   Bar (L86)                                                      |   COVERED |
-|     Bar.method_bar (L89)                                         |   COVERED |
-|       Bar.method_bar.InnerBar (L92)                              |   COVERED |
-|   _SemiprivateClass (L98)                                        |   COVERED |
-|   __PrivateClass (L104)                                          |   COVERED |
+|     Foo.simple_overload (L74)                                    |   COVERED |
+|     Foo.simple_overload (L78)                                    |   COVERED |
+|   top_level_func (L83)                                           |   COVERED |
+|     top_level_func.inner_func (L86)                              |   COVERED |
+|   Bar (L91)                                                      |   COVERED |
+|     Bar.method_bar (L94)                                         |   COVERED |
+|       Bar.method_bar.InnerBar (L97)                              |   COVERED |
+|   _SemiprivateClass (L103)                                       |   COVERED |
+|   __PrivateClass (L109)                                          |   COVERED |
+|   InitDocs (L116)                                                |   COVERED |
+|     InitDocs.__init__ (L117)                                     |   COVERED |
+|   ClassDocs (L123)                                               |   COVERED |
+|     ClassDocs.__init__ (L126)                                    |   COVERED |
 |------------------------------------------------------------------|-----------|
 | partial.py                                                       |           |
 |   Foo (L8)                                                       |   COVERED |
 |     Foo.__init__ (L11)                                           |   COVERED |
 |     Foo.__str__ (L15)                                            |   COVERED |
 |     Foo.__repr__ (L19)                                           |    MISSED |
 |     Foo._semiprivate_documented (L22)                            |   COVERED |
 |     Foo._semiprivate_undocumented (L26)                          |    MISSED |
 |     Foo.__private (L29)                                          |    MISSED |
 |     Foo.method_foo (L32)                                         |    MISSED |
 |     Foo.get (L35)                                                |    MISSED |
 |     Foo.get (L38)                                                |    MISSED |
 |     Foo.a_prop (L42)                                             |    MISSED |
 |     Foo.a_prop (L46)                                             |    MISSED |
-|     Foo.module_overload (L50)                                    |    MISSED |
-|     Foo.module_overload (L53)                                    |    MISSED |
-|     Foo.module_overload (L55)                                    |   COVERED |
-|     Foo.simple_overload (L60)                                    |    MISSED |
-|     Foo.simple_overload (L63)                                    |    MISSED |
-|     Foo.simple_overload (L65)                                    |   COVERED |
-|   documented_top_level_func (L70)                                |   COVERED |
-|     documented_top_level_func.documented_inner_func (L73)        |   COVERED |
-|   undocumented_top_level_func (L78)                              |    MISSED |
-|     undocumented_top_level_func.undocumented_inner_func (L79)    |    MISSED |
-|   Bar (L83)                                                      |    MISSED |
-|     Bar.method_bar (L84)                                         |    MISSED |
-|       Bar.method_bar.InnerBar (L85)                              |    MISSED |
-|   _SemiprivateClass (L89)                                        |    MISSED |
-|   __PrivateClass (L93)                                           |    MISSED |
+|     Foo.a_prop (L50)                                             |   COVERED |
+|     Foo.module_overload (L54)                                    |    MISSED |
+|     Foo.module_overload (L57)                                    |    MISSED |
+|     Foo.module_overload (L59)                                    |   COVERED |
+|     Foo.simple_overload (L64)                                    |    MISSED |
+|     Foo.simple_overload (L67)                                    |    MISSED |
+|     Foo.simple_overload (L69)                                    |   COVERED |
+|   documented_top_level_func (L74)                                |   COVERED |
+|     documented_top_level_func.documented_inner_func (L77)        |   COVERED |
+|   undocumented_top_level_func (L82)                              |    MISSED |
+|     undocumented_top_level_func.undocumented_inner_func (L83)    |    MISSED |
+|   Bar (L87)                                                      |    MISSED |
+|     Bar.method_bar (L88)                                         |    MISSED |
+|       Bar.method_bar.InnerBar (L89)                              |    MISSED |
+|   _SemiprivateClass (L93)                                        |    MISSED |
+|   __PrivateClass (L97)                                           |    MISSED |
 |------------------------------------------------------------------|-----------|
 | child_sample/child_sample_module.py                              |           |
 |   ChildFoo (L5)                                                  |    MISSED |
 |     ChildFoo.__init__ (L6)                                       |    MISSED |
 |     ChildFoo.__str__ (L9)                                        |    MISSED |
 |     ChildFoo._ignore_me (L12)                                    |    MISSED |
 |     ChildFoo.__ignore_me_too (L15)                               |    MISSED |
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/expected_detailed_single_file.txt` & `interrogate-1.7.0/tests/functional/fixtures/expected_detailed_single_file.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,29 +8,34 @@
 |     Foo._semiprivate (L19)                          |                COVERED |
 |     Foo.__private (L23)                             |                COVERED |
 |     Foo.method_foo (L27)                            |                COVERED |
 |     Foo.get (L31)                                   |                COVERED |
 |     Foo.get (L35)                                   |                COVERED |
 |     Foo.prop (L40)                                  |                COVERED |
 |     Foo.prop (L45)                                  |                COVERED |
-|     Foo.module_overload (L50)                       |                COVERED |
+|     Foo.prop (L50)                                  |                COVERED |
 |     Foo.module_overload (L55)                       |                COVERED |
-|     Foo.module_overload (L59)                       |                COVERED |
-|     Foo.simple_overload (L64)                       |                COVERED |
+|     Foo.module_overload (L60)                       |                COVERED |
+|     Foo.module_overload (L64)                       |                COVERED |
 |     Foo.simple_overload (L69)                       |                COVERED |
-|     Foo.simple_overload (L73)                       |                COVERED |
-|   top_level_func (L78)                              |                COVERED |
-|     top_level_func.inner_func (L81)                 |                COVERED |
-|   Bar (L86)                                         |                COVERED |
-|     Bar.method_bar (L89)                            |                COVERED |
-|       Bar.method_bar.InnerBar (L92)                 |                COVERED |
-|   _SemiprivateClass (L98)                           |                COVERED |
-|   __PrivateClass (L104)                             |                COVERED |
+|     Foo.simple_overload (L74)                       |                COVERED |
+|     Foo.simple_overload (L78)                       |                COVERED |
+|   top_level_func (L83)                              |                COVERED |
+|     top_level_func.inner_func (L86)                 |                COVERED |
+|   Bar (L91)                                         |                COVERED |
+|     Bar.method_bar (L94)                            |                COVERED |
+|       Bar.method_bar.InnerBar (L97)                 |                COVERED |
+|   _SemiprivateClass (L103)                          |                COVERED |
+|   __PrivateClass (L109)                             |                COVERED |
+|   InitDocs (L116)                                   |                COVERED |
+|     InitDocs.__init__ (L117)                        |                COVERED |
+|   ClassDocs (L123)                                  |                COVERED |
+|     ClassDocs.__init__ (L126)                       |                COVERED |
 |-----------------------------------------------------|------------------------|
 
 ----------------------------------- Summary ------------------------------------
 | Name             |        Total |        Miss |        Cover |        Cover% |
 |------------------|--------------|-------------|--------------|---------------|
-| full.py          |           24 |           0 |           24 |          100% |
+| full.py          |           29 |           0 |           29 |          100% |
 |------------------|--------------|-------------|--------------|---------------|
-| TOTAL            |           24 |           0 |           24 |        100.0% |
+| TOTAL            |           29 |           0 |           29 |        100.0% |
 --------------- RESULT: PASSED (minimum: 80.0%, actual: 100.0%) ----------------
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/expected_detailed_skip_covered.txt` & `interrogate-1.7.0/tests/functional/fixtures/expected_detailed_skip_covered.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,30 @@
 |     Foo._semiprivate_undocumented (L26)                          |    MISSED |
 |     Foo.__private (L29)                                          |    MISSED |
 |     Foo.method_foo (L32)                                         |    MISSED |
 |     Foo.get (L35)                                                |    MISSED |
 |     Foo.get (L38)                                                |    MISSED |
 |     Foo.a_prop (L42)                                             |    MISSED |
 |     Foo.a_prop (L46)                                             |    MISSED |
-|     Foo.module_overload (L50)                                    |    MISSED |
-|     Foo.module_overload (L53)                                    |    MISSED |
-|     Foo.module_overload (L55)                                    |   COVERED |
-|     Foo.simple_overload (L60)                                    |    MISSED |
-|     Foo.simple_overload (L63)                                    |    MISSED |
-|     Foo.simple_overload (L65)                                    |   COVERED |
-|   documented_top_level_func (L70)                                |   COVERED |
-|     documented_top_level_func.documented_inner_func (L73)        |   COVERED |
-|   undocumented_top_level_func (L78)                              |    MISSED |
-|     undocumented_top_level_func.undocumented_inner_func (L79)    |    MISSED |
-|   Bar (L83)                                                      |    MISSED |
-|     Bar.method_bar (L84)                                         |    MISSED |
-|       Bar.method_bar.InnerBar (L85)                              |    MISSED |
-|   _SemiprivateClass (L89)                                        |    MISSED |
-|   __PrivateClass (L93)                                           |    MISSED |
+|     Foo.a_prop (L50)                                             |   COVERED |
+|     Foo.module_overload (L54)                                    |    MISSED |
+|     Foo.module_overload (L57)                                    |    MISSED |
+|     Foo.module_overload (L59)                                    |   COVERED |
+|     Foo.simple_overload (L64)                                    |    MISSED |
+|     Foo.simple_overload (L67)                                    |    MISSED |
+|     Foo.simple_overload (L69)                                    |   COVERED |
+|   documented_top_level_func (L74)                                |   COVERED |
+|     documented_top_level_func.documented_inner_func (L77)        |   COVERED |
+|   undocumented_top_level_func (L82)                              |    MISSED |
+|     undocumented_top_level_func.undocumented_inner_func (L83)    |    MISSED |
+|   Bar (L87)                                                      |    MISSED |
+|     Bar.method_bar (L88)                                         |    MISSED |
+|       Bar.method_bar.InnerBar (L89)                              |    MISSED |
+|   _SemiprivateClass (L93)                                        |    MISSED |
+|   __PrivateClass (L97)                                           |    MISSED |
 |------------------------------------------------------------------|-----------|
 | child_sample/__init__.py (module)                                |    MISSED |
 |------------------------------------------------------------------|-----------|
 | child_sample/child_sample_module.py (module)                     |    MISSED |
 |   ChildFoo (L5)                                                  |    MISSED |
 |     ChildFoo.__init__ (L6)                                       |    MISSED |
 |     ChildFoo.__str__ (L9)                                        |    MISSED |
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/expected_summary.txt` & `interrogate-1.7.0/tests/functional/fixtures/expected_summary_skip_covered.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 | Name                                     |  Total |  Miss |  Cover |  Cover% |
 |------------------------------------------|--------|-------|--------|---------|
-| __init__.py                              |      1 |     0 |      1 |    100% |
 | empty.py                                 |      1 |     1 |      0 |      0% |
-| full.py                                  |     24 |     0 |     24 |    100% |
-| partial.py                               |     28 |    19 |      9 |     32% |
+| partial.py                               |     29 |    19 |     10 |     34% |
 | child_sample/__init__.py                 |      1 |     1 |      0 |      0% |
 | child_sample/child_sample_module.py      |     13 |    13 |      0 |      0% |
 |------------------------------------------|--------|-------|--------|---------|
-| TOTAL                                    |     68 |    34 |     34 |   50.0% |
+| TOTAL                                    |     74 |    34 |     40 |   54.1% |
+|------------------------------------------------------------------------------|
+|               (2 of 6 files omitted due to complete coverage)                |
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/expected_summary_no_module.txt` & `interrogate-1.7.0/tests/functional/fixtures/expected_summary_no_module.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ----------------------------------- Summary ------------------------------------
 | Name                                     |  Total |  Miss |  Cover |  Cover% |
 |------------------------------------------|--------|-------|--------|---------|
-| full.py                                  |     23 |     0 |     23 |    100% |
-| partial.py                               |     27 |    19 |      8 |     30% |
+| full.py                                  |     28 |     0 |     28 |    100% |
+| partial.py                               |     28 |    19 |      9 |     32% |
 | child_sample/child_sample_module.py      |     12 |    12 |      0 |      0% |
 |------------------------------------------|--------|-------|--------|---------|
-| TOTAL                                    |     62 |    31 |     31 |   50.0% |
----------------- RESULT: FAILED (minimum: 80.0%, actual: 50.0%) ----------------
+| TOTAL                                    |     68 |    31 |     37 |   54.4% |
+---------------- RESULT: FAILED (minimum: 80.0%, actual: 54.4%) ----------------
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/expected_summary_skip_covered.txt` & `interrogate-1.7.0/tests/functional/fixtures/windows/expected_summary_skip_covered.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-| Name                                     |  Total |  Miss |  Cover |  Cover% |
-|------------------------------------------|--------|-------|--------|---------|
-| empty.py                                 |      1 |     1 |      0 |      0% |
-| partial.py                               |     28 |    19 |      9 |     32% |
-| child_sample/__init__.py                 |      1 |     1 |      0 |      0% |
-| child_sample/child_sample_module.py      |     13 |    13 |      0 |      0% |
-|------------------------------------------|--------|-------|--------|---------|
-| TOTAL                                    |     68 |    34 |     34 |   50.0% |
-|------------------------------------------------------------------------------|
-|               (2 of 6 files omitted due to complete coverage)                |
+| Name                                    |  Total |  Miss |  Cover |  Cover% |
+|-----------------------------------------|--------|-------|--------|---------|
+| empty.py                                |      1 |     1 |      0 |      0% |
+| partial.py                              |     29 |    19 |     10 |     34% |
+| child_sample\__init__.py                |      1 |     1 |      0 |      0% |
+| child_sample\child_sample_module.py     |     13 |    13 |      0 |      0% |
+|-----------------------------------------|--------|-------|--------|---------|
+| TOTAL                                   |     74 |    34 |     40 |   54.1% |
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed.txt` & `interrogate-1.7.0/tests/functional/fixtures/expected_detailed.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,83 @@
------------------------------- Detailed Coverage ------------------------------
-| Name                                                            |    Status |
-|-----------------------------------------------------------------|-----------|
-| __init__.py (module)                                            |   COVERED |
-|-----------------------------------------------------------------|-----------|
-| empty.py (module)                                               |    MISSED |
-|-----------------------------------------------------------------|-----------|
-| full.py (module)                                                |   COVERED |
-|   Foo (L8)                                                      |   COVERED |
-|     Foo.__init__ (L11)                                          |   COVERED |
-|     Foo.__str__ (L15)                                           |   COVERED |
-|     Foo._semiprivate (L19)                                      |   COVERED |
-|     Foo.__private (L23)                                         |   COVERED |
-|     Foo.method_foo (L27)                                        |   COVERED |
-|     Foo.get (L31)                                               |   COVERED |
-|     Foo.get (L35)                                               |   COVERED |
-|     Foo.prop (L40)                                              |   COVERED |
-|     Foo.prop (L45)                                              |   COVERED |
-|     Foo.module_overload (L50)                                   |   COVERED |
-|     Foo.module_overload (L55)                                   |   COVERED |
-|     Foo.module_overload (L59)                                   |   COVERED |
-|     Foo.simple_overload (L64)                                   |   COVERED |
-|     Foo.simple_overload (L69)                                   |   COVERED |
-|     Foo.simple_overload (L73)                                   |   COVERED |
-|   top_level_func (L78)                                          |   COVERED |
-|     top_level_func.inner_func (L81)                             |   COVERED |
-|   Bar (L86)                                                     |   COVERED |
-|     Bar.method_bar (L89)                                        |   COVERED |
-|       Bar.method_bar.InnerBar (L92)                             |   COVERED |
-|   _SemiprivateClass (L98)                                       |   COVERED |
-|   __PrivateClass (L104)                                         |   COVERED |
-|-----------------------------------------------------------------|-----------|
-| partial.py (module)                                             |   COVERED |
-|   Foo (L8)                                                      |   COVERED |
-|     Foo.__init__ (L11)                                          |   COVERED |
-|     Foo.__str__ (L15)                                           |   COVERED |
-|     Foo.__repr__ (L19)                                          |    MISSED |
-|     Foo._semiprivate_documented (L22)                           |   COVERED |
-|     Foo._semiprivate_undocumented (L26)                         |    MISSED |
-|     Foo.__private (L29)                                         |    MISSED |
-|     Foo.method_foo (L32)                                        |    MISSED |
-|     Foo.get (L35)                                               |    MISSED |
-|     Foo.get (L38)                                               |    MISSED |
-|     Foo.a_prop (L42)                                            |    MISSED |
-|     Foo.a_prop (L46)                                            |    MISSED |
-|     Foo.module_overload (L50)                                   |    MISSED |
-|     Foo.module_overload (L53)                                   |    MISSED |
-|     Foo.module_overload (L55)                                   |   COVERED |
-|     Foo.simple_overload (L60)                                   |    MISSED |
-|     Foo.simple_overload (L63)                                   |    MISSED |
-|     Foo.simple_overload (L65)                                   |   COVERED |
-|   documented_top_level_func (L70)                               |   COVERED |
-|     documented_top_level_func.documented_inner_func (L73)       |   COVERED |
-|   undocumented_top_level_func (L78)                             |    MISSED |
-|     undocumented_top_level_func.undocumented_inner_func (L79)   |    MISSED |
-|   Bar (L83)                                                     |    MISSED |
-|     Bar.method_bar (L84)                                        |    MISSED |
-|       Bar.method_bar.InnerBar (L85)                             |    MISSED |
-|   _SemiprivateClass (L89)                                       |    MISSED |
-|   __PrivateClass (L93)                                          |    MISSED |
-|-----------------------------------------------------------------|-----------|
-| child_sample\__init__.py (module)                               |    MISSED |
-|-----------------------------------------------------------------|-----------|
-| child_sample\child_sample_module.py (module)                    |    MISSED |
-|   ChildFoo (L5)                                                 |    MISSED |
-|     ChildFoo.__init__ (L6)                                      |    MISSED |
-|     ChildFoo.__str__ (L9)                                       |    MISSED |
-|     ChildFoo._ignore_me (L12)                                   |    MISSED |
-|     ChildFoo.__ignore_me_too (L15)                              |    MISSED |
-|     ChildFoo.method_foo (L18)                                   |    MISSED |
-|   a_child_func (L22)                                            |    MISSED |
-|   ChildBar (L26)                                                |    MISSED |
-|     ChildBar.method_bar (L27)                                   |    MISSED |
-|       ChildBar.method_bar.InnerBar (L28)                        |    MISSED |
-|   _ChildBaz (L34)                                               |    MISSED |
-|   __ChildBla (L38)                                              |    MISSED |
-|-----------------------------------------------------------------|-----------|
+------------------------------ Detailed Coverage -------------------------------
+| Name                                                             |    Status |
+|------------------------------------------------------------------|-----------|
+| __init__.py (module)                                             |   COVERED |
+|------------------------------------------------------------------|-----------|
+| empty.py (module)                                                |    MISSED |
+|------------------------------------------------------------------|-----------|
+| full.py (module)                                                 |   COVERED |
+|   Foo (L8)                                                       |   COVERED |
+|     Foo.__init__ (L11)                                           |   COVERED |
+|     Foo.__str__ (L15)                                            |   COVERED |
+|     Foo._semiprivate (L19)                                       |   COVERED |
+|     Foo.__private (L23)                                          |   COVERED |
+|     Foo.method_foo (L27)                                         |   COVERED |
+|     Foo.get (L31)                                                |   COVERED |
+|     Foo.get (L35)                                                |   COVERED |
+|     Foo.prop (L40)                                               |   COVERED |
+|     Foo.prop (L45)                                               |   COVERED |
+|     Foo.prop (L50)                                               |   COVERED |
+|     Foo.module_overload (L55)                                    |   COVERED |
+|     Foo.module_overload (L60)                                    |   COVERED |
+|     Foo.module_overload (L64)                                    |   COVERED |
+|     Foo.simple_overload (L69)                                    |   COVERED |
+|     Foo.simple_overload (L74)                                    |   COVERED |
+|     Foo.simple_overload (L78)                                    |   COVERED |
+|   top_level_func (L83)                                           |   COVERED |
+|     top_level_func.inner_func (L86)                              |   COVERED |
+|   Bar (L91)                                                      |   COVERED |
+|     Bar.method_bar (L94)                                         |   COVERED |
+|       Bar.method_bar.InnerBar (L97)                              |   COVERED |
+|   _SemiprivateClass (L103)                                       |   COVERED |
+|   __PrivateClass (L109)                                          |   COVERED |
+|   InitDocs (L116)                                                |   COVERED |
+|     InitDocs.__init__ (L117)                                     |   COVERED |
+|   ClassDocs (L123)                                               |   COVERED |
+|     ClassDocs.__init__ (L126)                                    |   COVERED |
+|------------------------------------------------------------------|-----------|
+| partial.py (module)                                              |   COVERED |
+|   Foo (L8)                                                       |   COVERED |
+|     Foo.__init__ (L11)                                           |   COVERED |
+|     Foo.__str__ (L15)                                            |   COVERED |
+|     Foo.__repr__ (L19)                                           |    MISSED |
+|     Foo._semiprivate_documented (L22)                            |   COVERED |
+|     Foo._semiprivate_undocumented (L26)                          |    MISSED |
+|     Foo.__private (L29)                                          |    MISSED |
+|     Foo.method_foo (L32)                                         |    MISSED |
+|     Foo.get (L35)                                                |    MISSED |
+|     Foo.get (L38)                                                |    MISSED |
+|     Foo.a_prop (L42)                                             |    MISSED |
+|     Foo.a_prop (L46)                                             |    MISSED |
+|     Foo.a_prop (L50)                                             |   COVERED |
+|     Foo.module_overload (L54)                                    |    MISSED |
+|     Foo.module_overload (L57)                                    |    MISSED |
+|     Foo.module_overload (L59)                                    |   COVERED |
+|     Foo.simple_overload (L64)                                    |    MISSED |
+|     Foo.simple_overload (L67)                                    |    MISSED |
+|     Foo.simple_overload (L69)                                    |   COVERED |
+|   documented_top_level_func (L74)                                |   COVERED |
+|     documented_top_level_func.documented_inner_func (L77)        |   COVERED |
+|   undocumented_top_level_func (L82)                              |    MISSED |
+|     undocumented_top_level_func.undocumented_inner_func (L83)    |    MISSED |
+|   Bar (L87)                                                      |    MISSED |
+|     Bar.method_bar (L88)                                         |    MISSED |
+|       Bar.method_bar.InnerBar (L89)                              |    MISSED |
+|   _SemiprivateClass (L93)                                        |    MISSED |
+|   __PrivateClass (L97)                                           |    MISSED |
+|------------------------------------------------------------------|-----------|
+| child_sample/__init__.py (module)                                |    MISSED |
+|------------------------------------------------------------------|-----------|
+| child_sample/child_sample_module.py (module)                     |    MISSED |
+|   ChildFoo (L5)                                                  |    MISSED |
+|     ChildFoo.__init__ (L6)                                       |    MISSED |
+|     ChildFoo.__str__ (L9)                                        |    MISSED |
+|     ChildFoo._ignore_me (L12)                                    |    MISSED |
+|     ChildFoo.__ignore_me_too (L15)                               |    MISSED |
+|     ChildFoo.method_foo (L18)                                    |    MISSED |
+|   a_child_func (L22)                                             |    MISSED |
+|   ChildBar (L26)                                                 |    MISSED |
+|     ChildBar.method_bar (L27)                                    |    MISSED |
+|       ChildBar.method_bar.InnerBar (L28)                         |    MISSED |
+|   _ChildBaz (L34)                                                |    MISSED |
+|   __ChildBla (L38)                                               |    MISSED |
+|------------------------------------------------------------------|-----------|
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed_no_module.txt` & `interrogate-1.7.0/tests/functional/fixtures/windows/expected_detailed_no_module.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,56 +8,62 @@
 |     Foo._semiprivate (L19)                                      |   COVERED |
 |     Foo.__private (L23)                                         |   COVERED |
 |     Foo.method_foo (L27)                                        |   COVERED |
 |     Foo.get (L31)                                               |   COVERED |
 |     Foo.get (L35)                                               |   COVERED |
 |     Foo.prop (L40)                                              |   COVERED |
 |     Foo.prop (L45)                                              |   COVERED |
-|     Foo.module_overload (L50)                                   |   COVERED |
+|     Foo.prop (L50)                                              |   COVERED |
 |     Foo.module_overload (L55)                                   |   COVERED |
-|     Foo.module_overload (L59)                                   |   COVERED |
-|     Foo.simple_overload (L64)                                   |   COVERED |
+|     Foo.module_overload (L60)                                   |   COVERED |
+|     Foo.module_overload (L64)                                   |   COVERED |
 |     Foo.simple_overload (L69)                                   |   COVERED |
-|     Foo.simple_overload (L73)                                   |   COVERED |
-|   top_level_func (L78)                                          |   COVERED |
-|     top_level_func.inner_func (L81)                             |   COVERED |
-|   Bar (L86)                                                     |   COVERED |
-|     Bar.method_bar (L89)                                        |   COVERED |
-|       Bar.method_bar.InnerBar (L92)                             |   COVERED |
-|   _SemiprivateClass (L98)                                       |   COVERED |
-|   __PrivateClass (L104)                                         |   COVERED |
+|     Foo.simple_overload (L74)                                   |   COVERED |
+|     Foo.simple_overload (L78)                                   |   COVERED |
+|   top_level_func (L83)                                          |   COVERED |
+|     top_level_func.inner_func (L86)                             |   COVERED |
+|   Bar (L91)                                                     |   COVERED |
+|     Bar.method_bar (L94)                                        |   COVERED |
+|       Bar.method_bar.InnerBar (L97)                             |   COVERED |
+|   _SemiprivateClass (L103)                                      |   COVERED |
+|   __PrivateClass (L109)                                         |   COVERED |
+|   InitDocs (L116)                                               |   COVERED |
+|     InitDocs.__init__ (L117)                                    |   COVERED |
+|   ClassDocs (L123)                                              |   COVERED |
+|     ClassDocs.__init__ (L126)                                   |   COVERED |
 |-----------------------------------------------------------------|-----------|
 | partial.py                                                      |           |
 |   Foo (L8)                                                      |   COVERED |
 |     Foo.__init__ (L11)                                          |   COVERED |
 |     Foo.__str__ (L15)                                           |   COVERED |
 |     Foo.__repr__ (L19)                                          |    MISSED |
 |     Foo._semiprivate_documented (L22)                           |   COVERED |
 |     Foo._semiprivate_undocumented (L26)                         |    MISSED |
 |     Foo.__private (L29)                                         |    MISSED |
 |     Foo.method_foo (L32)                                        |    MISSED |
 |     Foo.get (L35)                                               |    MISSED |
 |     Foo.get (L38)                                               |    MISSED |
 |     Foo.a_prop (L42)                                            |    MISSED |
 |     Foo.a_prop (L46)                                            |    MISSED |
-|     Foo.module_overload (L50)                                   |    MISSED |
-|     Foo.module_overload (L53)                                   |    MISSED |
-|     Foo.module_overload (L55)                                   |   COVERED |
-|     Foo.simple_overload (L60)                                   |    MISSED |
-|     Foo.simple_overload (L63)                                   |    MISSED |
-|     Foo.simple_overload (L65)                                   |   COVERED |
-|   documented_top_level_func (L70)                               |   COVERED |
-|     documented_top_level_func.documented_inner_func (L73)       |   COVERED |
-|   undocumented_top_level_func (L78)                             |    MISSED |
-|     undocumented_top_level_func.undocumented_inner_func (L79)   |    MISSED |
-|   Bar (L83)                                                     |    MISSED |
-|     Bar.method_bar (L84)                                        |    MISSED |
-|       Bar.method_bar.InnerBar (L85)                             |    MISSED |
-|   _SemiprivateClass (L89)                                       |    MISSED |
-|   __PrivateClass (L93)                                          |    MISSED |
+|     Foo.a_prop (L50)                                            |   COVERED |
+|     Foo.module_overload (L54)                                   |    MISSED |
+|     Foo.module_overload (L57)                                   |    MISSED |
+|     Foo.module_overload (L59)                                   |   COVERED |
+|     Foo.simple_overload (L64)                                   |    MISSED |
+|     Foo.simple_overload (L67)                                   |    MISSED |
+|     Foo.simple_overload (L69)                                   |   COVERED |
+|   documented_top_level_func (L74)                               |   COVERED |
+|     documented_top_level_func.documented_inner_func (L77)       |   COVERED |
+|   undocumented_top_level_func (L82)                             |    MISSED |
+|     undocumented_top_level_func.undocumented_inner_func (L83)   |    MISSED |
+|   Bar (L87)                                                     |    MISSED |
+|     Bar.method_bar (L88)                                        |    MISSED |
+|       Bar.method_bar.InnerBar (L89)                             |    MISSED |
+|   _SemiprivateClass (L93)                                       |    MISSED |
+|   __PrivateClass (L97)                                          |    MISSED |
 |-----------------------------------------------------------------|-----------|
 | child_sample\child_sample_module.py                             |           |
 |   ChildFoo (L5)                                                 |    MISSED |
 |     ChildFoo.__init__ (L6)                                      |    MISSED |
 |     ChildFoo.__str__ (L9)                                       |    MISSED |
 |     ChildFoo._ignore_me (L12)                                   |    MISSED |
 |     ChildFoo.__ignore_me_too (L15)                              |    MISSED |
@@ -69,13 +75,13 @@
 |   _ChildBaz (L34)                                               |    MISSED |
 |   __ChildBla (L38)                                              |    MISSED |
 |-----------------------------------------------------------------|-----------|
 
 ----------------------------------- Summary -----------------------------------
 | Name                                    |  Total |  Miss |  Cover |  Cover% |
 |-----------------------------------------|--------|-------|--------|---------|
-| full.py                                 |     23 |     0 |     23 |    100% |
-| partial.py                              |     27 |    19 |      8 |     30% |
+| full.py                                 |     28 |     0 |     28 |    100% |
+| partial.py                              |     28 |    19 |      9 |     32% |
 | child_sample\child_sample_module.py     |     12 |    12 |      0 |      0% |
 |-----------------------------------------|--------|-------|--------|---------|
-| TOTAL                                   |     62 |    31 |     31 |   50.0% |
---------------- RESULT: FAILED (minimum: 80.0%, actual: 50.0%) ----------------
+| TOTAL                                   |     68 |    31 |     37 |   54.4% |
+--------------- RESULT: FAILED (minimum: 80.0%, actual: 54.4%) ----------------
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed_single_file.txt` & `interrogate-1.7.0/tests/functional/fixtures/windows/expected_detailed_single_file.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,29 +8,34 @@
 |     Foo._semiprivate (L19)                         |                COVERED |
 |     Foo.__private (L23)                            |                COVERED |
 |     Foo.method_foo (L27)                           |                COVERED |
 |     Foo.get (L31)                                  |                COVERED |
 |     Foo.get (L35)                                  |                COVERED |
 |     Foo.prop (L40)                                 |                COVERED |
 |     Foo.prop (L45)                                 |                COVERED |
-|     Foo.module_overload (L50)                      |                COVERED |
+|     Foo.prop (L50)                                 |                COVERED |
 |     Foo.module_overload (L55)                      |                COVERED |
-|     Foo.module_overload (L59)                      |                COVERED |
-|     Foo.simple_overload (L64)                      |                COVERED |
+|     Foo.module_overload (L60)                      |                COVERED |
+|     Foo.module_overload (L64)                      |                COVERED |
 |     Foo.simple_overload (L69)                      |                COVERED |
-|     Foo.simple_overload (L73)                      |                COVERED |
-|   top_level_func (L78)                             |                COVERED |
-|     top_level_func.inner_func (L81)                |                COVERED |
-|   Bar (L86)                                        |                COVERED |
-|     Bar.method_bar (L89)                           |                COVERED |
-|       Bar.method_bar.InnerBar (L92)                |                COVERED |
-|   _SemiprivateClass (L98)                          |                COVERED |
-|   __PrivateClass (L104)                            |                COVERED |
+|     Foo.simple_overload (L74)                      |                COVERED |
+|     Foo.simple_overload (L78)                      |                COVERED |
+|   top_level_func (L83)                             |                COVERED |
+|     top_level_func.inner_func (L86)                |                COVERED |
+|   Bar (L91)                                        |                COVERED |
+|     Bar.method_bar (L94)                           |                COVERED |
+|       Bar.method_bar.InnerBar (L97)                |                COVERED |
+|   _SemiprivateClass (L103)                         |                COVERED |
+|   __PrivateClass (L109)                            |                COVERED |
+|   InitDocs (L116)                                  |                COVERED |
+|     InitDocs.__init__ (L117)                       |                COVERED |
+|   ClassDocs (L123)                                 |                COVERED |
+|     ClassDocs.__init__ (L126)                      |                COVERED |
 |----------------------------------------------------|------------------------|
 
 ----------------------------------- Summary -----------------------------------
 | Name            |        Total |        Miss |        Cover |        Cover% |
 |-----------------|--------------|-------------|--------------|---------------|
-| full.py         |           24 |           0 |           24 |          100% |
+| full.py         |           29 |           0 |           29 |          100% |
 |-----------------|--------------|-------------|--------------|---------------|
-| TOTAL           |           24 |           0 |           24 |        100.0% |
+| TOTAL           |           29 |           0 |           29 |        100.0% |
 --------------- RESULT: PASSED (minimum: 80.0%, actual: 100.0%) ---------------
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed_skip_covered.txt` & `interrogate-1.7.0/tests/functional/fixtures/windows/expected_detailed_skip_covered.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,29 +12,30 @@
 |     Foo._semiprivate_undocumented (L26)                         |    MISSED |
 |     Foo.__private (L29)                                         |    MISSED |
 |     Foo.method_foo (L32)                                        |    MISSED |
 |     Foo.get (L35)                                               |    MISSED |
 |     Foo.get (L38)                                               |    MISSED |
 |     Foo.a_prop (L42)                                            |    MISSED |
 |     Foo.a_prop (L46)                                            |    MISSED |
-|     Foo.module_overload (L50)                                   |    MISSED |
-|     Foo.module_overload (L53)                                   |    MISSED |
-|     Foo.module_overload (L55)                                   |   COVERED |
-|     Foo.simple_overload (L60)                                   |    MISSED |
-|     Foo.simple_overload (L63)                                   |    MISSED |
-|     Foo.simple_overload (L65)                                   |   COVERED |
-|   documented_top_level_func (L70)                               |   COVERED |
-|     documented_top_level_func.documented_inner_func (L73)       |   COVERED |
-|   undocumented_top_level_func (L78)                             |    MISSED |
-|     undocumented_top_level_func.undocumented_inner_func (L79)   |    MISSED |
-|   Bar (L83)                                                     |    MISSED |
-|     Bar.method_bar (L84)                                        |    MISSED |
-|       Bar.method_bar.InnerBar (L85)                             |    MISSED |
-|   _SemiprivateClass (L89)                                       |    MISSED |
-|   __PrivateClass (L93)                                          |    MISSED |
+|     Foo.a_prop (L50)                                            |   COVERED |
+|     Foo.module_overload (L54)                                   |    MISSED |
+|     Foo.module_overload (L57)                                   |    MISSED |
+|     Foo.module_overload (L59)                                   |   COVERED |
+|     Foo.simple_overload (L64)                                   |    MISSED |
+|     Foo.simple_overload (L67)                                   |    MISSED |
+|     Foo.simple_overload (L69)                                   |   COVERED |
+|   documented_top_level_func (L74)                               |   COVERED |
+|     documented_top_level_func.documented_inner_func (L77)       |   COVERED |
+|   undocumented_top_level_func (L82)                             |    MISSED |
+|     undocumented_top_level_func.undocumented_inner_func (L83)   |    MISSED |
+|   Bar (L87)                                                     |    MISSED |
+|     Bar.method_bar (L88)                                        |    MISSED |
+|       Bar.method_bar.InnerBar (L89)                             |    MISSED |
+|   _SemiprivateClass (L93)                                       |    MISSED |
+|   __PrivateClass (L97)                                          |    MISSED |
 |-----------------------------------------------------------------|-----------|
 | child_sample\__init__.py (module)                               |    MISSED |
 |-----------------------------------------------------------------|-----------|
 | child_sample\child_sample_module.py (module)                    |    MISSED |
 |   ChildFoo (L5)                                                 |    MISSED |
 |     ChildFoo.__init__ (L6)                                      |    MISSED |
 |     ChildFoo.__str__ (L9)                                       |    MISSED |
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary.txt` & `interrogate-1.7.0/tests/functional/fixtures/windows/expected_summary.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 | Name                                    |  Total |  Miss |  Cover |  Cover% |
 |-----------------------------------------|--------|-------|--------|---------|
 | __init__.py                             |      1 |     0 |      1 |    100% |
 | empty.py                                |      1 |     1 |      0 |      0% |
-| full.py                                 |     24 |     0 |     24 |    100% |
-| partial.py                              |     28 |    19 |      9 |     32% |
+| full.py                                 |     29 |     0 |     29 |    100% |
+| partial.py                              |     29 |    19 |     10 |     34% |
 | child_sample\__init__.py                |      1 |     1 |      0 |      0% |
 | child_sample\child_sample_module.py     |     13 |    13 |      0 |      0% |
 |-----------------------------------------|--------|-------|--------|---------|
-| TOTAL                                   |     68 |    34 |     34 |   50.0% |
+| TOTAL                                   |     74 |    34 |     40 |   54.1% |
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary_no_module.txt` & `interrogate-1.7.0/tests/functional/fixtures/windows/expected_summary_no_module.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 ----------------------------------- Summary -----------------------------------
 | Name                                    |  Total |  Miss |  Cover |  Cover% |
 |-----------------------------------------|--------|-------|--------|---------|
-| full.py                                 |     23 |     0 |     23 |    100% |
-| partial.py                              |     27 |    19 |      8 |     30% |
+| full.py                                 |     28 |     0 |     28 |    100% |
+| partial.py                              |     28 |    19 |      9 |     32% |
 | child_sample\child_sample_module.py     |     12 |    12 |      0 |      0% |
 |-----------------------------------------|--------|-------|--------|---------|
+| TOTAL                                   |     68 |    31 |     37 |   54.4% |
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary_skip_covered.txt` & `interrogate-1.7.0/tests/functional/fixtures/expected_summary.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-| Name                                    |  Total |  Miss |  Cover |  Cover% |
-|-----------------------------------------|--------|-------|--------|---------|
-| empty.py                                |      1 |     1 |      0 |      0% |
-| partial.py                              |     28 |    19 |      9 |     32% |
-| child_sample\__init__.py                |      1 |     1 |      0 |      0% |
-| child_sample\child_sample_module.py     |     13 |    13 |      0 |      0% |
-|-----------------------------------------|--------|-------|--------|---------|
-| TOTAL                                   |     68 |    34 |     34 |   50.0% |
+| Name                                     |  Total |  Miss |  Cover |  Cover% |
+|------------------------------------------|--------|-------|--------|---------|
+| __init__.py                              |      1 |     0 |      1 |    100% |
+| empty.py                                 |      1 |     1 |      0 |      0% |
+| full.py                                  |     29 |     0 |     29 |    100% |
+| partial.py                               |     29 |    19 |     10 |     34% |
+| child_sample/__init__.py                 |      1 |     1 |      0 |      0% |
+| child_sample/child_sample_module.py      |     13 |    13 |      0 |      0% |
+|------------------------------------------|--------|-------|--------|---------|
+| TOTAL                                    |     74 |    34 |     40 |   54.1% |
```

### Comparing `interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary_skip_covered_all.txt` & `interrogate-1.7.0/tests/functional/fixtures/windows/expected_summary_skip_covered_all.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 ----------------------------------- Summary -----------------------------------
 | Name            |        Total |        Miss |        Cover |        Cover% |
 |-----------------|--------------|-------------|--------------|---------------|
-| TOTAL           |           24 |           0 |           24 |        100.0% |
+| TOTAL           |           29 |           0 |           29 |        100.0% |
 |-----------------------------------------------------------------------------|
 |               (1 of 1 file omitted due to complete coverage)                |
 --------------- RESULT: PASSED (minimum: 80.0%, actual: 100.0%) ---------------
```

### Comparing `interrogate-1.6.0/tests/functional/sample/full.py` & `interrogate-1.7.0/tests/functional/sample/full.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,14 +42,19 @@
         pass
 
     @prop.setter
     def prop(self):
         """this method has a set property decorator"""
         pass
 
+    @prop.deleter
+    def prop(self):
+        """this method as a del property decorator"""
+        pass
+
     @typing.overload
     def module_overload(a: None) -> None:
         """overloaded method"""
         ...
 
     @typing.overload
     def module_overload(a: int) -> int:
@@ -101,7 +106,22 @@
     pass
 
 
 class __PrivateClass:
     """a private class"""
 
     pass
+
+
+# Coverage % for InitDocs should be the same as ClassDocs
+class InitDocs:
+    def __init__(self):
+        """A docstring for init"""
+        pass
+
+
+# Coverage % for ClassDocs should be the same as InitDocs
+class ClassDocs:
+    """A docstring for a class"""
+
+    def __init__(self):
+        pass
```

### Comparing `interrogate-1.6.0/tests/functional/sample/partial.py` & `interrogate-1.7.0/tests/functional/sample/partial.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     def a_prop(self):
         pass
 
     @a_prop.setter
     def a_prop(self, x):
         pass
 
+    @a_prop.deleter
+    def a_prop(self):
+        """A documented del property decorator"""
+
     @typing.overload
     def module_overload(a: None) -> None: ...
 
     @typing.overload
     def module_overload(a: int) -> int: ...
 
     def module_overload(a):
```

### Comparing `interrogate-1.6.0/tests/functional/test_cli.py` & `interrogate-1.7.0/tests/functional/test_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,55 +29,55 @@
 
 def test_run_no_paths(runner, monkeypatch, tmpdir):
     """Assume current working directory if no paths are given."""
     monkeypatch.setattr(os, "getcwd", lambda: SAMPLE_DIR)
 
     result = runner.invoke(cli.main, [])
 
-    assert "actual: 50.0%" in result.output
+    assert "actual: 51.4%" in result.output
     assert 1 == result.exit_code
 
 
 @pytest.mark.parametrize(
     "flags,exp_result,exp_exit_code",
     (
         # no flags
-        ([], 50.0, 1),
+        ([], 51.4, 1),
         # ignore init module
-        (["-I"], 50.0, 1),
+        (["-I"], 51.4, 1),
         # ignore module docs
-        (["-M"], 50.0, 1),
+        (["-M"], 51.5, 1),
         # ignore semiprivate docs
-        (["-s"], 50.8, 1),
+        (["-s"], 52.2, 1),
         # ignore private docs
-        (["-p"], 51.6, 1),
-        # ignore property getter/setter decorators
+        (["-p"], 52.9, 1),
+        # ignore property getter/setter/deleter decorators
         (["-P"], 50.0, 1),
         # ignore property setter decorators
-        (["-S"], 50.0, 1),
+        (["-S"], 51.4, 1),
         # ignore magic method docs
-        (["-m"], 50.0, 1),
+        (["-m"], 51.4, 1),
         # ignore init method docs
-        (["-i"], 49.2, 1),
+        (["-i"], 50.7, 1),
         # ignore nested funcs
-        (["-n"], 49.2, 1),
+        (["-n"], 50.7, 1),
         # ignore nested classes
-        (["-C"], 50.8, 1),
+        (["-C"], 52.1, 1),
         # ignore @typing.overload-decorated functions
-        (["-O"], 50.0, 1),
+        (["-O"], 51.5, 1),
         # ignore regex
-        (["-r", "^get$"], 50.0, 1),
+        (["-r", "^get$"], 51.4, 1),
         # whitelist regex
         (["-w", "^get$"], 50.0, 1),
         # exclude file
-        (["-e", os.path.join(SAMPLE_DIR, "partial.py")], 62.5, 1),
+        (["-e", os.path.join(SAMPLE_DIR, "partial.py")], 62.2, 1),
         # exclude file which doesn't exist
-        (["-e", os.path.join(SAMPLE_DIR, "does.not.exist")], 50.0, 1),
+        (["-e", os.path.join(SAMPLE_DIR, "does.not.exist")], 51.4, 1),
         # fail under
-        (["-f", "40"], 50.0, 0),
+        (["-f", "40"], 51.4, 0),
     ),
 )
 def test_run_shortflags(flags, exp_result, exp_exit_code, runner):
     """Test CLI with single short flags"""
     cli_inputs = flags + [SAMPLE_DIR]
     result = runner.invoke(cli.main, cli_inputs)
 
@@ -85,29 +85,31 @@
     assert exp_partial_output in result.output
     assert exp_exit_code == result.exit_code
 
 
 @pytest.mark.parametrize(
     "flags,exp_result,exp_exit_code",
     (
-        (["--ignore-init-module"], 50.0, 1),
-        (["--ignore-module"], 50.0, 1),
-        (["--ignore-semiprivate"], 50.8, 1),
-        (["--ignore-private"], 51.6, 1),
+        (["--ignore-init-module"], 51.4, 1),
+        (["--ignore-module"], 51.5, 1),
+        (["--ignore-semiprivate"], 52.2, 1),
+        (["--ignore-private"], 52.9, 1),
         (["--ignore-property-decorators"], 50.0, 1),
-        (["--ignore-setters"], 50.0, 1),
-        (["--ignore-magic"], 50.0, 1),
-        (["--ignore-init-method"], 49.2, 1),
-        (["--ignore-nested-functions"], 49.2, 1),
-        (["--ignore-nested-classes"], 50.8, 1),
-        (["--ignore-overloaded-functions"], 50.0, 1),
-        (["--ignore-regex", "^get$"], 50.0, 1),
+        (["--ignore-setters"], 51.4, 1),
+        (["--ignore-magic"], 51.4, 1),
+        (["--ignore-init-method"], 50.7, 1),
+        (["--ignore-nested-functions"], 50.7, 1),
+        (["--ignore-nested-classes"], 52.1, 1),
+        (["--ignore-overloaded-functions"], 51.5, 1),
+        (["--ignore-regex", "^get$"], 51.4, 1),
+        (["--ext", "pyi"], 63.1, 1),
         (["--whitelist-regex", "^get$"], 50.0, 1),
-        (["--exclude", os.path.join(SAMPLE_DIR, "partial.py")], 62.5, 1),
-        (["--fail-under", "40"], 50.0, 0),
+        (["--exclude", os.path.join(SAMPLE_DIR, "partial.py")], 62.2, 1),
+        (["--fail-under", "40"], 51.4, 0),
+        (["--style", "google"], 54.1, 1),
     ),
 )
 def test_run_longflags(flags, exp_result, exp_exit_code, runner):
     """Test CLI with single long flags"""
     cli_inputs = flags + [SAMPLE_DIR]
     result = runner.invoke(cli.main, cli_inputs)
 
@@ -115,17 +117,17 @@
     assert exp_partial_output in result.output
     assert exp_exit_code == result.exit_code
 
 
 @pytest.mark.parametrize(
     "flags,exp_result,exp_exit_code",
     (
-        (["-i", "-I", "-r" "^method_foo$"], 50.0, 1),
-        (["-s", "-p", "-M"], 53.1, 1),
-        (["-m", "-f", "45"], 50.0, 0),
+        (["-i", "-I", "-r" "^method_foo$"], 51.6, 1),
+        (["-s", "-p", "-M"], 54.5, 1),
+        (["-m", "-f", "45"], 51.4, 0),
     ),
 )
 def test_run_multiple_flags(flags, exp_result, exp_exit_code, runner):
     """Test CLI with a hodge-podge of flags"""
     cli_inputs = flags + [SAMPLE_DIR]
     result = runner.invoke(cli.main, cli_inputs)
```

### Comparing `interrogate-1.6.0/tests/functional/test_coverage.py` & `interrogate-1.7.0/tests/functional/test_coverage.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,44 +40,44 @@
             (0, 0, 0, "100.0"),
         ),
         (
             [
                 SAMPLE_DIR,
             ],
             {},
-            (68, 34, 34, "50.0"),
+            (74, 38, 36, "51.4"),
         ),
-        ([os.path.join(SAMPLE_DIR, "partial.py")], {}, (28, 9, 19, "32.1")),
+        ([os.path.join(SAMPLE_DIR, "partial.py")], {}, (29, 10, 19, "34.5")),
         (
             [
                 os.path.join(SAMPLE_DIR, "full.py"),
             ],
             {"ignore_nested_functions": True},
-            (23, 23, 0, "100.0"),
+            (28, 26, 2, "92.9"),
         ),
         (
             [
                 os.path.join(SAMPLE_DIR, "partial.py"),
             ],
             {"ignore_nested_functions": True},
-            (26, 8, 18, "30.8"),
+            (27, 9, 18, "33.3"),
         ),
         (
             [
                 os.path.join(SAMPLE_DIR, "full.py"),
             ],
             {"ignore_overloaded_functions": True},
-            (20, 20, 0, "100.0"),
+            (25, 23, 2, "92.0"),
         ),
         (
             [
                 os.path.join(SAMPLE_DIR, "partial.py"),
             ],
             {"ignore_overloaded_functions": True},
-            (24, 9, 15, "37.5"),
+            (25, 10, 15, "40.0"),
         ),
     ),
 )
 def test_coverage_simple(paths, conf, exp_results, mocker):
     """Happy path - get expected results given a file or directory"""
     conf = config.InterrogateConfig(**conf)
     interrogate_coverage = coverage.InterrogateCoverage(paths=paths, conf=conf)
@@ -103,28 +103,34 @@
 
     interrogate_coverage = coverage.InterrogateCoverage(paths=[FIXTURES])
 
     with pytest.raises(SystemExit, match="1"):
         interrogate_coverage.get_coverage()
 
     captured = capsys.readouterr()
-    assert "E: No Python files found to interrogate in " in captured.err
+    assert (
+        "E: No Python or Python-like files found to interrogate in "
+        in captured.err
+    )
 
 
 @pytest.mark.parametrize(
     "level,exp_fixture_file",
     (
         (0, "expected_no_verbosity.txt"),
         (1, "expected_summary.txt"),
         (2, "expected_detailed.txt"),
     ),
 )
 def test_print_results(level, exp_fixture_file, capsys, monkeypatch):
     """Output of test results differ by verbosity."""
-    interrogate_coverage = coverage.InterrogateCoverage(paths=[SAMPLE_DIR])
+    interrogate_config = config.InterrogateConfig(docstring_style="google")
+    interrogate_coverage = coverage.InterrogateCoverage(
+        paths=[SAMPLE_DIR], conf=interrogate_config
+    )
     results = interrogate_coverage.get_coverage()
     interrogate_coverage.print_results(
         results=results, output=None, verbosity=level
     )
 
     captured = capsys.readouterr()
     expected_fixture = os.path.join(FIXTURES, exp_fixture_file)
@@ -145,15 +151,17 @@
         (2, "expected_detailed_skip_covered.txt"),
     ),
 )
 def test_print_results_omit_covered(
     level, exp_fixture_file, capsys, monkeypatch
 ):
     """Output of results differ by verbosity, omitting fully covered files."""
-    interrogate_config = config.InterrogateConfig(omit_covered_files=True)
+    interrogate_config = config.InterrogateConfig(
+        omit_covered_files=True, docstring_style="google"
+    )
     interrogate_coverage = coverage.InterrogateCoverage(
         paths=[SAMPLE_DIR], conf=interrogate_config
     )
     results = interrogate_coverage.get_coverage()
     interrogate_coverage.print_results(
         results=results, output=None, verbosity=level
     )
@@ -183,15 +191,17 @@
 
     captured = capsys.readouterr()
     assert "omitted due to complete coverage" not in captured.out
 
 
 def test_print_results_omit_all_summary(capsys, monkeypatch):
     """Output of test results for summary view, omitting all covered files."""
-    interrogate_config = config.InterrogateConfig(omit_covered_files=True)
+    interrogate_config = config.InterrogateConfig(
+        omit_covered_files=True, docstring_style="google"
+    )
     interrogate_coverage = coverage.InterrogateCoverage(
         paths=[os.path.join(SAMPLE_DIR, "full.py")], conf=interrogate_config
     )
     results = interrogate_coverage.get_coverage()
     interrogate_coverage.print_results(
         results=results, output=None, verbosity=1
     )
@@ -205,15 +215,17 @@
         expected_out = f.read()
 
     assert expected_out in captured.out
 
 
 def test_print_results_omit_all_detailed(capsys, monkeypatch):
     """Show no detail view when all files are omitted from skipping covered"""
-    interrogate_config = config.InterrogateConfig(omit_covered_files=True)
+    interrogate_config = config.InterrogateConfig(
+        omit_covered_files=True, docstring_style="google"
+    )
     interrogate_coverage = coverage.InterrogateCoverage(
         paths=[os.path.join(SAMPLE_DIR, "full.py")], conf=interrogate_config
     )
     results = interrogate_coverage.get_coverage()
     interrogate_coverage.print_results(
         results=results, output=None, verbosity=2
     )
@@ -233,15 +245,15 @@
         (True, 1, "expected_summary_no_module.txt"),
     ),
 )
 def test_print_results_ignore_module(
     ignore_module, level, exp_fixture_file, capsys, monkeypatch
 ):
     """Do not print module info if ignore_module is True."""
-    conf = {"ignore_module": ignore_module}
+    conf = {"ignore_module": ignore_module, "docstring_style": "google"}
     conf = config.InterrogateConfig(**conf)
 
     interrogate_coverage = coverage.InterrogateCoverage(
         paths=[SAMPLE_DIR], conf=conf
     )
     results = interrogate_coverage.get_coverage()
     interrogate_coverage.print_results(
@@ -257,15 +269,19 @@
 
     assert expected_out in captured.out
 
 
 def test_print_results_single_file(capsys, monkeypatch):
     """Results for a single file should still list the filename."""
     single_file = os.path.join(SAMPLE_DIR, "full.py")
-    interrogate_coverage = coverage.InterrogateCoverage(paths=[single_file])
+    conf = {"docstring_style": "google"}
+    conf = config.InterrogateConfig(**conf)
+    interrogate_coverage = coverage.InterrogateCoverage(
+        paths=[single_file], conf=conf
+    )
     results = interrogate_coverage.get_coverage()
     interrogate_coverage.print_results(
         results=results, output=None, verbosity=2
     )
 
     captured = capsys.readouterr()
     expected_fixture = os.path.join(
@@ -285,7 +301,36 @@
     # everywhere
     if not IS_WINDOWS:
         assert "tests/functional/sample/" in captured.out
         assert "tests/functional/sample/full.py" not in captured.out
     else:
         assert "tests\\functional\\sample\\" in captured.out
         assert "tests\\functional\\sample\\full.py" not in captured.out
+
+
+@pytest.mark.parametrize(
+    "fail_under,perc_covered,exp_ret",
+    [
+        (48.3, 48.27, 0),
+        (48.36, 48.359, 0),
+        (48.35, 48.349, 0),
+        (48.55, 48.500, 1),
+        (50.999999, 50.999998, 1),
+        (50.999999, 50.999999, 0),
+    ],
+)
+def test_pass_when_fail_under_exact(
+    fail_under, perc_covered, exp_ret, monkeypatch
+):
+    """Pass if actual coverage is exactly the `--fail-under` value.
+    See issue `#114 <https://github.com/econchick/interrogate/issues/114>`_.
+    """
+    monkeypatch.setattr(
+        coverage.InterrogateResults, "perc_covered", perc_covered
+    )
+
+    interrogate_config = config.InterrogateConfig(fail_under=fail_under)
+    interrogate_coverage = coverage.InterrogateCoverage(
+        paths=[SAMPLE_DIR], conf=interrogate_config
+    )
+    results = interrogate_coverage.get_coverage()
+    assert exp_ret == results.ret_code
```

### Comparing `interrogate-1.6.0/tests/unit/fixtures/default-style/0.svg` & `interrogate-1.7.0/tests/unit/fixtures/default-style/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/default-style/100.svg` & `interrogate-1.7.0/tests/unit/fixtures/default-style/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/default-style/45.svg` & `interrogate-1.7.0/tests/unit/fixtures/default-style/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/default-style/60.svg` & `interrogate-1.7.0/tests/unit/fixtures/default-style/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/default-style/89.svg` & `interrogate-1.7.0/tests/unit/fixtures/default-style/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/default-style/90.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/90.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/default-style/99.png` & `interrogate-1.7.0/tests/unit/fixtures/default-style/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/default-style/99.svg` & `interrogate-1.7.0/tests/unit/fixtures/default-style/99.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/default-style/default.svg` & `interrogate-1.7.0/tests/unit/fixtures/default-style/default.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/default-style/no_logo.svg` & `interrogate-1.7.0/tests/unit/fixtures/default-style/no_logo.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat/0.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat/100.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat/45.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat/60.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat/89.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat/90.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat/90.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat/99.png` & `interrogate-1.7.0/tests/unit/fixtures/flat/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat/99.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat/99.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat/default.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat/default.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square/0.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square/100.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square/45.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square/60.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square/89.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square/90.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square/90.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square/99.png` & `interrogate-1.7.0/tests/unit/fixtures/flat-square/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square/99.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square/99.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square/default.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square/default.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/0.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/100.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/45.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/60.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/89.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/90.svg` & `interrogate-1.7.0/tests/functional/fixtures/expected_badge.svg`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 2e63 6f6d 2f22 2073 7479 6c65 3d22 6669  .com/" style="fi
 000000d0: 6c6c 2d72 756c 653a 6576 656e 6f64 643b  ll-rule:evenodd;
 000000e0: 636c 6970 2d72 756c 653a 6576 656e 6f64  clip-rule:evenod
 000000f0: 643b 7374 726f 6b65 2d6c 696e 656a 6f69  d;stroke-linejoi
 00000100: 6e3a 726f 756e 643b 7374 726f 6b65 2d6d  n:round;stroke-m
 00000110: 6974 6572 6c69 6d69 743a 323b 223e 0a20  iterlimit:2;">. 
 00000120: 2020 203c 7469 746c 653e 696e 7465 7272     <title>interr
-00000130: 6f67 6174 653a 2039 302e 3025 3c2f 7469  ogate: 90.0%</ti
+00000130: 6f67 6174 653a 2035 312e 3425 3c2f 7469  ogate: 51.4%</ti
 00000140: 746c 653e 0a20 2020 203c 6720 7472 616e  tle>.    <g tran
 00000150: 7366 6f72 6d3d 226d 6174 7269 7828 312c  sform="matrix(1,
 00000160: 302c 302c 312c 3232 2c30 2922 3e0a 2020  0,0,1,22,0)">.  
 00000170: 2020 2020 2020 3c67 2069 643d 2262 6163        <g id="bac
 00000180: 6b67 726f 756e 6473 2220 7472 616e 7366  kgrounds" transf
 00000190: 6f72 6d3d 226d 6174 7269 7828 312e 3332  orm="matrix(1.32
 000001a0: 3738 392c 302c 302c 312c 2d32 322e 3338  789,0,0,1,-22.38
@@ -33,15 +33,15 @@
 00000200: 3835 2c38 3529 3b22 2f3e 0a20 2020 2020  85,85);"/>.     
 00000210: 2020 203c 2f67 3e0a 2020 2020 2020 2020     </g>.        
 00000220: 3c72 6563 7420 783d 2237 3122 2079 3d22  <rect x="71" y="
 00000230: 3022 2077 6964 7468 3d22 3437 2220 6865  0" width="47" he
 00000240: 6967 6874 3d22 3230 2220 6461 7461 2d69  ight="20" data-i
 00000250: 6e74 6572 726f 6761 7465 3d22 636f 6c6f  nterrogate="colo
 00000260: 7222 2073 7479 6c65 3d22 6669 6c6c 3a23  r" style="fill:#
-00000270: 3937 4341 3030 222f 3e0a 2020 2020 2020  97CA00"/>.      
+00000270: 6665 3764 3337 222f 3e0a 2020 2020 2020  fe7d37"/>.      
 00000280: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
 00000290: 6d61 7472 6978 2831 2e31 3937 3436 2c30  matrix(1.19746,0
 000002a0: 2c30 2c31 2c2d 3232 2e33 3734 342c 2d34  ,0,1,-22.3744,-4
 000002b0: 2e38 3537 3233 652d 3136 2922 3e0a 2020  .85723e-16)">.  
 000002c0: 2020 2020 2020 2020 2020 3c72 6563 7420            <rect 
 000002d0: 783d 2230 2220 793d 2230 2220 7769 6474  x="0" y="0" widt
 000002e0: 683d 2231 3138 2220 6865 6967 6874 3d22  h="118" height="
@@ -72,22 +72,22 @@
 00000470: 7465 7874 2078 3d22 3131 3630 2220 793d  text x="1160" y=
 00000480: 2231 3530 2220 6669 6c6c 3d22 2330 3130  "150" fill="#010
 00000490: 3130 3122 2066 696c 6c2d 6f70 6163 6974  101" fill-opacit
 000004a0: 793d 222e 3322 2074 7261 6e73 666f 726d  y=".3" transform
 000004b0: 3d22 7363 616c 6528 2e31 2922 2074 6578  ="scale(.1)" tex
 000004c0: 744c 656e 6774 683d 2233 3730 2220 6461  tLength="370" da
 000004d0: 7461 2d69 6e74 6572 726f 6761 7465 3d22  ta-interrogate="
-000004e0: 7265 7375 6c74 223e 3930 2e30 253c 2f74  result">90.0%</t
+000004e0: 7265 7375 6c74 223e 3531 2e34 253c 2f74  result">51.4%</t
 000004f0: 6578 743e 0a20 2020 2020 2020 203c 7465  ext>.        <te
 00000500: 7874 2078 3d22 3131 3630 2220 793d 2231  xt x="1160" y="1
 00000510: 3430 2220 7472 616e 7366 6f72 6d3d 2273  40" transform="s
 00000520: 6361 6c65 282e 3129 2220 7465 7874 4c65  cale(.1)" textLe
 00000530: 6e67 7468 3d22 3337 3022 2064 6174 612d  ngth="370" data-
 00000540: 696e 7465 7272 6f67 6174 653d 2272 6573  interrogate="res
-00000550: 756c 7422 3e39 302e 3025 3c2f 7465 7874  ult">90.0%</text
+00000550: 756c 7422 3e35 312e 3425 3c2f 7465 7874  ult">51.4%</text
 00000560: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
 00000570: 6720 6964 3d22 6c6f 676f 2d73 6861 646f  g id="logo-shado
 00000580: 7722 2073 6572 6966 3a69 643d 226c 6f67  w" serif:id="log
 00000590: 6f20 7368 6164 6f77 2220 7472 616e 7366  o shadow" transf
 000005a0: 6f72 6d3d 226d 6174 7269 7828 302e 3835  orm="matrix(0.85
 000005b0: 3438 3736 2c30 2c30 2c30 2e38 3534 3837  4876,0,0,0.85487
 000005c0: 362c 2d36 2e37 3335 3134 2c31 2e37 3332  6,-6.73514,1.732
```

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/99.png` & `interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/99.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/99.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/default.svg` & `interrogate-1.7.0/tests/unit/fixtures/flat-square-modified/default.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/0.svg` & `interrogate-1.7.0/tests/unit/fixtures/for-the-badge/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/100.svg` & `interrogate-1.7.0/tests/unit/fixtures/for-the-badge/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/45.svg` & `interrogate-1.7.0/tests/unit/fixtures/for-the-badge/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/60.svg` & `interrogate-1.7.0/tests/unit/fixtures/for-the-badge/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/89.svg` & `interrogate-1.7.0/tests/unit/fixtures/for-the-badge/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/90.svg` & `interrogate-1.7.0/tests/unit/fixtures/for-the-badge/90.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/99.png` & `interrogate-1.7.0/tests/unit/fixtures/for-the-badge/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/99.svg` & `interrogate-1.7.0/tests/unit/fixtures/for-the-badge/99.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/default.svg` & `interrogate-1.7.0/tests/unit/fixtures/for-the-badge/default.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/plastic/0.svg` & `interrogate-1.7.0/tests/unit/fixtures/plastic/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/plastic/100.svg` & `interrogate-1.7.0/tests/unit/fixtures/plastic/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/plastic/45.svg` & `interrogate-1.7.0/tests/unit/fixtures/plastic/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/plastic/60.svg` & `interrogate-1.7.0/tests/unit/fixtures/plastic/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/plastic/89.svg` & `interrogate-1.7.0/tests/unit/fixtures/plastic/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/plastic/90.svg` & `interrogate-1.7.0/tests/unit/fixtures/plastic/90.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/plastic/99.png` & `interrogate-1.7.0/tests/unit/fixtures/plastic/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/plastic/99.svg` & `interrogate-1.7.0/tests/unit/fixtures/plastic/99.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/plastic/default.svg` & `interrogate-1.7.0/tests/unit/fixtures/plastic/default.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/social/0.svg` & `interrogate-1.7.0/tests/unit/fixtures/social/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/social/100.svg` & `interrogate-1.7.0/tests/unit/fixtures/social/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/social/45.svg` & `interrogate-1.7.0/tests/unit/fixtures/social/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/social/60.svg` & `interrogate-1.7.0/tests/unit/fixtures/social/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/social/89.svg` & `interrogate-1.7.0/tests/unit/fixtures/social/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/social/90.svg` & `interrogate-1.7.0/tests/unit/fixtures/social/90.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/social/99.png` & `interrogate-1.7.0/tests/unit/fixtures/social/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/social/99.svg` & `interrogate-1.7.0/tests/unit/fixtures/social/99.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/fixtures/social/default.svg` & `interrogate-1.7.0/tests/unit/fixtures/social/default.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/test_badge_gen.py` & `interrogate-1.7.0/tests/unit/test_badge_gen.py`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tests/unit/test_config.py` & `interrogate-1.7.0/tests/unit/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 """Unit tests for interrogate/config.py module"""
 
 import configparser
 import pathlib
 
 import click
 import pytest
-import toml
+
+
+try:
+    import tomllib
+except ImportError:
+    import tomli as tomllib
 
 from interrogate import config
 
 
 @pytest.mark.parametrize(
     "srcs,patch_func, expected",
     (
@@ -204,15 +209,15 @@
     actual = config.read_config_file(ctx, "config", value)
     assert exp_ret == actual
     assert exp_defaults == ctx.default_map
 
 
 def test_read_config_file_raises(mocker, monkeypatch):
     """Handle exceptions while reading pyproject.toml/setup.cfg, if any."""
-    toml_error = toml.TomlDecodeError("toml error", doc="foo", pos=0)
+    toml_error = tomllib.TOMLDecodeError("toml error")
     os_error = OSError("os error")
     mock_parse_pyproject_toml = mocker.Mock()
     mock_parse_pyproject_toml.side_effect = (toml_error, os_error)
     monkeypatch.setattr(
         config, "parse_pyproject_toml", mock_parse_pyproject_toml
     )
     cfg_error = configparser.ParsingError("cfg parsing error")
```

### Comparing `interrogate-1.6.0/tests/unit/test_utils.py` & `interrogate-1.7.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `interrogate-1.6.0/tox.ini` & `interrogate-1.7.0/tox.ini`

 * *Files identical despite different names*

