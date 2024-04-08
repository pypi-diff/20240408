# Comparing `tmp/polaris-lib-0.2.5.tar.gz` & `tmp/polaris-lib-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polaris-lib-0.2.5.tar", last modified: Wed Mar 20 22:40:39 2024, max compression
+gzip compressed data, was "polaris-lib-0.2.6.tar", last modified: Mon Apr  8 17:53:24 2024, max compression
```

## Comparing `polaris-lib-0.2.5.tar` & `polaris-lib-0.2.6.tar`

### file list

```diff
@@ -1,120 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.914559 polaris-lib-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.898559 polaris-lib-0.2.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.898559 polaris-lib-0.2.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/.github/ISSUE_TEMPLATE/default-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/.github/changelog_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.898559 polaris-lib-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-03-20 22:40:39.914559 polaris-lib-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.898559 polaris-lib-0.2.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.902559 polaris-lib-0.2.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/adapters.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/base.md
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/benchmark.md
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/converters.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/dataset.md
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/evaluation.md
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/factory.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/hub.client.md
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/hub.polarisfs.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/load.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/subset.md
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/api/utils.types.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.894559 polaris-lib-0.2.5/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.902559 polaris-lib-0.2.5/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/assets/css/custom-polaris.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.902559 polaris-lib-0.2.5/docs/community/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/community/community.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.902559 polaris-lib-0.2.5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/images/logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.906559 polaris-lib-0.2.5/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    31902 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/tutorials/basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/tutorials/custom_dataset_benchmark.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1239792 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/tutorials/data_curation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    97750 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/tutorials/dataset_factory.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/docs/tutorials/dataset_zarr.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/env.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.906559 polaris-lib-0.2.5/polaris/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.906559 polaris-lib-0.2.5/polaris/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21051 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/benchmark/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/benchmark/_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.906559 polaris-lib-0.2.5/polaris/curation/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/curation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/curation/_chemistry_curator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/curation/_curator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/curation/_data_curator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/curation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/curation/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.906559 polaris-lib-0.2.5/polaris/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/dataset/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/dataset/_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    19424 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/dataset/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/dataset/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/dataset/_subset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.906559 polaris-lib-0.2.5/polaris/dataset/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/dataset/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/dataset/converters/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/dataset/converters/_sdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/dataset/converters/_zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.910559 polaris-lib-0.2.5/polaris/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/evaluate/_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/evaluate/_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.910559 polaris-lib-0.2.5/polaris/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27260 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/hub/polarisfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/hub/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.910559 polaris-lib-0.2.5/polaris/loader/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/loader/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.910559 polaris-lib-0.2.5/polaris/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/utils/dict2html.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/utils/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/polaris/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.914559 polaris-lib-0.2.5/polaris_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-03-20 22:40:39.000000 polaris-lib-0.2.5/polaris_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-20 22:40:39.000000 polaris-lib-0.2.5/polaris_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 22:40:39.000000 polaris-lib-0.2.5/polaris_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-20 22:40:39.000000 polaris-lib-0.2.5/polaris_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-20 22:40:39.000000 polaris-lib-0.2.5/polaris_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-20 22:40:39.000000 polaris-lib-0.2.5/polaris_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 22:40:39.914559 polaris-lib-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:40:39.914559 polaris-lib-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/tests/test_curation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/tests/test_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-20 22:38:43.000000 polaris-lib-0.2.5/tests/test_type_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.252645 polaris-lib-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.236645 polaris-lib-0.2.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.236645 polaris-lib-0.2.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/.github/ISSUE_TEMPLATE/default-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/.github/changelog_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.236645 polaris-lib-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-08 17:53:24.252645 polaris-lib-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.236645 polaris-lib-0.2.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.240645 polaris-lib-0.2.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/adapters.md
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/base.md
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/benchmark.md
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/converters.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/evaluation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/factory.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/hub.client.md
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/hub.polarisfs.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/load.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/subset.md
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/api/utils.types.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.232645 polaris-lib-0.2.6/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.240645 polaris-lib-0.2.6/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/assets/css/custom-polaris.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.240645 polaris-lib-0.2.6/docs/community/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/community/community.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.240645 polaris-lib-0.2.6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/images/logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.244645 polaris-lib-0.2.6/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    31902 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/tutorials/basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/tutorials/custom_dataset_benchmark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1239792 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/tutorials/data_curation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    97014 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/tutorials/dataset_factory.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/docs/tutorials/dataset_zarr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.244645 polaris-lib-0.2.6/polaris/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.244645 polaris-lib-0.2.6/polaris/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21051 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/benchmark/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/benchmark/_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.244645 polaris-lib-0.2.6/polaris/curation/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/curation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/curation/_chemistry_curator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/curation/_curator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/curation/_data_curator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/curation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/curation/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.244645 polaris-lib-0.2.6/polaris/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/dataset/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/dataset/_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18938 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/dataset/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/dataset/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/dataset/_subset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.248645 polaris-lib-0.2.6/polaris/dataset/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/dataset/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/dataset/converters/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/dataset/converters/_sdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/dataset/converters/_zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.248645 polaris-lib-0.2.6/polaris/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/evaluate/_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/evaluate/_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.248645 polaris-lib-0.2.6/polaris/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29692 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/hub/polarisfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/hub/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.248645 polaris-lib-0.2.6/polaris/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/loader/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.248645 polaris-lib-0.2.6/polaris/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/utils/dict2html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/utils/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/polaris/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.252645 polaris-lib-0.2.6/polaris_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-08 17:53:24.000000 polaris-lib-0.2.6/polaris_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-08 17:53:24.000000 polaris-lib-0.2.6/polaris_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:53:24.000000 polaris-lib-0.2.6/polaris_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 17:53:24.000000 polaris-lib-0.2.6/polaris_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-08 17:53:24.000000 polaris-lib-0.2.6/polaris_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 17:53:24.000000 polaris-lib-0.2.6/polaris_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:53:24.252645 polaris-lib-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:24.252645 polaris-lib-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/tests/test_curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/tests/test_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-08 17:49:57.000000 polaris-lib-0.2.6/tests/test_type_checks.py
```

### Comparing `polaris-lib-0.2.5/.github/CODE_OF_CONDUCT.md` & `polaris-lib-0.2.6/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/.github/ISSUE_TEMPLATE/default-template.md` & `polaris-lib-0.2.6/.github/ISSUE_TEMPLATE/default-template.md`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/.github/PULL_REQUEST_TEMPLATE.md` & `polaris-lib-0.2.6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/.github/workflows/code-check.yml` & `polaris-lib-0.2.6/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/.github/workflows/doc.yml` & `polaris-lib-0.2.6/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/.github/workflows/release.yml` & `polaris-lib-0.2.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/.github/workflows/test.yml` & `polaris-lib-0.2.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/.gitignore` & `polaris-lib-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/LICENSE` & `polaris-lib-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/PKG-INFO` & `polaris-lib-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polaris-lib
-Version: 0.2.5
+Version: 0.2.6
 Summary: Client for the Polaris Hub.
 Author-email: Lu Zhu <lu@valencediscovery.com>, Hadrien Mary <hadrien@valencediscovery.com>, Julien St-Laurent <julien.stl@valencediscovery.com>, Cas Wognum <cas@valencediscovery.com>
 Project-URL: Website, https://polarishub.io/
 Project-URL: Source Code, https://github.com/polaris-hub/polaris
 Project-URL: Bug Tracker, https://github.com/polaris-hub/polaris/issues
 Project-URL: Documentation, https://polaris-hub.github.io/polaris/
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polaris-lib Version: 0.2.5 Summary: Client for the
+Metadata-Version: 2.1 Name: polaris-lib Version: 0.2.6 Summary: Client for the
 Polaris Hub. Author-email: Lu Zhu
 valencediscovery.com>, Hadrien Mary
 valencediscovery.com>, Julien St-Laurent
 valencediscovery.com>, Cas Wognum
 valencediscovery.com> Project-URL: Website, https://polarishub.io/ Project-URL:
 Source Code, https://github.com/polaris-hub/polaris Project-URL: Bug Tracker,
 https://github.com/polaris-hub/polaris/issues Project-URL: Documentation,
```

### Comparing `polaris-lib-0.2.5/README.md` & `polaris-lib-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/docs/assets/css/custom-polaris.css` & `polaris-lib-0.2.6/docs/assets/css/custom-polaris.css`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/docs/index.md` & `polaris-lib-0.2.6/docs/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -47,11 +47,11 @@
 
 ---
 
 **:fontawesome-solid-comments:  Community**
 
 Whether you are a first-time contributor or open-source veteran, we welcome any contribution to Polaris. Learn more about our community initiatives.
 
