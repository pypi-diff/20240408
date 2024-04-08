# Comparing `tmp/statsforecast-1.7.3.tar.gz` & `tmp/statsforecast-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statsforecast-1.7.3.tar", last modified: Mon Feb  5 21:45:22 2024, max compression
+gzip compressed data, was "statsforecast-1.7.4.tar", last modified: Mon Apr  8 16:44:27 2024, max compression
```

## Comparing `statsforecast-1.7.3.tar` & `statsforecast-1.7.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 21:45:22.306483 statsforecast-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-02-05 21:45:14.000000 statsforecast-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-05 21:45:14.000000 statsforecast-1.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27400 2024-02-05 21:45:22.306483 statsforecast-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24960 2024-02-05 21:45:14.000000 statsforecast-1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 21:45:22.298483 statsforecast-1.7.3/action_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 21:45:14.000000 statsforecast-1.7.3/action_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-02-05 21:45:14.000000 statsforecast-1.7.3/action_files/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-05 21:45:14.000000 statsforecast-1.7.3/action_files/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-02-05 21:45:14.000000 statsforecast-1.7.3/action_files/test_fit_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-02-05 21:45:14.000000 statsforecast-1.7.3/action_files/test_ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-05 21:45:14.000000 statsforecast-1.7.3/action_files/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-02-05 21:45:14.000000 statsforecast-1.7.3/action_files/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-05 21:45:14.000000 statsforecast-1.7.3/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 21:45:22.306483 statsforecast-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-05 21:45:14.000000 statsforecast-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 21:45:22.302483 statsforecast-1.7.3/statsforecast/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    99251 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/_modidx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 21:45:22.302483 statsforecast-1.7.3/statsforecast/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/adapters/prophet.py
--rw-r--r--   0 runner    (1001) docker     (127)    85815 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/arima.py
--rw-r--r--   0 runner    (1001) docker     (127)    22508 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/ces.py
--rw-r--r--   0 runner    (1001) docker     (127)    61201 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 21:45:22.302483 statsforecast-1.7.3/statsforecast/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/distributed/fugue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/distributed/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    48393 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/ets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/garch.py
--rw-r--r--   0 runner    (1001) docker     (127)   211953 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/mstl.py
--rw-r--r--   0 runner    (1001) docker     (127)    28315 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/tbats.py
--rw-r--r--   0 runner    (1001) docker     (127)    20374 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/theta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-02-05 21:45:14.000000 statsforecast-1.7.3/statsforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 21:45:22.302483 statsforecast-1.7.3/statsforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27400 2024-02-05 21:45:22.000000 statsforecast-1.7.3/statsforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-05 21:45:22.000000 statsforecast-1.7.3/statsforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 21:45:22.000000 statsforecast-1.7.3/statsforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-05 21:45:22.000000 statsforecast-1.7.3/statsforecast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 21:45:22.000000 statsforecast-1.7.3/statsforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-05 21:45:22.000000 statsforecast-1.7.3/statsforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 21:45:22.000000 statsforecast-1.7.3/statsforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.718387 statsforecast-1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-08 16:44:21.000000 statsforecast-1.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 16:44:21.000000 statsforecast-1.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27435 2024-04-08 16:44:27.718387 statsforecast-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24960 2024-04-08 16:44:21.000000 statsforecast-1.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.710387 statsforecast-1.7.4/action_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/test_fit_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/test_ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-08 16:44:21.000000 statsforecast-1.7.4/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:44:27.718387 statsforecast-1.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-08 16:44:21.000000 statsforecast-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.710387 statsforecast-1.7.4/statsforecast/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99387 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/_modidx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.714387 statsforecast-1.7.4/statsforecast/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/adapters/prophet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85815 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/arima.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22508 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/ces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61494 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.714387 statsforecast-1.7.4/statsforecast/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16721 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/distributed/fugue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/distributed/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48393 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/ets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/garch.py
+-rw-r--r--   0 runner    (1001) docker     (127)   212642 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/mstl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29166 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/tbats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20374 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/theta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.714387 statsforecast-1.7.4/statsforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27435 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/top_level.txt
```

### Comparing `statsforecast-1.7.3/LICENSE` & `statsforecast-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/PKG-INFO` & `statsforecast-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statsforecast
-Version: 1.7.3
+Version: 1.7.4
 Summary: Time series forecasting suite using statistical models
 Home-page: https://github.com/Nixtla/statsforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting arima ets
 Classifier: Development Status :: 3 - Alpha
@@ -15,44 +15,45 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudpickle
+Requires-Dist: coreforecast>=0.0.7
 Requires-Dist: numba>=0.55.0
 Requires-Dist: numpy>=1.21.6
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: statsmodels>=0.13.2
 Requires-Dist: tqdm
 Requires-Dist: fugue>=0.8.1
 Requires-Dist: utilsforecast>=0.0.24
 Requires-Dist: threadpoolctl
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pmdarima; extra == "dev"
+Requires-Dist: fugue[ray]>=0.8.1; extra == "dev"
+Requires-Dist: scikit-learn; extra == "dev"
+Requires-Dist: nbdev_plotly; extra == "dev"
+Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: polars; extra == "dev"
+Requires-Dist: plotly; extra == "dev"
+Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
+Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "dev"
+Requires-Dist: fugue[dask]>=0.8.1; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
+Requires-Dist: prophet; extra == "dev"
+Requires-Dist: datasetsforecast; extra == "dev"
 Requires-Dist: supersmoother; extra == "dev"
+Requires-Dist: pandas[plot]; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: ray<2.8; extra == "dev"
 Requires-Dist: fugue[spark]>=0.8.1; extra == "dev"
