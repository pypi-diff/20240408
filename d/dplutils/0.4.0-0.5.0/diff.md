# Comparing `tmp/dplutils-0.4.0.tar.gz` & `tmp/dplutils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dplutils-0.4.0.tar", last modified: Thu Mar 21 21:09:19 2024, max compression
+gzip compressed data, was "dplutils-0.5.0.tar", last modified: Mon Apr  8 15:50:44 2024, max compression
```

## Comparing `dplutils-0.4.0.tar` & `dplutils-0.5.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.690928 dplutils-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-21 21:09:03.000000 dplutils-0.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-21 21:09:03.000000 dplutils-0.4.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.678928 dplutils-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-21 21:09:03.000000 dplutils-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.678928 dplutils-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-03-21 21:09:03.000000 dplutils-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-21 21:09:03.000000 dplutils-0.4.0/.github/workflows/dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-21 21:09:03.000000 dplutils-0.4.0/.github/workflows/security.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-03-21 21:09:03.000000 dplutils-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 21:09:03.000000 dplutils-0.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-21 21:09:03.000000 dplutils-0.4.0/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-21 21:09:03.000000 dplutils-0.4.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-21 21:09:03.000000 dplutils-0.4.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-03-21 21:09:03.000000 dplutils-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-21 21:09:03.000000 dplutils-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-03-21 21:09:19.690928 dplutils-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-03-21 21:09:03.000000 dplutils-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.678928 dplutils-0.4.0/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-21 21:09:03.000000 dplutils-0.4.0/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-03-21 21:09:03.000000 dplutils-0.4.0/docker/startray.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.678928 dplutils-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.678928 dplutils-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/_static/.DS_Store
--rwxr-xr-x   0 runner    (1001) docker     (127)    33376 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/_static/SSEC_logo_horiz_blue_1152x263.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    72437 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/_static/SSEC_logo_vert_white_lg_1184x661.png
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.682928 dplutils-0.4.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/api_cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/api_observers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/api_pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/api_streaming.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/execution.rst
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/extending.rst
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/tasks_graphs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-21 21:09:03.000000 dplutils-0.4.0/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.682928 dplutils-0.4.0/dplutils/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-21 21:09:19.000000 dplutils-0.4.0/dplutils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.686928 dplutils-0.4.0/dplutils/observer/
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/observer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/observer/aim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/observer/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/observer/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.686928 dplutils-0.4.0/dplutils/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/pipeline/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/pipeline/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/pipeline/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/pipeline/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/pipeline/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-21 21:09:03.000000 dplutils-0.4.0/dplutils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.690928 dplutils-0.4.0/dplutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-03-21 21:09:19.000000 dplutils-0.4.0/dplutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-21 21:09:19.000000 dplutils-0.4.0/dplutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 21:09:19.000000 dplutils-0.4.0/dplutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 21:09:19.000000 dplutils-0.4.0/dplutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-21 21:09:19.000000 dplutils-0.4.0/dplutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-21 21:09:19.000000 dplutils-0.4.0/dplutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.686928 dplutils-0.4.0/githooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      322 2024-03-21 21:09:03.000000 dplutils-0.4.0/githooks/pre-push
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-21 21:09:03.000000 dplutils-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.686928 dplutils-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-21 21:09:03.000000 dplutils-0.4.0/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-21 21:09:03.000000 dplutils-0.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-21 21:09:03.000000 dplutils-0.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-21 21:09:03.000000 dplutils-0.4.0/requirements/prd.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-21 21:09:03.000000 dplutils-0.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 21:09:19.690928 dplutils-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.686928 dplutils-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.686928 dplutils-0.4.0/tests/observer/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/observer/test_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/observer/test_observer_aim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/observer/test_observer_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/observer/test_observer_ray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:09:19.690928 dplutils-0.4.0/tests/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/pipeline/test_executor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/pipeline/test_pipeline_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/pipeline/test_pipeline_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/pipeline/test_pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/pipeline/test_ray_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/pipeline/test_ray_stream_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/pipeline/test_stream_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/pipeline/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-21 21:09:03.000000 dplutils-0.4.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-21 21:09:03.000000 dplutils-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.608008 dplutils-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-08 15:50:15.000000 dplutils-0.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 15:50:15.000000 dplutils-0.5.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.592008 dplutils-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 15:50:15.000000 dplutils-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.596008 dplutils-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-08 15:50:15.000000 dplutils-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-08 15:50:15.000000 dplutils-0.5.0/.github/workflows/dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-08 15:50:15.000000 dplutils-0.5.0/.github/workflows/security.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-08 15:50:15.000000 dplutils-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 15:50:15.000000 dplutils-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-08 15:50:15.000000 dplutils-0.5.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-08 15:50:15.000000 dplutils-0.5.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 15:50:15.000000 dplutils-0.5.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-08 15:50:15.000000 dplutils-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-08 15:50:15.000000 dplutils-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-08 15:50:44.608008 dplutils-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-08 15:50:15.000000 dplutils-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.596008 dplutils-0.5.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-08 15:50:15.000000 dplutils-0.5.0/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-04-08 15:50:15.000000 dplutils-0.5.0/docker/startray.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.596008 dplutils-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.596008 dplutils-0.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/_static/.DS_Store
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33376 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/_static/SSEC_logo_horiz_blue_1152x263.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72437 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/_static/SSEC_logo_vert_white_lg_1184x661.png
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.600008 dplutils-0.5.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/api_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/api_observers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/api_pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/api_streaming.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/execution.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/tasks_graphs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-08 15:50:15.000000 dplutils-0.5.0/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.600008 dplutils-0.5.0/dplutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 15:50:44.000000 dplutils-0.5.0/dplutils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.600008 dplutils-0.5.0/dplutils/observer/
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/observer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/observer/aim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/observer/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/observer/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.600008 dplutils-0.5.0/dplutils/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/pipeline/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/pipeline/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/pipeline/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13299 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/pipeline/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/pipeline/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 15:50:15.000000 dplutils-0.5.0/dplutils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.604008 dplutils-0.5.0/dplutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-08 15:50:44.000000 dplutils-0.5.0/dplutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-08 15:50:44.000000 dplutils-0.5.0/dplutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:50:44.000000 dplutils-0.5.0/dplutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:50:44.000000 dplutils-0.5.0/dplutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 15:50:44.000000 dplutils-0.5.0/dplutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 15:50:44.000000 dplutils-0.5.0/dplutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.600008 dplutils-0.5.0/githooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      322 2024-04-08 15:50:15.000000 dplutils-0.5.0/githooks/pre-push
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-08 15:50:15.000000 dplutils-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.604008 dplutils-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 15:50:15.000000 dplutils-0.5.0/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 15:50:15.000000 dplutils-0.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 15:50:15.000000 dplutils-0.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 15:50:15.000000 dplutils-0.5.0/requirements/prd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 15:50:15.000000 dplutils-0.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:50:44.608008 dplutils-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.604008 dplutils-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.604008 dplutils-0.5.0/tests/observer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/observer/test_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/observer/test_observer_aim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/observer/test_observer_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/observer/test_observer_ray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:50:44.604008 dplutils-0.5.0/tests/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/pipeline/test_executor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/pipeline/test_pipeline_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/pipeline/test_pipeline_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/pipeline/test_pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/pipeline/test_ray_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/pipeline/test_ray_stream_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/pipeline/test_stream_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/pipeline/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 15:50:15.000000 dplutils-0.5.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-08 15:50:15.000000 dplutils-0.5.0/tox.ini
```

### Comparing `dplutils-0.4.0/.github/workflows/ci.yml` & `dplutils-0.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/.github/workflows/dist.yml` & `dplutils-0.5.0/.github/workflows/dist.yml`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/.github/workflows/security.yml` & `dplutils-0.5.0/.github/workflows/security.yml`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/.gitignore` & `dplutils-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/.readthedocs.yaml` & `dplutils-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/.zenodo.json` & `dplutils-0.5.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/CITATION.cff` & `dplutils-0.5.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/CODE_OF_CONDUCT.md` & `dplutils-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/LICENSE` & `dplutils-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/PKG-INFO` & `dplutils-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dplutils
-Version: 0.4.0
+Version: 0.5.0
 Author-email: Scientifc Software Engineering Center at JHU <ssec@jhu.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Software Engineering Center at JHU
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `dplutils-0.4.0/README.md` & `dplutils-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/docker/Dockerfile` & `dplutils-0.5.0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/docs/Makefile` & `dplutils-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/docs/_static/.DS_Store` & `dplutils-0.5.0/docs/_static/.DS_Store`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/docs/_static/SSEC_logo_horiz_blue_1152x263.png` & `dplutils-0.5.0/docs/_static/SSEC_logo_horiz_blue_1152x263.png`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/docs/_static/SSEC_logo_vert_white_lg_1184x661.png` & `dplutils-0.5.0/docs/_static/SSEC_logo_vert_white_lg_1184x661.png`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/docs/make.bat` & `dplutils-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/docs/source/api_observers.rst` & `dplutils-0.5.0/docs/source/api_observers.rst`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/docs/source/conf.py` & `dplutils-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/docs/source/quickstart.rst` & `dplutils-0.5.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/dplutils/cli.py` & `dplutils-0.5.0/dplutils/cli.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/dplutils/observer/__init__.py` & `dplutils-0.5.0/dplutils/observer/__init__.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/dplutils/observer/aim.py` & `dplutils-0.5.0/dplutils/observer/aim.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/dplutils/observer/mlflow.py` & `dplutils-0.5.0/dplutils/observer/mlflow.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/dplutils/observer/ray.py` & `dplutils-0.5.0/dplutils/observer/ray.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/dplutils/pipeline/executor.py` & `dplutils-0.5.0/dplutils/pipeline/executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import uuid
 import pandas as pd
 import yaml
 from abc import ABC, abstractmethod
 from copy import deepcopy
+from dataclasses import dataclass
 from pathlib import Path
 from typing import Any
 from collections.abc import Iterable
 from dplutils.pipeline.graph import PipelineGraph
 from dplutils.pipeline.utils import dict_from_coord
 
 
+@dataclass
+class OutputBatch:
+    data: pd.DataFrame
+    task: str = None
+
+
 class PipelineExecutor(ABC):
     """Base class for pipeline executors.
 
     This class defines the interface for the execution of a graph of
     :class:`PipelineTask<dplutils.pipeline.task.PipelineTask>` objects.
 
     Subclasses must override the ``execute`` method, which is called by ``run``
@@ -104,15 +111,15 @@
     @property
     def run_id(self) -> str:
         if self._run_id is None:
             self._run_id = str(uuid.uuid1())
         return self._run_id
 
     @abstractmethod
-    def execute(self) -> Iterable[pd.DataFrame]:
+    def execute(self) -> Iterable[OutputBatch]:
         """Execute the task graph in batches.
 
         This method must be overridden by implementations. It should arrange for
         the functions defined in the graph of ``PipelineTask``s to execute with
         provided configuration, passing the upstream task output DataFrame to
         the input of Task ``func``.
 
@@ -120,30 +127,49 @@
         implemented as a dictionary locating task by name in ``self.tasks_idx``.
 
         For example, given a dataframe from the previous task, a call for
         ``task`` would be:
 
             task.func(prev_out_dataframe, **task.resolve_kwargs(self.context))
 
-        The method should return an iterator to the DataFrame batches of the
-        terminal tasks in the graph as they complete.
+        The method should return an iterator to the batches dataframes (stored
+        as :py:meth:`OutputBatch<OutputBatch>`s) of the terminal tasks in the
+        graph as they complete.
         """
         pass
 
-    def run(self) -> Iterable[pd.DataFrame]:
+    def run(self) -> Iterable[OutputBatch]:
         """Validate and run the pipeline.
 
         Calls the ``self.execute`` method, and returns an iterator to batches as
         they complete.
         """
         self.validate()
         self._run_id = None  # force reallocation
         return self.execute()
 
-    def writeto(self, outdir: Path|str) -> None:
+    def writeto(self, outdir: Path|str, partition_by_task: bool|None = None, task_partition_name: str = 'task') -> None:
         """Run pipeline, writing results to parquet table.
 
         args:
             outdir: path to the directory in which to write files
+            partition_by_task: If True, always create a hive-style partition by
+              the output task name in the output directory. If false, never
+              create such a partition. If None (default), create partitions if
+              there are multiple sink tasks, otherwise do not.
+            task_partition_name: name of the hive-style partition for
+              tasks. Default is task, e.g. create paths like
+              ``{outdir}/task={task}/...``
         """
+        if partition_by_task is None:
+            partition_by_task = False if len(self.graph.sink_tasks) == 1 else True
+
+        Path(outdir).mkdir(parents=True, exist_ok=True)
         for c, batch in enumerate(self.run()):
-            batch.to_parquet(Path(outdir) / f'{self.run_id}-{c}.parquet', index=False)
+            if partition_by_task:
+                part_name = batch.task or '__HIVE_DEFAULT_PARTITION__'
+                part_path = Path(outdir) / f'{task_partition_name}={part_name}'
+                part_path.mkdir(exist_ok=True)
+                outfile = part_path / f'{self.run_id}-{c}.parquet'
+            else:
+                outfile = Path(outdir) / f'{self.run_id}-{c}.parquet'
+            batch.data.to_parquet(outfile, index=False)
```

