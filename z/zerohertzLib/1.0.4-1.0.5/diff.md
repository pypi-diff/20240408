# Comparing `tmp/zerohertzLib-1.0.4.tar.gz` & `tmp/zerohertzLib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerohertzLib-1.0.4.tar", last modified: Fri Apr  5 09:07:00 2024, max compression
+gzip compressed data, was "zerohertzLib-1.0.5.tar", last modified: Mon Apr  8 09:33:56 2024, max compression
```

## Comparing `zerohertzLib-1.0.4.tar` & `zerohertzLib-1.0.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.428856 zerohertzLib-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-04-05 09:06:54.000000 zerohertzLib-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-05 09:06:54.000000 zerohertzLib-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-05 09:07:00.428856 zerohertzLib-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2316 2024-04-05 09:06:54.000000 zerohertzLib-1.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 09:07:00.428856 zerohertzLib-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2704 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.416856 zerohertzLib-1.0.4/test/
--rw-r--r--   0 root         (0) root         (0)     4501 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_api.py
--rw-r--r--   0 root         (0) root         (0)     1230 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)      220 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)     8641 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_plot.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_quant.py
--rw-r--r--   0 root         (0) root         (0)     1961 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_util.py
--rw-r--r--   0 root         (0) root         (0)    14679 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/
--rw-r--r--   0 root         (0) root         (0)     1794 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/algorithm/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2626 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/bisect.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/collections.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/fft.py
--rw-r--r--   0 root         (0) root         (0)     7065 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/graph.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/prime.py
--rw-r--r--   0 root         (0) root         (0)     8048 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/api/
--rw-r--r--   0 root         (0) root         (0)      446 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3865 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/discord.py
--rw-r--r--   0 root         (0) root         (0)    11096 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/github.py
--rw-r--r--   0 root         (0) root         (0)    30846 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/koreainvestment.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/open_ai.py
--rw-r--r--   0 root         (0) root         (0)     8841 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/logging/
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4738 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/logging/handler.py
--rw-r--r--   0 root         (0) root         (0)     5264 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/logging/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/mlops/
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/mlops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18002 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/mlops/triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/monitoring/
--rw-r--r--   0 root         (0) root         (0)      333 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2829 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/monitoring/cpu.py
--rw-r--r--   0 root         (0) root         (0)     5184 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/monitoring/gpu.py
--rw-r--r--   0 root         (0) root         (0)     2678 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/monitoring/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/plot/
--rw-r--r--   0 root         (0) root         (0)     1552 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15381 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/bar_chart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.424856 zerohertzLib-1.0.4/zerohertzLib/plot/fonts/
--rw-r--r--   0 root         (0) root         (0)  7549348 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
--rw-r--r--   0 root         (0) root         (0)   347988 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/fonts/times.ttf
--rw-r--r--   0 root         (0) root         (0)     3435 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/pie.py
--rw-r--r--   0 root         (0) root         (0)    11476 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/plot.py
--rw-r--r--   0 root         (0) root         (0)     4046 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/scatter.py
--rw-r--r--   0 root         (0) root         (0)     3292 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/table.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.424856 zerohertzLib-1.0.4/zerohertzLib/quant/
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14935 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/quant/backtest.py
--rw-r--r--   0 root         (0) root         (0)    13182 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/quant/methods.py
--rw-r--r--   0 root         (0) root         (0)    45370 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/quant/quant.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/quant/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.424856 zerohertzLib-1.0.4/zerohertzLib/util/
--rw-r--r--   0 root         (0) root         (0)      458 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4527 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/util/csv.py
--rw-r--r--   0 root         (0) root         (0)    11173 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/util/data.py
--rw-r--r--   0 root         (0) root         (0)    11650 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/util/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.428856 zerohertzLib-1.0.4/zerohertzLib/vision/
--rw-r--r--   0 root         (0) root         (0)     1623 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6967 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/compare.py
--rw-r--r--   0 root         (0) root         (0)    12885 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/convert.py
--rw-r--r--   0 root         (0) root         (0)    22648 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/data.py
--rw-r--r--   0 root         (0) root         (0)    14878 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/eval.py
--rw-r--r--   0 root         (0) root         (0)     4188 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/gif.py
--rw-r--r--   0 root         (0) root         (0)    22281 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/loader.py
--rw-r--r--   0 root         (0) root         (0)     7826 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/transform.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/util.py
--rw-r--r--   0 root         (0) root         (0)    17516 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-05 09:07:00.000000 zerohertzLib-1.0.4/zerohertzLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1923 2024-04-05 09:07:00.000000 zerohertzLib-1.0.4/zerohertzLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 09:07:00.000000 zerohertzLib-1.0.4/zerohertzLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      430 2024-04-05 09:07:00.000000 zerohertzLib-1.0.4/zerohertzLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-05 09:07:00.000000 zerohertzLib-1.0.4/zerohertzLib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-04-08 09:33:51.000000 zerohertzLib-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-08 09:33:51.000000 zerohertzLib-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-08 09:33:51.000000 zerohertzLib-1.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2704 2024-04-08 09:33:51.000000 zerohertzLib-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.680283 zerohertzLib-1.0.5/test/
+-rw-r--r--   0 root         (0) root         (0)     4501 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)      220 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_plot.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_quant.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    14679 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.680283 zerohertzLib-1.0.5/zerohertzLib/
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.680283 zerohertzLib-1.0.5/zerohertzLib/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/bisect.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/collections.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/fft.py
+-rw-r--r--   0 root         (0) root         (0)     7065 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/prime.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.684284 zerohertzLib-1.0.5/zerohertzLib/api/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/discord.py
+-rw-r--r--   0 root         (0) root         (0)    11096 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/github.py
+-rw-r--r--   0 root         (0) root         (0)    30846 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/koreainvestment.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/open_ai.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.684284 zerohertzLib-1.0.5/zerohertzLib/logging/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/logging/handler.py
+-rw-r--r--   0 root         (0) root         (0)     5264 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/logging/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.684284 zerohertzLib-1.0.5/zerohertzLib/mlops/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/mlops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18002 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/mlops/triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.684284 zerohertzLib-1.0.5/zerohertzLib/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      333 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/monitoring/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/monitoring/gpu.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/monitoring/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.684284 zerohertzLib-1.0.5/zerohertzLib/plot/
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15381 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/bar_chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/zerohertzLib/plot/fonts/
+-rw-r--r--   0 root         (0) root         (0)  7549348 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
+-rw-r--r--   0 root         (0) root         (0)   347988 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/fonts/times.ttf
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/pie.py
+-rw-r--r--   0 root         (0) root         (0)    11476 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/scatter.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/table.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/zerohertzLib/quant/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/quant/backtest.py
+-rw-r--r--   0 root         (0) root         (0)    13182 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/quant/methods.py
+-rw-r--r--   0 root         (0) root         (0)    45350 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/quant/quant.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/quant/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/zerohertzLib/util/
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/util/csv.py
+-rw-r--r--   0 root         (0) root         (0)    11173 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/util/data.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/util/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/zerohertzLib/vision/
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6967 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/compare.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/convert.py
+-rw-r--r--   0 root         (0) root         (0)    22648 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/data.py
+-rw-r--r--   0 root         (0) root         (0)    14878 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/eval.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/gif.py
+-rw-r--r--   0 root         (0) root         (0)    22281 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/loader.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/util.py
+-rw-r--r--   0 root         (0) root         (0)    17516 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.680283 zerohertzLib-1.0.5/zerohertzLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-04-08 09:33:56.000000 zerohertzLib-1.0.5/zerohertzLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-04-08 09:33:56.000000 zerohertzLib-1.0.5/zerohertzLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 09:33:56.000000 zerohertzLib-1.0.5/zerohertzLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-08 09:33:56.000000 zerohertzLib-1.0.5/zerohertzLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-08 09:33:56.000000 zerohertzLib-1.0.5/zerohertzLib.egg-info/top_level.txt
```

### Comparing `zerohertzLib-1.0.4/LICENSE` & `zerohertzLib-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/PKG-INFO` & `zerohertzLib-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.4
+Version: 1.0.5
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.4 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.5 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.4/README.md` & `zerohertzLib-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/setup.py` & `zerohertzLib-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/test/test_algorithm.py` & `zerohertzLib-1.0.5/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/test/test_api.py` & `zerohertzLib-1.0.5/test/test_api.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/test/test_logging.py` & `zerohertzLib-1.0.5/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/test/test_plot.py` & `zerohertzLib-1.0.5/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/test/test_quant.py` & `zerohertzLib-1.0.5/test/test_quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/test/test_util.py` & `zerohertzLib-1.0.5/test/test_util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/test/test_vision.py` & `zerohertzLib-1.0.5/test/test_vision.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/__init__.py` & `zerohertzLib-1.0.5/zerohertzLib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     print("=" * 100)
     print(f"[Warning] {error}")
     print("Please Install OpenCV Dependency")
     print("--->\t$ sudo apt install python3-opencv -y\t<---")
     print("(but you can use other submodules except zerohertzLib.vision)")
     print("=" * 100)
 
