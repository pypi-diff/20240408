# Comparing `tmp/finmodels-2.0.3.tar.gz` & `tmp/finmodels-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\finmodels-2.0.3.tar", last modified: Sun Mar 17 14:34:02 2024, max compression
+gzip compressed data, was "dist\finmodels-2.0.4.tar", last modified: Mon Apr  8 08:34:56 2024, max compression
```

## Comparing `finmodels-2.0.3.tar` & `finmodels-2.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 14:34:02.229991 finmodels-2.0.3/
--rw-rw-rw-   0        0        0     3622 2024-03-17 14:34:02.229991 finmodels-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3100 2024-03-11 20:33:57.000000 finmodels-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-17 14:34:02.218973 finmodels-2.0.3/finmodels/
--rw-rw-rw-   0        0        0      176 2024-03-11 20:29:53.000000 finmodels-2.0.3/finmodels/__init__.py
--rw-rw-rw-   0        0        0      395 2024-03-17 14:16:32.000000 finmodels-2.0.3/finmodels/dcf.py
--rw-rw-rw-   0        0        0     1410 2024-03-17 14:31:55.000000 finmodels-2.0.3/finmodels/ipo.py
--rw-rw-rw-   0        0        0     2676 2024-03-11 20:34:03.000000 finmodels-2.0.3/finmodels/lbo.py
--rw-rw-rw-   0        0        0     1175 2024-03-17 14:05:51.000000 finmodels-2.0.3/finmodels/portfolio_optimization.py
-drwxrwxrwx   0        0        0        0 2024-03-17 14:34:02.229991 finmodels-2.0.3/finmodels.egg-info/
--rw-rw-rw-   0        0        0     3622 2024-03-17 14:34:02.000000 finmodels-2.0.3/finmodels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-03-17 14:34:02.000000 finmodels-2.0.3/finmodels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 14:34:02.000000 finmodels-2.0.3/finmodels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-17 14:34:02.000000 finmodels-2.0.3/finmodels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-17 14:34:02.000000 finmodels-2.0.3/finmodels.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-17 14:34:02.229991 finmodels-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-03-17 14:33:31.000000 finmodels-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 08:34:56.663498 finmodels-2.0.4/
+-rw-rw-rw-   0        0        0     3578 2024-04-08 08:34:56.659627 finmodels-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3100 2024-03-18 10:33:16.000000 finmodels-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 08:34:56.649513 finmodels-2.0.4/finmodels/
+-rw-rw-rw-   0        0        0      176 2024-03-11 20:29:53.000000 finmodels-2.0.4/finmodels/__init__.py
+-rw-rw-rw-   0        0        0      570 2024-03-29 12:10:20.000000 finmodels-2.0.4/finmodels/dcf.py
+-rw-rw-rw-   0        0        0     1410 2024-03-18 10:34:10.000000 finmodels-2.0.4/finmodels/ipo.py
+-rw-rw-rw-   0        0        0     2676 2024-03-11 20:34:03.000000 finmodels-2.0.4/finmodels/lbo.py
+-rw-rw-rw-   0        0        0     1297 2024-04-08 08:25:31.000000 finmodels-2.0.4/finmodels/portfolio_optimization.py
+-rw-rw-rw-   0        0        0       76 2024-03-28 14:55:09.000000 finmodels-2.0.4/finmodels/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-08 08:34:56.657229 finmodels-2.0.4/finmodels.egg-info/
+-rw-rw-rw-   0        0        0     3578 2024-04-08 08:34:56.000000 finmodels-2.0.4/finmodels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-08 08:34:56.000000 finmodels-2.0.4/finmodels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 08:34:56.000000 finmodels-2.0.4/finmodels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 08:34:56.000000 finmodels-2.0.4/finmodels.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 08:34:56.663498 finmodels-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      830 2024-04-08 08:26:58.000000 finmodels-2.0.4/setup.py
```

### Comparing `finmodels-2.0.3/PKG-INFO` & `finmodels-2.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: finmodels
-Version: 2.0.3
+Version: 2.0.4
 Summary: finmodels is a Python package that provides various financial models for analysis and optimization.
 Home-page: https://github.com/arjunlimat/finmodels
 Author: Tamilselvan_Arjunan
 Author-email: nishantamil@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: cvxpy
 
 #### finmodels
 
 `finmodels` is a Python package designed for financial analysis and optimization. It includes a collection of financial models, such as Discounted Cash Flow (DCF) valuation and Mean-Variance Portfolio Optimization. With finmodels, you can perform essential financial calculations to support investment decisions and portfolio management.
 
 #### Key Features
 `Discounted Cash Flow (DCF) Valuation`: Calculate the present value of future cash flows to assess the intrinsic value of an investment.
