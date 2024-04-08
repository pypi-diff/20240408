# Comparing `tmp/qteasy-1.1.8.tar.gz` & `tmp/qteasy-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jackie/Projects/qteasy/dist/.tmp-gdqa728x/qteasy-1.1.8.tar", last modified: Fri Apr  5 14:24:31 2024, max compression
+gzip compressed data, was "/Users/jackie/Projects/qteasy/dist/.tmp-jvv8wh92/qteasy-1.1.9.tar", last modified: Mon Apr  8 15:19:43 2024, max compression
```

## Comparing `qteasy-1.1.8.tar` & `qteasy-1.1.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-05 14:24:31.000000 qteasy-1.1.8/
--rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.1.8/LICENSE
--rw-r--r--   0 jackie     (501) staff       (20)    27759 2024-04-05 14:24:31.000000 qteasy-1.1.8/PKG-INFO
--rwxr-xr-x   0 jackie     (501) staff       (20)    24521 2024-04-05 07:48:40.000000 qteasy-1.1.8/README.md
--rw-r--r--   0 jackie     (501) staff       (20)     2181 2024-04-05 07:48:40.000000 qteasy-1.1.8/pyproject.toml
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy/
--rwxr-xr-x   0 jackie     (501) staff       (20)     8505 2024-04-05 07:38:28.000000 qteasy-1.1.8/qteasy/__init__.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    66919 2024-04-02 02:35:24.000000 qteasy-1.1.8/qteasy/_arg_validators.py
--rw-r--r--   0 jackie     (501) staff       (20)    52929 2024-04-05 07:43:18.000000 qteasy-1.1.8/qteasy/backtest.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.1.8/qteasy/blender.py
--rw-r--r--   0 jackie     (501) staff       (20)    30242 2024-04-02 14:50:54.000000 qteasy-1.1.8/qteasy/broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   142287 2024-04-02 14:31:45.000000 qteasy-1.1.8/qteasy/built_in.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   109762 2024-04-03 15:52:24.000000 qteasy-1.1.8/qteasy/core.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   386464 2024-04-04 15:35:21.000000 qteasy-1.1.8/qteasy/database.py
--rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.1.8/qteasy/emfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34873 2024-04-05 14:06:04.000000 qteasy-1.1.8/qteasy/evaluate.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-04-05 07:19:15.000000 qteasy-1.1.8/qteasy/finance.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 12:38:58.000000 qteasy-1.1.8/qteasy/history.py
--rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.1.8/qteasy/optimization.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.1.8/qteasy/qt_operator.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:10:37.000000 qteasy-1.1.8/qteasy/space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    88152 2024-04-02 02:35:24.000000 qteasy-1.1.8/qteasy/strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   151551 2024-04-02 02:35:24.000000 qteasy-1.1.8/qteasy/tafuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)    47486 2024-04-02 02:35:24.000000 qteasy-1.1.8/qteasy/trade_recording.py
--rw-r--r--   0 jackie     (501) staff       (20)   180412 2024-04-03 15:51:09.000000 qteasy-1.1.8/qteasy/trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-04-05 13:49:08.000000 qteasy-1.1.8/qteasy/trading_util.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   140763 2024-04-02 02:35:24.000000 qteasy-1.1.8/qteasy/tsfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    75004 2024-04-03 15:52:24.000000 qteasy-1.1.8/qteasy/utilfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    79732 2024-04-03 15:51:09.000000 qteasy-1.1.8/qteasy/visual.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/
--rw-r--r--   0 jackie     (501) staff       (20)    27759 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/PKG-INFO
--rw-r--r--   0 jackie     (501) staff       (20)     1192 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/SOURCES.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/dependency_links.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.1.8/qteasy.egg-info/not-zip-safe
--rw-r--r--   0 jackie     (501) staff       (20)      154 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/requires.txt
--rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/top_level.txt
--rw-r--r--   0 jackie     (501) staff       (20)     1515 2024-04-05 14:24:31.000000 qteasy-1.1.8/setup.cfg
--rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.1.8/setup.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-05 14:24:31.000000 qteasy-1.1.8/tests/
--rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-03-29 13:24:03.000000 qteasy-1.1.8/tests/test_broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-04 02:50:52.000000 qteasy-1.1.8/tests/test_cashplan.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.1.8/tests/test_config.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.1.8/tests/test_core_sub_funcs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-04-05 07:21:23.000000 qteasy-1.1.8/tests/test_cost.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   117726 2024-04-04 13:00:13.000000 qteasy-1.1.8/tests/test_datasource.py
--rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.1.8/tests/test_eastmoney.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 13:44:14.000000 qteasy-1.1.8/tests/test_evaluations.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.1.8/tests/test_fast_experiments.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.1.8/tests/test_historypanel.py
--rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.1.8/tests/test_log.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 12:01:27.000000 qteasy-1.1.8/tests/test_loop.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-04-05 13:35:39.000000 qteasy-1.1.8/tests/test_operator_and_strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    44520 2024-04-03 15:52:24.000000 qteasy-1.1.8/tests/test_qt.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.1.8/tests/test_space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    39724 2024-03-08 14:36:48.000000 qteasy-1.1.8/tests/test_ta_funcs.py
--rw-r--r--   0 jackie     (501) staff       (20)    43391 2024-04-03 15:51:09.000000 qteasy-1.1.8/tests/test_trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    44385 2024-04-04 13:00:13.000000 qteasy-1.1.8/tests/test_trader_shell.py
--rw-r--r--   0 jackie     (501) staff       (20)   159405 2024-04-03 15:51:09.000000 qteasy-1.1.8/tests/test_trading.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.1.8/tests/test_tushare.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-04 03:20:12.000000 qteasy-1.1.8/tests/test_utilityfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.1.8/tests/test_visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-08 15:19:43.000000 qteasy-1.1.9/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.1.9/LICENSE
+-rw-r--r--   0 jackie     (501) staff       (20)    27754 2024-04-08 15:19:43.000000 qteasy-1.1.9/PKG-INFO
+-rwxr-xr-x   0 jackie     (501) staff       (20)    24516 2024-04-08 15:10:08.000000 qteasy-1.1.9/README.md
+-rw-r--r--   0 jackie     (501) staff       (20)     2181 2024-04-08 15:10:08.000000 qteasy-1.1.9/pyproject.toml
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8505 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/__init__.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    66919 2024-04-02 02:35:24.000000 qteasy-1.1.9/qteasy/_arg_validators.py
+-rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/backtest.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.1.9/qteasy/blender.py
+-rw-r--r--   0 jackie     (501) staff       (20)    30242 2024-04-02 14:50:54.000000 qteasy-1.1.9/qteasy/broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   142287 2024-04-02 14:31:45.000000 qteasy-1.1.9/qteasy/built_in.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   109762 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/core.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   386999 2024-04-08 15:18:39.000000 qteasy-1.1.9/qteasy/database.py
+-rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.1.9/qteasy/emfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/evaluate.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-04-05 14:28:39.000000 qteasy-1.1.9/qteasy/finance.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 14:28:39.000000 qteasy-1.1.9/qteasy/history.py
+-rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.1.9/qteasy/optimization.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.1.9/qteasy/qt_operator.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.1.9/qteasy/space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    88152 2024-04-02 02:35:24.000000 qteasy-1.1.9/qteasy/strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   151551 2024-04-02 02:35:24.000000 qteasy-1.1.9/qteasy/tafuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    50575 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/trade_recording.py
+-rw-r--r--   0 jackie     (501) staff       (20)   180412 2024-04-03 15:51:09.000000 qteasy-1.1.9/qteasy/trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-04-05 14:28:39.000000 qteasy-1.1.9/qteasy/trading_util.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   140763 2024-04-02 02:35:24.000000 qteasy-1.1.9/qteasy/tsfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    75004 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/utilfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/
+-rw-r--r--   0 jackie     (501) staff       (20)    27754 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/PKG-INFO
+-rw-r--r--   0 jackie     (501) staff       (20)     1192 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.1.9/qteasy.egg-info/not-zip-safe
+-rw-r--r--   0 jackie     (501) staff       (20)      154 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/requires.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/top_level.txt
+-rw-r--r--   0 jackie     (501) staff       (20)     1515 2024-04-08 15:19:43.000000 qteasy-1.1.9/setup.cfg
+-rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.1.9/setup.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-08 15:19:43.000000 qteasy-1.1.9/tests/
+-rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-03-29 13:24:03.000000 qteasy-1.1.9/tests/test_broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_cashplan.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.1.9/tests/test_config.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.1.9/tests/test_core_sub_funcs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_cost.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   121286 2024-04-08 15:18:58.000000 qteasy-1.1.9/tests/test_datasource.py
+-rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.1.9/tests/test_eastmoney.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_evaluations.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.1.9/tests/test_fast_experiments.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.1.9/tests/test_historypanel.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.1.9/tests/test_log.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_loop.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_operator_and_strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    44520 2024-04-07 13:30:44.000000 qteasy-1.1.9/tests/test_qt.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.1.9/tests/test_space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    39724 2024-03-08 14:36:48.000000 qteasy-1.1.9/tests/test_ta_funcs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    43391 2024-04-03 15:51:09.000000 qteasy-1.1.9/tests/test_trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    44385 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_trader_shell.py
+-rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-08 15:10:08.000000 qteasy-1.1.9/tests/test_trading.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.1.9/tests/test_tushare.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_utilityfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.1.9/tests/test_visual.py
```

### Comparing `qteasy-1.1.8/LICENSE` & `qteasy-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/PKG-INFO` & `qteasy-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.1.8
+Version: 1.1.9
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -92,15 +92,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.8`
+- Latest Version: `1.1.9`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -144,22 +144,22 @@
 
 ## 文档
 
 关于`QTEASY`系统的更多详细解释和使用方法，请参阅[QTEASY文档](https://qteasy.readthedocs.io)：
 
 
 ### python 版本
-- *`python` version >= 3.6, < 3.9* 
+- *`python` version >= 3.6, < 3.13* 
 
 ### 安装可选依赖包
 
 `qteasy`所有必要的依赖包都可以在pip安装的同时安装好，但如果需要使用`qteasy`的全部功能，需要安装以下依赖包：
 
-- **`ta-lib: == 0.4.18`**, 用于计算技术指标
-- **`pymysql: == 1.0.2`**, 用于连接MySQL数据库,将本地数据存储到MySQL数据库（qteasy默认使用csv文件作为本地数据源，但数据量大时推荐使用mysql数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
+- **`ta-lib`**, 以便使用所有的内置交易策略
+- **`pymysql`**, 用于连接MySQL数据库,将本地数据存储到MySQL数据库（qteasy默认使用csv文件作为本地数据源，但数据量大时推荐使用mysql数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
 
 ##  10分钟了解qteasy的功能
 
 ### 导入`qteasy`
 基本的模块导入方法如下
 
 ```python
```

### Comparing `qteasy-1.1.8/README.md` & `qteasy-1.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.8`
+- Latest Version: `1.1.9`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -94,22 +94,22 @@
 
 ## 文档
 
 关于`QTEASY`系统的更多详细解释和使用方法，请参阅[QTEASY文档](https://qteasy.readthedocs.io)：
 
 
 ### python 版本
-- *`python` version >= 3.6, < 3.9* 
+- *`python` version >= 3.6, < 3.13* 
 
 ### 安装可选依赖包
 
 `qteasy`所有必要的依赖包都可以在pip安装的同时安装好，但如果需要使用`qteasy`的全部功能，需要安装以下依赖包：
 
-- **`ta-lib: == 0.4.18`**, 用于计算技术指标
-- **`pymysql: == 1.0.2`**, 用于连接MySQL数据库,将本地数据存储到MySQL数据库（qteasy默认使用csv文件作为本地数据源，但数据量大时推荐使用mysql数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
+- **`ta-lib`**, 以便使用所有的内置交易策略
+- **`pymysql`**, 用于连接MySQL数据库,将本地数据存储到MySQL数据库（qteasy默认使用csv文件作为本地数据源，但数据量大时推荐使用mysql数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
 
 ##  10分钟了解qteasy的功能
 
 ### 导入`qteasy`
 基本的模块导入方法如下
 
 ```python
```

### Comparing `qteasy-1.1.8/pyproject.toml` & `qteasy-1.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 build-backend = "setuptools.build_meta"
 
 #[tool.setuptools.package.find]
 #where = "qteasy/"
 
 [project]
 name = "qteasy"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 maintainers = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 description = "A fast quantitative investment tool kit"
```

### Comparing `qteasy-1.1.8/qteasy/__init__.py` & `qteasy-1.1.9/qteasy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 from .built_in import built_ins, built_in_list, built_in_strategies, get_built_in_strategy
 from .visual import candle
 from .finance import CashPlan, set_cost, update_cost
 from .database import DataSource, find_history_data
 from ._arg_validators import QT_CONFIG, ConfigDict
 
 