-__version__ = "v1.0.4"
+__version__ = "v1.0.5"
```

### Comparing `zerohertzLib-1.0.4/zerohertzLib/algorithm/__init__.py` & `zerohertzLib-1.0.5/zerohertzLib/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/algorithm/bisect.py` & `zerohertzLib-1.0.5/zerohertzLib/algorithm/bisect.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/algorithm/collections.py` & `zerohertzLib-1.0.5/zerohertzLib/algorithm/collections.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/algorithm/fft.py` & `zerohertzLib-1.0.5/zerohertzLib/algorithm/fft.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/algorithm/graph.py` & `zerohertzLib-1.0.5/zerohertzLib/algorithm/graph.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/algorithm/prime.py` & `zerohertzLib-1.0.5/zerohertzLib/algorithm/prime.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/algorithm/sort.py` & `zerohertzLib-1.0.5/zerohertzLib/algorithm/sort.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/api/discord.py` & `zerohertzLib-1.0.5/zerohertzLib/api/discord.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/api/github.py` & `zerohertzLib-1.0.5/zerohertzLib/api/github.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/api/koreainvestment.py` & `zerohertzLib-1.0.5/zerohertzLib/api/koreainvestment.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/api/open_ai.py` & `zerohertzLib-1.0.5/zerohertzLib/api/open_ai.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/api/slack.py` & `zerohertzLib-1.0.5/zerohertzLib/api/slack.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/logging/handler.py` & `zerohertzLib-1.0.5/zerohertzLib/logging/handler.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/logging/logger.py` & `zerohertzLib-1.0.5/zerohertzLib/logging/logger.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/mlops/triton.py` & `zerohertzLib-1.0.5/zerohertzLib/mlops/triton.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/monitoring/cpu.py` & `zerohertzLib-1.0.5/zerohertzLib/monitoring/cpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/monitoring/gpu.py` & `zerohertzLib-1.0.5/zerohertzLib/monitoring/gpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/monitoring/storage.py` & `zerohertzLib-1.0.5/zerohertzLib/monitoring/storage.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/plot/__init__.py` & `zerohertzLib-1.0.5/zerohertzLib/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/plot/bar_chart.py` & `zerohertzLib-1.0.5/zerohertzLib/plot/bar_chart.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf` & `zerohertzLib-1.0.5/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/plot/fonts/times.ttf` & `zerohertzLib-1.0.5/zerohertzLib/plot/fonts/times.ttf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/plot/pie.py` & `zerohertzLib-1.0.5/zerohertzLib/plot/pie.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/plot/plot.py` & `zerohertzLib-1.0.5/zerohertzLib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/plot/scatter.py` & `zerohertzLib-1.0.5/zerohertzLib/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/plot/table.py` & `zerohertzLib-1.0.5/zerohertzLib/plot/table.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/plot/util.py` & `zerohertzLib-1.0.5/zerohertzLib/plot/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/quant/__init__.py` & `zerohertzLib-1.0.5/zerohertzLib/quant/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/quant/backtest.py` & `zerohertzLib-1.0.5/zerohertzLib/quant/backtest.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/quant/methods.py` & `zerohertzLib-1.0.5/zerohertzLib/quant/methods.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/quant/quant.py` & `zerohertzLib-1.0.5/zerohertzLib/quant/quant.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,20 +308,18 @@
 
     def __init__(
         self, account_no: str, path: Optional[str] = "./", kor: Optional[bool] = True
     ) -> None:
         super().__init__(account_no, path)
         self.balance = {"stock": defaultdict(list)}
         self.kor = kor