### Comparing `dplutils-0.4.0/dplutils/pipeline/graph.py` & `dplutils-0.5.0/dplutils/pipeline/graph.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/dplutils/pipeline/ray.py` & `dplutils-0.5.0/dplutils/pipeline/ray.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 import numpy as np
 from collections import defaultdict
 from copy import copy
 from dataclasses import dataclass
 from itertools import chain
 from dplutils import observer
-from dplutils.pipeline import PipelineTask, PipelineExecutor
+from dplutils.pipeline import PipelineTask, PipelineExecutor, OutputBatch
 from dplutils.pipeline.stream import StreamingGraphExecutor, StreamBatch
 
 
 def set_run_id(inputs, run_id):
     inputs.rename(columns={'id': 'batch_id'}, inplace=True)
     inputs['run_id'] = run_id
     return inputs
@@ -96,16 +96,17 @@
                 batch_size = None,
                 **ray_args,
             )
         return pipeline
 
     def execute(self):
         pipeline = self.make_pipeline()
+        sink_task_n = self.graph.sink_tasks[0].name  # there can be only one
         for batch in pipeline.iter_batches(batch_size = None, batch_format = 'pandas', prefetch_batches = 0):
-            yield batch
+            yield OutputBatch(batch, task=sink_task_n)
 
 
 def get_stream_wrapper(task: PipelineTask, context: dict):
     obs = observer.get_observer()
     def wrapper(*df_list):
         observer.set_observer(obs)
         task_df = pd.concat(df_list)
