# Comparing `tmp/pymonke-0.1.0.tar.gz` & `tmp/pymonke-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonke-0.1.0.tar", last modified: Tue Apr  2 20:39:27 2024, max compression
+gzip compressed data, was "pymonke-0.1.1.tar", last modified: Mon Apr  8 16:38:28 2024, max compression
```

## Comparing `pymonke-0.1.0.tar` & `pymonke-0.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.131871 pymonke-0.1.0/
--rw-rw-rw-   0        0        0     1095 2024-01-31 16:24:15.000000 pymonke-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      660 2024-04-02 20:39:27.131871 pymonke-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5033 2024-03-03 13:48:10.000000 pymonke-0.1.0/README.md
--rw-rw-rw-   0        0        0      160 2024-03-03 13:48:10.000000 pymonke-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      899 2024-04-02 20:39:27.132876 pymonke-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.068730 pymonke-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.079242 pymonke-0.1.0/src/pymonke/
--rw-rw-rw-   0        0        0      333 2024-04-02 12:37:38.000000 pymonke-0.1.0/src/pymonke/__init__.py
--rw-rw-rw-   0        0        0      269 2024-03-15 15:51:29.000000 pymonke-0.1.0/src/pymonke/__main__.py
--rw-rw-rw-   0        0        0     1548 2024-03-03 13:48:10.000000 pymonke-0.1.0/src/pymonke/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.088260 pymonke-0.1.0/src/pymonke/fit/
--rw-rw-rw-   0        0        0      133 2024-03-29 19:58:06.000000 pymonke-0.1.0/src/pymonke/fit/__init__.py
--rw-rw-rw-   0        0        0     1106 2024-03-29 19:57:55.000000 pymonke-0.1.0/src/pymonke/fit/__misc.py
--rw-rw-rw-   0        0        0    10447 2024-04-02 14:16:53.000000 pymonke-0.1.0/src/pymonke/fit/fit.py
--rw-rw-rw-   0        0        0     1601 2024-04-02 12:34:08.000000 pymonke-0.1.0/src/pymonke/fit/fit_result.py
--rw-rw-rw-   0        0        0     6700 2024-04-02 12:41:49.000000 pymonke-0.1.0/src/pymonke/fit/parse.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.098786 pymonke-0.1.0/src/pymonke/gui/
--rw-rw-rw-   0        0        0      289 2024-03-22 17:45:13.000000 pymonke-0.1.0/src/pymonke/gui/__init__.py
--rw-rw-rw-   0        0        0     3840 2024-03-25 21:06:09.000000 pymonke-0.1.0/src/pymonke/gui/app.py
--rw-rw-rw-   0        0        0     1185 2024-03-23 22:03:51.000000 pymonke-0.1.0/src/pymonke/gui/browse_frame.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.102792 pymonke-0.1.0/src/pymonke/gui/data_init/
--rw-rw-rw-   0        0        0        0 2024-03-17 12:55:10.000000 pymonke-0.1.0/src/pymonke/gui/data_init/__init__.py
--rw-rw-rw-   0        0        0      751 2024-03-23 20:42:12.000000 pymonke-0.1.0/src/pymonke/gui/data_init/browse_save_frame.py
--rw-rw-rw-   0        0        0     5217 2024-03-24 15:12:49.000000 pymonke-0.1.0/src/pymonke/gui/data_init/data_init_frame.py
--rw-rw-rw-   0        0        0     1398 2024-03-24 08:58:03.000000 pymonke-0.1.0/src/pymonke/gui/data_init/status_frame.py
--rw-rw-rw-   0        0        0     5729 2024-03-25 15:55:43.000000 pymonke-0.1.0/src/pymonke/gui/dict_frame.py
--rw-rw-rw-   0        0        0     1123 2024-03-23 22:07:47.000000 pymonke-0.1.0/src/pymonke/gui/entry_label_frame.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.107312 pymonke-0.1.0/src/pymonke/gui/fitting/
--rw-rw-rw-   0        0        0     3505 2024-03-25 22:43:11.000000 pymonke-0.1.0/src/pymonke/gui/fitting/add_args_frame.py
--rw-rw-rw-   0        0        0    10157 2024-03-25 22:19:06.000000 pymonke-0.1.0/src/pymonke/gui/fitting/fit_frame.py
--rw-rw-rw-   0        0        0     2462 2024-03-24 15:12:59.000000 pymonke-0.1.0/src/pymonke/gui/fitting/fit_option_menu.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.110311 pymonke-0.1.0/src/pymonke/gui/formula/
--rw-rw-rw-   0        0        0     2889 2024-03-23 21:13:25.000000 pymonke-0.1.0/src/pymonke/gui/formula/formula_frame.py
--rw-rw-rw-   0        0        0     1424 2024-03-23 21:18:19.000000 pymonke-0.1.0/src/pymonke/gui/formula/parameter_frame.py
--rw-rw-rw-   0        0        0     2421 2024-03-23 21:25:28.000000 pymonke-0.1.0/src/pymonke/gui/formula/parameters_scrollable_frame.py
--rw-rw-rw-   0        0        0      388 2024-03-23 21:44:32.000000 pymonke-0.1.0/src/pymonke/gui/info_label.py
--rw-rw-rw-   0        0        0      561 2024-03-25 22:19:40.000000 pymonke-0.1.0/src/pymonke/gui/labeled_entry.py
--rw-rw-rw-   0        0        0     2628 2024-03-25 15:19:40.000000 pymonke-0.1.0/src/pymonke/gui/list_frame.py
--rw-rw-rw-   0        0        0       85 2024-03-23 22:16:21.000000 pymonke-0.1.0/src/pymonke/gui/main.py
--rw-rw-rw-   0        0        0     3038 2024-03-23 22:27:18.000000 pymonke-0.1.0/src/pymonke/gui/misc.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.114337 pymonke-0.1.0/src/pymonke/gui/plot/
--rw-rw-rw-   0        0        0     3560 2024-03-25 13:24:18.000000 pymonke-0.1.0/src/pymonke/gui/plot/limits_frame.py
--rw-rw-rw-   0        0        0     4806 2024-03-26 15:12:55.000000 pymonke-0.1.0/src/pymonke/gui/plot/misc_data_frame.py
--rw-rw-rw-   0        0        0     2114 2024-03-24 10:01:38.000000 pymonke-0.1.0/src/pymonke/gui/plot/plot_canvas.py
--rw-rw-rw-   0        0        0     4544 2024-04-02 20:38:13.000000 pymonke-0.1.0/src/pymonke/gui/plot/plot_frame.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.118842 pymonke-0.1.0/src/pymonke/latex/
--rw-rw-rw-   0        0        0      175 2024-04-02 12:24:16.000000 pymonke-0.1.0/src/pymonke/latex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.120842 pymonke-0.1.0/src/pymonke/latex/tests/
--rw-rw-rw-   0        0        0        0 2024-03-03 13:48:10.000000 pymonke-0.1.0/src/pymonke/latex/tests/__init__.py
--rw-rw-rw-   0        0        0     1225 2024-03-03 13:48:10.000000 pymonke-0.1.0/src/pymonke/latex/tests/table_test.py
--rw-rw-rw-   0        0        0     3096 2024-04-02 08:30:50.000000 pymonke-0.1.0/src/pymonke/latex/tex_table.py
--rw-rw-rw-   0        0        0     4420 2024-04-02 11:45:56.000000 pymonke-0.1.0/src/pymonke/latex/utils.py
--rw-rw-rw-   0        0        0     1549 2024-03-03 13:48:10.000000 pymonke-0.1.0/src/pymonke/latex/utils.pyi
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.126372 pymonke-0.1.0/src/pymonke/misc/
--rw-rw-rw-   0        0        0        0 2024-03-13 17:06:30.000000 pymonke-0.1.0/src/pymonke/misc/__init__.py
--rw-rw-rw-   0        0        0     1853 2024-04-02 12:26:57.000000 pymonke-0.1.0/src/pymonke/misc/benchmark.py
--rw-rw-rw-   0        0        0     3198 2024-04-02 14:02:30.000000 pymonke-0.1.0/src/pymonke/misc/dataframe.py
--rw-rw-rw-   0        0        0     1010 2024-04-02 12:27:25.000000 pymonke-0.1.0/src/pymonke/misc/file_management.py
--rw-rw-rw-   0        0        0      757 2024-04-02 20:39:13.000000 pymonke-0.1.0/src/pymonke/misc/pymonke_json_decoder.py
--rw-rw-rw-   0        0        0      297 2024-04-02 14:33:51.000000 pymonke-0.1.0/src/pymonke/misc/pymonke_json_encoder.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.128872 pymonke-0.1.0/src/pymonke/mmath/
--rw-rw-rw-   0        0        0       65 2024-04-02 12:36:10.000000 pymonke-0.1.0/src/pymonke/mmath/__init__.py
--rw-rw-rw-   0        0        0      759 2024-04-02 12:35:53.000000 pymonke-0.1.0/src/pymonke/mmath/rounding.py
--rw-rw-rw-   0        0        0      890 2024-03-14 10:22:20.000000 pymonke-0.1.0/src/pymonke/mmath/statistics.py
--rw-rw-rw-   0        0        0        0 2024-03-03 13:48:10.000000 pymonke-0.1.0/src/pymonke/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.130872 pymonke-0.1.0/src/pymonke.egg-info/
--rw-rw-rw-   0        0        0      660 2024-04-02 20:39:27.000000 pymonke-0.1.0/src/pymonke.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1817 2024-04-02 20:39:27.000000 pymonke-0.1.0/src/pymonke.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 20:39:27.000000 pymonke-0.1.0/src/pymonke.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-02 20:39:27.000000 pymonke-0.1.0/src/pymonke.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 20:39:27.000000 pymonke-0.1.0/src/pymonke.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.129871 pymonke-0.1.0/tests/
--rw-rw-rw-   0        0        0     2243 2024-04-02 14:13:14.000000 pymonke-0.1.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.227686 pymonke-0.1.1/
+-rw-rw-rw-   0        0        0     1095 2024-01-31 16:24:15.000000 pymonke-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      695 2024-04-08 16:38:28.227185 pymonke-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5033 2024-03-03 13:48:10.000000 pymonke-0.1.1/README.md
+-rw-rw-rw-   0        0        0      160 2024-03-03 13:48:10.000000 pymonke-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      920 2024-04-08 16:38:28.228685 pymonke-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.172651 pymonke-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.183165 pymonke-0.1.1/src/pymonke/
+-rw-rw-rw-   0        0        0      371 2024-04-08 16:27:10.000000 pymonke-0.1.1/src/pymonke/__init__.py
+-rw-rw-rw-   0        0        0      269 2024-03-15 15:51:29.000000 pymonke-0.1.1/src/pymonke/__main__.py
+-rw-rw-rw-   0        0        0     1548 2024-03-03 13:48:10.000000 pymonke-0.1.1/src/pymonke/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.191167 pymonke-0.1.1/src/pymonke/fit/
+-rw-rw-rw-   0        0        0      133 2024-03-29 19:58:06.000000 pymonke-0.1.1/src/pymonke/fit/__init__.py
+-rw-rw-rw-   0        0        0     1106 2024-03-29 19:57:55.000000 pymonke-0.1.1/src/pymonke/fit/__misc.py
+-rw-rw-rw-   0        0        0    10791 2024-04-08 08:02:31.000000 pymonke-0.1.1/src/pymonke/fit/fit.py
+-rw-rw-rw-   0        0        0     3684 2024-04-08 07:55:52.000000 pymonke-0.1.1/src/pymonke/fit/fit_result.py
+-rw-rw-rw-   0        0        0     6855 2024-04-08 08:00:58.000000 pymonke-0.1.1/src/pymonke/fit/parse.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.200167 pymonke-0.1.1/src/pymonke/gui/
+-rw-rw-rw-   0        0        0      289 2024-03-22 17:45:13.000000 pymonke-0.1.1/src/pymonke/gui/__init__.py
+-rw-rw-rw-   0        0        0     3880 2024-04-08 16:31:06.000000 pymonke-0.1.1/src/pymonke/gui/app.py
+-rw-rw-rw-   0        0        0     1185 2024-03-23 22:03:51.000000 pymonke-0.1.1/src/pymonke/gui/browse_frame.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.203671 pymonke-0.1.1/src/pymonke/gui/data_init/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:55:10.000000 pymonke-0.1.1/src/pymonke/gui/data_init/__init__.py
+-rw-rw-rw-   0        0        0      751 2024-03-23 20:42:12.000000 pymonke-0.1.1/src/pymonke/gui/data_init/browse_save_frame.py
+-rw-rw-rw-   0        0        0     5217 2024-03-24 15:12:49.000000 pymonke-0.1.1/src/pymonke/gui/data_init/data_init_frame.py
+-rw-rw-rw-   0        0        0     1398 2024-03-24 08:58:03.000000 pymonke-0.1.1/src/pymonke/gui/data_init/status_frame.py
+-rw-rw-rw-   0        0        0     5729 2024-03-25 15:55:43.000000 pymonke-0.1.1/src/pymonke/gui/dict_frame.py
+-rw-rw-rw-   0        0        0     1123 2024-03-23 22:07:47.000000 pymonke-0.1.1/src/pymonke/gui/entry_label_frame.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.206173 pymonke-0.1.1/src/pymonke/gui/fitting/
+-rw-rw-rw-   0        0        0     3505 2024-03-25 22:43:11.000000 pymonke-0.1.1/src/pymonke/gui/fitting/add_args_frame.py
+-rw-rw-rw-   0        0        0    10162 2024-04-08 16:09:40.000000 pymonke-0.1.1/src/pymonke/gui/fitting/fit_frame.py
+-rw-rw-rw-   0        0        0     2462 2024-03-24 15:12:59.000000 pymonke-0.1.1/src/pymonke/gui/fitting/fit_option_menu.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.208672 pymonke-0.1.1/src/pymonke/gui/formula/
+-rw-rw-rw-   0        0        0     2889 2024-03-23 21:13:25.000000 pymonke-0.1.1/src/pymonke/gui/formula/formula_frame.py
+-rw-rw-rw-   0        0        0     1424 2024-03-23 21:18:19.000000 pymonke-0.1.1/src/pymonke/gui/formula/parameter_frame.py
+-rw-rw-rw-   0        0        0     2421 2024-04-08 16:10:31.000000 pymonke-0.1.1/src/pymonke/gui/formula/parameters_scrollable_frame.py
+-rw-rw-rw-   0        0        0      388 2024-03-23 21:44:32.000000 pymonke-0.1.1/src/pymonke/gui/info_label.py
+-rw-rw-rw-   0        0        0      561 2024-03-25 22:19:40.000000 pymonke-0.1.1/src/pymonke/gui/labeled_entry.py
+-rw-rw-rw-   0        0        0     2628 2024-03-25 15:19:40.000000 pymonke-0.1.1/src/pymonke/gui/list_frame.py
+-rw-rw-rw-   0        0        0      225 2024-04-08 16:32:10.000000 pymonke-0.1.1/src/pymonke/gui/main.py
+-rw-rw-rw-   0        0        0     3038 2024-03-23 22:27:18.000000 pymonke-0.1.1/src/pymonke/gui/misc.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.212174 pymonke-0.1.1/src/pymonke/gui/plot/
+-rw-rw-rw-   0        0        0     3560 2024-03-25 13:24:18.000000 pymonke-0.1.1/src/pymonke/gui/plot/limits_frame.py
+-rw-rw-rw-   0        0        0     5207 2024-04-08 16:19:07.000000 pymonke-0.1.1/src/pymonke/gui/plot/misc_data_frame.py
+-rw-rw-rw-   0        0        0     2148 2024-04-08 16:31:36.000000 pymonke-0.1.1/src/pymonke/gui/plot/plot_canvas.py
+-rw-rw-rw-   0        0        0     4544 2024-04-02 20:38:13.000000 pymonke-0.1.1/src/pymonke/gui/plot/plot_frame.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.215674 pymonke-0.1.1/src/pymonke/latex/
+-rw-rw-rw-   0        0        0      175 2024-04-02 12:24:16.000000 pymonke-0.1.1/src/pymonke/latex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.217175 pymonke-0.1.1/src/pymonke/latex/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-03 13:48:10.000000 pymonke-0.1.1/src/pymonke/latex/tests/__init__.py
+-rw-rw-rw-   0        0        0     1225 2024-03-03 13:48:10.000000 pymonke-0.1.1/src/pymonke/latex/tests/table_test.py
+-rw-rw-rw-   0        0        0     3096 2024-04-02 08:30:50.000000 pymonke-0.1.1/src/pymonke/latex/tex_table.py
+-rw-rw-rw-   0        0        0     4420 2024-04-02 11:45:56.000000 pymonke-0.1.1/src/pymonke/latex/utils.py
+-rw-rw-rw-   0        0        0     1549 2024-03-03 13:48:10.000000 pymonke-0.1.1/src/pymonke/latex/utils.pyi
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.222184 pymonke-0.1.1/src/pymonke/misc/
+-rw-rw-rw-   0        0        0        0 2024-03-13 17:06:30.000000 pymonke-0.1.1/src/pymonke/misc/__init__.py
+-rw-rw-rw-   0        0        0     1853 2024-04-02 12:26:57.000000 pymonke-0.1.1/src/pymonke/misc/benchmark.py
+-rw-rw-rw-   0        0        0     3198 2024-04-02 14:02:30.000000 pymonke-0.1.1/src/pymonke/misc/dataframe.py
+-rw-rw-rw-   0        0        0     1010 2024-04-02 12:27:25.000000 pymonke-0.1.1/src/pymonke/misc/file_management.py
+-rw-rw-rw-   0        0        0      757 2024-04-02 20:39:13.000000 pymonke-0.1.1/src/pymonke/misc/pymonke_json_decoder.py
+-rw-rw-rw-   0        0        0      297 2024-04-02 14:33:51.000000 pymonke-0.1.1/src/pymonke/misc/pymonke_json_encoder.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.224685 pymonke-0.1.1/src/pymonke/mmath/
+-rw-rw-rw-   0        0        0       65 2024-04-02 12:36:10.000000 pymonke-0.1.1/src/pymonke/mmath/__init__.py
+-rw-rw-rw-   0        0        0      759 2024-04-02 12:35:53.000000 pymonke-0.1.1/src/pymonke/mmath/rounding.py
+-rw-rw-rw-   0        0        0      890 2024-03-14 10:22:20.000000 pymonke-0.1.1/src/pymonke/mmath/statistics.py
+-rw-rw-rw-   0        0        0        0 2024-03-03 13:48:10.000000 pymonke-0.1.1/src/pymonke/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.226686 pymonke-0.1.1/src/pymonke.egg-info/
+-rw-rw-rw-   0        0        0      695 2024-04-08 16:38:28.000000 pymonke-0.1.1/src/pymonke.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1817 2024-04-08 16:38:28.000000 pymonke-0.1.1/src/pymonke.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:38:28.000000 pymonke-0.1.1/src/pymonke.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2024-04-08 16:38:28.000000 pymonke-0.1.1/src/pymonke.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 16:38:28.000000 pymonke-0.1.1/src/pymonke.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.225685 pymonke-0.1.1/tests/
+-rw-rw-rw-   0        0        0     2028 2024-04-08 16:33:36.000000 pymonke-0.1.1/tests/test.py
```

### Comparing `pymonke-0.1.0/LICENSE` & `pymonke-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/PKG-INFO` & `pymonke-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonke
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for creating lab reports and data analysis
 Home-page: https://github.com/GabrielRemi/pymonke
 Author: Gabriel Remiszewski
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -13,9 +13,10 @@
 Requires-Dist: pandas>=2.2
 Requires-Dist: nltk>=3.8
 Requires-Dist: matplotlib>=3.8
 Requires-Dist: mypy_extensions>=1.0
 Requires-Dist: scienceplots>=2.1
 Requires-Dist: customtkinter>=5.2
 Requires-Dist: scipy>=1.12
