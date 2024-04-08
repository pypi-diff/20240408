# Comparing `tmp/dash_express_components-0.0.90.tar.gz` & `tmp/dash_express_components-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_express_components-0.0.90.tar", last modified: Mon Nov 27 19:44:53 2023, max compression
+gzip compressed data, was "dash_express_components-0.0.91.tar", last modified: Mon Apr  8 13:27:30 2024, max compression
```

## Comparing `dash_express_components-0.0.90.tar` & `dash_express_components-0.0.91.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:44:53.894119 dash_express_components-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-11-27 19:44:53.890119 dash_express_components-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:44:53.886119 dash_express_components-0.0.90/dash_express_components/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/AggrTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/AsType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/BarCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/BinTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/CategoryLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/CombinecatTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/ConfigReceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/CoreGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/DropnaTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/EvalTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/FilterIqrTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2023-11-27 19:44:53.000000 dash_express_components-0.0.90/dash_express_components/Graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/GroupedSample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/HistogramLine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Imshow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Localstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/MeltTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/MetaCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Parameterize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/PlotterBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/RenameTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/ScatterMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/StrSplitTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/SubComponentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/Violin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/WideToLong.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/ZerosToNanTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/_imports_.py
--rw-r--r--   0 runner    (1001) docker     (127)  1163624 2023-11-27 19:44:50.000000 dash_express_components-0.0.90/dash_express_components/async-excel.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-27 19:44:50.000000 dash_express_components-0.0.90/dash_express_components/async-excel.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   711489 2023-11-27 19:44:50.000000 dash_express_components-0.0.90/dash_express_components/dash_express_components.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-27 19:44:50.000000 dash_express_components-0.0.90/dash_express_components/dash_express_components.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    91991 2023-11-27 19:44:52.000000 dash_express_components-0.0.90/dash_express_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/package-info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:44:53.886119 dash_express_components-0.0.90/dash_express_components/plottypes/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/plottypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/plottypes/_bar_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/plottypes/_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/plottypes/_histogram_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/plottypes/_imshow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/plottypes/_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/plottypes/_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/plottypes/_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:44:53.890119 dash_express_components-0.0.90/dash_express_components/transformationtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_aggr.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_asType.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_bin.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_catlookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_combinecat.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_dropna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_groupby_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_iqrfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_melt.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_strsplit.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_wide_to_long.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/transformationtypes/_zerostonan.py
--rw-r--r--   0 runner    (1001) docker     (127)    25418 2023-11-27 19:44:51.000000 dash_express_components-0.0.90/dash_express_components/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:44:53.886119 dash_express_components-0.0.90/dash_express_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-11-27 19:44:53.000000 dash_express_components-0.0.90/dash_express_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2023-11-27 19:44:53.000000 dash_express_components-0.0.90/dash_express_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 19:44:53.000000 dash_express_components-0.0.90/dash_express_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-27 19:44:53.000000 dash_express_components-0.0.90/dash_express_components.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:44:53.890119 dash_express_components-0.0.90/dash_express_components_base/
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:44:53.890119 dash_express_components-0.0.90/dash_express_components_base/plottypes/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/plottypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/plottypes/_bar_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/plottypes/_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/plottypes/_histogram_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/plottypes/_imshow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/plottypes/_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/plottypes/_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/plottypes/_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:44:53.890119 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_aggr.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_asType.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_bin.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_catlookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_combinecat.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_dropna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_groupby_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_iqrfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_melt.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_strsplit.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_wide_to_long.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_zerostonan.py
--rw-r--r--   0 runner    (1001) docker     (127)    25418 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/dash_express_components_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 19:44:53.894119 dash_express_components-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-11-27 19:43:53.000000 dash_express_components-0.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:27:30.777977 dash_express_components-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 13:27:30.777977 dash_express_components-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:27:30.769977 dash_express_components-0.0.91/dash_express_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/AggrTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/AsType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/BarCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/BinTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/CategoryLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/CombinecatTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/ConfigReceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/CoreGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/DropnaTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/EvalTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/FilterIqrTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/GroupedSample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/HistogramLine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Imshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Localstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/MeltTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/MetaCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/PlotterBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/RenameTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/ScatterMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/StrSplitTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/SubComponentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/Violin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/WideToLong.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/ZerosToNanTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/_imports_.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1163624 2024-04-08 13:27:27.000000 dash_express_components-0.0.91/dash_express_components/async-excel.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 13:27:27.000000 dash_express_components-0.0.91/dash_express_components/async-excel.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   711489 2024-04-08 13:27:27.000000 dash_express_components-0.0.91/dash_express_components/dash_express_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-08 13:27:27.000000 dash_express_components-0.0.91/dash_express_components/dash_express_components.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    91991 2024-04-08 13:27:29.000000 dash_express_components-0.0.91/dash_express_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/package-info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:27:30.769977 dash_express_components-0.0.91/dash_express_components/plottypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/plottypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/plottypes/_bar_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/plottypes/_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/plottypes/_histogram_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/plottypes/_imshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/plottypes/_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/plottypes/_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/plottypes/_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:27:30.773977 dash_express_components-0.0.91/dash_express_components/transformationtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_aggr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_asType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_catlookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_combinecat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_dropna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_groupby_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_iqrfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_melt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_strsplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_wide_to_long.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/transformationtypes/_zerostonan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-04-08 13:27:28.000000 dash_express_components-0.0.91/dash_express_components/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:27:30.769977 dash_express_components-0.0.91/dash_express_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 13:27:30.000000 dash_express_components-0.0.91/dash_express_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-08 13:27:30.000000 dash_express_components-0.0.91/dash_express_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:27:30.000000 dash_express_components-0.0.91/dash_express_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 13:27:30.000000 dash_express_components-0.0.91/dash_express_components.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:27:30.773977 dash_express_components-0.0.91/dash_express_components_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:27:30.773977 dash_express_components-0.0.91/dash_express_components_base/plottypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/plottypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/plottypes/_bar_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/plottypes/_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/plottypes/_histogram_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/plottypes/_imshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/plottypes/_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/plottypes/_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/plottypes/_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:27:30.777977 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_aggr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_asType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_catlookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_combinecat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_dropna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_groupby_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_iqrfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_melt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_strsplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_wide_to_long.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_zerostonan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/dash_express_components_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:27:30.777977 dash_express_components-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-08 13:26:26.000000 dash_express_components-0.0.91/setup.py
```

### Comparing `dash_express_components-0.0.90/README.md` & `dash_express_components-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/AggrTransform.py` & `dash_express_components-0.0.91/dash_express_components/AggrTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/AsType.py` & `dash_express_components-0.0.91/dash_express_components/AsType.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Bar.py` & `dash_express_components-0.0.91/dash_express_components/Bar.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/BarCount.py` & `dash_express_components-0.0.91/dash_express_components/BarCount.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Base.py` & `dash_express_components-0.0.91/dash_express_components/Base.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/BinTransform.py` & `dash_express_components-0.0.91/dash_express_components/BinTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Box.py` & `dash_express_components-0.0.91/dash_express_components/Box.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/CategoryLookup.py` & `dash_express_components-0.0.91/dash_express_components/CategoryLookup.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/CombinecatTransform.py` & `dash_express_components-0.0.91/dash_express_components/CombinecatTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/ConfigReceiver.py` & `dash_express_components-0.0.91/dash_express_components/ConfigReceiver.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Configurator.py` & `dash_express_components-0.0.91/dash_express_components/Configurator.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/CoreGraph.py` & `dash_express_components-0.0.91/dash_express_components/CoreGraph.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/DropnaTransform.py` & `dash_express_components-0.0.91/dash_express_components/DropnaTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/EvalTransform.py` & `dash_express_components-0.0.91/dash_express_components/EvalTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Filter.py` & `dash_express_components-0.0.91/dash_express_components/Filter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/FilterIqrTransform.py` & `dash_express_components-0.0.91/dash_express_components/FilterIqrTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Graph.py` & `dash_express_components-0.0.91/dash_express_components/Graph.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/GroupedSample.py` & `dash_express_components-0.0.91/dash_express_components/GroupedSample.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/HistogramLine.py` & `dash_express_components-0.0.91/dash_express_components/HistogramLine.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Imshow.py` & `dash_express_components-0.0.91/dash_express_components/Imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Localstore.py` & `dash_express_components-0.0.91/dash_express_components/Localstore.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/MeltTransform.py` & `dash_express_components-0.0.91/dash_express_components/MeltTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/MetaCheck.py` & `dash_express_components-0.0.91/dash_express_components/MetaCheck.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Parameterize.py` & `dash_express_components-0.0.91/dash_express_components/Parameterize.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Plotter.py` & `dash_express_components-0.0.91/dash_express_components/Plotter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/PlotterBase.py` & `dash_express_components-0.0.91/dash_express_components/PlotterBase.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Probability.py` & `dash_express_components-0.0.91/dash_express_components/Probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/RenameTransform.py` & `dash_express_components-0.0.91/dash_express_components/RenameTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Scatter.py` & `dash_express_components-0.0.91/dash_express_components/Scatter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/ScatterMatrix.py` & `dash_express_components-0.0.91/dash_express_components/ScatterMatrix.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/StrSplitTransform.py` & `dash_express_components-0.0.91/dash_express_components/StrSplitTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/SubComponentBase.py` & `dash_express_components-0.0.91/dash_express_components/SubComponentBase.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Table.py` & `dash_express_components-0.0.91/dash_express_components/Table.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Transform.py` & `dash_express_components-0.0.91/dash_express_components/Transform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/Violin.py` & `dash_express_components-0.0.91/dash_express_components/Violin.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/WideToLong.py` & `dash_express_components-0.0.91/dash_express_components/WideToLong.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/ZerosToNanTransform.py` & `dash_express_components-0.0.91/dash_express_components/ZerosToNanTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/__init__.py` & `dash_express_components-0.0.91/dash_express_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/_imports_.py` & `dash_express_components-0.0.91/dash_express_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/async-excel.js` & `dash_express_components-0.0.91/dash_express_components/async-excel.js`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/dash_express_components.min.js` & `dash_express_components-0.0.91/dash_express_components/dash_express_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -113,15 +113,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(l()),
                 n = c(e);
             if (!t) return n;
             var r = n.split("/"),
                 a = r.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_90m1701114274"), r.splice(-1, 1, a.join(".")), r.join("/")
+            return a.splice(1, 0, "v0_0_91m1712582831"), r.splice(-1, 1, a.join(".")), r.join("/")
         }
     }
     var u = window.webpackJsonpdash_express_components = window.webpackJsonpdash_express_components || [],
         s = u.push.bind(u);
     u.push = t, u = u.slice();
     for (var f = 0; f < u.length; f++) t(u[f]);
     var p = s;
```

