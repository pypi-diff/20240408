# Comparing `tmp/econpizza-0.6.2.tar.gz` & `tmp/econpizza-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econpizza-0.6.2.tar", last modified: Tue Feb 27 04:29:39 2024, max compression
+gzip compressed data, was "econpizza-0.6.3.tar", last modified: Mon Apr  8 07:11:45 2024, max compression
```

## Comparing `econpizza-0.6.2.tar` & `econpizza-0.6.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.248681 econpizza-0.6.2/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.232014 econpizza-0.6.2/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.235347 econpizza-0.6.2/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1353 2023-07-02 18:00:55.000000 econpizza-0.6.2/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.6.2/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.6.2/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.6.2/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4207 2024-02-27 04:29:39.248681 econpizza-0.6.2/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3549 2023-10-23 07:59:31.000000 econpizza-0.6.2/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.235347 econpizza-0.6.2/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.6.2/docs/Makefile
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.232014 econpizza-0.6.2/docs/_static/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.235347 econpizza-0.6.2/docs/_static/css/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.6.2/docs/_static/css/custom.css
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1551 2023-05-02 19:15:35.000000 econpizza-0.6.2/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.6.2/docs/content.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.238681 econpizza-0.6.2/docs/guide/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      563 2023-06-23 09:43:34.000000 econpizza-0.6.2/docs/guide/installation.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.6.2/docs/guide/method.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2606 2023-05-07 18:36:01.000000 econpizza-0.6.2/docs/guide/solution.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2161 2023-05-07 18:29:06.000000 econpizza-0.6.2/docs/guide/steady_state.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    14328 2023-05-02 15:47:57.000000 econpizza-0.6.2/docs/guide/the_yaml.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2420 2023-05-27 12:18:06.000000 econpizza-0.6.2/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.6.2/docs/lin_and_nlin.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.6.2/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.6.2/docs/p_and_n.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.6.2/docs/requirements.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.238681 econpizza-0.6.2/docs/tutorial/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.6.2/docs/tutorial/boehl_hommes.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389791 2023-06-06 14:13:17.000000 econpizza-0.6.2/docs/tutorial/hank1.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.6.2/docs/tutorial/hank2.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.6.2/docs/tutorial/quickstart.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.6.2/docs/tutorial/rank.ipynb
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.242014 econpizza-0.6.2/econpizza/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3480 2023-08-02 06:34:40.000000 econpizza-0.6.2/econpizza/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2024-02-27 04:22:33.000000 econpizza-0.6.2/econpizza/__version__.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.245347 econpizza-0.6.2/econpizza/examples/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.6.2/econpizza/examples/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-09-21 16:44:29.000000 econpizza-0.6.2/econpizza/examples/bh.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7086 2023-05-27 12:24:35.000000 econpizza-0.6.2/econpizza/examples/dsge.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.6.2/econpizza/examples/ghls.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.6.2/econpizza/examples/hank2.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.6.2/econpizza/examples/hank2_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.6.2/econpizza/examples/hank2_no_capital.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-05-13 03:15:20.000000 econpizza-0.6.2/econpizza/examples/hank_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3777 2023-06-27 10:04:44.000000 econpizza-0.6.2/econpizza/examples/hank_labor.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.6.2/econpizza/examples/hank_labor_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6233 2023-06-27 10:04:44.000000 econpizza-0.6.2/econpizza/examples/hank_with_comments.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.6.2/econpizza/examples/nk.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.6.2/econpizza/examples/tank.yml
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.245347 econpizza-0.6.2/econpizza/parser/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12390 2023-12-21 19:00:46.000000 econpizza-0.6.2/econpizza/parser/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-09-27 16:56:21.000000 econpizza-0.6.2/econpizza/parser/build_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-04-21 09:07:56.000000 econpizza-0.6.2/econpizza/parser/checks.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.6.2/econpizza/parser/het_agent_base_funcs.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4337 2023-05-12 08:16:06.000000 econpizza-0.6.2/econpizza/parser/write_dynamic_functions.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.245347 econpizza-0.6.2/econpizza/solvers/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.6.2/econpizza/solvers/shooting.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2726 2023-08-02 06:35:28.000000 econpizza-0.6.2/econpizza/solvers/solve_linear.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4823 2023-08-02 06:36:50.000000 econpizza-0.6.2/econpizza/solvers/solve_linear_state_space.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6205 2023-09-27 16:56:21.000000 econpizza-0.6.2/econpizza/solvers/stacking.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8472 2023-08-02 06:32:02.000000 econpizza-0.6.2/econpizza/solvers/steady_state.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.245347 econpizza-0.6.2/econpizza/testing/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.248681 econpizza-0.6.2/econpizza/testing/cache/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.6.2/econpizza/testing/cache/bh.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7472 2023-06-27 10:04:44.000000 econpizza-0.6.2/econpizza/testing/cache/hank_labor.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3152 2023-06-27 10:04:44.000000 econpizza-0.6.2/econpizza/testing/cache/hank_solid.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:35:27.000000 econpizza-0.6.2/econpizza/testing/test_nb_hank1.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:44:49.000000 econpizza-0.6.2/econpizza/testing/test_nb_hank2.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.6.2/econpizza/testing/test_nb_quickstart.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.6.2/econpizza/testing/test_nb_rank.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.6.2/econpizza/testing/test_nb_under_the_hood.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1883 2023-05-10 08:08:46.000000 econpizza-0.6.2/econpizza/testing/test_rest.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.6.2/econpizza/tools.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.248681 econpizza-0.6.2/econpizza/utilities/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-09-27 16:54:08.000000 econpizza-0.6.2/econpizza/utilities/dists.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-04-27 11:18:13.000000 econpizza-0.6.2/econpizza/utilities/grids.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4769 2023-05-04 15:35:28.000000 econpizza-0.6.2/econpizza/utilities/interp.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-09-27 16:56:21.000000 econpizza-0.6.2/econpizza/utilities/jacobian.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6395 2023-09-27 16:56:21.000000 econpizza-0.6.2/econpizza/utilities/newton.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-02-27 04:29:39.248681 econpizza-0.6.2/econpizza.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4207 2024-02-27 04:29:39.000000 econpizza-0.6.2/econpizza.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2024-02-27 04:29:39.000000 econpizza-0.6.2/econpizza.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2024-02-27 04:29:39.000000 econpizza-0.6.2/econpizza.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       81 2024-02-27 04:29:39.000000 econpizza-0.6.2/econpizza.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2024-02-27 04:29:39.000000 econpizza-0.6.2/econpizza.egg-info/top_level.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      163 2023-10-23 08:58:33.000000 econpizza-0.6.2/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2024-02-27 04:29:39.248681 econpizza-0.6.2/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1334 2023-10-23 08:58:24.000000 econpizza-0.6.2/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.646492 econpizza-0.6.3/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.496492 econpizza-0.6.3/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.506492 econpizza-0.6.3/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1353 2023-07-02 18:00:55.000000 econpizza-0.6.3/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.6.3/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.6.3/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.6.3/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4207 2024-04-08 07:11:45.643159 econpizza-0.6.3/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3549 2023-10-23 07:59:31.000000 econpizza-0.6.3/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.519825 econpizza-0.6.3/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.6.3/docs/Makefile
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.496492 econpizza-0.6.3/docs/_static/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.519825 econpizza-0.6.3/docs/_static/css/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.6.3/docs/_static/css/custom.css
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1551 2023-05-02 19:15:35.000000 econpizza-0.6.3/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.6.3/docs/content.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.526492 econpizza-0.6.3/docs/guide/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      563 2023-06-23 09:43:34.000000 econpizza-0.6.3/docs/guide/installation.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.6.3/docs/guide/method.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2606 2023-05-07 18:36:01.000000 econpizza-0.6.3/docs/guide/solution.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2161 2023-05-07 18:29:06.000000 econpizza-0.6.3/docs/guide/steady_state.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    14534 2024-03-15 13:07:14.000000 econpizza-0.6.3/docs/guide/the_yaml.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2420 2023-05-27 12:18:06.000000 econpizza-0.6.3/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.6.3/docs/lin_and_nlin.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.6.3/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.6.3/docs/p_and_n.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.6.3/docs/requirements.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.566492 econpizza-0.6.3/docs/tutorial/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.6.3/docs/tutorial/boehl_hommes.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389791 2023-06-06 14:13:17.000000 econpizza-0.6.3/docs/tutorial/hank1.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.6.3/docs/tutorial/hank2.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63738 2024-03-15 13:03:36.000000 econpizza-0.6.3/docs/tutorial/quickstart.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407386 2024-03-15 13:04:32.000000 econpizza-0.6.3/docs/tutorial/rank.ipynb
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.579825 econpizza-0.6.3/econpizza/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3480 2023-08-02 06:34:40.000000 econpizza-0.6.3/econpizza/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2024-04-08 07:11:27.000000 econpizza-0.6.3/econpizza/__version__.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.609825 econpizza-0.6.3/econpizza/examples/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.6.3/econpizza/examples/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-09-21 16:44:29.000000 econpizza-0.6.3/econpizza/examples/bh.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7086 2023-05-27 12:24:35.000000 econpizza-0.6.3/econpizza/examples/dsge.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.6.3/econpizza/examples/ghls.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8708 2024-03-20 09:49:14.000000 econpizza-0.6.3/econpizza/examples/hank2.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.6.3/econpizza/examples/hank2_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.6.3/econpizza/examples/hank2_no_capital.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-05-13 03:15:20.000000 econpizza-0.6.3/econpizza/examples/hank_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3777 2023-06-27 10:04:44.000000 econpizza-0.6.3/econpizza/examples/hank_labor.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.6.3/econpizza/examples/hank_labor_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6233 2023-06-27 10:04:44.000000 econpizza-0.6.3/econpizza/examples/hank_with_comments.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.6.3/econpizza/examples/nk.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.6.3/econpizza/examples/tank.yml
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.616492 econpizza-0.6.3/econpizza/parser/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12395 2024-04-08 07:06:16.000000 econpizza-0.6.3/econpizza/parser/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-09-27 16:56:21.000000 econpizza-0.6.3/econpizza/parser/build_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-04-21 09:07:56.000000 econpizza-0.6.3/econpizza/parser/checks.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.6.3/econpizza/parser/het_agent_base_funcs.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4337 2023-05-12 08:16:06.000000 econpizza-0.6.3/econpizza/parser/write_dynamic_functions.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.623159 econpizza-0.6.3/econpizza/solvers/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.6.3/econpizza/solvers/shooting.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2726 2023-08-02 06:35:28.000000 econpizza-0.6.3/econpizza/solvers/solve_linear.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4823 2023-08-02 06:36:50.000000 econpizza-0.6.3/econpizza/solvers/solve_linear_state_space.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6205 2023-09-27 16:56:21.000000 econpizza-0.6.3/econpizza/solvers/stacking.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8472 2023-08-02 06:32:02.000000 econpizza-0.6.3/econpizza/solvers/steady_state.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.629826 econpizza-0.6.3/econpizza/testing/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.633159 econpizza-0.6.3/econpizza/testing/cache/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.6.3/econpizza/testing/cache/bh.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7472 2023-06-27 10:04:44.000000 econpizza-0.6.3/econpizza/testing/cache/hank_labor.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3152 2023-06-27 10:04:44.000000 econpizza-0.6.3/econpizza/testing/cache/hank_solid.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:35:27.000000 econpizza-0.6.3/econpizza/testing/test_nb_hank1.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:44:49.000000 econpizza-0.6.3/econpizza/testing/test_nb_hank2.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.6.3/econpizza/testing/test_nb_quickstart.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.6.3/econpizza/testing/test_nb_rank.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.6.3/econpizza/testing/test_nb_under_the_hood.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1883 2023-05-10 08:08:46.000000 econpizza-0.6.3/econpizza/testing/test_rest.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.6.3/econpizza/tools.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.639826 econpizza-0.6.3/econpizza/utilities/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-09-27 16:54:08.000000 econpizza-0.6.3/econpizza/utilities/dists.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-04-27 11:18:13.000000 econpizza-0.6.3/econpizza/utilities/grids.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4769 2023-05-04 15:35:28.000000 econpizza-0.6.3/econpizza/utilities/interp.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-09-27 16:56:21.000000 econpizza-0.6.3/econpizza/utilities/jacobian.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6395 2023-09-27 16:56:21.000000 econpizza-0.6.3/econpizza/utilities/newton.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2024-04-08 07:11:45.639826 econpizza-0.6.3/econpizza.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4207 2024-04-08 07:11:44.000000 econpizza-0.6.3/econpizza.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2024-04-08 07:11:45.000000 econpizza-0.6.3/econpizza.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2024-04-08 07:11:44.000000 econpizza-0.6.3/econpizza.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       81 2024-04-08 07:11:44.000000 econpizza-0.6.3/econpizza.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2024-04-08 07:11:44.000000 econpizza-0.6.3/econpizza.egg-info/top_level.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      163 2023-10-23 08:58:33.000000 econpizza-0.6.3/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2024-04-08 07:11:45.646492 econpizza-0.6.3/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1334 2023-10-23 08:58:24.000000 econpizza-0.6.3/setup.py
```

### Comparing `econpizza-0.6.2/.github/workflows/continuous-integration.yml` & `econpizza-0.6.3/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/.readthedocs.yaml` & `econpizza-0.6.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/LICENSE` & `econpizza-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/PKG-INFO` & `econpizza-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.6.2
+Version: 0.6.3
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `econpizza-0.6.2/README.rst` & `econpizza-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/Makefile` & `econpizza-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/conf.py` & `econpizza-0.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/guide/installation.rst` & `econpizza-0.6.3/docs/guide/installation.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/guide/method.ipynb` & `econpizza-0.6.3/docs/guide/method.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/guide/solution.rst` & `econpizza-0.6.3/docs/guide/solution.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/guide/steady_state.rst` & `econpizza-0.6.3/docs/guide/steady_state.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/guide/the_yaml.rst` & `econpizza-0.6.3/docs/guide/the_yaml.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 1. list all variables, parameters and shocks
 2. provide the nonlinear equations. Note that each equation starts with a ``~``.
 3. define the values of the parameters and fixed steady state values in the ``steady_state`` section
 4. optionally provide auxiliary equations that are not directly part of the nonlinear system
 5. optionally provide initial guesses for all other steady state values and parameters
 
-I will first briefly discuss the YAML of the small scale *representative* agents NK model `from the quickstart tutorial <../tutorial/quickstart.ipynb>`_ and then turn to a more complex HANK model.
+I will first briefly discuss `the YAML <https://github.com/gboehl/econpizza/blob/master/econpizza/examples/nk.yml>`_ of the small scale *representative* agents NK model `from the quickstart tutorial <../tutorial/quickstart.ipynb>`_ and then turn to a more complex HANK model.
+A collection of examples is provided `with the package <https://github.com/gboehl/econpizza/tree/master/econpizza/examples>`_.
 
 YAML: representative agent models
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The GitHub version of the YAML file for the small scale NK model can be found `here <https://github.com/gboehl/econpizza/blob/master/econpizza/examples/nk.yml>`_. The first block (``variables`` and ``shocks``) is self explanatory:
 
 .. code-block:: yaml
