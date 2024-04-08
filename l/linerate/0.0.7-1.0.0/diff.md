# Comparing `tmp/linerate-0.0.7.tar.gz` & `tmp/linerate-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linerate-0.0.7.tar", max compression
+gzip compressed data, was "linerate-1.0.0.tar", max compression
```

## Comparing `linerate-0.0.7.tar` & `linerate-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1058 2023-06-28 10:00:53.772629 linerate-0.0.7/LICENSE
--rw-r--r--   0        0        0     3324 2023-06-28 10:00:53.772629 linerate-0.0.7/README.md
--rw-r--r--   0        0        0      221 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/__init__.py
--rw-r--r--   0        0        0      464 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/__init__.py
--rw-r--r--   0        0        0      148 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/cigre601/__init__.py
--rw-r--r--   0        0        0    22018 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/cigre601/convective_cooling.py
--rw-r--r--   0        0        0        0 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/cigre601/py.typed
--rw-r--r--   0        0        0     7621 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/cigre601/solar_heating.py
--rw-r--r--   0        0        0      147 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/ieee738/__init__.py
--rw-r--r--   0        0        0    11608 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/ieee738/convective_cooling.py
--rw-r--r--   0        0        0        0 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/ieee738/py.typed
--rw-r--r--   0        0        0     4559 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/ieee738/solar_heating.py
--rw-r--r--   0        0        0     5969 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/joule_heating.py
--rw-r--r--   0        0        0      553 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/math.py
--rw-r--r--   0        0        0        0 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/py.typed
--rw-r--r--   0        0        0     1351 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/radiative_cooling.py
--rw-r--r--   0        0        0     7276 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/equations/solar_angles.py
--rw-r--r--   0        0        0    21847 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/model.py
--rw-r--r--   0        0        0        0 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/py.typed
--rw-r--r--   0        0        0     6152 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/solver.py
--rw-r--r--   0        0        0     6697 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/types.py
--rw-r--r--   0        0        0     1476 2023-06-28 10:00:53.776630 linerate-0.0.7/linerate/units.py
--rw-r--r--   0        0        0     2325 2023-06-28 10:01:56.970604 linerate-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4110 1970-01-01 00:00:00.000000 linerate-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-04-08 11:36:41.365230 linerate-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3324 2024-04-08 11:36:41.365230 linerate-1.0.0/README.md
+-rw-r--r--   0        0        0      221 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/__init__.py
+-rw-r--r--   0        0        0      464 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/__init__.py
+-rw-r--r--   0        0        0      148 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/cigre601/__init__.py
+-rw-r--r--   0        0        0    22018 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/cigre601/convective_cooling.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/cigre601/py.typed
+-rw-r--r--   0        0        0     7634 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/cigre601/solar_heating.py
+-rw-r--r--   0        0        0      147 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/ieee738/__init__.py
+-rw-r--r--   0        0        0    11546 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/ieee738/convective_cooling.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/ieee738/py.typed
+-rw-r--r--   0        0        0     4559 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/ieee738/solar_heating.py
+-rw-r--r--   0        0        0     5969 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/joule_heating.py
+-rw-r--r--   0        0        0      331 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/math.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/py.typed
+-rw-r--r--   0        0        0     1351 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/radiative_cooling.py
+-rw-r--r--   0        0        0     7276 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/solar_angles.py
+-rw-r--r--   0        0        0    21848 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/model.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/py.typed
+-rw-r--r--   0        0        0     5754 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/solver.py
+-rw-r--r--   0        0        0     6697 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/types.py
+-rw-r--r--   0        0        0     1476 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/units.py
+-rw-r--r--   0        0        0     2227 2024-04-08 11:37:30.785199 linerate-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 linerate-1.0.0/PKG-INFO
```

### Comparing `linerate-0.0.7/LICENSE` & `linerate-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Copyright 2023 Statnett SF
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `linerate-0.0.7/README.md` & `linerate-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `linerate-0.0.7/linerate/equations/cigre601/convective_cooling.py` & `linerate-1.0.0/linerate/equations/cigre601/convective_cooling.py`

 * *Files identical despite different names*

### Comparing `linerate-0.0.7/linerate/equations/cigre601/solar_heating.py` & `linerate-1.0.0/linerate/equations/cigre601/solar_heating.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
     sin_H_s = sin_solar_altitude
     N_s = clearness_ratio
     y = height_above_sea_level
 
     I_B_0 = N_s * 1280 * sin_H_s / (sin_H_s + 0.314)
     # Equation 19 says that
