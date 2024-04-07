# Comparing `tmp/betanegbinfit-1.9.8.tar.gz` & `tmp/betanegbinfit-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betanegbinfit-1.9.8.tar", last modified: Fri Dec 15 16:08:52 2023, max compression
+gzip compressed data, was "betanegbinfit-1.9.9.tar", last modified: Fri Dec 15 16:15:54 2023, max compression
```

## Comparing `betanegbinfit-1.9.8.tar` & `betanegbinfit-1.9.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-12-15 16:08:52.103947 betanegbinfit-1.9.8/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-12-15 16:08:52.103947 betanegbinfit-1.9.8/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2023-11-13 11:14:10.000000 betanegbinfit-1.9.8/README.md
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-12-15 16:08:52.103947 betanegbinfit-1.9.8/betanegbinfit/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      725 2023-12-15 11:11:23.000000 betanegbinfit-1.9.8/betanegbinfit/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/betacdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/betainc.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/bridge_mixalime.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6400 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/cdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/combine.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/create.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    38510 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/distributions.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/hyp.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-12-15 16:08:52.103947 betanegbinfit-1.9.8/betanegbinfit/models/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/models/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/models/model.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    22244 2023-12-15 13:18:52.000000 betanegbinfit-1.9.8/betanegbinfit/models/model_line.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/models/model_line_lrt.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14815 2023-12-15 16:02:22.000000 betanegbinfit-1.9.8/betanegbinfit/models/model_mixture.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/models/model_mixtures.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29978 2023-12-15 16:02:16.000000 betanegbinfit-1.9.8/betanegbinfit/models/model_window.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/plot.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/stats.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-11-13 11:34:29.000000 betanegbinfit-1.9.8/betanegbinfit/tests.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29743 2023-12-15 12:21:27.000000 betanegbinfit-1.9.8/betanegbinfit/utils.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-12-15 16:08:52.103947 betanegbinfit-1.9.8/betanegbinfit.egg-info/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-12-15 16:08:52.000000 betanegbinfit-1.9.8/betanegbinfit.egg-info/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-12-15 16:08:52.000000 betanegbinfit-1.9.8/betanegbinfit.egg-info/SOURCES.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-12-15 16:08:52.000000 betanegbinfit-1.9.8/betanegbinfit.egg-info/dependency_links.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-12-15 16:08:52.000000 betanegbinfit-1.9.8/betanegbinfit.egg-info/requires.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-12-15 16:08:52.000000 betanegbinfit-1.9.8/betanegbinfit.egg-info/top_level.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-12-15 16:08:52.103947 betanegbinfit-1.9.8/setup.cfg
--rw-r--r--   0 georgy    (1000) georgy    (1001)      963 2023-11-13 11:14:10.000000 betanegbinfit-1.9.8/setup.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-12-15 16:15:54.298297 betanegbinfit-1.9.9/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-12-15 16:15:54.298297 betanegbinfit-1.9.9/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2023-11-13 11:14:10.000000 betanegbinfit-1.9.9/README.md
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-12-15 16:15:54.294963 betanegbinfit-1.9.9/betanegbinfit/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      725 2023-12-15 16:15:26.000000 betanegbinfit-1.9.9/betanegbinfit/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/betacdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/betainc.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/bridge_mixalime.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6400 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/cdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/combine.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/create.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    38510 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/distributions.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/hyp.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-12-15 16:15:54.294963 betanegbinfit-1.9.9/betanegbinfit/models/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/models/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/models/model.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    22244 2023-12-15 13:18:52.000000 betanegbinfit-1.9.9/betanegbinfit/models/model_line.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/models/model_line_lrt.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14363 2023-12-15 16:14:38.000000 betanegbinfit-1.9.9/betanegbinfit/models/model_mixture.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/models/model_mixtures.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29978 2023-12-15 16:02:16.000000 betanegbinfit-1.9.9/betanegbinfit/models/model_window.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/plot.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/stats.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-11-13 11:34:29.000000 betanegbinfit-1.9.9/betanegbinfit/tests.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29743 2023-12-15 12:21:27.000000 betanegbinfit-1.9.9/betanegbinfit/utils.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-12-15 16:15:54.294963 betanegbinfit-1.9.9/betanegbinfit.egg-info/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-12-15 16:15:54.000000 betanegbinfit-1.9.9/betanegbinfit.egg-info/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-12-15 16:15:54.000000 betanegbinfit-1.9.9/betanegbinfit.egg-info/SOURCES.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-12-15 16:15:54.000000 betanegbinfit-1.9.9/betanegbinfit.egg-info/dependency_links.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-12-15 16:15:54.000000 betanegbinfit-1.9.9/betanegbinfit.egg-info/requires.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-12-15 16:15:54.000000 betanegbinfit-1.9.9/betanegbinfit.egg-info/top_level.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-12-15 16:15:54.298297 betanegbinfit-1.9.9/setup.cfg
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      963 2023-11-13 11:14:10.000000 betanegbinfit-1.9.9/setup.py
```

### Comparing `betanegbinfit-1.9.8/PKG-INFO` & `betanegbinfit-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.9.8
+Version: 1.9.9
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `betanegbinfit-1.9.8/README.md` & `betanegbinfit-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/__init__.py` & `betanegbinfit-1.9.9/betanegbinfit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.9.8'
+__version__ = '1.9.9'
 
 import warnings
 # This will omit annoying FutureWarnings by JAX and RutimeWarnings caused by
 # estimates being clipped at bounds.
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.simplefilter(action='ignore', category=RuntimeWarning)
```