-[:material-arrow-right: Let's get started](https://portal.valencelabs.com/)
+[:material-arrow-right: Let's get started](https://discord.gg/vBFd8p6H7u)
 
 ---
```

### Comparing `polaris-lib-0.2.5/docs/quickstart.md` & `polaris-lib-0.2.6/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/docs/tutorials/basics.ipynb` & `polaris-lib-0.2.6/docs/tutorials/basics.ipynb`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/docs/tutorials/custom_dataset_benchmark.ipynb` & `polaris-lib-0.2.6/docs/tutorials/custom_dataset_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/docs/tutorials/data_curation.ipynb` & `polaris-lib-0.2.6/docs/tutorials/data_curation.ipynb`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/docs/tutorials/dataset_factory.ipynb` & `polaris-lib-0.2.6/docs/tutorials/dataset_factory.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995681793243438%*

 * *Differences: {"'cells'": "{5: {'outputs': {0: {'data': {'text/plain': ['<rdkit.Chem.rdchem.Mol at "*

 * *            "0x7f9d037bdaf0>']}}, delete: [0]}}, 11: {'outputs': {0: {'data': {'text/plain': "*

 * *            "['<rdkit.Chem.rdchem.Mol at 0x7f9cfe44b1f0>']}}}}, 14: {'outputs': {0: {'data': "*

 * *            "{'text/plain': ['<rdkit.Chem.rdchem.Mol at 0x7f9cfe43ad90>']}}}}, 16: {'outputs': {0: "*

 * *            "{'text': ['\\x1b[32m2024-03-26 13:16:43.897\\x1b[0m | \\x1b[1mINFO    \\x1b[0m | "*

 * *            '\\x1b[36mpolaris.dataset. […]*

```diff
@@ -71,30 +71,22 @@
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "0776f067-d01b-4b7c-89f6-a3c817f934fb",
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Failed to find the pandas get_adjustment() function to patch\n",
-                        "Failed to patch pandas - PandasTools will have limited functionality\n"
-                    ]
-                },
-                {
                     "data": {
                         "image/png": "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",
                         "text/html": [
                             "<table><tr><td colspan=\"2\" style=\"text-align: center;\"><image src=\"data:image/png;base64,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\"></td></tr>\n",
                             "<tr><th style=\"text-align: right\">my_property</th><td style=\"text-align: left\">my_value</td></tr></table>"
                         ],
                         "text/plain": [
-                            "<rdkit.Chem.rdchem.Mol at 0x7fc6b8d77920>"
+                            "<rdkit.Chem.rdchem.Mol at 0x7f9d037bdaf0>"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -201,15 +193,15 @@
             "id": "451b687e-34dd-4a86-9d36-b39d6247a24e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/plain": [
-                            "<rdkit.Chem.rdchem.Mol at 0x7fc6af2149a0>"
+                            "<rdkit.Chem.rdchem.Mol at 0x7f9cfe44b1f0>"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -244,15 +236,15 @@
             "id": "18beb7e0-95f2-4fd2-917d-8d4bcceb65af",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/plain": [
-                            "<rdkit.Chem.rdchem.Mol at 0x7fc6af2010d0>"
+                            "<rdkit.Chem.rdchem.Mol at 0x7f9cfe43ad90>"
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -282,15 +274,15 @@
             "id": "35b6e2cb-3b45-4944-903d-7da81ff1e7a4",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[32m2024-03-14 15:33:36.569\u001b[0m | \u001b[1mINFO    \u001b[0m | \u001b[36mpolaris.dataset._factory\u001b[0m:\u001b[36mregister_converter\u001b[0m:\u001b[36m100\u001b[0m - \u001b[1mYou are overwriting the converter for the sdf extension.\u001b[0m\n"
+                        "\u001b[32m2024-03-26 13:16:43.897\u001b[0m | \u001b[1mINFO    \u001b[0m | \u001b[36mpolaris.dataset._factory\u001b[0m:\u001b[36mregister_converter\u001b[0m:\u001b[36m112\u001b[0m - \u001b[1mYou are overwriting the converter for the sdf extension.\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "save_dst = dm.fs.join(SAVE_DIR, \"data2.zarr\")\n",
                 "factory.reset(save_dst)\n",
                 "\n",
@@ -325,15 +317,15 @@
                     "data": {
                         "image/png": "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",
                         "text/html": [
                             "<table><tr><td colspan=\"2\" style=\"text-align: center;\"><image src=\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAcIAAACWCAIAAADCEh9HAAAABmJLR0QA/wD/AP+gvaeTAAAZI0lEQVR4nO3de1hU1d4H8O8w3DHlYggaat4V0YRTjyhlgiAaCCKopGLlm+Xr8fR27Bw1FDnkBctL9qqlnkxMjEAkDK947PCGICcvKaAVISgoDigoSTAwM/v9Y0gDxYTZe7bK9/OXrplZ6zfPM8+Xvfdae22FIAggIqK2MpG7ACKiRxtjlIjIIIxRIiKDMEaJiAzCGCUiMghjlIjIIKZyF0BkdA0NOHwY589DEDBwIPz8YG4ud030CFNw3Si1LwUFCAhARQX+9CcAOHECDg7YuxcDB8pdGT2qGKPUnmg0GDoUdnbYvx8dOwJAdTXGj0d5OfLzYWYmd330SOK1UWpPDh7EuXNYt64xQwF07Ij161FQgLQ0WSujRxhjlNqT7Gx06oRnn23S6OEBBwdkZ8tUEz3yGKPUnlRWwtn5Hu3duuH6daNXQ48Jxii1J9bWqKy8R/v16+jQwejV0GOCMUrtiZsbKipQVtakUaVCWRnc3GSqiR55jFFqT4KC0KEDli9v0rhiBWxsEBIiU030yOPye2pP7OywdSumT4dKBV9fKBRIT0dKCnbsgL293MXRo4rrRql9+PZbqNUYMwYATp7Exo3Iy4MgYPBgzJ3buBSfqE0Yo9QOCAI8PHD6NBISMGWK3NXQ44bXRqkdSEnB6dNwdsaECQDQ0IDMTLlroscHY5Qed4KAmBgAWLwYVlYAEBeH55/HnDny1kWPDcYoyUMQhNraWmOMtHs3zpyBiwtmzQKAhgasWAEAL75ojNGpHWCMkgy+/vrrXr16RUVFST6STodlywAgMhIWFgDw6acoKoKrK8LCJB+d2gfGKMnAwcGhuLj4yy+/1Ol00o6UmIizZ9G9O159FQDq67FqFQBER8OEP34SB39JJANPT8+ePXuWlJRkZWVJOIxW23hVdMmSxo2Zt25FcTEGD+ZiexIRY5RkoFAoJk+eDCAhIUHCYRIScP48evZERAQAqNWIjQWAmBgeipKI+GMieUydOhVAYmKiRqORZACttvGq6NKljYeimzejtBTDhiE4WJIRqb1ijJI8hg0bNnDgwIqKim+++UaSAeLj8cMP6NMH06cDQF0d3n8fAKKjoVBIMiK1V4xRko105/UajUal73bJEpiaAsDHH+PyZbi7IzBQ9OGonWOMkmzCw8MB7NmzR61Wi9vzzp07nQ4cWB0QgGnTAKCuDqtXA0BMDA9FSXSMUZJN//79n3nmGVtbx3//+6KI3TY0NLz33nsAuoaHQ6kEUPPPf+LKFTz3HF56ScSBiPQYoySnV15JLy7+MS6un4h9xsXFXbhwoV+/flOmTAFQU1PTZ9my5c89V6ufcSISG2OU5DRxYmeFAqmpqKkRp8OGhoYVK1YAiImJUSqVADZs2HBVpdqnVFr5+oozBlFTjFGSU/fu8PTEr7+K9njjbdu2FRUVubq6hoWFAaipqVm7di2AGP06fCIJMEZJZvr9P0WZrq+vr4+NjQUQHR1tYmICYP369eXl5SNHjhyj37CZSALctplkdvUqnnoKpqa4ehW2tgZ1tWnTprlz5w4ePPjMmTMmJia3bt3q1atXRUXF0aNHR48eLVK9RM3xaJRk5uSEF1+EWo2vvjKoH7VavXLlSgAxMTH6Q9F169ZVVFR4eXkxQ0lSjFGSnyjn9Vu2bCktLR02bFhwcDCAmzdvfvjhhwCWcYKeJMYYJfmFhsLcHP/6F8rL29hDXV3dqlWrAPTr1y8iIuLq1avr1q2rrKz08fEZNWqUmLUS3YUPWCb52dlh+nTY2KANu5TU1tYeO3Zs9erVly9fBvDll1+amZmVlpaeOXMGgDF2hqZ2j1NMJL/SUmRn47nn0KNHY4tOh+RkjBiBbt3u/ZHCwuv79sXv27cvIyPj9r2knTt39vX1TUhIUCqVGo3Gz8/v0KFDRvkG1K7xaJTkl5ODyZPx3HPIzm7cCFSjweTJSElpEqNaLbKzkZaGI0dQXl5dUvIWABMTEw8PjzFjxgQEBIwcOVKhUFy8eFG/G/SSJUvk+T7UzjBG6aFgYoKiIvzzn5g9u/lLV69i/37s34/0dFRXNzba2T39+uv/8/zz7uPGjevcufPv3x8REZGVldW9e3cvLy+j1E7tHU/qSX7JyZg6FWvXIjoa58/D0RH19bCwQEoKdu3C7t24/SN1c8P48Rg/HiNGNG6Ad7eqqipnZ2eNRlNaWurk5GS0b0HtFmfq6WExZw6cnfHOO00au3WDpSXGjMGHH6K4GGfPIjYWL7zQYoYCsLOz8/f312q1iYmJUtdMBMYoPTxMTfHxx9i5E//6153GxYtx/TrS0/HWW3cmoP7QtGnTAMTHx0tQJlFzjFF6iDz/PF5+GfPmoaGhscXBAVZWre4nMDCwU6dOP/xQVlBwXdwKie7GGKWHy+rVuHIFmzcb1ImlpeWbb56tr78UH+8gUl1ELWKM0sPFyQkxMTD8Bs4xY7rX1WHnTnAOlaTGGKWHzty56NnT0E68vdGtGwoL8d13IpREdB+MUZKfoyN8fO78V6nEpk0YMwaOjm3v08SkcccTzjOR1LhulOS3YQMmTYKzs8jdnjoFDw84OuLy5fstkCIyEI9GSWYZGZg3Dx4ed2bnxeLuDldXlJc3WUFliLKysvT0dHH6oscIY5RktmgRAMydCzMz8TufOhUw+Ly+qKho/fr1vr6+3bt3DwkJqaurE6U2emzwVIfklJKC7Gw4OuIvf5Gk/5dfxvLlUCha/UFBEE6cOJGSkpKamnru3Dl9o5WVlY+PT2VlZdeuXUUulB5ljFGSjVYL/R5MUVF44glJhnByQkFBk22iGhpw6xZsbe+drQ0NyMjAv/+9Pi5udWlpqb7R3t4+ICAgKCjI39/f2tpakkLpUcYYJdns2IH8fDz9NF5/Xaoh3n4bW7bg888xfXpjy8GDmDABv/7a5Oao2locOYK0NHz1FcrLMWqUtrS01MXFZdy4cQEBAWPHjjU3N5eqRHr0MUZJHvX1eO89AFi2DJJmlKUl5s/HSy/Bzq75S+Xl2LsXqak4cgS3L3i6uWHs2Olr1oxyd3dXtOFyALU/jFGSx8aNKCqCm1vjLJB0XnwRV65g4cImN5jeuAE/P2RlQacDAKUSXl4IDkZwMHr3BuAIGLBmldoZxijJ4NYtxMYCQGxs43b30lEqsW4dfH0xcyZGjGhstLXFlSswN4eXFwICMHmy+KtWqf1gjJIMPvgA5eXw8sL48cYYztsboaGYMwcnT95pTElBr17o0MEYBdDjjetGydgqKrBuHYDGA1LjWLsWRUX43/+90zJkCDOUxMEYJWPbtGnvk0/WBwZi5EjjDdqtG5YuRUwMrl0z3qDUTvCeejKq4uLiAQMGCILy9OkLgwZ1kXq4N97A5ctISwMAjQbDhkGtRkFB8wVPRIbg0SgZVVRUlFqtDg8PM0KGNqN/SMnPPxt5WHr8MUbJePLy8uLj483NzaOiomQpwMsLM2bIMjI9zhijZDzvvvuuTqebM2dOr169jDCcIOC11xrP6G+Li4Mg8IyexMQYJSPJyclJS0vr0KHDIv2eTtJLSsLw4Zg1yzijUfvFGCUjWbhwoSAI8+fP79LFGFdFtVpERwOAp6cRRqN2jTP1ZAzx8fHTp0/v3LlzYWFhx44djTDitm2YNQt9++LcOW59T9Li74skdOnSpZSUlKSkpGPHjgGIjIw0TobW1zc+W/Qf/2CGkuR4NEri+/HHH/fs2ZOcnHzyd3dfOjo6Xrp0ycLCwggFfPQR3noLbm74/nvJ79kn4l9qEk9u7t7DhyO3b8/Ly9M3dOzY0d/fPyMjQ6VSrVq1yjgZWlODlSsBYPlyZigZA39lZLD8fERHY9AgDBnSLzU1Ly/Pzs5uxowZiYmJV65c8fPzq6ysfPLJJ2cYa8XmRx/h6lU8+ywCAowzILV3PBqlNhEEHD+O5GQkJ6O4uLHR0bGHh8fhJUtGjx5t+tslyRs3bjQ0NNTX1yuVSiPUdfMmVq8GgNjYtjyCiagNGKN0X9XV+OILnD0LrRb9+mHqVHTtiuJieHnh8uXG93TrhpAQTJoELy8rpdL3d5++efOmvb29mZnZzZs3z58/P3DgQKnr/eADVFbCxwfe3lIPRdSIU0zUstxcjB0LS0v4+MDcHJmZKCxEYiL8/eHiAlNTBAcjLAwjRjS7BllVVfX1118nJSWlp6er1Wp947JlyyIjIyWt99o19OqFX35BVhaXi5LxMEapBVotBg9Gly44dAj6qSH9zZUpKSgogFqNp55q/hGVCl99VX/wYKf9++vq6wEolcpRo0b179//448/HjZs2KlTpyQteenSwpiY3hMmIDVV0nGImmCMUguOHIGvb/PjOpUKPXrg/febPFe+ogIHDiApCQcPQqMB8OdnnvnexiYsLGzKlClOTk5qtdrR0bG6uvrnn3/u3bu3RPWWlJT069fP1fWFzz5Lc3Mzk2gUorvx2ii14ORJmJri2WebNHbpgt69G5/FUVTUOMWUkwP9H2NLS4wfj0mTPgoMNPndczgtLCxeeumlL774IiUl5Z133pGo3piYmLq6uv79OzNDyci44IlaUF0Ne/t73APUpQtu3gSA5cvxt7/h+HFYWiIgAHFxUKmQmoqICJO7nmUcEhICIDk5WaJiCwoKtm/frlQq5dqCj9ozHo1SCzp1wvXr0GiaJ6lKhe7dASA8HLW1mDQJ/v6wtr5/Z+PHj7exscnJySkpKXFxcRG92KioKI1G8/rrr/fv31/0zonuj0ej1AJ3d2i1yM9v0lhejsJCeHgAgI8P4uMREvKHGQrA2traz89PEIRUCWZ/cnNzExMTLS0tlyxZInrnRH+IMUotGD0affvi3Xf1s0aNoqNhYYHw8Db0N2nSJEhzXh8ZGanT6d58800pjnOJ/hBn6qllJ09i7Fg4O2PcOJibIyMDJ04gIQFBQW3o7JdffnF0dGxoaLhy5Yqjo6NYNf7nP/8ZPny4tbV1YWGhcXYyJWqGR6PUMg8P/PADZszA5csoKIC3N86da1uGAnjiiSe8vb21Wq245/WLFi0SBOHtt99mhpJceDRKxrNt27ZZs2aNHTv24MGDonR45MgRX19fW1vbCxcu2N21PIDIOHg0SsYTFBRkamp69OjRyspKUTrUzyktWLCAGUoyYoyS8Tg4OIwaNaqhoSGt2eM6W+/06dMRERHHjx93cnKaN2+eKOURtQ1jlIzKwPn6/Pz86OjoAQMGuLu7f/755507dw4MDLSxsRG1RqLW4fJ7MqqQkJB58+YdOnSourr6AZ/LJAhCTk7O7t27k5OTi3/b29TZ2bl3796ZmZnWD7BqlUhSPBolo+rSpYunp6darT5w4MD936nT6U6ePBkdHd23b19PT881a9YUFxc/9dRTs2fP3rt376VLl958800AKpXKKIUTtYhHo2RsISEhmZmZycnJU6ZMuftVnU6XlZWVlJSUnJx8+bedoV1cXCZOnBgWFjZixAiT3/Y21a9wKi8vN1rlRPfEBU9kbCUlJT169LCysqqoqLh9Sq7VarOzs5OSkpKSksrKyvSNPXr0CAoKCgsLGzlypOKuR4Lk5uYOGTLE1dX19hP0iGTBo1EyNhcXFw8PjxMnThw+fDgwMFCfnomJiVevXtW/oWfPnhMmTLhnel67dq1z5876f+uPRnlST7Lj0SjJIDY2dtGiRX369KmsrLy9hnTAgAGhoaGhoaFDhw5t9v6SkpI9e/YkJSXl5ORcvHixa9euAHQ6nYWFhVarVavVZmbcY5Rkw6NRksELL7zg7OxcWFgoCMKgQYMCAwMDAgK8vLyave3ChQvJycm7d+/+7rvv9H/vra2tz549q49RExMTBwcHlUp17do1Z2dnGb4GEQDGKMkiOzu7rKzM3d09Pj5+wIABzV4tLi5OTU1NSkrKysrSp6eVlZWPj09YWNjEiROfeOKJ2+/s0qWLSqVSqVSMUZIRY5RksGPHDgBRUVG/z9ALFy7onyd67NgxfYu1tbW3t3dYWFhISEiHDh3u7ke/UxQvj5K8GKNkbKdPnz579qyDg8O4ceP0LcnJyUuXLs3/bYtoOzu7wMDA0NBQPz8/C/1DSVswZMgKlSq6qmqw5EUTtYwxSsYWFxcHYNq0aebm5voWhUKRn59vZ2cXEBAQFhY2duzY2y/9kWdzc1FaKlmtRA+AMUpGpdFoEhISAMycOfN2o7+//6FDh7y9vU3vfoLefem3GOU5PcmLMUpGtW/fPpVK5erq6u7ufrtR/6SmNvSm30Sf9zGRvHhPPRmV/oz+lVdeEaU3Ho3Sw4AxSsZTWVm5f/9+U1PTadOmidIhY5QeBoxRMp5du3ap1Wo/Pz+xlnnqT+oZoyQvxigZj/6M/veTSwZydIRCgYoK6HRidUnUarynnozk3Llzrq6unTp1Kisrs7KyEqtbe3tUVeHaNTg4iNUlUetwpp6MZNeuviNHFo0alS1ihgLo0gVVVVCpGKMkGx6NkjHodOjRA6WlyMqCp6eYPR89CqUSf/oT+EAmkguPRskY0tNRWoq+fTF8uDgd1tUhIgKurli69E7jP/6Bbt3wX/8lzhBED4hTTGQMcXEAMHMm7trDvo00GiQlIToaR47caczIwKlT4vRP9OAYoyS56mqkpkKhwMsvi9yzpyfmzoVaLXK3RK3CGCXJJSbi118xejSeflrknv/2N1RXIzZW5G6JWoUxSpK7fUYvuo4dsXIlYmNRUCB+50QPiDFK0ioqwrFjsLFBSIgk/c+cCQ8P/Pd/S9I50YNgjJK0tm+HICA0FPfavb4Vbt68d7tCgU8+QUYG9uwxqH+iNmOMkoQEATt3Agaf0efno29fbN5871cHD8af/4y//x319QaNQtQ2jFGS0P/9Hy5cQI8eGDWq7Z0UF8PPDxUVOHwYLd0sEh2N2lpkZ7d9FKI2Y4yShFJTAWDGDJi09Yd27Rr8/XHlCl58EfHxLS477dgRa9ZwgxKSB+9iIgmtXo2AAPTt28aP//IL/P3x448YMgQpKbC0BIC0NOzejU2bsHkzfv9s5qlT0dAg/poqoj/Ee+pJTIGBUKuxd29j5AF4/30UFGDr1lZ3VV+PwEAcPozevZGZCScnAMjMhJ8famuxfbskK6iI2oAn9SSm3Fykp2PlyjstJSX46adW96PTYfp0HD6Mrl2Rnt6YoXl5mDABtbWYPZsZSg8RxiiJbNw4xMbi/HmDOlm6tCApCba2OHCg8Ty9qAh+fqiqQlAQNm4UpVIicTBGSWT+/vDxwZw5Lc6q/6HFixcvXz5gzJj/fP01hgwBgIoKjBuHsjKMHo2EBLTyMcxE0mKMkvjWrkV2duOK0dbatGnT8uXLTUwUc+aUenkBQHV140TT0KHYs+fOVVeihwRjlMQ3YADmz8c776CqqnUf3LVr17x58xQKxZYtW0JCQgDU1yM0FKdOoU8fHDoEW1tJCiYyBGOUJLF4MWxsEBPTio8cOXLk1Vdf1el0H3zwwWuvvQZAq8W0aUhPb5xo0j9OmehhwxglcVRWNvmvtTXWrsXGjXem6e+/Nj4nJyc4OLi+vn7hwoXz588HIAhCVNT+r76CnR0OHULPntLUTWQwxigZqrYWCxdi4EBcvdqkPTgYfn44fBgAyssxaBASEu7dQ35+/vjx42tqaiIiIlasWKFvjIyMXLHipeHDV6WlYfBgSb8BkUEYo2SQzEy4uWHVKty4gays5q9u3AhrawDYtAk//ojwcMyejZqa5m9LTk6urKwMDg7etm2bQqEAsGHDhpUrV5qZmS1a5DZihBG+B5EBBKI2qa0VFiwQlEoBEAYPFk6dEgRB+PZb4dKlJm87fVr47jtBpxM2bxasrQVAePpp4dix5r3t2LGjtrZW/++dO3eamJgoFIrPPvtM+u9BZCjGKLXFmTPC0KECIJiaCgsWCHV1D/Sp3FxhyBABEMzMhDVrqjQazd3vSUtLMzMzA7BmzRqRiyaSBmOUWqehQYiNFczNBUDo3Vv49tvWfbyuTliwQDA11Q4b5uPp6VlYWPj7V48fP25jYwMgMjJSzKKJpMQYpVbIyxM8PARAUCiE2bOFW7fa2M8331xwdnYGYGtr+8UXX+gbc3Nz7e3tAcycOVOn04lWNJHEGKP0QDQaTWxs7JAhtwChVy8hI8PQDisqKoKDg/UX6MPCwnJzc11cXABMmDChoaFBjJKJjIQb5dEf++mnn1555ZXs7Oy+fYPHjNnz/vsKAx+sdNuWLVv++te/1tTUKJVKrVY7evTo/fv3W/J+T3qkMEbpfgRB2Lp1qz7pnJyctm7dGhAQIO4QRUVF4eHh+fn5Dg4O33//vS3v96RHDWOUWnTx4sXXXnvt6NGjAMLCwj755BP9tUvR3bp16+LFi3369LGwsJCifyJJMUbp3pKSkt54442qqipHR8dPPvlk4sSJcldE9JDiXUzUnEqlCgoKmjx5clVVVWhoaF5eHjOU6D64/y01kZmZGRQUVFlZaW9vv2HDhvDwcLkrInrY8aSemrhx44abm5urq+unn37arVs3ucshegQwRqm5kpIS/RJOInoQjFEiIoNwiomIyCCMUSIigzBGiYgMwhglIjIIY5SIyCD/D9+G3rhq5bBLAAABTnpUWHRyZGtpdFBLTCByZGtpdCAyMDIzLjA5LjUAAHice79v7T0GIOBnQAA+KL+BkY0hAyTAyMzOoAFiMEMFmBkRAmCaBZ3mgNBMaBoZmQkq4GZgZGBkYmBi5mBiZmFgYeVgYmVjYGPnYGLjYODgZODgYuDi5mDi4mHg4WVgZWTgYWEQYQJqZGUEKmdlY+Pg4mFhFd8EMgqKGfiWv+A4EMzqfeAh9+T9qasm7JdQkz+wae76fb+tPuxjNbE9sOuWlf2P4MN2sicZDxgfmWl/TnKiXfyMnP0T627b/arT2h/tNG//60ds+3u8qvY36/fse1i1Z/+O9a/3u/zi3a/3X/RA1r2N+5oDM+2ntG8Fmm+w//3Jz/Y6V6QOeL8SsZcsnm5vzfh2n334ZPt9B4Udls1+su+DWIZ93K5OuwWdH+yuhX2xf28hat9UvM9eDACM1GEAYrR3BQAAAaF6VFh0TU9MIHJka2l0IDIwMjMuMDkuNQAAeJx9U0tOxDAM3fcUvgCR7TgfL5kZhBCiI8HAHdhzf2EnHZJsaOsqcZ+d52d3A7/eL6/fP/B3xcu2AeA/j6rCV0TE7Q18Aaen55cdzrfH091zvn7utw8gAUoWY/eKfbxd3+4egjM8cKCojAgPMVDhtqJAUitOwQx7c0dsAA5Sc/EVhijOaECjZ8UgWQ+ophwdEAqrzkixpBZfKXUgcvHvFBgpzsBkKTFwjdKPVBZuGYVrmYG5n51zxl4Hx3zEJM7L4aVDtZSjDi6x9iApnGZohau7qzRWnitJ7pSt+IWAuk6uSZFGUInkSEqVZyThwVWRWtGK96RCukKp1Z8qlYakGrkTkcxLUcRG1QCJPKfRw3pUJ5KXmig28RVdKhfX1WmSZl06b5N0buxqO8lYcG+S1LKc/bRflunq83a67pcxb37zmCnbQBxzYxuQMRxklsYIsFkejSazMprJZnU0jGyroynkNkvfHDQJzP4inoSk5omTYNReMinjJEZM6og0KzLX7/v7v2rr7RdbH7+0RVgL8gAAAOF6VFh0U01JTEVTIHJka2l0IDIwMjMuMDkuNQAAeJwlT0uuxDAIu8pbtlIaBUP4qOoq+86F5vAPMiuC7dhmvbSed+FZtI7nc77HOn8PrL/vcaETB9rFnQw5qZO43zV55I4urtau0Vn4ziEaG46p3EY3RNxJOs1CBywadQziROEs9TUgSK3ArSxUtYLAutkJjYLDbAfB2IsXw6wiLsRbN0UrI4tsGxaTdA0i2XJybPcYlBVi/NRCgawynSxRckbbVyDuXCdRS8fhO1lEZ2pjZMHsodH2vX6Xndc2HXWfuMX5/QcEX0W59Lht5AAAAABJRU5ErkJggg==\"></td></tr>\n",
                             "<tr><th style=\"text-align: right\">my_property</th><td style=\"text-align: left\">my_value</td></tr></table>"
                         ],
                         "text/plain": [
-                            "<rdkit.Chem.rdchem.Mol at 0x7fc6af2036f0>"
+                            "<rdkit.Chem.rdchem.Mol at 0x7f9cfe454360>"
                         ]
                     },
                     "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -372,26 +364,23 @@
                             "      <th>molecule</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>CN1C=NC2=C1C(=O)N(C)C(=O)N2C</td>\n",
-                            "      <td>/home/cas/.cache/polaris-tutorials/003/data2.z...</td>\n",
+                            "      <td>molecule#0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                         smiles  \\\n",
-                            "0  CN1C=NC2=C1C(=O)N(C)C(=O)N2C   \n",
-                            "\n",
-                            "                                            molecule  \n",
-                            "0  /home/cas/.cache/polaris-tutorials/003/data2.z...  "
+                            "                         smiles    molecule\n",
+                            "0  CN1C=NC2=C1C(=O)N(C)C(=O)N2C  molecule#0"
                         ]
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -415,16 +404,16 @@
             "id": "ef15bf98-f301-465d-9e93-2531f9f1f98c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[32m2024-03-14 15:33:36.611\u001b[0m | \u001b[1mINFO    \u001b[0m | \u001b[36mpolaris.dataset._factory\u001b[0m:\u001b[36mregister_converter\u001b[0m:\u001b[36m100\u001b[0m - \u001b[1mYou are overwriting the converter for the sdf extension.\u001b[0m\n",
-                        "\u001b[32m2024-03-14 15:33:36.614\u001b[0m | \u001b[1mINFO    \u001b[0m | \u001b[36mpolaris.dataset._factory\u001b[0m:\u001b[36mregister_converter\u001b[0m:\u001b[36m100\u001b[0m - \u001b[1mYou are overwriting the converter for the sdf extension.\u001b[0m\n"
+                        "\u001b[32m2024-03-26 13:16:43.938\u001b[0m | \u001b[1mINFO    \u001b[0m | \u001b[36mpolaris.dataset._factory\u001b[0m:\u001b[36mregister_converter\u001b[0m:\u001b[36m112\u001b[0m - \u001b[1mYou are overwriting the converter for the sdf extension.\u001b[0m\n",
+                        "\u001b[32m2024-03-26 13:16:43.945\u001b[0m | \u001b[1mINFO    \u001b[0m | \u001b[36mpolaris.dataset._factory\u001b[0m:\u001b[36mregister_converter\u001b[0m:\u001b[36m112\u001b[0m - \u001b[1mYou are overwriting the converter for the sdf extension.\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "save_dst = dm.fs.join(SAVE_DIR, \"data3.zarr\")\n",
                 "factory.reset(save_dst)\n",
                 "\n",
@@ -472,31 +461,25 @@
                             "      <th>molecule2</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>my_value</td>\n",
-                            "      <td>/home/cas/.cache/polaris-tutorials/003/data3.z...</td>\n",
+                            "      <td>molecule1#0</td>\n",
                             "      <td>CN1C=NC2=C1C(=O)N(C)C(=O)N2C</td>\n",
-                            "      <td>/home/cas/.cache/polaris-tutorials/003/data3.z...</td>\n",
+                            "      <td>molecule2#0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  my_property                                          molecule1  \\\n",
-                            "0    my_value  /home/cas/.cache/polaris-tutorials/003/data3.z...   \n",
-                            "\n",
-                            "                         smiles  \\\n",
-                            "0  CN1C=NC2=C1C(=O)N(C)C(=O)N2C   \n",
-                            "\n",
-                            "                                           molecule2  \n",
-                            "0  /home/cas/.cache/polaris-tutorials/003/data3.z...  "
+                            "  my_property    molecule1                        smiles    molecule2\n",
+                            "0    my_value  molecule1#0  CN1C=NC2=C1C(=O)N(C)C(=O)N2C  molecule2#0"
                         ]
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `polaris-lib-0.2.5/docs/tutorials/dataset_zarr.ipynb` & `polaris-lib-0.2.6/docs/tutorials/dataset_zarr.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986833243534483%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(2, \'train_path = f"{inp_col_name}#0"\\n\'), (3, '*

 * *            '\'test_path = f"{inp_col_name}#1"\')], delete: [3, 2]}}, 7: {\'source\': {insert: '*

 * *            "[(7, '    # We also need to specify the path to the root of the Zarr archive\\n'), "*

 * *            "(8, '    zarr_root_path=base_path,\\n')]}}, 8: {'source': ['Note how the table does "*

 * *            'not contain the image data, but rather stores a path relative to the root of the '*

 * *            'Zarr. \']}, 9: {\ […]*

```diff
@@ -125,16 +125,16 @@
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# For performance reasons, Polaris expects all data related to a column to be saved in a single Zarr array. \n",
                 "# To index a specific element in that array, the pointer path can have a suffix to specify the index. \n",
-                "train_path = f\"{base_path}/{inp_col_name}#0\"\n",
-                "test_path = f\"{base_path}/{inp_col_name}#1\""
+                "train_path = f\"{inp_col_name}#0\"\n",
+                "test_path = f\"{inp_col_name}#1\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "16543db7",
             "metadata": {
@@ -172,29 +172,31 @@
                 "from polaris.dataset import Dataset, ColumnAnnotation\n",
                 "\n",
                 "dataset = Dataset(\n",
                 "    table=table,\n",
                 "    # To indicate that we are dealing with a pointer column here,\n",
                 "    # we need to annotate the column.\n",
                 "    annotations={\"images\": ColumnAnnotation(is_pointer=True)},\n",
+                "    # We also need to specify the path to the root of the Zarr archive\n",
+                "    zarr_root_path=base_path,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2524c795",
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "Note how the table does not contain the image data, but rather stores a path. "
+                "Note how the table does not contain the image data, but rather stores a path relative to the root of the Zarr. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "19a39fab",
             "metadata": {
@@ -204,15 +206,15 @@
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'/home/cas/.cache/polaris-tutorials/002/data.zarr/images#0'"
+                            "'images#0'"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -356,20 +358,20 @@
                 "```\n",
                 "/\n",
                 "  column_a\n",
                 "```\n",
                 "\n",
                 "Which will get parsed into a table like: \n",
                 "\n",
-                "| column_a                             |\n",
-                "| ------------------------------------ |\n",
-                "| /path/to/root.zarr/column_a/array#1  |\n",
-                "| /path/to/root.zarr/column_a/array#2  |\n",
-                "|                 ...                  |\n",
-                "| /path/to/root.zarr/column_a/array#N  |\n",
+                "| column_a          |\n",
+                "| ----------------- |\n",
+                "| column_a/array#1  |\n",
+                "| column_a/array#2  |\n",
+                "|       ...         |\n",
+                "| column_a/array#N  |\n",
                 "\n",
                 "<div class=\"admonition info highlight\">\n",
                 "    <p class=\"admonition-title\">Note</p>\n",
                 "    <p>Notice the # suffix in the path, which indicates the index at which the data-point is stored within the big array. </p>\n",
                 "</div>"
             ]
         },
@@ -408,24 +410,17 @@
         {
             "cell_type": "code",
             "execution_count": 13,
             "id": "3c7c11ac",
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "A\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
-                            "'/home/cas/.cache/polaris-tutorials/002/zarr/data.zarr//images#0'"
+                            "'images#0'"
                         ]
                     },
                     "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -527,39 +522,40 @@
             "execution_count": 17,
             "id": "33c25a55",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<table border=\"1\"><tr><th>name</th><td>None</td></tr><tr><th>description</th><td></td></tr><tr><th>tags</th><td></td></tr><tr><th>user_attributes</th><td></td></tr><tr><th>owner</th><td>None</td></tr><tr><th>default_adapters</th><td>None</td></tr><tr><th>md5sum</th><td>6ef8d23737aafcbf82c421e7f99e1d95</td></tr><tr><th>readme</th><td></td></tr><tr><th>annotations</th><td><table border=\"1\"><tr><th>images</th><td><table border=\"1\"><tr><th>is_pointer</th><td>True</td></tr><tr><th>modality</th><td>UNKNOWN</td></tr><tr><th>description</th><td>None</td></tr><tr><th>user_attributes</th><td></td></tr><tr><th>dtype</th><td>object</td></tr></table></td></tr></table></td></tr><tr><th>source</th><td>None</td></tr><tr><th>license</th><td>None</td></tr><tr><th>curation_reference</th><td>None</td></tr><tr><th>cache_dir</th><td>/home/cas/.cache/polaris/datasets/None/6ef8d23737aafcbf82c421e7f99e1d95</td></tr><tr><th>artifact_id</th><td>None</td></tr><tr><th>n_rows</th><td>1000</td></tr><tr><th>n_columns</th><td>1</td></tr></table>"
+                            "<table border=\"1\"><tr><th>name</th><td>None</td></tr><tr><th>description</th><td></td></tr><tr><th>tags</th><td></td></tr><tr><th>user_attributes</th><td></td></tr><tr><th>owner</th><td>None</td></tr><tr><th>default_adapters</th><td></td></tr><tr><th>zarr_root_path</th><td>/home/cas/.cache/polaris-tutorials/002/json/data.zarr</td></tr><tr><th>md5sum</th><td>5488b4909fd67d3208624288e720e1b8</td></tr><tr><th>readme</th><td></td></tr><tr><th>annotations</th><td><table border=\"1\"><tr><th>images</th><td><table border=\"1\"><tr><th>is_pointer</th><td>True</td></tr><tr><th>modality</th><td>UNKNOWN</td></tr><tr><th>description</th><td>None</td></tr><tr><th>user_attributes</th><td></td></tr><tr><th>dtype</th><td>object</td></tr></table></td></tr></table></td></tr><tr><th>source</th><td>None</td></tr><tr><th>license</th><td>None</td></tr><tr><th>curation_reference</th><td>None</td></tr><tr><th>cache_dir</th><td>/home/cas/.cache/polaris/datasets/None/5488b4909fd67d3208624288e720e1b8</td></tr><tr><th>artifact_id</th><td>None</td></tr><tr><th>n_rows</th><td>1000</td></tr><tr><th>n_columns</th><td>1</td></tr></table>"
                         ],
                         "text/plain": [
                             "{\n",
                             "  \"name\": null,\n",
                             "  \"description\": \"\",\n",
                             "  \"tags\": [],\n",
                             "  \"user_attributes\": {},\n",
                             "  \"owner\": null,\n",
-                            "  \"default_adapters\": null,\n",
-                            "  \"md5sum\": \"6ef8d23737aafcbf82c421e7f99e1d95\",\n",
+                            "  \"default_adapters\": {},\n",
+                            "  \"zarr_root_path\": \"/home/cas/.cache/polaris-tutorials/002/json/data.zarr\",\n",
+                            "  \"md5sum\": \"5488b4909fd67d3208624288e720e1b8\",\n",
                             "  \"readme\": \"\",\n",
                             "  \"annotations\": {\n",
                             "    \"images\": {\n",
                             "      \"is_pointer\": true,\n",
                             "      \"modality\": \"UNKNOWN\",\n",
                             "      \"description\": null,\n",
                             "      \"user_attributes\": {},\n",
                             "      \"dtype\": \"object\"\n",
                             "    }\n",
                             "  },\n",
                             "  \"source\": null,\n",
                             "  \"license\": null,\n",
                             "  \"curation_reference\": null,\n",
-                            "  \"cache_dir\": \"/home/cas/.cache/polaris/datasets/None/6ef8d23737aafcbf82c421e7f99e1d95\",\n",
+                            "  \"cache_dir\": \"/home/cas/.cache/polaris/datasets/None/5488b4909fd67d3208624288e720e1b8\",\n",
                             "  \"artifact_id\": null,\n",
                             "  \"n_rows\": 1000,\n",
                             "  \"n_columns\": 1\n",
                             "}"
                         ]
                     },
                     "execution_count": 17,
