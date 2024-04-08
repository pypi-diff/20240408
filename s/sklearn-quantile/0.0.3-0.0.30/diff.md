# Comparing `tmp/sklearn_quantile-0.0.3.tar.gz` & `tmp/sklearn-quantile-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_quantile-0.0.3.tar", last modified: Fri Feb  4 17:31:28 2022, max compression
+gzip compressed data, was "sklearn-quantile-0.0.30.tar", last modified: Mon Apr  8 20:39:00 2024, max compression
```

## Comparing `sklearn_quantile-0.0.3.tar` & `sklearn-quantile-0.0.30.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.577214 sklearn_quantile-0.0.3/
--rw-r--r--   0 jroebroek   (501) staff       (20)     1515 2022-01-18 08:10:04.000000 sklearn_quantile-0.0.3/LICENSE
--rw-r--r--   0 jroebroek   (501) staff       (20)       42 2022-02-04 17:05:29.000000 sklearn_quantile-0.0.3/MANIFEST.in
--rw-r--r--   0 jroebroek   (501) staff       (20)     2784 2022-02-04 17:31:28.577307 sklearn_quantile-0.0.3/PKG-INFO
--rw-r--r--   0 jroebroek   (501) staff       (20)     2452 2022-02-04 17:30:34.000000 sklearn_quantile-0.0.3/README.md
--rw-r--r--   0 jroebroek   (501) staff       (20)       79 2022-02-04 17:31:28.577714 sklearn_quantile-0.0.3/setup.cfg
--rw-r--r--   0 jroebroek   (501) staff       (20)     1282 2022-02-04 17:31:23.000000 sklearn_quantile-0.0.3/setup.py
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.567810 sklearn_quantile-0.0.3/sklearn_quantile/
--rw-r--r--   0 jroebroek   (501) staff       (20)      290 2022-02-03 17:30:06.000000 sklearn_quantile-0.0.3/sklearn_quantile/__init__.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     1367 2022-02-03 18:27:39.000000 sklearn_quantile-0.0.3/sklearn_quantile/base.py
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.573440 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/
--rw-r--r--   0 jroebroek   (501) staff       (20)      223 2022-02-03 17:29:39.000000 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/__init__.py
--rw-r--r--   0 jroebroek   (501) staff       (20)  1150275 2022-02-04 14:41:20.000000 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/maximum.c
--rw-r--r--   0 jroebroek   (501) staff       (20)     5873 2022-02-04 14:41:17.000000 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/maximum.pyx
--rw-r--r--   0 jroebroek   (501) staff       (20)  1523734 2022-02-04 15:19:36.000000 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/quantile.c
--rw-r--r--   0 jroebroek   (501) staff       (20)    52546 2022-02-04 15:19:33.000000 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/quantile.pyx
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.573955 sklearn_quantile-0.0.3/sklearn_quantile/neighbors/
--rw-r--r--   0 jroebroek   (501) staff       (20)       50 2022-02-04 09:23:10.000000 sklearn_quantile-0.0.3/sklearn_quantile/neighbors/__init__.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     7220 2022-02-04 11:44:21.000000 sklearn_quantile-0.0.3/sklearn_quantile/neighbors/quantile.py
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.576811 sklearn_quantile-0.0.3/sklearn_quantile/utils/
--rw-r--r--   0 jroebroek   (501) staff       (20)       49 2022-01-17 17:41:49.000000 sklearn_quantile-0.0.3/sklearn_quantile/utils/__init__.py
--rw-r--r--   0 jroebroek   (501) staff       (20)  1066554 2022-02-04 11:36:32.000000 sklearn_quantile-0.0.3/sklearn_quantile/utils/weighted_quantile.c
--rw-r--r--   0 jroebroek   (501) staff       (20)      685 2021-06-10 12:55:07.000000 sklearn_quantile-0.0.3/sklearn_quantile/utils/weighted_quantile.pxd
--rw-r--r--   0 jroebroek   (501) staff       (20)    12224 2022-02-04 11:36:30.000000 sklearn_quantile-0.0.3/sklearn_quantile/utils/weighted_quantile.pyx
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.568901 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/
--rw-r--r--   0 jroebroek   (501) staff       (20)     2784 2022-02-04 17:31:28.000000 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/PKG-INFO
--rw-r--r--   0 jroebroek   (501) staff       (20)      767 2022-02-04 17:31:28.000000 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/SOURCES.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)        1 2022-02-04 17:31:28.000000 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/dependency_links.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)       91 2022-02-04 17:31:28.000000 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/requires.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)       17 2022-02-04 17:31:28.000000 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/top_level.txt
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.577029 sklearn_quantile-0.0.3/tests/
--rw-r--r--   0 jroebroek   (501) staff       (20)     3987 2022-02-04 11:40:57.000000 sklearn_quantile-0.0.3/tests/test_weighted_quantile.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2024-04-08 20:39:00.300069 sklearn-quantile-0.0.30/
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1515 2023-09-25 08:23:52.000000 sklearn-quantile-0.0.30/LICENSE
+-rw-r--r--   0 jroebroek   (501) staff       (20)       73 2023-09-20 15:41:33.000000 sklearn-quantile-0.0.30/MANIFEST.in
+-rw-r--r--   0 jroebroek   (501) staff       (20)     6649 2024-04-08 20:39:00.299614 sklearn-quantile-0.0.30/PKG-INFO
+-rw-r--r--   0 jroebroek   (501) staff       (20)     3214 2022-02-28 07:49:20.000000 sklearn-quantile-0.0.30/README.md
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1225 2024-04-08 20:38:58.000000 sklearn-quantile-0.0.30/pyproject.toml
+-rw-r--r--   0 jroebroek   (501) staff       (20)       38 2024-04-08 20:39:00.300168 sklearn-quantile-0.0.30/setup.cfg
+-rw-r--r--   0 jroebroek   (501) staff       (20)      786 2024-04-08 20:38:58.000000 sklearn-quantile-0.0.30/setup.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2024-04-08 20:39:00.291290 sklearn-quantile-0.0.30/sklearn_quantile/
+-rw-r--r--   0 jroebroek   (501) staff       (20)      290 2022-02-03 17:30:06.000000 sklearn-quantile-0.0.30/sklearn_quantile/__init__.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1366 2023-09-21 08:13:53.000000 sklearn-quantile-0.0.30/sklearn_quantile/base.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2024-04-08 20:39:00.293465 sklearn-quantile-0.0.30/sklearn_quantile/ensemble/
+-rw-r--r--   0 jroebroek   (501) staff       (20)      273 2023-04-13 13:11:21.000000 sklearn-quantile-0.0.30/sklearn_quantile/ensemble/__init__.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     5820 2024-04-08 20:36:29.000000 sklearn-quantile-0.0.30/sklearn_quantile/ensemble/maximum.pyx
+-rw-r--r--   0 jroebroek   (501) staff       (20)    63221 2024-04-08 20:36:29.000000 sklearn-quantile-0.0.30/sklearn_quantile/ensemble/quantile.pyx
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2024-04-08 20:39:00.294224 sklearn-quantile-0.0.30/sklearn_quantile/neighbors/
+-rw-r--r--   0 jroebroek   (501) staff       (20)       76 2023-04-13 13:11:22.000000 sklearn-quantile-0.0.30/sklearn_quantile/neighbors/__init__.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     7220 2022-02-04 11:44:21.000000 sklearn-quantile-0.0.30/sklearn_quantile/neighbors/quantile.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2024-04-08 20:39:00.295707 sklearn-quantile-0.0.30/sklearn_quantile/utils/
+-rw-r--r--   0 jroebroek   (501) staff       (20)       71 2023-04-13 13:11:22.000000 sklearn-quantile-0.0.30/sklearn_quantile/utils/__init__.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)      355 2024-04-08 20:31:33.000000 sklearn-quantile-0.0.30/sklearn_quantile/utils/utils.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)      678 2023-09-25 09:18:00.000000 sklearn-quantile-0.0.30/sklearn_quantile/utils/weighted_quantile.pxd
+-rw-r--r--   0 jroebroek   (501) staff       (20)    12400 2023-09-25 09:13:13.000000 sklearn-quantile-0.0.30/sklearn_quantile/utils/weighted_quantile.pyx
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2024-04-08 20:39:00.297092 sklearn-quantile-0.0.30/sklearn_quantile.egg-info/
+-rw-r--r--   0 jroebroek   (501) staff       (20)     6649 2024-04-08 20:39:00.000000 sklearn-quantile-0.0.30/sklearn_quantile.egg-info/PKG-INFO
+-rw-r--r--   0 jroebroek   (501) staff       (20)      741 2024-04-08 20:39:00.000000 sklearn-quantile-0.0.30/sklearn_quantile.egg-info/SOURCES.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)        1 2024-04-08 20:39:00.000000 sklearn-quantile-0.0.30/sklearn_quantile.egg-info/dependency_links.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)      257 2024-04-08 20:39:00.000000 sklearn-quantile-0.0.30/sklearn_quantile.egg-info/requires.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)       17 2024-04-08 20:39:00.000000 sklearn-quantile-0.0.30/sklearn_quantile.egg-info/top_level.txt
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2024-04-08 20:39:00.296712 sklearn-quantile-0.0.30/tests/
+-rw-r--r--   0 jroebroek   (501) staff       (20)     2368 2022-02-04 16:03:51.000000 sklearn-quantile-0.0.30/tests/test_quantile_KNN.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     7327 2023-09-21 08:28:04.000000 sklearn-quantile-0.0.30/tests/test_quantile_RF.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     3987 2022-02-04 11:40:57.000000 sklearn-quantile-0.0.30/tests/test_weighted_quantile.py
```

### Comparing `sklearn_quantile-0.0.3/LICENSE` & `sklearn-quantile-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_quantile-0.0.3/README.md` & `sklearn-quantile-0.0.30/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -16,18 +16,42 @@
   - ExtraTreesQuantileRegressor: the main implementation
   - SampleExtraTreesQuantileRegressor: an approximation, that is much faster than the main implementation.
 
 - Quantile K-nearest neighbors (KNeighborsQuantileRegressor)
 
 # Installation
 
-The package can be installed with pip (when cython and scikit-learn are already installed):
+The package can be installed with conda:
 
 ```
-pip install sklearn-quantile
+conda install --channel conda-forge sklearn-quantile
 ```
 
 # Example
 
 An example of Random Forest Quantile Regression in action (both the main implementation and its approximation):
 
-<img src="https://github.com/jasperroebroek/sklearn-quantile/raw/master/tests/examples/readme_example.png"/>
+<img src="https://github.com/jasperroebroek/sklearn-quantile/raw/master/docs/source/notebooks/example.png"/>
+
+# Usage example
+
+Random Forest Quantile Regressor predicting the 5th, 50th and 95th percentile of the California housing dataset.
+
+```
+from sklearn.datasets import fetch_california_housing
+from sklearn.model_selection import train_test_split
+from sklearn_quantile import RandomForestQuantileRegressor
+
+X, y = fetch_california_housing(return_X_y=True)
+X_train, X_test, y_train, y_test = train_test_split(X, y, train_size=0.5, random_state=0)
+
+qrf = RandomForestQuantileRegressor(q=[0.05, 0.50, 0.95])
+qrf.fit(X_train, y_train)
+
+y_pred_5, y_pred_median, y_pred_95 = qrf.predict(X_test)
+qrf.score(X_test, y_test)
+```
+
+# Important links
+
+- API reference: https://sklearn-quantile.readthedocs.io/en/latest/api.html
+- Documentation: https://sklearn-quantile.readthedocs.io/en/latest/index.html
```

### Comparing `sklearn_quantile-0.0.3/sklearn_quantile/base.py` & `sklearn-quantile-0.0.30/sklearn_quantile/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
             raise ValueError("Quantiles must be in the range [0, 1]")
 
         return q
 
     def score(self, X, y):
         """
         Mean pinball loss for the quantile regressors.
-
         The average over all quantiles is calculated when more than one is provided.
         """
         q = self.validate_quantiles()
         y_pred = self.predict(X)
         losses = np.empty(q.size)
         for i in range(q.size):
             losses[i] = mean_pinball_loss(y, y_pred[i], alpha=q[i])