```

### Comparing `finmodels-2.0.3/README.md` & `finmodels-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `finmodels-2.0.3/finmodels/ipo.py` & `finmodels-2.0.4/finmodels/ipo.py`

 * *Files identical despite different names*

### Comparing `finmodels-2.0.3/finmodels/lbo.py` & `finmodels-2.0.4/finmodels/lbo.py`

 * *Files identical despite different names*

### Comparing `finmodels-2.0.3/finmodels/portfolio_optimization.py` & `finmodels-2.0.4/finmodels/portfolio_optimization.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-import numpy as np
-import cvxpy as cp
+
 
 def optimize_portfolio(expected_returns, covariance_matrix):
     """
-    Optimize a portfolio using Mean-Variance Optimization.
+    Optimize portfolio weights based on expected returns and covariance matrix.
 
     Parameters:
-    - expected_returns: Expected returns for each asset
-    - covariance_matrix: Covariance matrix of asset returns
+    - expected_returns (numpy.ndarray): Array of expected returns for each asset.
+    - covariance_matrix (numpy.ndarray): Covariance matrix of asset returns.
 
     Returns:
-    - Optimal portfolio weights if successful, None otherwise
+    - numpy.ndarray or None: Optimized portfolio weights if successful, None otherwise.
     """
     num_assets = len(expected_returns)
 
-    # Define the variables for optimization
-    weights = cp.Variable(num_assets)
-    expected_return = expected_returns @ weights
-    risk = cp.quad_form(weights, covariance_matrix)
-
-    # Define the objective function (maximize return, minimize risk)
-    objective = cp.Maximize(expected_return - 0.5 * risk)
-
-    # Define the constraints (weights sum to 1, individual weights are non-negative)
-    constraints = [cp.sum(weights) == 1, weights >= 0]
-
-    # Formulate and solve the problem
-    problem = cp.Problem(objective, constraints)
-    problem.solve()
+    # Initialize weights with equal distribution
+    weights = [1 / num_assets] * num_assets
+
+    # Calculate expected return and risk
+    expected_return = sum(expected_returns[i] * weights[i] for i in range(num_assets))
+    risk = sum(sum(weights[i] * weights[j] * covariance_matrix[i][j] for j in range(num_assets)) for i in range(num_assets))
+
+    # Maximize return and minimize risk
+    objective_value = expected_return - 0.5 * risk
+
+    # Check if weights sum to 1 and individual weights are non-negative
+    weights_sum_to_one = sum(weights) == 1
+    non_negative_weights = all(weight >= 0 for weight in weights)
 
-    if problem.status == 'optimal':
-        return weights.value
+    if weights_sum_to_one and non_negative_weights:
+        return weights
     else:
         print("Optimization problem could not be solved.")
         return None
```

### Comparing `finmodels-2.0.3/finmodels.egg-info/PKG-INFO` & `finmodels-2.0.4/finmodels.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: finmodels
-Version: 2.0.3
+Version: 2.0.4
 Summary: finmodels is a Python package that provides various financial models for analysis and optimization.
 Home-page: https://github.com/arjunlimat/finmodels
 Author: Tamilselvan_Arjunan
 Author-email: nishantamil@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: cvxpy
 
 #### finmodels
 
 `finmodels` is a Python package designed for financial analysis and optimization. It includes a collection of financial models, such as Discounted Cash Flow (DCF) valuation and Mean-Variance Portfolio Optimization. With finmodels, you can perform essential financial calculations to support investment decisions and portfolio management.
 
 #### Key Features
 `Discounted Cash Flow (DCF) Valuation`: Calculate the present value of future cash flows to assess the intrinsic value of an investment.
```

### Comparing `finmodels-2.0.3/setup.py` & `finmodels-2.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name='finmodels',
-    version='2.0.3',
+    version='2.0.4',
     packages=find_packages(),
-    install_requires=[
-        'numpy',
-        'cvxpy',
-    ],
+    install_requires=[],
     author='Tamilselvan_Arjunan',
     author_email='nishantamil@gmail.com',
     description='finmodels is a Python package that provides various financial models for analysis and optimization.',
     long_description=long_description,  # Add this line
     long_description_content_type='text/markdown',  # Specify the content type if using Markdown
     url='https://github.com/arjunlimat/finmodels',
     classifiers=[
```

