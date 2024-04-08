# Comparing `tmp/hidden-py-1.1.2.tar.gz` & `tmp/hidden-py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidden-py-1.1.2.tar", last modified: Fri Mar  1 20:18:30 2024, max compression
+gzip compressed data, was "hidden-py-1.2.0.tar", last modified: Mon Apr  8 19:15:53 2024, max compression
```

## Comparing `hidden-py-1.1.2.tar` & `hidden-py-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:18:30.039752 hidden-py-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-01 20:18:22.000000 hidden-py-1.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-03-01 20:18:30.039752 hidden-py-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-03-01 20:18:22.000000 hidden-py-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:18:30.035752 hidden-py-1.1.2/hidden_py/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8893 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/dynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:18:30.039752 hidden-py-1.1.2/hidden_py/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/filters/bayesian.py
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/infer.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/log_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:18:30.039752 hidden-py-1.1.2/hidden_py/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/optimize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/optimize/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    20675 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/optimize/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/optimize/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/optimize/results.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 20:18:22.000000 hidden-py-1.1.2/hidden_py/optimize/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:18:30.039752 hidden-py-1.1.2/hidden_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-03-01 20:18:29.000000 hidden-py-1.1.2/hidden_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-01 20:18:30.000000 hidden-py-1.1.2/hidden_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 20:18:29.000000 hidden-py-1.1.2/hidden_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-01 20:18:29.000000 hidden-py-1.1.2/hidden_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-01 20:18:29.000000 hidden-py-1.1.2/hidden_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 20:18:30.043752 hidden-py-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-01 20:18:22.000000 hidden-py-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:18:30.039752 hidden-py-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-03-01 20:18:22.000000 hidden-py-1.1.2/tests/test_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-03-01 20:18:22.000000 hidden-py-1.1.2/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-03-01 20:18:22.000000 hidden-py-1.1.2/tests/test_inferrence.py
--rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-03-01 20:18:22.000000 hidden-py-1.1.2/tests/test_optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:53.069743 hidden-py-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 19:15:43.000000 hidden-py-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-04-08 19:15:53.065743 hidden-py-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-08 19:15:43.000000 hidden-py-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:53.061743 hidden-py-1.2.0/hidden_py/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8893 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/dynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:53.065743 hidden-py-1.2.0/hidden_py/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/filters/bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14058 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/log_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:53.065743 hidden-py-1.2.0/hidden_py/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/optimize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/optimize/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/optimize/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/optimize/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/optimize/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:43.000000 hidden-py-1.2.0/hidden_py/optimize/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:53.065743 hidden-py-1.2.0/hidden_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-04-08 19:15:53.000000 hidden-py-1.2.0/hidden_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 19:15:53.000000 hidden-py-1.2.0/hidden_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:15:53.000000 hidden-py-1.2.0/hidden_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 19:15:53.000000 hidden-py-1.2.0/hidden_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 19:15:53.000000 hidden-py-1.2.0/hidden_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:15:53.069743 hidden-py-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 19:15:43.000000 hidden-py-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:53.065743 hidden-py-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-08 19:15:43.000000 hidden-py-1.2.0/tests/test_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-04-08 19:15:43.000000 hidden-py-1.2.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-08 19:15:43.000000 hidden-py-1.2.0/tests/test_inferrence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-04-08 19:15:43.000000 hidden-py-1.2.0/tests/test_optimizers.py
```

### Comparing `hidden-py-1.1.2/LICENSE.txt` & `hidden-py-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hidden-py-1.1.2/PKG-INFO` & `hidden-py-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidden-py
-Version: 1.1.2
+Version: 1.2.0
 Summary: A python package for discrete-output hidden Markov models
 Author: Steven Large
 Author-email: stevelarge7@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/StevenJLarge/hmm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `hidden-py-1.1.2/README.md` & `hidden-py-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hidden-py-1.1.2/hidden_py/dynamics.py` & `hidden-py-1.2.0/hidden_py/dynamics.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.1.2/hidden_py/filters/bayesian.py` & `hidden-py-1.2.0/hidden_py/filters/bayesian.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.1.2/hidden_py/infer.py` & `hidden-py-1.2.0/hidden_py/infer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # File to contain the class definitions and routines for inferring the
 # properties of the HMM
-from typing import Iterable, Optional, Dict
+from typing import Iterable, Optional, Dict, Union
 import sys
 from loguru import logger
 import numpy as np
 from pandas import DataFrame, Series
 from hidden_py.optimize.registry import OPTIMIZER_REGISTRY
 from hidden_py.optimize.base import OptClass
 from hidden_py.optimize.results import OptimizationResult
@@ -23,30 +23,45 @@
             dim_obs (int): Number of possible observations
         """
         # Tracker lists for forward and backward estimates
         self.forward_tracker = None
         self.backward_tracker = None
         self.predictions = None
         self.predictions_back = None
-        self.bayes_smooth = None
+        self.bayes_tracker = None
         self.alpha_tracker = None
         self.beta_tracker = None
 
         # Dimension of target system and observation vector
         self.n_sys = dim_sys
         self.n_obs = dim_obs
 
+        # Initial guesses for transition and observation matrices
+        self.trans_init = None
+        self.obs_init = None
+
         # Flag for if logging output is desired
         self.logging = logging
         if logging:
             logger.remove()
             logger.add(sys.stdout, colorize=True, format=log_fmt)
 
+    def __repr__(self) -> str:
+        return f"MarkovInfer(dim_sys={self.n_sys}, dim_obs={self.n_obs})"
+
+    def set_initial_matrices(self, trans_init: np.ndarray, obs_init: np.ndarray) -> None:
+        if trans_init.shape != (self.n_sys, self.n_sys):
+            raise ValueError("Transition matrix must be square...")
+        if obs_init.shape != (self.n_sys, self.n_obs):
+            raise ValueError("Observation matrix must have correct dimensions...")
+        self.trans_init = trans_init
+        self.obs_init = obs_init
+
     @staticmethod
-    def _validate_input(obs_ts: Iterable) -> np.ndarray:
+    def _validate_input_observations(obs_ts: Iterable) -> np.ndarray:
         """Routine to validate input for observation timeseries. This will cast
         lists, and pandas Series/DataFrme to a 1-d numpy array, for use in the
         lower-level (numba-optimized) filter routines
 
         Args:
             obs_ts (Iterable): timeseries of observations
 
@@ -74,109 +89,157 @@
                 raise ValueError("Input observations must be 1-D...")
 
         else:
             raise NotImplementedError(
                 "observation timeseries must be list or pandas Series/DataFrame"
             )
 
+    def _validate_optimizer_input_args(
+        self, opt_type: Union[OptClass, str]
+    ) -> OptClass:
+        """Routine to validate the inpuit argumetns passed into the optimizer
+
+        Args:
+            opt_type (Union[OptClass, str]): type of optimization, should be
+                one of the valid OptClass enum mebers or, the string value
+                corresponding to the name (case-insensitive)
+
+        Raises:
+            ValueError: If transition and observation matrices have not been
+                set prior to calling the optimizer, this error will get raised
+            ValueError: If the opt_type provided is not an explicit OptClass
+                enum member, and if the string value cannot be coerced to one
+                of the valid member names
+            Exception: Catchall for other errors, for instance if opt_type is
+                not an OptClass or a string
+
+        Returns:
+            OptClass: if everything is validated, this returns the opt_type as
+                the OptClass enum member
+        """
+        if self.trans_init is None or self.trans_init is None:
+            raise ValueError(
+                "Initial guesses for transition and observation matrices "
+                "must be set (using `set_init`) before optimization..."
+            )
+
+        if not isinstance(opt_type, OptClass):
+            try:
+                # TODO This is messy... swap 'ExpMax' --> 'Baumwelch'?
+                opt_type = opt_type.title().replace('Expmax', 'ExpMax')
+                opt_type = OptClass._member_map_[opt_type]
+            except KeyError:
+                raise ValueError(
+                    'Invalid `opt_class`, must be a member of OptClass enum...'
+                )
+            except Exception as ex:
+                raise Exception(f'Unknown error: {ex}')
+
+        return opt_type
+
     def forward_algo(
         self,
         observations: Iterable[int],
         trans_matrix: np.ndarray,
         obs_matrix: np.ndarray,
-    ) -> None:
+    ) -> np.ndarray:
         """Wrapper routine to implement the forward filter algorithm, and write
         results to internal forward_tracker and prediction_tracker variables
 
         Args:
             observations (Iterable[int]): observation timeseries
             trans_matrix (np.ndarray): transition matrix
             obs_matrix (np.ndarray): observation matrix
+
         """
-        observations = self._validate_input(observations)
+        observations = self._validate_input_observations(observations)
         self.forward_tracker, self.prediction_tracker = bayesian.forward_algo(
             observations, trans_matrix, obs_matrix
         )
+        return self.forward_tracker
 
     def backward_algo(
         self,
         observations: Iterable[int],
         trans_matrix: np.ndarray,
         obs_matrix: np.ndarray,
-    ) -> None:
+    ) -> np.ndarray:
         """Wrapper routine to implement the backward filter algorithm, and write
         results to internal backward_tracker and prediction_back variables
 
         Args:
             observations (Iterable[int]): observation timeseries
             trans_matrix (np.ndarray): transition matrix
             obs_matrix (np.ndarray): observation matrix
         """
-        observations = self._validate_input(observations)
+        observations = self._validate_input_observations(observations)
         self.backward_tracker, self.predictions_back = bayesian.backward_algo(
             observations, trans_matrix, obs_matrix
         )
+        return self.backward_tracker
 
     def alpha(
         self, observations: np.ndarray, trans_matrix: np.ndarray,
         obs_matrix: np.ndarray, norm: Optional[bool] = False
-    ) -> None:
+    ) -> np.ndarray:
         """Wrapper routine to interface with alpha-calcualtion routine. Sets to
         internal alpha_tracker instance variable
 
         Args:
             observations (np.ndarray): timeseries of observations
             trans_matrix (np.ndarray): transition matrix
             obs_matrix (np.ndarray): observation matrix
             norm (Optional[bool], optional): whether or not there we want to
                 use normalized (across states) at each point in time.
                 Defaults to False.
         """
-        observations = self._validate_input(observations)
+        observations = self._validate_input_observations(observations)
         self.alpha_tracker = bayesian.alpha_prob(
             observations, trans_matrix, obs_matrix, norm=norm
         )
+        return self.alpha_tracker
 
     def beta(
         self, observations: np.ndarray, trans_matrix: np.ndarray,
         obs_matrix: np.ndarray, norm: Optional[bool] = False
-    ) -> None:
+    ) -> np.ndarray:
         """Wrapper routine to interface with beta-calcualtion routine. Sets to
         internal beta_tracker instance variable
 
         Args:
             observations (np.ndarray): timeseries of observations
             trans_matrix (np.ndarray): transition matrix
             obs_matrix (np.ndarray): observation matrix
             norm (Optional[bool], optional): whether or not there we want to
                 use normalized (across states) at each point in time.
                 Defaults to False.
         """
-        observations = self._validate_input(observations)
+        observations = self._validate_input_observations(observations)
         self.beta_tracker = bayesian.beta_prob(
             observations, trans_matrix, obs_matrix, norm=norm
         )
+        return self.beta_tracker
 
-    def bayesian_smooth(
+    def bayesian_smoothing_algo(
         self, observations: np.ndarray, trans_matrix: np.ndarray,
         obs_matrix: np.ndarray
-    ) -> None:
+    ) -> np.ndarray:
         """Wrapper routine to interface with bayesian smoothing routine. Sets
         to internal bayes_smooth instance variable
 
         Args:
             observations (np.ndarray): timeseries of observations
             trans_matrix (np.ndarray): transition matrix
             obs_matrix (np.ndarray): observation matrix
         """
-        observations = self._validate_input(observations)
+        observations = self._validate_input_observations(observations)
         self.bayes_smooth = bayesian.bayes_estimate(
             observations, trans_matrix, obs_matrix
         )
-        return self.bayes_smooth
+        return self.bayes_tracker
 
     def discord(self, est_1: Iterable, est_2: Iterable) -> float:
         """Calculates the discord order parameter for an HMM based on the
         disagreement between two different estimates. This is the typical
         `discord` measure for HMMs when one of the estimates is `naive` (equal
         to observation)
 
@@ -200,17 +263,16 @@
 
         Returns:
             float: error rate of predictions
         """
         return 1 - np.mean([p == s for p, s in zip(pred_ts, state_ts)])
 
     def optimize(
-        self, observations: Iterable, trans_init: np.ndarray,
-        obs_init: np.ndarray, symmetric: bool = False,
-        opt_type: OptClass = OptClass.Local, algo_opts: Dict = {},
+        self, observations: Iterable, symmetric: bool = False,
+        opt_type: Union[OptClass, str] = OptClass.Local, algo_opts: Dict = {},
     ) -> OptimizationResult:
         """Main entrypoint for optimizing an internal model
 
         Args:
             observations (Iterable): Time series of observations
             trans_init (np.ndarray): Initial guess at transition rate matrix
             obs_init (np.ndarray): Initial guess at observation matrix
@@ -226,39 +288,53 @@
         Raises:
             ValueError: If the provided optimization class is not registerd, or
                 valid.
 
         Returns:
             OptimizationResult: Result of optimization
         """
-        if self.logging:
-            logger.info('Entering optimization...')
+        opt_type = self._validate_optimizer_input_args(opt_type)
+        observations = self._validate_input_observations(observations)
 
-        if not isinstance(opt_type, OptClass):
-            raise ValueError(
-                'Invalid `opt_class`, must be a member of OptClass enum...'
-            )
-        observations = self._validate_input(observations)
         # For the global optimizer, dim_tuple, but no initial guesses
+        dim_tuple = (self.trans_init.shape, self.obs_init.shape)
+
+        optimization_params = {
+            'dim_tuple': dim_tuple,
+            'symmetric': symmetric,
+            'trans_matrix': self.trans_init,
+            'obs_matrix': self.obs_init
+        }
+
+        if self.logging:
+            logger.info('Building optimizer...')
         optimizer = OPTIMIZER_REGISTRY[opt_type](**algo_opts)
-        if (opt_type is OptClass.Global):
-            if self.logging:
-                logger.info('Running global optimization')
-            dim_tuple = (trans_init.shape, obs_init.shape)
-            return optimizer.optimize(observations, dim_tuple, symmetric)
-
-        # For EM opt, there is no option to input a symmetric constraint
-        elif (opt_type is OptClass.ExpMax):
-            if self.logging:
-                logger.info("Running Baum-Welch (EM) optimization...")
-            return optimizer.optimize(observations, trans_init, obs_init)
 
         if self.logging:
-            logger.info("Running local partial-data likelihood optimization...")
-        return optimizer.optimize(observations, trans_init, obs_init, symmetric)
+            logger.info('Entering optimization...')
+        return optimizer.optimize(observations, **optimization_params)
+
+        # The line above should replace all of this, just need to make sure
+        # that all of the underlying optimizers support the same argumetns
+        # being passed in
+        # if (opt_type is OptClass.Global):
+        #     if self.logging:
+        #         logger.info('Running global optimization')
+        #     dim_tuple = (self.trans_init.shape, self.obs_init.shape)
+        #     return optimizer.optimize(observations, dim_tuple, symmetric)
+
+        # # For EM opt, there is no option to input a symmetric constraint
+        # elif (opt_type is OptClass.ExpMax):
+        #     if self.logging:
+        #         logger.info("Running Baum-Welch (EM) optimization...")
+        #     return optimizer.optimize(observations, self.trans_init, self.obs_init)
+
+        # if self.logging:
+        #     logger.info("Running local partial-data likelihood optimization...")
+        # return optimizer.optimize(observations, self.trans_init, self.obs_init, symmetric)
 
 
 if __name__ == "__main__":
     analyzer = MarkovInfer(3, 3, logging=True)
 
     # logger.info('Testing logs')
     # logger.debug('Testing logs debug')
```