```

### Comparing `sklearn_quantile-0.0.3/sklearn_quantile/ensemble/maximum.pyx` & `sklearn-quantile-0.0.30/sklearn_quantile/ensemble/maximum.pyx`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,77 @@
 # cython: cdivision=True
 # cython: boundscheck=False
 # cython: wraparound=False
-# cython: profile=True
 
 # Authors: Jasper Roebroek <roebroek.jasper@gmail.com>
 # License: BSD 3 clause
 
 """
 Module providing the special case for quantile regression: predicting the maximum.
 It only has a single implementation called RandomForestMaxRegression, which has the
 same parameters as the regular RandomForestRegressor
 """
 import threading
 
-import joblib
-from cython.parallel cimport prange
-cimport openmp
-cimport numpy as np
 from joblib import Parallel
 
 import numpy as np
+cimport numpy as cnp
 from sklearn.tree import DecisionTreeRegressor
-from sklearn.utils.fixes import delayed, _joblib_parallel_args
-from sklearn.utils.validation import check_is_fitted, check_X_y
+from sklearn.utils.fixes import delayed
+from sklearn.utils.validation import check_is_fitted
 from sklearn.ensemble._base import _partition_estimators
-from sklearn.ensemble._forest import _generate_sample_indices
+from sklearn.ensemble._forest import ForestRegressor
 
 from sklearn_quantile.ensemble.quantile import BaseForestQuantileRegressor
 
 
-ctypedef np.npy_intp SIZE_t              # Type for indices and counters
+ctypedef cnp.intp_t SSIZE_t              # Type for indices and counters
 
 
 __all__ = ["RandomForestMaximumRegressor"]
 
 
-cdef void _maximum_per_leaf(SIZE_t[::1] leaves,
-                            SIZE_t[::1] unique_leaves,
+cdef void _maximum_per_leaf(SSIZE_t[::1] leaves,
                             float[::1] values,
-                            SIZE_t[::1] idx,
-                            float[::1] sampled_values,
-                            SIZE_t n_jobs):
-    """
-    Index of maximum value for each unique leaf
+                            float[::1] tree_values) nogil:
 
+    """
+    Store the highest value found for each leaf in the tree_values array.
+    
     Parameters
     ----------
     leaves : array, shape = (n_samples)
-        Leaves of a Regression tree, corresponding to weights and indices (idx)
-    unique_leaves : array, shape = (n_unique_leaves)
+        Leaves of a Regression tree, corresponding to locations in the tree_values array.
     values : array, shape = (n_samples)
-    idx : array, shape = (n_samples)
-        Indices of original observations. The output will drawn from this.
-    sampled_idx : shape = (n_unique_leaves)
-    n_jobs : number of threads, similar to joblib
+    tree_values: array, shape = (n_nodes)
+        Initialised with -np.inf. Filled at leaf nodes with highest value
     """
     cdef:
-        int i, j
-        double c_leaf
-        float c_max
-
-        int n_unique_leaves = unique_leaves.shape[0]
+        int i
+        ssize_t c_leaf
         int n_samples = leaves.shape[0]
 
-        int num_threads = joblib.effective_n_jobs(n_jobs)
+    with nogil:
+        for i in range(n_samples):
+            c_leaf = leaves[i]
+            if c_leaf == -1:
+                continue
+            if values[i] > tree_values[c_leaf]:
+                tree_values[c_leaf] = values[i]
+
+
+def _fit_each_tree(est):
+    values = np.full(est.tree_.node_count, dtype=np.float32, fill_value=-np.inf)
+
+    _maximum_per_leaf(leaves=est.y_train_leaves_,
+                      values=est.y_train_[:, 0],
+                      tree_values=values)
 
-    for i in prange(n_samples, num_threads=num_threads, nogil=True):
-        c_leaf = leaves[i]
-        for j in range(n_unique_leaves):
-            if unique_leaves[j] == c_leaf:
-                break
-
-        if values[i] > sampled_values[j]:
-            sampled_values[j] = values[i]
+    est.tree_.value[:, 0, 0] = values
 
 
 def _accumulate_prediction(predict, X, out, lock):
     """
     This is a utility function for joblib's Parallel. Based on the version in sklearn.ensemble._forest
     """
     prediction = predict(X, check_input=False)
@@ -88,87 +83,104 @@
     """
     A random forest regressor predicting conditional maxima
 
     Implementation is equivalent to Random Forest Quantile Regressor,
     but calculation is much faster. For other quantiles revert to the
     original predictor.
     """
-    def __init__(self,
-                 n_estimators=10,
-                 criterion='mse',
-                 max_depth=None,
-                 min_samples_split=2,
-                 min_samples_leaf=1,
-                 min_weight_fraction_leaf=0.0,
-                 max_features='auto',
-                 max_leaf_nodes=None,
-                 bootstrap=True,
-                 oob_score=False,
-                 n_jobs=1,
-                 random_state=None,
-                 verbose=0,
-                 warm_start=False):
-        super(BaseForestQuantileRegressor, self).__init__(
-            base_estimator=DecisionTreeRegressor(),
+    _parameter_constraints: dict = {
+        **ForestRegressor._parameter_constraints,
+        **DecisionTreeRegressor._parameter_constraints,
+    }
+    _parameter_constraints.pop("splitter")
+
+    def __init__(
+            self,
+            n_estimators=100,
+            *,
+            criterion="squared_error",
+            max_depth=None,
+            min_samples_split=2,
+            min_samples_leaf=1,
+            min_weight_fraction_leaf=0.0,
+            max_features=1.0,
+            max_leaf_nodes=None,
+            min_impurity_decrease=0.0,
+            bootstrap=True,
+            oob_score=False,
+            n_jobs=None,
+            random_state=None,
+            verbose=0,
+            warm_start=False,
+            ccp_alpha=0.0,
+            max_samples=None,
+            monotonic_cst=None,
+    ):
+        super().__init__(
+            estimator=DecisionTreeRegressor(),
             n_estimators=n_estimators,
-            estimator_params=("criterion", "max_depth", "min_samples_split",
-                              "min_samples_leaf", "min_weight_fraction_leaf",
-                              "max_features", "max_leaf_nodes",
-                              "random_state"),
+            estimator_params=(
+                "criterion",
+                "max_depth",
+                "min_samples_split",
+                "min_samples_leaf",
+                "min_weight_fraction_leaf",
+                "max_features",
+                "max_leaf_nodes",
+                "min_impurity_decrease",
+                "random_state",
+                "ccp_alpha",
+                "monotonic_cst",
+            ),
             bootstrap=bootstrap,
             oob_score=oob_score,
             n_jobs=n_jobs,
             random_state=random_state,
             verbose=verbose,
-            warm_start=warm_start)
+            warm_start=warm_start,
+            max_samples=max_samples,
+        )
 
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
+        self.min_impurity_decrease = min_impurity_decrease
+        self.ccp_alpha = ccp_alpha
+        self.monotonic_cst = monotonic_cst
         self.q = 1
 
     def fit(self, X, y, sample_weight=None):
         super(RandomForestMaximumRegressor, self).fit(X, y, sample_weight)
 
-        for i, est in enumerate(self.estimators_):
-            if self.verbose:
-                print(f"Sampling tree {i+1} of {self.n_estimators}")
-
-            mask = est.y_weights_ > 0
+        print("Sampling maximum per tree")
 
-            leaves = est.y_train_leaves_[mask]
-            idx = np.arange(self.n_samples_, dtype=np.intp)[mask]
-
-            unique_leaves = np.unique(leaves)
-
-            sampled_values = np.full(len(unique_leaves), -np.inf, dtype=np.float32)
-            _maximum_per_leaf(leaves, unique_leaves, est.y_train_[mask, 0], idx, sampled_values, self.n_jobs)
-
-            est.tree_.value[unique_leaves, 0, 0] = sampled_values
+        n_jobs, _, _ = _partition_estimators(self.n_estimators, self.n_jobs)
+        Parallel(n_jobs=n_jobs, verbose=self.verbose, require="sharedmem")(
+            delayed(_fit_each_tree)(e)
+            for e in self.estimators_)
 
         return self
 
     def predict(self, X):
         """
         predition, based on the predict function of ForestRegressor
         """
         check_is_fitted(self)
         # Check data
         X = self._validate_X_predict(X)
 
         # Assign chunk of trees to jobs
         n_jobs, _, _ = _partition_estimators(self.n_estimators, self.n_jobs)
 
-        y_hat = np.zeros(X.shape[0], dtype=np.float64)
+        y_hat = np.zeros(X.shape[0], dtype=np.float32)
 
         # Parallel loop
         lock = threading.Lock()
-        Parallel(n_jobs=n_jobs, verbose=self.verbose,
-                 **_joblib_parallel_args(require="sharedmem"))(
+        Parallel(n_jobs=n_jobs, verbose=self.verbose,require="sharedmem")(
             delayed(_accumulate_prediction)(e.predict, X, y_hat, lock)
             for e in self.estimators_)
 
         return y_hat
```

### Comparing `sklearn_quantile-0.0.3/sklearn_quantile/ensemble/quantile.pyx` & `sklearn-quantile-0.0.30/sklearn_quantile/ensemble/quantile.pyx`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,73 @@
 # cython: cdivision=True
 # cython: boundscheck=False
 # cython: wraparound=False
-# cython: profile=True
 
 # Authors: Jasper Roebroek <roebroek.jasper@gmail.com>
 # License: BSD 3 clause
 
 """
-This module is inspired on the skgarden implementation of Forest Quantile Regression,
-based on the following paper:
-
+Based on the following paper:
 Nicolai Meinshausen, Quantile Regression Forests
 http://www.jmlr.org/papers/volume7/meinshausen06a/meinshausen06a.pdf
 """
-from cython.parallel cimport prange
-cimport openmp
-cimport numpy as np
-from numpy cimport ndarray
+from libc.math cimport isnan
+
+cimport numpy as cnp
 
-from sklearn_quantile.utils.weighted_quantile cimport _weighted_quantile_presorted_1D, \
-    _weighted_quantile_unchecked_1D, Interpolation
+from sklearn_quantile.utils.weighted_quantile cimport _weighted_quantile_presorted_1D, Interpolation
 
 from abc import ABCMeta, abstractmethod
 
 import numpy as np
-from numpy.lib.function_base import _quantile_is_valid
 import threading
-import joblib
 from joblib import Parallel
 
 from sklearn.ensemble._forest import ForestRegressor, _accumulate_prediction, _generate_sample_indices
 from sklearn.ensemble._base import _partition_estimators
 from sklearn.utils.fixes import delayed
-from sklearn.utils.fixes import _joblib_parallel_args
 from sklearn.tree import DecisionTreeRegressor, ExtraTreeRegressor
 from sklearn.utils import check_array, check_X_y, check_random_state
 from sklearn.utils.validation import check_is_fitted
-from sklearn.metrics import mean_pinball_loss
 from sklearn_quantile.base import QuantileRegressorMixin
 
-ctypedef np.npy_intp SIZE_t              # Type for indices and counters
+ctypedef cnp.npy_intp SSIZE_t              # Type for indices and counters
 
 
 __all__ = ["RandomForestQuantileRegressor", "ExtraTreesQuantileRegressor", "SampleRandomForestQuantileRegressor",
            "SampleExtraTreesQuantileRegressor"]
 
 
