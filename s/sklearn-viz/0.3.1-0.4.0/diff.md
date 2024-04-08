# Comparing `tmp/sklearn_viz-0.3.1.tar.gz` & `tmp/sklearn_viz-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_viz-0.3.1.tar", max compression
+gzip compressed data, was "sklearn_viz-0.4.0.tar", max compression
```

## Comparing `sklearn_viz-0.3.1.tar` & `sklearn_viz-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0        0 2023-08-27 06:10:46.929402 sklearn_viz-0.3.1/elphick/sklearn_viz/__init__.py
--rw-r--r--   0        0        0      334 2023-09-18 13:02:51.287832 sklearn_viz-0.3.1/elphick/sklearn_viz/features/__init__.py
--rw-r--r--   0        0        0     7873 2023-10-10 12:02:36.000498 sklearn_viz-0.3.1/elphick/sklearn_viz/features/importance.py
--rw-r--r--   0        0        0     4738 2024-03-30 11:59:00.677281 sklearn_viz-0.3.1/elphick/sklearn_viz/features/outlier_detection.py
--rw-r--r--   0        0        0     2471 2024-03-30 11:59:00.682932 sklearn_viz-0.3.1/elphick/sklearn_viz/features/parallel_coordinates.py
--rw-r--r--   0        0        0    16988 2024-03-30 11:59:00.688949 sklearn_viz-0.3.1/elphick/sklearn_viz/features/principal_components.py
--rw-r--r--   0        0        0      668 2023-09-18 11:19:59.559906 sklearn_viz-0.3.1/elphick/sklearn_viz/features/scatter_matrix.py
--rw-r--r--   0        0        0      131 2023-09-18 13:02:51.313708 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/__init__.py
--rw-r--r--   0        0        0     6246 2023-09-11 12:55:18.110947 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/learning_curve.py
--rw-r--r--   0        0        0     1469 2024-04-02 23:43:43.297303 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/metrics.py
--rw-r--r--   0        0        0    20963 2024-04-02 23:43:43.308707 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/model_selection.py
--rw-r--r--   0        0        0     2552 2023-09-11 12:55:18.114966 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/models.py
--rw-r--r--   0        0        0      318 2023-11-12 09:19:44.575578 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/scorers.py
--rw-r--r--   0        0        0       22 2023-09-17 08:40:15.220711 sklearn_viz-0.3.1/elphick/sklearn_viz/residuals/__init__.py
--rw-r--r--   0        0        0     2120 2023-09-05 09:52:35.543294 sklearn_viz-0.3.1/elphick/sklearn_viz/residuals/error.py
--rw-r--r--   0        0        0       28 2023-08-27 06:10:46.931314 sklearn_viz-0.3.1/elphick/sklearn_viz/utils/__init__.py
--rw-r--r--   0        0        0     3191 2023-08-27 06:10:46.931314 sklearn_viz-0.3.1/elphick/sklearn_viz/utils/timer.py
--rw-r--r--   0        0        0     1090 2023-08-27 06:10:46.917578 sklearn_viz-0.3.1/LICENSE
--rw-r--r--   0        0        0      819 2024-04-02 23:43:43.333160 sklearn_viz-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      362 2023-08-27 06:10:46.918992 sklearn_viz-0.3.1/README.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-27 06:10:46.929402 sklearn_viz-0.4.0/elphick/sklearn_viz/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:00:29.935280 sklearn_viz-0.4.0/elphick/sklearn_viz/components/__init__.py
+-rw-r--r--   0        0        0     4482 2024-04-08 12:00:29.940581 sklearn_viz-0.4.0/elphick/sklearn_viz/components/estimators.py
+-rw-r--r--   0        0        0      334 2023-09-18 13:02:51.287832 sklearn_viz-0.4.0/elphick/sklearn_viz/features/__init__.py
+-rw-r--r--   0        0        0     8495 2024-04-08 12:00:29.951129 sklearn_viz-0.4.0/elphick/sklearn_viz/features/importance.py
+-rw-r--r--   0        0        0     4738 2024-03-30 11:59:00.677281 sklearn_viz-0.4.0/elphick/sklearn_viz/features/outlier_detection.py
+-rw-r--r--   0        0        0     2471 2024-03-30 11:59:00.682932 sklearn_viz-0.4.0/elphick/sklearn_viz/features/parallel_coordinates.py
+-rw-r--r--   0        0        0    16988 2024-03-30 11:59:00.688949 sklearn_viz-0.4.0/elphick/sklearn_viz/features/principal_components.py
+-rw-r--r--   0        0        0      668 2023-09-18 11:19:59.559906 sklearn_viz-0.4.0/elphick/sklearn_viz/features/scatter_matrix.py
+-rw-r--r--   0        0        0      131 2023-09-18 13:02:51.313708 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/__init__.py
+-rw-r--r--   0        0        0     6246 2023-09-11 12:55:18.110947 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/learning_curve.py
+-rw-r--r--   0        0        0     1622 2024-04-08 12:00:29.961992 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/metrics.py
+-rw-r--r--   0        0        0    21106 2024-04-08 12:00:29.972985 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/model_selection.py
+-rw-r--r--   0        0        0     2552 2023-09-11 12:55:18.114966 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/models.py
+-rw-r--r--   0        0        0      526 2024-04-08 12:00:29.983221 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/scorers.py
+-rw-r--r--   0        0        0       22 2023-09-17 08:40:15.220711 sklearn_viz-0.4.0/elphick/sklearn_viz/residuals/__init__.py
+-rw-r--r--   0        0        0     2120 2023-09-05 09:52:35.543294 sklearn_viz-0.4.0/elphick/sklearn_viz/residuals/error.py
+-rw-r--r--   0        0        0       28 2023-08-27 06:10:46.931314 sklearn_viz-0.4.0/elphick/sklearn_viz/utils/__init__.py
+-rw-r--r--   0        0        0     3191 2023-08-27 06:10:46.931314 sklearn_viz-0.4.0/elphick/sklearn_viz/utils/timer.py
+-rw-r--r--   0        0        0     1090 2023-08-27 06:10:46.917578 sklearn_viz-0.4.0/LICENSE
+-rw-r--r--   0        0        0      819 2024-04-08 12:00:29.999523 sklearn_viz-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      362 2023-08-27 06:10:46.918992 sklearn_viz-0.4.0/README.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.4.0/PKG-INFO
```

### Comparing `sklearn_viz-0.3.1/elphick/sklearn_viz/features/importance.py` & `sklearn_viz-0.4.0/elphick/sklearn_viz/features/importance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
-from typing import Union, Optional, Dict
+from typing import Union, Optional, Dict, Callable
 
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
+from sklearn.base import is_classifier
 
 from sklearn.inspection import permutation_importance
 from sklearn.pipeline import Pipeline
 from sklearn.utils.validation import check_is_fitted
 