-__version__ = '1.1.8'
+__version__ = '1.1.9'
 version_info = Namespace(
         major=1,
         minor=1,
-        patch=4,
+        patch=9,
         short=(1, 1),
-        full=(1, 1, 8),
-        string='1.1.8',
-        tuple=('1', '1', '8'),
+        full=(1, 1, 9),
+        string='1.1.9',
+        tuple=('1', '1', '9'),
         releaselevel='beta',
 )
 
 # 解析qteasy的本地安装路径
 QT_ROOT_PATH = os.path.normpath(os.path.join(os.path.dirname(__file__), os.pardir))
 QT_ROOT_PATH = os.path.join(QT_ROOT_PATH, 'qteasy/')
```

### Comparing `qteasy-1.1.8/qteasy/_arg_validators.py` & `qteasy-1.1.9/qteasy/_arg_validators.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/backtest.py` & `qteasy-1.1.9/qteasy/backtest.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #   Functions used for backtesting and
 # evaluation of trade results
 # ======================================
 
 import os
 import pandas as pd
 import numpy as np
-from numba import njit
+from numba import njit  # try taichi, which might be even faster
 
 import qteasy
 from .history import HistoryPanel
 from .finance import CashPlan, get_selling_result, get_purchase_result, get_cost_pamams
 from .qt_operator import Operator
 
 
@@ -486,18 +486,18 @@
     op_log_available_cash = []
     op_log_value = []
     op_log_matrix = []
     prev_date = 0
 
     if (op_type == 'batch') and (not trade_log):
         # batch模式下调用apply_loop_core函数:
-        looped_day_indices = list(pd.to_datetime(pd.to_datetime(looped_dates).date).astype('int'))
+        looped_day_indices = np.array(list(pd.to_datetime(pd.to_datetime(looped_dates).date).astype('int')))
         # 2, 将invset_dict处理为两个列表：invest_date_indices, invest_amount，因为invest_dict无法被Numba处理