+Requires-Dist: uncertainties>=3.1
 
 longer description
```

### Comparing `pymonke-0.1.0/README.md` & `pymonke-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/setup.cfg` & `pymonke-0.1.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 6f6e 6b65 0d0a 7665 7273   = pymonke..vers
-00000020: 696f 6e20 3d20 302e 312e 300d 0a61 7574  ion = 0.1.0..aut
+00000020: 696f 6e20 3d20 302e 312e 310d 0a61 7574  ion = 0.1.1..aut
 00000030: 686f 7220 3d20 4761 6272 6965 6c20 5265  hor = Gabriel Re
 00000040: 6d69 737a 6577 736b 690d 0a64 6573 6372  miszewski..descr
 00000050: 6970 7469 6f6e 203d 2054 6f6f 6c73 2066  iption = Tools f
 00000060: 6f72 2063 7265 6174 696e 6720 6c61 6220  or creating lab 
 00000070: 7265 706f 7274 7320 616e 6420 6461 7461  reports and data
 00000080: 2061 6e61 6c79 7369 730d 0a6c 6f6e 675f   analysis..long_
 00000090: 6465 7363 7269 7074 696f 6e20 3d20 6c6f  description = lo
@@ -28,30 +28,31 @@
 000001b0: 616e 6461 733e 3d32 2e32 0d0a 096e 6c74  andas>=2.2...nlt
 000001c0: 6b3e 3d33 2e38 0d0a 096d 6174 706c 6f74  k>=3.8...matplot
 000001d0: 6c69 623e 3d33 2e38 0d0a 096d 7970 795f  lib>=3.8...mypy_
 000001e0: 6578 7465 6e73 696f 6e73 3e3d 312e 300d  extensions>=1.0.
 000001f0: 0a09 7363 6965 6e63 6570 6c6f 7473 3e3d  ..scienceplots>=
 00000200: 322e 310d 0a09 6375 7374 6f6d 746b 696e  2.1...customtkin
 00000210: 7465 723e 3d35 2e32 0d0a 0973 6369 7079  ter>=5.2...scipy