```

### Comparing `econpizza-0.6.2/docs/index.rst` & `econpizza-0.6.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/lin_and_nlin.png` & `econpizza-0.6.3/docs/lin_and_nlin.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/make.bat` & `econpizza-0.6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/p_and_n.png` & `econpizza-0.6.3/docs/p_and_n.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/tutorial/boehl_hommes.rst` & `econpizza-0.6.3/docs/tutorial/boehl_hommes.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/tutorial/hank1.ipynb` & `econpizza-0.6.3/docs/tutorial/hank1.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/tutorial/hank2.ipynb` & `econpizza-0.6.3/docs/tutorial/hank2.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/docs/tutorial/quickstart.ipynb` & `econpizza-0.6.3/docs/tutorial/quickstart.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8716179653679654%*

 * *Differences: {"'cells'": "{1: {'source': ['Take a small-scale nonlinear New Keynesian model with ZLB as a "*

 * *            'starting point, which is provided as an example [(find the yaml file '*

 * *            'here)](https://github.com/gboehl/econpizza/blob/master/econpizza/examples/nk.yml). '*

 * *            'Here is how to simulate it and plot nonlinear impulse responses. Start with some misc '*

 * *            "imports and load the package:']}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.7'}}",*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -7,15 +7,15 @@
                 "# Quickstart"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Take a small-scale nonlinear New Keynesian model with ZLB as a starting point, which is provided [as an example](https://github.com/gboehl/econpizza/blob/master/econpizza/examples/nk.yml). Here is how to simulate it and plot nonlinear impulse responses. Start with some misc imports and load the package:"
+                "Take a small-scale nonlinear New Keynesian model with ZLB as a starting point, which is provided as an example [(find the yaml file here)](https://github.com/gboehl/econpizza/blob/master/econpizza/examples/nk.yml). Here is how to simulate it and plot nonlinear impulse responses. Start with some misc imports and load the package:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
@@ -220,13 +220,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.11.7"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `econpizza-0.6.2/docs/tutorial/rank.ipynb` & `econpizza-0.6.3/docs/tutorial/rank.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8728174603174603%*

 * *Differences: {"'cells'": "{1: {'source': ['Let us dive a bit deeper into the functionalities of the package by "*

 * *            'looking at a nonlinear medium scale DSGE model in the style of Smets & Wouters '*

 * *            '(2003,2007). The model features Rothemberg instead of Calvo pricing, the zero-lower '*

 * *            'bound on the nominal interest rate, and downwards nominal wage rigidity. The full '*

 * *            'model specification can be found in the appendix of the [original '*

 * *            'paper](https://gregorboehl.c […]*

```diff
@@ -7,15 +7,15 @@
                 "# RANK Tutorial"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Let us dive a bit deeper into the functionalities of the package by looking at a nonlinear medium scale DSGE model in the style of Smets & Wouters (2003,2007). The model features Rothemberg instead of Calvo pricing, the zero-lower bound on the nominal interest rate, and downwards nominal wage rigidity. The full model specification can be found in the appendix of the [original paper](https://gregorboehl.com/live/hank_speed_boehl.pdf)."
+                "Let us dive a bit deeper into the functionalities of the package by looking at a nonlinear medium scale DSGE model in the style of Smets & Wouters (2003,2007). The model features Rothemberg instead of Calvo pricing, the zero-lower bound on the nominal interest rate, and downwards nominal wage rigidity. The full model specification can be found in the appendix of the [original paper](https://gregorboehl.com/live/hank_speed_boehl.pdf), whereas the [yaml file can be found here](https://github.com/gboehl/econpizza/blob/master/econpizza/examples/dsge.yml)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Start with some misc imports and load the package. The rest of these tutorials rely on the ``grgrlib`` for plotting, which can be installed via the official repositories (\"``pip install grgrlib``\")."
@@ -503,13 +503,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.11.7"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `econpizza-0.6.2/econpizza/__init__.py` & `econpizza-0.6.3/econpizza/__init__.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/examples/bh.yml` & `econpizza-0.6.3/econpizza/examples/bh.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/examples/dsge.yml` & `econpizza-0.6.3/econpizza/examples/dsge.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/examples/ghls.yml` & `econpizza-0.6.3/econpizza/examples/ghls.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/examples/hank2.yml` & `econpizza-0.6.3/econpizza/examples/hank2.yml`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         sigma_c: 2. # intertemporal elasticity of substitution
         sigma_l: 2.9 # inverse Frisch elasticity of labour supply
         chi: .5 # utility weight of labor disutility
         theta: 6. # elasticity of substitution final good
         theta_w: 11. # elasticity of substitution wages
         delta: 0.025 # depreciation rate
         psi_p: 60. # parameter on the costs of price adjustment
-        psi_w: 96. # parameter on the costs of price adjustment
+        psi_w: 96. # parameter on the costs of wage adjustment
         psi_i: 5.6 # parameter on the costs of investment adjustment
         psi_u: 0.8 # parameter on the capital utilisation costs
         psi_a0: 0.25 # parameter on portfolio adjustment no.1
         psi_a1: 15 # parameter on portfolio adjustment no.2
         psi_a2: 2 # parameter on portfolio adjustment no.3
         zeta: 0.005 # liquidity premium
         phi_pi: 1.5 # Taylor rule coefficient on inflation
```

### Comparing `econpizza-0.6.2/econpizza/examples/hank2_functions.py` & `econpizza-0.6.3/econpizza/examples/hank2_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/examples/hank2_no_capital.yml` & `econpizza-0.6.3/econpizza/examples/hank2_no_capital.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/examples/hank_functions.py` & `econpizza-0.6.3/econpizza/examples/hank_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/examples/hank_labor.yml` & `econpizza-0.6.3/econpizza/examples/hank_labor.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/examples/hank_labor_functions.py` & `econpizza-0.6.3/econpizza/examples/hank_labor_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/examples/hank_with_comments.yml` & `econpizza-0.6.3/econpizza/examples/hank_with_comments.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/examples/nk.yml` & `econpizza-0.6.3/econpizza/examples/nk.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/examples/tank.yml` & `econpizza-0.6.3/econpizza/examples/tank.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/parser/__init__.py` & `econpizza-0.6.3/econpizza/parser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 
 def _eval_strs(vdict, context={}):
     """Evaluate a dictionary of strings into a given context
     """
 
     if vdict is None:
-        return None
+        return None, context
     else:
         vdict = vdict.copy()
     context = context.copy()
 
     for v in vdict:
         if isinstance(vdict[v], str):
             context[v] = eval(vdict[v], context)
@@ -144,15 +144,15 @@
     """
 
     try:
         # load as a module
         module = _load_as_module(model["functions_file"])
 
         def func_or_compiled(func): return isinstance(
-            func, jaxlib.xla_extension.CompiledFunction) or isfunction(func)
+            func, jaxlib.xla_extension.PjitFunction) or isfunction(func)
         for m in getmembers(module, func_or_compiled):
             context[m[0]] = m[1]
 
     except KeyError:
         pass
 
     return False
```

### Comparing `econpizza-0.6.2/econpizza/parser/build_functions.py` & `econpizza-0.6.3/econpizza/parser/build_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/parser/checks.py` & `econpizza-0.6.3/econpizza/parser/checks.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/parser/het_agent_base_funcs.py` & `econpizza-0.6.3/econpizza/parser/het_agent_base_funcs.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/parser/write_dynamic_functions.py` & `econpizza-0.6.3/econpizza/parser/write_dynamic_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/solvers/shooting.py` & `econpizza-0.6.3/econpizza/solvers/shooting.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/solvers/solve_linear.py` & `econpizza-0.6.3/econpizza/solvers/solve_linear.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/solvers/solve_linear_state_space.py` & `econpizza-0.6.3/econpizza/solvers/solve_linear_state_space.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/solvers/stacking.py` & `econpizza-0.6.3/econpizza/solvers/stacking.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/solvers/steady_state.py` & `econpizza-0.6.3/econpizza/solvers/steady_state.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/testing/cache/bh.npy` & `econpizza-0.6.3/econpizza/testing/cache/bh.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/testing/cache/hank_labor.npy` & `econpizza-0.6.3/econpizza/testing/cache/hank_labor.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/testing/cache/hank_solid.npy` & `econpizza-0.6.3/econpizza/testing/cache/hank_solid.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/testing/test_rest.py` & `econpizza-0.6.3/econpizza/testing/test_rest.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/tools.py` & `econpizza-0.6.3/econpizza/tools.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/utilities/dists.py` & `econpizza-0.6.3/econpizza/utilities/dists.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/utilities/grids.py` & `econpizza-0.6.3/econpizza/utilities/grids.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/utilities/interp.py` & `econpizza-0.6.3/econpizza/utilities/interp.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/utilities/jacobian.py` & `econpizza-0.6.3/econpizza/utilities/jacobian.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza/utilities/newton.py` & `econpizza-0.6.3/econpizza/utilities/newton.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/econpizza.egg-info/PKG-INFO` & `econpizza-0.6.3/econpizza.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.6.2
+Version: 0.6.3
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `econpizza-0.6.2/econpizza.egg-info/SOURCES.txt` & `econpizza-0.6.3/econpizza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.2/setup.py` & `econpizza-0.6.3/setup.py`

 * *Files identical despite different names*