-cpdef void _quantile_forest_predict(SIZE_t[:, ::1] X_leaves,
+cpdef void _quantile_forest_predict(SSIZE_t[:, ::1] X_leaves,
                                     float[:, ::1] y_train,
-                                    SIZE_t[:, ::1] y_train_leaves,
+                                    SSIZE_t[:, ::1] y_train_leaves,
                                     float[:, ::1] y_weights,
                                     float[::1] q,
                                     float[:, :, ::1] quantiles,
-                                    SIZE_t start,
-                                    SIZE_t stop):
+                                    SSIZE_t start,
+                                    SSIZE_t stop):
     """
     X_leaves : (n_estimators, n_test_samples)
     y_train : (n_samples, n_outputs)
     y_train_leaves : (n_estimators, n_samples)
     y_weights : (n_estimators, n_samples)
     q : (n_q)
     quantiles : output array (n_q, n_test_samples, n_outputs)
     start, stop : indices to break up computation across threads (used in range)
     """
-    # todo; this does not compile with function cdef, only with cpdef
+    # todo; remove option for having more than one output variable?
 
     cdef:
-        int n_estimators = X_leaves.shape[0]
-        int n_outputs = y_train.shape[1]
-        int n_q = q.shape[0]
-        int n_samples = y_train.shape[0]
-        int n_test_samples = X_leaves.shape[1]
+        size_t n_estimators = X_leaves.shape[0]
+        size_t n_outputs = y_train.shape[1]
+        size_t n_q = q.shape[0]
+        size_t n_samples = y_train.shape[0]
+        size_t n_test_samples = X_leaves.shape[1]
 
-        int i, j, e, o, count_samples
+        long i, j, e, o, count_samples
         float curr_weight
         bint sorted = y_train.shape[1] == 1
 
         float[::1] x_weights = np.empty(n_samples, dtype=np.float32)
         float[:, ::1] x_a = np.empty((n_samples, n_outputs), dtype=np.float32)
 
     with nogil:
@@ -92,63 +83,68 @@
                     x_a[count_samples] = y_train[j]
                     count_samples = count_samples + 1
             if sorted:
                 _weighted_quantile_presorted_1D(x_a[:count_samples, 0],
                                                 q, x_weights[:count_samples],
                                                 quantiles[:, i, 0], Interpolation.linear)
             else:
-                for o in range(n_outputs):
-                    _weighted_quantile_unchecked_1D(x_a[:count_samples, o], q, x_weights[:count_samples],
-                                                    quantiles[:, i, o], Interpolation.linear)
+                with gil:
+                    raise NotImplemented("Multiple features are currently not supported")
+                # for o in range(n_outputs):
+                #     _weighted_quantile_unchecked_1D(x_a[:count_samples, o], q, x_weights[:count_samples],
+                #                                     quantiles[:, i, o], Interpolation.linear)
 
 
-cdef void _weighted_random_sample(SIZE_t[::1] leaves,
-                                  SIZE_t[::1] unique_leaves,
+cdef void _weighted_random_sample(SSIZE_t[::1] leaves,
+                                  float[::1] values,
                                   float[::1] weights,
-                                  SIZE_t[::1] idx,
-                                  double[::1] random_numbers,
-                                  SIZE_t[::1] sampled_idx,
-                                  SIZE_t n_jobs):
+                                  float[::1] random_numbers,
+                                  float[::1] tree_values) nogil:
     """
     Random sample for each unique leaf
 
     Parameters
     ----------
     leaves : array, shape = (n_samples)
-        Leaves of a Regression tree, corresponding to weights and indices (idx)
-    unique_leaves : array, shape = (n_unique_leaves)
-
+        Leaves of a Regression tree, corresponding to random_numbers and tree_values
+    values : array, shape = (n_samples)
     weights : array, shape = (n_samples)
         Weights for each observation. They need to sum up to 1 per unique leaf.
-    idx : array, shape = (n_samples)
-        Indices of original observations. The output will drawn from this.
-    random numbers : array, shape = (n_unique_leaves)
-    sampled_idx : shape = (n_unique_leaves)
-    n_jobs : number of threads, similar to joblib
+    random numbers : array, shape = (n_nodes)
+    tree_values: array, shape = (n_nodes)
     """
+
     cdef:
-        long c_leaf
-        float p, r
-        int i, j
-
-        int n_unique_leaves = unique_leaves.shape[0]
-        int n_samples = weights.shape[0]
-        int num_threads = joblib.effective_n_jobs(n_jobs)
-
-    for i in prange(n_unique_leaves, nogil=True, num_threads=num_threads):
-        p = 0
-        r = random_numbers[i]
-        c_leaf = unique_leaves[i]
-
-        for j in range(n_samples):
-            if leaves[j] == c_leaf:
-                p = p + weights[j]
-                if p > r:
-                    sampled_idx[i] = idx[j]
-                    break
+        int i
+        ssize_t c_leaf
+        int n_samples = leaves.shape[0]
+
+    with nogil:
+        for i in range(n_samples):
+            c_leaf = leaves[i]
+            if c_leaf == -1:
+                continue
+
+            random_numbers[c_leaf] -= weights[i]
+            if random_numbers[c_leaf] <= 0 and isnan(tree_values[c_leaf]):
+                tree_values[c_leaf] = values[i]
+
+
+def _fit_sample_tree(est):
+    random_instance = check_random_state(est.random_state)
+    random_numbers = random_instance.rand(est.tree_.node_count).astype(np.float32)
+    values = np.full(est.tree_.node_count, dtype=np.float32, fill_value=np.nan)
+
+    _weighted_random_sample(leaves=est.y_train_leaves_,
+                            values=est.y_train_[:, 0],
+                            weights=est.y_weights_,
+                            random_numbers=random_numbers,
+                            tree_values=values)
+
+    est.tree_.value[:, 0, 0] = values
 
 
 def _accumulate_prediction(predict, X, i, out, lock):
     """
     Adapted from sklearn.ensemble._forest
     """
     prediction = predict(X, check_input=False)
@@ -191,21 +187,26 @@
         Returns
         -------
         self : object
             Returns self.
         """
         # apply method requires X to be of dtype np.float32
         # multi-output should likely work, but tests need to be written first.
-        #   known case of error: maximum regressor
-        X, y = check_X_y(
-            X, y, accept_sparse="csc", dtype=np.float32, multi_output=False)
+        X, y = check_X_y(X, y, accept_sparse="csc", dtype=np.float32, multi_output=False)
+
+        if self.verbose:
+            print("Training forest")
         super(BaseForestQuantileRegressor, self).fit(X, y, sample_weight=sample_weight)
 
         self.n_samples_ = len(y)
         self.y_train_ = y.reshape((-1, self.n_outputs_)).astype(np.float32)
+
+        if self.verbose:
+            print("Applying training samples")
+
         self.y_train_leaves_ = self.apply(X).T
         self.y_weights_ = np.zeros_like(self.y_train_leaves_, dtype=np.float32)
 
         if sample_weight is None:
             sample_weight = np.ones(self.n_samples_)
 
         for i, est in enumerate(self.estimators_):
@@ -282,16 +283,15 @@
 
         chunks = np.full(n_jobs, n_test_samples//n_jobs)
         chunks[:n_test_samples % n_jobs] +=1
         chunks = np.cumsum(np.insert(chunks, 0, 0))
 
         quantiles = np.empty((q.size, n_test_samples, self.n_outputs_), dtype=np.float32)
 
-        Parallel(n_jobs=n_jobs, verbose=self.verbose,
-                 **_joblib_parallel_args(require="sharedmem"))(
+        Parallel(n_jobs=n_jobs, verbose=self.verbose,require="sharedmem")(
             delayed(_quantile_forest_predict)(X_leaves, self.y_train_, self.y_train_leaves_, self.y_weights_, q,
                                               quantiles, chunks[i], chunks[i+1])
             for i in range(n_jobs))
 
         if q.size == 1:
             quantiles = quantiles[0]
         if self.n_outputs_ == 1:
@@ -305,35 +305,19 @@
     Base class for forest quantile regressors (both random forest and extree trees),
     fitting and predicting according to the approximation method chosen in the R package
     quantregForest.
     """
     def fit(self, X, y, sample_weight=None):
         super(SampleForestQuantileRegressor, self).fit(X, y, sample_weight=sample_weight)
 
-        for i, est in enumerate(self.estimators_):
-            if self.verbose:
-                print(f"Sampling tree {i+1} of {self.n_estimators}")
-
-            mask = est.y_weights_ > 0
-
-            leaves = est.y_train_leaves_[mask]
-            idx = np.arange(self.n_samples_, dtype=np.intp)[mask]
-
-            unique_leaves = np.unique(leaves)
-
-            random_instance = check_random_state(est.random_state)
-            random_numbers = random_instance.rand(len(unique_leaves))
-
-            sampled_idx = np.empty(len(unique_leaves), dtype=np.intp)
-            n_jobs, _, _ = _partition_estimators(self.n_estimators, self.n_jobs)
-
-            _weighted_random_sample(leaves, unique_leaves, est.y_weights_[mask], idx, random_numbers, sampled_idx,
-                                    n_jobs)
-
-            est.tree_.value[unique_leaves, :, 0] = self.y_train_[sampled_idx]
+        print("Sampling trees")
+        n_jobs, _, _ = _partition_estimators(self.n_estimators, self.n_jobs)
+        Parallel(n_jobs=n_jobs, verbose=self.verbose, require="sharedmem")(
+            delayed(_fit_sample_tree)(e)
+            for e in self.estimators_)
 
         return self
 
     def predict(self, X):
         check_is_fitted(self)
         q = self.validate_quantiles()
 
@@ -342,16 +326,15 @@
 
         # apply method requires X to be of dtype np.float32
         X = check_array(X, dtype=np.float32, accept_sparse="csc")
 
         predictions = np.empty((len(X), self.n_outputs_, self.n_estimators))
 
         lock = threading.Lock()
