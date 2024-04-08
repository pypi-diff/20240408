# Comparing `tmp/jax-sysid-0.2.0.tar.gz` & `tmp/jax-sysid-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-sysid-0.2.0.tar", last modified: Wed Mar 27 09:32:18 2024, max compression
+gzip compressed data, was "jax-sysid-0.3.0.tar", last modified: Mon Apr  8 19:57:06 2024, max compression
```

## Comparing `jax-sysid-0.2.0.tar` & `jax-sysid-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-03-27 09:32:18.014183 jax-sysid-0.2.0/
--rw-r--r--   0 bemporad   (501) staff       (20)    11345 2024-03-01 16:55:21.000000 jax-sysid-0.2.0/LICENSE.txt
--rw-r--r--   0 bemporad   (501) staff       (20)    12952 2024-03-27 09:32:18.013921 jax-sysid-0.2.0/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)    12152 2024-03-07 06:02:39.000000 jax-sysid-0.2.0/README.md
--rw-r--r--   0 bemporad   (501) staff       (20)      801 2024-03-27 09:31:39.000000 jax-sysid-0.2.0/pyproject.toml
--rw-r--r--   0 bemporad   (501) staff       (20)       38 2024-03-27 09:32:18.014217 jax-sysid-0.2.0/setup.cfg
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-03-27 09:32:18.011522 jax-sysid-0.2.0/src/
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-03-27 09:32:18.012571 jax-sysid-0.2.0/src/jax_sysid/
--rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 jax-sysid-0.2.0/src/jax_sysid/__init__.py
--rw-r--r--   0 bemporad   (501) staff       (20)    64637 2024-03-27 09:28:55.000000 jax-sysid-0.2.0/src/jax_sysid/models.py
--rw-r--r--   0 bemporad   (501) staff       (20)     9022 2024-03-27 09:28:05.000000 jax-sysid-0.2.0/src/jax_sysid/utils.py
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-03-27 09:32:18.013701 jax-sysid-0.2.0/src/jax_sysid.egg-info/
--rw-r--r--   0 bemporad   (501) staff       (20)    12952 2024-03-27 09:32:18.000000 jax-sysid-0.2.0/src/jax_sysid.egg-info/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)      314 2024-03-27 09:32:18.000000 jax-sysid-0.2.0/src/jax_sysid.egg-info/SOURCES.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        1 2024-03-27 09:32:18.000000 jax-sysid-0.2.0/src/jax_sysid.egg-info/dependency_links.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       49 2024-03-27 09:32:18.000000 jax-sysid-0.2.0/src/jax_sysid.egg-info/requires.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       10 2024-03-27 09:32:18.000000 jax-sysid-0.2.0/src/jax_sysid.egg-info/top_level.txt
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-03-27 09:32:18.013247 jax-sysid-0.2.0/tests/
--rw-r--r--   0 bemporad   (501) staff       (20)     5280 2024-03-06 15:24:05.000000 jax-sysid-0.2.0/tests/test_models.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-08 19:57:06.639337 jax-sysid-0.3.0/
+-rw-r--r--   0 bemporad   (501) staff       (20)    11345 2024-03-01 16:55:21.000000 jax-sysid-0.3.0/LICENSE.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)    12952 2024-04-08 19:57:06.639076 jax-sysid-0.3.0/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)    12152 2024-03-07 06:02:39.000000 jax-sysid-0.3.0/README.md
+-rw-r--r--   0 bemporad   (501) staff       (20)      801 2024-04-08 17:15:36.000000 jax-sysid-0.3.0/pyproject.toml
+-rw-r--r--   0 bemporad   (501) staff       (20)       38 2024-04-08 19:57:06.639375 jax-sysid-0.3.0/setup.cfg
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-08 19:57:06.636824 jax-sysid-0.3.0/src/
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-08 19:57:06.637673 jax-sysid-0.3.0/src/jax_sysid/
+-rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 jax-sysid-0.3.0/src/jax_sysid/__init__.py
+-rw-r--r--   0 bemporad   (501) staff       (20)    65267 2024-04-08 19:54:18.000000 jax-sysid-0.3.0/src/jax_sysid/models.py
+-rw-r--r--   0 bemporad   (501) staff       (20)    10944 2024-04-08 19:54:26.000000 jax-sysid-0.3.0/src/jax_sysid/utils.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-08 19:57:06.638830 jax-sysid-0.3.0/src/jax_sysid.egg-info/
+-rw-r--r--   0 bemporad   (501) staff       (20)    12952 2024-04-08 19:57:06.000000 jax-sysid-0.3.0/src/jax_sysid.egg-info/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)      314 2024-04-08 19:57:06.000000 jax-sysid-0.3.0/src/jax_sysid.egg-info/SOURCES.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        1 2024-04-08 19:57:06.000000 jax-sysid-0.3.0/src/jax_sysid.egg-info/dependency_links.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       49 2024-04-08 19:57:06.000000 jax-sysid-0.3.0/src/jax_sysid.egg-info/requires.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       10 2024-04-08 19:57:06.000000 jax-sysid-0.3.0/src/jax_sysid.egg-info/top_level.txt
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-08 19:57:06.638604 jax-sysid-0.3.0/tests/
+-rw-r--r--   0 bemporad   (501) staff       (20)     5280 2024-03-06 15:24:05.000000 jax-sysid-0.3.0/tests/test_models.py
```

### Comparing `jax-sysid-0.2.0/LICENSE.txt` & `jax-sysid-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jax-sysid-0.2.0/PKG-INFO` & `jax-sysid-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sysid
-Version: 0.2.0
+Version: 0.3.0
 Summary: jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/jax-sysid
 Keywords: system identification,subspace identification,nonlinear regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jax-sysid-0.2.0/README.md` & `jax-sysid-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jax-sysid-0.2.0/pyproject.toml` & `jax-sysid-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jax-sysid"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax."
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["numpy","scipy","jax","jaxopt","flax","tqdm","matplotlib","pmlb"]
```

### Comparing `jax-sysid-0.2.0/src/jax_sysid/models.py` & `jax-sysid-0.3.0/src/jax_sysid/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,28 +235,30 @@
             Use state_fcn=None and output_fcn=None to get a linear model. 
         output_fcn : callable, optional
             Function handle to the output function y(k)=output_fcn(x(k),u(k),params).
             If not None, a state-update function "state_fcn" must be also provided. 
             Use state_fcn=None and output_fcn=None to get a linear model.
         y_in_x : bool, optional
             If True, the output is equal to the first ny states, i.e., y = [I 0]x.