### Comparing `dash_express_components-0.0.90/dash_express_components/metadata.json` & `dash_express_components-0.0.91/dash_express_components/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/package-info.json` & `dash_express_components-0.0.91/dash_express_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.91'"}*

```diff
@@ -59,9 +59,9 @@
         "build:patch": "python _patch.py",
         "doc": "jsdoc -c ./jsdoc.conf.json -a public",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "test": "pytest --cov=dash_express_components tests --cov-report term-missing",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.90"
+    "version": "0.0.91"
 }
```

### Comparing `dash_express_components-0.0.90/dash_express_components/plottypes/_bar_count.py` & `dash_express_components-0.0.91/dash_express_components/plottypes/_bar_count.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/plottypes/_box.py` & `dash_express_components-0.0.91/dash_express_components/plottypes/_box.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/plottypes/_histogram_line.py` & `dash_express_components-0.0.91/dash_express_components/plottypes/_histogram_line.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/plottypes/_imshow.py` & `dash_express_components-0.0.91/dash_express_components/plottypes/_imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/plottypes/_probability.py` & `dash_express_components-0.0.91/dash_express_components/plottypes/_probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/plottypes/_scatter.py` & `dash_express_components-0.0.91/dash_express_components/plottypes/_scatter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/transformationtypes/_aggr.py` & `dash_express_components-0.0.91/dash_express_components/transformationtypes/_aggr.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/transformationtypes/_bin.py` & `dash_express_components-0.0.91/dash_express_components/transformationtypes/_bin.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/transformationtypes/_eval.py` & `dash_express_components-0.0.91/dash_express_components/transformationtypes/_eval.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/transformationtypes/_groupby_sample.py` & `dash_express_components-0.0.91/dash_express_components/transformationtypes/_groupby_sample.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/transformationtypes/_iqrfilter.py` & `dash_express_components-0.0.91/dash_express_components/transformationtypes/_iqrfilter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/transformationtypes/_strsplit.py` & `dash_express_components-0.0.91/dash_express_components/transformationtypes/_strsplit.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/transformationtypes/_wide_to_long.py` & `dash_express_components-0.0.91/dash_express_components/transformationtypes/_wide_to_long.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components/utils.py` & `dash_express_components-0.0.91/dash_express_components/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,16 @@
     from numpy import dtype
     import dask
     """
     extract the metadata from a dask dataframe.
     """
 
     def parse(key, val):