+from elphick.sklearn_viz.model_selection.scorers import r2_score_with_nan, classification_scorers, regression_scorers
 from elphick.sklearn_viz.utils import log_timer
 
 
 def plot_feature_importance(mdl,
                             sort: bool = False,
                             top_k: Optional[int] = None,
                             horizontal: bool = False,
@@ -48,31 +50,41 @@
 
 class FeatureImportance:
     def __init__(self,
                  mdl,
                  permute: bool = False,
                  pipeline_input_features: bool = False,
                  x_test: Optional[pd.DataFrame] = None,
-                 y_test: Optional[Union[pd.DataFrame, pd.Series]] = None):
+                 y_test: Optional[Union[pd.DataFrame, pd.Series]] = None,
+                 scorer: Optional[Union[str, Callable]] = None,):
         """
 
         Args:
             mdl: The scikit-learn model or pipeline.
             permute: If True plot permutation importance.  Better, but slower.  Requires X_test and y_test to be provided.
             pipeline_input_features: If True, and a pipeline is provided, report the features provided as inputs to
              the pipeline.  If False, reports the estimator (last pipeline step) input features.  Requires permute = True.
             x_test: X values provided to execute permuted importance.
             y_test: y values provided to execute permuted importance.
+            scorer: Optional callable scorer which the model will be fitted using
+
         """
         self._logger = logging.getLogger(name=__class__.__name__)
         self.mdl = mdl
         self.permute: bool = permute
         self.pipeline_input_features: bool = pipeline_input_features
         self.X_test: Optional[pd.DataFrame] = x_test
         self.y_test: Optional[Union[pd.DataFrame, pd.Series]] = y_test
+
+        if scorer is not None:
+            self.scorer = scorer
+        else:
+            self.scorer = classification_scorers[list(classification_scorers.keys())[0]] if is_classifier(self.mdl) else \
+                regression_scorers[list(regression_scorers.keys())[0]]
+
         self._data: Optional[pd.DataFrame] = None
         self.is_pipeline: bool = isinstance(mdl, Pipeline)
 
         if not self.permute:
             check_is_fitted(mdl[-1]) if self.is_pipeline else check_is_fitted(mdl)
 
     @property
@@ -87,15 +99,15 @@
                 self._logger.info("Generating feature importance by permutation")
                 x = self.X_test
                 if self.is_pipeline and not self.pipeline_input_features:
                     mdl = mdl[-1]
                     x = self.mdl[0:-1].transform(self.X_test)
 
                 result = permutation_importance(estimator=mdl, X=x, y=self.y_test, n_repeats=10, random_state=42,
-                                                n_jobs=2)
+                                                n_jobs=2, scoring=self.scorer)
                 importances = result.importances_mean
                 std = result.importances_std
             else:
                 self._logger.info("Extracting feature importance from the fitted model")
                 if self.is_pipeline:
                     mdl = mdl[-1]
                 try:  # trees