```

### Comparing `polaris-lib-0.2.5/env.yml` & `polaris-lib-0.2.6/env.yml`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/mkdocs.yml` & `polaris-lib-0.2.6/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
           - PolarisFileSystem: api/hub.polarisfs.md
       - Additional:
           - Dataset Factory: api/factory.md
           - Data Converters: api/converters.md
           - Data Adapters: api/adapters.md
           - Base classes: api/base.md
           - Types: api/utils.types.md
-  - Community: community/community.md
+  - Community: https://discord.gg/vBFd8p6H7u
   - Polaris Hub: https://polarishub.io/
 
 theme:
   name: material
   # NOTE(hadim): to customize the material primary and secondary color,
   # see check `docs/assets/css/custom-polaris.css`.
   palette:
```

### Comparing `polaris-lib-0.2.5/polaris/_artifact.py` & `polaris-lib-0.2.6/polaris/_artifact.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import json
 from typing import Dict, Optional, Union
 
 import fsspec
+from loguru import logger
+from packaging.version import Version
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
-    PrivateAttr,
     computed_field,
     field_serializer,
     field_validator,
 )
 from pydantic.alias_generators import to_camel
 
+import polaris as po
 from polaris.utils.misc import sluggify
 from polaris.utils.types import HubOwner, SlugCompatibleStringType
 
 
 class BaseArtifactModel(BaseModel):
     """
     Base class for all artifacts on the Hub. Specifies meta-data that is used by the Hub.
@@ -31,42 +33,57 @@
             Together with the owner, this is used by the Hub to uniquely identify the benchmark.
         description: A beginner-friendly, short description of the dataset.
         tags: A list of tags to categorize the benchmark by. This is used by the hub to search over benchmarks.
         user_attributes: A dict with additional, textual user attributes.
         owner: A slug-compatible name for the owner of the dataset.
             If the dataset comes from the Polaris Hub, this is the associated owner (organization or user).
             Together with the name, this is used by the Hub to uniquely identify the benchmark.
-        _verified: Whether the benchmark has been verified through the Polaris Hub.
+        polaris_version: The version of the Polaris library that was used to create the artifact.
     """
 
     model_config = ConfigDict(alias_generator=to_camel, populate_by_name=True, arbitrary_types_allowed=True)
 
     name: Optional[SlugCompatibleStringType] = None
     description: str = ""
     tags: list[str] = Field(default_factory=list)
     user_attributes: Dict[str, str] = Field(default_factory=dict)
     owner: Optional[HubOwner] = None