-    # I_B = I_B_0 * (1 + 1.4e-4 * y * (1367/I_B_0 - 1))
+    # I_B = I_B_0 * (1 + 1.4e-4 * y * (1367/I_B_0 - 1)) # noqa: E800
     # However, if I_B_0 = 0, this will divide by 0. To return NaN-values if and only
     # if the input is NaN, we therefore reformulate it
     scaled_y = 1.4e-4 * y
     I_B = I_B_0 * (1 - scaled_y) + 1367 * scaled_y
 
     return np.where(sin_H_s >= 0, I_B, 0 * I_B)
```

### Comparing `linerate-0.0.7/linerate/equations/ieee738/convective_cooling.py` & `linerate-1.0.0/linerate/equations/ieee738/convective_cooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,17 +230,14 @@
     N_Re = reynolds_number
     k_f = thermal_conductivity_of_air
     T_s = temperature_of_conductor_surface
     T_a = temperature_of_ambient_air
 
     q_c1 = K_angle * (1.01 + 1.35 * N_Re**0.52) * k_f * (T_s - T_a)
     q_c2 = K_angle * 0.754 * N_Re**0.6 * k_f * (T_s - T_a)
-    # if q_c1 > q_c2:
-    #     return q_c1
-    # return q_c2
 
     if hasattr(q_c1, "__len__"):
         q_cf = []
         for i in range(len(q_c1)):
             if q_c1[i] > q_c2[i]:
                 q_cf.append(q_c1[i])
             else:
```

### Comparing `linerate-0.0.7/linerate/equations/ieee738/solar_heating.py` & `linerate-1.0.0/linerate/equations/ieee738/solar_heating.py`

 * *Files identical despite different names*

### Comparing `linerate-0.0.7/linerate/equations/joule_heating.py` & `linerate-1.0.0/linerate/equations/joule_heating.py`

 * *Files identical despite different names*

### Comparing `linerate-0.0.7/linerate/equations/radiative_cooling.py` & `linerate-1.0.0/linerate/equations/radiative_cooling.py`

 * *Files identical despite different names*

### Comparing `linerate-0.0.7/linerate/equations/solar_angles.py` & `linerate-1.0.0/linerate/equations/solar_angles.py`

 * *Files identical despite different names*

### Comparing `linerate-0.0.7/linerate/model.py` & `linerate-1.0.0/linerate/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 These thermal model classes provide an easy-to-use interface to compute the thermal rating.
 They store conductor and span metadata as well as the weather parameters, compute all the
 heating and cooling effects and use those to estimate the thermal rating and conductor
 temperature. All numerical heavy-lifting is handled by the ``linerate.equations`` and the
 ``linerate.solver`` modules.
 """
+
 from abc import ABC, abstractmethod
 from numbers import Real
 from typing import Dict
 
 import numpy as np
 
 from linerate import solver
```

### Comparing `linerate-0.0.7/linerate/solver.py` & `linerate-1.0.0/linerate/solver.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from functools import partial
-from typing import Callable, Optional
+from typing import Callable
 
 import numpy as np
 
 from .units import Ampere, Celsius, FloatOrFloatArray, WattPerMeter
 
 __all__ = ["bisect", "compute_conductor_temperature", "compute_conductor_ampacity"]
 
 
 def bisect(
     f: Callable[[FloatOrFloatArray], FloatOrFloatArray],
     xmin: FloatOrFloatArray,
     xmax: FloatOrFloatArray,
     tolerance: float,
-    invalid_value: Optional[float] = None,
 ) -> FloatOrFloatArray:
     r"""Compute the roots of a function using a vectorized bisection method.
 
     Parameters
     ----------
     f:
         :math:`f: \mathbb{R}^n \to \mathbb{R}^n`. Function whose roots we wish to find.