-        self.symbols = []
         response = self.get_balance(kor)
         if self.kor:
             for stock in response["output1"]:
                 if int(stock["hldg_qty"]) > 0:  # 보유수량
-                    self.symbols.append(stock["prdt_name"])
                     self.balance["stock"][stock["prdt_name"]] = [
                         stock["pdno"],  # 종목번호
                         float(
                             stock["pchs_avg_pric"]
                         ),  # 매입평균가격 (매입금액 / 보유수량)
                         int(stock["prpr"]),  # 현재가
                         int(stock["hldg_qty"]),  # 보유수량
@@ -330,15 +328,14 @@
                             stock["evlu_pfls_amt"]
                         ),  # 평가손익금액 (평가금액 - 매입금액)
                     ]
             self.balance["cash"] = int(response["output2"][0]["nass_amt"])  # 순자산금액
         else:
             for stock in response["output1"]:
                 if int(float(stock["ccld_qty_smtl1"])) > 0:  # 체결수량합계
-                    self.symbols.append(stock["prdt_name"])
                     self.balance["stock"][stock["prdt_name"]] = [
                         stock["pdno"],  # 종목번호
                         float(stock["avg_unpr3"]),  # 평균단가
                         float(stock["ovrs_now_pric1"]),  # 해외현재가격
                         int(float(stock["ccld_qty_smtl1"])),  # 해외잔고수량
                         float(stock["evlu_pfls_rt1"]),  # 평가손익율
                         float(stock["evlu_pfls_amt2"]),  # 평가손익금액
@@ -360,14 +357,15 @@
         self.balance["stock"] = dict(
             sorted(
                 self.balance["stock"].items(),
                 key=lambda item: item[1][1] * item[1][3],
                 reverse=True,
             )
         )
+        self.symbols = list(self.balance["stock"].keys())
 
     def __contains__(self, item: Any) -> bool:
         return item in self.balance["stock"]
 
     def __len__(self) -> int:
         return len(self.balance["stock"])
 
@@ -461,14 +459,15 @@
         self.balance["stock"] = dict(
             sorted(
                 self.balance["stock"].items(),
                 key=lambda item: item[1][1] * item[1][3],
                 reverse=True,
             )
         )
+        self.symbols = list(self.balance["stock"].keys())
 
     def items(self) -> ItemsView[str, List[Union[int, float, str]]]:
         """보유 주식의 반복문 사용을 위한 method
 
         Returns:
             ``ItemsView[str, List[Union[int, float, str]]]``: 보유 종목 code와 그에 따른 정보들
 
@@ -518,38 +517,38 @@
                 "Profit and Loss (P&L) [$]",
             ]
         row = []
         data = []
         purchase_total = 0
         current_total = 0
         for name, value in self.items():
-            _, purchase, current, quantity, pal, pal_price = value
+            _, purchase, current, quantity, pandl_per, pandl_abs = value
             row.append(name)
             data.append(
                 [
                     _cash2str(purchase, self.kor),
                     _cash2str(current, self.kor),
                     quantity,
-                    f"{pal}%",
-                    _cash2str(pal_price, self.kor),
+                    f"{pandl_per:.2f}%",
+                    _cash2str(pandl_abs, self.kor),
                 ]
             )
             purchase_total += purchase * quantity
             current_total += current * quantity
         row.append("TOTAL")
         if purchase_total == 0:
-            pl_percentage = 0
+            pandl_total = 0
         else:
-            pl_percentage = (current_total - purchase_total) / purchase_total * 100
+            pandl_total = (current_total - purchase_total) / purchase_total * 100
         data.append(
             [
                 _cash2str(purchase_total, self.kor),
                 _cash2str(current_total, self.kor),
                 "-",
-                f"{pl_percentage:.2f}%",
+                f"{pandl_total:.2f}%",
                 f"{_cash2str(current_total - purchase_total, self.kor)}\n\n{_cash2str(self(), self.kor)}",
             ]
         )
         return table(
             data,
             col,
             row,
```

### Comparing `zerohertzLib-1.0.4/zerohertzLib/quant/util.py` & `zerohertzLib-1.0.5/zerohertzLib/quant/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/util/csv.py` & `zerohertzLib-1.0.5/zerohertzLib/util/csv.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/util/data.py` & `zerohertzLib-1.0.5/zerohertzLib/util/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/util/json.py` & `zerohertzLib-1.0.5/zerohertzLib/util/json.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/vision/__init__.py` & `zerohertzLib-1.0.5/zerohertzLib/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/vision/compare.py` & `zerohertzLib-1.0.5/zerohertzLib/vision/compare.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/vision/convert.py` & `zerohertzLib-1.0.5/zerohertzLib/vision/convert.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/vision/data.py` & `zerohertzLib-1.0.5/zerohertzLib/vision/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/vision/eval.py` & `zerohertzLib-1.0.5/zerohertzLib/vision/eval.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/vision/gif.py` & `zerohertzLib-1.0.5/zerohertzLib/vision/gif.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/vision/loader.py` & `zerohertzLib-1.0.5/zerohertzLib/vision/loader.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/vision/transform.py` & `zerohertzLib-1.0.5/zerohertzLib/vision/transform.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/vision/util.py` & `zerohertzLib-1.0.5/zerohertzLib/vision/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib/vision/visual.py` & `zerohertzLib-1.0.5/zerohertzLib/vision/visual.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.4/zerohertzLib.egg-info/PKG-INFO` & `zerohertzLib-1.0.5/zerohertzLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.4
+Version: 1.0.5
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.4 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.5 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.4/zerohertzLib.egg-info/SOURCES.txt` & `zerohertzLib-1.0.5/zerohertzLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