-    _verified: bool = PrivateAttr(False)
+    polaris_version: str = po.__version__
 
     @computed_field
     @property
     def artifact_id(self) -> Optional[str]:
         return f"{self.owner}/{sluggify(self.name)}" if self.owner and self.name else None
 
-    @field_serializer("owner")
-    def _serialize_owner(self, value: HubOwner) -> Union[str, None]:
-        return self.owner.slug if self.owner else None
+    @field_validator("polaris_version")
+    @classmethod
+    def _validate_version(cls, value: str) -> str:
+        if value != "dev":
+            # Make sure it is a valid semantic version
+            Version(value)
+
+        current_version = po.__version__
+        if value != current_version:
+            logger.info(
+                f"The version of Polaris that was used to create the artifact ({value}) is different "
+                f"from the currently installed version of Polaris ({current_version})."
+            )
+        return value
 
     @field_validator("owner", mode="before")
     @classmethod
     def _validate_owner(cls, value: Union[str, HubOwner, None]):
         if isinstance(value, str):
             return HubOwner(slug=value)
         return value
 
+    @field_serializer("owner")
+    def _serialize_owner(self, value: HubOwner) -> Union[str, None]:
+        return value.slug if value else None
+
     @classmethod
     def from_json(cls, path: str):
         """Loads a benchmark from a JSON file.
 
         Args:
             path: Loads a benchmark specification from a JSON file.
         """
```

### Comparing `polaris-lib-0.2.5/polaris/benchmark/_base.py` & `polaris-lib-0.2.6/polaris/benchmark/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 import os
 from hashlib import md5
 from typing import Any, Callable, Optional, Union
 
 import fsspec
 import numpy as np
 import pandas as pd
+from datamol.utils import fs
 from pydantic import (
     Field,
     FieldValidationInfo,
     computed_field,
     field_serializer,
     field_validator,
     model_validator,
 )
 from sklearn.utils.multiclass import type_of_target
 
 from polaris._artifact import BaseArtifactModel
 from polaris.dataset import Dataset, Subset
 from polaris.evaluate import BenchmarkResults, Metric, ResultsType
 from polaris.hub.settings import PolarisHubSettings