@@ -28,52 +27,47 @@
         :math:`x_\max`. Maximum value for the free parameter, :math:`\mathbf{x}`. It is required
         that :math:`\text{sign}(f_i(x_\min)) \neq \text{sign}(f_i(x_\max))`. for all :math:`i`.
     tolerance:
         :math:`\Delta x`. The bisection iterations will terminate once all :math:`x_i`-s are
         bounded within an interval of size :math:`\Delta x` or less. The bisection method will
         run for :math:`\left\lceil\frac{x_\max - x_\min}{\Delta x}\right\rceil`
         iterations.
-    invalid_value:
-        If provided, then the this value is used whenever
-        :math:`\text{sign}(f(\mathbf{x}_\min)) = \text{sign}(f(\mathbf{x}_\max))`.
 
     Returns
     -------
     Union[float, float64, ndarray[Any, dtype[float64]]]
         :math:`\tilde{\mathbf{x}}`. Estimate for the roots of :math:`f`. For each :math:`f_i`,
         there is a root :math:`x_i \in [\tilde{x}_i - 0.5 \Delta x, \tilde{x}_i + 0.5 \Delta x]`
         so :math:`f_i(x_i) = 0`.
     """
-    if not np.isfinite(xmin) or not np.isfinite(xmax):
+    if not np.all(np.isfinite(xmin)) or not np.all(np.isfinite(xmax)):
         raise ValueError("xmin and xmax must be finite.")
     interval = np.max(np.abs(xmax - xmin))
 
     f_left = f(xmin)
     f_right = f(xmax)
 
     invalid_mask = np.sign(f_left) == np.sign(f_right)
-    if np.any(invalid_mask) and invalid_value is None:
+    if np.any(invalid_mask):
         raise ValueError(
             "f(xmin) and f(xmax) have the same sign. Consider increasing the search interval."
         )
-    elif isinstance(invalid_mask, bool) and invalid_mask:
-        return invalid_value  # type: ignore
 
     while interval > tolerance:
         xmid = 0.5 * (xmax + xmin)
         interval *= 0.5
         f_mid = f(xmid)
 
         mask = f_mid * f_left > 0  # fast way to check sign(f_mid) == sign(f_left)
         xmin = np.where(mask, xmid, xmin)
         xmax = np.where(mask, xmax, xmid)
         f_left = np.where(mask, f_mid, f_left)
         f_right = np.where(mask, f_right, f_mid)
 
-    out = np.where(invalid_mask, invalid_value, 0.5 * (xmax + xmin))  # type: ignore
+    out = 0.5 * (xmax + xmin)
     return out
 
 
 def compute_conductor_temperature(
     heat_balance: Callable[[Celsius, Ampere], WattPerMeter],
     current: Ampere,
     min_temperature: Celsius = -30,
@@ -135,17 +129,17 @@
     max_ampacity:
         :math:`I_\text{min}~\left[\text{A}\right]`. Upper bound for the numerical scheme for
         computing the ampacity
     tolerance:
         :math:`\Delta I~\left[\text{A}\right]`. The numerical accuracy of the ampacity. The
         bisection iterations will stop once the numerical ampacity uncertainty is below
         :math:`\Delta I`. The bisection method will run for
-        :math:`\left\lceil\frac{I_\text{min} - I_\text{min}}{\Delta I}\right\rceil` iterations.
+        :math:`\left\lceil\frac{I_\text{max} - I_\text{min}}{\Delta I}\right\rceil` iterations.
 
     Returns
     -------
     Union[float, float64, ndarray[Any, dtype[float64]]]
         :math:`I~\left[\text{A}\right]`. The thermal rating.
     """
     f = partial(heat_balance, max_conductor_temperature)
 