-        Parallel(n_jobs=n_jobs, verbose=self.verbose,
-                 **_joblib_parallel_args(require="sharedmem"))(
+        Parallel(n_jobs=n_jobs, verbose=self.verbose,require="sharedmem")(
             delayed(_accumulate_prediction)(est.predict, X, i, predictions, lock)
             for i, est in enumerate(self.estimators_))
 
         quantiles = np.quantile(predictions, q=q, axis=-1)
         if q.size == 1:
             quantiles = quantiles[0]
         if self.n_outputs_ == 1:
@@ -365,164 +348,314 @@
     """
     A random forest regressor providing quantile estimates.
 
     Note that this implementation is rather slow for large datasets. Above 10000 samples
     it is recommended to use func:`sklearn_quantile.SampleRandomForestQuantileRegressor`,
     which is a model approximating the true conditional quantile.
 
-    Parameters
+	Parameters
     ----------
     q : float or array-like, optional
         Quantiles used for prediction (values ranging from 0 to 1)
 
-    n_estimators : integer, optional (default=10)
+    n_estimators : int, default=100
         The number of trees in the forest.
 
-    criterion : string, optional (default="mse")
+        .. versionchanged:: 0.22
+           The default value of ``n_estimators`` changed from 10 to 100
+           in 0.22.
+
+    criterion : {"squared_error", "absolute_error", "friedman_mse", "poisson"}, \
+            default="squared_error"
         The function to measure the quality of a split. Supported criteria
-        are "mse" for the mean squared error, which is equal to variance
-        reduction as feature selection criterion, and "mae" for the mean
-        absolute error.
+        are "squared_error" for the mean squared error, which is equal to
+        variance reduction as feature selection criterion and minimizes the L2
+        loss using the mean of each terminal node, "friedman_mse", which uses
+        mean squared error with Friedman's improvement score for potential
+        splits, "absolute_error" for the mean absolute error, which minimizes
+        the L1 loss using the median of each terminal node, and "poisson" which
+        uses reduction in Poisson deviance to find splits.
+        Training using "absolute_error" is significantly slower
+        than when using "squared_error".
+
         .. versionadded:: 0.18
            Mean Absolute Error (MAE) criterion.
 
-    max_features : int, float, string or None, optional (default="auto")
-        The number of features to consider when looking for the best split:
-        - If int, then consider `max_features` features at each split.
-        - If float, then `max_features` is a percentage and
-          `int(max_features * n_features)` features are considered at each
-          split.
-        - If "auto", then `max_features=n_features`.
-        - If "sqrt", then `max_features=sqrt(n_features)`.
-        - If "log2", then `max_features=log2(n_features)`.
-        - If None, then `max_features=n_features`.
-        Note: the search for a split does not stop until at least one
-        valid partition of the node samples is found, even if it requires to
-        effectively inspect more than ``max_features`` features.
+        .. versionadded:: 1.0
+           Poisson criterion.
 
-    max_depth : integer or None, optional (default=None)
+    max_depth : int, default=None
         The maximum depth of the tree. If None, then nodes are expanded until
         all leaves are pure or until all leaves contain less than
         min_samples_split samples.
 
-    min_samples_split : int, float, optional (default=2)
+    min_samples_split : int or float, default=2
         The minimum number of samples required to split an internal node:
+
         - If int, then consider `min_samples_split` as the minimum number.
-        - If float, then `min_samples_split` is a percentage and
+        - If float, then `min_samples_split` is a fraction and
           `ceil(min_samples_split * n_samples)` are the minimum
           number of samples for each split.
+
         .. versionchanged:: 0.18
-           Added float values for percentages.
+           Added float values for fractions.
+
+    min_samples_leaf : int or float, default=1
+        The minimum number of samples required to be at a leaf node.
+        A split point at any depth will only be considered if it leaves at
+        least ``min_samples_leaf`` training samples in each of the left and
+        right branches.  This may have the effect of smoothing the model,
+        especially in regression.
 
-    min_samples_leaf : int, float, optional (default=1)
-        The minimum number of samples required to be at a leaf node:
         - If int, then consider `min_samples_leaf` as the minimum number.
-        - If float, then `min_samples_leaf` is a percentage and
+        - If float, then `min_samples_leaf` is a fraction and
           `ceil(min_samples_leaf * n_samples)` are the minimum
           number of samples for each node.
+
         .. versionchanged:: 0.18
-           Added float values for percentages.
+           Added float values for fractions.
 
-    min_weight_fraction_leaf : float, optional (default=0.)
+    min_weight_fraction_leaf : float, default=0.0
         The minimum weighted fraction of the sum total of weights (of all
         the input samples) required to be at a leaf node. Samples have
         equal weight when sample_weight is not provided.
 
-    max_leaf_nodes : int or None, optional (default=None)
+    max_features : {"sqrt", "log2", None}, int or float, default=1.0
+        The number of features to consider when looking for the best split:
+
+        - If int, then consider `max_features` features at each split.
+        - If float, then `max_features` is a fraction and
+          `max(1, int(max_features * n_features_in_))` features are considered at each
+          split.
+        - If "sqrt", then `max_features=sqrt(n_features)`.
+        - If "log2", then `max_features=log2(n_features)`.
+        - If None or 1.0, then `max_features=n_features`.
+
+        .. note::
+            The default of 1.0 is equivalent to bagged trees and more
+            randomness can be achieved by setting smaller values, e.g. 0.3.
+
+        .. versionchanged:: 1.1
+            The default of `max_features` changed from `"auto"` to 1.0.
+
+        Note: the search for a split does not stop until at least one
+        valid partition of the node samples is found, even if it requires to
+        effectively inspect more than ``max_features`` features.
+
+    max_leaf_nodes : int, default=None
         Grow trees with ``max_leaf_nodes`` in best-first fashion.
         Best nodes are defined as relative reduction in impurity.
         If None then unlimited number of leaf nodes.
 
-    bootstrap : boolean, optional (default=True)
-        Whether bootstrap samples are used when building trees.
+    min_impurity_decrease : float, default=0.0
+        A node will be split if this split induces a decrease of the impurity
+        greater than or equal to this value.
+
+        The weighted impurity decrease equation is the following::
 
-    oob_score : bool, optional (default=False)
-        whether to use out-of-bag samples to estimate
-        the R^2 on unseen data.
-
-    n_jobs : integer, optional (default=1)
-        The number of jobs to run in parallel for both `fit` and `predict`.
-        If -1, then the number of jobs is set to the number of cores.
-
-    random_state : int, RandomState instance or None, optional (default=None)
-        If int, random_state is the seed used by the random number generator;
-        If RandomState instance, random_state is the random number generator;
-        If None, the random number generator is the RandomState instance used
-        by `np.random`.
+            N_t / N * (impurity - N_t_R / N_t * right_impurity
+                                - N_t_L / N_t * left_impurity)
 
-    verbose : int, optional (default=0)
-        Controls the verbosity of the tree building process.
+        where ``N`` is the total number of samples, ``N_t`` is the number of
+        samples at the current node, ``N_t_L`` is the number of samples in the
+        left child, and ``N_t_R`` is the number of samples in the right child.
+
+        ``N``, ``N_t``, ``N_t_R`` and ``N_t_L`` all refer to the weighted sum,
+        if ``sample_weight`` is passed.
+
+        .. versionadded:: 0.19
+
+    bootstrap : bool, default=True
+        Whether bootstrap samples are used when building trees. If False, the
+        whole dataset is used to build each tree.
 
-    warm_start : bool, optional (default=False)
+    oob_score : bool or callable, default=False
+        Whether to use out-of-bag samples to estimate the generalization score.
+        By default, :func:`~sklearn.metrics.r2_score` is used.
+        Provide a callable with signature `metric(y_true, y_pred)` to use a
+        custom metric. Only available if `bootstrap=True`.
+
+    n_jobs : int, default=None
+        The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
+        :meth:`decision_path` and :meth:`apply` are all parallelized over the
+        trees. ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
+        context. ``-1`` means using all processors. See :term:`Glossary
+        <n_jobs>` for more details.
+
+    random_state : int, RandomState instance or None, default=None
+        Controls both the randomness of the bootstrapping of the samples used
+        when building trees (if ``bootstrap=True``) and the sampling of the
+        features to consider when looking for the best split at each node
+        (if ``max_features < n_features``).
+        See :term:`Glossary <random_state>` for details.
+
+    verbose : int, default=0
+        Controls the verbosity when fitting and predicting.
+
+    warm_start : bool, default=False
         When set to ``True``, reuse the solution of the previous call to fit
         and add more estimators to the ensemble, otherwise, just fit a whole
-        new forest.
+        new forest. See :term:`Glossary <warm_start>` and
+        :ref:`gradient_boosting_warm_start` for details.
+
+    ccp_alpha : non-negative float, default=0.0
+        Complexity parameter used for Minimal Cost-Complexity Pruning. The
+        subtree with the largest cost complexity that is smaller than
+        ``ccp_alpha`` will be chosen. By default, no pruning is performed. See
+        :ref:`minimal_cost_complexity_pruning` for details.
+
+        .. versionadded:: 0.22
+
+    max_samples : int or float, default=None
+        If bootstrap is True, the number of samples to draw from X
+        to train each base estimator.
+
+        - If None (default), then draw `X.shape[0]` samples.
+        - If int, then draw `max_samples` samples.
+        - If float, then draw `max(round(n_samples * max_samples), 1)` samples. Thus,
+          `max_samples` should be in the interval `(0.0, 1.0]`.
+
+        .. versionadded:: 0.22
+
+    monotonic_cst : array-like of int of shape (n_features), default=None
+        Indicates the monotonicity constraint to enforce on each feature.
+          - 1: monotonically increasing
+          - 0: no constraint
+          - -1: monotonically decreasing
+
+        If monotonic_cst is None, no constraints are applied.
+
+        Monotonicity constraints are not supported for:
+          - multioutput regressions (i.e. when `n_outputs_ > 1`),
+          - regressions trained on data with missing values.
+
+        Read more in the :ref:`User Guide <monotonic_cst_gbdt>`.
+
+        .. versionadded:: 1.4
 
     Attributes
     ----------
+    estimator_ : :class:`~sklearn.tree.DecisionTreeRegressor`
+        The child estimator template used to create the collection of fitted
+        sub-estimators.
+
+        .. versionadded:: 1.2
+           `base_estimator_` was renamed to `estimator_`.
+
     estimators_ : list of DecisionTreeRegressor
         The collection of fitted sub-estimators.
 
-    feature_importances_ : array of shape = [n_features]
-        The feature importances (the higher, the more important the feature).
+    feature_importances_ : ndarray of shape (n_features,)
+        The impurity-based feature importances.
+        The higher, the more important the feature.
+        The importance of a feature is computed as the (normalized)
+        total reduction of the criterion brought by that feature.  It is also
+        known as the Gini importance.
+
+        Warning: impurity-based feature importances can be misleading for
+        high cardinality features (many unique values). See
+        :func:`sklearn.inspection.permutation_importance` as an alternative.
+
+    n_features_in_ : int
+        Number of features seen during :term:`fit`.
 
-    n_features_ : int
-        The number of features when ``fit`` is performed.
+        .. versionadded:: 0.24
+
+    feature_names_in_ : ndarray of shape (`n_features_in_`,)
+        Names of features seen during :term:`fit`. Defined only when `X`
+        has feature names that are all strings.
+
+        .. versionadded:: 1.0
 
     n_outputs_ : int
         The number of outputs when ``fit`` is performed.
 
     oob_score_ : float
         Score of the training dataset obtained using an out-of-bag estimate.
+        This attribute exists only when ``oob_score`` is True.
 
-    oob_prediction_ : array of shape = [n_samples]
+    oob_prediction_ : ndarray of shape (n_samples,) or (n_samples, n_outputs)
         Prediction computed with out-of-bag estimate on the training set.
+        This attribute exists only when ``oob_score`` is True.
+
+    estimators_samples_ : list of arrays
+        The subset of drawn samples (i.e., the in-bag samples) for each base
+        estimator. Each subset is defined by an array of the indices selected.
 
-    References
+        .. versionadded:: 1.4
+
+	References
     ----------
     .. [1] Nicolai Meinshausen, Quantile Regression Forests
         http://www.jmlr.org/papers/volume7/meinshausen06a/meinshausen06a.pdf
     """
-    def __init__(self,
-                 q=None,
-                 n_estimators=10,
-                 criterion='mse',
-                 max_depth=None,
-                 min_samples_split=2,
-                 min_samples_leaf=1,
-                 min_weight_fraction_leaf=0.0,
-                 max_features='auto',
-                 max_leaf_nodes=None,
-                 bootstrap=True,
-                 oob_score=False,
-                 n_jobs=1,
-                 random_state=None,
-                 verbose=0,
-                 warm_start=False):
-        super(BaseForestQuantileRegressor, self).__init__(
-            base_estimator=DecisionTreeRegressor(),
+    _parameter_constraints: dict = {
+        **ForestRegressor._parameter_constraints,
+        **DecisionTreeRegressor._parameter_constraints,
+    }
+    _parameter_constraints.pop("splitter")
+
+    def __init__(
+            self,
+            n_estimators=100,
+            q=None,
+            *,
+            criterion="squared_error",
+            max_depth=None,
+            min_samples_split=2,
+            min_samples_leaf=1,
+            min_weight_fraction_leaf=0.0,
+            max_features=1.0,
+            max_leaf_nodes=None,
+            min_impurity_decrease=0.0,
+            bootstrap=True,
+            oob_score=False,
+            n_jobs=None,
+            random_state=None,
+            verbose=0,
+            warm_start=False,
+            ccp_alpha=0.0,
+            max_samples=None,
+            monotonic_cst=None,
+    ):
+        super().__init__(
+            estimator=DecisionTreeRegressor(),
             n_estimators=n_estimators,
-            estimator_params=("criterion", "max_depth", "min_samples_split",
-                              "min_samples_leaf", "min_weight_fraction_leaf",
-                              "max_features", "max_leaf_nodes",
-                              "random_state"),
+            estimator_params=(
+                "criterion",
+                "max_depth",
+                "min_samples_split",
+                "min_samples_leaf",
+                "min_weight_fraction_leaf",
+                "max_features",
+                "max_leaf_nodes",
+                "min_impurity_decrease",
+                "random_state",
+                "ccp_alpha",
+                "monotonic_cst",
+            ),
             bootstrap=bootstrap,
             oob_score=oob_score,
             n_jobs=n_jobs,
             random_state=random_state,
             verbose=verbose,
-            warm_start=warm_start)
+            warm_start=warm_start,
+            max_samples=max_samples,
+        )
 
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
+        self.min_impurity_decrease = min_impurity_decrease
+        self.ccp_alpha = ccp_alpha
+        self.monotonic_cst = monotonic_cst
         self.q = q
 
 
 class ExtraTreesQuantileRegressor(ForestQuantileRegressor):
     """
     A extra trees regressor providing quantile estimates.
 
@@ -538,31 +671,30 @@
     n_estimators : int, default=100
         The number of trees in the forest.
 
         .. versionchanged:: 0.22
            The default value of ``n_estimators`` changed from 10 to 100
            in 0.22.
 
-    criterion : {"squared_error", "absolute_error"}, default="squared_error"
+    criterion : {"squared_error", "absolute_error", "friedman_mse", "poisson"}, \
+            default="squared_error"
         The function to measure the quality of a split. Supported criteria
         are "squared_error" for the mean squared error, which is equal to
-        variance reduction as feature selection criterion, and "absolute_error"
-        for the mean absolute error.
+        variance reduction as feature selection criterion and minimizes the L2
+        loss using the mean of each terminal node, "friedman_mse", which uses
+        mean squared error with Friedman's improvement score for potential
+        splits, "absolute_error" for the mean absolute error, which minimizes
+        the L1 loss using the median of each terminal node, and "poisson" which
+        uses reduction in Poisson deviance to find splits.
+        Training using "absolute_error" is significantly slower
+        than when using "squared_error".
 
         .. versionadded:: 0.18
            Mean Absolute Error (MAE) criterion.
 
-        .. deprecated:: 1.0
-            Criterion "mse" was deprecated in v1.0 and will be removed in
-            version 1.2. Use `criterion="squared_error"` which is equivalent.
-
-        .. deprecated:: 1.0
-            Criterion "mae" was deprecated in v1.0 and will be removed in
-            version 1.2. Use `criterion="absolute_error"` which is equivalent.
-
     max_depth : int, default=None
         The maximum depth of the tree. If None, then nodes are expanded until
         all leaves are pure or until all leaves contain less than
         min_samples_split samples.
 
     min_samples_split : int or float, default=2
         The minimum number of samples required to split an internal node:
@@ -596,32 +728,27 @@
         equal weight when sample_weight is not provided.
 
     max_features : {"sqrt", "log2", None}, int or float, default=1.0
         The number of features to consider when looking for the best split:
 
         - If int, then consider `max_features` features at each split.
         - If float, then `max_features` is a fraction and
-          `round(max_features * n_features)` features are considered at each
+          `max(1, int(max_features * n_features_in_))` features are considered at each
           split.
-        - If "auto", then `max_features=n_features`.
         - If "sqrt", then `max_features=sqrt(n_features)`.
         - If "log2", then `max_features=log2(n_features)`.
         - If None or 1.0, then `max_features=n_features`.
 
         .. note::
             The default of 1.0 is equivalent to bagged trees and more
             randomness can be achieved by setting smaller values, e.g. 0.3.
 
         .. versionchanged:: 1.1
             The default of `max_features` changed from `"auto"` to 1.0.
 
-        .. deprecated:: 1.1
-            The `"auto"` option was deprecated in 1.1 and will be removed
-            in 1.3.
-
         Note: the search for a split does not stop until at least one
         valid partition of the node samples is found, even if it requires to
         effectively inspect more than ``max_features`` features.
 
     max_leaf_nodes : int, default=None
         Grow trees with ``max_leaf_nodes`` in best-first fashion.
         Best nodes are defined as relative reduction in impurity.
@@ -645,17 +772,19 @@
 
         .. versionadded:: 0.19
 
     bootstrap : bool, default=False
         Whether bootstrap samples are used when building trees. If False, the
         whole dataset is used to build each tree.
 
-    oob_score : bool, default=False
+    oob_score : bool or callable, default=False
         Whether to use out-of-bag samples to estimate the generalization score.
-        Only available if bootstrap=True.
+        By default, :func:`~sklearn.metrics.r2_score` is used.
+        Provide a callable with signature `metric(y_true, y_pred)` to use a
+        custom metric. Only available if `bootstrap=True`.
 
     n_jobs : int, default=None
         The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
         :meth:`decision_path` and :meth:`apply` are all parallelized over the
         trees. ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
         context. ``-1`` means using all processors. See :term:`Glossary
         <n_jobs>` for more details.
@@ -673,15 +802,16 @@
 
     verbose : int, default=0
         Controls the verbosity when fitting and predicting.
 
     warm_start : bool, default=False
         When set to ``True``, reuse the solution of the previous call to fit
         and add more estimators to the ensemble, otherwise, just fit a whole
-        new forest. See :term:`the Glossary <warm_start>`.
+        new forest. See :term:`Glossary <warm_start>` and
+        :ref:`gradient_boosting_warm_start` for details.
 
     ccp_alpha : non-negative float, default=0.0
         Complexity parameter used for Minimal Cost-Complexity Pruning. The
         subtree with the largest cost complexity that is smaller than
         ``ccp_alpha`` will be chosen. By default, no pruning is performed. See
         :ref:`minimal_cost_complexity_pruning` for details.
 
@@ -694,41 +824,53 @@
         - If None (default), then draw `X.shape[0]` samples.
         - If int, then draw `max_samples` samples.
         - If float, then draw `max_samples * X.shape[0]` samples. Thus,
           `max_samples` should be in the interval `(0.0, 1.0]`.
 
         .. versionadded:: 0.22
 
+    monotonic_cst : array-like of int of shape (n_features), default=None
+        Indicates the monotonicity constraint to enforce on each feature.
+          - 1: monotonically increasing
+          - 0: no constraint
+          - -1: monotonically decreasing
+
+        If monotonic_cst is None, no constraints are applied.
+
+        Monotonicity constraints are not supported for:
+          - multioutput regressions (i.e. when `n_outputs_ > 1`),
+          - regressions trained on data with missing values.
+
+        Read more in the :ref:`User Guide <monotonic_cst_gbdt>`.
+
+        .. versionadded:: 1.4
+
     Attributes
     ----------
-    base_estimator_ : ExtraTreeRegressor
+    estimator_ : :class:`~sklearn.tree.ExtraTreeRegressor`
         The child estimator template used to create the collection of fitted
         sub-estimators.
 
+        .. versionadded:: 1.2
+           `base_estimator_` was renamed to `estimator_`.
+
     estimators_ : list of DecisionTreeRegressor
         The collection of fitted sub-estimators.
 
     feature_importances_ : ndarray of shape (n_features,)
         The impurity-based feature importances.
         The higher, the more important the feature.
         The importance of a feature is computed as the (normalized)
         total reduction of the criterion brought by that feature.  It is also
         known as the Gini importance.
 
         Warning: impurity-based feature importances can be misleading for
         high cardinality features (many unique values). See
         :func:`sklearn.inspection.permutation_importance` as an alternative.
 
-    n_features_ : int
-        The number of features.
-
-        .. deprecated:: 1.0
-            Attribute `n_features_` was deprecated in version 1.0 and will be
-            removed in 1.2. Use `n_features_in_` instead.
-
     n_features_in_ : int
         Number of features seen during :term:`fit`.
 
         .. versionadded:: 0.24
 
     feature_names_in_ : ndarray of shape (`n_features_in_`,)
         Names of features seen during :term:`fit`. Defined only when `X`
@@ -743,82 +885,64 @@
         Score of the training dataset obtained using an out-of-bag estimate.
         This attribute exists only when ``oob_score`` is True.
 
     oob_prediction_ : ndarray of shape (n_samples,) or (n_samples, n_outputs)
         Prediction computed with out-of-bag estimate on the training set.
         This attribute exists only when ``oob_score`` is True.
 
-    See Also
-    --------
-    ExtraTreesClassifier : An extra-trees classifier with random splits.
-    RandomForestClassifier : A random forest classifier with optimal splits.
-    RandomForestRegressor : Ensemble regressor using trees with optimal splits.
-
-    Notes
-    -----
-    The default values for the parameters controlling the size of the trees
-    (e.g. ``max_depth``, ``min_samples_leaf``, etc.) lead to fully grown and
-    unpruned trees which can potentially be very large on some data sets. To
-    reduce memory consumption, the complexity and size of the trees should be
-    controlled by setting those parameter values.
-
-    References
-    ----------
-    .. [1] P. Geurts, D. Ernst., and L. Wehenkel, "Extremely randomized trees",
-           Machine Learning, 63(1), 3-42, 2006.
+    estimators_samples_ : list of arrays
+        The subset of drawn samples (i.e., the in-bag samples) for each base
+        estimator. Each subset is defined by an array of the indices selected.
 
-    Examples
-    --------
-    >>> from sklearn.datasets import load_diabetes
-    >>> from sklearn.model_selection import train_test_split
-    >>> from sklearn.ensemble import ExtraTreesRegressor
-    >>> X, y = load_diabetes(return_X_y=True)
-    >>> X_train, X_test, y_train, y_test = train_test_split(
-    ...     X, y, random_state=0)
-    >>> reg = ExtraTreesRegressor(n_estimators=100, random_state=0).fit(
-    ...    X_train, y_train)
-    >>> reg.score(X_test, y_test)
-    0.2727...
+        .. versionadded:: 1.4
     """
+    _parameter_constraints: dict = {
+        **ForestRegressor._parameter_constraints,
+        **DecisionTreeRegressor._parameter_constraints,
+    }
+    _parameter_constraints.pop("splitter")
+
     def __init__(
-        self,
-        n_estimators=100,
-        q=None,
-        *,
-        criterion="squared_error",
-        max_depth=None,
-        min_samples_split=2,
-        min_samples_leaf=1,
-        min_weight_fraction_leaf=0.0,
-        max_features=1.0,
-        max_leaf_nodes=None,
-        min_impurity_decrease=0.0,
-        bootstrap=False,
-        oob_score=False,
-        n_jobs=None,
-        random_state=None,
-        verbose=0,
-        warm_start=False,
-        ccp_alpha=0.0,
-        max_samples=None,
+            self,
+            n_estimators=100,
+            q=None,
+            *,
+            criterion="squared_error",
+            max_depth=None,
+            min_samples_split=2,
+            min_samples_leaf=1,
+            min_weight_fraction_leaf=0.0,
+            max_features=1.0,
+            max_leaf_nodes=None,
+            min_impurity_decrease=0.0,
+            bootstrap=False,
+            oob_score=False,
+            n_jobs=None,
+            random_state=None,
+            verbose=0,
+            warm_start=False,
+            ccp_alpha=0.0,
+            max_samples=None,
+            monotonic_cst=None,
     ):
         super().__init__(
-            base_estimator=ExtraTreeRegressor(),
+            estimator=ExtraTreeRegressor(),
             n_estimators=n_estimators,
             estimator_params=(
                 "criterion",
                 "max_depth",
                 "min_samples_split",
                 "min_samples_leaf",
                 "min_weight_fraction_leaf",
                 "max_features",
                 "max_leaf_nodes",
                 "min_impurity_decrease",
                 "random_state",
                 "ccp_alpha",
+                "monotonic_cst",
             ),
             bootstrap=bootstrap,
             oob_score=oob_score,
             n_jobs=n_jobs,
             random_state=random_state,
             verbose=verbose,
             warm_start=warm_start,
@@ -830,14 +954,15 @@
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
         self.min_impurity_decrease = min_impurity_decrease
         self.ccp_alpha = ccp_alpha
+        self.monotonic_cst = monotonic_cst
         self.q = q
 
 
 class SampleRandomForestQuantileRegressor(SampleForestQuantileRegressor):
     """
     An approximation random forest regressor providing quantile estimates.
 
@@ -846,159 +971,309 @@
     For mathematical accuracy use :func:`sklearn_quantile.RandomForestQuantileRegressor`.
 
     Parameters
     ----------
     q : float or array-like, optional
         Quantiles used for prediction (values ranging from 0 to 1)
 
-    n_estimators : integer, optional (default=10)
+    n_estimators : int, default=100
         The number of trees in the forest.
 
-    criterion : string, optional (default="mse")
+        .. versionchanged:: 0.22
+           The default value of ``n_estimators`` changed from 10 to 100
+           in 0.22.
+
+    criterion : {"squared_error", "absolute_error", "friedman_mse", "poisson"}, \
+            default="squared_error"
         The function to measure the quality of a split. Supported criteria
-        are "mse" for the mean squared error, which is equal to variance
-        reduction as feature selection criterion, and "mae" for the mean
-        absolute error.
+        are "squared_error" for the mean squared error, which is equal to
+        variance reduction as feature selection criterion and minimizes the L2
+        loss using the mean of each terminal node, "friedman_mse", which uses
+        mean squared error with Friedman's improvement score for potential
+        splits, "absolute_error" for the mean absolute error, which minimizes
+        the L1 loss using the median of each terminal node, and "poisson" which
+        uses reduction in Poisson deviance to find splits.
+        Training using "absolute_error" is significantly slower
+        than when using "squared_error".
+
         .. versionadded:: 0.18
            Mean Absolute Error (MAE) criterion.
 
-    max_features : int, float, string or None, optional (default="auto")
-        The number of features to consider when looking for the best split:
-        - If int, then consider `max_features` features at each split.
-        - If float, then `max_features` is a percentage and
-          `int(max_features * n_features)` features are considered at each
-          split.
-        - If "auto", then `max_features=n_features`.
-        - If "sqrt", then `max_features=sqrt(n_features)`.
-        - If "log2", then `max_features=log2(n_features)`.
-        - If None, then `max_features=n_features`.
-        Note: the search for a split does not stop until at least one
-        valid partition of the node samples is found, even if it requires to
-        effectively inspect more than ``max_features`` features.
+        .. versionadded:: 1.0
+           Poisson criterion.
 
-    max_depth : integer or None, optional (default=None)
+    max_depth : int, default=None
         The maximum depth of the tree. If None, then nodes are expanded until
         all leaves are pure or until all leaves contain less than
         min_samples_split samples.
 
-    min_samples_split : int, float, optional (default=2)
+    min_samples_split : int or float, default=2
         The minimum number of samples required to split an internal node:
+
         - If int, then consider `min_samples_split` as the minimum number.
-        - If float, then `min_samples_split` is a percentage and
+        - If float, then `min_samples_split` is a fraction and
           `ceil(min_samples_split * n_samples)` are the minimum
           number of samples for each split.
+
         .. versionchanged:: 0.18
-           Added float values for percentages.
+           Added float values for fractions.
+
+    min_samples_leaf : int or float, default=1
+        The minimum number of samples required to be at a leaf node.
+        A split point at any depth will only be considered if it leaves at
+        least ``min_samples_leaf`` training samples in each of the left and
+        right branches.  This may have the effect of smoothing the model,
+        especially in regression.
 
-    min_samples_leaf : int, float, optional (default=1)
-        The minimum number of samples required to be at a leaf node:
         - If int, then consider `min_samples_leaf` as the minimum number.
-        - If float, then `min_samples_leaf` is a percentage and
+        - If float, then `min_samples_leaf` is a fraction and
           `ceil(min_samples_leaf * n_samples)` are the minimum
           number of samples for each node.
+
         .. versionchanged:: 0.18
-           Added float values for percentages.
+           Added float values for fractions.
 
-    min_weight_fraction_leaf : float, optional (default=0.)
+    min_weight_fraction_leaf : float, default=0.0
         The minimum weighted fraction of the sum total of weights (of all
         the input samples) required to be at a leaf node. Samples have
         equal weight when sample_weight is not provided.
 
-    max_leaf_nodes : int or None, optional (default=None)
+    max_features : {"sqrt", "log2", None}, int or float, default=1.0
+        The number of features to consider when looking for the best split:
+
+        - If int, then consider `max_features` features at each split.
+        - If float, then `max_features` is a fraction and
+          `max(1, int(max_features * n_features_in_))` features are considered at each
+          split.
+        - If "sqrt", then `max_features=sqrt(n_features)`.
+        - If "log2", then `max_features=log2(n_features)`.
+        - If None or 1.0, then `max_features=n_features`.
+
+        .. note::
+            The default of 1.0 is equivalent to bagged trees and more
+            randomness can be achieved by setting smaller values, e.g. 0.3.
+
+        .. versionchanged:: 1.1
+            The default of `max_features` changed from `"auto"` to 1.0.
+
+        Note: the search for a split does not stop until at least one
+        valid partition of the node samples is found, even if it requires to
+        effectively inspect more than ``max_features`` features.
+
+    max_leaf_nodes : int, default=None
         Grow trees with ``max_leaf_nodes`` in best-first fashion.
         Best nodes are defined as relative reduction in impurity.
         If None then unlimited number of leaf nodes.
 
-    bootstrap : boolean, optional (default=True)
-        Whether bootstrap samples are used when building trees.
+    min_impurity_decrease : float, default=0.0
+        A node will be split if this split induces a decrease of the impurity
+        greater than or equal to this value.
+
+        The weighted impurity decrease equation is the following::
+
+            N_t / N * (impurity - N_t_R / N_t * right_impurity
+                                - N_t_L / N_t * left_impurity)
+
+        where ``N`` is the total number of samples, ``N_t`` is the number of
+        samples at the current node, ``N_t_L`` is the number of samples in the
+        left child, and ``N_t_R`` is the number of samples in the right child.
 
-    oob_score : bool, optional (default=False)
-        whether to use out-of-bag samples to estimate
-        the R^2 on unseen data.
-
-    n_jobs : integer, optional (default=1)
-        The number of jobs to run in parallel for both `fit` and `predict`.
-        If -1, then the number of jobs is set to the number of cores.
-
-    random_state : int, RandomState instance or None, optional (default=None)
-        If int, random_state is the seed used by the random number generator;
-        If RandomState instance, random_state is the random number generator;
-        If None, the random number generator is the RandomState instance used
-        by `np.random`.
+        ``N``, ``N_t``, ``N_t_R`` and ``N_t_L`` all refer to the weighted sum,
+        if ``sample_weight`` is passed.
 
-    verbose : int, optional (default=0)
-        Controls the verbosity of the tree building process.
+        .. versionadded:: 0.19
 
-    warm_start : bool, optional (default=False)
+    bootstrap : bool, default=True
+        Whether bootstrap samples are used when building trees. If False, the
+        whole dataset is used to build each tree.
+
+    oob_score : bool or callable, default=False
+        Whether to use out-of-bag samples to estimate the generalization score.
+        By default, :func:`~sklearn.metrics.r2_score` is used.
+        Provide a callable with signature `metric(y_true, y_pred)` to use a
+        custom metric. Only available if `bootstrap=True`.
+
+    n_jobs : int, default=None
+        The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
+        :meth:`decision_path` and :meth:`apply` are all parallelized over the
+        trees. ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
+        context. ``-1`` means using all processors. See :term:`Glossary
+        <n_jobs>` for more details.
+
+    random_state : int, RandomState instance or None, default=None
+        Controls both the randomness of the bootstrapping of the samples used
+        when building trees (if ``bootstrap=True``) and the sampling of the
+        features to consider when looking for the best split at each node
+        (if ``max_features < n_features``).
+        See :term:`Glossary <random_state>` for details.
+
+    verbose : int, default=0
+        Controls the verbosity when fitting and predicting.
+
+    warm_start : bool, default=False
         When set to ``True``, reuse the solution of the previous call to fit
         and add more estimators to the ensemble, otherwise, just fit a whole
-        new forest.
+        new forest. See :term:`Glossary <warm_start>` and
+        :ref:`gradient_boosting_warm_start` for details.
+
+    ccp_alpha : non-negative float, default=0.0
+        Complexity parameter used for Minimal Cost-Complexity Pruning. The
+        subtree with the largest cost complexity that is smaller than
+        ``ccp_alpha`` will be chosen. By default, no pruning is performed. See
+        :ref:`minimal_cost_complexity_pruning` for details.
+
+        .. versionadded:: 0.22
+
+    max_samples : int or float, default=None
+        If bootstrap is True, the number of samples to draw from X
+        to train each base estimator.
+
+        - If None (default), then draw `X.shape[0]` samples.
+        - If int, then draw `max_samples` samples.
+        - If float, then draw `max(round(n_samples * max_samples), 1)` samples. Thus,
+          `max_samples` should be in the interval `(0.0, 1.0]`.
+
+        .. versionadded:: 0.22
+
+    monotonic_cst : array-like of int of shape (n_features), default=None
+        Indicates the monotonicity constraint to enforce on each feature.
+          - 1: monotonically increasing
+          - 0: no constraint
+          - -1: monotonically decreasing
+
+        If monotonic_cst is None, no constraints are applied.
+
+        Monotonicity constraints are not supported for:
+          - multioutput regressions (i.e. when `n_outputs_ > 1`),
+          - regressions trained on data with missing values.
+
+        Read more in the :ref:`User Guide <monotonic_cst_gbdt>`.
+
+        .. versionadded:: 1.4
 
     Attributes
     ----------
+    estimator_ : :class:`~sklearn.tree.DecisionTreeRegressor`
+        The child estimator template used to create the collection of fitted
+        sub-estimators.
+
+        .. versionadded:: 1.2
+           `base_estimator_` was renamed to `estimator_`.
+
     estimators_ : list of DecisionTreeRegressor
         The collection of fitted sub-estimators.
 
-    feature_importances_ : array of shape = [n_features]
-        The feature importances (the higher, the more important the feature).
+    feature_importances_ : ndarray of shape (n_features,)
+        The impurity-based feature importances.
+        The higher, the more important the feature.
+        The importance of a feature is computed as the (normalized)
+        total reduction of the criterion brought by that feature.  It is also
+        known as the Gini importance.
+
+        Warning: impurity-based feature importances can be misleading for
+        high cardinality features (many unique values). See
+        :func:`sklearn.inspection.permutation_importance` as an alternative.
+
+    n_features_in_ : int
+        Number of features seen during :term:`fit`.
+
+        .. versionadded:: 0.24
+
+    feature_names_in_ : ndarray of shape (`n_features_in_`,)
+        Names of features seen during :term:`fit`. Defined only when `X`
+        has feature names that are all strings.
 
-    n_features_ : int
-        The number of features when ``fit`` is performed.
+        .. versionadded:: 1.0
 
     n_outputs_ : int
         The number of outputs when ``fit`` is performed.
 
     oob_score_ : float
         Score of the training dataset obtained using an out-of-bag estimate.
+        This attribute exists only when ``oob_score`` is True.
 
-    oob_prediction_ : array of shape = [n_samples]
+    oob_prediction_ : ndarray of shape (n_samples,) or (n_samples, n_outputs)
         Prediction computed with out-of-bag estimate on the training set.
+        This attribute exists only when ``oob_score`` is True.
+
+    estimators_samples_ : list of arrays
+        The subset of drawn samples (i.e., the in-bag samples) for each base
+        estimator. Each subset is defined by an array of the indices selected.
+
+        .. versionadded:: 1.4
 
-    References
+	References
     ----------
     .. [1] Nicolai Meinshausen, Quantile Regression Forests
         http://www.jmlr.org/papers/volume7/meinshausen06a/meinshausen06a.pdf
     """
-    def __init__(self,
-                 q=None,
-                 n_estimators=10,
-                 criterion='mse',
-                 max_depth=None,
-                 min_samples_split=2,
-                 min_samples_leaf=1,
-                 min_weight_fraction_leaf=0.0,
-                 max_features='auto',
-                 max_leaf_nodes=None,
-                 bootstrap=True,
-                 oob_score=False,
-                 n_jobs=1,
-                 random_state=None,
-                 verbose=0,
-                 warm_start=False):
-        super(BaseForestQuantileRegressor, self).__init__(
-            base_estimator=DecisionTreeRegressor(),
+    _parameter_constraints: dict = {
+        **ForestRegressor._parameter_constraints,
+        **DecisionTreeRegressor._parameter_constraints,
+    }
+    _parameter_constraints.pop("splitter")
+
+    def __init__(
+            self,
+            n_estimators=100,
+            q=None,
+            *,
+            criterion="squared_error",
+            max_depth=None,
+            min_samples_split=2,
+            min_samples_leaf=1,
+            min_weight_fraction_leaf=0.0,
+            max_features=1.0,
+            max_leaf_nodes=None,
+            min_impurity_decrease=0.0,
+            bootstrap=True,
+            oob_score=False,
+            n_jobs=None,
+            random_state=None,
+            verbose=0,
+            warm_start=False,
+            ccp_alpha=0.0,
+            max_samples=None,
+            monotonic_cst=None,
+    ):
+        super().__init__(
+            estimator=DecisionTreeRegressor(),
             n_estimators=n_estimators,
-            estimator_params=("criterion", "max_depth", "min_samples_split",
-                              "min_samples_leaf", "min_weight_fraction_leaf",
-                              "max_features", "max_leaf_nodes",
-                              "random_state"),
+            estimator_params=(
+                "criterion",
+                "max_depth",
+                "min_samples_split",
+                "min_samples_leaf",
+                "min_weight_fraction_leaf",
+                "max_features",
+                "max_leaf_nodes",
+                "min_impurity_decrease",
+                "random_state",
+                "ccp_alpha",
+                "monotonic_cst",
+            ),
             bootstrap=bootstrap,
             oob_score=oob_score,
             n_jobs=n_jobs,
             random_state=random_state,
             verbose=verbose,
-            warm_start=warm_start)
+            warm_start=warm_start,
+            max_samples=max_samples,
+        )
 
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
+        self.min_impurity_decrease = min_impurity_decrease
+        self.ccp_alpha = ccp_alpha
+        self.monotonic_cst = monotonic_cst
         self.q = q
 
 
 class SampleExtraTreesQuantileRegressor(SampleForestQuantileRegressor):
     """
     An approximation extra trees regressor providing quantile estimates.
 
@@ -1014,31 +1289,30 @@
     n_estimators : int, default=100
         The number of trees in the forest.
 
         .. versionchanged:: 0.22
            The default value of ``n_estimators`` changed from 10 to 100
            in 0.22.
 
-    criterion : {"squared_error", "absolute_error"}, default="squared_error"
+    criterion : {"squared_error", "absolute_error", "friedman_mse", "poisson"}, \
+            default="squared_error"
         The function to measure the quality of a split. Supported criteria
         are "squared_error" for the mean squared error, which is equal to
-        variance reduction as feature selection criterion, and "absolute_error"
-        for the mean absolute error.
+        variance reduction as feature selection criterion and minimizes the L2
+        loss using the mean of each terminal node, "friedman_mse", which uses
+        mean squared error with Friedman's improvement score for potential
+        splits, "absolute_error" for the mean absolute error, which minimizes
+        the L1 loss using the median of each terminal node, and "poisson" which
+        uses reduction in Poisson deviance to find splits.
+        Training using "absolute_error" is significantly slower
+        than when using "squared_error".
 
         .. versionadded:: 0.18
            Mean Absolute Error (MAE) criterion.
 
-        .. deprecated:: 1.0
-            Criterion "mse" was deprecated in v1.0 and will be removed in
-            version 1.2. Use `criterion="squared_error"` which is equivalent.
-
-        .. deprecated:: 1.0
-            Criterion "mae" was deprecated in v1.0 and will be removed in
-            version 1.2. Use `criterion="absolute_error"` which is equivalent.
-
     max_depth : int, default=None
         The maximum depth of the tree. If None, then nodes are expanded until
         all leaves are pure or until all leaves contain less than
         min_samples_split samples.
 
     min_samples_split : int or float, default=2
         The minimum number of samples required to split an internal node:
@@ -1072,32 +1346,27 @@
         equal weight when sample_weight is not provided.
 
     max_features : {"sqrt", "log2", None}, int or float, default=1.0
         The number of features to consider when looking for the best split:
 
         - If int, then consider `max_features` features at each split.
         - If float, then `max_features` is a fraction and
-          `round(max_features * n_features)` features are considered at each
+          `max(1, int(max_features * n_features_in_))` features are considered at each
           split.
-        - If "auto", then `max_features=n_features`.
         - If "sqrt", then `max_features=sqrt(n_features)`.
         - If "log2", then `max_features=log2(n_features)`.
         - If None or 1.0, then `max_features=n_features`.
 
         .. note::
             The default of 1.0 is equivalent to bagged trees and more
             randomness can be achieved by setting smaller values, e.g. 0.3.
 
         .. versionchanged:: 1.1
             The default of `max_features` changed from `"auto"` to 1.0.
 
-        .. deprecated:: 1.1
-            The `"auto"` option was deprecated in 1.1 and will be removed
-            in 1.3.
-
         Note: the search for a split does not stop until at least one
         valid partition of the node samples is found, even if it requires to
         effectively inspect more than ``max_features`` features.
 
     max_leaf_nodes : int, default=None
         Grow trees with ``max_leaf_nodes`` in best-first fashion.
         Best nodes are defined as relative reduction in impurity.
@@ -1121,17 +1390,19 @@
 
         .. versionadded:: 0.19
 
     bootstrap : bool, default=False
         Whether bootstrap samples are used when building trees. If False, the
         whole dataset is used to build each tree.
 
-    oob_score : bool, default=False
+    oob_score : bool or callable, default=False
         Whether to use out-of-bag samples to estimate the generalization score.
-        Only available if bootstrap=True.
+        By default, :func:`~sklearn.metrics.r2_score` is used.
+        Provide a callable with signature `metric(y_true, y_pred)` to use a
+        custom metric. Only available if `bootstrap=True`.
 
     n_jobs : int, default=None
         The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
         :meth:`decision_path` and :meth:`apply` are all parallelized over the
         trees. ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
         context. ``-1`` means using all processors. See :term:`Glossary
         <n_jobs>` for more details.
@@ -1149,15 +1420,16 @@
 
     verbose : int, default=0
         Controls the verbosity when fitting and predicting.
 
     warm_start : bool, default=False
         When set to ``True``, reuse the solution of the previous call to fit
         and add more estimators to the ensemble, otherwise, just fit a whole
-        new forest. See :term:`the Glossary <warm_start>`.
+        new forest. See :term:`Glossary <warm_start>` and
+        :ref:`gradient_boosting_warm_start` for details.
 
     ccp_alpha : non-negative float, default=0.0
         Complexity parameter used for Minimal Cost-Complexity Pruning. The
         subtree with the largest cost complexity that is smaller than
         ``ccp_alpha`` will be chosen. By default, no pruning is performed. See
         :ref:`minimal_cost_complexity_pruning` for details.
 
@@ -1170,41 +1442,53 @@
         - If None (default), then draw `X.shape[0]` samples.
         - If int, then draw `max_samples` samples.
         - If float, then draw `max_samples * X.shape[0]` samples. Thus,
           `max_samples` should be in the interval `(0.0, 1.0]`.
 
         .. versionadded:: 0.22
 
+    monotonic_cst : array-like of int of shape (n_features), default=None
+        Indicates the monotonicity constraint to enforce on each feature.
+          - 1: monotonically increasing
+          - 0: no constraint
+          - -1: monotonically decreasing
+
+        If monotonic_cst is None, no constraints are applied.
+
+        Monotonicity constraints are not supported for:
+          - multioutput regressions (i.e. when `n_outputs_ > 1`),
+          - regressions trained on data with missing values.
+
+        Read more in the :ref:`User Guide <monotonic_cst_gbdt>`.
+
+        .. versionadded:: 1.4
+
     Attributes
     ----------
-    base_estimator_ : ExtraTreeRegressor
+    estimator_ : :class:`~sklearn.tree.ExtraTreeRegressor`
         The child estimator template used to create the collection of fitted
         sub-estimators.
 
+        .. versionadded:: 1.2
+           `base_estimator_` was renamed to `estimator_`.
+
     estimators_ : list of DecisionTreeRegressor
         The collection of fitted sub-estimators.
 
     feature_importances_ : ndarray of shape (n_features,)
         The impurity-based feature importances.
         The higher, the more important the feature.
         The importance of a feature is computed as the (normalized)
         total reduction of the criterion brought by that feature.  It is also
         known as the Gini importance.
 
         Warning: impurity-based feature importances can be misleading for
         high cardinality features (many unique values). See
         :func:`sklearn.inspection.permutation_importance` as an alternative.
 
-    n_features_ : int
-        The number of features.
-
-        .. deprecated:: 1.0
-            Attribute `n_features_` was deprecated in version 1.0 and will be
-            removed in 1.2. Use `n_features_in_` instead.
-
     n_features_in_ : int
         Number of features seen during :term:`fit`.
 
         .. versionadded:: 0.24
 
     feature_names_in_ : ndarray of shape (`n_features_in_`,)
         Names of features seen during :term:`fit`. Defined only when `X`
@@ -1219,82 +1503,64 @@
         Score of the training dataset obtained using an out-of-bag estimate.
         This attribute exists only when ``oob_score`` is True.
 
     oob_prediction_ : ndarray of shape (n_samples,) or (n_samples, n_outputs)
         Prediction computed with out-of-bag estimate on the training set.
         This attribute exists only when ``oob_score`` is True.
 
-    See Also
-    --------
-    ExtraTreesClassifier : An extra-trees classifier with random splits.
-    RandomForestClassifier : A random forest classifier with optimal splits.
-    RandomForestRegressor : Ensemble regressor using trees with optimal splits.
-
-    Notes
-    -----
-    The default values for the parameters controlling the size of the trees
-    (e.g. ``max_depth``, ``min_samples_leaf``, etc.) lead to fully grown and
-    unpruned trees which can potentially be very large on some data sets. To
-    reduce memory consumption, the complexity and size of the trees should be
-    controlled by setting those parameter values.
+    estimators_samples_ : list of arrays
+        The subset of drawn samples (i.e., the in-bag samples) for each base
+        estimator. Each subset is defined by an array of the indices selected.
 
-    References
-    ----------
-    .. [1] P. Geurts, D. Ernst., and L. Wehenkel, "Extremely randomized trees",
-           Machine Learning, 63(1), 3-42, 2006.
-
-    Examples
-    --------
-    >>> from sklearn.datasets import load_diabetes
-    >>> from sklearn.model_selection import train_test_split
-    >>> from sklearn.ensemble import ExtraTreesRegressor
-    >>> X, y = load_diabetes(return_X_y=True)
-    >>> X_train, X_test, y_train, y_test = train_test_split(
-    ...     X, y, random_state=0)
-    >>> reg = ExtraTreesRegressor(n_estimators=100, random_state=0).fit(
-    ...    X_train, y_train)
-    >>> reg.score(X_test, y_test)
-    0.2727...
+        .. versionadded:: 1.4
     """
+    _parameter_constraints: dict = {
+        **ForestRegressor._parameter_constraints,
+        **DecisionTreeRegressor._parameter_constraints,
+    }
+    _parameter_constraints.pop("splitter")
+
     def __init__(
-        self,
-        n_estimators=100,
-        q=None,
-        *,
-        criterion="squared_error",
-        max_depth=None,
-        min_samples_split=2,
-        min_samples_leaf=1,
-        min_weight_fraction_leaf=0.0,
-        max_features=1.0,
-        max_leaf_nodes=None,
-        min_impurity_decrease=0.0,
-        bootstrap=False,
-        oob_score=False,
-        n_jobs=None,
-        random_state=None,
-        verbose=0,
-        warm_start=False,
-        ccp_alpha=0.0,
-        max_samples=None,
+            self,
+            n_estimators=100,
+            q=None,
+            *,
+            criterion="squared_error",
+            max_depth=None,
+            min_samples_split=2,
+            min_samples_leaf=1,
+            min_weight_fraction_leaf=0.0,
+            max_features=1.0,
+            max_leaf_nodes=None,
+            min_impurity_decrease=0.0,
+            bootstrap=False,
+            oob_score=False,
+            n_jobs=None,
+            random_state=None,
+            verbose=0,
+            warm_start=False,
+            ccp_alpha=0.0,
+            max_samples=None,
+            monotonic_cst=None,
     ):
         super().__init__(
-            base_estimator=ExtraTreeRegressor(),
+            estimator=ExtraTreeRegressor(),
             n_estimators=n_estimators,
             estimator_params=(
                 "criterion",
                 "max_depth",
                 "min_samples_split",
                 "min_samples_leaf",
                 "min_weight_fraction_leaf",
                 "max_features",
                 "max_leaf_nodes",
                 "min_impurity_decrease",
                 "random_state",
                 "ccp_alpha",
+                "monotonic_cst",
             ),
             bootstrap=bootstrap,
             oob_score=oob_score,
             n_jobs=n_jobs,
             random_state=random_state,
             verbose=verbose,
             warm_start=warm_start,
@@ -1306,8 +1572,9 @@
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
         self.min_impurity_decrease = min_impurity_decrease
         self.ccp_alpha = ccp_alpha
+        self.monotonic_cst = monotonic_cst
         self.q = q
```

### Comparing `sklearn_quantile-0.0.3/sklearn_quantile/neighbors/quantile.py` & `sklearn-quantile-0.0.30/sklearn_quantile/neighbors/quantile.py`

 * *Files identical despite different names*

### Comparing `sklearn_quantile-0.0.3/sklearn_quantile/utils/weighted_quantile.pxd` & `sklearn-quantile-0.0.30/sklearn_quantile/utils/weighted_quantile.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 cdef enum Interpolation:
     linear, lower, higher, midpoint, nearest
 
 cdef void _weighted_quantile_presorted_1D(float[:] a,
-                                          float[:] q,
-                                          float[:] weights,
-                                          float[:] quantiles,
-                                          Interpolation interpolation) nogil
+                                         float[:] q,
+                                         float[:] weights,
+                                         float[:] quantiles,
+                                         Interpolation interpolation) nogil
 
 cdef void _weighted_quantile_unchecked_1D(float[:] a,
-                                          float[:] q,
-                                          float[:] weights,
-                                          float[:] quantiles,
-                                          Interpolation interpolation) nogil
+                                         float[:] q,
+                                         float[:] weights,
+                                         float[:] quantiles,
+                                         Interpolation interpolation) nogil
```

### Comparing `sklearn_quantile-0.0.3/sklearn_quantile/utils/weighted_quantile.pyx` & `sklearn-quantile-0.0.30/sklearn_quantile/utils/weighted_quantile.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 # cython: cdivision=True
 # cython: boundscheck=False
 # cython: wraparound=False
-# distutils: language = c
+# distutils: language=c
 
-cimport numpy as np
+cimport numpy as cnp
 import numpy as np
 from numpy.lib.function_base import _quantile_is_valid
 from libc.math cimport isnan
-from libc.stdlib cimport malloc, free
+from libc.stdlib cimport malloc, free, calloc
 
 
 cdef extern from "stdlib.h":
-    ctypedef void const_void "const void"
     void qsort(void *base, int nmemb, int size,
-            int(*compar)(const_void *, const_void *)) nogil
+               int(*compar)(const void *, const void *)) nogil
 
 
 cdef struct IndexedElement:
-    np.ulong_t index
-    np.float32_t value
+    size_t index
+    float value
 
 
-cdef int _compare(const_void *a, const_void *b):
-    cdef np.float32_t v
-    if isnan((<IndexedElement*> a).value): return 1
-    if isnan((<IndexedElement*> b).value): return -1
-    v = (<IndexedElement*> a).value-(<IndexedElement*> b).value
-    if v < 0: return -1
-    if v >= 0: return 1
+cdef int _compare(const void *a, const void *b) noexcept nogil:
+    cdef float v
+    if isnan((<IndexedElement*> a).value) and isnan((<IndexedElement*> b).value): 
+        return 0
+    if isnan((<IndexedElement*> a).value): 
+        return 1
+    if isnan((<IndexedElement*> b).value): 
+        return -1
+    
+    v = (<IndexedElement*> a).value - (<IndexedElement*> b).value
+    if v < 0: 
+        return -1
+    if v >= 0: 
+        return 1
 
 
 cdef long[:] argsort(float[:] data) nogil:
     """source: https://github.com/jcrudy/cython-argsort/blob/master/cyargsort/argsort.pyx"""
-    cdef np.ulong_t i
-    cdef np.ulong_t n = data.shape[0]
-    cdef long[:] order
+    cdef:
+        unsigned long i
+        size_t n = data.shape[0]
+        long[:] order
 
     with gil:
         order = np.empty(n, dtype=np.int_)
 
     # Allocate index tracking array.
     cdef IndexedElement *order_struct = <IndexedElement *> malloc(n * sizeof(IndexedElement))