### Comparing `betanegbinfit-1.9.8/betanegbinfit/betacdnb.py` & `betanegbinfit-1.9.9/betanegbinfit/betacdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/betainc.py` & `betanegbinfit-1.9.9/betanegbinfit/betainc.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/bridge_mixalime.py` & `betanegbinfit-1.9.9/betanegbinfit/bridge_mixalime.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/cdnb.py` & `betanegbinfit-1.9.9/betanegbinfit/cdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/combine.py` & `betanegbinfit-1.9.9/betanegbinfit/combine.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/create.py` & `betanegbinfit-1.9.9/betanegbinfit/create.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/distributions.py` & `betanegbinfit-1.9.9/betanegbinfit/distributions.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/hyp.py` & `betanegbinfit-1.9.9/betanegbinfit/hyp.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/models/model.py` & `betanegbinfit-1.9.9/betanegbinfit/models/model.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/models/model_line.py` & `betanegbinfit-1.9.9/betanegbinfit/models/model_line.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/models/model_line_lrt.py` & `betanegbinfit-1.9.9/betanegbinfit/models/model_line_lrt.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/models/model_mixture.py` & `betanegbinfit-1.9.9/betanegbinfit/models/model_mixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -391,19 +391,8 @@
         s1 = sampler(p1, n)
         if self.bad == 1:
             return s1
         p2 = self.get_param('p2', params)
         s2 = sampler(p2, n)
         w = self.get_param('w', params)
         w = np.random.choice([1, 0], size=n, p=[w, 1 - w])
-        return w * s1 + (1 - w) * s2
-
-    def get_param(self, key, params):
-        res = super().get_param(key, params)
-        if self.constrain_p and self.estimate_p and self.bad != 1 and key in ('p1', 'p2'):
-            p1 = res if key == 'p1' else super().get_param('p1', params)
-            p2 = res if key == 'p2' else super().get_param('p2', params)
-            if key == 'p1':
-                res = p1 * p2
-            else:
-                res = p1 * (1 - p2)
-        return res
+        return w * s1 + (1 - w) * s2
```

### Comparing `betanegbinfit-1.9.8/betanegbinfit/models/model_mixtures.py` & `betanegbinfit-1.9.9/betanegbinfit/models/model_mixtures.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/models/model_window.py` & `betanegbinfit-1.9.9/betanegbinfit/models/model_window.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/plot.py` & `betanegbinfit-1.9.9/betanegbinfit/plot.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/stats.py` & `betanegbinfit-1.9.9/betanegbinfit/stats.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/tests.py` & `betanegbinfit-1.9.9/betanegbinfit/tests.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit/utils.py` & `betanegbinfit-1.9.9/betanegbinfit/utils.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/betanegbinfit.egg-info/PKG-INFO` & `betanegbinfit-1.9.9/betanegbinfit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.9.8
+Version: 1.9.9
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `betanegbinfit-1.9.8/betanegbinfit.egg-info/SOURCES.txt` & `betanegbinfit-1.9.9/betanegbinfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.8/setup.py` & `betanegbinfit-1.9.9/setup.py`

 * *Files identical despite different names*