-    return bisect(f, min_ampacity, max_ampacity, tolerance, invalid_value=0)
+    return bisect(f, min_ampacity, max_ampacity, tolerance)
```

### Comparing `linerate-0.0.7/linerate/types.py` & `linerate-1.0.0/linerate/types.py`

 * *Files identical despite different names*

### Comparing `linerate-0.0.7/linerate/units.py` & `linerate-1.0.0/linerate/units.py`

 * *Files identical despite different names*

### Comparing `linerate-0.0.7/pyproject.toml` & `linerate-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 [tool.poetry]
 name = "linerate"
-version = "0.0.7"
+version = "1.0.0"
 description = "Library for computing line ampacity ratings for overhead lines"
-authors = ["Statnett Datascience <Datascience.Drift@Statnett.no>", "Yngve Mardal Moe <yngve.moe@statnett.no>"]
-repository = "https://gitlab.statnett.no/datascience/vest/linerate.git"
+authors = ["Statnett Datascience <Datascience.Drift@Statnett.no>", "Yngve Mardal Moe <yngve.m.moe@gmail.com>"]
+repository = "https://github.com/statnett/linerate.git"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.9,<3.13"
 numpy = "*"
 scipy = "*"
 numba = ">=0.56.4"
 pygeodesy = "*"
-typing-extensions = { version = ">=4.0.0", python = "<3.9" }
 
 [tool.poetry.dev-dependencies]
-black = "22.10.0"
+black = "24.3.0"
 coverage = { version = "*", extras = ['toml'] }
-flake8 = "6.0.0"
-flake8-bugbear = "23.2.13"
+flake8 = "7.0.0"
+flake8-bugbear = "24.2.6"
 hypothesis = ">= 6.56.2"
-isort = "5.12.0"
+isort = "5.13.2"
 pre-commit = "*"
-pytest = "7.2.1"
-pytest-cov = "4.0.0"
-pytest-randomly = "3.12.0"
+pytest = "8.1.1"
+pytest-cov = "5.0.0"
+pytest-randomly = "3.15.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^5.2.3"
+sphinx = "^7.0.0"
 sphinxcontrib-bibtex = "^2.5.0"
-sphinx-gallery = "^0.11.1"
-pydata-sphinx-theme = "^0.11.0"
-pillow = "^9.2.0"
+sphinx-gallery = "^0.15.0"
+pydata-sphinx-theme = "^0.15.0"
 matplotlib = "^3.6.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 pattern = "^(?P<base>\\d+\\.\\d+\\.\\d+)(-?((?P<stage>[a-zA-Z]+)\\.?(?P<revision>\\d+)?))?$"
```

### Comparing `linerate-0.0.7/PKG-INFO` & `linerate-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: linerate
-Version: 0.0.7
+Version: 1.0.0
 Summary: Library for computing line ampacity ratings for overhead lines
-Home-page: https://gitlab.statnett.no/datascience/vest/linerate.git
+Home-page: https://github.com/statnett/linerate.git
 Author: Statnett Datascience
 Author-email: Datascience.Drift@Statnett.no
-Requires-Python: >=3.8.1,<4.0
+Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numba (>=0.56.4)
 Requires-Dist: numpy
 Requires-Dist: pygeodesy
 Requires-Dist: scipy
-Requires-Dist: typing-extensions (>=4.0.0) ; python_version < "3.9"
-Project-URL: Repository, https://gitlab.statnett.no/datascience/vest/linerate.git
+Project-URL: Repository, https://github.com/statnett/linerate.git
 Description-Content-Type: text/markdown
 
 # Overview
 
 A package containing functionality to compute ampacity line ratings for overhead lines.
 Currently, the package only contains equations from CIGRE TB 601.
```