-            This forces nx>=ny and feedthrough=False. The output function output_fcn is ignored.
+            This forces nx>=ny. The output function output_fcn is ignored.
         Ts : float, optional
             Sample time (default: 1 time unit).
         """
         self.nx = nx  # number of states
         self.ny = ny  # number of outputs
         self.nu = nu  # number of inputs
         self.y_in_x = y_in_x
         self.state_fcn = state_fcn  # state function
         self.output_fcn = output_fcn
 
         if y_in_x:
             self.nx = max(nx, ny)  # force nx>=ny
-            self.output_fcn = None  # ignore output function
+            def output_fcn(x, u, params): 
+                return x[0:ny]
+            self.output_fcn = output_fcn 
         self.isLinear = False  # By default, the model is nonlinear
         self.Ts = Ts  # sample time
 
         self.output_loss = None
         self.rho_x0 = None
         self.rho_th = None
         self.tau_th = None
@@ -304,22 +306,37 @@
             State trajectory (N-by-nx numpy array).
         """
         U = vec_reshape(U)
         x = x0.copy().reshape(-1)
         nx = self.nx
         N = U.shape[0]
         ny = self.ny
-        Y = np.empty((N, ny))
-        X = np.empty((N, nx))
-        for k in range(N):
-            u = U[k]
-            Y[k] = self.output_fcn(x, u, self.params) + \
-                qy * np.random.randn(ny)
-            X[k] = x
-            x = self.state_fcn(x, u, self.params) + qx * np.random.randn(nx)
+        
+        use_scan = (qx is None or qx == 0.) and (qy is None or qy == 0.)
+             
+        if not use_scan:
+            # simulate with noise in a for-loop
+            Y = np.empty((N, ny))
+            X = np.empty((N, nx))
+            for k in range(N):
+                u = U[k]
+                Y[k] = self.output_fcn(x, u, self.params) + \
+                    qy * np.random.randn(ny)
+                X[k] = x
+                x = self.state_fcn(x, u, self.params) + qx * np.random.randn(nx)
+        else:
+            @jax.jit
+            def model_step(x, u):
+                y = jnp.hstack((self.output_fcn(x, u, self.params),x))
+                x = self.state_fcn(x, u, self.params).reshape(-1)
+                return x, y
+            _, YX = jax.lax.scan(model_step, x0, U)
+            Y = YX[:,0:ny]
+            X = YX[:,ny:]
+
         return Y, X
 
     def loss(self, output_loss=None, rho_x0=0.001, rho_th=0.01, tau_th=0.0, tau_g=0.0, group_lasso_fcn=None, zero_coeff=0., xsat=1000., train_x0=True, custom_regularization=None):
         """Define the overall loss function for system identification
 
         Parameters
         ----------
@@ -1331,15 +1348,15 @@
         -------
         Y : ndarray
             Output signal.
         """
         U = vec_reshape(U)
         return self.output_fcn(U, self.params)
 