+    if order_struct == NULL:
+        raise MemoryError()
 
     # Copy data into index tracking array.
     for i in range(n):
         order_struct[i].index = i
         order_struct[i].value = data[i]
 
     # Sort index tracking array.
@@ -61,17 +70,16 @@
 
 
 cdef int _searchsorted1D(float[:] A, float x) nogil:
     """
     source: https://github.com/gesellkammer/numpyx/blob/master/numpyx.pyx
     """
     cdef:
-        int imin = 0
-        int imax = A.shape[0]
-        int imid
+        int imid, imin = 0, imax = A.shape[0]
+
     while imin < imax:
         imid = imin + ((imax - imin) / 2)
         if A[imid] < x:
             imin = imid + 1
         else:
             imax = imid
     return imin
@@ -82,20 +90,18 @@
                                           float[:] weights,
                                           float[:] quantiles,
                                           Interpolation interpolation) nogil:
     """
     Weighted quantile (1D) on presorted data. 
     Note: the weights data will be changed
     """
-    cdef long q_idx
-    cdef float weights_total, weights_cum, frac
-    cdef int i
-
-    cdef int n_samples = a.shape[0]
-    cdef int n_q = q.shape[0]
+    cdef:
+        unsigned long i
+        size_t q_idx, n_samples = a.shape[0], n_q = q.shape[0]
+        float weights_total, weights_cum, frac
 
     weights_total = 0
     for i in range(n_samples):
         weights_total += weights[i]
 
     weights_cum = weights[0]
     weights[0] = 0.5 * weights[0] / weights_total