-        if val == dtype('O'):
+        
+        if val == dtype('O') or val == 'string':
 
             cat = df[key].unique()
             if len(cat) > large_threshold:
                 return {
                     "type": "categorical",
                     "large": True,
                     "cat": []
@@ -117,15 +118,15 @@
                 "type": "bool"
             }
         elif "time" in str(val):
             return {
                 "type": "temporal",
                 "min": df[key].min(),
                 "max": df[key].max(),
-                "median": df[key].mean()
+                "median": df[key].max()
             }
         else:
             return {
                 "type": "numerical",
                 "min": df[key].min(),
                 "max": df[key].max(),
                 "median": df[key].mean()
@@ -138,17 +139,19 @@
     }
 
     # compute it
     res = dask.compute(res, scheduler='single-threaded')[0]
 
     # transform the variables to simple python (json dump needed)
     for k, v in res.items():
-        if "cat" in v:
+        if "cat" in v and not isinstance(v["cat"], list):
             v["cat"] = v["cat"].tolist()
         for ik in ["min", "max", "median"]:
+            if v["type"] == "temporal":
+                continue
             if ik in v:
                 v[ik] = float(v[ik])
 
     return res
 
 
 def get_meta_sparkpandas(df, large_threshold=1000):
```

### Comparing `dash_express_components-0.0.90/dash_express_components.egg-info/SOURCES.txt` & `dash_express_components-0.0.91/dash_express_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/__init__.py` & `dash_express_components-0.0.91/dash_express_components_base/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/plottypes/_bar_count.py` & `dash_express_components-0.0.91/dash_express_components_base/plottypes/_bar_count.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/plottypes/_box.py` & `dash_express_components-0.0.91/dash_express_components_base/plottypes/_box.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/plottypes/_histogram_line.py` & `dash_express_components-0.0.91/dash_express_components_base/plottypes/_histogram_line.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/plottypes/_imshow.py` & `dash_express_components-0.0.91/dash_express_components_base/plottypes/_imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/plottypes/_probability.py` & `dash_express_components-0.0.91/dash_express_components_base/plottypes/_probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/plottypes/_scatter.py` & `dash_express_components-0.0.91/dash_express_components_base/plottypes/_scatter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_aggr.py` & `dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_aggr.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_bin.py` & `dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_bin.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_eval.py` & `dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_eval.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_groupby_sample.py` & `dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_groupby_sample.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_iqrfilter.py` & `dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_iqrfilter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_strsplit.py` & `dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_strsplit.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/transformationtypes/_wide_to_long.py` & `dash_express_components-0.0.91/dash_express_components_base/transformationtypes/_wide_to_long.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.90/dash_express_components_base/utils.py` & `dash_express_components-0.0.91/dash_express_components_base/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,16 @@
     from numpy import dtype
     import dask
     """
     extract the metadata from a dask dataframe.
     """
 
     def parse(key, val):