-    def loss(self, output_loss=None, rho_th=0.01, tau_th=0.0, tau_g=0.0, group_lasso_fcn=None, zero_coeff=0.e-4, custom_regularization=None):
+    def loss(self, output_loss=None, rho_th=0.01, tau_th=0.0, tau_g=0.0, group_lasso_fcn=None, zero_coeff=0., custom_regularization=None):
         """Define the overall loss function for training the model.
 
         Parameters
         ----------
         output_loss : function
             Loss function penalizing output fit errors, loss=output_loss(Yhat,Y), where Yhat is the sequence of predicted outputs and Y is the measured output.
             If None, use standard mean squared error loss=sum((Yhat-Y)^2)/Y.shape[0]
@@ -1599,15 +1616,16 @@
                         lb.append(0. * z[i]+epsil_lasso)
                     z, state = solver.run(z, bounds=(lb, np.inf))
                     z[0:nth] = [
                         z1 - z2 for (z1, z2) in zip(z[0:nth], z[nth:2 * nth])]
                     iter_num = state.iter_num
                     Jopt = state.fun_val
 
-                print('L-BFGS-B done in %d iterations.' % iter_num)
+                if self.iprint > -1:
+                    print('L-BFGS-B done in %d iterations.' % iter_num)
 
             else:
                 raise (Exception("\033[1mUnknown solver\033[0m"))
 
             t_solve = time.time() - t_solve
             return z[0:nth], Jopt, t_solve
```

### Comparing `jax-sysid-0.2.0/src/jax_sysid/utils.py` & `jax-sysid-0.3.0/src/jax_sysid/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -81,131 +81,181 @@
     Returns
     -------
     X : ndarray
         Unscaled array X = Xs/gain + offset
     """
     return Xs/gain+offset
 
+
 def vec_reshape(y):
     """Reshape an array to a 2D array if it is 1D.
-    
+
     (C) 2024 A. Bemporad
-    
+
     Parameters
     ----------
     y : ndarray
         Input array
 
     Returns:
     --------
     y : ndarray
         Possibly reshaped array
     """
     if len(y.shape) == 1:
         y = y.reshape(-1, 1)
-    return y                
+    return y
+
 
 def compute_scores(Y_train, Yhat_train, Y_test, Yhat_test, fit='R2'):
     """Compute R2-score, best fit rate, or accuracy score on (possibly multi-dimensional) 
        training and test output data
 
     (C) 2024 A. Bemporad
 
     Parameters
     ----------
-    Y_train : ndarray
+    Y_train : ndarray or None
         Reference output data for training, with shape (n_samples_training, n_outputs)
-    Yhat_train : ndarray
+    Yhat_train : ndarray or None
         Predicted output data for training, with shape (n_samples_training, n_outputs)
-    Y_test : ndarray
+    Y_test : ndarray or None
         Reference output data for testing, with shape (n_samples_test, n_outputs)
-    Yhat_test : ndarray
+    Yhat_test : ndarray or None
         Predicted output data for testing, with shape (n_samples_test, n_outputs)
     fit : str, optional
-        Metrics used: 'R2' (default), or 'BFR', or 'Accuracy'
+        Metrics used: 'R2' (default), or 'BFR', or 'RMSE', or 'Accuracy'
 
     Returns
     -------
     score_train: array
-        Score on training data (one entry per output)
+        Score on training data (one entry per output). If training data are not provided, a NaN is returned.
     score_test : array
-        Score on test data (one entry per output)
+        Score on test data (one entry per output). If test data are not provided, a NaN is returned.
     msg : string
         Printout summarizing computed performance results
         """