-from polaris.utils import fs
 from polaris.utils.context import tmp_attribute_change
 from polaris.utils.dict2html import dict2html
 from polaris.utils.errors import InvalidBenchmarkError, PolarisChecksumError
 from polaris.utils.misc import listit
 from polaris.utils.types import (
     AccessType,
     HubOwner,
```

### Comparing `polaris-lib-0.2.5/polaris/benchmark/_definitions.py` & `polaris-lib-0.2.6/polaris/benchmark/_definitions.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/cli.py` & `polaris-lib-0.2.6/polaris/cli.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/curation/_chemistry_curator.py` & `polaris-lib-0.2.6/polaris/curation/_chemistry_curator.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/curation/_curator.py` & `polaris-lib-0.2.6/polaris/curation/_curator.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/curation/_data_curator.py` & `polaris-lib-0.2.6/polaris/curation/_data_curator.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/curation/utils.py` & `polaris-lib-0.2.6/polaris/curation/utils.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/curation/viz_utils.py` & `polaris-lib-0.2.6/polaris/curation/viz_utils.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/dataset/_column.py` & `polaris-lib-0.2.6/polaris/dataset/_column.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/dataset/_dataset.py` & `polaris-lib-0.2.6/polaris/dataset/_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import json
-import os.path
-from collections import defaultdict
 from hashlib import md5
 from typing import Dict, List, Optional, Tuple, Union
 
 import fsspec
 import numpy as np
 import pandas as pd
 import zarr
+from datamol.utils import fs
 from loguru import logger
 from pydantic import (
     Field,
+    PrivateAttr,
     computed_field,
     field_serializer,
     field_validator,
     model_validator,
 )
 
 from polaris._artifact import BaseArtifactModel
 from polaris.dataset._adapters import Adapter
 from polaris.dataset._column import ColumnAnnotation
-from polaris.hub.settings import PolarisHubSettings
-from polaris.utils import fs
+from polaris.hub.polarisfs import PolarisFileSystem
 from polaris.utils.constants import DEFAULT_CACHE_DIR
 from polaris.utils.dict2html import dict2html
 from polaris.utils.errors import InvalidDatasetError, PolarisChecksumError
-from polaris.utils.io import get_zarr_root, robust_copy
-from polaris.utils.types import AccessType, HttpUrlString, HubOwner, License
+from polaris.utils.types import AccessType, HttpUrlString, HubOwner, SupportedLicenseType
 
 # Constants
 _SUPPORTED_TABLE_EXTENSIONS = ["parquet"]
 _CACHE_SUBDIR = "datasets"
 _INDEX_SEP = "#"
 
 
@@ -47,49 +45,52 @@
         In that case, the table contains _pointers_ to these blobs that are dynamically loaded when needed.
 
     Attributes:
         table: The core data-structure, storing data-points in a row-wise manner. Can be specified as either a
             path to a `.parquet` file or a `pandas.DataFrame`.
         default_adapters: The adapters that the Dataset recommends to use by default to change the format of the data
             for specific columns.
+        zarr_root_path: The data for any pointer column should be saved in the Zarr archive this path points to.
         md5sum: The checksum is used to verify the version of the dataset specification. If specified, it will
             raise an error if the specified checksum doesn't match the computed checksum.
         readme: Markdown text that can be used to provide a formatted description of the dataset.
             If using the Polaris Hub, it is worth noting that this field is more easily edited through the Hub UI
             as it provides a rich text editor for writing markdown.
         annotations: Each column _can be_ annotated with a [`ColumnAnnotation`][polaris.dataset.ColumnAnnotation] object.
             Importantly, this is used to annotate whether a column is a pointer column.
         source: The data source, e.g. a DOI, Github repo or URI.
-        license: The dataset license
+        license: The dataset license. Polaris only supports some Creative Commons licenses. See [`SupportedLicenseType`][polaris.utils.types.SupportedLicenseType] for accepted ID values.
         curation_reference: A reference to the curation process, e.g. a DOI, Github repo or URI.
     For additional meta-data attributes, see the [`BaseArtifactModel`][polaris._artifact.BaseArtifactModel] class.
 
     Raises:
         InvalidDatasetError: If the dataset does not conform to the Pydantic data-model specification.
         PolarisChecksumError: If the specified checksum does not match the computed checksum.
     """
 
     # Public attributes
     # Data
     table: Union[pd.DataFrame, str]
     default_adapters: Dict[str, Adapter] = Field(default_factory=dict)
+    zarr_root_path: Optional[str] = None
     md5sum: Optional[str] = None
 
     # Additional meta-data
     readme: str = ""
     annotations: Dict[str, ColumnAnnotation] = Field(default_factory=dict)
     source: Optional[HttpUrlString] = None
-    license: Optional[License] = None
+    license: Optional[SupportedLicenseType] = None
     curation_reference: Optional[HttpUrlString] = None
 
     # Config
     cache_dir: Optional[str] = None  # Where to cache the data to if cache() is called.
 
     # Private attributes
-    _path_to_hash: Dict[str, Dict[str, str]] = defaultdict(dict)
+    _zarr_root: Optional[zarr.Group] = PrivateAttr(None)
+    _client = PrivateAttr(None)  # Optional[PolarisHubClient]
     _has_been_warned: bool = False
     _has_been_cached: bool = False
 
     @field_validator("table")
     def _validate_table(cls, v):
         """
         If the table is not a dataframe yet, assume it's a path and try load it.
@@ -149,17 +150,17 @@
         # Set the default cache dir if none and make sure it exists
         if m.cache_dir is None:
             m.cache_dir = fs.join(DEFAULT_CACHE_DIR, _CACHE_SUBDIR, m.name, m.md5sum)
         fs.mkdir(m.cache_dir, exist_ok=True)
 
         return m
 
-    @field_validator("default_adapters")
+    @field_validator("default_adapters", mode="before")
     def _validate_adapters(cls, value):
-        """Serializes the adapters"""
+        """Validate the adapters"""
         return {k: Adapter[v] if isinstance(v, str) else v for k, v in value.items()}
 
     @field_serializer("default_adapters")
     def _serialize_adapters(self, value: List[Adapter]):
         """Serializes the adapters"""
         return {k: v.name for k, v in value.items()}
 
@@ -184,14 +185,57 @@
         # Use the sum of the row-wise hashes s.t. the hash is insensitive to the row-ordering
         table_hash = pd.util.hash_pandas_object(df, index=False).sum()
         hash_fn.update(table_hash)
 
         checksum = hash_fn.hexdigest()
         return checksum
 
+    @property
+    def client(self):
+        """The Polaris Hub client used to interact with the Polaris Hub."""
+
+        # Import it here to prevent circular imports
+        from polaris.hub.client import PolarisHubClient
+
+        if self._client is None:
+            self._client = PolarisHubClient()
+        return self._client
+
+    @property
+    def zarr_root(self):
+        """Open the zarr archive in read-write mode if it is not already open."""
+        if self.zarr_root_path is None or not any(anno.is_pointer for anno in self.annotations.values()):
+            return None
+
+        saved_on_hub = PolarisFileSystem.is_polarisfs_path(self.zarr_root_path)
+        saved_remote = saved_on_hub or not fs.is_local_path(self.zarr_root_path)
+
+        if saved_remote and not self._has_been_warned:
+            logger.warning(
+                f"You're loading data from a remote location. "
+                f"To speed up this process, consider caching the dataset first "
+                f"using {self.__class__.__name__}.cache()"
+            )
+            self._has_been_warned = True
+
+        # We open the archive in read-only mode if it is saved on the Hub
+        if self._zarr_root is None:
+            try:
+                if saved_on_hub:
+                    self._zarr_root = self.client.open_zarr_file(
+                        self.owner, self.name, self.zarr_root_path, "r+"
+                    )
+                else:
+                    self._zarr_root = zarr.open_consolidated(self.zarr_root_path, mode="r+")
+            except KeyError as error:
+                raise InvalidDatasetError(
+                    "A Zarr archive associated with a Polaris dataset has to be consolidated."
+                ) from error
+        return self._zarr_root
+
     @computed_field
     @property
     def n_rows(self) -> int:
         """The number of rows in the dataset."""
         return len(self.rows)
 
     @computed_field
@@ -222,74 +266,47 @@
                 If None, will use the default adapters specified for the dataset.
 
         Returns:
             A numpy array with the data at the specified indices. If the column is a pointer column,
                 the content of the referenced file is loaded to memory.
         """
 
+        # Fetch adapters for dataset and a given column
         adapters = adapters or self.default_adapters
+        adapter = adapters.get(col)
 
-        def _load(p: str, index: Union[int, slice]) -> np.ndarray:
-            """Tiny helper function to reduce code repetition."""
-            arr = zarr.open(p, mode="r")
-            arr = arr[index]
-
-            if isinstance(index, slice):
-                arr = tuple(arr)
-
-            adapter = adapters.get(col)
-            if adapter is not None:
-                arr = adapter(arr)
-
-            return arr
-
+        # If not a pointer, return it here. Apply adapter if specified.
         value = self.table.loc[row, col]
         if not self.annotations[col].is_pointer:
+            if adapter is not None:
+                return adapter(value)
             return value
 
-        value, index = self._split_index_from_path(value)
+        # Load the data from the Zarr archive
+        path, index = self._split_index_from_path(value)
+        arr = self.zarr_root[path][index]
+
+        # Change to tuple if a slice
+        if isinstance(index, slice):
+            arr = tuple(arr)
+
+        # Adapt the input to the specified format
+        if adapter is not None:
+            arr = adapter(arr)
 
-        # In the case it is a pointer column, we need to load additional data into memory
-        # We first check if the data has been downloaded to the cache.
-        path = self._get_cache_path(column=col, value=value)
-        if fs.exists(path):
-            return _load(path, index)
-
-        # If it doesn't exist, we load from the original path and warn if not local
-        if not fs.is_local_path(value) and not self._has_been_warned:
-            logger.warning(
-                f"You're loading data from a remote location. "
-                f"To speed up this process, consider caching the dataset first "
-                f"using {self.__class__.__name__}.cache()"
-            )
-            self._has_been_warned = True
-        return _load(value, index)
+        return arr
 
     def upload_to_hub(
-        self,
-        env_file: Optional[Union[str, os.PathLike]] = None,
-        settings: Optional[PolarisHubSettings] = None,
-        cache_auth_token: bool = True,
-        access: Optional[AccessType] = "private",
-        owner: Optional[Union[HubOwner, str]] = None,
-        **kwargs: dict,
+        self, access: Optional[AccessType] = "private", owner: Optional[Union[HubOwner, str]] = None
     ):
         """
         Very light, convenient wrapper around the
         [`PolarisHubClient.upload_dataset`][polaris.hub.client.PolarisHubClient.upload_dataset] method.
         """
-        from polaris.hub.client import PolarisHubClient
-
-        with PolarisHubClient(
-            env_file=env_file,
-            settings=settings,
-            cache_auth_token=cache_auth_token,
-            **kwargs,
-        ) as client:
-            return client.upload_dataset(self, access=access, owner=owner)
+        self.client.upload_dataset(self, access=access, owner=owner)
 
     @classmethod
     def from_json(cls, path: str):
         """Loads a benchmark from a JSON file.
         Overrides the method from the base class to remove the caching dir from the file to load from,
         as that should be user dependent.
 
@@ -319,27 +336,34 @@
 
         Returns:
             The path to the JSON file.
         """
         fs.mkdir(destination, exist_ok=True)
         table_path = fs.join(destination, "table.parquet")
         dataset_path = fs.join(destination, "dataset.json")
-        pointer_dir = fs.join(destination, "data")
-
-        # Save additional data
-        new_table = self._copy_and_update_pointers(pointer_dir, inplace=False)
+        zarr_archive = fs.join(destination, "data.zarr")
 
         # Lu: Avoid serilizing and sending None to hub app.
         serialized = self.model_dump(exclude={"cache_dir"}, exclude_none=True)
         serialized["table"] = table_path
 
-        # We need to recompute the checksum, as the pointer paths have changed
-        serialized["md5sum"] = self._compute_checksum(new_table)
+        # Copy over Zarr data to the destination
+        if self.zarr_root is not None:
+            dest = zarr.open(zarr_archive, "w")
+            zarr.copy_all(source=self.zarr_root, dest=dest)
+
+            # Copy the .zmetadata file
+            # To track discussions on whether this should be done by copy_all()
+            # see https://github.com/zarr-developers/zarr-python/issues/1731
+            zmetadata_content = self.zarr_root.store.store[".zmetadata"]
+            dest.store[".zmetadata"] = zmetadata_content
+
+            serialized["zarr_root_path"] = zarr_archive
 
-        new_table.to_parquet(table_path)
+        self.table.to_parquet(table_path)
         with fsspec.open(dataset_path, "w") as f:
             json.dump(serialized, f)
 
         return dataset_path
 
     def cache(self, cache_dir: Optional[str] = None) -> str:
         """Caches the dataset by downloading all additional data for pointer columns to a local directory.
@@ -351,40 +375,24 @@
         Returns:
             The path to the cache directory.
         """
 
         if cache_dir is not None:
             self.cache_dir = cache_dir
 
+        self.to_json(self.cache_dir)
+
+        if self.zarr_root_path is not None:
+            self.zarr_root_path = fs.join(self.cache_dir, "data.zarr")
+            self._zarr_root = None
+
         if not self._has_been_cached:
-            self._copy_and_update_pointers(self.cache_dir, inplace=True)
             self._has_been_cached = True
         return self.cache_dir
 
-    def _get_cache_path(self, column: str, value: str) -> Optional[str]:
-        """
-        Returns where the data _would be_ cached for any entry in the pointer columns,
-        or None if the column is not a pointer column.
-        """
-        if not self.annotations[column].is_pointer:
-            return
-
-        if value not in self._path_to_hash[column]:
-            h = md5(value.encode("utf-8")).hexdigest()
-
-            value, _ = self._split_index_from_path(value)
-            ext = fs.get_extension(value)
-            dst = fs.join(self.cache_dir, column, f"{h}.{ext}")
-
-            # The reason for caching the path is to speed-up retrieval. Hashing can be slow and with large
-            # datasets this could become a bottleneck.
-            self._path_to_hash[column][value] = dst
-
-        return self._path_to_hash[column][value]
-
     def size(self):
         return self.rows, self.n_columns
 
     def _split_index_from_path(self, path: str) -> Tuple[str, Optional[int]]:
         """
         Paths can have an additional index appended to them.
         This extracts that index from the path.
@@ -398,47 +406,14 @@
                 index = int(index[0])
             elif len(index) == 2:
                 index = slice(int(index[0]), int(index[1]))
             else:
                 raise ValueError(f"Invalid index format: {index}")
         return path, index
 
-    def _copy_and_update_pointers(
-        self, save_dir: str, table: Optional[pd.DataFrame] = None, inplace: bool = False
-    ) -> pd.DataFrame:
-        """Copy and update the path in the table to the new destination"""
-
-        def fn(path):
-            """Helper function that can be used within Pandas apply to copy and update all files"""
-
-            # We copy the entire .zarr hierarchy
-            root = get_zarr_root(path)
-            if root is None:
-                raise NotImplementedError(
-                    "Only the .zarr file format is currently supported for pointer columns"
-                )
-
-            # We could introduce name collisions here and thus use a hash of the original path for the destination
-            dst = fs.join(save_dir, f"{md5(root.encode('utf-8')).hexdigest()}.zarr")
-            robust_copy(root, dst)
-
-            diff = os.path.relpath(path, root)
-            dst = fs.join(dst, diff)
-            return dst
-
-        if table is None:
-            table = self.table
-        if not inplace:
-            table = self.table.copy(deep=True)
-
-        for c in table.columns:
-            if self.annotations[c].is_pointer:
-                table[c] = table[c].apply(fn)
-        return table
-
     def __getitem__(self, item):
         """Allows for indexing the dataset directly"""
         ret = self.table.loc[item]
         if isinstance(ret, pd.Series):
             # Load the data from the pointer columns
 
             if ret.name in self.table.columns:
@@ -482,7 +457,12 @@
         return self.__repr__()
 
     def __eq__(self, other):
         """Whether two datasets are equal is solely determined by the checksum"""
         if not isinstance(other, Dataset):
             return False
         return self.md5sum == other.md5sum
+
+    def __del__(self):
+        """Close the connection of the client"""
+        if self._client is not None:
+            self._client.close()
```

### Comparing `polaris-lib-0.2.5/polaris/dataset/_factory.py` & `polaris-lib-0.2.6/polaris/dataset/_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,15 +85,19 @@
     @property
     def zarr_root(self) -> zarr.Group:
         """
         The root of the zarr archive for the Dataset that is being built.
         All data for a single dataset is expected to be stored in the same Zarr archive.
         """
         if self._zarr_root is None:
-            self._zarr_root = zarr.open(self.zarr_root_path, "w")
+            # NOTE (cwognum): The DirectoryStore is the default store when calling zarr.open
+            #   I nevertheless explicitly set it here to make it clear that this is a design decision.
+            #   We could consider using different stores, such as the NestedDirectoryStore.
+            store = zarr.DirectoryStore(self.zarr_root_path)
+            self._zarr_root = zarr.open(store, "w")
             if not isinstance(self._zarr_root, zarr.Group):
                 raise ValueError("The root of the zarr hierarchy should be a group")
         return self._zarr_root
 
     def register_converter(self, ext: str, converter: Converter):
         """
         Registers a new converter for a specific file type.
@@ -207,18 +211,20 @@
             raise ValueError(f"No converter found for extension {ext}")
 
         table, annotations, adapters = converter.convert(path, self)
         self.add_columns(table, annotations, adapters)
 
     def build(self) -> Dataset:
         """Returns a Dataset based on the current state of the factory."""
+        zarr.consolidate_metadata(self.zarr_root.store)
         return Dataset(
             table=self._table,
             annotations=self._annotations,
             default_adapters=self._adapters,
+            zarr_root_path=self.zarr_root_path,
         )
 
     def reset(self, zarr_root_path: Optional[str] = None):
         """
         Resets the factory to its initial state to start building the next dataset from scratch.
         Note that this will not reset the registered converters.
```

### Comparing `polaris-lib-0.2.5/polaris/dataset/_subset.py` & `polaris-lib-0.2.6/polaris/dataset/_subset.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/dataset/converters/_base.py` & `polaris-lib-0.2.6/polaris/dataset/converters/_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 class Converter(abc.ABC):
     @abc.abstractmethod
     def convert(self, path: str) -> FactoryProduct:
         """This converts a file into a table and possibly annotations"""
         raise NotImplementedError
 
     @staticmethod
-    def get_pointer(root: str, column: str, index: Union[int, slice]) -> str:
+    def get_pointer(column: str, index: Union[int, slice]) -> str:
         """
         Creates a pointer.
 
         Args:
-            root: The root path of the zarr hierarchy.
             column: The name of the column. Each column has its own group in the root.
             index: The index or slice of the pointer.
         """
         if isinstance(index, slice):
             index_substr = f"{_INDEX_SEP}{index.start}:{index.stop}"
         else:
             index_substr = f"{_INDEX_SEP}{index}"
-        return f"{root}/{column}{index_substr}"
+        return f"{column}{index_substr}"
```

### Comparing `polaris-lib-0.2.5/polaris/dataset/converters/_sdf.py` & `polaris-lib-0.2.6/polaris/dataset/converters/_sdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,24 +119,24 @@
                     raise ValueError(
                         f"After grouping by {self.groupby_key}, values for other columns are not unique within a group. "
                         "Please handle this manually to ensure aggregation is done correctly."
                     )
 
                 # Get the pointer path
                 pointer_idx = f"{start}:{end}" if start != end else f"{start}"
-                pointer = self.get_pointer(factory.zarr_root_path, self.mol_column, pointer_idx)
+                pointer = self.get_pointer(self.mol_column, pointer_idx)
 
                 # Get the single unique value per column for the group and append
                 unique_values = [group[col].unique()[0] for col in df.columns]
                 grouped.loc[len(grouped)] = [*unique_values, pointer]
 
             df = grouped
 
         else:
-            pointers = [self.get_pointer(factory.zarr_root_path, self.mol_column, i) for i in range(len(df))]
+            pointers = [self.get_pointer(self.mol_column, i) for i in range(len(df))]
             df[self.mol_column] = pd.Series(pointers)
 
         # Set the annotations
         annotations = {self.mol_column: ColumnAnnotation(is_pointer=True, modality=Modality.MOLECULE_3D)}
         if self.smiles_column is not None:
             annotations[self.smiles_column] = ColumnAnnotation(modality=Modality.MOLECULE)
```

### Comparing `polaris-lib-0.2.5/polaris/dataset/converters/_zarr.py` & `polaris-lib-0.2.6/polaris/dataset/converters/_zarr.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,22 +30,20 @@
     def convert(self, path: str, factory: "DatasetFactory") -> FactoryProduct:
         src = zarr.open(path, "r")
 
         v = next(src.group_keys(), None)
         if v is not None:
             raise ValueError("The root of the zarr hierarchy should only contain arrays.")
 
+        # Copy to the source zarr, so everything is in one place
+        zarr.copy_all(source=src, dest=factory.zarr_root)
+
         # Construct the table
         # Parse any group into a column
         data = defaultdict(dict)
         for col, arr in src.arrays():
-            # Copy to the source zarr, so everything is in one place
-            dst = zarr.open_group("/".join([factory.zarr_root_path, col]), "w")
-            zarr.copy(arr, dst)
-
             for i in range(len(arr)):
-                # In case all data is saved in a single array, we construct a path with an index suffix.
-                data[col][i] = self.get_pointer(path, arr.name, i)
+                data[col][i] = self.get_pointer(arr.name.removeprefix("/"), i)
 
         # Construct the dataset
         table = pd.DataFrame(data)
         return table, {k: ColumnAnnotation(is_pointer=True) for k in table.columns}, {}
```

### Comparing `polaris-lib-0.2.5/polaris/evaluate/_metric.py` & `polaris-lib-0.2.6/polaris/evaluate/_metric.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/evaluate/_results.py` & `polaris-lib-0.2.6/polaris/evaluate/_results.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/hub/client.py` & `polaris-lib-0.2.6/polaris/hub/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import json
 import os
 import ssl
 import webbrowser
 from hashlib import md5
 from io import BytesIO
-from typing import Callable, Optional, Union
+from typing import Callable, Optional, Union, get_args
 from urllib.parse import urljoin
 
 import certifi
 import fsspec
 import httpx
 import pandas as pd
 import zarr
 from authlib.common.security import generate_token
 from authlib.integrations.base_client.errors import InvalidTokenError, MissingTokenError
 from authlib.integrations.httpx_client import OAuth2Client, OAuthError
 from authlib.oauth2.client import OAuth2Client as _OAuth2Client
+from datamol.utils import fs
 from httpx import HTTPStatusError
 from httpx._types import HeaderTypes, URLTypes
 from loguru import logger
 
 from polaris.benchmark import (
     BenchmarkSpecification,
     MultiTaskBenchmarkSpecification,
     SingleTaskBenchmarkSpecification,
 )
 from polaris.dataset import Dataset
 from polaris.evaluate import BenchmarkResults
 from polaris.hub.polarisfs import PolarisFileSystem
 from polaris.hub.settings import PolarisHubSettings
-from polaris.utils import fs
 from polaris.utils.constants import DEFAULT_CACHE_DIR
-from polaris.utils.errors import PolarisHubError, PolarisUnauthorizedError
-from polaris.utils.types import AccessType, HubOwner, IOMode, TimeoutTypes
+from polaris.utils.context import tmp_attribute_change
+from polaris.utils.errors import InvalidDatasetError, PolarisHubError, PolarisUnauthorizedError
+from polaris.utils.types import AccessType, HubOwner, IOMode, SupportedLicenseType, TimeoutTypes
 
 _HTTPX_SSL_ERROR_CODE = "[SSL: CERTIFICATE_VERIFY_FAILED]"
 
 
 class PolarisHubClient(OAuth2Client):
     """
     A client for the Polaris Hub API. The Polaris Hub is a central repository of datasets, benchmarks and results.
@@ -110,14 +111,15 @@
             scope=settings.scopes,
             token=token,
             token_endpoint=self.settings.token_fetch_url,
             code_challenge_method="S256",
             # httpx.Client
             base_url=settings.api_url,
             verify=verify,
+            timeout=self.settings.default_timeout,
             # Extra
             **kwargs,
         )
 
     def _load_from_signed_url(self, url: URLTypes, load_fn: Callable, headers: Optional[HeaderTypes] = None):
         """Utility function to load a file from a signed URL"""
         response = self.get(url, auth=None, headers=headers)  # type: ignore
@@ -148,14 +150,33 @@
         try:
             response = response.json()
         except json.JSONDecodeError:
             pass
 
         return response
 
+    def _normalize_owner(
+        self,
+        artifact_owner: Optional[Union[str, HubOwner]] = None,
+        parameter_owner: Optional[Union[str, HubOwner]] = None,
+    ) -> HubOwner:
+        """
+        Normalize the owner of an artifact to a `HubOwner` instance.
+        The parameter owner takes precedence over the artifact owner.
+        """
+        if parameter_owner is not None:
+            artifact_owner = parameter_owner
+
+        if artifact_owner is None:
+            raise ValueError(
+                "Either specify the `owner` attribute for the artifact or pass the `owner` parameter."
+            )
+
+        return artifact_owner if isinstance(artifact_owner, HubOwner) else HubOwner(slug=artifact_owner)
+
     # =========================
     #     Overrides
     # =========================
 
     @_OAuth2Client.token.setter
     def token(self, value):
         """Override the token setter to additionally save the token to a cache"""
@@ -334,36 +355,43 @@
 
         if not verify_checksum:
             response.pop("md5Sum", None)
 
         return Dataset(**response)
 
     def open_zarr_file(
-        self, owner: Union[str, HubOwner], name: str, path: str, mode: IOMode
+        self, owner: Union[str, HubOwner], name: str, path: str, mode: IOMode, as_consolidated: bool = True
     ) -> zarr.hierarchy.Group:
         """Open a Zarr file from a Polaris dataset
 
         Args:
             owner: Which Hub user or organization owns the artifact.
             name: Name of the dataset.
             path: Path to the Zarr file within the dataset.
             mode: The mode in which the file is opened.
+            as_consolidated: Whether to open the store with consolidated metadata for optimized reading. This is only applicable in 'r' and 'r+' modes.
 
         Returns:
             The Zarr object representing the dataset.
         """
+        if as_consolidated and mode not in ["r", "r+"]:
+            raise ValueError("Consolidated archives can only be used with 'r' or 'r+' mode.")
+
         polaris_fs = PolarisFileSystem(
             polaris_client=self,
             dataset_owner=owner,
             dataset_name=name,
         )
 
         try:
             store = zarr.storage.FSStore(path, fs=polaris_fs)
+            if mode in ["r", "r+"] and as_consolidated:
+                return zarr.open_consolidated(store, mode=mode)
             return zarr.open(store, mode=mode)
+
         except Exception as e:
             raise PolarisHubError("Error opening Zarr store") from e
 
     def list_benchmarks(self, limit: int = 100, offset: int = 0) -> list[str]:
         """List all available benchmarks on the Polaris Hub.
 
         Args:
@@ -439,27 +467,19 @@
             Importantly, `results.benchmark_name` and `results.benchmark_owner` must be specified
             and match an existing benchmark on the Polaris Hub. If these results were generated by
             `benchmark.evaluate(...)`, this is done automatically.
 
         Args:
             results: The results to upload.
             access: Grant public or private access to result
-            owner: Which Hub user or organization owns the artifact.
-                Optional if and only if the `benchmark.owner` attribute is set.
+            owner: Which Hub user or organization owns the artifact. Takes precedence over `results.owner`.
         """
 
         # Get the serialized model data-structure
-
-        if results.owner is None:
-            if owner is None:
-                raise ValueError(
-                    "The `owner` argument must be specified if the `results.owner` attribute is not set."
-                )
-            results.owner = owner if isinstance(owner, HubOwner) else HubOwner(slug=owner)
-
+        results.owner = self._normalize_owner(results.owner, owner)
         result_json = results.model_dump(by_alias=True, exclude_none=True)
 
         # Make a request to the hub
         response = self._base_request_to_hub(
             url="/result", method="POST", json={"access": access, **result_json}
         )
 
@@ -494,32 +514,39 @@
             dataset: The dataset to upload.
             access: Grant public or private access to result
             timeout: Request timeout values. User can modify the value when uploading large dataset as needed.
                 This can be a single value with the timeout in seconds for all IO operations, or a more granular
                 tuple with (connect_timeout, write_timeout). The type of the the timout parameter comes from `httpx`.
                 Since datasets can get large, it might be needed to increase the write timeout for larger datasets.
                 See also: https://www.python-httpx.org/advanced/#timeout-configuration
-            owner: Which Hub user or organization owns the artifact.
-                Optional if and only if the `benchmark.owner` attribute is set.
+            owner: Which Hub user or organization owns the artifact. Takes precedence over `dataset.owner`.
         """
 
-        if dataset.owner is None:
-            if owner is None:
-                raise ValueError(
-                    "The `owner` argument must be specified if the `dataset.owner` attribute is not set."
-                )
-            dataset.owner = owner if isinstance(owner, HubOwner) else HubOwner(slug=owner)
+        # Check if a dataset license was specified prior to upload
+        if not dataset.license:
+            raise InvalidDatasetError(
+                f"\nPlease specify a supported license for this dataset prior to uploading to the Polaris Hub.\nOnly some Creative Commons licenses are supported - {get_args(SupportedLicenseType)}. For more information, see https://creativecommons.org/share-your-work/cclicenses/"
+            )
+
+        # Normalize timeout
+        if timeout is None:
+            timeout = self.settings.default_timeout
 
         # Get the serialized data-model
-        # We exclude the table as it handled separately and the cache_dir as it is user-specific
+        # We exclude the table as it handled separately and we exclude the cache_dir as it is user-specific
+        dataset.owner = self._normalize_owner(dataset.owner, owner)
         dataset_json = dataset.model_dump(exclude={"cache_dir", "table"}, exclude_none=True, by_alias=True)
 
-        # Uploading a dataset is a two-step process.
+        # We will save the Zarr archive to the Hub as well
+        dataset_json["zarrRootPath"] = f"{PolarisFileSystem.protocol}://data.zarr"
+
+        # Uploading a dataset is a three-step process.
         # 1. Upload the dataset meta data to the hub and prepare the hub to receive the parquet file
         # 2. Upload the parquet file to the hub
+        # 3. Upload the associated Zarr archive
         # TODO: Revert step 1 in case step 2 fails - Is this needed? Or should this be taken care of by the hub?
 
         # Write the parquet file directly to a buffer
         buffer = BytesIO()
         dataset.table.to_parquet(buffer, engine="auto")
         parquet_size = len(buffer.getbuffer())
         parquet_md5 = md5(buffer.getbuffer()).hexdigest()
@@ -535,24 +562,26 @@
                     "size": parquet_size,
                     "fileType": "parquet",
                     "md5sum": parquet_md5,
                 },
                 "access": access,
                 **dataset_json,
             },