@@ -127,28 +133,26 @@
                 else:
                     frac = 1
 
             quantiles[i] = a[q_idx] + frac * (a[q_idx + 1] - a[q_idx])
 
 
 cdef void _weighted_quantile_unchecked_1D(float[:] a,
-                                          float[:] q,
-                                          float[:] weights,
-                                          float[:] quantiles,
-                                          Interpolation interpolation) nogil:
+                                         float[:] q,
+                                         float[:] weights,
+                                         float[:] quantiles,
+                                         Interpolation interpolation) nogil:
     """
     Weighted quantile (1D)
     Note: the data is not guaranteed to not be changed within this function
     """
-    cdef long[:] sort_idx
-    cdef int n_samples = a.shape[0]
-    cdef long count_samples = 0
-    cdef float[:] a_processed
-    cdef float[:] weights_processed
-    cdef int i
+    cdef:
+        long[:] sort_idx
+        size_t i, count_samples = 0, n_samples = a.shape[0]
+        float[:] a_processed, weights_processed
 
     for i in range(n_samples):
         if isnan(a[i]):
             continue
         elif weights[i] == 0:
             continue
         else:
@@ -166,15 +170,17 @@
         a_processed[i] = a[sort_idx[i]]
         weights_processed[i] = weights[sort_idx[i]]
 
     _weighted_quantile_presorted_1D(a_processed[:count_samples], q, weights_processed[:count_samples],
                                     quantiles, interpolation)
 
 