-        
-    Y_train = vec_reshape(Y_train)
-    Yhat_train = vec_reshape(Yhat_train)
-    Y_test = vec_reshape(Y_test)
-    Yhat_test = vec_reshape(Yhat_test)
-    
-    if Y_train.shape != Yhat_train.shape:
-        raise ValueError(
-            "Inconsistent dimensions between reference and predicted training output data.")
-    if Y_test.shape != Yhat_test.shape:
-        raise ValueError(
-            "Inconsistent dimensions between reference and predicted test output data.")
-    
-    ny = Y_train.shape[1]
+
+    use_training = Y_train is not None and Yhat_train is not None
+    use_test = Y_test is not None and Yhat_test is not None
+
+    if use_training:
+        Y_train = vec_reshape(Y_train)
+        Yhat_train = vec_reshape(Yhat_train)
+        if Y_train.shape != Yhat_train.shape:
+            raise ValueError(
+                "Inconsistent dimensions between reference and predicted training output data.")
+        ny = Y_train.shape[1]
+
+    if use_test:
+        Y_test = vec_reshape(Y_test)
+        Yhat_test = vec_reshape(Yhat_test)
+        if Y_test.shape != Yhat_test.shape:
+            raise ValueError(
+                "Inconsistent dimensions between reference and predicted test output data.")
+        # this could be a repetition of the previous assignment if use_training is True
+        ny = Y_test.shape[1]
+
     score_train = np.zeros(ny)
     score_test = np.zeros(ny)
     msg = ''
     isR2 = fit.lower() == 'r2'
     isBFR = fit.lower() == 'bfr'
+    isRMSE = fit.lower() == 'rmse'
     isAcc = fit.lower()[0:3] == 'acc'
-    if not (isR2 or isBFR or isAcc):
+    if not (isR2 or isBFR or isRMSE or isAcc):
         raise ValueError(
             "Invalid fit metric, only 'R2', 'BFR', and 'Accuracy' are supported.")
 
     if isAcc:
         unit = "%"
     else:
         unit = ""
 
     if ny > 1:
         for i in range(ny):
-            if isR2 or isBFR:
-                nY_train2 = np.sum((Y_train[:, i] - np.mean(Y_train[:, i]))**2)
-                nY_test2 = np.sum((Y_test[:, i] - np.mean(Y_test[:, i]))**2)
+            if isR2 or isBFR or isRMSE:
+                if use_training:
+                    nY_train2 = np.sum(
+                        (Y_train[:, i] - np.mean(Y_train[:, i]))**2)
+                if use_test:
+                    nY_test2 = np.sum(
+                        (Y_test[:, i] - np.mean(Y_test[:, i]))**2)
             text = f"y{i+1}: "
             if isR2:
-                score_train[i] = 100. * \
-                    (1. - np.sum((Yhat_train[:, i] -
-                     Y_train[:, i]) ** 2) / nY_train2)
-                score_test[i] = 100. * \
-                    (1. - np.sum((Yhat_test[:, i] -
-                     Y_test[:, i]) ** 2) / nY_test2)
+                if use_training:
+                    score_train[i] = 100. * \
+                        (1. - np.sum((Yhat_train[:, i] -
+                                      Y_train[:, i]) ** 2) / nY_train2)
+                if use_test:
+                    score_test[i] = 100. * \
+                        (1. - np.sum((Yhat_test[:, i] -
+                                      Y_test[:, i]) ** 2) / nY_test2)
             elif isBFR:
-                score_train[i] = 100. * (1. - np.linalg.norm(
-                    Yhat_train[:, i] - Y_train[:, i]) / np.sqrt(nY_train2))
-                score_test[i] = 100. * (1. - np.linalg.norm(
-                    Yhat_test[:, i] - Y_test[:, i]) / np.sqrt(nY_test2))
+                if use_training:
+                    score_train[i] = 100. * (1. - np.linalg.norm(
+                        Yhat_train[:, i] - Y_train[:, i]) / np.sqrt(nY_train2))
+                if use_test:
+                    score_test[i] = 100. * (1. - np.linalg.norm(
+                        Yhat_test[:, i] - Y_test[:, i]) / np.sqrt(nY_test2))
+            if isRMSE:
+                if use_training:
+                    score_train[i] = np.sqrt(nY_train2/Y_train.shape[0])
+                if use_test:
+                    score_test[i] = np.sqrt(nY_test2/Y_test.shape[0])
             elif isAcc:
-                score_train[i] = np.mean(Yhat_train[:, i] == Y_train[:, i])*100
-                score_test[i] = np.mean(Yhat_test[:, i] == Y_test[:, i])*100
+                if use_training:
+                    score_train[i] = np.mean(
+                        Yhat_train[:, i] == Y_train[:, i])*100
+                if use_test:
+                    score_test[i] = np.mean(
+                        Yhat_test[:, i] == Y_test[:, i])*100
+            if not use_training:
+                score_train[i] = np.nan
+            if not use_test:
+                score_test[i] = np.nan
+
             text += f"{fit.capitalize()} score: training = {score_train[i]: 5.4f}{unit}, test = {score_test[i]: 5.4f}{unit}"
             msg += '\n' + text
             # print(text)
         msg += "\n-----\nAverage "
     else:
-        nY_train2 = np.sum((Y_train-np.mean(Y_train))**2)
-        nY_test2 = np.sum((Y_test - np.mean(Y_test))**2)
+        if use_training:
+            nY_train2 = np.sum((Y_train-np.mean(Y_train))**2)
+        if use_test:
+            nY_test2 = np.sum((Y_test - np.mean(Y_test))**2)
         if isR2:
-            score_train = 100. * \
-                (1. - np.sum((Yhat_train - Y_train) ** 2) / nY_train2)
-            score_test = 100. * \
-                (1. - np.sum((Yhat_test - Y_test) ** 2) / nY_test2)
+            if use_training:
+                score_train = 100. * \
+                    (1. - np.sum((Yhat_train - Y_train) ** 2) / nY_train2)
+            if use_test:
+                score_test = 100. * \
+                    (1. - np.sum((Yhat_test - Y_test) ** 2) / nY_test2)
         elif isBFR:
-            score_train = 100. * \
-                (1. - np.linalg.norm(Yhat_train-Y_train) / np.sqrt(nY_train2))
-            score_test = 100. * (1. - np.linalg.norm(Yhat_test -
-                                                     Y_test) / np.sqrt(nY_test2))
+            if use_training:
+                score_train = 100. * \
+                    (1. - np.linalg.norm(Yhat_train-Y_train) / np.sqrt(nY_train2))
+            if use_test:
+                score_test = 100. * (1. - np.linalg.norm(Yhat_test -
+                                                         Y_test) / np.sqrt(nY_test2))
+        elif isRMSE:
+            if use_training:
+                score_train = np.sqrt(nY_train2/Y_train.shape[0])
+            if use_test:
+                score_test = np.sqrt(nY_test2/Y_test.shape[0])
         elif isAcc:
-            score_train = np.mean(Yhat_train == Y_train)*100
-            score_test = np.mean(Yhat_test == Y_test)*100
+            if use_training:
+                score_train = np.mean(Yhat_train == Y_train)*100
+            if use_test:
+                score_test = np.mean(Yhat_test == Y_test)*100
+        if not use_training:
+            score_train = np.nan
+        if not use_test:
+            score_test = np.nan
+
     msg += f"{fit.capitalize()} score:  training = {np.sum(score_train) / ny: 5.4f}{unit}, test = {np.sum(score_test) / ny: 5.4f}{unit}"
     return score_train, score_test, msg
 
 
 def print_eigs(A):
     """Print the eigenvalues of a given square matrix.
```

### Comparing `jax-sysid-0.2.0/src/jax_sysid.egg-info/PKG-INFO` & `jax-sysid-0.3.0/src/jax_sysid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sysid
-Version: 0.2.0
+Version: 0.3.0
 Summary: jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/jax-sysid
 Keywords: system identification,subspace identification,nonlinear regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jax-sysid-0.2.0/tests/test_models.py` & `jax-sysid-0.3.0/tests/test_models.py`

 * *Files identical despite different names*