-00000220: 3e3d 312e 3132 0d0a 0d0a 5b6d 7970 795d  >=1.12....[mypy]
-00000230: 0d0a 6469 7361 6c6c 6f77 5f75 6e74 7970  ..disallow_untyp
-00000240: 6564 5f64 6566 7320 3d20 5472 7565 0d0a  ed_defs = True..
-00000250: 6469 7361 6c6c 6f77 5f73 7562 636c 6173  disallow_subclas
-00000260: 7369 6e67 5f61 6e79 203d 2046 616c 7365  sing_any = False
-00000270: 0d0a 0d0a 5b6d 7970 792d 7363 6970 792e  ....[mypy-scipy.
-00000280: 2a2c 6e6c 746b 2e2a 2c73 6369 656e 6365  *,nltk.*,science
-00000290: 706c 6f74 732e 2a2c 6375 7374 6f6d 746b  plots.*,customtk
-000002a0: 696e 7465 722e 2a2c 6963 6563 7265 616d  inter.*,icecream
-000002b0: 2c75 6e63 6572 7461 696e 7469 6573 2e2a  ,uncertainties.*
-000002c0: 5d0d 0a69 676e 6f72 655f 6d69 7373 696e  ]..ignore_missin
-000002d0: 675f 696d 706f 7274 7320 3d20 7472 7565  g_imports = true
-000002e0: 0d0a 0d0a 5b6d 7970 792d 6d61 7470 6c6f  ....[mypy-matplo
-000002f0: 746c 6962 2e62 6163 6b65 6e64 732e 2a5d  tlib.backends.*]
-00000300: 0d0a 696d 706c 6963 6974 5f72 6565 7870  ..implicit_reexp
-00000310: 6f72 7420 3d20 5472 7565 0d0a 6469 7361  ort = True..disa
-00000320: 6c6c 6f77 5f75 6e74 7970 6564 5f64 6566  llow_untyped_def
-00000330: 7320 3d20 4661 6c73 650d 0a63 6865 636b  s = False..check
-00000340: 5f75 6e74 7970 6564 5f64 6566 7320 3d20  _untyped_defs = 
-00000350: 4661 6c73 650d 0a0d 0a5b 6567 675f 696e  False....[egg_in
-00000360: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000370: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000380: 0a0d 0a                                  ...
+00000220: 3e3d 312e 3132 0d0a 0975 6e63 6572 7461  >=1.12...uncerta
+00000230: 696e 7469 6573 3e3d 332e 310d 0a0d 0a5b  inties>=3.1....[
+00000240: 6d79 7079 5d0d 0a64 6973 616c 6c6f 775f  mypy]..disallow_
+00000250: 756e 7479 7065 645f 6465 6673 203d 2054  untyped_defs = T
+00000260: 7275 650d 0a64 6973 616c 6c6f 775f 7375  rue..disallow_su
+00000270: 6263 6c61 7373 696e 675f 616e 7920 3d20  bclassing_any = 
+00000280: 4661 6c73 650d 0a0d 0a5b 6d79 7079 2d73  False....[mypy-s
+00000290: 6369 7079 2e2a 2c6e 6c74 6b2e 2a2c 7363  cipy.*,nltk.*,sc
+000002a0: 6965 6e63 6570 6c6f 7473 2e2a 2c63 7573  ienceplots.*,cus
+000002b0: 746f 6d74 6b69 6e74 6572 2e2a 2c69 6365  tomtkinter.*,ice
+000002c0: 6372 6561 6d2c 756e 6365 7274 6169 6e74  cream,uncertaint
+000002d0: 6965 732e 2a5d 0d0a 6967 6e6f 7265 5f6d  ies.*]..ignore_m
+000002e0: 6973 7369 6e67 5f69 6d70 6f72 7473 203d  issing_imports =
+000002f0: 2074 7275 650d 0a0d 0a5b 6d79 7079 2d6d   true....[mypy-m
+00000300: 6174 706c 6f74 6c69 622e 6261 636b 656e  atplotlib.backen
+00000310: 6473 2e2a 5d0d 0a69 6d70 6c69 6369 745f  ds.*]..implicit_
+00000320: 7265 6578 706f 7274 203d 2054 7275 650d  reexport = True.
+00000330: 0a64 6973 616c 6c6f 775f 756e 7479 7065  .disallow_untype
+00000340: 645f 6465 6673 203d 2046 616c 7365 0d0a  d_defs = False..
+00000350: 6368 6563 6b5f 756e 7479 7065 645f 6465  check_untyped_de
+00000360: 6673 203d 2046 616c 7365 0d0a 0d0a 5b65  fs = False....[e
+00000370: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000380: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000390: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `pymonke-0.1.0/src/pymonke/constants.py` & `pymonke-0.1.1/src/pymonke/constants.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/fit/__misc.py` & `pymonke-0.1.1/src/pymonke/fit/__misc.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/fit/fit.py` & `pymonke-0.1.1/src/pymonke/fit/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from matplotlib.axes import Axes
 from mypy_extensions import VarArg
 import numpy as np
 from pandas import DataFrame, Series
 from scipy import odr
 from scipy.optimize import curve_fit
 
-from .fit_result import FitResult
+from .fit_result import FitResult, result
 from .parse import parse_function, replace_funcs, numerical, scalar, array, parse_variable_str
 from ..misc.dataframe import get_error_column_name, has_uncertainty
 from ..misc.file_management import read_data_into_dataframe
 
 func_type: TypeAlias = Callable[[numerical, VarArg(scalar)], numerical]
 
 
@@ -67,15 +67,14 @@
             if (dpi := self.meta.get("figure_dpi")) is None:
                 dpi = 120
             plt.figure(num=figure_id, figsize=size, dpi=dpi)
 
         data = self.__get_data()
         x, y, sx, sy = data["x"], data["y"], data["sx"], data["sy"]
 
-
         plotting_style = {
             "linestyle": "",
             "ms": 4,
             "marker": "o",
             "capsize": 3.5,
             "zorder": 2
         }
@@ -121,15 +120,15 @@
 
         limits: List[float] = list(self.__get_xlim(meta))
         if (val := meta.get("plot_x_min_limit")) is not None:
             limits[0] = val
         if (val := meta.get("plot_x_max_limit")) is not None:
             limits[1] = val
         x = np.linspace(*limits, points)
-        label = parse_variable_str(meta.get("label") or "$\\chi^2 = #chi $", fit_res)
+        label = parse_variable_str(meta.get("label") or "$\\chi^2 = #chi $", fit_res, self.meta.get("latex") or False)
         if ax is None:
             plt.plot(x, fit_res.eval(x), **plotting_style, label=label)
         else:
             ax.plot(x, fit_res.eval(x), **plotting_style, label=label)
 
     # ----------------------------------------------------------------------------------------
 
@@ -186,16 +185,18 @@
         if (b := meta.get("absolute_sigma")) is None:
             b = False
         if (check_finite := meta.get("check_finite")) is None:
             check_finite = False
         out: tuple = curve_fit(function, xdata=x, ydata=y, sigma=y_error, absolute_sigma=b,
                                check_finite=check_finite, p0=p0)
         popt, pcov = out
-        fit_res = FitResult(function, params, popt, np.sqrt(pcov.diagonal()))
-        fit_res.set_reduced_chi_squared(x, y, y_error)
+        # fit_res = FitResult(function, params, popt, np.sqrt(pcov.diagonal()))
+        # fit_res.set_reduced_chi_squared(x, y, y_error)
+        fit_res = result(function, x, y, y_error, param_names=params, params=popt,
+                         params_std_dev=np.sqrt(pcov.diagonal()))
         return fit_res
 
     def __do_odr_fit(self, meta: dict) -> FitResult:
         function, params, p0, lim, arrays = self.__get_fitting_data(meta)
         x, y, sy = arrays["x"], arrays["y"], arrays["sy"]
         sx = arrays.get("sx")
         assert isinstance(x, Series) and isinstance(y, Series) and isinstance(sy, Series)
@@ -212,31 +213,32 @@
 
         def odr_func(_b: list, _x: float | int) -> numerical:
             return function(_x, *_b)
 
         odr_model = odr.Model(odr_func)
         odr_odr = odr.ODR(odr_data, odr_model, p0)
         odr_out: odr.Output = odr_odr.run()
-        fit_res = FitResult(function, params, odr_out.beta, odr_out.sd_beta)
-        fit_res.set_reduced_chi_squared(x, y, sy)
+        # fit_res = FitResult(function, params, odr_out.beta, odr_out.sd_beta)
+        # fit_res.set_reduced_chi_squared(x, y, sy)
+        fit_res = result(function, x, y, sy, param_names=params, params=odr_out.beta, params_std_dev=odr_out.sd_beta,
+                         sx=sx)
         return fit_res
 
     def __get_fitting_data(self, meta: dict) -> Any:
 
         p0: List[float | int] = meta["start_parameters"]
         x_min, x_max = self.__get_xlim(meta)
 
         query = f"{self.column_names['x']} >= {x_min} and {self.column_names['x']} <= {x_max}"
         # data = self.data.query(query)
 
         fitting_data = self.__get_data(query)
 
         function, params = parse_function(replace_funcs(meta["function"]))
 
-
         lim: Tuple[float, float] = (x_min, x_max)
 
         return function, params, p0, lim, fitting_data
 
     def __get_data(self, query: str = None) -> dict[str, Any]:
         if query is None:
             data = self.data
@@ -266,9 +268,7 @@
             "x": x,
             "y": y,
             "sy": sy,
             "sx": sx,
         }
 
         return fitting_data
-
-
```

### Comparing `pymonke-0.1.0/src/pymonke/fit/parse.py` & `pymonke-0.1.1/src/pymonke/fit/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         raise SyntaxError(e)
     except ArithmeticError:
         pass
 
     return function, params
 
 
-def parse_variable_str(label_str: str, result: FitResult) -> str:
+def parse_variable_str(label_str: str, result: FitResult, latex: bool = False) -> str:
     """Reads a string that has variable names marked with '#' and replaces them with their values
     from the FitResult object."""
     res_dict = result.as_dict(chi_square=True)
     tokens = label_str.split()
     for index, tok in enumerate(tokens):
         if tok[0] != "#":
             continue
@@ -182,15 +182,19 @@
         value_error = f"Cannot access attribute of parameter {tok}. Only #paramter.val or #paramter.err are "
         f"allowed as inputs"
         if "." not in tok:
             if tok == "chi":
                 tokens[index] = str(round(res_dict["reduced_chi_squared"], 2))
             else:
                 try:
-                    tokens[index] = str(res_dict[tok])
+                    if latex:
+                        tokens[index] = "{:L}".format(res_dict[tok])
+                    else:
+                        tokens[index] = str(res_dict[tok])
+
                 except KeyError:
                     raise KeyError(key_error)
         else:
             try:
                 param, attr = tok.split(".")
             except:
                 raise ValueError(value_error)
```

### Comparing `pymonke-0.1.0/src/pymonke/gui/app.py` & `pymonke-0.1.1/src/pymonke/gui/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     def __init__(self, rel_height: float = 0.6, rel_width: float = 0.8):
         ctk.CTk.__init__(self)
 
         self.geometry(self.__get_geometry(rel_height, rel_width))
         self.title("PyMonke data fitting")
         self.grid_columnconfigure((0, 1), weight=5)
         self.grid_columnconfigure(2, weight=8)
+        self.fit: Optional[Fit] = None
 
         # DATA
         self.meta: dict[str, Any] = dict()
         self.data: Optional[DataFrame] = None
         self.fit_result: Optional[dict[str, FitResult]] = None
 
         self.plot_frame = PlotFrame(master=self)
```

### Comparing `pymonke-0.1.0/src/pymonke/gui/browse_frame.py` & `pymonke-0.1.1/src/pymonke/gui/browse_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/data_init/browse_save_frame.py` & `pymonke-0.1.1/src/pymonke/gui/data_init/browse_save_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/data_init/data_init_frame.py` & `pymonke-0.1.1/src/pymonke/gui/data_init/data_init_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/data_init/status_frame.py` & `pymonke-0.1.1/src/pymonke/gui/data_init/status_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/dict_frame.py` & `pymonke-0.1.1/src/pymonke/gui/dict_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/entry_label_frame.py` & `pymonke-0.1.1/src/pymonke/gui/entry_label_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/fitting/add_args_frame.py` & `pymonke-0.1.1/src/pymonke/gui/fitting/add_args_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/fitting/fit_frame.py` & `pymonke-0.1.1/src/pymonke/gui/fitting/fit_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     def set_params_values_from_results(self) -> None:
         fit_name = self.get_fit_name()
         if fit_name is not None:
             fit_result = get_root(self).fit_result
             if fit_result is not None:
                 result = fit_result.get(fit_name)
                 if result is not None:
-                    get_root(self).get_fit_frame().set_param_values(result.as_dict())
+                    get_root(self).get_fit_frame().set_param_values(result.as_dict(False))
 
     def get_fit_type(self) -> str:
         if self.fit_type_option.get() == "OLS":
             return "optimize.curve_fit"
         elif self.fit_type_option.get() == "ODR":
             return "odr"
         else:
```

### Comparing `pymonke-0.1.0/src/pymonke/gui/fitting/fit_option_menu.py` & `pymonke-0.1.1/src/pymonke/gui/fitting/fit_option_menu.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/formula/formula_frame.py` & `pymonke-0.1.1/src/pymonke/gui/formula/formula_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/formula/parameter_frame.py` & `pymonke-0.1.1/src/pymonke/gui/formula/parameter_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/formula/parameters_scrollable_frame.py` & `pymonke-0.1.1/src/pymonke/gui/formula/parameters_scrollable_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/labeled_entry.py` & `pymonke-0.1.1/src/pymonke/gui/labeled_entry.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/list_frame.py` & `pymonke-0.1.1/src/pymonke/gui/list_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/misc.py` & `pymonke-0.1.1/src/pymonke/gui/misc.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/plot/limits_frame.py` & `pymonke-0.1.1/src/pymonke/gui/plot/limits_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/gui/plot/misc_data_frame.py` & `pymonke-0.1.1/src/pymonke/gui/plot/misc_data_frame.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from customtkinter import CTkFrame
+from customtkinter import CTkFrame, CTkCheckBox
 
 import json
 from typing import Any, Optional, AnyStr
 
 from ..labeled_entry import LabeledEntry
 from ..misc import get_meta
 
@@ -29,40 +29,48 @@
         self.dpi_entry.entry.bind("<Return>", self.callback)
         self.dpi_entry.grid(row=0, column=1, pady=5)
 
         self.label_entry = LabeledEntry(master=self, label="Label")
         self.label_entry.entry.bind("<Return>", self.callback)
         self.label_entry.grid(row=1, column=1, pady=5)
 
+        self.latex_check_box = CTkCheckBox(master=self, text="Latex", command=self.callback)
+        self.latex_check_box.grid(row=2, column=0, pady=5)
+
         self.meta = meta
 
     def callback(self, _: Any = None) -> None:
         # self.update_figure_style(self.figure_style_entry.text_var.get())
         figure_style: Optional[list[str]] = self.set_figure_style(self.figure_style_entry.text_var.get())
         figure_size: Optional[tuple[float, float]] = self.set_figure_size(self.figure_size_entry.text_var.get())
         dpi: Optional[float] = self.set_dpi(self.dpi_entry.text_var.get())
         label: str = self.get_label()
-
+        latex: bool = bool(self.latex_check_box.get())
         data = {
             "figure_style": figure_style,
             "figure_size": figure_size,
             "figure_dpi": dpi,
-            "label": label
+            "label": label,
+            "latex": latex,
         }
 
         if self.meta is not None:
             self.meta.update(data)
 
     def load_from_meta(self) -> None:
         if self.meta is None:
             return
         self.set_figure_style((self.meta.get("figure_style") or ""))
         self.set_figure_size(self.meta.get("figure_size") or "")
         self.set_dpi(self.meta.get("figure_dpi") or "")
         self.set_label(self.meta.get("label") or "")
+        if self.meta.get("latex") or False:
+            self.latex_check_box.select()
+        else:
+            self.latex_check_box.deselect()
 
     def get_figure_style(self) -> list[str]:
         text = self.figure_style_entry.text
         ret = text.split(",")
         assert isinstance(ret, list)
         return ret
```

### Comparing `pymonke-0.1.0/src/pymonke/gui/plot/plot_canvas.py` & `pymonke-0.1.1/src/pymonke/gui/plot/plot_canvas.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,8 +52,9 @@
         self.set_x_limits(_x_min, _x_max)
         self.set_y_limits(_y_min, _y_max)
 
     def plot_data(self) -> None:
         fit = get_root(self).do_fit()
         self.ax.clear()
         fit.plot(ax=self.ax)
+        get_root(self).fit = fit
         self.canvas.draw()  # type: ignore
```

### Comparing `pymonke-0.1.0/src/pymonke/gui/plot/plot_frame.py` & `pymonke-0.1.1/src/pymonke/gui/plot/plot_frame.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/latex/tests/table_test.py` & `pymonke-0.1.1/src/pymonke/latex/tests/table_test.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/latex/tex_table.py` & `pymonke-0.1.1/src/pymonke/latex/tex_table.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/latex/utils.py` & `pymonke-0.1.1/src/pymonke/latex/utils.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/latex/utils.pyi` & `pymonke-0.1.1/src/pymonke/latex/utils.pyi`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/misc/benchmark.py` & `pymonke-0.1.1/src/pymonke/misc/benchmark.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/misc/dataframe.py` & `pymonke-0.1.1/src/pymonke/misc/dataframe.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/misc/file_management.py` & `pymonke-0.1.1/src/pymonke/misc/file_management.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/misc/pymonke_json_decoder.py` & `pymonke-0.1.1/src/pymonke/misc/pymonke_json_decoder.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/mmath/rounding.py` & `pymonke-0.1.1/src/pymonke/mmath/rounding.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke/mmath/statistics.py` & `pymonke-0.1.1/src/pymonke/mmath/statistics.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.1.0/src/pymonke.egg-info/PKG-INFO` & `pymonke-0.1.1/src/pymonke.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonke
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for creating lab reports and data analysis
 Home-page: https://github.com/GabrielRemi/pymonke
 Author: Gabriel Remiszewski
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -13,9 +13,10 @@
 Requires-Dist: pandas>=2.2
 Requires-Dist: nltk>=3.8
 Requires-Dist: matplotlib>=3.8
 Requires-Dist: mypy_extensions>=1.0
 Requires-Dist: scienceplots>=2.1
 Requires-Dist: customtkinter>=5.2
 Requires-Dist: scipy>=1.12
+Requires-Dist: uncertainties>=3.1
 
 longer description
```

### Comparing `pymonke-0.1.0/src/pymonke.egg-info/SOURCES.txt` & `pymonke-0.1.1/src/pymonke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