### Comparing `hidden-py-1.1.2/hidden_py/optimize/base.py` & `hidden-py-1.2.0/hidden_py/optimize/base.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.1.2/hidden_py/optimize/optimization.py` & `hidden-py-1.2.0/hidden_py/optimize/optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         self.algo = algorithm
         super().__init__()
 
     def __repr__(self):
         return f"LocalLikelihoodOptimizer(algorithm={self.algo})"
 
     def optimize(
-        self, obs_ts: Iterable, A_guess: np.ndarray, B_guess: np.ndarray,
-        symmetric: Optional[bool] = False
+        self, obs_ts: Iterable, trans_matrix: np.ndarray,
+        obs_matrix: np.ndarray, symmetric: Optional[bool] = False, **kwargs
     ) -> LikelihoodOptimizationResult:
         """Routine to run actual optimization of the model. Passes off the
         objective function and encoded parameter array to a scipy optimizer
 
         Args:
             obs_ts (Iterable): integer sequence of observation values
             A_guess (np.ndarray): Initial guess at transition matrix
@@ -48,17 +48,21 @@
             LikelihoodOptimizationResult: Container object for model results
         """
         # Cast observations to numpy array if they are a list
         obs_ts = np.array(obs_ts)
 
         # Encode model parameters into parameter vector
         if symmetric:
-            param_init, dim_tuple = self._encode_parameters_symmetric(A_guess, B_guess)
+            param_init, dim_tuple = self._encode_parameters_symmetric(
+                trans_matrix, obs_matrix
+            )
         else:
-            param_init, dim_tuple = self._encode_parameters(A_guess, B_guess)
+            param_init, dim_tuple = self._encode_parameters(
+                trans_matrix, obs_matrix
+            )
 
         # Additional arguments to pass into optimizer
         opt_args = (dim_tuple, obs_ts, symmetric)
         # Parameter bounds in optimization
         bnds = self._build_optimization_bounds(len(param_init))
         if any(d > 2 for d in itertools.chain(*dim_tuple)):
             const = self._build_optimization_constraints(dim_tuple, symmetric)
@@ -124,15 +128,15 @@
             N_a //= 2
             N_b //= 2
 
         return N_a + N_b
 
     def optimize(
         self, obs_ts: Iterable, dim_tuple: Tuple,
-        symmetric: Optional[bool] = False
+        symmetric: Optional[bool] = False, **kwargs
     ) -> LikelihoodOptimizationResult:
         """Routine to run actual optimization of the model. Passes off the
         objective function and encoded parameter array to a scipy optimizer.
 
         This global optimizer uses the 'Simplical Homology Global Optimizer'
         `shgo` algorithm in the scipy library.
         See https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.shgo.html
@@ -420,15 +424,15 @@
             obs_ts, _bayes, self._laplace
         )
 
         return trans_matrix_updated, obs_matrix_updated
 
     def optimize(
         self, obs_ts: np.ndarray, trans_matrix: np.ndarray,
-        obs_matrix: np.ndarray
+        obs_matrix: np.ndarray, **kwargs
     ) -> EMOptimizationResult:
         """Main entrypoint for executing on Baum-Welch optimization procedure
         this routine will iterate updates to the input transition and
         observation matrices until EITHER the iteration limit is hit OR the
         maximum change to the A or B matrix during the previous step is below
         a threshold (both the threshold level and maximum iteration number)
         are specified in the constructor. Here, update size is quantified by a