-Requires-Dist: plotly; extra == "dev"
-Requires-Dist: nbdev_plotly; extra == "dev"
-Requires-Dist: fugue[ray]>=0.8.1; extra == "dev"
-Requires-Dist: pyarrow; extra == "dev"
-Requires-Dist: pandas[plot]; extra == "dev"
-Requires-Dist: datasetsforecast; extra == "dev"
-Requires-Dist: prophet; extra == "dev"
-Requires-Dist: fugue[dask]>=0.8.1; extra == "dev"
-Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "dev"
-Requires-Dist: scikit-learn; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
-Requires-Dist: plotly-resampler; extra == "dev"
-Requires-Dist: polars; extra == "dev"
 Provides-Extra: dask
 Requires-Dist: fugue[dask]>=0.8.1; extra == "dask"
 Provides-Extra: ray
 Requires-Dist: fugue[ray]>=0.8.1; extra == "ray"
 Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "ray"
 Requires-Dist: ray<2.8; extra == "ray"
 Provides-Extra: spark
```

### Comparing `statsforecast-1.7.3/README.md` & `statsforecast-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/action_files/conftest.py` & `statsforecast-1.7.4/action_files/conftest.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/action_files/test_dask.py` & `statsforecast-1.7.4/action_files/test_dask.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/action_files/test_ray.py` & `statsforecast-1.7.4/action_files/test_ray.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/action_files/test_spark.py` & `statsforecast-1.7.4/action_files/test_spark.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/action_files/utils.py` & `statsforecast-1.7.4/action_files/utils.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/settings.ini` & `statsforecast-1.7.4/settings.ini`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 user = Nixtla
 description = Time series forecasting suite using statistical models
 keywords = time-series forecasting arima ets 
 author = Nixtla
 author_email = business@nixtla.io
 copyright = Nixtla Inc.
 branch = main
-version = 1.7.3
+version = 1.7.4
 min_python = 3.8
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 2
-requirements = cloudpickle numba>=0.55.0 numpy>=1.21.6 pandas>=1.3.5 scipy>=1.7.3 statsmodels>=0.13.2 tqdm fugue>=0.8.1 utilsforecast>=0.0.24 threadpoolctl
+requirements = cloudpickle coreforecast>=0.0.7 numba>=0.55.0 numpy>=1.21.6 pandas>=1.3.5 scipy>=1.7.3 statsmodels>=0.13.2 tqdm fugue>=0.8.1 utilsforecast>=0.0.24 threadpoolctl
 polars_requirements = polars
 ray_requirements = fugue[ray]>=0.8.1 protobuf>=3.15.3,<4.0.0 ray<2.8
 dask_requirements = fugue[dask]>=0.8.1
 spark_requirements = fugue[spark]>=0.8.1
 plotly_requirements = plotly plotly-resampler
 dev_requirements = nbdev black mypy flake8 pandas[plot] pmdarima prophet pyarrow scikit-learn datasetsforecast supersmoother nbdev_plotly
 nbs_path = nbs
```

### Comparing `statsforecast-1.7.3/setup.py` & `statsforecast-1.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/statsforecast/_modidx.py` & `statsforecast-1.7.4/statsforecast/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -768,12 +768,13 @@
                                      'statsforecast.utils.ConformalIntervals.__init__': ( 'src/utils.html#conformalintervals.__init__',
                                                                                           'statsforecast/utils.py'),
                                      'statsforecast.utils._calculate_intervals': ( 'src/utils.html#_calculate_intervals',
                                                                                    'statsforecast/utils.py'),
                                      'statsforecast.utils._calculate_sigma': ('src/utils.html#_calculate_sigma', 'statsforecast/utils.py'),
                                      'statsforecast.utils._ensure_float': ('src/utils.html#_ensure_float', 'statsforecast/utils.py'),
                                      'statsforecast.utils._naive': ('src/utils.html#_naive', 'statsforecast/utils.py'),
+                                     'statsforecast.utils._old_kw_to_pos': ('src/utils.html#_old_kw_to_pos', 'statsforecast/utils.py'),
                                      'statsforecast.utils._quantiles': ('src/utils.html#_quantiles', 'statsforecast/utils.py'),
                                      'statsforecast.utils._repeat_val': ('src/utils.html#_repeat_val', 'statsforecast/utils.py'),
                                      'statsforecast.utils._repeat_val_seas': ('src/utils.html#_repeat_val_seas', 'statsforecast/utils.py'),
                                      'statsforecast.utils._seasonal_naive': ('src/utils.html#_seasonal_naive', 'statsforecast/utils.py'),
                                      'statsforecast.utils.generate_series': ('src/utils.html#generate_series', 'statsforecast/utils.py')}}}