@@ -154,37 +155,42 @@
         opportunity to re-evaluate cluster resources in case it has expanded
         since last scheduling loop
       \*args, \*\*kwargs: These are passed to
         :py:class:`StreamingGraphexecutor<dplutils.pipeline.stream.StreamingGraphExecutor>`
     """
     def __init__(self, *args, ray_poll_timeout: int = 20, **kwargs):
         super().__init__(*args, **kwargs)
-        # bootstrap remote tasks at initialization and keep reference - this is
-        # more efficient than doing so for each remote task run due to required
-        # serialization
         self.ray_poll_timeout = ray_poll_timeout
+        self.remote_splitter = ray.remote(stream_split_func)
+        self.sched_resources = defaultdict(float)
+
+    def _setup_remote_tasks(self):
+        # bootstrap remote tasks prior to execution and keep reference - this is
+        # more efficient than doing so for each remote task run due to required
+        # serialization. This should be done just prior to running, as task ray
+        # configuration and resources will be baked into the remote.
         self.remote_task_map = {}
         for name, task in self.graph.task_map.items():
             self.remote_task_map[name] = ray.remote(
                 get_stream_wrapper(task, self.ctx)
             ).options(
                 num_cpus = task.num_cpus,
                 num_gpus = task.num_gpus,
                 resources = task.resources,
                 name = f'{task.name}<{task.func.__name__}>',
                 num_returns = 2,  # the remote wrapper returns (len of df, df)
             )
-        self.remote_splitter = ray.remote(stream_split_func)
-        self.sched_resources = defaultdict(float)
 
     def execute(self):
         if not ray.is_initialized():
             ray.init()
+        self._setup_remote_tasks()
         for batch in super().execute():
-            yield ray.get(batch)
+            batch.data = ray.get(batch.data)
+            yield batch
 
     def task_submittable(self, task, rank):
         cluster_r = ray.cluster_resources()
         ck_map = {'num_cpus': 'CPU', 'num_gpus': 'GPU'}
         task_r = task_resources(task)
         for k in task_r:
             avail = cluster_r.get(ck_map.get(k, k), 0) - self.sched_resources.get(k, 0)
```

### Comparing `dplutils-0.4.0/dplutils/pipeline/stream.py` & `dplutils-0.5.0/dplutils/pipeline/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 import networkx as nx
 from abc import ABC, abstractmethod
 from collections import deque
 from collections.abc import Generator
 from dataclasses import dataclass, field
 from typing import Any, Callable
-from dplutils.pipeline import PipelineTask, PipelineExecutor
+from dplutils.pipeline import PipelineTask, PipelineExecutor, OutputBatch
 from dplutils.pipeline.utils import deque_extract
 
 
 @dataclass
 class StreamBatch:
     """Container for task output tracking
 