@@ -474,16 +478,16 @@
             iter_count += 1
 
         meta_dict = {
             'max_iter': self._max_iter,
             'conv_threshold': self._opt_threshold
         }
         if self._track:
-            meta_dict["trans_tracker"]: trans_mat_tracker
-            meta_dict["obs_tracker"]: obs_mat_tracker
+            meta_dict["trans_tracker"] = trans_mat_tracker
+            meta_dict["obs_tracker"] = obs_mat_tracker
 
         return EMOptimizationResult(
             trans_matrix, obs_matrix, update_tracker, iter_count,
             metadata=meta_dict
         )
```

### Comparing `hidden-py-1.1.2/hidden_py/optimize/results.py` & `hidden-py-1.2.0/hidden_py/optimize/results.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.1.2/hidden_py.egg-info/PKG-INFO` & `hidden-py-1.2.0/hidden_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidden-py
-Version: 1.1.2
+Version: 1.2.0
 Summary: A python package for discrete-output hidden Markov models
 Author: Steven Large
 Author-email: stevelarge7@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/StevenJLarge/hmm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `hidden-py-1.1.2/hidden_py.egg-info/SOURCES.txt` & `hidden-py-1.2.0/hidden_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hidden-py-1.1.2/setup.py` & `hidden-py-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # README contents
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='hidden-py',
     packages=find_packages(),
-    version="1.1.2",
+    version="1.2.0",
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='''
         A python package for discrete-output hidden Markov models
     ''',
     author='Steven Large',
     author_email='stevelarge7@gmail.com',
```