```

### Comparing `statsforecast-1.7.3/statsforecast/adapters/prophet.py` & `statsforecast-1.7.4/statsforecast/adapters/prophet.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/statsforecast/arima.py` & `statsforecast-1.7.4/statsforecast/arima.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/statsforecast/ces.py` & `statsforecast-1.7.4/statsforecast/ces.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/statsforecast/core.py` & `statsforecast-1.7.4/statsforecast/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1190,22 +1190,24 @@
         # compute parallel forecasts
         result = {}
         with Pool(self.n_jobs, **pool_kwargs) as executor:
             futures = []
             for ga, X_ in zip(gas, Xs):
                 future = executor.apply_async(
                     ga.forecast,
-                    (
-                        self.models,
-                        h,
-                        self.fallback_model,
-                        fitted,
-                        X_,
-                        level,
-                        target_col,
+                    tuple(),
+                    dict(
+                        models=self.models,
+                        h=h,
+                        fallback_model=self.fallback_model,
+                        fitted=fitted,
+                        X=X_,
+                        level=level,
+                        verbose=self.verbose,
+                        target_col=target_col,
                     ),
                 )
                 futures.append(future)
             out = [f.get() for f in futures]
             fcsts = [d["forecasts"] for d in out]
             fcsts = np.vstack(fcsts)
             cols = out[0]["cols"]
@@ -1227,25 +1229,27 @@
         # compute parallel forecasts
         result = {}
         with Pool(self.n_jobs, **pool_kwargs) as executor:
             futures = []
             for ga in gas:
                 future = executor.apply_async(
                     ga.cross_validation,
-                    (
-                        self.models,
-                        h,
-                        test_size,
-                        self.fallback_model,
-                        step_size,
-                        input_size,
-                        fitted,
-                        level,
-                        refit,
-                        target_col,
+                    tuple(),
+                    dict(
+                        models=self.models,
+                        h=h,
+                        test_size=test_size,
+                        fallback_model=self.fallback_model,
+                        step_size=step_size,
+                        input_size=input_size,
+                        fitted=fitted,
+                        level=level,
+                        refit=refit,
+                        verbose=self.verbose,
+                        target_col=target_col,
                     ),
                 )
                 futures.append(future)
             out = [f.get() for f in futures]
             fcsts = [d["forecasts"] for d in out]
             fcsts = np.vstack(fcsts)
             cols = out[0]["cols"]
```

### Comparing `statsforecast-1.7.3/statsforecast/distributed/fugue.py` & `statsforecast-1.7.4/statsforecast/distributed/fugue.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,15 +382,17 @@
         else:
             if X_df is None:
                 res_with_fitted = transform(df, self._forecast_noX_fitted, **tfm_kwargs)
             else:
                 res_with_fitted = _cotransform(
                     df, X_df, self._forecast_X_fitted, **tfm_kwargs
                 )
-            self._results = res_with_fitted
+            # the persist here avoids recomputing the whole thing
+            # when retrieving the fitted values
+            self._results = fa.persist(res_with_fitted)
             res = transform(
                 self._results,
                 FugueBackend._retrieve_forecast_df,
                 schema=self._fcst_schema,
                 engine=self._engine,
             )
         return res
```

### Comparing `statsforecast-1.7.3/statsforecast/distributed/multiprocess.py` & `statsforecast-1.7.4/statsforecast/distributed/multiprocess.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/statsforecast/ets.py` & `statsforecast-1.7.4/statsforecast/ets.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/statsforecast/feature_engineering.py` & `statsforecast-1.7.4/statsforecast/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/statsforecast/garch.py` & `statsforecast-1.7.4/statsforecast/garch.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/statsforecast/models.py` & `statsforecast-1.7.4/statsforecast/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from .garch import garch_model, garch_forecast
 from .tbats import tbats_selection, tbats_forecast, _compute_sigmah
 from statsforecast.utils import (
     _calculate_sigma,
     _calculate_intervals,
     _ensure_float,
     _naive,
+    _old_kw_to_pos,
     _quantiles,
     _repeat_val,
     _repeat_val_seas,
     _seasonal_naive,
     CACHE,
     ConformalIntervals,
     NOGIL,
@@ -5317,49 +5318,52 @@
     ----------
     - [De Livera, A. M., Hyndman, R. J., & Snyder, R. D. (2011). Forecasting time series with complex seasonal patterns using exponential smoothing. Journal of the American statistical association, 106(496), 1513-1527.](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=f3de25596ab60ef0e886366826bf58a02b35a44f)
 
     - [De Livera, Alysha M (2017). Modeling time series with complex seasonal patterns using exponential smoothing. Monash University. Thesis.](https://doi.org/10.4225/03/589299681de3d)
 
     Parameters
     ----------
-    seasonal_periods : int or list of int.
+    season_length : int or list of int.
         Number of observations per unit of time. Ex: 24 Hourly data.
     use_boxcox : bool (default=True)
         Whether or not to use a Box-Cox transformation.
     bc_lower_bound : float (default=0.0)
         Lower bound for the Box-Cox transformation.
-    bc_upper_bound : float (default=1.5)
+    bc_upper_bound : float (default=1.0)
         Upper bound for the Box-Cox transformation.
     use_trend : bool (default=True)
         Whether or not to use a trend component.
     use_damped_trend : bool (default=False)
         Whether or not to dampen the trend component.
     use_arma_errors : bool (default=False)
         Whether or not to use a ARMA errors.
     alias : str
         Custom name of the model.
     """
 
+    @_old_kw_to_pos(["seasonal_periods"], [1])
     def __init__(
         self,
-        seasonal_periods: Union[int, List[int]],
+        season_length: Union[int, List[int]],
         use_boxcox: Optional[bool] = True,
         bc_lower_bound: float = 0.0,
-        bc_uppper_bound: float = 1.5,
+        bc_upper_bound: float = 1.0,
         use_trend: Optional[bool] = True,
         use_damped_trend: Optional[bool] = False,
         use_arma_errors: bool = False,
         alias: str = "TBATS",
+        *,
+        seasonal_periods=None,  # noqa: ARG002
     ):
-        if isinstance(seasonal_periods, int):
-            seasonal_periods = [seasonal_periods]
-        self.seasonal_periods = list(seasonal_periods)
+        if isinstance(season_length, int):
+            season_length = [season_length]
+        self.season_length = list(season_length)
         self.use_boxcox = use_boxcox
         self.bc_lower_bound = bc_lower_bound
-        self.bc_upper_bound = bc_uppper_bound
+        self.bc_upper_bound = bc_upper_bound
         self.use_trend = use_trend
         self.use_damped_trend = use_damped_trend
         self.use_arma_errors = use_arma_errors
         self.alias = alias
 
     def __repr__(self):
         return self.alias
@@ -5379,15 +5383,15 @@
         Returns
         -------
         self :
             TBATS model.
         """
         self.model_ = tbats_selection(
             y=y,
-            seasonal_periods=self.seasonal_periods,
+            seasonal_periods=self.season_length,
             use_boxcox=self.use_boxcox,
             bc_lower_bound=self.bc_lower_bound,
             bc_upper_bound=self.bc_upper_bound,
             use_trend=self.use_trend,
             use_damped_trend=self.use_damped_trend,
             use_arma_errors=self.use_arma_errors,
         )
@@ -5417,14 +5421,16 @@
             sigmah = _compute_sigmah(self.model_, h)
             pred_int = _calculate_intervals(res, level, h, sigmah)
             res = {**res, **pred_int}
         if self.model_["BoxCox_lambda"] is not None:
             res_trans = {
                 k: inv_boxcox(v, self.model_["BoxCox_lambda"]) for k, v in res.items()
             }
+            for k, v in res_trans.items():
+                res_trans[k] = np.where(np.isnan(v), res[k], v)
         else:
             res_trans = res
         return res_trans
 
     def predict_in_sample(self, level: Optional[Tuple[int]] = None):
         """Access fitted TBATS model predictions.
 
@@ -5443,14 +5449,16 @@
             se = _calculate_sigma(self.model_["errors"], self.model_["errors"].shape[1])
             fitted_pred_int = _add_fitted_pi(res, se, level)
             res = {**res, **fitted_pred_int}
         if self.model_["BoxCox_lambda"] is not None:
             res_trans = {
                 k: inv_boxcox(v, self.model_["BoxCox_lambda"]) for k, v in res.items()
             }
+            for k, v in res_trans.items():
+                res_trans[k] = np.where(np.isnan(v), res[k], v)
         else:
             res_trans = res
         return res_trans
 
     def forecast(
         self,
         y: np.ndarray,
@@ -5480,15 +5488,15 @@
         Returns
         -------
         forecasts : dict
             Dictionary with entries `mean` for point predictions and `level_*` for probabilistic predictions.
         """
         mod = tbats_selection(
             y=y,
-            seasonal_periods=self.seasonal_periods,
+            seasonal_periods=self.season_length,
             use_boxcox=self.use_boxcox,
             bc_lower_bound=self.bc_lower_bound,
             bc_upper_bound=self.bc_upper_bound,
             use_trend=self.use_trend,
             use_damped_trend=self.use_damped_trend,
             use_arma_errors=self.use_arma_errors,
         )
@@ -5503,14 +5511,16 @@
             res = {**res, **pred_int}
             if fitted:
                 se = _calculate_sigma(mod["errors"], mod["errors"].shape[1])
                 fitted_pred_int = _add_fitted_pi(res, se, level)
                 res = {**res, **fitted_pred_int}
         if mod["BoxCox_lambda"] is not None:
             res_trans = {k: inv_boxcox(v, mod["BoxCox_lambda"]) for k, v in res.items()}
+            for k, v in res_trans.items():
+                res_trans[k] = np.where(np.isnan(v), res[k], v)
         else:
             res_trans = res
         return res_trans
 
 # %% ../nbs/src/core/models.ipynb 388
 class AutoTBATS(TBATS):
     """AutoTBATS model.
@@ -5529,38 +5539,45 @@
     ----------
     seasonal_periods : int or list of int.
         Number of observations per unit of time. Ex: 24 Hourly data.
     use_boxcox : bool (default=None)
         Whether or not to use a Box-Cox transformation. By default tries both.
     bc_lower_bound : float (default=0.0)
         Lower bound for the Box-Cox transformation.
-    bc_upper_bound : float (default=1.5)
+    bc_upper_bound : float (default=1.0)
         Upper bound for the Box-Cox transformation.
     use_trend : bool (default=None)
         Whether or not to use a trend component. By default tries both.
     use_damped_trend : bool (default=None)
         Whether or not to dampen the trend component. By default tries both.
     use_arma_errors : bool (default=True)
         Whether or not to use a ARMA errors. Default is True and this evaluates both models.
     alias : str
         Custom name of the model.
     """
 
+    @_old_kw_to_pos(["seasonal_periods"], [1])
     def __init__(
         self,
-        seasonal_periods: Union[int, List[int]],
+        season_length: Union[int, List[int]],
         use_boxcox: Optional[bool] = None,
+        bc_lower_bound: float = 0.0,
+        bc_upper_bound: float = 1.0,
         use_trend: Optional[bool] = None,
         use_damped_trend: Optional[bool] = None,
         use_arma_errors: bool = True,
         alias: str = "AutoTBATS",
+        *,
+        seasonal_periods=None  # noqa: ARG002
     ):
         super().__init__(
-            seasonal_periods,
+            season_length=season_length,
             use_boxcox=use_boxcox,
+            bc_lower_bound=bc_lower_bound,
+            bc_upper_bound=bc_upper_bound,
             use_trend=use_trend,
             use_damped_trend=use_damped_trend,
             use_arma_errors=use_arma_errors,
             alias=alias,
         )
 
 # %% ../nbs/src/core/models.ipynb 398
```

### Comparing `statsforecast-1.7.3/statsforecast/mstl.py` & `statsforecast-1.7.4/statsforecast/mstl.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/statsforecast/tbats.py` & `statsforecast-1.7.4/statsforecast/tbats.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,84 +7,80 @@
 import warnings
 from functools import partial
 from itertools import product
 
 import numpy as np
 import pandas as pd
 import scipy.linalg
+from coreforecast.scalers import boxcox, boxcox_lambda, inv_boxcox
 from numba import njit
 from numpy.polynomial.polynomial import Polynomial
-from scipy.special import inv_boxcox
-from scipy.stats import boxcox
 from scipy.optimize import minimize
-from statsmodels.tsa.stattools import adfuller
 from threadpoolctl import threadpool_limits
-
 from .arima import auto_arima_f
 from .utils import NOGIL, CACHE
 
 # %% ../nbs/src/tbats.ipynb 7
 def find_harmonics(y, m):
+
     # Compute a 2 x m moving average to estimate the trend
     window_size = 2 * m
-    data = pd.DataFrame({"value": y})
-    f_t = data["value"].rolling(window=window_size, center=True).mean()
-
-    # Obtain an approximation of seasonal component using z_t = y_t - f_t
-    data["f_t"] = f_t
-    data["z_t"] = data["value"] - data["f_t"]
+    f_t = pd.Series(y).rolling(window=window_size, min_periods=1).mean().to_numpy()
 
-    # Drop missing values (due to the moving average)
-    data.dropna(inplace=True)
-
-    if data.empty:
-        return 1
+    # Obtain an approximation of seasonal component using z_t = y_t - f_t. If f_t=0, don't detrend series
+    z = y - f_t
 
     # Approximate the seasonal component using trigonometric terms
-    t = np.arange(len(data))
+    t = np.arange(len(y))
     if m % 2 == 0:
         max_harmonics = int(m / 2)
     else:
         max_harmonics = int((m - 1) / 2)
 
-    max_harmonics = min(max_harmonics, len(data))
-
-    aic = np.inf
-    num_harmonics = 0
+    max_harmonics = min(max_harmonics, len(y))
+    if max_harmonics == 0:
+        return 1, y
 
     # Create cosine and sine terms
-    fourier = np.empty((len(data), 2 * max_harmonics))
+    fourier = np.empty((len(y), 2 * max_harmonics))
     for i in range(max_harmonics):
         fourier[:, 2 * i] = np.cos(2 * np.pi * (i + 1) * t / m)
         fourier[:, 2 * i + 1] = np.sin(2 * np.pi * (i + 1) * t / m)
 
+    aic = np.inf
+    num_harmonics = 0
+    tol = 2
+    without_improv = 0
     for h in range(1, max_harmonics + 1):
         # Perform regression to estimate the coefficients
         X = fourier[:, : 2 * h]
-        y = data["z_t"]
-        model, residuals = np.linalg.lstsq(X, y, rcond=None)[:2]
+        model, residuals = np.linalg.lstsq(X, z, rcond=None)[:2]
         k = model.size
-        n = len(y)
+        n = len(z)
         new_aic = n * np.log(residuals / n) + 2 * k
 
         if new_aic.size > 0 and new_aic < aic:
             aic = new_aic
             num_harmonics = h
+            best_model = model
+            without_improv = 0
         else:
-            break
+            without_improv += 1
+            if without_improv >= tol:
+                break
 
     if num_harmonics == 0:
-        num_harmonics += 1
+        num_harmonics = 1
+        best_model = np.zeros(2)
 
-    return num_harmonics
+    return num_harmonics, y - X[:, : 2 * num_harmonics] @ best_model
 
 # %% ../nbs/src/tbats.ipynb 9
-def initial_parameters(
-    seasonal_periods, k_vector, use_trend, use_damped_trend, ar_coeffs, ma_coeffs
-):
+def initial_parameters(k_vector, use_trend, use_damped_trend, ar_coeffs, ma_coeffs):
+
     alpha = 0.09
 
     if use_trend:
         adj_beta = 1
         beta = 0.05
         b = 0
         if use_damped_trend:
@@ -121,14 +117,15 @@
         s_vector,
         d_vector,
         epsilon_vector,
     )
 
 # %% ../nbs/src/tbats.ipynb 11
 def makeXMatrix(b, s_vector, d_vector, epsilon_vector):
+
     # x = (l_t, b_t, s_vector, d_vector, epsilon_vector)
     x = np.array([0.0])
     if b is not None:
         x = np.append(x, b)
     if s_vector is not None:
         x = np.concatenate((x, s_vector))
     if d_vector is not None:
@@ -177,14 +174,15 @@
 
     return w_transpose
 
 # %% ../nbs/src/tbats.ipynb 17
 def makeTBATSGMatrix(
     k_vector, alpha, adj_beta, beta, gamma_one_v, gamma_two_v, p, q, tau
 ):
+
     # g = (alpha, beta, gamma_bold, 1, 0_{p-1}, 1, 0_{q-1})
     g = np.zeros((1 + adj_beta + 2 * np.sum(k_vector) + p + q, 1))
 
     g[0, 0] = alpha
 
     if beta is not None:
         g[1, 0] = beta
@@ -317,14 +315,15 @@
         F = np.vstack((F, ma_rows))
 
     return F
 
 # %% ../nbs/src/tbats.ipynb 21
 @njit(nogil=NOGIL, cache=CACHE)
 def calcTBATSFaster(y_trans, w_transpose, g, F, x_nought):
+
     n = y_trans.shape[0]
 
     yhat = np.zeros((1, n))
     e = np.zeros((1, n))
     x = np.zeros((n, len(x_nought)))
 
     yhat[0, 0] = np.dot(w_transpose[0], x_nought)
@@ -401,17 +400,17 @@
     if phi is not None:
         adjBeta = 1
         w_transpose[0, 1] = phi
 
     if p != 0:
         w_transpose[0, adjBeta + tau + 1 : adjBeta + tau + p + 1] = ar_coeffs
         if q != 0:
-            w_transpose[
-                0, adjBeta + tau + p + 1 : adjBeta + tau + p + q + 1
-            ] = ma_coeffs
+            w_transpose[0, adjBeta + tau + p + 1 : adjBeta + tau + p + q + 1] = (
+                ma_coeffs
+            )
     elif q != 0:
         # here p = 0
         w_transpose[0, adjBeta + tau + 1 : adjBeta + tau + q + 1] = ma_coeffs
 
     return w_transpose
 
 # %% ../nbs/src/tbats.ipynb 27
@@ -450,17 +449,17 @@
             F[1, (betaAdjust + tau + 1) : (betaAdjust + tau + p + 1)] = beta * ar_coeffs
         if tau > 0:
             B = np.dot(gamma_bold.reshape(-1, 1), ar_coeffs.reshape(1, -1))
             F[
                 (1 + betaAdjust) : (betaAdjust + tau + 1),
                 (betaAdjust + tau + 1) : (betaAdjust + tau + p + 1),
             ] = B
-        F[
-            betaAdjust + tau + 1, (betaAdjust + tau + 1) : (betaAdjust + tau + p + 1)
-        ] = ar_coeffs
+        F[betaAdjust + tau + 1, (betaAdjust + tau + 1) : (betaAdjust + tau + p + 1)] = (
+            ar_coeffs
+        )
     if ma_coeffs is not None:
         F[0, (betaAdjust + tau + p + 1) : (betaAdjust + tau + p + q + 1)] = (
             alpha * ma_coeffs
         )
         if betaAdjust == 1:
             F[1, (betaAdjust + tau + p + 1) : (betaAdjust + tau + p + q + 1)] = (
                 beta * ma_coeffs
@@ -477,23 +476,15 @@
                 (betaAdjust + tau + p + 1) : (betaAdjust + tau + p + q + 1),
             ] = ma_coeffs
 
     return F
 
 # %% ../nbs/src/tbats.ipynb 31
 def checkAdmissibility(
-    BoxCox_lambda,
-    bc_lower_bound,
-    bc_upper_bound,
-    alpha,
-    beta,
-    phi,
-    ar_coeffs,
-    ma_coeffs,
-    D,
+    BoxCox_lambda, bc_lower_bound, bc_upper_bound, phi, ar_coeffs, ma_coeffs, D
 ):
     if BoxCox_lambda is not None:
         if (BoxCox_lambda < bc_lower_bound) or (BoxCox_lambda > bc_upper_bound):
             return False
 
     if phi is not None:
         if (phi < 0.8) or (phi > 1):
@@ -539,33 +530,27 @@
     gamma_bold,
     x_nought,
     x_nought_untransformed,
     bc_lower_bound,
     bc_upper_bound,
     p,
     q,
+    scale,
 ):
-    (
-        BoxCox_lambda,
-        alpha,
-        beta,
-        phi,
-        gamma_one_v,
-        gamma_two_v,
-        ar_coeffs,
-        ma_coeffs,
-    ) = extract_params(
-        params,
-        use_boxcox,
-        use_trend,
-        use_damped_trend,
-        use_arma_errors,
-        seasonal_periods,
-        p,
-        q,
+    BoxCox_lambda, alpha, beta, phi, gamma_one_v, gamma_two_v, ar_coeffs, ma_coeffs = (
+        extract_params(
+            params * scale,
+            use_boxcox,
+            use_trend,
+            use_damped_trend,
+            use_arma_errors,
+            seasonal_periods,
+            p,
+            q,
+        )
     )
 
     w_transpose = updateTBATSWMatrix(w_transpose, phi, tau, ar_coeffs, ma_coeffs, p, q)
     g = updateTBATSGMatrix(
         g, gamma_bold, alpha, beta, k_vector, gamma_one_v, gamma_two_v
     )
     F = updateTBATSFMatrix(
@@ -584,23 +569,15 @@
         ) * np.nansum(np.log(y))
     else:
         log_likelihood = n * np.log(np.nansum(e**2))
 
     D = F - np.dot(g, w_transpose)
 
     if checkAdmissibility(
-        BoxCox_lambda,
-        bc_lower_bound,
-        bc_upper_bound,
-        alpha,
-        beta,
-        phi,
-        ar_coeffs,
-        ma_coeffs,
-        D,
+        BoxCox_lambda, bc_lower_bound, bc_upper_bound, phi, ar_coeffs, ma_coeffs, D
     ):
         return log_likelihood
     else:
         return 10**20
 
 # %% ../nbs/src/tbats.ipynb 36
 def tbats_model_generator(
@@ -612,17 +589,24 @@
     bc_upper_bound,
     use_trend,
     use_damped_trend,
     use_arma_errors,
     ar_coeffs,
     ma_coeffs,
 ):
+
     # Initial Box-Cox transformation (if required)
     if use_boxcox:
-        BoxCox_lambda = 0  # This is the initial value used in the thesis
+        BoxCox_lambda = boxcox_lambda(
+            y,
+            method="guerrero",
+            season_length=max(seasonal_periods),
+            lower=bc_lower_bound,
+            upper=bc_upper_bound,
+        )
         y_trans = boxcox(y, BoxCox_lambda)
     else:
         BoxCox_lambda = None
         y_trans = y
 
     p, q = findPQ(ar_coeffs, ma_coeffs)
 
@@ -634,17 +618,15 @@
         b,
         phi,
         gamma_one_v,
         gamma_two_v,
         s_vector,
         d_vector,
         epsilon_vector,
-    ) = initial_parameters(
-        seasonal_periods, k_vector, use_trend, use_damped_trend, ar_coeffs, ma_coeffs
-    )
+    ) = initial_parameters(k_vector, use_trend, use_damped_trend, ar_coeffs, ma_coeffs)
 
     # seed states
     x_nought = makeXMatrix(b, s_vector, d_vector, epsilon_vector)
 
     # tau
     tau = 2 * np.sum(k_vector)
 
@@ -699,34 +681,44 @@
 
     if (p != 0) or (q != 0):
         arma_seed_states = np.zeros((p + q,))
         x_nought = np.concatenate((x_nought, arma_seed_states))
 
     # Optimization
     # Create vector with parameters
+    scale = []
     if use_boxcox:
         params = np.concatenate([np.array([BoxCox_lambda]), np.array([alpha])])
+        scale.extend([0.001, 0.01])
     else:
         params = np.array([alpha])
+        scale.append(0.01)
     if beta is not None:
         params = np.concatenate([params, np.array([beta])])
+        scale.append(0.01)
     if phi is not None and phi != 1:
         use_damped_trend = True
         params = np.concatenate([params, np.array([phi])])
+        scale.append(0.01)
     else:
         use_damped_trend = False
     params = np.concatenate([params, gamma_one_v, gamma_two_v])
+    scale.extend((gamma_one_v.size + gamma_two_v.size) * [1e-5])
     if ar_coeffs is not None:
         params = np.concatenate([params, ar_coeffs])
+        scale.extend(ar_coeffs.size * [0.1])
     if ma_coeffs is not None:
         params = np.concatenate([params, ma_coeffs])
+        scale.extend(ma_coeffs.size * [0.1])
     if use_boxcox:
         x_nought_untransformed = inv_boxcox(x_nought, BoxCox_lambda)
     else:
         x_nought_untransformed = x_nought
+    scale = np.array(scale)
+    params = params / scale
 
     objective_fn = partial(
         calcLikelihoodTBATS,
         use_boxcox=use_boxcox,
         use_trend=use_trend,
         use_damped_trend=use_damped_trend,
         use_arma_errors=use_arma_errors,
@@ -741,17 +733,25 @@
         gamma_bold=gamma_bold,
         x_nought=x_nought,
         x_nought_untransformed=x_nought_untransformed,
         bc_lower_bound=bc_lower_bound,
         bc_upper_bound=bc_upper_bound,
         p=p,
         q=q,
+        scale=scale,
     )
+
     # Solve optimization problem
-    optim_params = minimize(objective_fn, params, method="Nelder-Mead").x
+    res = minimize(
+        objective_fn,
+        params,
+        method="Nelder-Mead",
+        options={"maxiter": 100 * params.size**2},
+    )
+    optim_params = res.x * scale
 
     (
         optim_BoxCox_lambda,
         optim_alpha,
         optim_beta,
         optim_phi,
         optim_gamma_one_v,
@@ -792,28 +792,35 @@
         p,
         q,
         tau,
     )
 
     if use_boxcox:
         y_trans = boxcox(y, optim_BoxCox_lambda)
+        x_nought = boxcox(x_nought_untransformed, optim_BoxCox_lambda)
 
     fitted, errors, x = calcTBATSFaster(y_trans, w_transpose, g, F, x_nought)
 
     sigma2 = np.sum(errors * errors) / len(y_trans)
 
     # Calculate log-likelihood
-    if use_boxcox:
-        log_likelihood = len(y_trans) * np.log(np.nansum(errors**2)) - 2 * (
-            optim_BoxCox_lambda - 1
-        ) * np.nansum(np.log(y))
-    else:
-        log_likelihood = len(y_trans) * np.log(np.nansum(errors**2))
+    log_likelihood = res.fun
 
+    # AIC
     kval = len(optim_params) + x_nought.shape[0]
+    # special cases
+    if optim_BoxCox_lambda == 1:
+        kval -= 1
+    if optim_beta is not None:
+        if abs(optim_beta) < 1e-08:
+            kval -= 1
+    if optim_phi is not None:
+        if optim_phi == 1:
+            kval -= 1
+
     aic = log_likelihood + 2 * kval
 
     res = {
         "fitted": fitted,
         "errors": errors,
         "sigma2": sigma2,
         "aic": aic,
@@ -822,14 +829,15 @@
         "w_transpose": w_transpose,
         "g": g,
         "x": x,
         "k_vector": k_vector,
         "BoxCox_lambda": optim_BoxCox_lambda,
         "p": p,
         "q": q,
+        "seed_states": x_nought,
     }
 
     return res
 
 # %% ../nbs/src/tbats.ipynb 38
 def tbats_model(
     y,
@@ -838,14 +846,15 @@
     use_boxcox,
     bc_lower_bound,
     bc_upper_bound,
     use_trend,
     use_damped_trend,
     use_arma_errors,
 ):
+
     # First model - No ARMA errors
     ar_coeffs = None
     ma_coeffs = None
 
     best_model = tbats_model_generator(
         y,
         seasonal_periods,
@@ -917,56 +926,63 @@
     use_boxcox,
     bc_lower_bound,
     bc_upper_bound,
     use_trend,
     use_damped_trend,
     use_arma_errors,
 ):
+
     # Check for banned parameter combinations
-    if (not use_trend) and use_damped_trend:
+    if not use_trend and use_damped_trend:
         raise ValueError("Can't use damped trend without trend")
 
     # Sort seasonal periods
     seasonal_periods = np.sort(seasonal_periods)
 
     # Check if there are missing values
     indices = np.where(np.isnan(y))[0]
     if len(indices) > 0:
         max_index = indices[-1]
         y = y[max_index + 1 : len(y)]
 
     # Check if there are negative values
-    if np.any(y < 0):
-        use_boxcox = False
-
-    # Check if there is a trend
-    adf = adfuller(y, regression="ct")
-    if adf[1] <= 0.05:
+    if use_boxcox in (True, None) and np.any(y <= 0):
         warnings.warn(
-            "The time series is trend-stationary, disabling trend components."
+            "Data contains zero or negative values, disabling Box-Cox transformation."
         )
-        use_trend = False
-        use_damped_trend = False
-    else:
-        use_trend = True
+        use_boxcox = False
 
     # Choose the number of harmonics
-    k_vector = np.array([find_harmonics(y, m) for m in seasonal_periods])
+    ks = []
+    z = y.copy()
+    for period in seasonal_periods:
+        k, z = find_harmonics(z, period)
+        ks.append(k)
+    k_vector = np.array(ks)
 
     # Select combinations to try out
     if use_boxcox is None:
         B = [True, False]
     else:
         B = [use_boxcox]
 
-    if use_trend:
+    if use_trend is None:
+        if use_damped_trend is None:
+            T = [[True, True], [True, False], [False, False]]
+        elif use_damped_trend:
+            T = [[True, True]]
+        else:
+            T = [[True, False], [False, False]]
+    elif use_trend:
         if use_damped_trend is None:
             T = [[True, True], [True, False]]
+        elif use_damped_trend:
+            T = [[True, True]]
         else:
-            T = [[True, use_damped_trend]]
+            T = [[True, False]]
     else:
         T = [[False, False]]
 
     A = [use_arma_errors]
 
     combinations = [(b, t, a) for b, t, a in product(B, T, A)]
```

### Comparing `statsforecast-1.7.3/statsforecast/theta.py` & `statsforecast-1.7.4/statsforecast/theta.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/statsforecast/utils.py` & `statsforecast-1.7.4/statsforecast/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/src/utils.ipynb.
 
 # %% auto 0
 __all__ = ['AirPassengers', 'AirPassengersDF', 'generate_series']
 
 # %% ../nbs/src/utils.ipynb 3
-from typing import Dict
+import inspect
 import math
 import os
 import warnings
+from functools import wraps
+from typing import Dict
 
 import numpy as np
 import pandas as pd
 from scipy.stats import norm
 
 from utilsforecast.compat import DataFrame
 from utilsforecast.data import generate_series as utils_generate_series
@@ -230,15 +232,17 @@
     ]
 )
 
 # %% ../nbs/src/utils.ipynb 12
 AirPassengersDF = pd.DataFrame(
     {
         "unique_id": np.ones(len(AirPassengers)),
-        "ds": pd.date_range(start="1949-01-01", periods=len(AirPassengers), freq="M"),
+        "ds": pd.date_range(
+            start="1949-01-01", periods=len(AirPassengers), freq=pd.offsets.MonthEnd()
+        ),
         "y": AirPassengers,
     }
 )
 
 # %% ../nbs/src/utils.ipynb 17
 def _repeat_val_seas(season_vals: np.ndarray, h: int) -> np.ndarray:
     repeats = math.ceil(h / season_vals.size)