-        if val == dtype('O'):
+        
+        if val == dtype('O') or val == 'string':
 
             cat = df[key].unique()
             if len(cat) > large_threshold:
                 return {
                     "type": "categorical",
                     "large": True,
                     "cat": []
@@ -117,15 +118,15 @@
                 "type": "bool"
             }
         elif "time" in str(val):
             return {
                 "type": "temporal",
                 "min": df[key].min(),
                 "max": df[key].max(),
-                "median": df[key].mean()
+                "median": df[key].max()
             }
         else:
             return {
                 "type": "numerical",
                 "min": df[key].min(),
                 "max": df[key].max(),
                 "median": df[key].mean()
@@ -138,17 +139,19 @@
     }
 
     # compute it
     res = dask.compute(res, scheduler='single-threaded')[0]
 
     # transform the variables to simple python (json dump needed)
     for k, v in res.items():
-        if "cat" in v:
+        if "cat" in v and not isinstance(v["cat"], list):
             v["cat"] = v["cat"].tolist()
         for ik in ["min", "max", "median"]:
+            if v["type"] == "temporal":
+                continue
             if ik in v:
                 v[ik] = float(v[ik])
 
     return res
 
 
 def get_meta_sparkpandas(df, large_threshold=1000):
```

### Comparing `dash_express_components-0.0.90/package.json` & `dash_express_components-0.0.91/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.91'"}*

```diff
@@ -59,9 +59,9 @@
         "build:patch": "python _patch.py",
         "doc": "jsdoc -c ./jsdoc.conf.json -a public",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "test": "pytest --cov=dash_express_components tests --cov-report term-missing",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.90"
+    "version": "0.0.91"
 }
```

### Comparing `dash_express_components-0.0.90/setup.py` & `dash_express_components-0.0.91/setup.py`

 * *Files identical despite different names*

