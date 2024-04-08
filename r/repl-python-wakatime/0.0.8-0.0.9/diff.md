# Comparing `tmp/repl-python-wakatime-0.0.8.tar.gz` & `tmp/repl-python-wakatime-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repl-python-wakatime-0.0.8.tar", last modified: Wed Nov 29 08:09:40 2023, max compression
+gzip compressed data, was "repl-python-wakatime-0.0.9.tar", last modified: Mon Dec  4 18:18:34 2023, max compression
```

## Comparing `repl-python-wakatime-0.0.8.tar` & `repl-python-wakatime-0.0.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.323078 repl-python-wakatime-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.315078 repl-python-wakatime-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.315078 repl-python-wakatime-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      101 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/.gitlint
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/.yamlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2023-11-29 08:09:40.323078 repl-python-wakatime-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.315078 repl-python-wakatime-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.315078 repl-python-wakatime-0.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/docs/api/python_wakatime.md
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.315078 repl-python-wakatime-0.0.8/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.315078 repl-python-wakatime-0.0.8/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (127)      118 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/requirements/ipython.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      111 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/requirements/keyring.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       54 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/requirements/ptipython.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       43 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/requirements/ptpython.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-29 08:09:40.323078 repl-python-wakatime-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.311078 repl-python-wakatime-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.319078 repl-python-wakatime-0.0.8/src/repl_python_wakatime/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-11-29 08:09:40.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime/_metainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-29 08:09:40.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.319078 repl-python-wakatime-0.0.8/src/repl_python_wakatime/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime/hooks/codestats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime/hooks/wakatime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime/ipython.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime/ptpython.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.319078 repl-python-wakatime-0.0.8/src/repl_python_wakatime/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime/utils/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.319078 repl-python-wakatime-0.0.8/src/repl_python_wakatime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2023-11-29 08:09:40.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-11-29 08:09:40.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 08:09:40.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-11-29 08:09:40.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-29 08:09:40.000000 repl-python-wakatime-0.0.8/src/repl_python_wakatime.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.319078 repl-python-wakatime-0.0.8/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 08:09:40.319078 repl-python-wakatime-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-11-29 08:09:31.000000 repl-python-wakatime-0.0.8/tests/test_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.735042 repl-python-wakatime-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.727042 repl-python-wakatime-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.727042 repl-python-wakatime-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      101 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/.yamlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2023-12-04 18:18:34.735042 repl-python-wakatime-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.727042 repl-python-wakatime-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.727042 repl-python-wakatime-0.0.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/docs/api/python_wakatime.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.727042 repl-python-wakatime-0.0.9/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.731042 repl-python-wakatime-0.0.9/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      118 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/requirements/ipython.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      111 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/requirements/keyring.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       54 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/requirements/ptipython.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       43 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/requirements/ptpython.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-04 18:18:34.735042 repl-python-wakatime-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.723042 repl-python-wakatime-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.731042 repl-python-wakatime-0.0.9/src/repl_python_wakatime/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-04 18:18:34.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-04 18:18:34.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.731042 repl-python-wakatime-0.0.9/src/repl_python_wakatime/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime/hooks/codestats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime/hooks/wakatime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime/ptpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.731042 repl-python-wakatime-0.0.9/src/repl_python_wakatime/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime/utils/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.735042 repl-python-wakatime-0.0.9/src/repl_python_wakatime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2023-12-04 18:18:34.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-04 18:18:34.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 18:18:34.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-04 18:18:34.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-04 18:18:34.000000 repl-python-wakatime-0.0.9/src/repl_python_wakatime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.731042 repl-python-wakatime-0.0.9/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:18:34.735042 repl-python-wakatime-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-04 18:18:22.000000 repl-python-wakatime-0.0.9/tests/test_project.py
```

### Comparing `repl-python-wakatime-0.0.8/.github/workflows/main.yml` & `repl-python-wakatime-0.0.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/.gitignore` & `repl-python-wakatime-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/.pre-commit-config.yaml` & `repl-python-wakatime-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/LICENSE` & `repl-python-wakatime-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/PKG-INFO` & `repl-python-wakatime-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repl-python-wakatime
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python REPL plugin for automatic time tracking and metrics generated from your programming activity
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://repl-python-wakatime.readthedocs.io
 Project-URL: Download, https://github.com/wakatime/repl-python-wakatime/releases
 Project-URL: Bug Report, https://github.com/wakatime/repl-python-wakatime/issues
 Project-URL: Source, https://github.com/wakatime/repl-python-wakatime