### Comparing `hidden-py-1.1.2/tests/test_dynamics.py` & `hidden-py-1.2.0/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.1.2/tests/test_filters.py` & `hidden-py-1.2.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.1.2/tests/test_inferrence.py` & `hidden-py-1.2.0/tests/test_inferrence.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     [0, 1, 0, 1]
 ]
 
 sample_err = [1, 0, 0.5]
 sample_disc = [2, 0, 1]
 
 sym_test = [True, False]
-opt_type_test = OptClass._member_names_
+opt_type_test = OptClass._member_names_ + list(OptClass._member_map_.values())
 
 sample_obs = (
     np.array([0, 1, 2]), [0, 1, 2], pd.DataFrame([0, 1, 2]),
     pd.DataFrame({'0': 0, '1': 1, "2": 2}, index=[0]), pd.Series([1, 2, 3])
 )
 sample_obs_err = (
     np.ones((4, 2)), pd.DataFrame(np.ones((4, 2))), {'0': 0, '1': 1, '2': 2}
@@ -69,15 +69,15 @@
 
     # Assert
     assert BayesInfer.n_sys == 2
     assert BayesInfer.n_obs == 2
 
     assert BayesInfer.forward_tracker is None
     assert BayesInfer.backward_tracker is None
-    assert BayesInfer.bayes_smooth is None
+    assert BayesInfer.bayes_tracker is None
     assert BayesInfer.predictions is None
     assert BayesInfer.predictions_back is None
     assert BayesInfer.alpha_tracker is None
     assert BayesInfer.beta_tracker is None
 
 
 def test_forward_algorithm_tracking(test_hmm):
@@ -114,15 +114,15 @@
     # Arrange
     n_steps = 10
     BayesInfer = infer.MarkovInfer(2, 2)
 
     # Act
     test_hmm.run_dynamics(n_steps)
     obs_ts = test_hmm.obs_ts
-    BayesInfer.bayesian_smooth(obs_ts, test_hmm.A, test_hmm.B)
+    BayesInfer.bayesian_smoothing_algo(obs_ts, test_hmm.A, test_hmm.B)
 
     # Assert
     assert len(BayesInfer.bayes_smooth) == len(obs_ts)
 
 
 def test_alpha_algorithm_tracking(test_hmm):
     # Arrange
@@ -170,25 +170,25 @@
     assert discord_ == discord
 
 
 # Tests for input validation
 @pytest.mark.parametrize('obs_input', sample_obs)
 def test_input_observations_validation(obs_input):
     # Arrange / Act
-    obs = infer.MarkovInfer._validate_input(obs_input)
+    obs = infer.MarkovInfer._validate_input_observations(obs_input)
 
     # Assert
     assert isinstance(obs, np.ndarray)
 
 
 @pytest.mark.parametrize('obs_input', sample_obs_err)
 def test_invalid_input_observation_raises_in_validation(obs_input):
     # Arrange / Act / Assert
     with pytest.raises((ValueError, NotImplementedError)):
-        _ = infer.MarkovInfer._validate_input(obs_input)
+        _ = infer.MarkovInfer._validate_input_observations(obs_input)
 
 
 @pytest.mark.parametrize(
     'sample_data',
     [(i, j, k) for i, j, k in zip(sample_pred, sample_state, sample_err)]
 )
 def test_error_rate_calculation(sample_data):
@@ -202,40 +202,54 @@
     error_rate = BayesInfer.error_rate(pred_ts, state_ts)
 
     # Assert
     assert error_rate == err
 
 
 # Optimizations
-def check_optimizer_raises_for_invalid_class(test_hmm):
+def test_check_optimizer_raises_for_invalid_class(test_hmm):
     # Arrange
     BayesInfer = infer.MarkovInfer(2, 2)
     sample_obs = np.zeros(10)
+    BayesInfer.set_initial_matrices(test_hmm.A, test_hmm.B)
 
     # Act / Assert
     with pytest.raises(ValueError):
-        BayesInfer.optimize(
-            sample_obs, test_hmm.A, test_hmm.B, obs_type="INVALID"
-        )
+        BayesInfer.optimize(sample_obs, opt_type="INVALID",)
 
 
 @pytest.mark.parametrize(
-    ['sym', 'opt_type'], [itertools.product(sym_test, opt_type_test)]
+    'sym, opt_type', list(itertools.product(sym_test, opt_type_test))
 )
-def check_optimizer_runs_with_correct_return_type_for_valid_input(test_hmm, sym, opt_type):
+def test_check_optimizer_runs_with_correct_return_type_for_valid_input(
+    test_hmm, sym, opt_type
+):
     # Arrange
     n_steps = 100
     BayesInfer = infer.MarkovInfer(2, 2)
-
+    BayesInfer.set_initial_matrices(test_hmm.A, test_hmm.B)
+ 
     # Act
     test_hmm.run_dynamics(n_steps)
     obs_ts = test_hmm.obs_ts
-    opt_res = BayesInfer.optimize(
-        obs_ts, test_hmm.A, test_hmm.B, symmetric=sym, opt_type=opt_type
-    )
+    opt_res = BayesInfer.optimize(obs_ts, symmetric=sym, opt_type=opt_type)
 
     # Assert
     assert isinstance(opt_res, OptimizationResult)
 
 
+def test_optimizer_raises_when_matrices_are_not_initialized(test_hmm):
+    # Arange
+    n_steps = 100
+    BayesInfer = infer.MarkovInfer(2, 2)
+
+    # Act
+    test_hmm.run_dynamics(n_steps)
+    obs_ts = test_hmm.obs_ts
+
+    # Assert
+    with pytest.raises(ValueError):
+        _ = BayesInfer.optimize(obs_ts)
+
+
 if __name__ == "__main__":
     pytest.main([__file__])
```

### Comparing `hidden-py-1.1.2/tests/test_optimizers.py` & `hidden-py-1.2.0/tests/test_optimizers.py`

 * *Files identical despite different names*