@@ -334,7 +338,38 @@
             )
         allowed_methods = ["conformal_distribution"]
         if method not in allowed_methods:
             raise ValueError(f"method must be one of {allowed_methods}")
         self.n_windows = n_windows
         self.h = h
         self.method = method
+
+# %% ../nbs/src/utils.ipynb 21
+def _old_kw_to_pos(old_names, new_positions):
+    def decorator(f):
+        @wraps(f)
+        def inner(*args, **kwargs):
+            arg_names = inspect.getfullargspec(f).args
+            new_args = list(args)
+            for old_name, pos in zip(old_names, new_positions):
+                if old_name in kwargs:
+                    new_name = arg_names[pos]
+                    warnings.warn(
+                        f"`{old_name}` has been deprecated, please use `{new_name}` instead.",
+                        FutureWarning,
+                    )
+                    if len(new_args) > pos:
+                        new_args = [
+                            *new_args[:pos],
+                            kwargs[old_name],
+                            *new_args[pos + 1 :],
+                        ]
+                    else:
+                        new_args = list(new_args)
+                        for i in range(len(new_args), pos):
+                            new_args.append(kwargs.pop(arg_names[i]))
+                        new_args.append(kwargs.pop(old_name))
+            return f(*new_args, **kwargs)
+
+        return inner
+
+    return decorator
```

### Comparing `statsforecast-1.7.3/statsforecast.egg-info/PKG-INFO` & `statsforecast-1.7.4/statsforecast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statsforecast
-Version: 1.7.3
+Version: 1.7.4
 Summary: Time series forecasting suite using statistical models
 Home-page: https://github.com/Nixtla/statsforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting arima ets
 Classifier: Development Status :: 3 - Alpha
