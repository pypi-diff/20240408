# Comparing `tmp/anesthetic-2.8.3.tar.gz` & `tmp/anesthetic-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anesthetic-2.8.3.tar", last modified: Sun Mar 17 20:27:02 2024, max compression
+gzip compressed data, was "anesthetic-2.8.4.tar", last modified: Mon Apr  8 19:51:53 2024, max compression
```

## Comparing `anesthetic-2.8.3.tar` & `anesthetic-2.8.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:27:02.403535 anesthetic-2.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-17 20:26:58.000000 anesthetic-2.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-03-17 20:27:02.403535 anesthetic-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-03-17 20:26:58.000000 anesthetic-2.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:27:02.395535 anesthetic-2.8.3/anesthetic/
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/_code_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/_format.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:27:02.399535 anesthetic-2.8.3/anesthetic/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/examples/_matplotlib_agg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/examples/perfect_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:27:02.399535 anesthetic-2.8.3/anesthetic/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/gui/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/gui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    58348 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:27:02.399535 anesthetic-2.8.3/anesthetic/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/plotting/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:27:02.399535 anesthetic-2.8.3/anesthetic/plotting/_matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/plotting/_matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/plotting/_matplotlib/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/plotting/_matplotlib/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/plotting/_matplotlib/hist.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/plotting/_matplotlib/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:27:02.399535 anesthetic-2.8.3/anesthetic/read/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/read/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/read/cobaya.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/read/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/read/getdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/read/hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/read/multinest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/read/nestedfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/read/polychord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/read/ultranest.py
--rw-r--r--   0 runner    (1001) docker     (127)    53434 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/weighted_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-03-17 20:26:58.000000 anesthetic-2.8.3/anesthetic/weighted_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:27:02.403535 anesthetic-2.8.3/anesthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-03-17 20:27:02.000000 anesthetic-2.8.3/anesthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-17 20:27:02.000000 anesthetic-2.8.3/anesthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 20:27:02.000000 anesthetic-2.8.3/anesthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-17 20:27:02.000000 anesthetic-2.8.3/anesthetic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-17 20:27:02.000000 anesthetic-2.8.3/anesthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-17 20:27:02.000000 anesthetic-2.8.3/anesthetic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-17 20:26:58.000000 anesthetic-2.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-17 20:27:02.403535 anesthetic-2.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:27:02.403535 anesthetic-2.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-17 20:26:58.000000 anesthetic-2.8.3/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-03-17 20:26:58.000000 anesthetic-2.8.3/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-17 20:26:58.000000 anesthetic-2.8.3/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    19493 2024-03-17 20:26:58.000000 anesthetic-2.8.3/tests/test_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    35940 2024-03-17 20:26:58.000000 anesthetic-2.8.3/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-03-17 20:26:58.000000 anesthetic-2.8.3/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    72706 2024-03-17 20:26:58.000000 anesthetic-2.8.3/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-17 20:26:58.000000 anesthetic-2.8.3/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-03-17 20:26:58.000000 anesthetic-2.8.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-17 20:26:58.000000 anesthetic-2.8.3/tests/test_weighted_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-03-17 20:26:58.000000 anesthetic-2.8.3/tests/test_weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:51:53.328245 anesthetic-2.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 19:51:49.000000 anesthetic-2.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-08 19:51:53.328245 anesthetic-2.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-08 19:51:49.000000 anesthetic-2.8.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:51:53.320245 anesthetic-2.8.4/anesthetic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/_code_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:51:53.320245 anesthetic-2.8.4/anesthetic/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/examples/_matplotlib_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/examples/perfect_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:51:53.320245 anesthetic-2.8.4/anesthetic/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/gui/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/gui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:51:53.320245 anesthetic-2.8.4/anesthetic/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/plotting/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:51:53.320245 anesthetic-2.8.4/anesthetic/plotting/_matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/plotting/_matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/plotting/_matplotlib/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/plotting/_matplotlib/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/plotting/_matplotlib/hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/plotting/_matplotlib/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:51:53.324245 anesthetic-2.8.4/anesthetic/read/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/read/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/read/cobaya.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/read/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/read/getdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/read/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/read/multinest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/read/nestedfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/read/polychord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/read/ultranest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53464 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/weighted_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-04-08 19:51:49.000000 anesthetic-2.8.4/anesthetic/weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:51:53.324245 anesthetic-2.8.4/anesthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-08 19:51:53.000000 anesthetic-2.8.4/anesthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-08 19:51:53.000000 anesthetic-2.8.4/anesthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:51:53.000000 anesthetic-2.8.4/anesthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 19:51:53.000000 anesthetic-2.8.4/anesthetic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 19:51:53.000000 anesthetic-2.8.4/anesthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 19:51:53.000000 anesthetic-2.8.4/anesthetic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-08 19:51:49.000000 anesthetic-2.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 19:51:53.328245 anesthetic-2.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:51:53.324245 anesthetic-2.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-08 19:51:49.000000 anesthetic-2.8.4/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-08 19:51:49.000000 anesthetic-2.8.4/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-08 19:51:49.000000 anesthetic-2.8.4/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19493 2024-04-08 19:51:49.000000 anesthetic-2.8.4/tests/test_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35940 2024-04-08 19:51:49.000000 anesthetic-2.8.4/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-04-08 19:51:49.000000 anesthetic-2.8.4/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73424 2024-04-08 19:51:49.000000 anesthetic-2.8.4/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-08 19:51:49.000000 anesthetic-2.8.4/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-08 19:51:49.000000 anesthetic-2.8.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-08 19:51:49.000000 anesthetic-2.8.4/tests/test_weighted_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-08 19:51:49.000000 anesthetic-2.8.4/tests/test_weighted_pandas.py
```

### Comparing `anesthetic-2.8.3/LICENSE` & `anesthetic-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/PKG-INFO` & `anesthetic-2.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.8.3
+Version: 2.8.4
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Deborah Odunuyi <debbieodunuyi@gmail.com>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>, Dily Ong <dlo26@cam.ac.uk>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -80,15 +80,15 @@
 Requires-Dist: getdist; extra == "all"
 Requires-Dist: tables; extra == "all"
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.8.3
+:Version: 2.8.4
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.8.3/README.rst` & `anesthetic-2.8.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.8.3
+:Version: 2.8.4
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.8.3/anesthetic/__init__.py` & `anesthetic-2.8.4/anesthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/_code_utils.py` & `anesthetic-2.8.4/anesthetic/_code_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/_format.py` & `anesthetic-2.8.4/anesthetic/_format.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/boundary.py` & `anesthetic-2.8.4/anesthetic/boundary.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/convert.py` & `anesthetic-2.8.4/anesthetic/convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/examples/perfect_ns.py` & `anesthetic-2.8.4/anesthetic/examples/perfect_ns.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/examples/utils.py` & `anesthetic-2.8.4/anesthetic/examples/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/gui/plot.py` & `anesthetic-2.8.4/anesthetic/gui/plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/gui/widgets.py` & `anesthetic-2.8.4/anesthetic/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/kde.py` & `anesthetic-2.8.4/anesthetic/kde.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/labelled_pandas.py` & `anesthetic-2.8.4/anesthetic/labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/plot.py` & `anesthetic-2.8.4/anesthetic/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import matplotlib.pyplot as plt
 from scipy.stats import gaussian_kde
 from scipy.special import erf
 from matplotlib.gridspec import GridSpec, GridSpecFromSubplotSpec
 from matplotlib.axes import Axes
 import matplotlib.cbook as cbook
 import matplotlib.lines as mlines
