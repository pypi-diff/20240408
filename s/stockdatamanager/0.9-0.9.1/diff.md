# Comparing `tmp/stockdatamanager-0.9.tar.gz` & `tmp/stockdatamanager-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockdatamanager-0.9.tar", last modified: Sat Apr  6 20:47:38 2024, max compression
+gzip compressed data, was "stockdatamanager-0.9.1.tar", last modified: Sat Apr  6 21:02:47 2024, max compression
```

## Comparing `stockdatamanager-0.9.tar` & `stockdatamanager-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:38.853747 stockdatamanager-0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 20:46:47.000000 stockdatamanager-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-06 20:47:38.853747 stockdatamanager-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-06 20:46:47.000000 stockdatamanager-0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:47:38.853747 stockdatamanager-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-06 20:46:47.000000 stockdatamanager-0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:38.849748 stockdatamanager-0.9/stockdatamanager/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/ToDo.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/customerrors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/datafetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)    56671 2024-04-06 20:46:47.000000 stockdatamanager-0.9/stockdatamanager/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:38.853747 stockdatamanager-0.9/stockdatamanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-06 20:47:38.000000 stockdatamanager-0.9/stockdatamanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 20:47:38.000000 stockdatamanager-0.9/stockdatamanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:47:38.000000 stockdatamanager-0.9/stockdatamanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-06 20:47:38.000000 stockdatamanager-0.9/stockdatamanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 20:47:38.000000 stockdatamanager-0.9/stockdatamanager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:38.853747 stockdatamanager-0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-06 20:46:47.000000 stockdatamanager-0.9/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:02:47.630648 stockdatamanager-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 21:02:03.000000 stockdatamanager-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-06 21:02:47.630648 stockdatamanager-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-06 21:02:03.000000 stockdatamanager-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 21:02:47.630648 stockdatamanager-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-06 21:02:03.000000 stockdatamanager-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:02:47.630648 stockdatamanager-0.9.1/stockdatamanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-06 21:02:03.000000 stockdatamanager-0.9.1/stockdatamanager/ToDo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-06 21:02:03.000000 stockdatamanager-0.9.1/stockdatamanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-06 21:02:03.000000 stockdatamanager-0.9.1/stockdatamanager/customerrors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-04-06 21:02:03.000000 stockdatamanager-0.9.1/stockdatamanager/datafetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-04-06 21:02:03.000000 stockdatamanager-0.9.1/stockdatamanager/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56671 2024-04-06 21:02:03.000000 stockdatamanager-0.9.1/stockdatamanager/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:02:47.630648 stockdatamanager-0.9.1/stockdatamanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-06 21:02:47.000000 stockdatamanager-0.9.1/stockdatamanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 21:02:47.000000 stockdatamanager-0.9.1/stockdatamanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 21:02:47.000000 stockdatamanager-0.9.1/stockdatamanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-06 21:02:47.000000 stockdatamanager-0.9.1/stockdatamanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 21:02:47.000000 stockdatamanager-0.9.1/stockdatamanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:02:47.630648 stockdatamanager-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-06 21:02:03.000000 stockdatamanager-0.9.1/tests/test.py
```

### Comparing `stockdatamanager-0.9/LICENSE` & `stockdatamanager-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stockdatamanager-0.9/PKG-INFO` & `stockdatamanager-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdatamanager
-Version: 0.9
+Version: 0.9.1
 Summary: A comprehensive library for financial analysis
 Home-page: https://github.com/GiorgioMB/stockdatafetcher/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stockdatamanager-0.9/README.md` & `stockdatamanager-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `stockdatamanager-0.9/setup.py` & `stockdatamanager-0.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module sets up the package for distribution."""
 from setuptools import setup, find_packages
 
 setup(
     name='stockdatamanager',
-    version='0.9',
+    version='0.9.1',
     packages=find_packages(),
     description='A comprehensive library for financial analysis',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Giorgio Micaletto',
     author_email='giorgio.micaletto@studbocconi.it',
     url='https://github.com/GiorgioMB/stockdatafetcher/',
```

### Comparing `stockdatamanager-0.9/stockdatamanager/datafetcher.py` & `stockdatamanager-0.9.1/stockdatamanager/datafetcher.py`

 * *Files identical despite different names*

### Comparing `stockdatamanager-0.9/stockdatamanager/indicators.py` & `stockdatamanager-0.9.1/stockdatamanager/indicators.py`

 * *Files identical despite different names*

### Comparing `stockdatamanager-0.9/stockdatamanager/options.py` & `stockdatamanager-0.9.1/stockdatamanager/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -957,342 +957,342 @@
                     self.dividend_yield,
                     self.sigma,
                     self.is_call,
                     self.american)
     return option.price()
 
   def trinom_american(self, N: int = 100, pd_: float = 0, pu: float = 0) -> float:
-    Option = Option(self.S,
+    option = Option(self.S,
                     self.K,
                     self.risk_free_rate,
                     self.T,
                     N,
                     pu,
                     pd_,
                     self.dividend_yield,
                     self.sigma,
                     self.is_call,
                     self.american)
-    u = np.exp(Option.sigma * np.sqrt(2 * Option.dt))
+    u = np.exp(option.sigma * np.sqrt(2 * option.dt))
     d = 1 / u
     m = 1
-    qu = ((np.exp((Option.r - Option.div) * Option.dt / 2) - np.exp(-Option.sigma * np.sqrt(Option.dt / 2))) / (np.exp(Option.sigma * np.sqrt(Option.dt / 2)) - np.exp(-Option.sigma * np.sqrt(Option.dt / 2)))) ** 2
-    qd = ((np.exp(Option.sigma * np.sqrt(Option.dt / 2)) - np.exp((Option.r - Option.div) * Option.dt / 2)) / (np.exp(Option.sigma * np.sqrt(Option.dt / 2)) - np.exp(-Option.sigma * np.sqrt(Option.dt / 2)))) ** 2
+    qu = ((np.exp((option.r - option.div) * option.dt / 2) - np.exp(-option.sigma * np.sqrt(option.dt / 2))) / (np.exp(option.sigma * np.sqrt(option.dt / 2)) - np.exp(-option.sigma * np.sqrt(option.dt / 2)))) ** 2
+    qd = ((np.exp(option.sigma * np.sqrt(option.dt / 2)) - np.exp((option.r - option.div) * option.dt / 2)) / (np.exp(option.sigma * np.sqrt(option.dt / 2)) - np.exp(-option.sigma * np.sqrt(option.dt / 2)))) ** 2
     qm = 1 - qu - qd
     def init_stock_price_tree():
-      Option.STs = [np.array([Option.S])]
+      option.STs = [np.array([option.S])]
       for i in range(N):
-        prev_branches = Option.STs[-1]
+        prev_branches = option.STs[-1]
         st = np.concatenate((prev_branches * u, [prev_branches[-1]* m, prev_branches[-1]* d]))
-        Option.STs.append(st)
+        option.STs.append(st)
     def init_payoffs_tree():
       if self.is_call:
-        return np.maximum(0, Option.STs - Option.K)
+        return np.maximum(0, option.STs - option.K)
       else:
-        return np.maximum(0, Option.K - Option.STs)
+        return np.maximum(0, option.K - option.STs)
     def check_early(payoffs, node):
       if self.is_call:
         return np.maximum(payoffs, self.STs[node] - self.K)
       else:
         return np.maximum(payoffs, self.K - self.STs[node])
     def traverse_tree(payoffs):
       for i in reversed(range(N)):
-        payoffs = check_early((payoffs[:-2] * qu + payoffs[1:-1] * qm + payoffs[2:] * qd) * Option.df, i)
+        payoffs = check_early((payoffs[:-2] * qu + payoffs[1:-1] * qm + payoffs[2:] * qd) * option.df, i)
       return payoffs
     def begin_tree_traversal():
       payoffs = init_payoffs_tree()
       return traverse_tree(payoffs)
     init_stock_price_tree()
     payoff = begin_tree_traversal()
     return payoff[0]
 
   def trinom_european(self, N: int = 100, pd_: float = 0, pu: float = 0) -> float:
-    Option = Option(self.S,
+    option = Option(self.S,
                     self.K,
                     self.risk_free_rate,
                     self.T,
                     N,
                     pu,
                     pd_,
                     self.dividend_yield,
                     self.sigma,
                     self.is_call,
                     self.american)
-    u = np.exp(Option.sigma * np.sqrt(2 * Option.dt))
+    u = np.exp(option.sigma * np.sqrt(2 * option.dt))
     d = 1 / u
     m = 1
-    qu = ((np.exp((Option.r - Option.div) * Option.dt / 2) - np.exp(-Option.sigma * np.sqrt(Option.dt / 2))) / (np.exp(Option.sigma * np.sqrt(Option.dt / 2)) - np.exp(-Option.sigma * np.sqrt(Option.dt / 2)))) ** 2
-    qd = ((np.exp(Option.sigma * np.sqrt(Option.dt / 2)) - np.exp((Option.r - Option.div) * Option.dt / 2)) / (np.exp(Option.sigma * np.sqrt(Option.dt / 2)) - np.exp(-Option.sigma * np.sqrt(Option.dt / 2)))) ** 2
+    qu = ((np.exp((option.r - option.div) * option.dt / 2) - np.exp(-option.sigma * np.sqrt(option.dt / 2))) / (np.exp(option.sigma * np.sqrt(option.dt / 2)) - np.exp(-option.sigma * np.sqrt(option.dt / 2)))) ** 2
+    qd = ((np.exp(option.sigma * np.sqrt(option.dt / 2)) - np.exp((option.r - option.div) * option.dt / 2)) / (np.exp(option.sigma * np.sqrt(option.dt / 2)) - np.exp(-option.sigma * np.sqrt(option.dt / 2)))) ** 2
     qm = 1 - qu - qd
     def init_stock_price_tree():
-      Option.STs = [np.array([Option.S])]
+      option.STs = [np.array([option.S])]
       for i in range(N):
-        prev_branches = Option.STs[-1]
+        prev_branches = option.STs[-1]
         st = np.concatenate((prev_branches * u, [prev_branches[-1]* m, prev_branches[-1]* d]))
-        Option.STs.append(st)
+        option.STs.append(st)
     def init_payoffs_tree():
       if self.is_call:
-        return np.maximum(0, Option.STs - Option.K)
+        return np.maximum(0, option.STs - option.K)
       else:
-        return np.maximum(0, Option.K - Option.STs)
+        return np.maximum(0, option.K - option.STs)
     def traverse_tree(payoffs):
       for i in reversed(range(N)):
-        payoffs = (payoffs[:-2] * qu + payoffs[1:-1] * qm + payoffs[2:] * qd) * Option.df
+        payoffs = (payoffs[:-2] * qu + payoffs[1:-1] * qm + payoffs[2:] * qd) * option.df
       return payoffs
     def begin_tree_traversal():
       payoffs = init_payoffs_tree()
       return traverse_tree(payoffs)
     init_stock_price_tree()
     payoff = begin_tree_traversal()
     return payoff[0]
     
   def us_lr_tree(self, N: int = 1000, pd_: float = 0, pu: float = 0) -> float:
-    Option = Option(self.S,
+    option = Option(self.S,
                     self.K,
                     self.risk_free_rate,
                     self.T,
                     N,
                     pu,
                     pd_,
                     self.dividend_yield,
                     self.sigma,
                     self.is_call,
                     self.american)
     odd_N = N if N % 2 == 1 else N + 1
     def pp_2_inversion(z, n):
         return .5 + math.copysign(1, z) * math.sqrt(.25 - .25 * math.exp( -((z / (n + 1 / 3+ .1 / (n + 1))) ** 2.) * (n + 1/6)))
-    d1 = (np.log(Option.S / Option.K) + ((Option.r - Option.div) + (Option.sigma ** 2) / 2) * Option.T) / (Option.sigma * np.sqrt(Option.T))
-    d2 = (np.log(Option.S / Option.K) + ((Option.r - Option.div) - (Option.sigma ** 2) / 2) * Option.T) / (Option.sigma * np.sqrt(Option.T))
+    d1 = (np.log(option.S / option.K) + ((option.r - option.div) + (option.sigma ** 2) / 2) * option.T) / (option.sigma * np.sqrt(option.T))
+    d2 = (np.log(option.S / option.K) + ((option.r - option.div) - (option.sigma ** 2) / 2) * option.T) / (option.sigma * np.sqrt(option.T))
     pbar = pp_2_inversion(d1, odd_N)
     p = pp_2_inversion(d2, odd_N)
-    u = 1 / Option.df * pbar / p
-    d = (1/Option.df - p * u) / (1 - p)
+    u = 1 / option.df * pbar / p
+    d = (1/option.df - p * u) / (1 - p)
     qu = p
     qd = 1 - p
     def init_stock_price_tree():
-      Option.STs = [np.array([Option.S])]
+      option.STs = [np.array([option.S])]
       for i in range(N):
-        prev_branches = Option.STs[-1]
+        prev_branches = option.STs[-1]
         st = np.concatenate((prev_branches * u, [prev_branches[-1]* d]))
-        Option.STs.append(st)
+        option.STs.append(st)
     def init_payoffs_tree():
       if self.is_call:
-        return np.maximum(0, Option.STs - Option.K)
+        return np.maximum(0, option.STs - option.K)
       else:
-        return np.maximum(0, Option.K - Option.STs)
+        return np.maximum(0, option.K - option.STs)
     def check_early(payoffs, node):
       if self.is_call:
         return np.maximum(payoffs, self.STs[node] - self.K)
       else:
         return np.maximum(payoffs, self.K - self.STs[node])
     def traverse_tree(payoffs):
       for i in reversed(range(N)):
-        payoffs = check_early((payoffs[:-1] * qu + payoffs[1:] * qd) * Option.df, i)
+        payoffs = check_early((payoffs[:-1] * qu + payoffs[1:] * qd) * option.df, i)
       return payoffs
     def begin_tree_traversal():
       payoffs = init_payoffs_tree()
       return traverse_tree(payoffs)
     init_stock_price_tree()
     payoff = begin_tree_traversal()
     return payoff[0]
 
   def european_lr_tree(self, N: int = 1000, pd_: float = 0, pu: float = 0) -> float:
-    Option = Option(self.S,
+    option = Option(self.S,
                     self.K,
                     self.risk_free_rate,
                     self.T,
                     N,
                     pu,
                     pd_,
                     self.dividend_yield,
                     self.sigma,
                     self.is_call,
                     self.american)
     odd_N = N if N % 2 == 1 else N + 1
     def pp_2_inversion(z, n):
         return .5 + math.copysign(1, z) * math.sqrt(.25 - .25 * math.exp( -((z / (n + 1 / 3+ .1 / (n + 1))) ** 2.) * (n + 1/6)))
-    d1 = (np.log(Option.S / Option.K) + ((Option.r - Option.div) + (Option.sigma ** 2) / 2) * Option.T) / (Option.sigma * np.sqrt(Option.T))
-    d2 = (np.log(Option.S / Option.K) + ((Option.r - Option.div) - (Option.sigma ** 2) / 2) * Option.T) / (Option.sigma * np.sqrt(Option.T))
+    d1 = (np.log(option.S / option.K) + ((option.r - option.div) + (option.sigma ** 2) / 2) * option.T) / (option.sigma * np.sqrt(option.T))
+    d2 = (np.log(option.S / option.K) + ((option.r - option.div) - (option.sigma ** 2) / 2) * option.T) / (option.sigma * np.sqrt(option.T))
     pbar = pp_2_inversion(d1, odd_N)
     p = pp_2_inversion(d2, odd_N)
-    u = 1 / Option.df * pbar / p
-    d = (1/Option.df - p * u) / (1 - p)
+    u = 1 / option.df * pbar / p
+    d = (1/option.df - p * u) / (1 - p)
     qu = p
     qd = 1 - p
     def init_stock_price_tree():
-      Option.STs = np.zeros(M)
+      option.STs = np.zeros(M)
       for i in range(M):
-        Option.STs[i] = self.S * (u ** (N - i)) * (d ** i)
+        option.STs[i] = self.S * (u ** (N - i)) * (d ** i)
     def init_payoffs_tree():
       if self.is_call:
-        return np.maximum(0, Option.STs - Option.K)
+        return np.maximum(0, option.STs - option.K)
       else:
-        return np.maximum(0, Option.K - Option.STs)
+        return np.maximum(0, option.K - option.STs)
     def traverse_tree(payoffs):
       for i in range(N):
-        payoffs = (payoffs[:-1] * qu + payoffs[1:] * qd) * Option.df
+        payoffs = (payoffs[:-1] * qu + payoffs[1:] * qd) * option.df
       return payoffs
     def begin_tree_traversal():
       payoffs = init_payoffs_tree()
       return traverse_tree(payoffs)
     init_stock_price_tree()
     payoff = begin_tree_traversal()
     return payoff[0]
 
   def eu_cox_ross_rubinstein(self, N: int = 1000, pd_: float = 0, pu: float = 0) -> float:
-    Option = Option(self.S,
+    option = Option(self.S,
                     self.K,
                     self.risk_free_rate,
                     self.T,
                     N,
                     pu,
                     pd_,
                     self.dividend_yield,
                     self.sigma,
                     self.is_call,
                     self.american)
-    u = math.exp(Option.sigma * math.sqrt(Option.dt))
+    u = math.exp(option.sigma * math.sqrt(option.dt))
     d = 1 / u
-    qu = (math.exp(Option.r - Option.div) - d) / (u - d)
+    qu = (math.exp(option.r - option.div) - d) / (u - d)
     qd = 1 - qu
     def init_stock_price_tree():
-      Option.STs = np.zeros(M)
+      option.STs = np.zeros(M)
       for i in range(M):
-        Option.STs[i] = self.S * (u ** (N - i)) * (d ** i)
+        option.STs[i] = self.S * (u ** (N - i)) * (d ** i)
     def init_payoffs_tree():
       if self.is_call:
-        return np.maximum(0, Option.STs - Option.K)
+        return np.maximum(0, option.STs - option.K)
       else:
-        return np.maximum(0, Option.K - Option.STs)
+        return np.maximum(0, option.K - option.STs)
     def traverse_tree(payoffs):
       for i in range(N):
-        payoffs = (payoffs[:-1] * qu + payoffs[1:] * qd) * Option.df
+        payoffs = (payoffs[:-1] * qu + payoffs[1:] * qd) * option.df
       return payoffs
     def begin_tree_traversal():
       payoffs = init_payoffs_tree()
       return traverse_tree(payoffs)
     init_stock_price_tree()
     payoff = begin_tree_traversal()
     return payoff[0]
 
   def us_cox_ross_rubinstein(self, N: int = 1000, pd_: float = 0, pu: float = 0) -> float:
-    Option = Option(self.S,
+    option = Option(self.S,
                     self.K,
                     self.risk_free_rate,
                     self.T,
                     N,
                     pu,
                     pd_,
                     self.dividend_yield,
                     self.sigma,
                     self.is_call,
                     self.american)
-    u = math.exp(Option.sigma * math.sqrt(Option.dt))
+    u = math.exp(option.sigma * math.sqrt(option.dt))
     d = 1 / u
-    qu = (math.exp(Option.r - Option.div) - d) / (u - d)
+    qu = (math.exp(option.r - option.div) - d) / (u - d)
     qd = 1 - qu
     def init_stock_price_tree():
-      Option.STs = [np.array([Option.S])]
+      option.STs = [np.array([option.S])]
       for i in range(N):
-        prev_branches = Option.STs[-1]
+        prev_branches = option.STs[-1]
         st = np.concatenate((prev_branches * u, [prev_branches[-1]* d]))
-        Option.STs.append(st)
+        option.STs.append(st)
     def init_payoffs_tree():
       if self.is_call:
-        return np.maximum(0, Option.STs - Option.K)
+        return np.maximum(0, option.STs - option.K)
       else:
-        return np.maximum(0, Option.K - Option.STs)
+        return np.maximum(0, option.K - option.STs)
     def check_early(payoffs, node):
       if self.is_call:
         return np.maximum(payoffs, self.STs[node] - self.K)
       else:
         return np.maximum(payoffs, self.K - self.STs[node])
     def traverse_tree(payoffs):
       for i in reversed(range(N)):
-        payoffs = check_early((payoffs[:-1] * qu + payoffs[1:] * qd) * Option.df, i)
+        payoffs = check_early((payoffs[:-1] * qu + payoffs[1:] * qd) * option.df, i)
       return payoffs
     def begin_tree_traversal():
       payoffs = init_payoffs_tree()
       return traverse_tree(payoffs)
     init_stock_price_tree()
     payoff = begin_tree_traversal()
     return payoff[0]
 
   def binom_american(self, N: int = 1000, pd_: float = 0, pu: float = 0) -> float:
-    Option = Option(self.S,
+    option = Option(self.S,
                     self.K,
                     self.risk_free_rate,
                     self.T,
                     N,
                     pu,
                     pd_,
                     self.dividend_yield,
                     self.sigma,
                     self.is_call,
                     self.american)
     u = 1 + pu
     d = 1 - pd_
-    qu = (math.exp(Option.r - Option.div) * Option.dt) - d / (u - d)
+    qu = (math.exp(option.r - option.div) * option.dt) - d / (u - d)
     qd = 1 - qu
     def init_stock_price_tree():
-      Option.STs = [np.array([Option.S])]
+      option.STs = [np.array([option.S])]
       for i in range(N):
-        prev_branches = Option.STs[-1]
+        prev_branches = option.STs[-1]
         st = np.concatenate((prev_branches * u, [prev_branches[-1]* d]))
-        Option.STs.append(st)
+        option.STs.append(st)
     def init_payoffs_tree():
       if self.is_call:
-        return np.maximum(0, Option.STs - Option.K)
+        return np.maximum(0, option.STs - option.K)
       else:
-        return np.maximum(0, Option.K - Option.STs)
+        return np.maximum(0, option.K - option.STs)
     def check_early(payoffs, node):
       if self.is_call:
         return np.maximum(payoffs, self.STs[node] - self.K)
       else:
         return np.maximum(payoffs, self.K - self.STs[node])
     def traverse_tree(payoffs):
       for i in reversed(range(N)):
-        payoffs = check_early((payoffs[:-1] * qu + payoffs[1:] * qd) * Option.df, i)
+        payoffs = check_early((payoffs[:-1] * qu + payoffs[1:] * qd) * option.df, i)
       return payoffs
     def begin_tree_traversal():
       payoffs = init_payoffs_tree()
       return traverse_tree(payoffs)
     init_stock_price_tree()
     payoff = begin_tree_traversal()
     return payoff[0]
   
   def binom_european(self, N: int = 1000, pd_: float = 0, pu: float = 0) -> float:
-    Option = Option(self.S, 
+    option = Option(self.S, 
                     self.K, 
                     self.risk_free_rate, 
                     self.T, 
                     N, 
                     pu, 
                     pd_, 
                     self.dividend_yield, 
                     self.sigma, 
                     self.is_call, 
                     self.american)
     M = N + 1
     u = 1 + pu
     d = 1 - pd_
-    qu =(math.exp(Option.r - Option.div) * Option.dt) - d / (u - d)
+    qu =(math.exp(option.r - option.div) * option.dt) - d / (u - d)
     qd = 1 - qu
     def init_stock_price_tree():
-      Option.STs = np.zeros(M)
+      option.STs = np.zeros(M)
       for i in range(M):
-        Option.STs[i] = self.S * (u ** (N - i)) * (d ** i)
+        option.STs[i] = self.S * (u ** (N - i)) * (d ** i)
     def init_payoffs_tree():
       if self.is_call:
-        return np.maximum(0, Option.STs - Option.K)
+        return np.maximum(0, option.STs - option.K)
       else:
-        return np.maximum(0, Option.K - Option.STs)
+        return np.maximum(0, option.K - option.STs)
     def traverse_tree(payoffs):
       for i in range(N):
-        payoffs = (payoffs[:-1] * qu + payoffs[1:] * qd) * Option.df
+        payoffs = (payoffs[:-1] * qu + payoffs[1:] * qd) * option.df
       return payoffs
     def begin_tree_traversal():
       payoffs = init_payoffs_tree()
       return traverse_tree(payoffs)
     init_stock_price_tree()
     payoff = begin_tree_traversal()
     return payoff[0]
```

### Comparing `stockdatamanager-0.9/stockdatamanager.egg-info/PKG-INFO` & `stockdatamanager-0.9.1/stockdatamanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdatamanager
-Version: 0.9
+Version: 0.9.1
 Summary: A comprehensive library for financial analysis
 Home-page: https://github.com/GiorgioMB/stockdatafetcher/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stockdatamanager-0.9/tests/test.py` & `stockdatamanager-0.9.1/tests/test.py`

 * *Files identical despite different names*