@@ -15,44 +15,45 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudpickle
+Requires-Dist: coreforecast>=0.0.7
 Requires-Dist: numba>=0.55.0
 Requires-Dist: numpy>=1.21.6
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: statsmodels>=0.13.2
 Requires-Dist: tqdm
 Requires-Dist: fugue>=0.8.1
 Requires-Dist: utilsforecast>=0.0.24
 Requires-Dist: threadpoolctl
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pmdarima; extra == "dev"
+Requires-Dist: fugue[ray]>=0.8.1; extra == "dev"
+Requires-Dist: scikit-learn; extra == "dev"
+Requires-Dist: nbdev_plotly; extra == "dev"
+Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: polars; extra == "dev"
+Requires-Dist: plotly; extra == "dev"
+Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
+Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "dev"
+Requires-Dist: fugue[dask]>=0.8.1; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
+Requires-Dist: prophet; extra == "dev"
+Requires-Dist: datasetsforecast; extra == "dev"
 Requires-Dist: supersmoother; extra == "dev"
+Requires-Dist: pandas[plot]; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: ray<2.8; extra == "dev"
 Requires-Dist: fugue[spark]>=0.8.1; extra == "dev"
-Requires-Dist: plotly; extra == "dev"
-Requires-Dist: nbdev_plotly; extra == "dev"
-Requires-Dist: fugue[ray]>=0.8.1; extra == "dev"
-Requires-Dist: pyarrow; extra == "dev"
-Requires-Dist: pandas[plot]; extra == "dev"
-Requires-Dist: datasetsforecast; extra == "dev"
-Requires-Dist: prophet; extra == "dev"
-Requires-Dist: fugue[dask]>=0.8.1; extra == "dev"
-Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "dev"
-Requires-Dist: scikit-learn; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
-Requires-Dist: plotly-resampler; extra == "dev"
-Requires-Dist: polars; extra == "dev"
 Provides-Extra: dask
 Requires-Dist: fugue[dask]>=0.8.1; extra == "dask"
 Provides-Extra: ray
 Requires-Dist: fugue[ray]>=0.8.1; extra == "ray"
 Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "ray"
 Requires-Dist: ray<2.8; extra == "ray"
 Provides-Extra: spark
