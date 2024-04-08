# Comparing `tmp/mlforecast-0.9.2.tar.gz` & `tmp/mlforecast-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforecast-0.9.2.tar", last modified: Tue Aug 29 17:56:12 2023, max compression
+gzip compressed data, was "mlforecast-0.9.3.tar", last modified: Tue Sep 12 17:35:25 2023, max compression
```

## Comparing `mlforecast-0.9.2.tar` & `mlforecast-0.9.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 17:56:12.974030 mlforecast-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (999)     4398 2023-08-29 17:55:57.000000 mlforecast-0.9.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (999)    11336 2023-08-29 17:55:57.000000 mlforecast-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      111 2023-08-29 17:55:57.000000 mlforecast-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)    12470 2023-08-29 17:56:12.974030 mlforecast-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    11575 2023-08-29 17:55:57.000000 mlforecast-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 17:56:12.970030 mlforecast-0.9.2/mlforecast/
--rw-r--r--   0 runner    (1001) docker     (999)       90 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    32813 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (999)    26333 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 17:56:12.974030 mlforecast-0.9.2/mlforecast/distributed/
--rw-r--r--   0 runner    (1001) docker     (999)      102 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    25805 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 17:56:12.974030 mlforecast-0.9.2/mlforecast/distributed/models/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 17:56:12.974030 mlforecast-0.9.2/mlforecast/distributed/models/dask/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/models/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      714 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/models/dask/lgb.py
--rw-r--r--   0 runner    (1001) docker     (999)      527 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/models/dask/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 17:56:12.974030 mlforecast-0.9.2/mlforecast/distributed/models/ray/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/models/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      450 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/models/ray/lgb.py
--rw-r--r--   0 runner    (1001) docker     (999)      552 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/models/ray/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 17:56:12.974030 mlforecast-0.9.2/mlforecast/distributed/models/spark/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/models/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      836 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/models/spark/lgb.py
--rw-r--r--   0 runner    (1001) docker     (999)      862 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/distributed/models/spark/xgb.py
--rw-r--r--   0 runner    (1001) docker     (999)    31891 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/forecast.py
--rw-r--r--   0 runner    (1001) docker     (999)     7697 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/grouped_array.py
--rw-r--r--   0 runner    (1001) docker     (999)    22522 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/lgb_cv.py
--rw-r--r--   0 runner    (1001) docker     (999)     5445 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/target_transforms.py
--rw-r--r--   0 runner    (1001) docker     (999)     7576 2023-08-29 17:55:57.000000 mlforecast-0.9.2/mlforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 17:56:12.970030 mlforecast-0.9.2/mlforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)    12470 2023-08-29 17:56:12.000000 mlforecast-0.9.2/mlforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      977 2023-08-29 17:56:12.000000 mlforecast-0.9.2/mlforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 17:56:12.000000 mlforecast-0.9.2/mlforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 17:56:12.000000 mlforecast-0.9.2/mlforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)      295 2023-08-29 17:56:12.000000 mlforecast-0.9.2/mlforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-29 17:56:12.000000 mlforecast-0.9.2/mlforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       59 2023-08-29 17:55:57.000000 mlforecast-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)     1033 2023-08-29 17:55:57.000000 mlforecast-0.9.2/settings.ini
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-29 17:56:12.974030 mlforecast-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     2613 2023-08-29 17:55:57.000000 mlforecast-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:25.835696 mlforecast-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2023-09-12 17:35:09.000000 mlforecast-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2023-09-12 17:35:09.000000 mlforecast-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-09-12 17:35:09.000000 mlforecast-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2023-09-12 17:35:25.835696 mlforecast-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11575 2023-09-12 17:35:09.000000 mlforecast-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:25.831696 mlforecast-0.9.3/mlforecast/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34811 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26210 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:25.831696 mlforecast-0.9.3/mlforecast/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25805 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:25.831696 mlforecast-0.9.3/mlforecast/distributed/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:25.831696 mlforecast-0.9.3/mlforecast/distributed/models/dask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/models/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/models/dask/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/models/dask/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:25.831696 mlforecast-0.9.3/mlforecast/distributed/models/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/models/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/models/ray/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/models/ray/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:25.831696 mlforecast-0.9.3/mlforecast/distributed/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/models/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/models/spark/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/distributed/models/spark/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34969 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/grouped_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22522 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/lgb_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/target_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2023-09-12 17:35:09.000000 mlforecast-0.9.3/mlforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 17:35:25.831696 mlforecast-0.9.3/mlforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2023-09-12 17:35:25.000000 mlforecast-0.9.3/mlforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2023-09-12 17:35:25.000000 mlforecast-0.9.3/mlforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 17:35:25.000000 mlforecast-0.9.3/mlforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 17:35:25.000000 mlforecast-0.9.3/mlforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2023-09-12 17:35:25.000000 mlforecast-0.9.3/mlforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-12 17:35:25.000000 mlforecast-0.9.3/mlforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-09-12 17:35:09.000000 mlforecast-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-09-12 17:35:09.000000 mlforecast-0.9.3/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-12 17:35:25.835696 mlforecast-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2023-09-12 17:35:09.000000 mlforecast-0.9.3/setup.py
```

### Comparing `mlforecast-0.9.2/CONTRIBUTING.md` & `mlforecast-0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mlforecast-0.9.2/LICENSE` & `mlforecast-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlforecast-0.9.2/PKG-INFO` & `mlforecast-0.9.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: mlforecast
-Version: 0.9.2
-Summary: Scalable machine learning based time series forecasting
-Home-page: https://github.com/Nixtla/mlforecast
-Author: José Morales
-Author-email: jmoralz92@gmail.com
-License: Apache Software License 2.0
-Keywords: python forecast forecasting machine-learning dask
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: distributed
-Provides-Extra: dev
-License-File: LICENSE
-
 Nixtla  
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting)
  [![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
```

### Comparing `mlforecast-0.9.2/README.md` & `mlforecast-0.9.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,58 @@
+Metadata-Version: 2.1
+Name: mlforecast
+Version: 0.9.3
+Summary: Scalable machine learning based time series forecasting
+Home-page: https://github.com/Nixtla/mlforecast
+Author: José Morales
+Author-email: jmoralz92@gmail.com
+License: Apache Software License 2.0
+Keywords: python forecast forecasting machine-learning dask
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numba
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
+Requires-Dist: window-ops
+Provides-Extra: distributed
+Requires-Dist: dask[complete]; extra == "distributed"
+Requires-Dist: fugue[ray]; extra == "distributed"
+Requires-Dist: pyspark; extra == "distributed"
+Requires-Dist: lightgbm_ray; extra == "distributed"
+Requires-Dist: xgboost_ray; extra == "distributed"
+Provides-Extra: dev
+Requires-Dist: numba; extra == "dev"
+Requires-Dist: pandas; extra == "dev"
+Requires-Dist: scikit-learn; extra == "dev"
+Requires-Dist: window-ops; extra == "dev"
+Requires-Dist: dask[complete]; extra == "dev"
+Requires-Dist: fugue[ray]; extra == "dev"
+Requires-Dist: pyspark; extra == "dev"
+Requires-Dist: lightgbm_ray; extra == "dev"
+Requires-Dist: xgboost_ray; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: datasetsforecast; extra == "dev"
+Requires-Dist: lightgbm; extra == "dev"
+Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: utilsforecast; extra == "dev"
+Requires-Dist: xgboost; extra == "dev"
+
 Nixtla  
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting)
  [![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
```

### Comparing `mlforecast-0.9.2/mlforecast/_modidx.py` & `mlforecast-0.9.3/mlforecast/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,20 @@
                                                          'mlforecast.distributed.models.spark.xgb.SparkXGBForecast.extract_local_model': ( 'distributed.models.spark.xgb.html#sparkxgbforecast.extract_local_model',
                                                                                                                                            'mlforecast/distributed/models/spark/xgb.py')},
             'mlforecast.forecast': { 'mlforecast.forecast.MLForecast': ('forecast.html#mlforecast', 'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.__init__': ( 'forecast.html#mlforecast.__init__',
                                                                                   'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.__repr__': ( 'forecast.html#mlforecast.__repr__',
                                                                                   'mlforecast/forecast.py'),
+                                     'mlforecast.forecast.MLForecast._compute_fitted_values': ( 'forecast.html#mlforecast._compute_fitted_values',
+                                                                                                'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast._conformity_scores': ( 'forecast.html#mlforecast._conformity_scores',
                                                                                             'mlforecast/forecast.py'),
+                                     'mlforecast.forecast.MLForecast._invert_transforms_fitted': ( 'forecast.html#mlforecast._invert_transforms_fitted',
+                                                                                                   'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.cross_validation': ( 'forecast.html#mlforecast.cross_validation',
                                                                                           'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.cross_validation_fitted_values': ( 'forecast.html#mlforecast.cross_validation_fitted_values',
                                                                                                         'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.fit': ('forecast.html#mlforecast.fit', 'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.fit_models': ( 'forecast.html#mlforecast.fit_models',
                                                                                     'mlforecast/forecast.py'),
@@ -145,14 +149,16 @@
                                                                                                     'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.expand_target': ( 'grouped_array.html#groupedarray.expand_target',
                                                                                                    'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.from_sorted_df': ( 'grouped_array.html#groupedarray.from_sorted_df',
                                                                                                     'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.restore_difference': ( 'grouped_array.html#groupedarray.restore_difference',
                                                                                                         'mlforecast/grouped_array.py'),
+                                          'mlforecast.grouped_array.GroupedArray.restore_fitted_difference': ( 'grouped_array.html#groupedarray.restore_fitted_difference',
+                                                                                                               'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.take': ( 'grouped_array.html#groupedarray.take',
                                                                                           'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.take_from_groups': ( 'grouped_array.html#groupedarray.take_from_groups',
                                                                                                       'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.transform_series': ( 'grouped_array.html#groupedarray.transform_series',
                                                                                                       'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array._append_one': ( 'grouped_array.html#_append_one',
@@ -162,14 +168,16 @@
                                           'mlforecast.grouped_array._apply_difference': ( 'grouped_array.html#_apply_difference',
                                                                                           'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array._diff': ('grouped_array.html#_diff', 'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array._expand_target': ( 'grouped_array.html#_expand_target',
                                                                                        'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array._restore_difference': ( 'grouped_array.html#_restore_difference',
                                                                                             'mlforecast/grouped_array.py'),
+                                          'mlforecast.grouped_array._restore_fitted_difference': ( 'grouped_array.html#_restore_fitted_difference',
+                                                                                                   'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array._transform_series': ( 'grouped_array.html#_transform_series',
                                                                                           'mlforecast/grouped_array.py')},
             'mlforecast.lgb_cv': { 'mlforecast.lgb_cv.LightGBMCV': ('lgb_cv.html#lightgbmcv', 'mlforecast/lgb_cv.py'),
                                    'mlforecast.lgb_cv.LightGBMCV.__init__': ('lgb_cv.html#lightgbmcv.__init__', 'mlforecast/lgb_cv.py'),
                                    'mlforecast.lgb_cv.LightGBMCV.__repr__': ('lgb_cv.html#lightgbmcv.__repr__', 'mlforecast/lgb_cv.py'),
                                    'mlforecast.lgb_cv.LightGBMCV._multithreaded_partial_fit': ( 'lgb_cv.html#lightgbmcv._multithreaded_partial_fit',
                                                                                                 'mlforecast/lgb_cv.py'),
@@ -191,46 +199,51 @@
                                    'mlforecast.lgb_cv._update_and_predict': ('lgb_cv.html#_update_and_predict', 'mlforecast/lgb_cv.py')},
             'mlforecast.target_transforms': { 'mlforecast.target_transforms.BaseTargetTransform': ( 'target_transforms.html#basetargettransform',
                                                                                                     'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.BaseTargetTransform.fit_transform': ( 'target_transforms.html#basetargettransform.fit_transform',
                                                                                                                   'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.BaseTargetTransform.inverse_transform': ( 'target_transforms.html#basetargettransform.inverse_transform',
                                                                                                                       'mlforecast/target_transforms.py'),
+                                              'mlforecast.target_transforms.BaseTargetTransform.inverse_transform_fitted': ( 'target_transforms.html#basetargettransform.inverse_transform_fitted',
+                                                                                                                             'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.BaseTargetTransform.set_column_names': ( 'target_transforms.html#basetargettransform.set_column_names',
                                                                                                                      'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.Differences': ( 'target_transforms.html#differences',
                                                                                             'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.Differences.__init__': ( 'target_transforms.html#differences.__init__',
                                                                                                      'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.Differences.fit_transform': ( 'target_transforms.html#differences.fit_transform',
                                                                                                           'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.Differences.inverse_transform': ( 'target_transforms.html#differences.inverse_transform',
                                                                                                               'mlforecast/target_transforms.py'),
+                                              'mlforecast.target_transforms.Differences.inverse_transform_fitted': ( 'target_transforms.html#differences.inverse_transform_fitted',
+                                                                                                                     'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.GlobalSklearnTransformer': ( 'target_transforms.html#globalsklearntransformer',
                                                                                                          'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.GlobalSklearnTransformer.__init__': ( 'target_transforms.html#globalsklearntransformer.__init__',
                                                                                                                   'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.GlobalSklearnTransformer.fit_transform': ( 'target_transforms.html#globalsklearntransformer.fit_transform',
                                                                                                                        'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.GlobalSklearnTransformer.inverse_transform': ( 'target_transforms.html#globalsklearntransformer.inverse_transform',
                                                                                                                            'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.LocalStandardScaler': ( 'target_transforms.html#localstandardscaler',
                                                                                                     'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.LocalStandardScaler.fit_transform': ( 'target_transforms.html#localstandardscaler.fit_transform',
                                                                                                                   'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms.LocalStandardScaler.inverse_transform': ( 'target_transforms.html#localstandardscaler.inverse_transform',
                                                                                                                       'mlforecast/target_transforms.py'),
-                                              'mlforecast.target_transforms._standard_scaler_inverse_transform': ( 'target_transforms.html#_standard_scaler_inverse_transform',
-                                                                                                                   'mlforecast/target_transforms.py'),
+                                              'mlforecast.target_transforms.LocalStandardScaler.inverse_transform_fitted': ( 'target_transforms.html#localstandardscaler.inverse_transform_fitted',
+                                                                                                                             'mlforecast/target_transforms.py'),
                                               'mlforecast.target_transforms._standard_scaler_transform': ( 'target_transforms.html#_standard_scaler_transform',
                                                                                                            'mlforecast/target_transforms.py')},
             'mlforecast.utils': { 'mlforecast.utils.PredictionIntervals': ('utils.html#predictionintervals', 'mlforecast/utils.py'),
                                   'mlforecast.utils.PredictionIntervals.__init__': ( 'utils.html#predictionintervals.__init__',
                                                                                      'mlforecast/utils.py'),
                                   'mlforecast.utils.PredictionIntervals.__repr__': ( 'utils.html#predictionintervals.__repr__',
                                                                                      'mlforecast/utils.py'),
+                                  'mlforecast.utils._ensure_shallow_copy': ('utils.html#_ensure_shallow_copy', 'mlforecast/utils.py'),
                                   'mlforecast.utils.backtest_splits': ('utils.html#backtest_splits', 'mlforecast/utils.py'),
                                   'mlforecast.utils.generate_daily_series': ('utils.html#generate_daily_series', 'mlforecast/utils.py'),
                                   'mlforecast.utils.generate_prices_for_series': ( 'utils.html#generate_prices_for_series',
                                                                                    'mlforecast/utils.py'),
                                   'mlforecast.utils.old_kw_to_pos': ('utils.html#old_kw_to_pos', 'mlforecast/utils.py'),
                                   'mlforecast.utils.single_split': ('utils.html#single_split', 'mlforecast/utils.py')}}}
```

### Comparing `mlforecast-0.9.2/mlforecast/core.py` & `mlforecast-0.9.3/mlforecast/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import numpy as np
 import pandas as pd
 from numba import njit
 from sklearn.base import BaseEstimator
 
 from .grouped_array import GroupedArray
 from .target_transforms import BaseTargetTransform, Differences
+from .utils import _ensure_shallow_copy
 
 # %% ../nbs/core.ipynb 10
 date_features_dtypes = {
     "year": np.uint16,
     "month": np.uint8,
     "day": np.uint8,
     "hour": np.uint8,
@@ -365,19 +366,15 @@
         # assemble return
         if return_X_y:
             return df, target
         if max_horizon is not None:
             for i in range(max_horizon):
                 df[f"{self.target_col}{i}"] = target[:, i]
         else:
-            from packaging.version import Version
-
-            if Version(pd.__version__) < Version("1.4"):
-                # https://github.com/pandas-dev/pandas/pull/43406
-                df = df.copy()
+            df = _ensure_shallow_copy(df)
             df[self.target_col] = target
         return df
 
     def fit_transform(
         self,
         data: pd.DataFrame,
         id_col: str,
```

### Comparing `mlforecast-0.9.2/mlforecast/distributed/forecast.py` & `mlforecast-0.9.3/mlforecast/distributed/forecast.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.9.2/mlforecast/distributed/models/dask/lgb.py` & `mlforecast-0.9.3/mlforecast/distributed/models/dask/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.9.2/mlforecast/distributed/models/dask/xgb.py` & `mlforecast-0.9.3/mlforecast/distributed/models/dask/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.9.2/mlforecast/distributed/models/ray/xgb.py` & `mlforecast-0.9.3/mlforecast/distributed/models/ray/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.9.2/mlforecast/distributed/models/spark/lgb.py` & `mlforecast-0.9.3/mlforecast/distributed/models/spark/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.9.2/mlforecast/distributed/models/spark/xgb.py` & `mlforecast-0.9.3/mlforecast/distributed/models/spark/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.9.2/mlforecast/forecast.py` & `mlforecast-0.9.3/mlforecast/forecast.py`

 * *Files 7% similar despite different names*

```diff
@@ -321,14 +321,73 @@
         )
         # conformity score for each model
         for model in self.models.keys():
             # compute absolute error for each model
             cv_results[model] = np.abs(cv_results[model] - cv_results[target_col])
         return cv_results.drop(columns=target_col)
 
+    def _invert_transforms_fitted(self, df: pd.DataFrame) -> pd.DataFrame:
+        if self.ts.target_transforms is None:
+            return df
+        sizes = df.groupby(self.ts.id_col, observed=True).size().values
+        for tfm in self.ts.target_transforms[::-1]:
+            df = tfm.inverse_transform_fitted(df, sizes)
+        return df
+
+    def _compute_fitted_values(
+        self,
+        X_with_info: pd.DataFrame,
+        y: np.ndarray,
+        id_col: str,
+        time_col: str,
+        target_col: str,
+        max_horizon: Optional[int],
+    ) -> pd.DataFrame:
+        base = X_with_info[[id_col, time_col]].copy(deep=False)
+        X = X_with_info[self.ts.features_order_]
+        idx = pd.MultiIndex.from_frame(base)
+        if not idx.is_monotonic_increasing:
+            sort_idxs: Optional[np.ndarray] = idx.argsort()
+        else:
+            sort_idxs = None
+        if max_horizon is None:
+            fitted_values = base
+            fitted_values[target_col] = y
+            if sort_idxs is not None:
+                fitted_values = fitted_values.iloc[sort_idxs]
+            for name, model in self.models_.items():
+                assert not isinstance(model, list)  # mypy
+                fitted_values[name] = model.predict(X)
+            fitted_values = self._invert_transforms_fitted(fitted_values)
+        else:
+            horizon_fitted_values = []
+            for horizon in range(max_horizon):
+                horizon_base = base.copy()
+                horizon_base[target_col] = y[:, horizon]
+                if sort_idxs is not None:
+                    horizon_base = horizon_base.iloc[sort_idxs]
+                horizon_fitted_values.append(horizon_base)
+            for name, horizon_models in self.models_.items():
+                for horizon, model in enumerate(horizon_models):
+                    horizon_fitted_values[horizon][name] = model.predict(X)
+            for horizon, horizon_df in enumerate(horizon_fitted_values):
+                keep_mask = horizon_df[target_col].notnull()
+                horizon_df = horizon_df[keep_mask].copy()
+                horizon_df = self._invert_transforms_fitted(horizon_df)
+                horizon_df["h"] = horizon + 1
+                horizon_fitted_values[horizon] = horizon_df
+            fitted_values = pd.concat(horizon_fitted_values)
+        if self.ts.target_transforms is not None:
+            for tfm in self.ts.target_transforms[::-1]:
+                if hasattr(tfm, "store_fitted"):
+                    tfm.store_fitted = False
+                if hasattr(tfm, "fitted_"):
+                    tfm.fitted_ = []
+        return fitted_values
+
     @old_kw_to_pos(["data"], [1])
     def fit(
         self,
         df: pd.DataFrame,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
@@ -370,14 +429,18 @@
             Series data in long format. This argument has been replaced by df and will be removed in a later release.
 
         Returns
         -------
         self : MLForecast
             Forecast object with series values and trained models.
         """
+        if fitted and self.ts.target_transforms is not None:
+            for tfm in self.ts.target_transforms:
+                if hasattr(tfm, "store_fitted"):
+                    tfm.store_fitted = True
         self._cs_df: Optional[pd.DataFrame] = None
         if prediction_intervals is not None:
             self.prediction_intervals = prediction_intervals
             self._cs_df = self._conformity_scores(
                 df=df,
                 id_col=id_col,
                 time_col=time_col,
@@ -398,33 +461,23 @@
             keep_last_n=keep_last_n,
             max_horizon=max_horizon,
             return_X_y=True,
         )
         X = X_with_info[self.ts.features_order_]
         self.fit_models(X, y)
         if fitted:
-            base = X_with_info[[id_col, time_col, target_col]].copy(deep=False)
-            if max_horizon is None:
-                self.fcst_fitted_values_ = base
-                for name, model in self.models_.items():
-                    assert not isinstance(model, list)  # mypy
-                    self.fcst_fitted_values_[name] = model.predict(X)
-            else:
-                fitted_values = []
-                for h in range(max_horizon):
-                    horizon_base = base[[id_col, time_col]].copy()
-                    horizon_base["h"] = h
-                    horizon_base[target_col] = y[:, h]
-                    fitted_values.append(horizon_base)
-                for name, horizon_models in self.models_.items():
-                    for h, model in enumerate(horizon_models):
-                        fitted_values[h][name] = model.predict(X)
-                self.fcst_fitted_values_ = pd.concat(fitted_values).reset_index(
-                    drop=True
-                )
+            fitted_values = self._compute_fitted_values(
+                X_with_info=X_with_info,
+                y=y,
+                id_col=id_col,
+                time_col=time_col,
+                target_col=target_col,
+                max_horizon=max_horizon,
+            )
+            self.fcst_fitted_values_ = fitted_values.reset_index(drop=True)
         return self
 
     def forecast_fitted_values(self):
         """Access in-sample predictions."""
         if not hasattr(self, "fcst_fitted_values_"):
             raise Exception("Please run the `fit` method using `fitted=True`")
         return self.fcst_fitted_values_
@@ -482,14 +535,27 @@
         result : pandas DataFrame
             Predictions for each serie and timestep, with one column per model.
         """
         if not hasattr(self, "models_"):
             raise ValueError(
                 "No fitted models found. You have to call fit or preprocess + fit_models."
             )
+        first_model_is_list = isinstance(next(iter(self.models_.values())), list)
+        max_horizon = self.ts.max_horizon
+        if first_model_is_list and max_horizon is None:
+            raise ValueError(
+                "Found one model per horizon but `max_horizon` is None. "
+                "If you ran preprocess after fit please run fit again."
+            )
+        elif not first_model_is_list and max_horizon is not None:
+            raise ValueError(
+                "Found a single model for all horizons "
+                f"but `max_horizon` is {max_horizon}. "
+                "If you ran preprocess after fit please run fit again."
+            )
         if new_data is not None:
             warnings.warn(
                 "`new_data` has been deprecated, please use `new_df` instead.",
                 DeprecationWarning,
             )
             new_df = new_data
         if dynamic_dfs is not None:
@@ -685,38 +751,47 @@
                     time_col=time_col,
                     target_col=target_col,
                     static_features=static_features,
                     dropna=dropna,
                     keep_last_n=keep_last_n,
                     max_horizon=max_horizon,
                     prediction_intervals=prediction_intervals,
+                    fitted=fitted,
                 )
                 self.cv_models_.append(self.models_)
-            if fitted:
-                insample_results = train[[id_col, time_col]].copy()
-                trainX, _ = self.preprocess(
+                if fitted:
+                    self.cv_fitted_values_.append(
+                        self.fcst_fitted_values_.assign(fold=i_window)
+                    )
+            if fitted and not should_fit:
+                if self.ts.target_transforms is not None:
+                    for tfm in self.ts.target_transforms:
+                        if hasattr(tfm, "store_fitted"):
+                            tfm.store_fitted = True
+                train_X, train_y = self.preprocess(
                     train,
                     id_col=id_col,
                     time_col=time_col,
                     target_col=target_col,
                     static_features=static_features,
-                    dropna=False,
+                    dropna=dropna,
                     keep_last_n=keep_last_n,
                     max_horizon=max_horizon,
                     return_X_y=True,
                 )
-                trainX = trainX[self.ts.features_order_]
-                for name, model in self.models_.items():
-                    insample_results[name] = model.predict(trainX)  # type: ignore[union-attr]
-                if self.ts.target_transforms is not None:
-                    for tfm in self.ts.target_transforms[::-1]:
-                        insample_results = tfm.inverse_transform(insample_results)
-                insample_results["fold"] = i_window
-                insample_results[target_col] = train[target_col].values
-                self.cv_fitted_values_.append(insample_results)
+                fitted_values = self._compute_fitted_values(
+                    X_with_info=train_X,
+                    y=train_y,
+                    id_col=id_col,
+                    time_col=time_col,
+                    target_col=target_col,
+                    max_horizon=max_horizon,
+                )
+                fitted_values["fold"] = i_window
+                self.cv_fitted_values_.append(fitted_values)
             static = self.ts.static_features_.columns.drop(id_col).tolist()
             dynamic = valid.columns.drop(static + [id_col, time_col, target_col])
             if not dynamic.empty:
                 X_df = valid.drop(columns=static + [target_col])
             else:
                 X_df = None
             y_pred = self.predict(
```

### Comparing `mlforecast-0.9.2/mlforecast/grouped_array.py` & `mlforecast-0.9.3/mlforecast/grouped_array.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,26 @@
         for j in range(min(h, d)):
             preds[i * h + j] += s[j]
         for j in range(d, h):
             preds[i * h + j] += preds[i * h + j - d]
 
 
 @njit
+def _restore_fitted_difference(diffs_data, diffs_indptr, data, indptr, d):
+    n_series = len(indptr) - 1
+    for i in range(n_series):
+        serie = data[indptr[i] : indptr[i + 1]]
+        diffs_size = diffs_indptr[i + 1] - diffs_indptr[i]
+        dropped_rows = diffs_size - serie.size
+        start_idx = max(0, d - dropped_rows)
+        for j in range(start_idx, serie.size):
+            serie[j] += diffs_data[diffs_indptr[i + 1] - serie.size - d + j]
+
+
+@njit
 def _expand_target(data, indptr, max_horizon):
     out = np.empty((data.size, max_horizon), dtype=data.dtype)
     n_series = len(indptr) - 1
     n = 0
     for i in range(n_series):
         serie = data[indptr[i] : indptr[i + 1]]
         for j in range(serie.size):
@@ -174,17 +186,30 @@
         return cls(data, indptr)
 
     def transform_series(
         self, updates_only: bool, lag: int, func: Callable, *args
     ) -> np.ndarray:
         return _transform_series(self.data, self.indptr, updates_only, lag, func, *args)
 
-    def restore_difference(self, preds: np.ndarray, d: int):
+    def restore_difference(self, preds: np.ndarray, d: int) -> None:
         _restore_difference(preds, self.data, self.indptr, d)
 
+    def restore_fitted_difference(
+        self, series_data: np.ndarray, series_indptr: np.ndarray, d: int
+    ) -> None:
+        if len(self.indptr) != len(series_indptr):
+            raise ValueError("Found different number of groups in fitted differences.")
+        _restore_fitted_difference(
+            self.data,
+            self.indptr,
+            series_data,
+            series_indptr,
+            d,
+        )
+
     def expand_target(self, max_horizon: int) -> np.ndarray:
         return _expand_target(self.data, self.indptr, max_horizon)
 
     def take_from_groups(self, idx: Union[int, slice]) -> "GroupedArray":
         """Takes `idx` from each group in the array."""
         ranges = [
             range(self.indptr[i], self.indptr[i + 1])[idx] for i in range(self.ngroups)
```

### Comparing `mlforecast-0.9.2/mlforecast/lgb_cv.py` & `mlforecast-0.9.3/mlforecast/lgb_cv.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.9.2/mlforecast/target_transforms.py` & `mlforecast-0.9.3/mlforecast/target_transforms.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 # %% auto 0
 __all__ = ['BaseTargetTransform', 'Differences', 'LocalStandardScaler', 'GlobalSklearnTransformer']
 
 # %% ../nbs/target_transforms.ipynb 3
 import abc
 import reprlib
-from typing import Iterable, Optional
+from typing import Iterable, List, Optional
 
 import numpy as np
 import pandas as pd
 from sklearn.base import TransformerMixin, clone
 from numba import njit
 
 from .grouped_array import GroupedArray, _apply_difference
+from .utils import _ensure_shallow_copy
 
 # %% ../nbs/target_transforms.ipynb 5
 class BaseTargetTransform(abc.ABC):
     """Base class used for target transformations."""
 
     idxs: Optional[np.ndarray] = None
 
@@ -30,105 +31,138 @@
     def fit_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         raise NotImplementedError
 
     @abc.abstractmethod
     def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         raise NotImplementedError
 
+    def inverse_transform_fitted(
+        self, df: pd.DataFrame, _sizes: np.ndarray
+    ) -> pd.DataFrame:
+        return self.inverse_transform(df)
+
 # %% ../nbs/target_transforms.ipynb 6
 class Differences(BaseTargetTransform):
     """Subtracts previous values of the serie. Can be used to remove trend or seasonalities."""
 
+    store_fitted = False
+
     def __init__(self, differences: Iterable[int]):
         self.differences = list(differences)
 
     def fit_transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        self.fitted_: List[GroupedArray] = []
         ga = GroupedArray.from_sorted_df(df, self.id_col, self.target_col)
-        uids = df[self.id_col].unique()
-        original_sizes = ga.indptr[1:].cumsum()
+        original_sizes = np.diff(ga.indptr)
         total_diffs = sum(self.differences)
-        small_series = uids[original_sizes < total_diffs]
-        if small_series.size:
-            msg = reprlib.repr(small_series.tolist())
+        small_series = original_sizes < total_diffs
+        if small_series.any():
+            uids = df[self.id_col].unique()
+            msg = reprlib.repr(uids[small_series].tolist())
             raise ValueError(
                 f"The following series are too short for the differences: {msg}"
             )
         self.original_values_ = []
         n_series = len(ga.indptr) - 1
         for d in self.differences:
+            if self.store_fitted:
+                # these are saved in order to be able to perform a correct
+                # inverse transform when trying to retrieve the fitted values.
+                self.fitted_.append(GroupedArray(ga.data.copy(), ga.indptr.copy()))
             new_data = np.empty_like(ga.data, shape=n_series * d)
             new_indptr = d * np.arange(n_series + 1, dtype=np.int32)
             _apply_difference(ga.data, ga.indptr, new_data, new_indptr, d)
             self.original_values_.append(GroupedArray(new_data, new_indptr))
         df = df.copy(deep=False)
+        df = _ensure_shallow_copy(df)
         df[self.target_col] = ga.data
         return df
 
     def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         model_cols = df.columns.drop([self.id_col, self.time_col])
         df = df.copy(deep=False)
+        df = _ensure_shallow_copy(df)
         for model in model_cols:
             model_preds = df[model].values.copy()
             for d, ga in zip(
                 reversed(self.differences), reversed(self.original_values_)
             ):
                 if self.idxs is not None:
                     ga = ga.take(self.idxs)
                 ga.restore_difference(model_preds, d)
             df[model] = model_preds
         return df
 
-# %% ../nbs/target_transforms.ipynb 7
+    def inverse_transform_fitted(
+        self, df: pd.DataFrame, sizes: np.ndarray
+    ) -> pd.DataFrame:
+        model_cols = df.columns.drop([self.id_col, self.time_col])
+        df = df.copy(deep=False)
+        df = _ensure_shallow_copy(df)
+        indptr = np.append(0, sizes.cumsum())
+        for model in model_cols:
+            model_preds = df[model].values.copy()
+            for d, ga in zip(reversed(self.differences), reversed(self.fitted_)):
+                ga.restore_fitted_difference(model_preds, indptr, d)
+            df[model] = model_preds
+        return df
+
+# %% ../nbs/target_transforms.ipynb 9
 @njit
 def _standard_scaler_transform(data, indptr, stats, out):
     n_series = len(indptr) - 1
     for i in range(n_series):
         sl = slice(indptr[i], indptr[i + 1])
         subs = data[sl]
         mean_ = np.nanmean(subs)
         std_ = np.nanstd(subs)
         stats[i] = mean_, std_
         out[sl] = (data[sl] - mean_) / std_
 
-
-@njit
-def _standard_scaler_inverse_transform(preds, stats):
-    n_series = stats.shape[0]
-    h = preds.size // n_series
-    k = 0
-    for i in range(n_series):
-        mean_, std_ = stats[i]
-        for _ in range(h):
-            preds[k] = preds[k] * std_ + mean_
-            k += 1
-
-# %% ../nbs/target_transforms.ipynb 8
+# %% ../nbs/target_transforms.ipynb 10
 class LocalStandardScaler(BaseTargetTransform):
     """Standardizes each serie by subtracting its mean and dividing by its standard deviation."""
 
-    def fit_transform(self, df: "pd.DataFrame") -> "pd.DataFrame":
+    def fit_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         ga = GroupedArray.from_sorted_df(df, self.id_col, self.target_col)
         self.stats_ = np.empty((len(ga.indptr) - 1, 2))
         out = np.empty_like(ga.data)
         _standard_scaler_transform(ga.data, ga.indptr, self.stats_, out)
         df = df.copy(deep=False)
+        df = _ensure_shallow_copy(df)
         df[self.target_col] = out
         return df
 
-    def inverse_transform(self, df: "pd.DataFrame") -> "pd.DataFrame":
+    def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         df = df.copy(deep=False)
+        df = _ensure_shallow_copy(df)
+        stats = self.stats_
+        if self.idxs is not None:
+            stats = stats[self.idxs]
+        h = df.shape[0] // stats.shape[0]
+        means = np.repeat(stats[:, 0], h)
+        stds = np.repeat(stats[:, 1], h)
         model_cols = df.columns.drop([self.id_col, self.time_col])
-        stats = self.stats_ if self.idxs is None else self.stats_[self.idxs]
         for model in model_cols:
-            model_preds = df[model].values
-            _standard_scaler_inverse_transform(model_preds, stats)
-            df[model] = model_preds
+            df[model] = df[model].values * stds + means
         return df
 
-# %% ../nbs/target_transforms.ipynb 10
+    def inverse_transform_fitted(
+        self, df: pd.DataFrame, sizes: np.ndarray
+    ) -> pd.DataFrame:
+        df = df.copy(deep=False)
+        df = _ensure_shallow_copy(df)
+        means = np.repeat(self.stats_[:, 0], sizes)
+        stds = np.repeat(self.stats_[:, 1], sizes)
+        model_cols = df.columns.drop([self.id_col, self.time_col])
+        for model in model_cols:
+            df[model] = df[model].values * stds + means
+        return df
+
+# %% ../nbs/target_transforms.ipynb 12
 class GlobalSklearnTransformer(BaseTargetTransform):
     """Applies the same scikit-learn transformer to all series."""
 
     def __init__(self, transformer: TransformerMixin):
         self.transformer = transformer
 
     def fit_transform(self, df: pd.DataFrame) -> pd.DataFrame:
```

### Comparing `mlforecast-0.9.2/mlforecast/utils.py` & `mlforecast-0.9.3/mlforecast/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,7 +210,16 @@
             raise ValueError(f"method must be one of {allowed_methods}")
         self.n_windows = n_windows
         self.h = h
         self.method = method
 
     def __repr__(self):
         return f"PredictionIntervals(n_windows={self.n_windows}, h={self.h}, method='{self.method}')"
+
+# %% ../nbs/utils.ipynb 25
+def _ensure_shallow_copy(df: pd.DataFrame) -> pd.DataFrame:
+    from packaging.version import Version
+
+    if Version(pd.__version__) < Version("1.4"):
+        # https://github.com/pandas-dev/pandas/pull/43406
+        df = df.copy()
+    return df
```

### Comparing `mlforecast-0.9.2/mlforecast.egg-info/PKG-INFO` & `mlforecast-0.9.3/mlforecast.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.9.2
+Version: 0.9.3
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
@@ -14,17 +14,44 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numba
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
+Requires-Dist: window-ops
 Provides-Extra: distributed
+Requires-Dist: dask[complete]; extra == "distributed"
+Requires-Dist: fugue[ray]; extra == "distributed"
+Requires-Dist: pyspark; extra == "distributed"
+Requires-Dist: lightgbm_ray; extra == "distributed"
+Requires-Dist: xgboost_ray; extra == "distributed"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: numba; extra == "dev"
+Requires-Dist: pandas; extra == "dev"
+Requires-Dist: scikit-learn; extra == "dev"
+Requires-Dist: window-ops; extra == "dev"
+Requires-Dist: dask[complete]; extra == "dev"
+Requires-Dist: fugue[ray]; extra == "dev"
+Requires-Dist: pyspark; extra == "dev"
+Requires-Dist: lightgbm_ray; extra == "dev"
+Requires-Dist: xgboost_ray; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: datasetsforecast; extra == "dev"
+Requires-Dist: lightgbm; extra == "dev"
+Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: utilsforecast; extra == "dev"
+Requires-Dist: xgboost; extra == "dev"
 
 Nixtla  
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting)
  [![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
```

### Comparing `mlforecast-0.9.2/mlforecast.egg-info/SOURCES.txt` & `mlforecast-0.9.3/mlforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlforecast-0.9.2/settings.ini` & `mlforecast-0.9.3/settings.ini`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 user = Nixtla
 description = Scalable machine learning based time series forecasting
 keywords = python forecast forecasting machine-learning dask
 author = José Morales
 author_email = jmoralz92@gmail.com
 copyright = Nixtla
 branch = main
-version = 0.9.2
+version = 0.9.3
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 3
 requirements = numba pandas scikit-learn window-ops
 distributed_requirements = dask[complete] fugue[ray] pyspark lightgbm_ray xgboost_ray
-dev_requirements = black datasetsforecast lightgbm matplotlib mypy nbdev ruff statsforecast xgboost
+dev_requirements = black datasetsforecast lightgbm matplotlib mypy nbdev ruff utilsforecast xgboost
 nbs_path = nbs
 doc_path = _docs
 recursive = True
 doc_host = https://Nixtla.github.io
 doc_baseurl = /
 git_url = https://github.com/Nixtla/mlforecast
 lib_path = mlforecast
```

### Comparing `mlforecast-0.9.2/setup.py` & `mlforecast-0.9.3/setup.py`

 * *Files identical despite different names*