```

### Comparing `sklearn_viz-0.3.1/elphick/sklearn_viz/features/outlier_detection.py` & `sklearn_viz-0.4.0/elphick/sklearn_viz/features/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.1/elphick/sklearn_viz/features/parallel_coordinates.py` & `sklearn_viz-0.4.0/elphick/sklearn_viz/features/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.1/elphick/sklearn_viz/features/principal_components.py` & `sklearn_viz-0.4.0/elphick/sklearn_viz/features/principal_components.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.1/elphick/sklearn_viz/features/scatter_matrix.py` & `sklearn_viz-0.4.0/elphick/sklearn_viz/features/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/learning_curve.py` & `sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/learning_curve.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/metrics.py` & `sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,18 +25,26 @@
 
 def r2(y_true, y_est):
     ssr = ((y_true - y_est) ** 2).sum()
     sst = ((y_true - y_true.mean()) ** 2).sum()
     return 1 - (ssr / sst)
 
 
-regression_metrics = {'r2_score': r2_score,
-                      'me': mean_error,
-                      'r2': r2,
-                      'mae': mean_absolute_error,
-                      'mse': mean_squared_error,
-                      'rmse': partial(mean_squared_error, squared=False),
-                      'moe': partial(moe_95, metric='moe'),
-                      'moe_lo': partial(moe_95, metric='lo'),
-                      'moe_hi': partial(moe_95, metric='hi')}
+def r2_with_nan(y_true, y_est):
+    numerator = np.nansum((y_true - y_est) ** 2, axis=0, dtype=np.float64)
+    denominator = np.nansum((y_true - np.nanmean(y_true, axis=0)) ** 2, axis=0, dtype=np.float64)
+    return np.mean(1 - numerator / denominator)
+
+
+regression_metrics = {
+    # 'r2_nan': r2_with_nan,
+    'r2_score': r2_score,
+    'me': mean_error,
+    'r2': r2,
+    'mae': mean_absolute_error,
+    'mse': mean_squared_error,
+    'rmse': partial(mean_squared_error, squared=False),
+    'moe': partial(moe_95, metric='moe'),
+    'moe_lo': partial(moe_95, metric='lo'),
+    'moe_hi': partial(moe_95, metric='hi')}
 
 classification_metrics = {'f1': f1_score}
```

### Comparing `sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/model_selection.py` & `sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/model_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             raise NotImplementedError("Cannot have multiple algorithms and multiple datasets.")
 
     @property
     def data(self) -> Optional[Dict]:
         if self.metrics is None:
             cv_kwargs: Dict = dict()
         else:
-            cv_kwargs: Dict = dict(return_estimator=True, return_indices=True)
+            cv_kwargs: Dict = dict(return_estimator=True, return_indices=True, error_score=np.nan)
 
         if self._data is not None:
             results = self._data
         else:
             results: Dict = {}
             for data_key, data in self.datasets.items():
                 self._logger.info(f"Commencing Cross Validation for dataset {data_key}")
@@ -376,14 +376,16 @@
 
         for k, fn_metric in self.metrics.items():
             metric_values: List = []
             metric_groups: Dict = {}
             for estimator, test_indexes in zip(estimators, indices['test']):
                 y_true = y[y.index[test_indexes]]
                 y_est = estimator.predict(x.loc[x.index[test_indexes], :])
+                if isinstance(y_est, pd.DataFrame) and y_est.shape[1] == 1:
+                    y_est = y_est.iloc[:, 0]
                 metric_values.append(fn_metric(y_true, y_est))
                 if group is not None:
                     # calculate the metric by each group in the group series.
                     y_est = pd.merge(left=pd.Series(y_est, name='y_est', index=x.index[test_indexes]),
                                      right=group, left_index=True, right_index=True)
                     y_est_grouped = y_est.groupby([group.name])
                     grouped_results = [y_est_grouped.get_group(x) for x in y_est_grouped.groups]
```

### Comparing `sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/models.py` & `sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/models.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.1/elphick/sklearn_viz/residuals/error.py` & `sklearn_viz-0.4.0/elphick/sklearn_viz/residuals/error.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.1/elphick/sklearn_viz/utils/timer.py` & `sklearn_viz-0.4.0/elphick/sklearn_viz/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.1/LICENSE` & `sklearn_viz-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.1/pyproject.toml` & `sklearn_viz-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sklearn-viz"
-version = "0.3.1"
+version = "0.4.0"
 description = ""
 authors = ["Greg <11791585+elphick@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "elphick/sklearn_viz" }]
 
 [[tool.poetry.source]]
 name = "PyPI"
```

### Comparing `sklearn_viz-0.3.1/PKG-INFO` & `sklearn_viz-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-viz
-Version: 0.3.1
+Version: 0.4.0
 Summary: 
 Author: Greg
 Author-email: 11791585+elphick@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