-from matplotlib.ticker import MaxNLocator, AutoMinorLocator
+from matplotlib.ticker import MaxNLocator, AutoMinorLocator, LogLocator
 from matplotlib.colors import LinearSegmentedColormap
 from matplotlib.transforms import Affine2D
 from anesthetic.utils import nest_level
 from anesthetic.utils import (sample_compression_1d, quantile,
                               triangular_sample_compression_2d,
                               iso_probability_contours,
                               match_contour_to_contourf, histogram_bin_edges)
@@ -384,14 +384,23 @@
             for x, ax in rows.items():
                 if ax is not None:
                     if x in self._logx:
                         ax.set_xscale('log')
                     if y in self._logy:
                         ax.set_yscale('log')
 
+    def _set_logticks(self):
+        for y, rows in self.iterrows():
+            for x, ax in rows.items():
+                if ax is not None:
+                    if x in self._logx:
+                        ax.xaxis.set_major_locator(LogLocator(numticks=3))
+                    if y in self._logy:
+                        ax.yaxis.set_major_locator(LogLocator(numticks=3))
+
     @staticmethod
     def _set_labels(axes, labels, **kwargs):
         all_params = list(axes.columns) + list(axes.index)
         if labels is None:
             labels = {}
         labels = {p: labels[p] if p in labels else p for p in all_params}