@@ -40,15 +40,15 @@
         return hash(self.task)
 
     @property
     def name(self):
         return self.task.name
 
     def total_pending(self):
-        return sum(len(i)  for i in [self.data_in, self.pending, self.split_pending])
+        return sum(len(i) for i in [self.data_in, self.pending, self.split_pending])
 
 
 class StreamingGraphExecutor(PipelineExecutor, ABC):
     """Base class for implementing streaming remote graph execution
 
     This class implements the :meth:`execute` method of
     :class:`PipelineExecutor` and contains logic necessary to schedule tasks,
@@ -115,15 +115,15 @@
         # Walk graph forward to promote completed tasks to next task
         # queue. Dataframes for completed sink tasks are returned here in order
         # to prioritize flushing.
         for task in self.stream_graph.walk_fwd():
             for ready in deque_extract(task.pending, self.is_task_ready):
                 block_info = self.task_resolve_output(ready)
                 if task in self.stream_graph.sink_tasks:
-                    return block_info.data
+                    return OutputBatch(block_info.data, task = task.name)
                 else:
                     for next_task in self.stream_graph.neighbors(task):
                         next_task.data_in.appendleft(block_info)
 
             for ready in deque_extract(task.split_pending, self.is_task_ready):
                 task.data_in.extendleft(self.task_resolve_output(ready))
         return None
```

### Comparing `dplutils-0.4.0/dplutils/pipeline/task.py` & `dplutils-0.5.0/dplutils/pipeline/task.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/dplutils.egg-info/PKG-INFO` & `dplutils-0.5.0/dplutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dplutils
-Version: 0.4.0
+Version: 0.5.0
 Author-email: Scientifc Software Engineering Center at JHU <ssec@jhu.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Software Engineering Center at JHU
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `dplutils-0.4.0/dplutils.egg-info/SOURCES.txt` & `dplutils-0.5.0/dplutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/pyproject.toml` & `dplutils-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/tests/conftest.py` & `dplutils-0.5.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import pytest
 import ray
 from pathlib import Path
-from dplutils.pipeline import PipelineTask, PipelineExecutor, PipelineGraph
+from dplutils.pipeline import PipelineTask, PipelineExecutor, OutputBatch, PipelineGraph
 
 
 DATA_PATH = Path(__file__).parent / "data"
 
 
 @pytest.fixture
 def pipelinestartdf():
@@ -24,15 +24,15 @@
     testfile.write_text('TESTDATA\n')
     return testfile
 
 
 class DummyExecutor(PipelineExecutor):
     def execute(self):
         for i in range(10):
-            yield pd.DataFrame({'id': range(10)})
+            yield OutputBatch(pd.DataFrame({'id': range(10)}), task=self.graph.sink_tasks[0].name)
 
 
 @pytest.fixture
 def dummy_steps():
     return [
         PipelineTask(
             'task1',
@@ -51,14 +51,31 @@
     t2A = PipelineTask('task2A', lambda x: x.assign(t2A = '2A'))
     t2B = PipelineTask('task2B', lambda x: x.assign(t2B = '2B'))
     t3 = PipelineTask('task3', lambda x: x.assign(t3 = '3'))
     return PipelineGraph([(t1, t2A), (t1, t2B), (t2A, t3), (t2B, t3)])
 
 
 @pytest.fixture
+def multi_output_graph():
+    t1 = PipelineTask('task1', lambda x: x.assign(t1 = '1'))
+    t2A = PipelineTask('task2A', lambda x: x.assign(t2A = '2A'))
+    t2B = PipelineTask('task2B', lambda x: x.assign(t2B = '2B'))
+    return PipelineGraph([(t1, t2A), (t1, t2B)])
+
+
+@pytest.fixture
+def graph_suite(dummy_steps, dummy_pipeline_graph, multi_output_graph):
+    return {
+        'dummy_steps': dummy_steps,
+        'dummy_pipeline_graph': dummy_pipeline_graph,
+        'multi_output_graph': multi_output_graph,
+    }
+
+
+@pytest.fixture
 def generic_task():
     def func(dataframe, optional = 1):
         pass
     return PipelineTask('name', func)
 
 
 @pytest.fixture
```

### Comparing `dplutils-0.4.0/tests/observer/test_observer.py` & `dplutils-0.5.0/tests/observer/test_observer.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/tests/observer/test_observer_aim.py` & `dplutils-0.5.0/tests/observer/test_observer_aim.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/tests/observer/test_observer_mlflow.py` & `dplutils-0.5.0/tests/observer/test_observer_mlflow.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/tests/observer/test_observer_ray.py` & `dplutils-0.5.0/tests/observer/test_observer_ray.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/tests/pipeline/test_executor_base.py` & `dplutils-0.5.0/tests/pipeline/test_executor_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,21 +49,24 @@
 def test_pipeline_executor_set_context(dummy_executor):
     ret = dummy_executor.set_context('newcontext', 'somevalue')
     assert ret == dummy_executor
     assert dummy_executor.ctx['newcontext'] == 'somevalue'
 
 
 def test_pipeline_executor_output_writer(dummy_executor, tmp_path):
-    dummy_executor.writeto(tmp_path)
+    dummy_executor.writeto(tmp_path, partition_by_task=False)
     for i in range(10):
         assert (tmp_path / f'{dummy_executor.run_id}-{i}.parquet').is_file()
     data = pd.read_parquet(tmp_path / f'{dummy_executor.run_id}-{i}.parquet')
     # these test the expected data inside each batch, hence len fixed at 10
     assert len(data) == 10
     assert len(data.id) == 10
+    dummy_executor.writeto(tmp_path, partition_by_task=True)
+    for i in range(10):
+        assert (tmp_path / 'task=task2' / f'{dummy_executor.run_id}-{i}.parquet').is_file()
 
 
 def test_pipeline_executor_from_list_graph(dummy_executor, dummy_steps):
     executor_class = dummy_executor.__class__
     obj = executor_class.from_graph(dummy_steps)
     assert isinstance(obj, executor_class)
     assert obj.graph.to_list() == dummy_steps
```

### Comparing `dplutils-0.4.0/tests/pipeline/test_pipeline_graph.py` & `dplutils-0.5.0/tests/pipeline/test_pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/tests/pipeline/test_pipeline_task.py` & `dplutils-0.5.0/tests/pipeline/test_pipeline_task.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/tests/pipeline/test_ray_executor.py` & `dplutils-0.5.0/tests/pipeline/test_ray_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import ray
 import pandas as pd
 import pytest
-from dplutils.pipeline import  PipelineTask
+from ray.exceptions import RayTaskError
+from dplutils.pipeline import  PipelineTask, OutputBatch
 from dplutils.pipeline.ray import RayDataPipelineExecutor, get_remote_wrapper, set_run_id
 from dplutils import observer
 from dplutils.observer.ray import RayActorWrappedObserver, RayMetricsObserver
 
 @pytest.fixture
 def dummy_ray_pipeline(dummy_steps):
     return RayDataPipelineExecutor(dummy_steps, n_batches=10)
@@ -53,35 +54,37 @@
     observer.set_observer(RayMetricsObserver())
     def confused_task(indf):
         observer.observe('gauge', 1)
         observer.increment('counter')
         observer.increment('gauge')
         return indf
     pl = RayDataPipelineExecutor([PipelineTask('task', confused_task)], n_batches=2)
-    with pytest.raises(TypeError):
+    # for ray 2.10+ unfortunately ray data no longer unfolds exception, and
+    # in fact doesn't look like a way to get at it
+    with pytest.raises((TypeError, RayTaskError)):
         for batch in pl.set_config('task.batch_size', task_batch_size).run():
             pass
 
 
 def test_pipeline_create_returns_ray_dataset(dummy_ray_pipeline, raysession):
     pl = dummy_ray_pipeline.make_pipeline()
     assert isinstance(pl, ray.data.Dataset)
 
 
 def test_pipeline_run_dummy_runs_steps_and_generates_outputs(dummy_ray_pipeline, raysession):
     it = dummy_ray_pipeline.run()
-    batch1 = next(it)
+    batch1 = next(it).data
     assert isinstance(batch1, pd.DataFrame)
     assert batch1['run_id'].iloc[0] == dummy_ray_pipeline.run_id
     assert len(batch1) == 10
     # we expect first step to take 1 row, just identifiers, and generate batch of size
     assert batch1['step1'].iloc[0] == 1
     # the other steps should see that batch size
     if dummy_ray_pipeline.n_batches > 1:
-        batch2 = next(it)
+        batch2 = next(it).data
         assert batch1['batch_id'].iloc[0] != batch2['batch_id'].iloc[0]
         assert len(batch2) == 10
         assert batch2['step2'].iloc[0] == 10
 
 
 def test_pipeline_splits_tasks_into_separate_remotes_with_context(raysession, test_file):
     def expand(indf):
@@ -91,26 +94,28 @@
         indf['ctxdata'] = ctxdata.read_text()
         return indf
     it = RayDataPipelineExecutor([
         PipelineTask('in', expand),
         PipelineTask('task', task_func, context_kwargs={'ctxdata': 'testfile'}, batch_size=10)
     ]).set_context('testfile', test_file).run()
     batch = next(it)
-    assert len(set(batch['task_id'])) == 10
-    assert batch['ctxdata'].iloc[0] == 'TESTDATA\n'
+    assert isinstance(batch, OutputBatch)
+    assert batch.task == 'task'
+    assert len(set(batch.data['task_id'])) == 10
+    assert batch.data['ctxdata'].iloc[0] == 'TESTDATA\n'
 
 
 def test_pipeline_non_split_task_has_access_to_context(raysession, test_file):
     def task_func(indf, ctxdata):
         indf['ctxdata'] = ctxdata.read_text()
         return indf
     it = RayDataPipelineExecutor([
         PipelineTask('task', task_func, context_kwargs={'ctxdata': 'testfile'})
     ]).set_context('testfile', test_file).run()
-    batch = next(it)
+    batch = next(it).data
     assert batch['ctxdata'].iloc[0] == 'TESTDATA\n'
 
 
 def test_remote_wrapper_sets_name_based_on_task_info():
     def funcname(): pass
     wrapper = get_remote_wrapper(PipelineTask('taskname', funcname), None)
     assert wrapper.__name__ == 'taskname<funcname>'
```

### Comparing `dplutils-0.4.0/tests/pipeline/test_ray_stream_executor.py` & `dplutils-0.5.0/tests/pipeline/test_ray_stream_executor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import pandas as pd
+import ray
 import dplutils.pipeline.ray
 from dplutils.pipeline import PipelineTask
 from dplutils.pipeline.ray import RayStreamGraphExecutor, get_stream_wrapper, stream_split_func
 from test_suite import PipelineExecutorTestSuite
 
 
 @pytest.fixture(autouse=True)
@@ -46,7 +47,18 @@
     im = raymock()
     monkeypatch.setattr(dplutils.pipeline.ray.ray, 'is_initialized', im.is_initialized)
     monkeypatch.setattr(dplutils.pipeline.ray.ray, 'init', im.init)
     pl = RayStreamGraphExecutor(dummy_steps)
     assert not im.is_initialized()
     next(pl.run())
     assert im.is_initialized()
+
+def test_ray_stream_remote_tasks_configuration_applies():
+    def get_runtime_env(x):
+        ncpu = ray.runtime_context.get_runtime_context().get_assigned_resources()['CPU']
+        return x.assign(ncpu = ncpu)
+
+    pl = RayStreamGraphExecutor([PipelineTask('task', get_runtime_env)], max_batches=1)
+    res_df = next(pl.run()).data
+    assert(res_df.iloc[0].ncpu == 1)
+    res_df = next(pl.set_config('task.num_cpus', 0.1).run()).data
+    assert(res_df.iloc[0].ncpu == 0.1)
```

### Comparing `dplutils-0.4.0/tests/pipeline/test_stream_executor.py` & `dplutils-0.5.0/tests/pipeline/test_stream_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,11 +32,11 @@
 def test_stream_executor_generator_override(max_batches):
     st = PipelineTask('task_name', lambda x: x)
     def generator():
         n = 12
         for i in range(n):
             yield pd.DataFrame({'customgen': [i]})
     pl = LocalSerialExecutor([st], max_batches=max_batches, generator=generator)
-    res = list(pl.run())
+    res = list(i.data for i in pl.run())
     expected_rows = max_batches if max_batches else 12
     assert len(res) == expected_rows
     assert pd.concat(res).customgen.to_list() == list(range(expected_rows))
```

### Comparing `dplutils-0.4.0/tests/test_cli.py` & `dplutils-0.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.4.0/tox.ini` & `dplutils-0.5.0/tox.ini`

 * *Files identical despite different names*

