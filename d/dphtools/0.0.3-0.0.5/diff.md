# Comparing `tmp/dphtools-0.0.3.tar.gz` & `tmp/dphtools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dphtools-0.0.3.tar", last modified: Fri Sep  9 05:47:11 2022, max compression
+gzip compressed data, was "dphtools-0.0.5.tar", last modified: Mon Apr  8 20:52:43 2024, max compression
```

## Comparing `dphtools-0.0.3.tar` & `dphtools-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 05:47:11.683506 dphtools-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11346 2022-09-09 05:47:08.000000 dphtools-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-09 05:47:08.000000 dphtools-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-09-09 05:47:11.683506 dphtools-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-09-09 05:47:08.000000 dphtools-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 05:47:11.683506 dphtools-0.0.3/dphtools/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-09-09 05:47:08.000000 dphtools-0.0.3/dphtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-09-09 05:47:11.683506 dphtools-0.0.3/dphtools/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    20665 2022-09-09 05:47:08.000000 dphtools-0.0.3/dphtools/display.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 05:47:11.683506 dphtools-0.0.3/dphtools/utils/
--rw-r--r--   0 runner    (1001) docker     (121)    25062 2022-09-09 05:47:08.000000 dphtools-0.0.3/dphtools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3623 2022-09-09 05:47:08.000000 dphtools-0.0.3/dphtools/utils/beads.py
--rw-r--r--   0 runner    (1001) docker     (121)    18430 2022-09-09 05:47:08.000000 dphtools-0.0.3/dphtools/utils/fitfuncs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-09-09 05:47:08.000000 dphtools-0.0.3/dphtools/utils/histstats.py
--rw-r--r--   0 runner    (1001) docker     (121)    23139 2022-09-09 05:47:08.000000 dphtools-0.0.3/dphtools/utils/lm.py
--rw-r--r--   0 runner    (1001) docker     (121)    21011 2022-09-09 05:47:08.000000 dphtools-0.0.3/dphtools/utils/lpsvd.py
--rw-r--r--   0 runner    (1001) docker     (121)    28269 2022-09-09 05:47:08.000000 dphtools-0.0.3/dphtools/utils/registration.py
--rw-r--r--   0 runner    (1001) docker     (121)     7417 2022-09-09 05:47:08.000000 dphtools-0.0.3/dphtools/utils/rolling_ball.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 05:47:11.679506 dphtools-0.0.3/dphtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-09-09 05:47:11.000000 dphtools-0.0.3/dphtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-09-09 05:47:11.000000 dphtools-0.0.3/dphtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 05:47:11.000000 dphtools-0.0.3/dphtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-09 05:47:11.000000 dphtools-0.0.3/dphtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-09 05:47:11.000000 dphtools-0.0.3/dphtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-09 05:47:08.000000 dphtools-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-09 05:47:11.683506 dphtools-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-09-09 05:47:08.000000 dphtools-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 05:47:11.683506 dphtools-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-09-09 05:47:08.000000 dphtools-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-09-09 05:47:08.000000 dphtools-0.0.3/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-09-09 05:47:08.000000 dphtools-0.0.3/tests/test_fitfuncs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8512 2022-09-09 05:47:08.000000 dphtools-0.0.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    69935 2022-09-09 05:47:08.000000 dphtools-0.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:52:43.114302 dphtools-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-08 20:52:35.000000 dphtools-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 20:52:35.000000 dphtools-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-08 20:52:43.114302 dphtools-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-08 20:52:35.000000 dphtools-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:52:43.114302 dphtools-0.0.5/dphtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-08 20:52:35.000000 dphtools-0.0.5/dphtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 20:52:43.114302 dphtools-0.0.5/dphtools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20665 2024-04-08 20:52:35.000000 dphtools-0.0.5/dphtools/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:52:43.114302 dphtools-0.0.5/dphtools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    26525 2024-04-08 20:52:35.000000 dphtools-0.0.5/dphtools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-08 20:52:35.000000 dphtools-0.0.5/dphtools/utils/beads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18430 2024-04-08 20:52:35.000000 dphtools-0.0.5/dphtools/utils/fitfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-08 20:52:35.000000 dphtools-0.0.5/dphtools/utils/histstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23139 2024-04-08 20:52:35.000000 dphtools-0.0.5/dphtools/utils/lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21011 2024-04-08 20:52:35.000000 dphtools-0.0.5/dphtools/utils/lpsvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28269 2024-04-08 20:52:35.000000 dphtools-0.0.5/dphtools/utils/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-04-08 20:52:35.000000 dphtools-0.0.5/dphtools/utils/rolling_ball.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:52:43.114302 dphtools-0.0.5/dphtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-08 20:52:43.000000 dphtools-0.0.5/dphtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 20:52:43.000000 dphtools-0.0.5/dphtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:52:43.000000 dphtools-0.0.5/dphtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 20:52:43.000000 dphtools-0.0.5/dphtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 20:52:43.000000 dphtools-0.0.5/dphtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 20:52:35.000000 dphtools-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 20:52:43.114302 dphtools-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 20:52:35.000000 dphtools-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:52:43.114302 dphtools-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 20:52:35.000000 dphtools-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 20:52:35.000000 dphtools-0.0.5/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-08 20:52:35.000000 dphtools-0.0.5/tests/test_fitfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-04-08 20:52:35.000000 dphtools-0.0.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-08 20:52:35.000000 dphtools-0.0.5/versioneer.py
```

### Comparing `dphtools-0.0.3/LICENSE` & `dphtools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/PKG-INFO` & `dphtools-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: dphtools
-Version: 0.0.3
+Version: 0.0.5
 Summary: Tools for optics and image analysis
 Home-page: https://github.com/david-hoffman/dphtools
 Author: David Hoffman
 Author-email: dave.p.hoffman@gmail.com
 License: Apache V2.0