```

### Comparing `statsforecast-1.7.3/statsforecast.egg-info/SOURCES.txt` & `statsforecast-1.7.4/statsforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.3/statsforecast.egg-info/requires.txt` & `statsforecast-1.7.4/statsforecast.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 cloudpickle
+coreforecast>=0.0.7
 numba>=0.55.0
 numpy>=1.21.6
 pandas>=1.3.5
 scipy>=1.7.3
 statsmodels>=0.13.2
 tqdm
 fugue>=0.8.1
 utilsforecast>=0.0.24
 threadpoolctl
 
 [dask]
 fugue[dask]>=0.8.1
 
 [dev]
-flake8
 pmdarima
+fugue[ray]>=0.8.1
+scikit-learn
+nbdev_plotly
+plotly-resampler
+polars
+plotly
+pyarrow
+flake8
+nbdev
+protobuf<4.0.0,>=3.15.3
+fugue[dask]>=0.8.1
 mypy
+prophet
+datasetsforecast
 supersmoother
+pandas[plot]
 black
 ray<2.8
 fugue[spark]>=0.8.1
-plotly
-nbdev_plotly
-fugue[ray]>=0.8.1
-pyarrow
-pandas[plot]
-datasetsforecast
-prophet
-fugue[dask]>=0.8.1
-protobuf<4.0.0,>=3.15.3
-scikit-learn
-nbdev
-plotly-resampler
-polars
 
 [plotly]
 plotly
 plotly-resampler
 
 [polars]
 polars
```