```

### Comparing `anesthetic-2.8.3/anesthetic/plotting/_core.py` & `anesthetic-2.8.4/anesthetic/plotting/_core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/plotting/_matplotlib/__init__.py` & `anesthetic-2.8.4/anesthetic/plotting/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/plotting/_matplotlib/boxplot.py` & `anesthetic-2.8.4/anesthetic/plotting/_matplotlib/boxplot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/plotting/_matplotlib/core.py` & `anesthetic-2.8.4/anesthetic/plotting/_matplotlib/core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/plotting/_matplotlib/hist.py` & `anesthetic-2.8.4/anesthetic/plotting/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/read/chain.py` & `anesthetic-2.8.4/anesthetic/read/chain.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/read/cobaya.py` & `anesthetic-2.8.4/anesthetic/read/cobaya.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/read/csv.py` & `anesthetic-2.8.4/anesthetic/read/csv.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/read/getdist.py` & `anesthetic-2.8.4/anesthetic/read/getdist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/read/hdf.py` & `anesthetic-2.8.4/anesthetic/read/hdf.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/read/multinest.py` & `anesthetic-2.8.4/anesthetic/read/multinest.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/read/nestedfit.py` & `anesthetic-2.8.4/anesthetic/read/nestedfit.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/read/polychord.py` & `anesthetic-2.8.4/anesthetic/read/polychord.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/read/ultranest.py` & `anesthetic-2.8.4/anesthetic/read/ultranest.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/samples.py` & `anesthetic-2.8.4/anesthetic/samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,14 +351,16 @@
                             ax.set_ylabel(ylabel)
                     else:
                         if x == y:
                             ax.twin.plot([], [])
                         else:
                             ax.plot([], [])
 
+        axes._set_logticks()
+
         return axes
 
     plot_2d_default_kinds = {
         'default': {'diagonal': 'kde_1d',
                     'lower': 'kde_2d',
                     'upper': 'scatter_2d'},
         'kde': {'diagonal': 'kde_1d', 'lower': 'kde_2d'},
```

### Comparing `anesthetic-2.8.3/anesthetic/scripts.py` & `anesthetic-2.8.4/anesthetic/scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/utils.py` & `anesthetic-2.8.4/anesthetic/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/weighted_labelled_pandas.py` & `anesthetic-2.8.4/anesthetic/weighted_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic/weighted_pandas.py` & `anesthetic-2.8.4/anesthetic/weighted_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/anesthetic.egg-info/PKG-INFO` & `anesthetic-2.8.4/anesthetic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.8.3
+Version: 2.8.4
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Deborah Odunuyi <debbieodunuyi@gmail.com>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>, Dily Ong <dlo26@cam.ac.uk>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -80,15 +80,15 @@
 Requires-Dist: getdist; extra == "all"
 Requires-Dist: tables; extra == "all"
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.8.3
+:Version: 2.8.4
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.8.3/anesthetic.egg-info/SOURCES.txt` & `anesthetic-2.8.4/anesthetic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/pyproject.toml` & `anesthetic-2.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/tests/test_convert.py` & `anesthetic-2.8.4/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/tests/test_examples.py` & `anesthetic-2.8.4/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/tests/test_gui.py` & `anesthetic-2.8.4/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/tests/test_labelled_pandas.py` & `anesthetic-2.8.4/tests/test_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/tests/test_plot.py` & `anesthetic-2.8.4/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/tests/test_reader.py` & `anesthetic-2.8.4/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/tests/test_samples.py` & `anesthetic-2.8.4/tests/test_samples.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,14 +510,33 @@
                     if x == 'x2':
                         assert ax.twin.get_xscale() == 'log'
                     else:
                         assert ax.twin.get_xscale() == 'linear'
                     assert ax.twin.get_yscale() == 'linear'
 
 
+def test_logscale_ticks():
+    np.random.seed(42)
+    ndim = 5
+    data = np.exp(10 * np.random.randn(200, ndim))
+    params = [f'a{i}' for i in range(ndim)]
+    fig, axes = make_2d_axes(params, logx=params, logy=params, upper=False)
+    samples = Samples(data, columns=params)
+    samples.plot_2d(axes)
+    for _, col in axes.iterrows():
+        for _, ax in col.items():
+            if ax is not None:
+                xlims = ax.get_xlim()
+                xticks = ax.get_xticks()
+                assert np.sum((xticks > xlims[0]) & (xticks < xlims[1])) > 1
+                ylims = ax.get_ylim()
+                yticks = ax.get_yticks()
+                assert np.sum((yticks > ylims[0]) & (yticks < ylims[1])) > 1
+
+
 @pytest.mark.parametrize('k', ['hist_1d', 'hist'])
 @pytest.mark.parametrize('b', ['scott', 10, np.logspace(-3, 0, 20)])
 @pytest.mark.parametrize('r', [None, (1e-5, 1)])
 def test_plot_logscale_hist_kwargs(k, b, r):
     ns = read_chains('./tests/example_data/pc')
     with pytest.warns(UserWarning) if k == 'hist' else nullcontext():
         axes = ns[['x2']].plot_1d(kind=k, logx=['x2'], bins=b, range=r)
```

### Comparing `anesthetic-2.8.3/tests/test_scripts.py` & `anesthetic-2.8.4/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/tests/test_utils.py` & `anesthetic-2.8.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/tests/test_weighted_labelled_pandas.py` & `anesthetic-2.8.4/tests/test_weighted_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.3/tests/test_weighted_pandas.py` & `anesthetic-2.8.4/tests/test_weighted_pandas.py`

 * *Files identical despite different names*

