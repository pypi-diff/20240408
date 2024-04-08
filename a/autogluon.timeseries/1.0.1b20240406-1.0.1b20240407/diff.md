# Comparing `tmp/autogluon.timeseries-1.0.1b20240406.tar.gz` & `tmp/autogluon.timeseries-1.0.1b20240407.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-1.0.1b20240406.tar", last modified: Sat Apr  6 09:05:30 2024, max compression
+gzip compressed data, was "autogluon.timeseries-1.0.1b20240407.tar", last modified: Sun Apr  7 09:05:42 2024, max compression
```

## Comparing `autogluon.timeseries-1.0.1b20240406.tar` & `autogluon.timeseries-1.0.1b20240407.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.628128 autogluon.timeseries-1.0.1b20240406/
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-06 09:05:30.628128 autogluon.timeseries-1.0.1b20240406/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 09:05:30.628128 autogluon.timeseries-1.0.1b20240406/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.616128 autogluon.timeseries-1.0.1b20240406/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.616128 autogluon.timeseries-1.0.1b20240406/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45567 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23391 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30977 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14873 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/npts.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/statsforecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    81011 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.628128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/lags.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/time_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.581641 autogluon.timeseries-1.0.1b20240407/
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-07 09:05:42.581641 autogluon.timeseries-1.0.1b20240407/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 09:05:42.581641 autogluon.timeseries-1.0.1b20240407/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.569640 autogluon.timeseries-1.0.1b20240407/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.569640 autogluon.timeseries-1.0.1b20240407/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.573640 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.573640 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.573640 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45567 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.577641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/metrics/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/metrics/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/metrics/quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.577641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.577641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23391 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.577641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30977 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.577641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/chronos/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/chronos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/chronos/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/chronos/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.577641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.577641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.577641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.577641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/local/npts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/local/statsforecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.581641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81222 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.581641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.581641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.581641 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/datetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/datetime/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/datetime/lags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/datetime/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/datetime/time_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-07 09:04:19.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-07 09:05:42.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:05:42.573640 autogluon.timeseries-1.0.1b20240407/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-07 09:05:42.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-07 09:05:42.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 09:05:42.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 09:05:42.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-07 09:05:42.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 09:05:42.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 09:05:42.000000 autogluon.timeseries-1.0.1b20240407/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-1.0.1b20240406/PKG-INFO` & `autogluon.timeseries-1.0.1b20240407/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.0.1b20240406
+Version: 1.0.1b20240407
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.0.1b20240406/setup.py` & `autogluon.timeseries-1.0.1b20240407/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/__init__.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/abstract.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/metrics/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/point.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/metrics/point.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/quantile.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/metrics/quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/utils.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/model.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/chronos/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,16 @@
         if self.context_length is not None and self.context_length > self.maximum_context_length:
             logger.warning(
                 f"\tContext length {self.context_length} exceeds maximum context length {self.maximum_context_length}."
                 f"Context length will be set to {self.maximum_context_length}."
             )
             self.context_length = self.maximum_context_length
 