-def _weighted_quantile_unchecked(a, q, weights, axis, overwrite_input=False, interpolation='linear'):
+def _weighted_quantile_unchecked(a, q, weights, axis, 
+                                 overwrite_input=False, 
+                                 interpolation='linear'):
     """
     Numpy implementation
     Axis should not be none and a should have more than 1 dimension
     This implementation is faster than doing it manually in cython (as the
     looping currently happens with the GIL)
 
     Return shape (q, chosen axis, other axes)
@@ -280,15 +286,15 @@
     Returns
     -------
     quantile : scalar or ndarray
         If `q` is a single quantile and `axis=None`, then the result
         is a scalar. If multiple quantiles are given, first axis of
         the result corresponds to the quantiles. The other axes are
         the axes that remain after the reduction of `a`. The output
-        dtype is ``float64``.
+        dtype is ``float32``.
 
     References
     ----------
     1. https://en.wikipedia.org/wiki/Percentile#The_Weighted_Percentile_method
     """
     q = np.atleast_1d(q)
     if not _quantile_is_valid(q):
```

### Comparing `sklearn_quantile-0.0.3/sklearn_quantile.egg-info/SOURCES.txt` & `sklearn-quantile-0.0.30/sklearn_quantile.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.cfg
+pyproject.toml
 setup.py
 sklearn_quantile/__init__.py
 sklearn_quantile/base.py
 sklearn_quantile.egg-info/PKG-INFO
 sklearn_quantile.egg-info/SOURCES.txt
 sklearn_quantile.egg-info/dependency_links.txt
 sklearn_quantile.egg-info/requires.txt
 sklearn_quantile.egg-info/top_level.txt
 sklearn_quantile/ensemble/__init__.py
-sklearn_quantile/ensemble/maximum.c
 sklearn_quantile/ensemble/maximum.pyx
-sklearn_quantile/ensemble/quantile.c
 sklearn_quantile/ensemble/quantile.pyx
 sklearn_quantile/neighbors/__init__.py
 sklearn_quantile/neighbors/quantile.py
 sklearn_quantile/utils/__init__.py
-sklearn_quantile/utils/weighted_quantile.c
+sklearn_quantile/utils/utils.py
 sklearn_quantile/utils/weighted_quantile.pxd
 sklearn_quantile/utils/weighted_quantile.pyx
+tests/test_quantile_KNN.py
+tests/test_quantile_RF.py
 tests/test_weighted_quantile.py
```

### Comparing `sklearn_quantile-0.0.3/tests/test_weighted_quantile.py` & `sklearn-quantile-0.0.30/tests/test_weighted_quantile.py`

 * *Files identical despite different names*