@@ -79,14 +79,16 @@
 [![pypi/format](https://shields.io/pypi/format/repl-python-wakatime)](https://pypi.org/project/repl-python-wakatime/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/repl-python-wakatime)](https://pypi.org/project/repl-python-wakatime/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/repl-python-wakatime)](https://pypi.org/project/repl-python-wakatime/#files)
 
 Python REPL plugin for automatic time tracking and metrics generated from your
 programming activity.
 
+![screenshot](https://github.com/wakatime/repl-python-wakatime/assets/32936898/d0ac2fab-f9c2-4213-99e3-4249279b1213)
+
 Supported REPLs:
 
 - [x] [python](https://github.com/python/cpython):
   - executes
     [`str(sys.ps1)`](https://docs.python.org/3/library/sys.html#sys.ps1) after
     every input.
   - configure file:
```

### Comparing `repl-python-wakatime-0.0.8/README.md` & `repl-python-wakatime-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 [![pypi/format](https://shields.io/pypi/format/repl-python-wakatime)](https://pypi.org/project/repl-python-wakatime/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/repl-python-wakatime)](https://pypi.org/project/repl-python-wakatime/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/repl-python-wakatime)](https://pypi.org/project/repl-python-wakatime/#files)
 
 Python REPL plugin for automatic time tracking and metrics generated from your
 programming activity.
 
+![screenshot](https://github.com/wakatime/repl-python-wakatime/assets/32936898/d0ac2fab-f9c2-4213-99e3-4249279b1213)
+
 Supported REPLs:
 
 - [x] [python](https://github.com/python/cpython):
   - executes
     [`str(sys.ps1)`](https://docs.python.org/3/library/sys.html#sys.ps1) after
     every input.
   - configure file:
```

### Comparing `repl-python-wakatime-0.0.8/docs/conf.py` & `repl-python-wakatime-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/docs/resources/install.md` & `repl-python-wakatime-0.0.9/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/pyproject.toml` & `repl-python-wakatime-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/src/repl_python_wakatime/_metainfo.py` & `repl-python-wakatime-0.0.9/src/repl_python_wakatime/_metainfo.py`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/src/repl_python_wakatime/hooks/codestats.py` & `repl-python-wakatime-0.0.9/src/repl_python_wakatime/hooks/codestats.py`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/src/repl_python_wakatime/hooks/wakatime.py` & `repl-python-wakatime-0.0.9/src/repl_python_wakatime/hooks/wakatime.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Wakatime
 ===========
 
 Refer `create-plugin <https://wakatime.com/help/creating-plugin>`_.
 """
 import os
-from subprocess import run  # nosec: B404
-from threading import Thread
+from subprocess import Popen  # nosec: B404
 from typing import Any, Callable
 
 
-def send_wakatime_heartbeat(
+def wakatime_hook(
     project: str = "",
     category: str = "coding",
     plugin: str = "repl-python-wakatime",
     filenames: list[str] = [".git"],
     detect_func: Callable[[str], bool] = os.path.isdir,
     *args: Any,
     **kwargs: Any,
@@ -37,34 +36,19 @@
     :type detect_func: Callable[[str], bool]
     :rtype: None
     """
     if project == "":
         from ..utils.project import get_project
 
         project = get_project(filenames, detect_func)
-    run(  # nosec: B603 B607
+    Popen(  # nosec: B603 B607
         [
             "wakatime-cli",
             "--write",
             f"--category={category}",
             f"--plugin={plugin}",
             "--entity-type=app",
             "--entity=python",
             "--alternate-language=python",
             f"--project={project}",
-        ],
-        stdout=open(os.devnull, "w"),
+        ]
     )
-
-
-def wakatime_hook(*args: Any, **kwargs: Any) -> None:
-    """Wakatime hook.
-
-    :param args:
-    :type args: Any
-    :param kwargs:
-    :type kwargs: Any
-    :rtype: None
-    """
-    task = Thread(target=send_wakatime_heartbeat, args=args, kwargs=kwargs)
-    task.daemon = True
-    task.start()
```

### Comparing `repl-python-wakatime-0.0.8/src/repl_python_wakatime/ipython.py` & `repl-python-wakatime-0.0.9/src/repl_python_wakatime/ipython.py`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/src/repl_python_wakatime/ptpython.py` & `repl-python-wakatime-0.0.9/src/repl_python_wakatime/ptpython.py`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/src/repl_python_wakatime/python.py` & `repl-python-wakatime-0.0.9/src/repl_python_wakatime/python.py`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/src/repl_python_wakatime/utils/api.py` & `repl-python-wakatime-0.0.9/src/repl_python_wakatime/utils/api.py`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/src/repl_python_wakatime/utils/project.py` & `repl-python-wakatime-0.0.9/src/repl_python_wakatime/utils/project.py`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/src/repl_python_wakatime.egg-info/PKG-INFO` & `repl-python-wakatime-0.0.9/src/repl_python_wakatime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repl-python-wakatime
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python REPL plugin for automatic time tracking and metrics generated from your programming activity
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://repl-python-wakatime.readthedocs.io
 Project-URL: Download, https://github.com/wakatime/repl-python-wakatime/releases
 Project-URL: Bug Report, https://github.com/wakatime/repl-python-wakatime/issues
 Project-URL: Source, https://github.com/wakatime/repl-python-wakatime
@@ -79,14 +79,16 @@
 [![pypi/format](https://shields.io/pypi/format/repl-python-wakatime)](https://pypi.org/project/repl-python-wakatime/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/repl-python-wakatime)](https://pypi.org/project/repl-python-wakatime/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/repl-python-wakatime)](https://pypi.org/project/repl-python-wakatime/#files)
 
 Python REPL plugin for automatic time tracking and metrics generated from your
 programming activity.
 
+![screenshot](https://github.com/wakatime/repl-python-wakatime/assets/32936898/d0ac2fab-f9c2-4213-99e3-4249279b1213)
+
 Supported REPLs:
 
 - [x] [python](https://github.com/python/cpython):
   - executes
     [`str(sys.ps1)`](https://docs.python.org/3/library/sys.html#sys.ps1) after
     every input.
   - configure file:
```

### Comparing `repl-python-wakatime-0.0.8/src/repl_python_wakatime.egg-info/SOURCES.txt` & `repl-python-wakatime-0.0.9/src/repl_python_wakatime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/tests/test_api.py` & `repl-python-wakatime-0.0.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `repl-python-wakatime-0.0.8/tests/test_project.py` & `repl-python-wakatime-0.0.9/tests/test_project.py`

 * *Files identical despite different names*