+            timeout=timeout,
         )
 
         # Step 2: Upload the parquet file
         # create an empty PUT request to get the table content URL from cloudflare
         hub_response = self.request(
             url=response["tableContent"]["url"],
             method="PUT",
             headers={
                 "Content-type": "application/vnd.apache.parquet",
             },
+            timeout=timeout,
         )
 
         if hub_response.status_code == 307:
             # If the hub returns a 307 redirect, we need to follow it to get the signed URL
             hub_response_body = hub_response.json()
             # Upload the data to the cloudflare url
             bucket_response = self.request(
@@ -564,14 +593,36 @@
                 timeout=timeout,  # required for large size dataset
             )
             bucket_response.raise_for_status()
 
         else:
             hub_response.raise_for_status()
 
+        # Step 3: Upload any associated Zarr archive
+        if dataset.zarr_root is not None:
+            with tmp_attribute_change(self.settings, "default_timeout", timeout):
+                # Copy the Zarr archive to the hub
+                dest = self.open_zarr_file(
+                    owner=dataset.owner,
+                    name=dataset.name,
+                    path=dataset_json["zarrRootPath"],
+                    mode="w",
+                    as_consolidated=False,
+                )
+
+                # Locally consolidate Zarr archive metadata. Future updates on handling consolidated
+                # metadata based on Zarr developers' recommendations can be tracked at:
+                # https://github.com/zarr-developers/zarr-python/issues/1731
+                zarr.consolidate_metadata(dataset.zarr_root.store.store)
+                zmetadata_content = dataset.zarr_root.store.store[".zmetadata"]
+                dest.store[".zmetadata"] = zmetadata_content
+
+                logger.info("Copying Zarr archive to the Hub. This may take a while.")
+                zarr.copy_all(source=dataset.zarr_root, dest=dest, log=logger.info)
+
         logger.success(
             "Your dataset has been successfully uploaded to the Hub. "
             f"View it here: {urljoin(self.settings.hub_url, f'datasets/{dataset.owner}/{dataset.name}')}"
         )
 
         return response
 