-        model_path_safe = str.replace(model_path_input, "/", "__")
+        # we truncate the name to avoid long path errors on Windows
+        model_path_safe = str(model_path_input).replace("/", "__").replace(os.path.sep, "__")[-50:]
         name = (name if name is not None else "Chronos") + f"[{model_path_safe}]"
 
         super().__init__(
             path=path,
             freq=freq,
             prediction_length=prediction_length,
             name=name,
```

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/pipeline.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/chronos/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/npts.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/local/npts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,16 +447,16 @@
             columns with ``object`` and ``str`` dtypes as categorical features, and will ignore the rest of columns.
 
             For example, to ensure that column "store_id" with dtype ``int`` is interpreted as a category,
             we need to change its type to ``category``::
 
                 data.static_features["store_id"] = data.static_features["store_id"].astype("category")
 
-            If provided data is an instance of pandas DataFrame, AutoGluon will attempt to automatically convert it
-            to a ``TimeSeriesDataFrame``.
+            If provided data is a path or a pandas.DataFrame, AutoGluon will attempt to automatically convert it to a
+            ``TimeSeriesDataFrame``.
 
         tuning_data : Union[TimeSeriesDataFrame, pd.DataFrame, Path, str], optional
             Data reserved for model selection and hyperparameter tuning, rather than training individual models. Also
             used to compute the validation scores. Note that only the last ``prediction_length`` time steps of each
             time series are used for computing the validation score.
 
             If ``tuning_data`` is provided, multi-window backtesting on training data will be disabled, the
@@ -468,16 +468,16 @@
             If ``known_covariates_names`` were specified when creating the predictor, ``tuning_data`` must also include
             the columns listed in ``known_covariates_names`` with the covariates values aligned with the target time
             series.
 
             If ``train_data`` has past covariates or static features, ``tuning_data`` must have also include them (with
             same columns names and dtypes).
 
-            If provided data is an instance of pandas DataFrame, AutoGluon will attempt to automatically convert it
-            to a ``TimeSeriesDataFrame``.
+            If provided data is a path or a pandas.DataFrame, AutoGluon will attempt to automatically convert it to a
+            ``TimeSeriesDataFrame``.
 
         time_limit : int, optional
             Approximately how long :meth:`~autogluon.timeseries.TimeSeriesPredictor.fit` will run (wall-clock time in
             seconds). If not specified, :meth:`~autogluon.timeseries.TimeSeriesPredictor.fit` will run until all models
             have completed training.
         presets : str, optional
             Optional preset configurations for various arguments in
@@ -851,16 +851,19 @@
 
         This method measures the forecast accuracy using the last ``self.prediction_length`` time steps of each time
         series in ``data`` as a hold-out set.
 
         Parameters
         ----------
         data : Union[TimeSeriesDataFrame, pd.DataFrame, Path, str]
-            The data to evaluate the best model on. The last ``prediction_length`` time steps of the data set, for each
-            item, will be held out for prediction and forecast accuracy will be calculated on these time steps.
+            The data to evaluate the best model on. The last ``prediction_length`` time steps of each time series in
+            ``data`` will be held out for prediction and forecast accuracy will be calculated on these time steps.
+
+            Must include both historic and future data (i.e., length of all time series in ``data`` must be at least
+            ``prediction_length + 1``).
 
             If ``known_covariates_names`` were specified when creating the predictor, ``data`` must include the columns
             listed in ``known_covariates_names`` with the covariates values aligned with the target time series.
 
             If ``train_data`` used to train the predictor contained past covariates or static features, then ``data``
             must also include them (with same column names and dtypes).
 
@@ -1175,25 +1178,25 @@
         * ``fit_time_marginal``: The fit time required to train the model (ignoring base models for ensembles).
         * ``fit_order``: The order in which models were fit. The first model fit has ``fit_order=1``, and the Nth
           model fit has ``fit_order=N``.
 
         Parameters
         ----------
         data : Union[TimeSeriesDataFrame, pd.DataFrame, Path, str], optional
-            dataset used for additional evaluation. If not provided, the validation set used during training will be
-            used.
+            dataset used for additional evaluation. Must include both historic and future data (i.e., length of all
+            time series in ``data`` must be at least ``prediction_length + 1``).
 
             If ``known_covariates_names`` were specified when creating the predictor, ``data`` must include the columns
             listed in ``known_covariates_names`` with the covariates values aligned with the target time series.
 
             If ``train_data`` used to train the predictor contained past covariates or static features, then ``data``
             must also include them (with same column names and dtypes).
 
-            If provided data is an instance of pandas DataFrame, AutoGluon will attempt to automatically convert it
-            to a ``TimeSeriesDataFrame``.
+            If provided data is a path or a pandas.DataFrame, AutoGluon will attempt to automatically convert it to a
+            ``TimeSeriesDataFrame``.
 
         display : bool, default = False
             If True, the leaderboard DataFrame will be printed.
         use_cache : bool, default = True
             If True, will attempt to use the cached predictions. If False, cached predictions will be ignored.
             This argument is ignored if ``cache_predictions`` was set to False when creating the ``TimeSeriesPredictor``.
```

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/base.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/datetime/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/lags.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/datetime/lags.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/seasonality.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/datetime/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/time_features.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/datetime/time_features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-1.0.1b20240407/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-1.0.1b20240407/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.0.1b20240406
+Version: 1.0.1b20240407
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-1.0.1b20240407/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/requires.txt` & `autogluon.timeseries-1.0.1b20240407/src/autogluon.timeseries.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 networkx<4,>=3.0
 statsforecast<1.5,>=1.4.0
 mlforecast<0.10.1,>=0.10.0
 utilsforecast<0.0.11,>=0.0.10
 tqdm<5,>=4.38
 orjson~=3.9
 tensorboard<3,>=2.9
-autogluon.core[raytune]==1.0.1b20240406
-autogluon.common==1.0.1b20240406
-autogluon.tabular[catboost,lightgbm,xgboost]==1.0.1b20240406
+autogluon.core[raytune]==1.0.1b20240407
+autogluon.common==1.0.1b20240407
+autogluon.tabular[catboost,lightgbm,xgboost]==1.0.1b20240407
 
 [all]
-optimum[nncf,openvino]<1.18,>=1.17
 optimum[onnxruntime]<1.18,>=1.17
+optimum[nncf,openvino]<1.18,>=1.17
 
 [chronos-onnx]
 optimum[onnxruntime]<1.18,>=1.17
 
 [chronos-openvino]
 optimum[nncf,openvino]<1.18,>=1.17
```