-Description: <!-- [![PyPI version](https://badge.fury.io/py/dphtools.svg)](https://badge.fury.io/py/dphtools) -->
-        <!-- [![Anaconda version](https://anaconda.org/david-hoffman/dphtools/badges/downloads.svg)](https://anaconda.org/david-hoffman/dphtools) -->
-        <!-- [![Conda Badge](https://anaconda.org/david-hoffman/dphtools/badges/installer/conda.svg)](https://anaconda.org/david-hoffman/dphtools) -->
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![ci](https://github.com/david-hoffman/dphtools/workflows/ci/badge.svg)](https://github.com/david-hoffman/dphtools/actions?query=workflow%3Aci)
-        [![Create Release](https://github.com/david-hoffman/dphtools/workflows/Create%20Release/badge.svg)](https://github.com/david-hoffman/dphtools/actions?query=workflow%3A%22Create+Release%22)
-        
-        # dphtools
-        
-        Tools for optics and image analysis
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<!-- [![PyPI version](https://badge.fury.io/py/dphtools.svg)](https://badge.fury.io/py/dphtools) -->
+<!-- [![Anaconda version](https://anaconda.org/david-hoffman/dphtools/badges/downloads.svg)](https://anaconda.org/david-hoffman/dphtools) -->
+<!-- [![Conda Badge](https://anaconda.org/david-hoffman/dphtools/badges/installer/conda.svg)](https://anaconda.org/david-hoffman/dphtools) -->
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![ci](https://github.com/david-hoffman/dphtools/workflows/ci/badge.svg)](https://github.com/david-hoffman/dphtools/actions?query=workflow%3Aci)
+[![Create Release](https://github.com/david-hoffman/dphtools/workflows/Create%20Release/badge.svg)](https://github.com/david-hoffman/dphtools/actions?query=workflow%3A%22Create+Release%22)
+
+# dphtools
+
+Tools for optics and image analysis
```

### Comparing `dphtools-0.0.3/README.md` & `dphtools-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/dphtools/display.py` & `dphtools-0.0.5/dphtools/display.py`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/dphtools/utils/__init__.py` & `dphtools-0.0.5/dphtools/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -418,15 +418,15 @@
     k_kernel = rfftn(ifftshift(kernel), pad_data.shape, **kwargs)
     k_data = rfftn(pad_data, pad_data.shape, **kwargs)
     convolve_data = irfftn(k_kernel * k_data, pad_data.shape, **kwargs)
     # return data with same shape as original data
     return convolve_data[fslice]
 
 
-def win_nd(size, win_func=scipy.signal.hann, **kwargs):
+def win_nd(size, win_func=scipy.signal.windows.hann, **kwargs):
     """Make a multidimensional version of a window function.
 
     Parameters
     ----------
     size : tuple of ints
         size of the output window
     win_func : callable
@@ -709,15 +709,22 @@
 
     # build A matrix for quadratic function
     A = np.c_[X * X, Y * Y, X, Y, X * Y, np.ones(len(Z))]
 
     # calculate best fit coefs
     C, _, _, _ = scipy.linalg.lstsq(A, Z)
 
-    return C
+    n, k = A.shape
+    res = Z - A @ C
+    VCV = 1 / (n - k) * (res.T @ res) * np.linalg.inv(A.T @ A)
+
+    ## Standard errors of the estimated coefficients
+    stderr = np.sqrt(np.diagonal(VCV))
+
+    return C, stderr
 
 
 def find_center(x: np.ndarray, y: np.ndarray, z: np.ndarray) -> np.ndarray:
     """Find center of parabola.
 
     https://en.wikipedia.org/wiki/Quadratic_function#Minimum/maximum
 
@@ -729,30 +736,72 @@
 
     Returns
     -------
     (x_m, y_m) : floats
         The center as determined by a parabolic fit
     """
     # get fit coefs
-    quad_coefs = fit_quadratic(x, y, z)
-    return find_center_quad_coefs(quad_coefs)
+    quad_coefs, stderr = fit_quadratic(x, y, z)
+    return find_center_quad_coefs(quad_coefs, stderr)
+
+
+def find_center_quad_coefs(quad_coefs, stderr):
+    """Find the center of a quadratic fit given it's coefficients.
+
+    Parameters
+    ----------
+    quad_coefs : np.ndarray
+        Coefficients of the quadratic fit: see `fit_quadratic` for functional form.
+    stderr : np.ndarray
+        Standard error on those coefficients
 
+    Returns
+    -------
+    x0, y0 : tuple
+        Found center
+    x0_e, y0_e : tuple
+        standard error on the found center
 
-def find_center_quad_coefs(quad_coefs):
+    NOTE: the error of the center is found using the normal simplification which may not
+    be applicable or desireable here (https://en.wikipedia.org/wiki/Propagation_of_uncertainty#Simplification)
+    """
     aa, bb, cc, dd, ee, _ = quad_coefs
+    aa_e, bb_e, cc_e, dd_e, ee_e, _ = stderr
+
     denom = 4 * aa * bb - ee * ee
+    denom_e = np.sqrt((4 * bb * aa_e) ** 2 + (4 * aa * bb_e) ** 2 + (2 * ee * ee_e) ** 2)
 
     # check if an extreme point is found
     assert denom > 0, "No extrema found"
 
     # calculate the maximum or minimum
     x_m = -(2 * bb * cc - dd * ee) / denom
+    x_m_e = (
+        np.sqrt(
+            (2 * cc * bb_e) ** 2
+            + (2 * bb * cc_e) ** 2
+            + (ee * dd_e) ** 2
+            + (dd * ee_e) ** 2
+            + (x_m * denom_e) ** 2
+        )
+        / denom
+    )
     y_m = -(2 * aa * dd - cc * ee) / denom
+    y_m_e = (
+        np.sqrt(
+            (2 * dd * aa_e) ** 2
+            + (2 * aa * dd_e) ** 2
+            + (ee * cc_e) ** 2
+            + (cc * ee_e) ** 2
+            + (y_m * denom_e) ** 2
+        )
+        / denom
+    )
 
-    return (x_m, y_m)
+    return (x_m, y_m), (x_m_e, y_m_e)
 
 
 class EasyTimer(object):
     """Makes timing things easy with a `with` statement."""
 
     def __init__(self, msg=""):
         """Create an EasyTimer, choose the emit message."""
```

### Comparing `dphtools-0.0.3/dphtools/utils/beads.py` & `dphtools-0.0.5/dphtools/utils/beads.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def remove_coord_mean(df, *, coords=["x0", "y0"]):
     """Remove the mean value of the coordinates."""
     df_new = df.copy()
-    df_new[coords] = df_new[coords].astype(np.float)
+    df_new[coords] = df_new[coords].astype(float)
     coord_mean = df_new[coords].mean()
     df_new[coords] -= coord_mean
     return df_new.dropna()
 
 
 def calc_drift(
     fiducials_df,
```

### Comparing `dphtools-0.0.3/dphtools/utils/fitfuncs.py` & `dphtools-0.0.5/dphtools/utils/fitfuncs.py`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/dphtools/utils/histstats.py` & `dphtools-0.0.5/dphtools/utils/histstats.py`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/dphtools/utils/lm.py` & `dphtools-0.0.5/dphtools/utils/lm.py`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/dphtools/utils/lpsvd.py` & `dphtools-0.0.5/dphtools/utils/lpsvd.py`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/dphtools/utils/registration.py` & `dphtools-0.0.5/dphtools/utils/registration.py`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/dphtools/utils/rolling_ball.py` & `dphtools-0.0.5/dphtools/utils/rolling_ball.py`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/dphtools.egg-info/PKG-INFO` & `dphtools-0.0.5/dphtools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: dphtools
-Version: 0.0.3
+Version: 0.0.5
 Summary: Tools for optics and image analysis
 Home-page: https://github.com/david-hoffman/dphtools
 Author: David Hoffman
 Author-email: dave.p.hoffman@gmail.com
 License: Apache V2.0
-Description: <!-- [![PyPI version](https://badge.fury.io/py/dphtools.svg)](https://badge.fury.io/py/dphtools) -->
-        <!-- [![Anaconda version](https://anaconda.org/david-hoffman/dphtools/badges/downloads.svg)](https://anaconda.org/david-hoffman/dphtools) -->
-        <!-- [![Conda Badge](https://anaconda.org/david-hoffman/dphtools/badges/installer/conda.svg)](https://anaconda.org/david-hoffman/dphtools) -->
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![ci](https://github.com/david-hoffman/dphtools/workflows/ci/badge.svg)](https://github.com/david-hoffman/dphtools/actions?query=workflow%3Aci)
-        [![Create Release](https://github.com/david-hoffman/dphtools/workflows/Create%20Release/badge.svg)](https://github.com/david-hoffman/dphtools/actions?query=workflow%3A%22Create+Release%22)
-        
-        # dphtools
-        
-        Tools for optics and image analysis
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<!-- [![PyPI version](https://badge.fury.io/py/dphtools.svg)](https://badge.fury.io/py/dphtools) -->
+<!-- [![Anaconda version](https://anaconda.org/david-hoffman/dphtools/badges/downloads.svg)](https://anaconda.org/david-hoffman/dphtools) -->
+<!-- [![Conda Badge](https://anaconda.org/david-hoffman/dphtools/badges/installer/conda.svg)](https://anaconda.org/david-hoffman/dphtools) -->
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![ci](https://github.com/david-hoffman/dphtools/workflows/ci/badge.svg)](https://github.com/david-hoffman/dphtools/actions?query=workflow%3Aci)
+[![Create Release](https://github.com/david-hoffman/dphtools/workflows/Create%20Release/badge.svg)](https://github.com/david-hoffman/dphtools/actions?query=workflow%3A%22Create+Release%22)
+
+# dphtools
+
+Tools for optics and image analysis
```

### Comparing `dphtools-0.0.3/dphtools.egg-info/SOURCES.txt` & `dphtools-0.0.5/dphtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/setup.py` & `dphtools-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/tests/__init__.py` & `dphtools-0.0.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/tests/test_fitfuncs.py` & `dphtools-0.0.5/tests/test_fitfuncs.py`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/tests/test_utils.py` & `dphtools-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dphtools-0.0.3/versioneer.py` & `dphtools-0.0.5/versioneer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,63 @@
-# Version: 0.19
+# Version: 0.29
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible with: Python 3.6, 3.7, 3.8, 3.9 and pypy3
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10, 3.11 and pypy3
 * [![Latest Version][pypi-image]][pypi-url]
 * [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
 * `pip install versioneer` to somewhere in your $PATH
-* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
-* run `versioneer install` in your source tree, commit the results
-* Verify version information with `python setup.py version`
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -226,17 +254,18 @@
 
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -251,59 +280,92 @@
 
 ## Similar projects
 
 * [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
   dependency
 * [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
   versioneer
+* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
+  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
 
 [pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
 [pypi-url]: https://pypi.python.org/pypi/versioneer/
 [travis-image]:
 https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
 [travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
 import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
+from typing import NoReturn
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    versionfile_source: str
+    versionfile_build: Optional[str]
+    parentdir_prefix: Optional[str]
+    verbose: Optional[bool]
 
-def get_root():
+
+def get_root() -> str:
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
     setup_py = os.path.join(root, "setup.py")
+    pyproject_toml = os.path.join(root, "pyproject.toml")
     versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py) or os.path.exists(pyproject_toml) or os.path.exists(versioneer_py)
+    ):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
+        pyproject_toml = os.path.join(root, "pyproject.toml")
         versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py) or os.path.exists(pyproject_toml) or os.path.exists(versioneer_py)
+    ):
         err = (
             "Versioneer was unable to run the project root directory. "
             "Versioneer requires setup.py to be executed from "
             "its immediate directory (like 'python setup.py COMMAND'), "
             "or in a way that lets it use sys.argv[0] to find the root "
             "(like 'python path/to/setup.py COMMAND')."
         )
@@ -311,138 +373,172 @@
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        me = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(me)[0])
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print(
                 "Warning: build in %s is using versioneer.py from %s"
-                % (os.path.dirname(me), versioneer_py)
+                % (os.path.dirname(my_path), versioneer_py)
             )
     except NameError:
         pass
     return root
 
 
-def get_config_from_root(root):
+def get_config_from_root(root: str) -> VersioneerConfig:
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.ConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.read_file(f)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    def get(parser, name):
-        if parser.has_option("versioneer", name):
-            return parser.get("versioneer", name)
-        return None
+    root_pth = Path(root)
+    pyproject_toml = root_pth / "pyproject.toml"
+    setup_cfg = root_pth / "setup.cfg"
+    section: Union[Dict[str, Any], configparser.SectionProxy, None] = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, "rb") as fobj:
+                pp = tomllib.load(fobj)
+            section = pp["tool"]["versioneer"]
+        except (tomllib.TOMLDecodeError, KeyError) as e:
+            print(f"Failed to load config from {pyproject_toml}: {e}")
+            print("Try to load it from setup.cfg")
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
+    # `cast`` really shouldn't be used, but its simplest for the
+    # common VersioneerConfig users at the moment. We verify against
+    # `None` values elsewhere where it matters
 
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = get(parser, "style") or ""
-    cfg.versionfile_source = get(parser, "versionfile_source")
-    cfg.versionfile_build = get(parser, "versionfile_build")
-    cfg.tag_prefix = get(parser, "tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.VCS = section["VCS"]
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = cast(str, section.get("versionfile_source"))
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = cast(str, section.get("tag_prefix"))
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
-    cfg.verbose = get(parser, "verbose")
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    if isinstance(section, configparser.SectionProxy):
+        # Make sure configparser translates to bool
+        cfg.verbose = section.getboolean("verbose")
+    else:
+        cfg.verbose = section.get("verbose")
+
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
 
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
+        HANDLERS.setdefault(vcs, {})[method] = f
         return f
 
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen(
-                [c] + args,
+            process = subprocess.Popen(
+                [command] + args,
                 cwd=cwd,
                 env=env,
                 stdout=subprocess.PIPE,
                 stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
             )
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = p.communicate()[0].strip().decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
 LONG_VERSION_PY[
     "git"
 ] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.19 (https://github.com/python-versioneer/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.29
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Any, Callable, Dict, List, Optional, Tuple
+import functools
 
 
-def get_keywords():
+def get_keywords() -> Dict[str, str]:
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
@@ -450,16 +546,23 @@
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    parentdir_prefix: str
+    versionfile_source: str
+    verbose: bool
 
-def get_config():
+
+def get_config() -> VersioneerConfig:
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "%(STYLE)s"
     cfg.tag_prefix = "%(TAG_PREFIX)s"
@@ -469,123 +572,142 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = p.communicate()[0].strip().decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
         date = date.splitlines()[-1]
 
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
@@ -596,36 +718,41 @@
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -633,52 +760,97 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%%s*" %% tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -687,15 +859,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -712,37 +884,35 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -759,31 +929,79 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post0.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post0.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post0.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
         rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -802,15 +1020,44 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -824,15 +1071,15 @@
         # exception #1
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -844,15 +1091,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -864,47 +1111,51 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%%s'" %% style)
 
     return {"version": rendered, "full-revisionid": pieces["long"],
             "dirty": pieces["dirty"], "error": None,
             "date": pieces.get("date")}
 
 
-def get_versions():
+def get_versions() -> Dict[str, Any]:
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
@@ -917,15 +1168,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for i in cfg.versionfile_source.split('/'):
+        for _ in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -944,47 +1195,50 @@
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
             "error": "unable to compute version", "date": None}
 '''
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
         date = date.splitlines()[-1]
 
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
@@ -995,36 +1249,41 @@
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r"\d", r)])
+        tags = {r for r in refs if re.search(r"\d", r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix) :]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r"\d", r):
+                continue
             if verbose:
                 print("picking %s" % r)
             return {
                 "version": r,
                 "full-revisionid": keywords["full"].strip(),
                 "dirty": False,
                 "error": None,
@@ -1039,52 +1298,101 @@
         "dirty": False,
         "error": "no suitable tags",
         "date": None,
     }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str, root: str, verbose: bool, runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(
+    describe_out, rc = runner(
         GITS,
-        ["describe", "--tags", "--dirty", "--always", "--long", "--match", "%s*" % tag_prefix],
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            f"{tag_prefix}[[:digit:]]*",
+        ],
         cwd=root,
     )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1093,15 +1401,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
@@ -1116,98 +1424,101 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        me = __file__
-        if me.endswith(".pyc") or me.endswith(".pyo"):
-            me = os.path.splitext(me)[0] + ".py"
-        versioneer_file = os.path.relpath(me)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
-        for line in f.readlines():
-            if line.strip().startswith(versionfile_source):
-                if "export-subst" in line.strip().split()[1:]:
-                    present = True
-        f.close()
-    except EnvironmentError:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
         pass
     if not present:
-        f = open(".gitattributes", "a+")
-        f.write("%s export-subst\n" % versionfile_source)
-        f.close()
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {
                 "version": dirname[len(parentdir_prefix) :],
                 "full-revisionid": None,
                 "dirty": False,
                 "error": None,
                 "date": None,
             }
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print(
             "Tried directories %s but none started with prefix %s"
             % (str(rootdirs), parentdir_prefix)
         )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.19) from
+# This file was generated by 'versioneer.py' (0.29) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1216,47 +1527,46 @@
 
 
 def get_versions():
     return json.loads(version_json)
 """
 
 
-def versions_from_file(filename):
+def versions_from_file(filename: str) -> Dict[str, Any]:
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
-def write_to_version_file(filename, versions):
+def write_to_version_file(filename: str, versions: Dict[str, Any]) -> None:
     """Write the given version number to the given _version.py file."""
-    os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -1272,31 +1582,78 @@
         # exception #1
         rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post0.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post0.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post0.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
         rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1315,15 +1672,44 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -1337,15 +1723,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1357,15 +1743,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1377,15 +1763,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {
             "version": "unknown",
             "full-revisionid": pieces.get("long"),
             "dirty": None,
             "error": pieces["error"],
@@ -1393,18 +1779,22 @@
         }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -1419,30 +1809,30 @@
     }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
-def get_versions(verbose=False):
+def get_versions(verbose: bool = False) -> Dict[str, Any]:
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or cfg.verbose
+    verbose = verbose or bool(cfg.verbose)  # `bool()` used to avoid `None`
     assert cfg.versionfile_source is not None, "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
@@ -1498,21 +1888,21 @@
         "full-revisionid": None,
         "dirty": None,
         "error": "unable to compute version",
         "date": None,
     }
 
 
-def get_version():
+def get_version() -> str:
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass(cmdclass=None):
-    """Get the custom setuptools/distutils subclasses used by Versioneer.
+def get_cmdclass(cmdclass: Optional[Dict[str, Any]] = None):
+    """Get the custom setuptools subclasses used by Versioneer.
 
     If the package uses a different cmdclass (e.g. one from numpy), it
     should be provide as an argument.
     """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
@@ -1526,114 +1916,128 @@
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
         # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
     cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
-        user_options = []
-        boolean_options = []
+        user_options: List[Tuple[str, str, str]] = []
+        boolean_options: List[str] = []
 
-        def initialize_options(self):
+        def initialize_options(self) -> None:
             pass
 
-        def finalize_options(self):
+        def finalize_options(self) -> None:
             pass
 
-        def run(self):
+        def run(self) -> None:
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
 
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
     if "build_py" in cmds:
-        _build_py = cmds["build_py"]
-    elif "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+        _build_py: Any = cmds["build_py"]
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
     cmds["build_py"] = cmd_build_py
 
-    if "setuptools" in sys.modules:
-        from setuptools.command.build_ext import build_ext as _build_ext
+    if "build_ext" in cmds:
+        _build_ext: Any = cmds["build_ext"]
     else:
-        from distutils.command.build_ext import build_ext as _build_ext
+        from setuptools.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_ext.run(self)
             if self.inplace:
                 # build_ext --inplace will only build extensions in
                 # build/lib<..> dir with no _version.py to write to.
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
-            target_versionfile = os.path.join(self.build_lib, cfg.versionfile_source)
+            if not cfg.versionfile_build:
+                return
+            target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(
+                    f"Warning: {target_versionfile} does not exist, skipping "
+                    "version update. This can happen if you are running build_ext "
+                    "without first running build_py."
+                )
+                return
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
 
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe
+        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore
 
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
         class cmd_build_exe(_build_exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1652,18 +2056,21 @@
                         }
                     )
 
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if "py2exe" in sys.modules:  # py2exe enabled?
-        from py2exe.distutils_buildexe import py2exe as _py2exe
+        try:
+            from py2exe.setuptools_buildexe import py2exe as _py2exe  # type: ignore
+        except ImportError:
+            from py2exe.distutils_buildexe import py2exe as _py2exe  # type: ignore
 
         class cmd_py2exe(_py2exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1680,32 +2087,69 @@
                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
                         }
                     )
 
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if "egg_info" in cmds:
+        _egg_info: Any = cmds["egg_info"]
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self) -> None:
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append("versioneer.py")
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+
+            normalized = [
+                unicode_utils.filesys_decode(f).replace(os.sep, "/") for f in self.filelist.files
+            ]
+
+            manifest_filename = os.path.join(self.egg_info, "SOURCES.txt")
+            with open(manifest_filename, "w") as fobj:
+                fobj.write("\n".join(normalized))
+
+    cmds["egg_info"] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
     if "sdist" in cmds:
-        _sdist = cmds["sdist"]
-    elif "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+        _sdist: Any = cmds["sdist"]
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
-        def run(self):
+        def run(self) -> None:
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
-        def make_release_tree(self, base_dir, files):
+        def make_release_tree(self, base_dir: str, files: List[str]) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
@@ -1750,28 +2194,33 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-INIT_PY_SNIPPET = """
+OLD_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
 
-def do_setup():
+
+def do_setup() -> int:
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError, configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+    except (OSError, configparser.NoSectionError, configparser.NoOptionError) as e:
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
@@ -1785,69 +2234,45 @@
                 "TAG_PREFIX": cfg.tag_prefix,
                 "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                 "VERSIONFILE_SOURCE": cfg.versionfile_source,
             }
         )
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
+    maybe_ipy: Optional[str] = ipy
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
-        if INIT_PY_SNIPPET not in old:
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(INIT_PY_SNIPPET)
+                f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
-        ipy = None
-
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" % cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
+        maybe_ipy = None
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, maybe_ipy)
     return 0
 
 
-def scan_setup_py():
+def scan_setup_py() -> int:
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
     with open("setup.py", "r") as f:
         for line in f.readlines():
             if "import versioneer" in line:
@@ -1876,14 +2301,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command() -> NoReturn:
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