@@ -596,26 +647,19 @@
         Note: Non-existent datasets
             The client will _not_ upload the associated dataset to the hub if it does not yet exist.
             Make sure to specify an existing dataset or upload the dataset first.
 
         Args:
             benchmark: The benchmark to upload.
             access: Grant public or private access to result
-            owner: Which Hub user or organization owns the artifact.
-                Optional if and only if the `benchmark.owner` attribute is set.
+            owner: Which Hub user or organization owns the artifact. Takes precedence over `benchmark.owner`.
         """
-        if benchmark.owner is None:
-            if owner is None:
-                raise ValueError(
-                    "The `owner` argument must be specified if the `benchmark.owner` attribute is not set."
-                )
-            benchmark.owner = owner if isinstance(owner, HubOwner) else HubOwner(slug=owner)
-
         # Get the serialized data-model
         # We exclude the dataset as we expect it to exist on the hub already.
+        benchmark.owner = self._normalize_owner(benchmark.owner, owner)
         benchmark_json = benchmark.model_dump(exclude={"dataset"}, exclude_none=True, by_alias=True)
         benchmark_json["datasetArtifactId"] = benchmark.dataset.artifact_id
         benchmark_json["access"] = access
 
         url = f"/benchmark/{benchmark.owner}/{benchmark.name}"
         response = self._base_request_to_hub(url=url, method="PUT", json=benchmark_json)
```

### Comparing `polaris-lib-0.2.5/polaris/hub/polarisfs.py` & `polaris-lib-0.2.6/polaris/hub/polarisfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+import hashlib
 from datetime import datetime, timezone
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+
 import fsspec
-import hashlib
 
 from polaris.utils.errors import PolarisHubError
 from polaris.utils.types import TimeoutTypes
 
 if TYPE_CHECKING:
     from polaris.hub.client import PolarisHubClient
 
@@ -50,14 +51,26 @@
         self.polaris_client = polaris_client
         self.default_timeout = self.polaris_client.settings.default_timeout
 
         # Prefix to remove from ls entries
         self.prefix = f"dataset/{dataset_owner}/{dataset_name}/"
         self.base_path = f"/storage/{self.prefix.rstrip('/')}"
 
+    @staticmethod
+    def is_polarisfs_path(path: str) -> bool:
+        """Check if the given path is a PolarisFS path.
+
+        Args:
+            path: The path to check.
+
+        Returns:
+            True if the path is a PolarisFS path; otherwise, False.
+        """
+        return path.startswith(f"{PolarisFileSystem.protocol}://")
+
     def ls(
         self,
         path: str,
         detail: bool = False,
         timeout: Optional[TimeoutTypes] = None,
         **kwargs: dict,
     ) -> Union[List[str], List[Dict[str, Any]]]:
@@ -169,15 +182,15 @@
         """
         if timeout is None:
             timeout = self.default_timeout
 
         pipe_path = self.sep.join([self.base_path, path])
 
         # PUT request to Polaris Hub to put object in path
-        response = self.polaris_client.put(pipe_path, timeout=timeout, content=content)
+        response = self.polaris_client.put(pipe_path, timeout=timeout)
 
         if response.status_code != 307:
             raise PolarisHubError("Could not get signed URL from Polaris Hub.")
 
         hub_response_body = response.json()
         signed_url = hub_response_body["url"]
```

### Comparing `polaris-lib-0.2.5/polaris/hub/settings.py` & `polaris-lib-0.2.6/polaris/hub/settings.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/loader/load.py` & `polaris-lib-0.2.6/polaris/loader/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 
 import fsspec
+from datamol.utils import fs
 
 from polaris.benchmark._definitions import (
     MultiTaskBenchmarkSpecification,
     SingleTaskBenchmarkSpecification,
 )
 from polaris.dataset import Dataset, create_dataset_from_file
 from polaris.hub.client import PolarisHubClient
-from polaris.utils import fs
 
 
 def load_dataset(path: str, verify_checksum: bool = True) -> Dataset:
     """
     Loads a Polaris dataset.
 
     In Polaris, a dataset is a tabular data structure that stores data-points in a row-wise manner.
```

### Comparing `polaris-lib-0.2.5/polaris/utils/dict2html.py` & `polaris-lib-0.2.6/polaris/utils/dict2html.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/utils/errors.py` & `polaris-lib-0.2.6/polaris/utils/errors.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/utils/httpx.py` & `polaris-lib-0.2.6/polaris/utils/httpx.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/utils/misc.py` & `polaris-lib-0.2.6/polaris/utils/misc.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/polaris/utils/types.py` & `polaris-lib-0.2.6/polaris/utils/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-import json
 from enum import Enum
-from typing import Annotated, Any, ClassVar, Literal, Optional, Tuple, Union
+from typing import Annotated, Any, Literal, Optional, Tuple, Union
 
-import fsspec
 import numpy as np
-from loguru import logger
 from pydantic import (
     AfterValidator,
     BaseModel,
     ConfigDict,
     HttpUrl,
     StringConstraints,
-    model_validator,
 )
 from pydantic.alias_generators import to_camel
 from typing_extensions import TypeAlias
 
 SplitIndicesType: TypeAlias = list[int]
 """
 A split is defined by a sequence of integers.