-        investment_date_pos = list(investment_date_pos)
-        invest_amounts = list(invest_dict.values())
+        investment_date_pos = np.array(list(investment_date_pos))
+        invest_amounts = np.array(list(invest_dict.values()))
         cashes, fees, values, amounts_matrix = apply_loop_core(share_count,
                                                                looped_day_indices,
                                                                inflation_factors,
                                                                investment_date_pos,
                                                                invest_amounts,
                                                                price,
                                                                op_list,
@@ -760,16 +760,16 @@
     """
 
     # 初始化计算结果列表
     own_cash = 0.  # 持有现金总额，期初现金总额总是0，在回测过程中到现金投入日时再加入现金
     available_cash = 0.  # 每期可用现金总额
     own_amounts = np.zeros(shape=(share_count,))  # 投资组合中各个资产的持有数量，初始值为全0向量
     available_amounts = np.zeros(shape=(share_count,))  # 每期可用的资产数量
-    cash_delivery_queue = []  # 用于模拟现金交割延迟期的定长队列
-    stock_delivery_queue = []  # 用于模拟股票交割延迟期的定长队列
+    cash_delivery_queue = []  # 用于模拟现金交割延迟期的定长队列  # TODO: 使用numpy数组代替list
+    stock_delivery_queue = []  # 用于模拟股票交割延迟期的定长队列  # TODO: 使用numpy数组代替list
     signal_count = len(op_list_bt_indices)
     cashes = np.empty(shape=(signal_count,))  # 中间变量用于记录各个资产买入卖出时消耗或获得的现金
     fees = np.empty(shape=(signal_count,))  # 交易费用，记录每个操作时点产生的交易费用
     values = np.empty(shape=(signal_count,))  # 资产总价值，记录每个操作时点的资产和现金价值总和
     amounts_matrix = np.empty(shape=(signal_count, share_count))
     total_value = 0
     prev_date = 0
```

### Comparing `qteasy-1.1.8/qteasy/blender.py` & `qteasy-1.1.9/qteasy/blender.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/broker.py` & `qteasy-1.1.9/qteasy/broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/built_in.py` & `qteasy-1.1.9/qteasy/built_in.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/core.py` & `qteasy-1.1.9/qteasy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2112,15 +2112,15 @@
                 reference_data=hist_opti_ref,
         )
         # 使用how确定优化方法并生成优化后的参数和性能数据
         how = config['opti_method']
 
         # 检查numpy的版本和优化算法，当numpy版本高于1.21,优化算法为2-incremental时，使用多进程计算反而会导致效率降低（原因尚待调查）
         # TODO: 临时解决办法：
-        #  1, 当numpy版本高于1.21且算法为2-incremental时，强制禁用多进程计算，并打印warning信息
+        #  1, 当numpy版本高于1.22且算法为2-incremental时，强制禁用多进程计算，并打印warning信息
         np_version = np.__version__
         if np_version >= '1.22' and how == 2:
             import warnings
             config['parallel'] = False if config['parallel'] else config['parallel']
             msg = f'Performance Warning: the optimization algorithm 2-incremental is much slower than ' \
                   f'expected when numpy version is higher than 1.21 in parallel computing mode, ' \
                   f'the parallel computing is disabled to avoid performance degradation.'
```

### Comparing `qteasy-1.1.8/qteasy/database.py` & `qteasy-1.1.9/qteasy/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -3120,14 +3120,15 @@
         update_cols = [item for item in tbl_columns if item not in primary_key]
         if (len(df.columns) != len(tbl_columns)) or (any(i_d != i_t for i_d, i_t in zip(df.columns, tbl_columns))):
             raise KeyError(f'df columns {df.columns.to_list()} does not fit table schema {list(tbl_columns)}')
         df = df.where(pd.notna(df), None)  # fill None in Dataframe will result in filling Nan since pandas v2.0
         pd_version = pd.__version__
         if pd_version >= '2.0':
             df.replace(np.nan, None, inplace=True)
+        # df.replace(np.nan, None, inplace=True)  # fill Nan with None in pandas<2.0 will only fill previous value
         df_tuple = tuple(df.itertuples(index=False, name=None))
         sql = f"INSERT INTO "
         sql += f"`{db_table}` ("
         for col in tbl_columns[:-1]:
             sql += f"`{col}`, "
         sql += f"`{tbl_columns[-1]}`)\nVALUES\n("
         for val in tbl_columns[:-1]:
@@ -3178,15 +3179,18 @@
         -------
         int: rows affected
         """
 
         # 生成删除记录的SQL语句
         sql = f"DELETE FROM `{db_table}` WHERE "
         # 设置删除的条件
-        sql += f"`{primary_key}` IN {tuple(record_ids)}"
+        if len(record_ids) > 1:
+            sql += f"`{primary_key}` IN {tuple(record_ids)}"
+        elif len(record_ids) == 1:
+            sql += f"`{primary_key}` = {record_ids[0]}"
         import pymysql
         con = pymysql.connect(
                 host=self.host,
                 port=self.port,
                 user=self.__user__,
                 password=self.__password__,
                 db=self.db_name,
@@ -3808,15 +3812,15 @@
             raise NotImplementedError
         elif channel == 'tushare':
             # 通过tushare的API下载数据
             api_name = TABLE_MASTERS[table][TABLE_MASTER_COLUMNS.index('tushare')]
             try:
                 dnld_data = acquire_data(api_name, **kwargs)
             except Exception as e:
-                raise Exception(f'data {table} can not be acquired from tushare\n{e}')
+                raise Exception(f'{e}: data {table} can not be acquired from tushare')
         else:
             raise NotImplementedError
         res = set_primary_key_frame(dnld_data, primary_key=primary_keys, pk_dtypes=pk_dtypes)
         return res
 
     def fetch_realtime_price_data(self, table, channel, symbols):
         """ 获取分钟级实时股票价格数据，并进行内容写入前的预处理, 目前只支持下面的数据表获取实时分钟数据：
@@ -4271,15 +4275,16 @@
                   f"WHERE `TABLE_SCHEMA` = %s\n" \
                   f"AND `TABLE_NAME` = %s;"
 
             try:
                 cursor.execute(sql, (db_name, table))
                 con.commit()
                 res = cursor.fetchall()
-                return res[0][0] - 1
+                # return last id if
+                return res[0][0] - 1 if res[0][0] is not None else 1
             except Exception as e:
                 raise RuntimeError(
                     f'{e}, An error occurred when getting last record_id for table {table} with SQL:\n{sql}')
             finally:
                 con.close()
 
         else:  # for other unexpected cases
@@ -4500,15 +4505,15 @@
 
         # 插入数据
         self.update_table_data(table, df, merge_type='update')
         # TODO: 这里为什么要用'ignore'而不是'update'? 现在改为'update'，
         #  test_database和test_trading测试都能通过，后续完整测试
         return record_id
 
-    def delete_sys_table_data(self, table, record_ids) -> int:
+    def delete_sys_table_data(self, table: str, record_ids: (list, tuple)) -> int:
         """ 删除系统数据表中的某些记录，被删除的记录的ID使用列表或tuple传入
 
         parameters
         ----------
         table: str
             需要删除数据的表名
         record_ids: list of int or tuple of int
@@ -5119,17 +5124,18 @@
                     progress_bar(total, total, f'<{table}:{arg_coverage[0]}-{arg_coverage[-1]}>'
                                                f'{total_written}wrtn in {strftime_elapsed}\n')
                 else:
                     progress_bar(total, total, f'[{table}:None>'
                                                f'{total_written}wrtn in {strftime_elapsed}\n')
             except Exception as e:
                 total_written += self.update_table_data(table, dnld_data)
-                warnings.warn(f'\n{e.__class__}:{str(e)} \ndownload process interrupted at [{table}]:'
-                              f'<{arg_coverage[0]}>-<{arg_coverage[completed - 1]}>\n'
-                              f'{total_written} rows downloaded, will proceed with next table!')
+                msg = f'\n{str(e)}: \ndownload process interrupted at [{table}]:' \
+                              f'<{arg_coverage[0]}>-<{arg_coverage[completed - 1]}>\n' \
+                              f'{total_written} rows downloaded, will proceed with next table!'
+                warnings.warn(msg)
                 # progress_bar(completed, total, f'[Interrupted! {table}] <{arg_coverage[0]} to {arg_coverage[-1]}>:'
                 #                                f'{total_written} written in {sec_to_duration(time_elapsed)}\n')
 
     def get_all_basic_table_data(self, refresh_cache=False, raise_error=True):
         """ 一个快速获取所有basic数据表的函数，通常情况缓存处理以加快速度
         如果设置refresh_cache为True，则清空缓存并重新下载数据
 
@@ -5494,28 +5500,30 @@
     >>> set_primary_key_index(df, ['a'], ['int'])
     >>> df
          b
     a
     1    4
     2    5
     3    6
-
     """
 
     if not isinstance(df, pd.DataFrame):
         raise TypeError(f'df should be a pandas DataFrame, got {type(df)} instead')
     if df.empty:
         return df
     if not isinstance(primary_key, list):
         raise TypeError(f'primary key should be a list, got {type(primary_key)} instead')
     if not isinstance(pk_dtypes, list):
         raise TypeError(f'primary key should be a list, got {type(primary_key)} instead')
-    # TODO: 增加检查：primary_key中的元素是否在df.column中存，
-    #  如果不存在，df必须有index，且index.name必须存在且与primary_key中的元素一致
-    #  否则报错
+
+    all_columns = df.columns
+    if not all(item in all_columns for item in primary_key):
+        if not all(key in df.index.names for key in primary_key):
+            msg = f'primary key contains invalid value: {[item for item in primary_key if item not in all_columns]}'
+            raise KeyError(msg)
 
     idx_columns = list(df.index.names)
     pk_columns = primary_key
 
     if idx_columns != [None]:
         # index中有值，需要将index中的值放入DataFrame中
         index_frame = df.index.to_frame()
@@ -5531,15 +5539,15 @@
 
     # 设置正确的时间日期格式(找到pk_dtype中是否有"date"或"TimeStamp"类型，将相应的列设置为TimeStamp
     set_datetime_format_frame(df, primary_key, pk_dtypes)
 
     return df
 
 
-def set_datetime_format_frame(df, primary_key, pk_dtypes):
+def set_datetime_format_frame(df, primary_key: [str], pk_dtypes: [str]) -> None:
     """ 根据primary_key的rule为df的主键设置正确的时间日期类型
 
     Parameters
     ----------
     df: pd.DataFrame
         需要操作的df
     primary_key: list of str
@@ -5572,20 +5580,22 @@
                                      b
     a
     1970-01-01 00:00:00.000000001    4
     1970-01-01 00:00:00.000000002    5
     1970-01-01 00:00:00.000000003    6
 
     """
-    # 设置正确的时间日期格式(找到pk_dtype中是否有"date"或"TimeStamp"类型，将相应的列设置为TimeStamp
-    if ("date" in pk_dtypes) or ("TimeStamp" in pk_dtypes):
+    # 设置正确的时间日期格式(找到pk_dtype中是否有"date", "datetime"或"TimeStamp"类型，将相应的列设置为TimeStamp
+    datetime_dtypes = ['date', 'datetime', 'TimeStamp']
+
+    if any(dtype in pk_dtypes for dtype in datetime_dtypes):
         # 需要设置正确的时间日期格式：
         # 有时候pk会包含多列，可能有多个时间日期，因此需要逐个设置
         for pk_item, dtype in zip(primary_key, pk_dtypes):
-            if dtype in ['date', 'TimeStamp']:
+            if dtype in datetime_dtypes:
                 df[pk_item] = pd.to_datetime(df[pk_item])
     return None
 
 
 def get_primary_key_range(df, primary_key, pk_dtypes):
     """ 给定一个dataframe，给出这个df表的主键的范围，用于下载数据时用作传入参数
         如果主键类型为string，则给出一个list，包含所有的元素
```

### Comparing `qteasy-1.1.8/qteasy/emfuncs.py` & `qteasy-1.1.9/qteasy/emfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/evaluate.py` & `qteasy-1.1.9/qteasy/evaluate.py`

 * *Files 0% similar despite different names*

```diff
@@ -639,15 +639,16 @@
     looped_val['annual_rtn'] = (looped_val.rtn + 1) ** (1 / ys) - 1
     looped_val['pct_change'] = looped_val.value / looped_val.value.shift(1) - 1
     skewness = looped_val['pct_change'].skew()
     kurtosis = looped_val['pct_change'].kurtosis()
 
     first_year = looped_val.index[0].year
     last_year = looped_val.index[-1].year
-    month_freq_code = 'ME' if pd.__version__ > '2.0' else 'M'  # freq='ME' if pandas_version > 2.0
+
+    month_freq_code = 'ME' if pd.__version__ > '2.2' else 'M'  # freq='ME' if pandas_version > 2.0
     starts = pd.date_range(start=str(first_year - 1) + '1231',
                            end=str(last_year) + '1130',
                            freq=month_freq_code) + pd.Timedelta(1, 'd')
     ends = pd.date_range(start=str(first_year) + '0101',
                          end=str(last_year) + '1231',
                          freq=month_freq_code)
     # 计算每个月的收益率
@@ -662,15 +663,15 @@
     monthly_returns = np.array(monthly_returns).reshape(year_count, 12)
     monthly_return_df = pd.DataFrame(monthly_returns,
                                      columns=['Jan', 'Feb', 'Mar', 'Apr',
                                               'May', 'Jun', 'Jul', 'Aug',
                                               'Sep', 'Oct', 'Nov', 'Dec'],
                                      index=range(first_year, last_year + 1))
     # 计算每年的收益率
-    year_freq_code = 'YE' if pd.__version__ > '2.0' else 'Y'  # freq='YE' if pandas_version > 2.0
+    year_freq_code = 'YE' if pd.__version__ > '2.2' else 'Y'  # freq='YE' if pandas_version > 2.0
     starts = pd.date_range(start=str(first_year - 1) + '1231',
                            end=str(last_year) + '1130',
                            freq=year_freq_code) + pd.Timedelta(1, 'd')
     ends = pd.date_range(start=str(first_year) + '0101',
                          end=str(last_year) + '1231',
                          freq=year_freq_code)
     # 组装出月度、年度收益率矩阵
```

### Comparing `qteasy-1.1.8/qteasy/finance.py` & `qteasy-1.1.9/qteasy/finance.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/history.py` & `qteasy-1.1.9/qteasy/history.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/optimization.py` & `qteasy-1.1.9/qteasy/optimization.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/qt_operator.py` & `qteasy-1.1.9/qteasy/qt_operator.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/space.py` & `qteasy-1.1.9/qteasy/space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/strategy.py` & `qteasy-1.1.9/qteasy/strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/tafuncs.py` & `qteasy-1.1.9/qteasy/tafuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/trade_recording.py` & `qteasy-1.1.9/qteasy/trade_recording.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # TODO: add TIMEZONE to qt config arguments
 # TODO: move all secondary functions to trading_util.py
 TIMEZONE = 'Asia/Shanghai'
 
 
 # TODO: 创建一个模块级变量，用于存储交易信号的数据源，所有的交易信号都从这个数据源中读取
-#  避免交易信号从不同的数据源中获取，导致交易信号的不一致性
+#  避免交易信号从不同的数据源中获取，导致交易信号的不一致性 ?? 这是不是最好的做法？？
 # 9 foundational functions for account and position management
 def new_account(user_name, cash_amount, data_source=None, **account_data):
     """ 创建一个新的账户
 
     Parameters
     ----------
     user_name: str
@@ -196,33 +196,86 @@
             record_id=account_id,
             cash_amount=cash_amount,
             available_cash=available_cash,
             total_invest=total_investment,
     )
 
 
-def delete_account(id):
-    """ 删除账户
+def delete_account(account_id: int, data_source=None) -> None:
+    """ 删除账户，删除账户时，需要同时删除账户的持仓和交易信号。如果账户不存在，则直接返回None
+    在删除账户时，同时删除账户的持仓和交易信号，如果删除账户的持仓或交易信号失败，则会回滚删除操作
 
     Parameters
     ----------
-    id: int
+    account_id: int
         账户的id
+    data_source: DataSource, optional
+        进行操作的数据源, 默认为None, 表示使用默认的数据源
 
     Returns
     -------
     None
     """
 
-    import qteasy as qt
-    data_source = qt.QT_DATA_SOURCE
-    if not isinstance(data_source, qt.DataSource):
-        raise TypeError(f'data_source must be a DataSource instance, got {type(data_source)} instead')
-
-    raise NotImplementedError('This function is not implemented yet!')
+    if data_source is None:
+        import qteasy as qt
+        data_source = qt.QT_DATA_SOURCE
+    if not isinstance(data_source, DataSource):
+        msg = f'data_source must be a DataSource instance, got {type(data_source)} instead'
+        raise TypeError(msg)
+
+    # 检查account_id是否存在，如果不存在，则直接返回None
+    account = get_account(account_id, data_source=data_source)
+    if account is None:
+        # Nothing is deleted
+        return None
+
+    # 找出与account_id相关的所有持仓和交易订单记忆交易结果
+    positions = get_account_positions(account_id, data_source=data_source)
+    pos_ids = positions.index.tolist() if not positions.empty else []
+    orders = query_trade_orders(account_id=account_id, data_source=data_source)
+    order_ids = orders.index.tolist() if not orders.empty else []
+    results = read_trade_results_by_order_id(order_id=order_ids, data_source=data_source)
+    result_ids = results.index.tolist() if not results.empty else []
+
+    # 临时保留将要操作的完整数据表，以便回滚
+    account_table_data = data_source.read_sys_table_data('sys_op_live_accounts')
+    position_table_data = data_source.read_sys_table_data('sys_op_positions')
+    order_table_data = data_source.read_sys_table_data('sys_op_trade_orders')
+    result_table_data = data_source.read_sys_table_data('sys_op_trade_results')
+
+    # 开始删除数据：
+    print(f'Deleting account {account_id} ...')
+    print(f'Following records will be deleted: \n'
+          f'account: {account_id}\n'
+          f'positions: {pos_ids}\n'
+          f'orders: {order_ids}\n'
+          f'results: {result_ids}')
+    try:
+        # 删除账户
+        data_source.delete_sys_table_data('sys_op_live_accounts', record_ids=[account_id])
+        # 删除持仓
+        data_source.delete_sys_table_data('sys_op_positions', record_ids=pos_ids)
+        # 删除交易信号
+        data_source.delete_sys_table_data('sys_op_trade_orders', record_ids=order_ids)
+        # 删除交易结果
+        data_source.delete_sys_table_data('sys_op_trade_results', record_ids=result_ids)
+    except Exception as e:
+        # 如果删除失败，则回滚删除操作
+        data_source.drop_table_data('sys_op_live_accounts')
+        data_source.drop_table_data('sys_op_positions')
+        data_source.drop_table_data('sys_op_trade_orders')
+        data_source.drop_table_data('sys_op_trade_results')
+        data_source.write_table_data(account_table_data, 'sys_op_live_accounts')
+        data_source.write_table_data(position_table_data, 'sys_op_positions')
+        data_source.write_table_data(order_table_data, 'sys_op_trade_orders')
+        data_source.write_table_data(result_table_data, 'sys_op_trade_results')
+        import warnings
+        msg = f'Error occurred: {e}, delete account failed, rollback to previous state!'
+        warnings.warn(msg, RuntimeWarning)
 
 
 def get_position_by_id(pos_id, data_source=None):
     """ 通过pos_id获取持仓的信息
 
     Parameters
     ----------
```

### Comparing `qteasy-1.1.8/qteasy/trader.py` & `qteasy-1.1.9/qteasy/trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/trading_util.py` & `qteasy-1.1.9/qteasy/trading_util.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/tsfuncs.py` & `qteasy-1.1.9/qteasy/tsfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/qteasy/utilfuncs.py` & `qteasy-1.1.9/qteasy/utilfuncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
             while mtries > 1:
                 try:
                     return f(*args, **kwargs)
                 except exception_to_check as e:
                     # TODO: define the error to escape retry: no permission, no such file, etc.
                     exception_to_escape = [ValueError, TypeError, AttributeError, FileNotFoundError, PermissionError,]
                     error_str = str(e)
-                    if ('没有访问该接口的权限' in error_str) or ('token凭证码' in error_str):
+                    if ('没有访问该接口的权限' in error_str) or ('api init error' in error_str):
                         raise e
                     if e.__class__ in exception_to_escape:
                         raise e
                     msg = f'Error in {f.__name__}: {e.__class__}:{str(e)}, Retrying in {mdelay} seconds...'
                     if mute:
                         if logger:
                             logger.debug(msg)
```

### Comparing `qteasy-1.1.8/qteasy/visual.py` & `qteasy-1.1.9/qteasy/visual.py`

 * *Files 0% similar despite different names*

```diff
@@ -1333,14 +1333,16 @@
             ax.spines['left'].set_visible(False)
             ax.set_ylabel(f'{name}')
             ax.yaxis.tick_right()
             # 根据config中设置的参数，选择生成三种不同类型的图表之一
             p_type = config.indicator_plot_type
             # 在图表中应该舍去np.inf值，暂时将inf作为na值处理，因此可以使用dropna()去除inf值
             with pd.option_context('mode.use_inf_as_na', True):
+                # TODO: FutureWarning: use_inf_as_na option is deprecated and will be removed in a future version.
+                #  Convert inf values to NaN before operating instead.
                 opti_label = f'opti:{opti_indicator_df[name].mean():.2f}±{opti_indicator_df[name].std():.2f}'
                 test_label = f'test:{test_indicator_df[name].mean():.2f}±{test_indicator_df[name].std():.2f}'
                 opti_v = opti_indicator_df[name].fillna(np.nan)
                 test_v = test_indicator_df[name].fillna(np.nan)
                 if p_type == 0 or p_type == 'errorbar':
                     max_v = np.nanmax(opti_v)
                     min_v = np.nanmin(opti_v)
```

### Comparing `qteasy-1.1.8/qteasy.egg-info/PKG-INFO` & `qteasy-1.1.9/qteasy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.1.8
+Version: 1.1.9
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -92,15 +92,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.8`
+- Latest Version: `1.1.9`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -144,22 +144,22 @@
 
 ## 文档
 
 关于`QTEASY`系统的更多详细解释和使用方法，请参阅[QTEASY文档](https://qteasy.readthedocs.io)：
 
 
 ### python 版本
-- *`python` version >= 3.6, < 3.9* 
+- *`python` version >= 3.6, < 3.13* 
 
 ### 安装可选依赖包
 
 `qteasy`所有必要的依赖包都可以在pip安装的同时安装好，但如果需要使用`qteasy`的全部功能，需要安装以下依赖包：
 
-- **`ta-lib: == 0.4.18`**, 用于计算技术指标
-- **`pymysql: == 1.0.2`**, 用于连接MySQL数据库,将本地数据存储到MySQL数据库（qteasy默认使用csv文件作为本地数据源，但数据量大时推荐使用mysql数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
+- **`ta-lib`**, 以便使用所有的内置交易策略
+- **`pymysql`**, 用于连接MySQL数据库,将本地数据存储到MySQL数据库（qteasy默认使用csv文件作为本地数据源，但数据量大时推荐使用mysql数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
 
 ##  10分钟了解qteasy的功能
 
 ### 导入`qteasy`
 基本的模块导入方法如下
 
 ```python
```

### Comparing `qteasy-1.1.8/qteasy.egg-info/SOURCES.txt` & `qteasy-1.1.9/qteasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/setup.cfg` & `qteasy-1.1.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qteasy
-version = 1.1.8
+version = 1.1.9
 author = Jackie PENG
 author_email = jackie.pengzhao@gmail.com
 maintainer = Jackie PENG
 description = A fast quantitative investment tool kit
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shepherdpp/qteasy
```

### Comparing `qteasy-1.1.8/tests/test_broker.py` & `qteasy-1.1.9/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_cashplan.py` & `qteasy-1.1.9/tests/test_cashplan.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_config.py` & `qteasy-1.1.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_core_sub_funcs.py` & `qteasy-1.1.9/tests/test_core_sub_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_cost.py` & `qteasy-1.1.9/tests/test_cost.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_datasource.py` & `qteasy-1.1.9/tests/test_datasource.py`

 * *Files 3% similar despite different names*

```diff
@@ -1223,14 +1223,23 @@
                 df = ds.read_table_data(table)
                 print(f'df read from arr source: \n{ds.source_type}-{ds.connection_type} \nis:\n{df}')
                 self.assertEqual(df.shape[0], 3)
                 self.assertEqual(df.index[0], 1)
                 self.assertEqual(df.index[1], 3)
                 self.assertEqual(df.index[2], 5)
 
+                # delete records from the table
+                ds.delete_sys_table_data(table, record_ids=[1])
+
+                df = ds.read_table_data(table)
+                print(f'df read from arr source: \n{ds.source_type}-{ds.connection_type} \nis:\n{df}')
+                self.assertEqual(df.shape[0], 2)
+                self.assertEqual(df.index[0], 3)
+                self.assertEqual(df.index[1], 5)
+
     def test_get_history_panel_data(self):
         """ test getting arr, from real database """
         ds = qt.QT_DATA_SOURCE
         shares = ['000001.SZ', '000002.SZ', '600067.SH', '000300.SH', '518860.SH']
         htypes = 'pe, close, open, swing, strength'
         htypes = str_to_list(htypes)
         start = '20210101'
@@ -1865,14 +1874,71 @@
         self.assertEqual(freq_dither('90min', ['5min', '15min', '30min', 'd', 'w', 'm']), '30MIN')
         self.assertEqual(freq_dither('90min', ['5min', '15min', 'd', 'w', 'm']), '15MIN')
         self.assertEqual(freq_dither('t', ['5min', '15min', '30min', 'd', 'w', 'm']), '5MIN')
         self.assertEqual(freq_dither('d', ['w', 'm', 'q']), 'W')
         self.assertEqual(freq_dither('d', ['m', 'q']), 'M')
         self.assertEqual(freq_dither('m', ['5min', '15min', '30min', 'd', 'w', 'q']), 'W')
 
+    def test_manipulating_primary_keys(self):
+        """  testing functions that manipulate dataframes with their primary keys, including setting up primary keys in
+        index and columns, and resetting primary keys:
+        1. set_primary_key_frame
+        2. set_primary_key_index
+        """
+
+        df = pd.DataFrame(np.random.randint(0, 100, size=(10, 5)), columns=list('ABCDE'))
+        # test function set_primary_key_index()
+        print('test function set_primary_key_index()')
+        set_primary_key_index(df, ['A'], ['int'])
+        print(df)
+        self.assertEqual(df.index.name, 'A')
+        self.assertTrue(all(item in df.columns for item in ['B', 'C', 'D', 'E']))
+        print('set primary key to column A and type is float')
+        df = set_primary_key_frame(df, ['A'], ['int'])
+        print(df)
+        self.assertIsNone(df.index.name)
+        self.assertTrue(all(item in df.columns for item in ['A', 'B', 'C', 'D', 'E']))
+        print('set primary key to column A and B')
+        set_primary_key_index(df, ['A', 'B'], ['int', 'str'])
+        print(df)
+        self.assertEqual(df.index.names, ['A', 'B'])
+        self.assertTrue(all(item in df.columns for item in ['C', 'D', 'E']))
+        df = set_primary_key_frame(df, ['A', 'B'], [])
+        print(df)
+        print('set primary key to column A and C')
+        df = set_primary_key_frame(df, ['A', 'C'], ['float', 'str'])  # dtypes are not working here
+        print(df)
+        self.assertIsNone(df.index.name)
+        self.assertTrue(all(item in df.columns for item in ['A', 'C', 'B', 'D', 'E']))
+        self.assertEqual(df.columns[0], 'A')  # A should be the first column
+        self.assertEqual(df.columns[1], 'C')  # C should be the second column
+        self.assertEqual(df.A.dtype, 'int')
+        self.assertEqual(df.C.dtype, 'int')
+        # test function set_primary_key_frame()
+        print('test function set_primary_key_frame()')
+        print('set primary key to column A and type is datetime')
+        df = set_primary_key_frame(df, ['A'], ['datetime'])  # only datetime dtype will force type conversion
+        print(df)
+        self.assertIsNone(df.index.name)
+        self.assertTrue(all(item in df.columns for item in ['A', 'B', 'C', 'D', 'E']))
+        self.assertEqual(df.columns[0], 'A')  # A should be the first column
+        self.assertEqual(df.A.dtype, 'datetime64[ns]')
+
+        # test raises with wrong input
+        with self.assertRaises(TypeError):
+            set_primary_key_index('wrong_input', ['A'], ['int'])  # wrong input type
+            set_primary_key_frame('wrong_input', ['A'], ['int'])  # wrong input type
+            set_primary_key_index(df, 'A', ['int', 'str'])  # wrong input type
+            set_primary_key_frame(df, 'A', ['int', 'str'])  # wrong input type
+            set_primary_key_index(df, ['A'], 'int')  # wrong input type
+            set_primary_key_frame(df, ['A'], 'int')  # wrong input type
+        with self.assertRaises(KeyError):
+            set_primary_key_index(df, ['Not_in_frame'], ['int'])  # wrong input key
+            set_primary_key_frame(df, ['Not_in_frame'], ['int'])  # wrong input key
+
     def test_insert_read_sys_table_data(self):
         # 测试正常情况下写入及读取表的数据
         test_order_data = {
                     'pos_id': 1,
                     'direction': 'buy',
                     'order_type': 'limit',
                     'qty': 100,
```

### Comparing `qteasy-1.1.8/tests/test_eastmoney.py` & `qteasy-1.1.9/tests/test_eastmoney.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_evaluations.py` & `qteasy-1.1.9/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_fast_experiments.py` & `qteasy-1.1.9/tests/test_fast_experiments.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_historypanel.py` & `qteasy-1.1.9/tests/test_historypanel.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_loop.py` & `qteasy-1.1.9/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_operator_and_strategy.py` & `qteasy-1.1.9/tests/test_operator_and_strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_qt.py` & `qteasy-1.1.9/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_space.py` & `qteasy-1.1.9/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_ta_funcs.py` & `qteasy-1.1.9/tests/test_ta_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_trader.py` & `qteasy-1.1.9/tests/test_trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_trader_shell.py` & `qteasy-1.1.9/tests/test_trader_shell.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_trading.py` & `qteasy-1.1.9/tests/test_trading.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from qteasy.trade_recording import new_account, get_account, update_account, update_account_balance
 from qteasy.trade_recording import update_position, get_account_positions, get_or_create_position
 from qteasy.trade_recording import record_trade_order, update_trade_order, read_trade_order
 from qteasy.trade_recording import query_trade_orders, get_position_by_id, update_trade_result
 from qteasy.trade_recording import get_position_ids, read_trade_order_detail, save_parsed_trade_orders
 from qteasy.trade_recording import get_account_cash_availabilities, get_account_position_availabilities
 from qteasy.trade_recording import write_trade_result, get_account_position_details, read_trade_result_by_id
-from qteasy.trade_recording import read_trade_results_by_order_id
+from qteasy.trade_recording import read_trade_results_by_order_id, delete_account
 
 
 class TestTradeRecording(unittest.TestCase):
 
     def setUp(self) -> None:
         """ execute before each test"""
         from qteasy import QT_ROOT_PATH, QT_CONFIG
@@ -46,15 +46,15 @@
                 host=QT_CONFIG['test_db_host'],
                 port=QT_CONFIG['test_db_port'],
                 user=QT_CONFIG['test_db_user'],
                 password=QT_CONFIG['test_db_password'],
                 db_name=QT_CONFIG['test_db_name']
         )
         # 清空测试数据源中的所有相关表格数据
-        for table in ['sys_op_live_accounts', 'sys_op_positions', 'sys_op_trade_orders', 'sys_op_trade_orders']:
+        for table in ['sys_op_live_accounts', 'sys_op_positions', 'sys_op_trade_orders', 'sys_op_trade_results']:
             if self.test_ds.table_data_exists(table):
                 self.test_ds.drop_table_data(table)
 
     # test foundational functions related to database info read and write
     def test_create_and_get_account(self):
         """ test new_account function """
         if self.test_ds.table_data_exists('sys_op_live_accounts'):
@@ -432,41 +432,41 @@
         # writing test accounts and positions
         new_account('test_user', 100000, data_source=self.test_ds)
         get_or_create_position(1, 'AAPL', 'long', data_source=self.test_ds)
         get_or_create_position(1, 'MSFT', 'long', data_source=self.test_ds)
         get_or_create_position(1, 'GOOG', 'long', data_source=self.test_ds)
         # test recording and reading signals
         test_signal = {
-            'pos_id': 1,
-            'direction': 'buy',
-            'order_type': 'market',
-            'qty': 300,
-            'price': 10.0,
+            'pos_id':         1,
+            'direction':      'buy',
+            'order_type':     'market',
+            'qty':            300,
+            'price':          10.0,
             'submitted_time': None,
-            'status': 'created',
+            'status':         'created',
         }
         record_trade_order(test_signal, data_source=self.test_ds)
         test_signal = {
-            'pos_id': 2,
-            'direction': 'buy',
-            'order_type': 'market',
-            'qty': 200,
-            'price': 10.0,
+            'pos_id':         2,
+            'direction':      'buy',
+            'order_type':     'market',
+            'qty':            200,
+            'price':          10.0,
             'submitted_time': None,
-            'status': 'created',
+            'status':         'created',
         }
         record_trade_order(test_signal, data_source=self.test_ds)
         test_signal = {
-            'pos_id': 3,
-            'direction': 'sell',
-            'order_type': 'market',
-            'qty': 100,
-            'price': 10.0,
+            'pos_id':         3,
+            'direction':      'sell',
+            'order_type':     'market',
+            'qty':            100,
+            'price':          10.0,
             'submitted_time': None,
-            'status': 'created',
+            'status':         'created',
         }
         record_trade_order(test_signal, data_source=self.test_ds)
         signal = read_trade_order(1, data_source=self.test_ds)
         self.assertIsInstance(signal, dict)
         self.assertEqual(signal['pos_id'], 1)
         self.assertEqual(signal['direction'], 'buy')
         self.assertEqual(signal['order_type'], 'market')
@@ -493,32 +493,32 @@
         with self.assertRaises(TypeError):
             record_trade_order(None, data_source=self.test_ds)
         with self.assertRaises(TypeError):
             record_trade_order(1, data_source=self.test_ds)
         with self.assertRaises(TypeError):
             record_trade_order('test', data_source=self.test_ds)
         bad_signal = {
-            'account_id': 'a',
-            'pos_id': 'a',
-            'direction': 'buy',
-            'order_type': 'market',
-            'qty': 300,
-            'price': 10.0,
+            'account_id':     'a',
+            'pos_id':         'a',
+            'direction':      'buy',
+            'order_type':     'market',
+            'qty':            300,
+            'price':          10.0,
             'submitted_time': None,
         }
         with self.assertRaises(TypeError):
             record_trade_order(bad_signal, data_source=self.test_ds)
         bad_signal = {
             'account_id': 1,
-            'pos_id': 1,
-            'direction': 'buy',
+            'pos_id':     1,
+            'direction':  'buy',
             'order_type': 'market',
-            'qty': -300,
-            'price': -10.0,
-            'status': 'created',
+            'qty':        -300,
+            'price':      -10.0,
+            'status':     'created',
         }
         with self.assertRaises(RuntimeError):
             record_trade_order(bad_signal, data_source=self.test_ds)
         # test read signal with bad input
         # self.assertIsNone(read_trade_order(None, data_source=self.test_ds))  # will return all signals
         with self.assertRaises(TypeError):
             read_trade_order(1.0, data_source=self.test_ds)
@@ -911,15 +911,15 @@
         self.assertEqual(signal_detail['qty'], 500)
         self.assertEqual(signal_detail['price'], 50.0)
         self.assertEqual(signal_detail['status'], 'created')
         # create test positions for account 2, and add buy and sell signals for account 2
         get_or_create_position(2, 'GOOG', 'long', self.test_ds)  # pos_id = 6, qty = 1000
         get_or_create_position(2, 'FB', 'long', self.test_ds)  # pos_id = 7
         get_or_create_position(2, 'AAPL', 'long', self.test_ds)  # pos_id = 8
-        get_or_create_position(2, 'AMZN', 'long', self.test_ds)   # pos_id = 9
+        get_or_create_position(2, 'AMZN', 'long', self.test_ds)  # pos_id = 9
         get_or_create_position(2, 'MSFT', 'long', self.test_ds)  # pos_id = 10
         get_or_create_position(2, 'GOOG', 'short', self.test_ds)  # pos_id = 11
         get_or_create_position(2, 'FB', 'short', self.test_ds)  # pos_id = 12
         get_or_create_position(2, 'AAPL', 'short', self.test_ds)  # pos_id = 13
         get_or_create_position(2, 'AMZN', 'short', self.test_ds)  # pos_id = 14
         get_or_create_position(2, 'MSFT', 'short', self.test_ds)  # pos_id = 15
         # set position qty 1000 for some positions, make sure that only
@@ -1242,20 +1242,20 @@
     def test_read_and_write_result(self):
         """ test read_trade_result and write_trade_result functions """
         # 检查datasource中的数据表，删除所有的trade_result数据
         if self.test_ds.table_data_exists('sys_op_trade_results'):
             self.test_ds.drop_table_data('sys_op_trade_results')
         # 生成一个trade_result
         trade_result = {
-            'order_id': 1,
-            'filled_qty': 100.0,
-            'price': 10.0,
+            'order_id':        1,
+            'filled_qty':      100.0,
+            'price':           10.0,
             'transaction_fee': 5.0,
-            'execution_time': pd.to_datetime('now'),
-            'canceled_qty': 0.0,
+            'execution_time':  pd.to_datetime('now'),
+            'canceled_qty':    0.0,
             'delivery_amount': 100.0,
             'delivery_status': 'ND',
         }
         # 将trade_result写入datasource
         result_id = write_trade_result(trade_result, data_source=self.test_ds)
         # 从datasource中读取trade_result
         trade_result = read_trade_result_by_id(result_id, data_source=self.test_ds)
@@ -1264,32 +1264,32 @@
         self.assertEqual(trade_result['order_id'], 1)
         self.assertEqual(trade_result['filled_qty'], 100.0)
         self.assertEqual(trade_result['price'], 10.0)
         self.assertEqual(trade_result['transaction_fee'], 5.0)
         self.assertEqual(trade_result['canceled_qty'], 0.0)
         # 再次写入两个trade_results，order_id分别为1, 2，检查是否能正确读取order_id为1的两条交易结果
         trade_result = {
-            'order_id': 1,
-            'filled_qty': 200.0,
-            'price': 10.5,
+            'order_id':        1,
+            'filled_qty':      200.0,
+            'price':           10.5,
             'transaction_fee': 5.0,
-            'execution_time': pd.to_datetime('now'),
-            'canceled_qty': 0.0,
+            'execution_time':  pd.to_datetime('now'),
+            'canceled_qty':    0.0,
             'delivery_amount': 200.0,
             'delivery_status': 'ND',
         }
         result_id = write_trade_result(trade_result, data_source=self.test_ds)
         self.assertEqual(result_id, 2)
         trade_result = {
-            'order_id': 2,
-            'filled_qty': 0.0,
-            'price': 10.0,
+            'order_id':        2,
+            'filled_qty':      0.0,
+            'price':           10.0,
             'transaction_fee': 5.0,
-            'execution_time': pd.to_datetime('now'),
-            'canceled_qty': 100.0,
+            'execution_time':  pd.to_datetime('now'),
+            'canceled_qty':    100.0,
             'delivery_amount': 0.0,
             'delivery_status': 'ND',
         }
         result_id = write_trade_result(trade_result, data_source=self.test_ds)
         self.assertEqual(result_id, 3)
         trade_results = read_trade_results_by_order_id(order_id=1, data_source=self.test_ds)
         self.assertIsInstance(trade_results, pd.DataFrame)
@@ -1319,121 +1319,262 @@
             update_trade_result(1, delivery_status='Invalid Status', data_source=None)
 
         # test write_trade_result with bad input
         with self.assertRaises(TypeError):
             write_trade_result(None, data_source=self.test_ds)
         with self.assertRaises(TypeError):
             write_trade_result({
-                'order_id': '1',
-                'filled_qty': 200.0,
-                'price': 10.5,
+                'order_id':        '1',
+                'filled_qty':      200.0,
+                'price':           10.5,
                 'transaction_fee': 5.0,
-                'execution_time': pd.to_datetime('now'),
-                'canceled_qty': 0.0,
+                'execution_time':  pd.to_datetime('now'),
+                'canceled_qty':    0.0,
                 'delivery_amount': 200.0,
                 'delivery_status': 'ND',
             }, data_source=self.test_ds)
         with self.assertRaises(TypeError):
             write_trade_result({
-                'order_id': 1,
-                'filled_qty': '200.0',
-                'price': 10.5,
+                'order_id':        1,
+                'filled_qty':      '200.0',
+                'price':           10.5,
                 'transaction_fee': 5.0,
-                'execution_time': pd.to_datetime('now'),
-                'canceled_qty': 0.0,
+                'execution_time':  pd.to_datetime('now'),
+                'canceled_qty':    0.0,
             }, data_source=self.test_ds)
         with self.assertRaises(TypeError):
             write_trade_result({
-                'order_id': 1,
-                'filled_qty': 200.0,
-                'price': '10.5',
+                'order_id':        1,
+                'filled_qty':      200.0,
+                'price':           '10.5',
                 'transaction_fee': 5.0,
-                'execution_time': pd.to_datetime('now'),
-                'canceled_qty': 0.0,
+                'execution_time':  pd.to_datetime('now'),
+                'canceled_qty':    0.0,
                 'delivery_amount': 200.0,
                 'delivery_status': 'ND',
             }, data_source=self.test_ds)
         with self.assertRaises(TypeError):
             write_trade_result({
-                'order_id': 1,
-                'filled_qty': 200.0,
-                'price': 10.5,
+                'order_id':        1,
+                'filled_qty':      200.0,
+                'price':           10.5,
                 'transaction_fee': '5.0',
-                'execution_time': pd.to_datetime('now'),
-                'canceled_qty': 0.0,
+                'execution_time':  pd.to_datetime('now'),
+                'canceled_qty':    0.0,
                 'delivery_amount': 200.0,
                 'delivery_status': 'ND',
             }, data_source=self.test_ds)
         with self.assertRaises(TypeError):
             write_trade_result({
-                'order_id': 1,
-                'filled_qty': 200.0,
-                'price': 10.5,
+                'order_id':        1,
+                'filled_qty':      200.0,
+                'price':           10.5,
                 'transaction_fee': 5.0,
-                'execution_time': pd.to_datetime('now'),
-                'canceled_qty': '0.0',
+                'execution_time':  pd.to_datetime('now'),
+                'canceled_qty':    '0.0',
                 'delivery_amount': 200.0,
                 'delivery_status': 'ND',
             }, data_source=self.test_ds)
         with self.assertRaises(ValueError):
             write_trade_result({
-                'order_id': -1,
-                'filled_qty': 200.0,
-                'price': 10.5,
+                'order_id':        -1,
+                'filled_qty':      200.0,
+                'price':           10.5,
                 'transaction_fee': 5.0,
-                'execution_time': pd.to_datetime('now'),
-                'canceled_qty': 0.0,
+                'execution_time':  pd.to_datetime('now'),
+                'canceled_qty':    0.0,
                 'delivery_amount': 200.0,
                 'delivery_status': 'ND',
             }, data_source=self.test_ds)
         with self.assertRaises(ValueError):
             write_trade_result({
-                'order_id': 1,
-                'filled_qty': -200.0,
-                'price': 10.5,
+                'order_id':        1,
+                'filled_qty':      -200.0,
+                'price':           10.5,
                 'transaction_fee': 5.0,
-                'execution_time': pd.to_datetime('now'),
-                'canceled_qty': 0.0,
+                'execution_time':  pd.to_datetime('now'),
+                'canceled_qty':    0.0,
                 'delivery_amount': 200.0,
                 'delivery_status': 'ND',
             }, data_source=self.test_ds)
         with self.assertRaises(ValueError):
             write_trade_result({
-                'order_id': 1,
-                'filled_qty': 200.0,
-                'price': -10.5,
+                'order_id':        1,
+                'filled_qty':      200.0,
+                'price':           -10.5,
                 'transaction_fee': 5.0,
-                'execution_time': pd.to_datetime('now'),
-                'canceled_qty': 0.0,
+                'execution_time':  pd.to_datetime('now'),
+                'canceled_qty':    0.0,
                 'delivery_amount': 200.0,
                 'delivery_status': 'ND',
             }, data_source=self.test_ds)
         with self.assertRaises(ValueError):
             write_trade_result({
-                'order_id': 1,
-                'filled_qty': 200.0,
-                'price': 10.5,
+                'order_id':        1,
+                'filled_qty':      200.0,
+                'price':           10.5,
                 'transaction_fee': -5.0,
-                'execution_time': pd.to_datetime('now'),
-                'canceled_qty': 0.0,
+                'execution_time':  pd.to_datetime('now'),
+                'canceled_qty':    0.0,
                 'delivery_amount': 200.0,
                 'delivery_status': 'ND',
             }, data_source=self.test_ds)
         with self.assertRaises(ValueError):
             write_trade_result({
-                'order_id': 1,
-                'filled_qty': 200.0,
-                'price': 10.5,
+                'order_id':        1,
+                'filled_qty':      200.0,
+                'price':           10.5,
                 'transaction_fee': 5.0,
-                'execution_time': pd.to_datetime('now'),
-                'canceled_qty': -100.0,
+                'execution_time':  pd.to_datetime('now'),
+                'canceled_qty':    -100.0,
                 'delivery_amount': 200.0,
                 'delivery_status': 'ND',
             }, data_source=self.test_ds)
 
+    def test_delete_account(self):
+        """ test function delete_account """
+        # create and add test accounts, positions, trade orders and trade results
+        new_account('test_user1', 100000, self.test_ds)
+        new_account('test_user2', 150000, self.test_ds)
+        get_or_create_position(1, 'GOOG', 'long', data_source=self.test_ds)
+        get_or_create_position(1, 'AAPL', 'long', data_source=self.test_ds)
+        get_or_create_position(1, 'MSFT', 'long', data_source=self.test_ds)
+        get_or_create_position(1, 'AMZN', 'long', data_source=self.test_ds)
+        get_or_create_position(1, 'FB', 'long', data_source=self.test_ds)
+        get_or_create_position(2, 'GOOG', 'long', data_source=self.test_ds)
+        get_or_create_position(2, 'AAPL', 'long', data_source=self.test_ds)
+        get_or_create_position(2, 'MSFT', 'long', data_source=self.test_ds)
+        get_or_create_position(2, 'AMZN', 'long', data_source=self.test_ds)
+        get_or_create_position(2, 'FB', 'long', data_source=self.test_ds)
+        update_position(1, data_source=self.test_ds, qty_change=100, available_qty_change=100)
+        update_position(2, data_source=self.test_ds, qty_change=200, available_qty_change=200)
+        update_position(3, data_source=self.test_ds, qty_change=300, available_qty_change=300)
+        update_position(4, data_source=self.test_ds, qty_change=400, available_qty_change=400)
+        update_position(5, data_source=self.test_ds, qty_change=500, available_qty_change=500)
+        update_position(6, data_source=self.test_ds, qty_change=600, available_qty_change=600)
+        update_position(7, data_source=self.test_ds, qty_change=700, available_qty_change=700)
+        update_position(8, data_source=self.test_ds, qty_change=800, available_qty_change=800)
+        update_position(9, data_source=self.test_ds, qty_change=900, available_qty_change=900)
+        update_position(10, data_source=self.test_ds, qty_change=1000, available_qty_change=1000)
+        parsed_signals_batch_1 = (
+            ['GOOG', 'AAPL', 'MSFT', 'AMZN', 'FB', ],
+            ['long', 'long', 'long', 'long', 'long'],
+            ['buy', 'sell', 'sell', 'buy', 'buy'],
+            [100, 100, 100, 100, 100],
+            [60.0, 70.0, 80.0, 90.0, 100.0],
+        )
+        # create trade orders for account 1
+        order_ids = save_parsed_trade_orders(
+                account_id=1,
+                symbols=parsed_signals_batch_1[0],
+                positions=parsed_signals_batch_1[1],
+                directions=parsed_signals_batch_1[2],
+                quantities=parsed_signals_batch_1[3],
+                prices=parsed_signals_batch_1[4],
+                data_source=self.test_ds,
+        )
+        orders_created = query_trade_orders(account_id=1, data_source=self.test_ds)
+        print(f'orders_written: {order_ids}\norders_read: \n{orders_created}')
+        # create trade orders for account 2
+        parsed_signals_batch_2 = (
+            ['GOOG', 'AAPL', 'MSFT', 'AMZN', 'FB', ],
+            ['long', 'long', 'long', 'long', 'long'],
+            ['buy', 'sell', 'sell', 'buy', 'buy'],
+            [200, 200, 200, 200, 200],
+            [60.0, 70.0, 80.0, 90.0, 100.0],
+        )
+        order_ids = save_parsed_trade_orders(
+                account_id=2,
+                symbols=parsed_signals_batch_2[0],
+                positions=parsed_signals_batch_2[1],
+                directions=parsed_signals_batch_2[2],
+                quantities=parsed_signals_batch_2[3],
+                prices=parsed_signals_batch_2[4],
+                data_source=self.test_ds,
+        )
+        orders_created = query_trade_orders(account_id=2, data_source=self.test_ds)
+        print(f'orders_written: {order_ids}\norders_read: \n{orders_created}')
+        # create trade results for account 1
+        trade_result = {
+            'order_id':        1,
+            'filled_qty':      100.0,
+            'price':           10.0,
+            'transaction_fee': 5.0,
+            'execution_time':  pd.to_datetime('now'),
+            'canceled_qty':    0.0,
+            'delivery_amount': 100.0,
+            'delivery_status': 'ND',
+        }
+        # 将trade_result写入datasource
+        result_id = write_trade_result(trade_result, data_source=self.test_ds)
+        trade_result = {
+            'order_id':        2,
+            'filled_qty':      200.0,
+            'price':           10.5,
+            'transaction_fee': 5.0,
+            'execution_time':  pd.to_datetime('now'),
+            'canceled_qty':    0.0,
+            'delivery_amount': 200.0,
+            'delivery_status': 'ND',
+        }
+        result_id = write_trade_result(trade_result, data_source=self.test_ds)
+        # create trade results for account 2
+        trade_result = {
+            'order_id':        6,
+            'filled_qty':      200.0,
+            'price':           10.0,
+            'transaction_fee': 5.0,
+            'execution_time':  pd.to_datetime('now'),
+            'canceled_qty':    0.0,
+            'delivery_amount': 300.0,
+            'delivery_status': 'ND',
+        }
+        result_id = write_trade_result(trade_result, data_source=self.test_ds)
+        trade_result = {
+            'order_id':        7,
+            'filled_qty':      200.0,
+            'price':           10.5,
+            'transaction_fee': 5.0,
+            'execution_time':  pd.to_datetime('now'),
+            'canceled_qty':    0.0,
+            'delivery_amount': 400.0,
+            'delivery_status': 'ND',
+        }
+        result_id = write_trade_result(trade_result, data_source=self.test_ds)
+        # read all data from tables and print to check
+        print(f'before deleting:')
+        accounts = self.test_ds.read_sys_table_data('sys_op_live_accounts')
+        positions = self.test_ds.read_sys_table_data('sys_op_positions')
+        orders = self.test_ds.read_sys_table_data('sys_op_trade_orders')
+        results = self.test_ds.read_sys_table_data('sys_op_trade_results')
+        print(f'accounts: \n{accounts}\npositions: \n{positions}\norders: \n{orders}\nresults: \n{results}')
+        self.assertEqual(accounts.index.to_list(), [1, 2])
+        self.assertEqual(positions.index.to_list(), [1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
+        self.assertEqual(orders.index.to_list(), [1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
+        self.assertEqual(results.index.to_list(), [1, 2, 3, 4])
+        # delete account 2
+        delete_account(2, data_source=self.test_ds)
+        # read all data from tables and print to check
+        print(f'after deleting:')
+        accounts = self.test_ds.read_sys_table_data('sys_op_live_accounts')
+        positions = self.test_ds.read_sys_table_data('sys_op_positions')
+        orders = self.test_ds.read_sys_table_data('sys_op_trade_orders')
+        results = self.test_ds.read_sys_table_data('sys_op_trade_results')
+        print(f'accounts: \n{accounts}\npositions: \n{positions}\norders: \n{orders}\nresults: \n{results}')
+        self.assertEqual(accounts.index.to_list(), [1])
+        self.assertEqual(positions.index.to_list(), [1, 2, 3, 4, 5])
+        self.assertEqual(orders.index.to_list(), [1, 2, 3, 4, 5])
+        self.assertEqual(results.index.to_list(), [1, 2])
+        # test fail to delete account with bad input
+        with self.assertRaises(TypeError):
+            delete_account('1', data_source=self.test_ds)
+            delete_account(None, data_source=self.test_ds)
+            delete_account(1, data_source='not_a_datasource')
+            delete_account(-1, data_source=self.test_ds)
+            delete_account(3, data_source=self.test_ds)
 
 class TestTradingUtilFuncs(unittest.TestCase):
     """ test trading util funcs """
 
     def setUp(self):
         """ execute before each test"""
         from qteasy import QT_ROOT_PATH, QT_CONFIG
@@ -1459,21 +1600,21 @@
         """ test function create_daily_task_schedule """
         # test create daily task agenda with only one strategy, run_freq='d', run_timing='close'
         op = qt.Operator(strategies='macd')
         stg = op.strategies[0]
         self.assertEqual(stg.strategy_run_freq, 'd')
         self.assertEqual(stg.strategy_run_timing, 'close')
         config = {
-            'market_open_time_am': '09:30:00',
-            'market_close_time_pm': '15:30:00',
-            'market_open_time_pm': '13:00:00',
-            'market_close_time_am': '11:30:00',
-            'exchange': 'SSE',
+            'market_open_time_am':               '09:30:00',
+            'market_close_time_pm':              '15:30:00',
+            'market_open_time_pm':               '13:00:00',
+            'market_close_time_am':              '11:30:00',
+            'exchange':                          'SSE',
             'strategy_open_close_timing_offset': 1,
-            'live_price_acquire_freq': '15min',
+            'live_price_acquire_freq':           '15min',
         }
         agenda = create_daily_task_schedule(op, config)
         print(f'agenda: {agenda}')
         self.assertIsInstance(agenda, list)
         self.assertEqual(len(agenda), 25)
         self.assertEqual(agenda[0], ('09:15:00', 'pre_open'))
         self.assertEqual(agenda[1], ('09:30:00', 'open_market'))
@@ -1491,21 +1632,21 @@
 
         # test create daily task agenda with only one strategy, run_freq='h', run_timing='open'
         op = qt.Operator(strategies='macd')
         stg = op.strategies[0]
         stg.strategy_run_freq = 'h'
         stg.strategy_run_timing = 'open'
         config = {
-            'market_open_time_am': '09:30:00',
-            'market_close_time_pm': '15:30:00',
-            'market_open_time_pm': '13:00:00',
-            'market_close_time_am': '11:30:00',
-            'exchange': 'SSE',
+            'market_open_time_am':               '09:30:00',
+            'market_close_time_pm':              '15:30:00',
+            'market_open_time_pm':               '13:00:00',
+            'market_close_time_am':              '11:30:00',
+            'exchange':                          'SSE',
             'strategy_open_close_timing_offset': 1,
-            'live_price_acquire_freq': '15min',
+            'live_price_acquire_freq':           '15min',
         }
         agenda = create_daily_task_schedule(op, config)
         print(f'agenda: {agenda}')
         self.assertIsInstance(agenda, list)
         self.assertEqual(len(agenda), 29)
         self.assertEqual(agenda[0], ('09:15:00', 'pre_open'))
         self.assertEqual(agenda[1], ('09:30:00', 'open_market'))
@@ -1529,21 +1670,21 @@
         stg = op.strategies[1]
         stg.strategy_run_freq = '30min'
         stg.strategy_run_timing = 'open'
         stg = op.strategies[2]
         stg.strategy_run_freq = 'd'
         stg.strategy_run_timing = '10:30'
         config = {
-            'market_open_time_am': '09:30:00',
-            'market_close_time_pm': '15:30:00',
-            'market_open_time_pm': '13:00:00',
-            'market_close_time_am': '11:30:00',
-            'exchange': 'SSE',
+            'market_open_time_am':               '09:30:00',
+            'market_close_time_pm':              '15:30:00',
+            'market_open_time_pm':               '13:00:00',
+            'market_close_time_am':              '11:30:00',
+            'exchange':                          'SSE',
             'strategy_open_close_timing_offset': 1,
-            'live_price_acquire_freq': '60min',
+            'live_price_acquire_freq':           '60min',
         }
         agenda = create_daily_task_schedule(op, config)
         print(f'agenda: {agenda}')
         self.assertIsInstance(agenda, list)
         self.assertEqual(len(agenda), 21)
         self.assertEqual(agenda[0], ('09:15:00', 'pre_open'))
         self.assertEqual(agenda[1], ('09:30:00', 'open_market'))
@@ -1581,15 +1722,15 @@
             self.test_ds.drop_table_data('sys_op_positions')
         if self.test_ds.table_data_exists('sys_op_trade_orders'):
             self.test_ds.drop_table_data('sys_op_trade_orders')
         if self.test_ds.table_data_exists('sys_op_trade_results'):
             self.test_ds.drop_table_data('sys_op_trade_results')
         # 重新创建account及trade_signal数据, position会在submit_signal中自动创建
         delivery_config = {
-            'cash_delivery_period': 0,
+            'cash_delivery_period':  0,
             'stock_delivery_period': 0,
         }
         # create test accounts
         new_account('test_user1', 100000, self.test_ds)
         # create test trade signals
         # create test signals, all signals are buy signals, because the test starts with zero positions
         parsed_signals_batch_1 = (
@@ -1662,19 +1803,19 @@
         self.assertEqual(summary[0], ['GOOG', 'AMZN', 'TSLA', ])
         self.assertEqual(list(summary[1]), [0, 0, 0])
         self.assertEqual(list(summary[2]), [0, 0, 0])
 
         # 生成交易结果并逐个处理, 注意raw_results没有execution_time字段
         # signal 1 is filled with 100 shares at 60.5, transaction fee is 5.0
         raw_trade_result = {
-            'order_id': 1,
-            'filled_qty': 100,
-            'price': 60.5,
+            'order_id':        1,
+            'filled_qty':      100,
+            'price':           60.5,
             'transaction_fee': 5.0,
-            'canceled_qty': 0.0,
+            'canceled_qty':    0.0,
         }
         print(f'\n------------START PROCESS TRADE RESULT-----------------\n'
               f'before processing trade result 1, trade signal: \n'
               f'{read_trade_order_detail(1, data_source=self.test_ds)}\n')
         process_account_delivery(account_id=1, data_source=self.test_ds, config=delivery_config)
         process_trade_result(raw_trade_result, data_source=self.test_ds, config=delivery_config)
         print(f'after processing trade result 1, position data of account_id == 1: \n'
@@ -1717,19 +1858,19 @@
         print(f'last trade result summary of account_id == 1 with shares ["GOOG", "AAPL", "AMZN"]: \n{summary}')
         self.assertEqual(summary[0], ['AAPL', 'GOOG', 'AMZN'])
         self.assertEqual(list(summary[1]), [0, 100, 0])
         self.assertEqual(list(summary[2]), [0, 60.5, 0])
 
         # order 2 is canceled with no transaction fee
         raw_trade_result = {
-            'order_id': 2,
-            'filled_qty': 0,
-            'price': 0.0,
+            'order_id':        2,
+            'filled_qty':      0,
+            'price':           0.0,
             'transaction_fee': 0.0,
-            'canceled_qty': 100.0,
+            'canceled_qty':    100.0,
         }
         print(f'\n------------START PROCESS TRADE RESULT-----------------\n'
               f'before processing trade result 2, trade signal: \n'
               f'{read_trade_order_detail(2, data_source=self.test_ds)}\n')
         process_account_delivery(account_id=1, data_source=self.test_ds, config=delivery_config)
         process_trade_result(raw_trade_result, data_source=self.test_ds, config=delivery_config)
         print(f'after processing trade result 2, position data of account_id == 1: \n'
@@ -1778,19 +1919,19 @@
         print(f'last trade result summary of account_id == 1 with shares ["GOOG", "AAPL", "AMZN", "FB"]: \n{summary}')
         self.assertEqual(summary[0], ['AAPL', 'GOOG', 'AMZN', 'FB'])
         self.assertEqual(list(summary[1]), [0, 100, 0, 0])
         self.assertEqual(list(summary[2]), [0, 60.5, 0, 0])
 
         # signal 3 is partially filled with 100 shares bought at 81, with transaction fee 12.5
         raw_trade_result = {
-            'order_id': 3,
-            'filled_qty': 100.0,
-            'price': 81.0,
+            'order_id':        3,
+            'filled_qty':      100.0,
+            'price':           81.0,
             'transaction_fee': 12.5,
-            'canceled_qty': 0.0,
+            'canceled_qty':    0.0,
         }
         print(f'\n------------START PROCESS TRADE RESULT-----------------\n'
               f'before processing trade result 3, trade signal: \n'
               f'{read_trade_order_detail(3, data_source=self.test_ds)}\n')
         process_account_delivery(account_id=1, data_source=self.test_ds, config=delivery_config)
         process_trade_result(raw_trade_result, data_source=self.test_ds, config=delivery_config)
         print(f'after processing trade result 3, position data of account_id == 1: \n'
@@ -1839,19 +1980,19 @@
         print(f'last trade result summary of account_id == 1 with shares ["GOOG", "AAPL", "MSFT", "FB"]: \n{summary}')
         self.assertEqual(summary[0], ['AAPL', 'GOOG', 'MSFT', 'FB'])
         self.assertEqual(list(summary[1]), [0, 100, 100, 0])
         self.assertEqual(list(summary[2]), [0, 60.5, 81, 0])
 
         # signal 4 is filled with 400 shares bought at 89.5, with transaction fee 7.5
         raw_trade_result = {
-            'order_id': 4,
-            'filled_qty': 400.0,
-            'price': 89.5,
+            'order_id':        4,
+            'filled_qty':      400.0,
+            'price':           89.5,
             'transaction_fee': 7.5,
-            'canceled_qty': 0.0,
+            'canceled_qty':    0.0,
         }
         print(f'\n------------START PROCESS TRADE RESULT-----------------\n'
               f'before processing trade result 4, trade signal: \n'
               f'{read_trade_order_detail(4, data_source=self.test_ds)}\n')
         process_account_delivery(account_id=1, data_source=self.test_ds, config=delivery_config)
         process_trade_result(raw_trade_result, data_source=self.test_ds, config=delivery_config)
         print(f'after processing trade result 4, position data of account_id == 1: \n'
@@ -1925,19 +2066,19 @@
         self.assertIsNone(submit_order(1, data_source=self.test_ds))
         self.assertEqual(submit_order(6, data_source=self.test_ds), 6)
         self.assertEqual(submit_order(7, data_source=self.test_ds), 7)
         self.assertEqual(submit_order(9, data_source=self.test_ds), 9)
 
         # signal 7 is filled with 100 shares sold at 90.0, with transaction fee 5.5
         raw_trade_result = {
-            'order_id': 7,
-            'filled_qty': 100.0,
-            'price': 90.0,
+            'order_id':        7,
+            'filled_qty':      100.0,
+            'price':           90.0,
             'transaction_fee': 5.5,
-            'canceled_qty': 0.0,
+            'canceled_qty':    0.0,
         }
         print(f'\n------------START PROCESS TRADE RESULT-----------------\n'
               f'before processing trade result 7, trade signal: \n'
               f'{read_trade_order_detail(7, data_source=self.test_ds)}\n')
         process_account_delivery(account_id=1, data_source=self.test_ds, config=delivery_config)
         process_trade_result(raw_trade_result, data_source=self.test_ds, config=delivery_config)
         print(f'after processing trade result 7, position data of account_id == 1: \n'
@@ -1947,15 +2088,16 @@
               f'trade_signal_detail of order_id == 7: \n'
               f'{read_trade_order_detail(7, data_source=self.test_ds)}\n'
               f'trade_result_detail of order_id == 7: \n'
               f'{read_trade_results_by_order_id(7, data_source=self.test_ds).loc[5].to_dict()}')
         trade_result = read_trade_result_by_id(5, data_source=self.test_ds)
         # check cash availability
         own_cash, available_cash, total_invest = get_account_cash_availabilities(1, data_source=self.test_ds)
-        self.assertEqual(own_cash, 100000.0 - 100 * 60.5 - 5.0 - 100 * 81.0 - 12.5 - 400 * 89.5 - 7.5 + 100 * 90.0 - 5.5)
+        self.assertEqual(own_cash,
+                         100000.0 - 100 * 60.5 - 5.0 - 100 * 81.0 - 12.5 - 400 * 89.5 - 7.5 + 100 * 90.0 - 5.5)
         self.assertEqual(available_cash, 100000.0 - 100 * 60.5 - 5.0 - 100 * 81.0 - 12.5 - 400 * 89.5 - 7.5)
         self.assertAlmostEqual(total_invest, 100000.0)
         trade_signal_detail = read_trade_order_detail(7, data_source=self.test_ds)
         # check available qty availability
         symbols, own_qty, available_qty, costs = get_account_position_availabilities(
                 1,
                 trade_signal_detail['symbol'],
@@ -1986,19 +2128,19 @@
         print(f'last trade result summary of account_id == 1 with shares ["GOOG", "AAPL", "MSFT", "FB"]: \n{summary}')
         self.assertEqual(summary[0], ['AAPL', 'GOOG', 'MSFT', 'FB'])
         self.assertEqual(list(summary[1]), [0, -100, 100, 0])
         self.assertEqual(list(summary[2]), [0, 90, 81, 0])
 
         # signal 9 is partially filled with 300 shares sold at 140.0, with transaction fee 65.3
         raw_trade_result = {
-            'order_id': 9,
-            'filled_qty': 300.0,
-            'price': 140.0,
+            'order_id':        9,
+            'filled_qty':      300.0,
+            'price':           140.0,
             'transaction_fee': 65.3,
-            'canceled_qty': 0.0,
+            'canceled_qty':    0.0,
         }
         print(f'\n------------START PROCESS TRADE RESULT-----------------\n'
               f'before processing trade result 9, trade signal: \n'
               f'{read_trade_order_detail(9, data_source=self.test_ds)}\n')
         process_account_delivery(account_id=1, data_source=self.test_ds, config=delivery_config)
         process_trade_result(raw_trade_result, data_source=self.test_ds, config=delivery_config)
         print(f'after processing trade result 9, position data of account_id == 1: \n'
@@ -2047,15 +2189,15 @@
         print(f'last trade result summary of account_id == 1 with shares ["GOOG", "AAPL", "MSFT", "FB"]: \n{summary}')
         self.assertEqual(summary[0], ['AAPL', 'GOOG', 'MSFT', 'FB'])
         self.assertEqual(list(summary[1]), [0, -100, 100, 0])
         self.assertEqual(list(summary[2]), [0, 90, 81, 0])
 
         # partially filled order 9 with 99 shares sold at 191.0, with transaction fee 23.9
         raw_trade_result = {
-            'order_id':       9,
+            'order_id':        9,
             'filled_qty':      99.0,
             'price':           191.0,
             'transaction_fee': 23.9,
             'canceled_qty':    0.0,
         }
         process_account_delivery(account_id=1, data_source=self.test_ds, config=delivery_config)
         process_trade_result(raw_trade_result, data_source=self.test_ds, config=delivery_config)
@@ -2146,184 +2288,184 @@
         shares = ['000001', '000002', '000003']
         prices = np.array([20., 20., 20.])
         own_shares = np.array([500., 500., 1000.])
         own_cash = 100000.0
         available_amounts = np.array([500., 500., 1000.])
         available_cash = 100000.0
         test_config = {
-            'PT_buy_threshold': 0.0,
+            'PT_buy_threshold':  0.0,
             'PT_sell_threshold': 0.0,
-            'allow_sell_short': True,
-            'trade_batch_size': 100.,
-            'sell_batch_size': 1.,
+            'allow_sell_short':  True,
+            'trade_batch_size':  100.,
+            'sell_batch_size':   1.,
         }
         # create test data for PT signal and parse it
         pt_signal = np.array([0.1, 0.1, 0.1])
         parsed_signal_elements = parse_trade_signal(
-            signals=pt_signal,
-            signal_type='pt',
-            shares=shares,
-            prices=prices,
-            own_amounts=own_shares,
-            own_cash=own_cash,
-            available_amounts=available_amounts,
-            available_cash=available_cash,
-            config=test_config,
+                signals=pt_signal,
+                signal_type='pt',
+                shares=shares,
+                prices=prices,
+                own_amounts=own_shares,
+                own_cash=own_cash,
+                available_amounts=available_amounts,
+                available_cash=available_cash,
+                config=test_config,
         )
         print(f'parsed_signal_elements with signal {pt_signal}: \n{parsed_signal_elements}')
         self.assertEqual(parsed_signal_elements[0], ['000001', '000002', '000003'])
         self.assertEqual(parsed_signal_elements[1], ['long', 'long', 'long'])
         self.assertEqual(parsed_signal_elements[2], ['buy', 'buy', 'sell'])
         self.assertEqual(parsed_signal_elements[3], [200.0, 200.0, 300.0])
         pt_signal = np.array([-0.1, 0.2, 0.3])
         parsed_signal_elements = parse_trade_signal(
-            signals=pt_signal,
-            signal_type='pt',
-            shares=shares,
-            prices=prices,
-            own_amounts=own_shares,
-            own_cash=own_cash,
-            available_amounts=available_amounts,
-            available_cash=available_cash,
-            config=test_config,
+                signals=pt_signal,
+                signal_type='pt',
+                shares=shares,
+                prices=prices,
+                own_amounts=own_shares,
+                own_cash=own_cash,
+                available_amounts=available_amounts,
+                available_cash=available_cash,
+                config=test_config,
         )
         print(f'parsed_signal_elements with signal {pt_signal}: \n{parsed_signal_elements}')
         self.assertEqual(parsed_signal_elements[0], ['000001', '000001', '000002', '000003'])
         self.assertEqual(parsed_signal_elements[1], ['long', 'short', 'long', 'long'])
         self.assertEqual(parsed_signal_elements[2], ['sell', 'buy', 'buy', 'buy'])
         self.assertEqual(parsed_signal_elements[3], [500.0, 700.0, 900.0, 1100.0])
 
         # create test data for PS signal and parse it
         ps_signal = np.array([0.1, 0.1, 0.1])
         parsed_signal_elements = parse_trade_signal(
-            signals=ps_signal,
-            signal_type='ps',
-            shares=shares,
-            prices=prices,
-            own_amounts=own_shares,
-            own_cash=own_cash,
-            available_amounts=available_amounts,
-            available_cash=available_cash,
-            config=test_config,
+                signals=ps_signal,
+                signal_type='ps',
+                shares=shares,
+                prices=prices,
+                own_amounts=own_shares,
+                own_cash=own_cash,
+                available_amounts=available_amounts,
+                available_cash=available_cash,
+                config=test_config,
         )
         print(f'parsed_signal_elements with ps signal {ps_signal}: \n{parsed_signal_elements}')
         self.assertEqual(parsed_signal_elements[0], ['000001', '000002', '000003'])
         self.assertEqual(parsed_signal_elements[1], ['long', 'long', 'long'])
         self.assertEqual(parsed_signal_elements[2], ['buy', 'buy', 'buy'])
         self.assertEqual(parsed_signal_elements[3], [700.0, 700.0, 700.0])
         ps_signal = np.array([-1.5, -1, 0.3])
         parsed_signal_elements = parse_trade_signal(
-            signals=ps_signal,
-            signal_type='ps',
-            shares=shares,
-            prices=prices,
-            own_amounts=own_shares,
-            own_cash=own_cash,
-            available_amounts=available_amounts,
-            available_cash=available_cash,
-            config=test_config,
+                signals=ps_signal,
+                signal_type='ps',
+                shares=shares,
+                prices=prices,
+                own_amounts=own_shares,
+                own_cash=own_cash,
+                available_amounts=available_amounts,
+                available_cash=available_cash,
+                config=test_config,
         )
         print(f'parsed_signal_elements with ps signal {ps_signal}: \n{parsed_signal_elements}')
         self.assertEqual(parsed_signal_elements[0], ['000001', '000001', '000002', '000003'])
         self.assertEqual(parsed_signal_elements[1], ['long', 'short', 'long', 'long'])
         self.assertEqual(parsed_signal_elements[2], ['sell', 'buy', 'sell', 'buy'])
         self.assertEqual(parsed_signal_elements[3], [500.0, 250.0, 500.0, 2100.0])
 
         # create test data for VS signal and parse it
         vs_signal = np.array([300, 400, 500])
         parsed_signal_elements = parse_trade_signal(
-            signals=vs_signal,
-            signal_type='vs',
-            shares=shares,
-            prices=prices,
-            own_amounts=own_shares,
-            own_cash=own_cash,
-            available_amounts=available_amounts,
-            available_cash=available_cash,
-            config=test_config,
+                signals=vs_signal,
+                signal_type='vs',
+                shares=shares,
+                prices=prices,
+                own_amounts=own_shares,
+                own_cash=own_cash,
+                available_amounts=available_amounts,
+                available_cash=available_cash,
+                config=test_config,
         )
         print(f'parsed_signal_elements with vs signal {vs_signal}: \n{parsed_signal_elements}')
         self.assertEqual(parsed_signal_elements[0], ['000001', '000002', '000003'])
         self.assertEqual(parsed_signal_elements[1], ['long', 'long', 'long'])
         self.assertEqual(parsed_signal_elements[2], ['buy', 'buy', 'buy'])
         self.assertEqual(parsed_signal_elements[3], [300.0, 400.0, 500.0])
         vs_signal = np.array([-1300, 400, -500])
         parsed_signal_elements = parse_trade_signal(
-            signals=vs_signal,
-            signal_type='vs',
-            shares=shares,
-            prices=prices,
-            own_amounts=own_shares,
-            own_cash=own_cash,
-            available_amounts=available_amounts,
-            available_cash=available_cash,
-            config=test_config,
+                signals=vs_signal,
+                signal_type='vs',
+                shares=shares,
+                prices=prices,
+                own_amounts=own_shares,
+                own_cash=own_cash,
+                available_amounts=available_amounts,
+                available_cash=available_cash,
+                config=test_config,
         )
         print(f'parsed_signal_elements with vs signal {vs_signal}: \n{parsed_signal_elements}')
         self.assertEqual(parsed_signal_elements[0], ['000001', '000001', '000002', '000003'])
         self.assertEqual(parsed_signal_elements[1], ['long', 'short', 'long', 'long'])
         self.assertEqual(parsed_signal_elements[2], ['sell', 'buy', 'buy', 'sell'])
         self.assertEqual(parsed_signal_elements[3], [500.0, 800.0, 400.0, 500.0])
 
         # test allow_sell_short = False
         test_config = {
-            'PT_buy_threshold': 0.1,
+            'PT_buy_threshold':  0.1,
             'PT_sell_threshold': -0.1,
-            'allow_sell_short': False,
-            'trade_batch_size': 0.,
-            'sell_batch_size': 0.,
+            'allow_sell_short':  False,
+            'trade_batch_size':  0.,
+            'sell_batch_size':   0.,
         }
         # test pt signal previously used
         pt_signal = np.array([-0.1, 0.2, 0.3])
         parsed_signal_elements = parse_trade_signal(
-            signals=pt_signal,
-            signal_type='pt',
-            shares=shares,
-            prices=prices,
-            own_amounts=own_shares,
-            own_cash=own_cash,
-            available_amounts=available_amounts,
-            available_cash=available_cash,
-            config=test_config,
+                signals=pt_signal,
+                signal_type='pt',
+                shares=shares,
+                prices=prices,
+                own_amounts=own_shares,
+                own_cash=own_cash,
+                available_amounts=available_amounts,
+                available_cash=available_cash,
+                config=test_config,
         )
         print(f'parsed_signal_elements with signal {pt_signal} not allow short: \n{parsed_signal_elements}')
         self.assertEqual(parsed_signal_elements[0], ['000001', '000002', '000003'])
         self.assertEqual(parsed_signal_elements[1], ['long', 'long', 'long'])
         self.assertEqual(parsed_signal_elements[2], ['sell', 'buy', 'buy'])
         self.assertEqual(parsed_signal_elements[3], [500.0, 900.0, 1100.0])
         # test ps signal previously used
         ps_signal = np.array([-1.5, -1, 0.3])
         parsed_signal_elements = parse_trade_signal(
-            signals=ps_signal,
-            signal_type='ps',
-            shares=shares,
-            prices=prices,
-            own_amounts=own_shares,
-            own_cash=own_cash,
-            available_amounts=available_amounts,
-            available_cash=available_cash,
-            config=test_config,
+                signals=ps_signal,
+                signal_type='ps',
+                shares=shares,
+                prices=prices,
+                own_amounts=own_shares,
+                own_cash=own_cash,
+                available_amounts=available_amounts,
+                available_cash=available_cash,
+                config=test_config,
         )
         print(f'parsed_signal_elements with signal {ps_signal} not allow short: \n{parsed_signal_elements}')
         self.assertEqual(parsed_signal_elements[0], ['000001', '000002', '000003'])
         self.assertEqual(parsed_signal_elements[1], ['long', 'long', 'long'])
         self.assertEqual(parsed_signal_elements[2], ['sell', 'sell', 'buy'])
         self.assertEqual(parsed_signal_elements[3], [500.0, 500.0, 2100.0])
         # test vs signal previously used
         vs_signal = np.array([-1300, 400, -500])
         parsed_signal_elements = parse_trade_signal(
-            signals=vs_signal,
-            signal_type='vs',
-            shares=shares,
-            prices=prices,
-            own_amounts=own_shares,
-            own_cash=own_cash,
-            available_amounts=available_amounts,
-            available_cash=available_cash,
-            config=test_config,
+                signals=vs_signal,
+                signal_type='vs',
+                shares=shares,
+                prices=prices,
+                own_amounts=own_shares,
+                own_cash=own_cash,
+                available_amounts=available_amounts,
+                available_cash=available_cash,
+                config=test_config,
         )
         print(f'parsed_signal_elements with vs signal {vs_signal} not allow short: \n{parsed_signal_elements}')
         self.assertEqual(parsed_signal_elements[0], ['000001', '000002', '000003'])
         self.assertEqual(parsed_signal_elements[1], ['long', 'long', 'long'])
         self.assertEqual(parsed_signal_elements[2], ['sell', 'buy', 'sell'])
         self.assertEqual(parsed_signal_elements[3], [500.0, 400.0, 500.0])
 
@@ -2849,51 +2991,52 @@
 
         # TODO: 此处手动添加所需要的数据，避免从网上下载导致测试失败
         # self.test_ds.refill_local_source(
         #         tables='stock_basic, index_basic',
         #         parallel=False,
         # )
         stock_basic_df = pd.DataFrame({
-            'ts_code': ['000001.SZ', '000002.SZ', '000004.SZ', '600251.SH', '000006.SZ', '000008.SZ'],
-            'symbol': ['000001', '000002', '000004', '600251', '000006', '000008'],
-            'name': ['平安银行', '万科A', '国华网安', '冠农股份', '深振业A', '神州高铁'],
-            'area': ['深圳', '深圳', '深圳', '深圳', '深圳', '深圳'],
-            'industry': ['银行', '全国地产', '软件服务', '农药化肥', '区域地产', '其他商业'],
-            'full_name': ['平安银行', '万科A', '国华网安', '冠农股份', '深振业A', '神州高铁'],
-            'en_name': ['Ping An Bank', 'Vanke A', 'Guohua Network Security', 'Guannong Shares', 'Shenzhen Zhenye A', 'Shenzhou High Speed Railway'],
-            'cnspell': ['PAYH', 'WK', 'GHWA', 'GN', 'SZYA', 'SZGJ'],
-            'market': ['主板', '主板', '主板', '主板', '主板', '主板'],
-            'exchange': ['SZSE', 'SZSE', 'SZSE', 'SSE', 'SZSE', 'SZSE'],
-            'curr_type': ['CNY', 'CNY', 'CNY', 'CNY', 'CNY', 'CNY'],
+            'ts_code':     ['000001.SZ', '000002.SZ', '000004.SZ', '600251.SH', '000006.SZ', '000008.SZ'],
+            'symbol':      ['000001', '000002', '000004', '600251', '000006', '000008'],
+            'name':        ['平安银行', '万科A', '国华网安', '冠农股份', '深振业A', '神州高铁'],
+            'area':        ['深圳', '深圳', '深圳', '深圳', '深圳', '深圳'],
+            'industry':    ['银行', '全国地产', '软件服务', '农药化肥', '区域地产', '其他商业'],
+            'full_name':   ['平安银行', '万科A', '国华网安', '冠农股份', '深振业A', '神州高铁'],
+            'en_name':     ['Ping An Bank', 'Vanke A', 'Guohua Network Security', 'Guannong Shares',
+                            'Shenzhen Zhenye A', 'Shenzhou High Speed Railway'],
+            'cnspell':     ['PAYH', 'WK', 'GHWA', 'GN', 'SZYA', 'SZGJ'],
+            'market':      ['主板', '主板', '主板', '主板', '主板', '主板'],
+            'exchange':    ['SZSE', 'SZSE', 'SZSE', 'SSE', 'SZSE', 'SZSE'],
+            'curr_type':   ['CNY', 'CNY', 'CNY', 'CNY', 'CNY', 'CNY'],
             'list_status': ['L', 'L', 'L', 'L', 'L', 'L'],
-            'list_date': ['19910403', '19910129', '19910114', '19901210', '19920427', '19910625'],
+            'list_date':   ['19910403', '19910129', '19910114', '19901210', '19920427', '19910625'],
             'delist_date': ['22001231', '22001231', '22001231', '22001231', '22001231', '22001231'],
-            'is_hs': ['N', 'N', 'N', 'N', 'N', 'N'],
+            'is_hs':       ['N', 'N', 'N', 'N', 'N', 'N'],
         })
         stock_basic = self.test_ds.fetch_history_table_data(
                 table='stock_basic',
                 channel='df',
                 df=stock_basic_df,
         )
         self.test_ds.update_table_data('stock_basic', stock_basic)
 
         index_basic_df = pd.DataFrame({
-            'ts_code': ['000001.SH', '000002.SH', '000004.SH', '000006.SH', '000008.SH'],
-            'name': ['上证指数', 'A股指数', '工业指数', '地产指数', '综合指数'],
-            'fullname': ['上证指数', 'A股指数', '工业指数', '地产指数', '综合指数'],
-            'market': ['上证', '上证', '上证', '上证', '上证'],
-            'publisher': ['上证', '上证', '上证', '上证', '上证'],
-            'index_type': ['1', '1', '1', '1', '1'],
-            'category': ['1', '1', '1', '1', '1'],
-            'base_date': ['19901219', '19910129', '19910114', '19910129', '19910114'],
-            'base_point': ['100.0', '100.0', '100.0', '100.0', '100.0'],
-            'list_date': ['19910403', '19910129', '19910114', '19910129', '19910114'],
+            'ts_code':     ['000001.SH', '000002.SH', '000004.SH', '000006.SH', '000008.SH'],
+            'name':        ['上证指数', 'A股指数', '工业指数', '地产指数', '综合指数'],
+            'fullname':    ['上证指数', 'A股指数', '工业指数', '地产指数', '综合指数'],
+            'market':      ['上证', '上证', '上证', '上证', '上证'],
+            'publisher':   ['上证', '上证', '上证', '上证', '上证'],
+            'index_type':  ['1', '1', '1', '1', '1'],
+            'category':    ['1', '1', '1', '1', '1'],
+            'base_date':   ['19901219', '19910129', '19910114', '19910129', '19910114'],
+            'base_point':  ['100.0', '100.0', '100.0', '100.0', '100.0'],
+            'list_date':   ['19910403', '19910129', '19910114', '19910129', '19910114'],
             'weight_rule': ['等权', '等权', '等权', '等权', '等权'],
-            'desc': ['描述', '描述', '描述', '描述', '描述'],
-            'exp_date': ['22001231', '22001231', '22001231', '22001231', '22001231'],
+            'desc':        ['描述', '描述', '描述', '描述', '描述'],
+            'exp_date':    ['22001231', '22001231', '22001231', '22001231', '22001231'],
         })
         index_basic = self.test_ds.fetch_history_table_data(
                 table='index_basic',
                 channel='df',
                 df=index_basic_df,
         )
         self.test_ds.update_table_data('index_basic', index_basic)
@@ -2945,35 +3088,35 @@
         print(symbol_names)
         self.assertEqual(symbol_names, ['平安银行', '万科A', 'N/A', 'N/A'])
 
         # download func basic data and names will be returned after refresh
         print('test get_symbol_names with symbols whose basic data is now downloaded but not refreshed')
 
         fund_basic_df = pd.DataFrame({
-            'ts_code': ['000606.OF', '000291.OF'],
-            'name': ['天弘优选', '鹏华普悦'],
-            'management': ['天弘基金', '鹏华基金'],
-            'custodian': ['中国银行', '中国银行'],
-            'fund_type': ['股票型', '股票型'],
-            'found_date': ['20150130', '20150130'],
-            'due_date': ['22001231', '22001231'],
-            'list_date': ['20150130', '20150130'],
-            'issue_date': ['20150130', '20150130'],
-            'delist_date': ['22001231', '22001231'],
-            'issue_amount': ['1000000000.0', '1000000000.0'],
-            'm_fee': ['0.1', '0.1'],
-            'c_fee': ['0.1', '0.1'],
+            'ts_code':       ['000606.OF', '000291.OF'],
+            'name':          ['天弘优选', '鹏华普悦'],
+            'management':    ['天弘基金', '鹏华基金'],
+            'custodian':     ['中国银行', '中国银行'],
+            'fund_type':     ['股票型', '股票型'],
+            'found_date':    ['20150130', '20150130'],
+            'due_date':      ['22001231', '22001231'],
+            'list_date':     ['20150130', '20150130'],
+            'issue_date':    ['20150130', '20150130'],
+            'delist_date':   ['22001231', '22001231'],
+            'issue_amount':  ['1000000000.0', '1000000000.0'],
+            'm_fee':         ['0.1', '0.1'],
+            'c_fee':         ['0.1', '0.1'],
             'duration_year': ['3.0', '3.0'],
-            'p_value': ['1.0', '1.0'],
-            'min_amount': ['100.0', '100.0'],
-            'exp_return': ['0.1', '0.1'],
-            'benchmark': ['沪深300', '沪深300'],
-            'status': ['在售', '在售'],
-            'invest_type': ['股票型', '股票型'],
-            'type': ['开放式', '开放式'],
+            'p_value':       ['1.0', '1.0'],
+            'min_amount':    ['100.0', '100.0'],
+            'exp_return':    ['0.1', '0.1'],
+            'benchmark':     ['沪深300', '沪深300'],
+            'status':        ['在售', '在售'],
+            'invest_type':   ['股票型', '股票型'],
+            'type':          ['开放式', '开放式'],
         })
         fund_basic = self.test_ds.fetch_history_table_data(
                 table='fund_basic',
                 channel='df',
                 df=fund_basic_df,
         )
         self.test_ds.update_table_data('fund_basic', fund_basic)
@@ -2991,8 +3134,8 @@
                 refresh=True,
         )
         print(symbol_names)
         self.assertEqual(symbol_names, ['平安银行', '万科A', '天弘优选', '鹏华普悦'])
 
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

### Comparing `qteasy-1.1.8/tests/test_tushare.py` & `qteasy-1.1.9/tests/test_tushare.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_utilityfuncs.py` & `qteasy-1.1.9/tests/test_utilityfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.8/tests/test_visual.py` & `qteasy-1.1.9/tests/test_visual.py`

 * *Files identical despite different names*