@@ -92,14 +88,21 @@
 """
 
 IOMode: TypeAlias = Literal["r", "r+", "a", "w", "w-"]
 """
 Type to specify the mode for input/output operations (I/O) when interacting with a file or resource.
 """
 
+SupportedLicenseType: TypeAlias = Literal[
+    "CC-BY-4.0", "CC-BY-SA-4.0", "CC-BY-NC-4.0", "CC-BY-NC-SA-4.0", "CC0-1.0"
+]
+"""
+Supported license types for dataset uploads to Polaris Hub
+"""
+
 
 class HubOwner(BaseModel):
     """An owner of an artifact on the Polaris Hub
 
     The slug is most important as it is the user-facing part of this data model.
     The externalId and type are added to be consistent with the model returned by the Polaris Hub .
     """
@@ -111,56 +114,14 @@
     # Pydantic config
     model_config = ConfigDict(alias_generator=to_camel, populate_by_name=True)
 
     def __str__(self):
         return self.slug
 
 
-class License(BaseModel):
-    """An artifact license.
-
-    Attributes:
-        id: The license ID. Either from [SPDX](https://spdx.org/licenses/) or custom.
-        reference: A reference to the license text. If the ID is found in SPDX, this is automatically set.
-            Else it is required to manually specify this.
-    """
-
-    SPDX_LICENSE_DATA_PATH: ClassVar[str] = (
-        "https://raw.githubusercontent.com/spdx/license-list-data/main/json/licenses.json"
-    )
-
-    id: str
-    reference: Optional[HttpUrlString] = None
-
-    @model_validator(mode="after")  # type: ignore
-    @classmethod
-    def _validate_license_id(cls, m: "License"):
-        """
-        If a license ID exists in the SPDX database, we use the reference from there.
-        Otherwise, it is up to the user to specify the license.
-        """
-
-        # Load the ground truth references
-        with fsspec.open(cls.SPDX_LICENSE_DATA_PATH) as f:
-            data = json.load(f)
-        data = {license["licenseId"]: license for license in data["licenses"]}
-
-        if m.id in data:
-            if m.reference is not None and m.reference != data[m.id]["reference"]:
-                logger.warning(f"Found license ID {m.id} in SPDX, using the associated reference.")
-            m.reference = data[m.id]["reference"]
-
-        if m.id not in data and m.reference is None:
-            raise ValueError(
-                f"License with ID {m.id} not found in SPDX. "
-                "It is required to then also specify the name and reference."
-            )
-        return m
-
-
 class TargetType(Enum):
     """The high-level classification of different targets."""
 
     REGRESSION = "regression"
     CLASSIFICATION = "classification"
```

### Comparing `polaris-lib-0.2.5/polaris_lib.egg-info/PKG-INFO` & `polaris-lib-0.2.6/polaris_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polaris-lib
-Version: 0.2.5
+Version: 0.2.6
 Summary: Client for the Polaris Hub.
 Author-email: Lu Zhu <lu@valencediscovery.com>, Hadrien Mary <hadrien@valencediscovery.com>, Julien St-Laurent <julien.stl@valencediscovery.com>, Cas Wognum <cas@valencediscovery.com>
 Project-URL: Website, https://polarishub.io/
 Project-URL: Source Code, https://github.com/polaris-hub/polaris
 Project-URL: Bug Tracker, https://github.com/polaris-hub/polaris/issues
 Project-URL: Documentation, https://polaris-hub.github.io/polaris/
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polaris-lib Version: 0.2.5 Summary: Client for the
+Metadata-Version: 2.1 Name: polaris-lib Version: 0.2.6 Summary: Client for the
 Polaris Hub. Author-email: Lu Zhu
 valencediscovery.com>, Hadrien Mary
 valencediscovery.com>, Julien St-Laurent
 valencediscovery.com>, Cas Wognum
 valencediscovery.com> Project-URL: Website, https://polarishub.io/ Project-URL:
 Source Code, https://github.com/polaris-hub/polaris Project-URL: Bug Tracker,
 https://github.com/polaris-hub/polaris/issues Project-URL: Documentation,
```

### Comparing `polaris-lib-0.2.5/polaris_lib.egg-info/SOURCES.txt` & `polaris-lib-0.2.6/polaris_lib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -69,17 +69,15 @@
 polaris/loader/__init__.py
 polaris/loader/load.py
 polaris/utils/__init__.py
 polaris/utils/constants.py
 polaris/utils/context.py
 polaris/utils/dict2html.py
 polaris/utils/errors.py
-polaris/utils/fs.py
 polaris/utils/httpx.py
-polaris/utils/io.py
 polaris/utils/misc.py
 polaris/utils/types.py
 polaris_lib.egg-info/PKG-INFO
 polaris_lib.egg-info/SOURCES.txt
 polaris_lib.egg-info/dependency_links.txt
 polaris_lib.egg-info/entry_points.txt
 polaris_lib.egg-info/requires.txt
```

### Comparing `polaris-lib-0.2.5/pyproject.toml` & `polaris-lib-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/tests/conftest.py` & `polaris-lib-0.2.6/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import datamol as dm
 import numpy as np
 import pytest
 import zarr
+from datamol.utils import fs
 
+import polaris as po
 from polaris.benchmark import (
     MultiTaskBenchmarkSpecification,
     SingleTaskBenchmarkSpecification,
 )
 from polaris.dataset import ColumnAnnotation, Dataset
-from polaris.utils import fs
-from polaris.utils.types import HubOwner, License
+from polaris.utils.types import HubOwner
+
+
+def check_version(artifact):
+    assert po.__version__ == artifact.polaris_version
 
 
 @pytest.fixture(scope="module")
 def test_data():
     data = dm.data.freesolv()[:100]
     # set an abitrary threshold for testing purpose.
     data["CLASS_expt"] = data["expt"].gt(0).astype(int).values
@@ -51,41 +56,44 @@
 @pytest.fixture(scope="module")
 def test_user_owner():
     return HubOwner(userId="test-user", slug="test-user")
 
 
 @pytest.fixture(scope="module")
 def test_dataset(test_data, test_org_owner):
-    return Dataset(
+    dataset = Dataset(
         table=test_data,
         name="test-dataset",
         source="https://www.example.com",
-        annotations={"expt": ColumnAnnotation(is_pointer=False, user_attributes={"unit": "kcal/mol"})},
+        annotations={"expt": ColumnAnnotation(user_attributes={"unit": "kcal/mol"})},
         tags=["tagA", "tagB"],
         user_attributes={"attributeA": "valueA", "attributeB": "valueB"},
         owner=test_org_owner,
-        license=License(id="MIT"),
+        license="CC-BY-4.0",
         curation_reference="https://www.example.com",
     )
+    check_version(dataset)
+    return dataset
 
 
 @pytest.fixture(scope="function")
 def zarr_archive(tmp_path):
-    tmp_path = fs.join(str(tmp_path), "data.zarr")
-    root = zarr.open_group(tmp_path, mode="w")
+    tmp_path = fs.join(tmp_path, "data.zarr")
+    root = zarr.open(tmp_path, mode="w")
     root.array("A", data=np.random.random((100, 2048)))
     root.array("B", data=np.random.random((100, 2048)))
+    zarr.consolidate_metadata(root.store)
     return tmp_path
 
 
 @pytest.fixture(scope="function")
 def test_single_task_benchmark(test_dataset):
     train_indices = list(range(90))
     test_indices = list(range(90, 100))
-    return SingleTaskBenchmarkSpecification(
+    benchmark = SingleTaskBenchmarkSpecification(
         name="single-task-benchmark",
         dataset=test_dataset,
         metrics=[
             "mean_absolute_error",
             "mean_squared_error",
             "r2",
             "spearmanr",
@@ -93,36 +101,40 @@
             "explained_var",
         ],
         main_metric="mean_absolute_error",
         split=(train_indices, test_indices),
         target_cols="expt",
         input_cols="smiles",
     )
+    check_version(benchmark)
+    return benchmark
 
 
 @pytest.fixture(scope="function")
 def test_single_task_benchmark_clf(test_dataset):
     train_indices = list(range(90))
     test_indices = list(range(90, 100))
-    return SingleTaskBenchmarkSpecification(
+    benchmark = SingleTaskBenchmarkSpecification(
         name="single-task-benchmark",
         dataset=test_dataset,
         main_metric="accuracy",
         metrics=["accuracy", "f1", "roc_auc", "pr_auc", "mcc", "cohen_kappa"],
         split=(train_indices, test_indices),
         target_cols="CLASS_expt",
         input_cols="smiles",
     )
+    check_version(benchmark)
+    return benchmark
 
 
 @pytest.fixture(scope="function")
 def test_single_task_benchmark_multiple_test_sets(test_dataset):
     train_indices = list(range(90))
     test_indices = {"test_1": list(range(90, 95)), "test_2": list(range(95, 100))}
-    return SingleTaskBenchmarkSpecification(
+    benchmark = SingleTaskBenchmarkSpecification(
         name="single-task-benchmark",
         dataset=test_dataset,
         metrics=[
             "mean_absolute_error",
             "mean_squared_error",
             "r2",
             "spearmanr",
@@ -130,22 +142,24 @@
             "explained_var",
         ],
         main_metric="r2",
         split=(train_indices, test_indices),
         target_cols="expt",
         input_cols="smiles",
     )
+    check_version(benchmark)
+    return benchmark
 
 
 @pytest.fixture(scope="function")
 def test_multi_task_benchmark(test_dataset):
     # For the sake of simplicity, just use a small set of indices
     train_indices = list(range(90))
     test_indices = list(range(90, 100))
-    return MultiTaskBenchmarkSpecification(
+    benchmark = MultiTaskBenchmarkSpecification(
         name="multi-task-benchmark",
         dataset=test_dataset,
         main_metric="mean_absolute_error",
         metrics=[
             "mean_absolute_error",
             "mean_squared_error",
             "r2",
@@ -154,23 +168,27 @@
             "explained_var",
         ],
         split=(train_indices, test_indices),
         target_cols=["expt", "calc"],
         input_cols="smiles",
         target_types={"expt": "regression"},
     )
+    check_version(benchmark)
+    return benchmark
 
 
 @pytest.fixture(scope="function")
 def test_multi_task_benchmark_clf(test_dataset):
     # For the sake of simplicity, just use a small set of indices
     train_indices = list(range(90))
     test_indices = list(range(90, 100))
-    return MultiTaskBenchmarkSpecification(
+    benchmark = MultiTaskBenchmarkSpecification(
         name="multi-task-benchmark",
         dataset=test_dataset,
         main_metric="accuracy",
         metrics=["accuracy", "f1", "roc_auc", "pr_auc", "mcc", "cohen_kappa"],
         split=(train_indices, test_indices),
         target_cols=["CLASS_expt", "CLASS_calc"],
         input_cols="smiles",
     )
+    check_version(benchmark)
+    return benchmark
```

### Comparing `polaris-lib-0.2.5/tests/test_benchmark.py` & `polaris-lib-0.2.6/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/tests/test_curation.py` & `polaris-lib-0.2.6/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/tests/test_dataset.py` & `polaris-lib-0.2.6/tests/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 import pandas as pd
 import pytest
 import zarr
+from datamol.utils import fs
 from pydantic import ValidationError
 
 from polaris.dataset import Dataset, create_dataset_from_file
 from polaris.loader import load_dataset
-from polaris.utils import fs
 from polaris.utils.errors import PolarisChecksumError
 
 
 def _equality_test(dataset_1, dataset_2):
     """
     Utility function.
 
@@ -39,25 +39,26 @@
 def test_load_data(tmp_path, with_slice, with_caching):
     """Test accessing the data, specifically whether pointer columns are properly handled."""
 
     # Dummy data (could e.g. be a 3D structure or Image)
     arr = np.random.random((100, 100))
 
     tmpdir = str(tmp_path)
-    path = fs.join(tmpdir, "data.zarr")
+    zarr_path = fs.join(tmpdir, "data.zarr")
 
-    root = zarr.open(path, "w")
+    root = zarr.open(zarr_path, "w")
     root.array("A", data=arr)
+    zarr.consolidate_metadata(root.store)
 
-    path = f"{path}/A#0:5" if with_slice else f"{path}/A#0"
+    path = "A#0:5" if with_slice else "A#0"
     table = pd.DataFrame({"A": [path]}, index=[0])
-    dataset = Dataset(table=table, annotations={"A": {"is_pointer": True}})
+    dataset = Dataset(table=table, annotations={"A": {"is_pointer": True}}, zarr_root_path=zarr_path)
 
     if with_caching:
-        dataset.cache(tmpdir)
+        dataset.cache(fs.join(tmpdir, "cache"))
 
     data = dataset.get_data(row=0, col="A")
 
     if with_slice:
         assert isinstance(data, tuple)
         assert len(data) == 5
 
@@ -160,12 +161,10 @@
     archive = zarr_archive
 
     original_dataset = create_dataset_from_file(archive, tmpdir.join("original1"))
     cached_dataset = create_dataset_from_file(archive, tmpdir.join("original2"))
     assert original_dataset == cached_dataset
 
     cache_dir = cached_dataset.cache(tmpdir.join("cached").strpath)
-    for i in range(len(cached_dataset)):
-        assert cached_dataset.table.loc[i, "A"].startswith(cache_dir)
-        assert cached_dataset.table.loc[i, "B"].startswith(cache_dir)
+    assert cached_dataset.zarr_root_path.startswith(cache_dir)
 
     assert _equality_test(cached_dataset, original_dataset)
```

### Comparing `polaris-lib-0.2.5/tests/test_evaluate.py` & `polaris-lib-0.2.6/tests/test_evaluate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import os
 
 import numpy as np
 import pandas as pd
 
-from polaris.benchmark import MultiTaskBenchmarkSpecification, SingleTaskBenchmarkSpecification
+import polaris as po
+from polaris.benchmark import (
+    MultiTaskBenchmarkSpecification,
+    SingleTaskBenchmarkSpecification,
+)
 from polaris.evaluate._metric import Metric
 from polaris.evaluate._results import BenchmarkResults
 from polaris.utils.types import HubOwner
 
 
 def test_result_to_json(tmpdir: str, test_user_owner: HubOwner):
     scores = pd.DataFrame(
@@ -32,22 +36,28 @@
         paper_url="https://chemrxiv.org/",
         contributors=["my-user", "other-user"],
     )
 
     path = os.path.join(tmpdir, "result.json")
     result.to_json(path)
     BenchmarkResults.from_json(path)
+    assert po.__version__ == result.polaris_version
 
 
 def test_metrics_singletask_reg(tmpdir: str, test_single_task_benchmark: SingleTaskBenchmarkSpecification):
     _, test = test_single_task_benchmark.get_train_test_split()
     predictions = np.random.random(size=test.inputs.shape[0])
     result = test_single_task_benchmark.evaluate(predictions)
     assert isinstance(result.results, pd.DataFrame)
-    assert set(result.results.columns) == {"Test set", "Target label", "Metric", "Score"}
+    assert set(result.results.columns) == {
+        "Test set",
+        "Target label",
+        "Metric",
+        "Score",
+    }
     for metric in test_single_task_benchmark.metrics:
         assert metric in result.results.Metric.tolist()
 
 
 def test_metrics_multitask_reg(tmpdir: str, test_multi_task_benchmark: MultiTaskBenchmarkSpecification):
     train, test = test_multi_task_benchmark.get_train_test_split()
     predictions = {
@@ -71,15 +81,20 @@
 def test_metrics_multitask_clf(tmpdir: str, test_multi_task_benchmark_clf: MultiTaskBenchmarkSpecification):
     train, test = test_multi_task_benchmark_clf.get_train_test_split()
     predictions = {
         target_col: np.random.randint(2, size=test.inputs.shape[0]) for target_col in train.target_cols
     }
     result = test_multi_task_benchmark_clf.evaluate(predictions)
     assert isinstance(result.results, pd.DataFrame)
-    assert set(result.results.columns) == {"Test set", "Target label", "Metric", "Score"}
+    assert set(result.results.columns) == {
+        "Test set",
+        "Target label",
+        "Metric",
+        "Score",
+    }
     # check the targets and metrics
     assert result.results.shape[0] == len(test_multi_task_benchmark_clf.target_cols) * len(
         test_multi_task_benchmark_clf.metrics
     )
     for metric in test_multi_task_benchmark_clf.metrics:
         assert metric in result.results.Metric.tolist()
```

### Comparing `polaris-lib-0.2.5/tests/test_factory.py` & `polaris-lib-0.2.6/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/tests/test_integration.py` & `polaris-lib-0.2.6/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `polaris-lib-0.2.5/tests/test_subset.py` & `polaris-lib-0.2.6/tests/test_subset.py`

 * *Files identical despite different names*

