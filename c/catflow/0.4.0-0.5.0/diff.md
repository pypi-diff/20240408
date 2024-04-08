# Comparing `tmp/catflow-0.4.0.tar.gz` & `tmp/catflow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catflow-0.4.0.tar", max compression
+gzip compressed data, was "catflow-0.5.0.tar", max compression
```

## Comparing `catflow-0.4.0.tar` & `catflow-0.5.0.tar`

### file list

```diff
@@ -1,45 +1,78 @@
--rw-r--r--   0        0        0    11357 2023-11-20 07:30:41.104884 catflow-0.4.0/LICENSE
--rw-r--r--   0        0        0     1644 2023-11-20 07:30:41.104884 catflow-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/__init__.py
--rw-r--r--   0        0        0      100 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/__main__.py
--rw-r--r--   0        0        0        0 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/atomic/__init__.py
--rw-r--r--   0        0        0      826 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/atomic/atomic_energy.py
--rw-r--r--   0        0        0     4532 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/atomic/utils.py
--rw-r--r--   0        0        0        0 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/cmdline/__init__.py
--rw-r--r--   0        0        0      277 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/cmdline/base.py
--rw-r--r--   0        0        0        0 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/graph/__init__.py
--rw-r--r--   0        0        0     2472 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/graph/plotting.py
--rw-r--r--   0        0        0        0 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/metad/__init__.py
--rw-r--r--   0        0        0    30516 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/metad/fes.py
--rw-r--r--   0        0        0     4392 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/metad/hills.py
--rw-r--r--   0        0        0     6442 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/metad/profile.py
--rw-r--r--   0        0        0    15578 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/metad/string.py
--rw-r--r--   0        0        0        0 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/structure/__init__.py
--rw-r--r--   0        0        0     4927 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/structure/cluster.py
--rw-r--r--   0        0        0     2287 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/structure/coordination_number.py
--rw-r--r--   0        0        0    10297 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/structure/dynamic_selection.py
--rw-r--r--   0        0        0     1377 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/structure/lindemann_index.py
--rw-r--r--   0        0        0        0 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/__init__.py
--rw-r--r--   0        0        0        0 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/ai2_kit/__init__.py
--rw-r--r--   0        0        0     1431 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/ai2_kit/exploration.py
--rw-r--r--   0        0        0      546 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/ai2_kit/labeling.py
--rw-r--r--   0        0        0     1736 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/ai2_kit/task.py
--rw-r--r--   0        0        0     1444 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/ai2_kit/training.py
--rw-r--r--   0        0        0        0 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/base/__init__.py
--rw-r--r--   0        0        0    24695 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/base/exploration.py
--rw-r--r--   0        0        0     4457 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/base/labeling.py
--rw-r--r--   0        0        0      829 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/base/task.py
--rw-r--r--   0        0        0     2795 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/base/training.py
--rw-r--r--   0        0        0        0 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/dpgen/__init__.py
--rw-r--r--   0        0        0    11313 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/dpgen/exploration.py
--rw-r--r--   0        0        0      731 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/dpgen/labeling.py
--rw-r--r--   0        0        0     3356 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/dpgen/task.py
--rw-r--r--   0        0        0     2052 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/tesla/dpgen/training.py
--rw-r--r--   0        0        0       54 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/utils/__init__.py
--rw-r--r--   0        0        0       57 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/utils/files.py
--rw-r--r--   0        0        0      524 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/utils/lammps.py
--rw-r--r--   0        0        0     1083 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/utils/log_factory.py
--rw-r--r--   0        0        0       45 2023-11-20 07:30:41.104884 catflow-0.4.0/catflow/utils/output.py
--rw-r--r--   0        0        0     1077 2023-11-20 07:30:41.116884 catflow-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 catflow-0.4.0/setup.py
--rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 catflow-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 08:43:29.925534 catflow-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3433 2024-04-08 08:43:29.925534 catflow-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/atomic/__init__.py
+-rw-r--r--   0        0        0      826 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/atomic/atomic_energy.py
+-rw-r--r--   0        0        0     4532 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/atomic/utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/graph/__init__.py
+-rw-r--r--   0        0        0     2472 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/graph/plotting.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.925534 catflow-0.5.0/catflow/analyzer/metad/__init__.py
+-rw-r--r--   0        0        0    34345 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/metad/fes.py
+-rw-r--r--   0        0        0     4392 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/metad/hills.py
+-rw-r--r--   0        0        0     6469 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/metad/profile.py
+-rw-r--r--   0        0        0    15587 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/metad/string.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/structure/__init__.py
+-rw-r--r--   0        0        0     4936 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/structure/cluster.py
+-rw-r--r--   0        0        0     2287 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/structure/coordination_number.py
+-rw-r--r--   0        0        0    10306 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/structure/dynamic_selection.py
+-rw-r--r--   0        0        0     1377 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/structure/lindemann_index.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/__init__.py
+-rw-r--r--   0        0        0     1449 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/exploration.py
+-rw-r--r--   0        0        0      573 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/labeling.py
+-rw-r--r--   0        0        0     1750 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/task.py
+-rw-r--r--   0        0        0     1471 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/training.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/base/__init__.py
+-rw-r--r--   0        0        0    24722 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/base/exploration.py
+-rw-r--r--   0        0        0     4475 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/base/labeling.py
+-rw-r--r--   0        0        0      829 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/base/task.py
+-rw-r--r--   0        0        0     2813 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/base/training.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/dpgen/__init__.py
+-rw-r--r--   0        0        0    11349 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/dpgen/exploration.py
+-rw-r--r--   0        0        0      749 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/dpgen/labeling.py
+-rw-r--r--   0        0        0     3365 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/dpgen/task.py
+-rw-r--r--   0        0        0     2079 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/analyzer/tesla/dpgen/training.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/__init__.py
+-rw-r--r--   0        0        0      553 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/base.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/calculation/__init__.py
+-rw-r--r--   0        0        0     1520 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/calculation/dpgen.py
+-rw-r--r--   0        0        0      468 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/calculation/vasp.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/workflow/__init__.py
+-rw-r--r--   0        0        0      796 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/workflow/pmf.py
+-rw-r--r--   0        0        0     1644 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/cmdline/workflow/tesla.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/__init__.py
+-rw-r--r--   0        0        0      111 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/calculation/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/calculation/cp2k.py
+-rw-r--r--   0        0        0    18491 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/calculation/dpgen.py
+-rw-r--r--   0        0        0     9017 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/calculation/vasp.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/code/__init__.py
+-rw-r--r--   0        0        0      915 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/code/base.py
+-rw-r--r--   0        0        0      150 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/code/vasp.py
+-rw-r--r--   0        0        0      882 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/configs/workflow/pmf_cp2k.yml
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/flows/__init__.py
+-rw-r--r--   0        0        0    32933 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/flows/pmf_flow.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/resources/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/resources/config.py
+-rw-r--r--   0        0        0     1446 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/resources/submit.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/runner/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/defaults/__init__.py
+-rw-r--r--   0        0        0     1795 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/defaults/pmf.py
+-rw-r--r--   0        0        0    12976 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/pmf.py
+-rw-r--r--   0        0        0    10450 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/screen.py
+-rw-r--r--   0        0        0    24938 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/tasker/tasks/tesla.py
+-rw-r--r--   0        0        0       54 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/config.py
+-rw-r--r--   0        0        0     1957 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/constant.py
+-rw-r--r--   0        0        0    13850 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/cp2k.py
+-rw-r--r--   0        0        0      966 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/file.py
+-rw-r--r--   0        0        0     3585 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/lammps.py
+-rw-r--r--   0        0        0     1083 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/log_factory.py
+-rw-r--r--   0        0        0     1283 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/messager.py
+-rw-r--r--   0        0        0       45 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/output.py
+-rw-r--r--   0        0        0     1629 2024-04-08 08:43:29.929534 catflow-0.5.0/catflow/utils/statistics.py
+-rw-r--r--   0        0        0     1229 2024-04-08 08:43:29.945534 catflow-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5344 1970-01-01 00:00:00.000000 catflow-0.5.0/setup.py
+-rw-r--r--   0        0        0     4790 1970-01-01 00:00:00.000000 catflow-0.5.0/PKG-INFO
```

### Comparing `catflow-0.4.0/LICENSE` & `catflow-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `catflow-0.4.0/catflow/atomic/atomic_energy.py` & `catflow-0.5.0/catflow/analyzer/atomic/atomic_energy.py`

 * *Files identical despite different names*

### Comparing `catflow-0.4.0/catflow/atomic/utils.py` & `catflow-0.5.0/catflow/analyzer/atomic/utils.py`

 * *Files identical despite different names*

### Comparing `catflow-0.4.0/catflow/graph/plotting.py` & `catflow-0.5.0/catflow/analyzer/graph/plotting.py`

 * *Files identical despite different names*

### Comparing `catflow-0.4.0/catflow/metad/fes.py` & `catflow-0.5.0/catflow/analyzer/metad/fes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 from copy import deepcopy
 from joblib import Parallel, delayed
-from typing import Optional, List, Union, Dict, Any
+from typing import Optional, List, Tuple, Union, Dict, Any
 from itertools import product
 from numpy.typing import ArrayLike
 from matplotlib.colors import Colormap
 
-from catflow.metad.hills import Hills
-from catflow.graph.plotting import canvas_style
+from catflow.analyzer.metad.hills import Hills
+from catflow.analyzer.graph.plotting import canvas_style
+from catflow.utils.config import parse_slice_string
 from catflow.utils.log_factory import logger
 
+dp2_cutoff_a = 1.0/(1.0 - np.exp(-6.25))
+dp2_cutoff_b = - np.exp(-6.25)/(1.0 - np.exp(-6.25))
 
 class FreeEnergySurface:
     """
     Computes the free energy surface corresponding to the provided Hills object.
 
     Usage:
     ```python
-    from catflow.metad.fes import FreeEnergySurface
+    from catflow.analyzer.metad.fes import FreeEnergySurface
     fes = FreeEnergySurface(hills)
     ```
 
     Args:
         hills (Hills): The Hills object used for computing the free energy surface.
         resolution (int, optional): \
             The resolution of the free energy surface. Defaults to 256.
@@ -47,15 +50,15 @@
         self,
         resolution: int = 256
     ):
         self.res = resolution
 
     @classmethod
     def from_hills(
-        cls, 
+        cls,
         hills: Hills,
         resolution: int = 256
     ):
         """Generate a FES object from a Hills object."""
         fes = cls(resolution=resolution)
 
         fes.cvs = hills.cvs
@@ -101,15 +104,15 @@
         fes.cv_max = np.array(cv_max)
         fes.cv_fes_range = np.array(cv_max) - np.array(cv_min)
         fes.periodic = np.array(periodic, dtype=bool)
         fes.cv_name = cv_name
         fes.res = resolution
         fes.cvs = len(cv_name)
         return fes
-    
+
     def name_cv(self):
         if self.cv_name is None:
             self.cv_name = []
             for i in range(self.cvs):
                 self.cv_name.append(f"CV{i+1}")
 
     def get_e_beta_c(
@@ -162,18 +165,16 @@
             (self.hills.cv[time_min:time_max, :cvs] -
              cv_min) * resolution / cv_fes_range
         ).T.astype(int)
 
         sigma = self.hills.sigma[:cvs, 0]
         sigma_res = (sigma * resolution) / (cv_max - cv_min)
 
-        gauss_res = (8 * sigma_res).astype(int)
-        for i, _ in enumerate(gauss_res):
-            if _ % 2 == 0:
-                gauss_res[i] += 1
+        gauss_res = np.ceil(8 * sigma_res).astype(int)
+        gauss_res[gauss_res % 2 == 0] += 1
 
         gauss = self._gauss_kernel(gauss_res, sigma_res)
         gauss_center = np.array(gauss.shape) // 2
 
         fes = np.zeros([resolution] * cvs)
         e_beta_c = np.zeros(len(cv_bins[0]))
 
@@ -182,32 +183,131 @@
                 self._sum_bias(
                     gauss_center, gauss, cv_bins, line, cvs, resolution
                 )
             fes[fes_index_to_edit] += delta_fes
 
             local_fes = fes - np.min(fes)
             exp_local_fes = np.exp(-local_fes / (kb * temp))
+            exp_local_fes_bias = np.exp(-local_fes / (kb * temp * bias_factor))
 
             numerator = np.sum(exp_local_fes)
-            denominator = np.sum(exp_local_fes / bias_factor)
+            denominator = np.sum(exp_local_fes_bias)
             e_beta_c[line] = numerator / denominator
         if return_fes:
             fes -= np.min(fes)
             return e_beta_c, fes
         else:
             return e_beta_c
 
+    def save_fes_with_correction(
+        self,
+        resolution=None,
+        time_min=None,
+        time_max=None,
+        kb: float = 8.314e-3,
+        temp: float = 300.0,
+        filename: Optional[str] = "fes_profile.hdf5"
+    ):
+        """
+        Calculate the free energy surface (FES) with correction.
+        Using eq.12 of doi:10.1021/jp504920s to get FES with correction,
+        as error estimator of FES surface.
+
+        Args:
+            resolution (int, optional): The resolution of the FES grid. Defaults to None.
+            time_min (int, optional): The minimum time index. Defaults to None.
+            time_max (int, optional): The maximum time index. Defaults to None.
+            kb (float, optional): The Boltzmann constant. Defaults to 8.314e-3.
+            temp (float, optional): The temperature. Defaults to 300.0.
+            return_fes (bool, optional): Whether to return the FES. Defaults to False.
+
+        Returns:
+            list: Returns a list containing the FES profile.
+        """
+        import h5py
+        from tqdm import trange
+
+        if resolution is None:
+            resolution = self.res
+
+        if self.hills is None:
+            raise ValueError("Hills not loaded yet.")
+
+        if time_min is None:
+            time_min = 0
+
+        if time_max is None:
+            time_max = len(self.hills.cv[:, 0])
+
+        cvs = self.cvs
+
+        cv_min = self.cv_min
+        cv_max = self.cv_max
+        if self.cv_fes_range is None:
+            self.cv_fes_range = cv_max - cv_min
+        cv_fes_range = self.cv_fes_range
+
+        cv_bins = np.ceil(
+            (self.hills.cv[time_min:time_max, :cvs] -
+             cv_min) * resolution / cv_fes_range
+        ).T.astype(int)
+
+        sigma = self.hills.sigma[:cvs, 0]
+        sigma_res = (sigma * resolution) / (cv_max - cv_min)
+
+        gauss_res = np.ceil(8 * sigma_res).astype(int)
+        gauss_res[gauss_res % 2 == 0] += 1
+
+        gauss = self._gauss_kernel(gauss_res, sigma_res)
+        gauss_center = np.array(gauss.shape) // 2
+
+        fes = np.zeros([resolution] * cvs)
+        d_cv = np.prod(cv_fes_range / resolution)
+
+        with h5py.File(filename, "w") as f:
+            fes_data = f.create_dataset(
+                "fes_data", 
+                shape=(len(cv_bins[0]), *fes.shape), 
+                dtype=np.float64, 
+                chunks=(1, *fes.shape)
+            )
+            for line in trange(len(cv_bins[0])):
+                fes_index_to_edit, delta_fes = \
+                    self._sum_bias(
+                        gauss_center, gauss, cv_bins, line, cvs, resolution
+                    )
+                fes[fes_index_to_edit] += delta_fes
+                correction = np.sum(np.exp(- fes / kb / temp)) * d_cv
+                fes_corrected = fes + kb * temp * np.log(correction)
+                fes_data[line] = fes_corrected
+        del fes, d_cv, fes_corrected
+
+    def load_fes_with_correction(
+        self, 
+        filename: str,
+        slice_string: Optional[str] = None
+    ):
+        import h5py
+
+        with h5py.File(filename, 'r') as f:
+            dataset = f["fes_data"]
+            if slice_string:
+                data_slice = parse_slice_string(slice_string)
+                return dataset[data_slice] # type: ignore
+            else:
+                return dataset[:] # type: ignore
+
     def _gauss_kernel(self, gauss_res, sigma_res):
 
         gauss_center = gauss_res // 2
         grids = np.indices(gauss_res)
-        
+
         grids_flatten = grids.reshape(gauss_res.shape[0], -1).T
         exponent = np.sum(
-            -(grids_flatten - gauss_center)**2 / (2 * sigma_res**2), 
+            -(grids_flatten - gauss_center)**2 / (2 * sigma_res**2),
             axis=1
         )
         gauss = -np.exp(exponent.T.reshape(gauss_res))
         return gauss
 
     def _sum_bias(
         self, gauss_center, gauss, cv_bins, line, cvs, resolution
@@ -238,15 +338,16 @@
     def reweighting(
         self,
         colvar_file: str,
         e_beta_c: ArrayLike,
         cv_indexes: Optional[List[int]] = None,
         resolution: int = 64,
         kb: float = 8.314e-3,
-        temp: float = 300.0
+        temp: float = 300.0,
+        bias_index: int = 2
     ):
         """
         Reweights the free energy surface based on the given collective variables.
 
         Args:
             colvar_file (str): The path to the file containing the collective variables.
             e_beta_c (ArrayLike): The array of e^(-beta*C(t)) values.
@@ -268,57 +369,49 @@
             colvar_value = np.vstack(
                 [colvar[:, i + 1] for i in cv_indexes]
             ).T
         cv_array = colvar_value - np.min(colvar_value, axis=0)
         cv_range = np.max(cv_array)
         cv_array = np.floor((resolution - 1) * cv_array / cv_range).astype(int)
 
-        bias = colvar[:, 9]
+        bias = colvar[:, bias_index]
         probs = np.zeros([resolution] * cvs)
 
         e_beta_c = np.array(e_beta_c)
         reweighted_fes = np.zeros([len(e_beta_c)] + [resolution] * cvs)
 
         for i in np.arange(len(e_beta_c)):
             index = tuple(cv_array[i])
             probs[index] += np.exp(bias[i]/(kb * temp)) / e_beta_c[i]
             reweighted_fes[i] = -kb * temp * np.log(probs)
 
         return reweighted_fes
 
-    def _calculate_dp2(self, index, time_min, time_max):
-        if self.hills is None:
-            raise ValueError("Hills not loaded yet.")
-
-        cv_min = self.cv_min
-        if self.cv_fes_range is None:
-            self.cv_fes_range = self.cv_max - self.cv_min
-        cv_fes_range = self.cv_fes_range
-        cvs = self.cvs
+    def _calculate_dp2(self, index, cv, sigma, cv_min, cv_fes_range):
 
-        dp2 = np.zeros(time_max - time_min)
-        for i, cv_idx in enumerate(range(cvs)):
+        dp2 = np.zeros(cv.shape[0])
+        for cv_idx in range(cv.shape[1]):
             dist_cv = \
-                self.hills.cv[time_min:time_max, cv_idx] - \
-                (cv_min[i] + index[i] * cv_fes_range[i] / self.res)
+                cv[:, cv_idx] - \
+                (cv_min[cv_idx] + index[cv_idx] * cv_fes_range[cv_idx] / self.res)
             if self.periodic[cv_idx]:
-                dist_cv[dist_cv < -0.5*cv_fes_range[i]] += cv_fes_range[i]
-                dist_cv[dist_cv > +0.5*cv_fes_range[i]] -= cv_fes_range[i]
+                dist_cv[dist_cv < -0.5*cv_fes_range[cv_idx]] += cv_fes_range[cv_idx]
+                dist_cv[dist_cv > +0.5*cv_fes_range[cv_idx]] -= cv_fes_range[cv_idx]
             dp2_local = dist_cv ** 2 / \
-                (2 * self.hills.sigma[cv_idx][0] ** 2)
+                (2 * sigma[:, cv_idx] ** 2)
             dp2 += dp2_local
 
         return dp2
 
     def make_fes_original(
         self,
         resolution: Optional[int],
         time_min: Optional[int] = None,
         time_max: Optional[int] = None,
-        n_workers: int = 2
+        n_workers: int = -1
     ):
         """
         Function internally used to sum Hills in the same way as Plumed `sum_hills`. 
 
         Args:
             resolution (int, optional): \
                 The resolution of the free energy surface. Defaults to 256.
@@ -337,26 +430,38 @@
 
         if time_min is None:
             time_min = 0
         if time_max is None:
             time_max = len(self.hills.cv[:, 0])
         time_limit = time_max - time_min
 
-        def calculate_fes(index):
-            dp2 = self._calculate_dp2(index, time_min, time_max)
+        if self.hills is None:
+            raise ValueError("Hills not loaded yet.")
+
+        cv_min = self.cv_min
+        if self.cv_fes_range is None:
+            self.cv_fes_range = self.cv_max - self.cv_min
+        cv_fes_range = self.cv_fes_range
+        cvs = self.cvs
+        cv = self.hills.cv[time_min:time_max, :]
+        sigma = self.hills.sigma[time_min:time_max, :]
+        heights = self.hills.heights
+
+        def calculate_fes(index, cv, sigma, cv_min, cv_fes_range, heights):
+            dp2 = self._calculate_dp2(index, cv, sigma, cv_min, cv_fes_range)
 
             tmp = np.zeros(time_limit)
-            tmp[dp2 < 6.25] = self.hills.heights[dp2 < 6.25] * \
-                (np.exp(-dp2[dp2 < 6.25]) *
-                 1.00193418799744762399 - 0.00193418799744762399)
+            tmp[dp2 < 6.25] = heights[dp2 < 6.25] * \
+                (np.exp(-dp2[dp2 < 6.25]) * dp2_cutoff_a + dp2_cutoff_b)
             return index, -tmp.sum()
 
-        indices = list(np.ndindex(fes.shape))
         results = Parallel(n_jobs=n_workers)(
-            delayed(calculate_fes)(index) for index in indices
+            delayed(calculate_fes)(
+                index, cv, sigma, cv_min, cv_fes_range, heights
+            ) for index in np.ndindex(fes.shape)
         )
         if results is not None:
             for index, value in results:
                 fes[index] = value
             fes -= np.min(fes)
         self.fes = fes
         return fes
@@ -478,18 +583,19 @@
         cv_max = self.cv_max
 
         if int(nbins) != nbins:
             nbins = int(nbins)
             logger.info(
                 f"Number of bins must be an integer, it will be set to {nbins}.")
         if self.res % nbins != 0:
-            raise ValueError("Resolution of FES must be divisible by number of bins.")
+            raise ValueError(
+                "Resolution of FES must be divisible by number of bins.")
         if nbins > self.res/2:
             raise ValueError("Number of bins is too high.")
-        
+
         bin_size = int(self.res/nbins)
 
         for index in np.ndindex(tuple([nbins] * self.cvs)):
             # index serve as bin number
             _fes_slice = tuple(
                 slice(
                     index[i] * bin_size, (index[i] + 1) * bin_size
@@ -539,15 +645,16 @@
                         around[product_index] = np.inf
 
                     else:
                         around[product_index] = self.fes[tuple(
                             converted_index)]
 
                 if (around > bin_min).all():
-                    min_cv = (((min_cv_b+0.5)/self.res) * (cv_max-cv_min))+cv_min
+                    min_cv = (((min_cv_b+0.5)/self.res)
+                              * (cv_max-cv_min))+cv_min
                     local_minima = np.concatenate([
                         [np.round(bin_min, 6)], min_cv_b, np.round(min_cv, 6)
                     ])
                     if self.minima is None:
                         self.minima = local_minima
                     else:
                         self.minima = np.vstack((self.minima, local_minima))
@@ -644,25 +751,26 @@
                     xlabel=xlabel, ylabel=ylabel,
                     energy_unit=energy_unit,
                     **surface_params, **kwargs
                 )
             fig, ax = PlottingFES._plot2d(
                 self,
                 levels=levels, cmap=cmap, image_size=image_size, dpi=dpi,
-                xlabel=xlabel, ylabel=ylabel, **kwargs
+                xlabel=xlabel, ylabel=ylabel, 
+                energy_unit=energy_unit, **kwargs
             )
 
         else:
             raise ValueError("Only 1D and 2D FES are supported.")
 
         if png_name != None:
             fig.savefig(png_name)
 
         return fig, ax
-    
+
     def plot_minima(self, mark_color="white", png_name=None, **kwargs):
         fig, ax = PlottingFES.plot_minima(self, mark_color, **kwargs)
         if png_name is not None:
             fig.savefig(png_name)
         return fig, ax
 
 
@@ -720,24 +828,25 @@
                 subplot_kw={"projection": "3d"}
             )
             ax.plot_surface(X, Y, Z, cmap=cmap,  # type: ignore
                             rstride=rstride, cstride=cstride)
 
             if xlabel == None:
                 ax.set_xlabel(
-                    f'CV1 - {fes.cv_name[0]}', size=label_size) # type: ignore
+                    f'CV1 - {fes.cv_name[0]}', size=label_size)  # type: ignore
             else:
                 ax.set_xlabel(xlabel, size=label_size)
             if ylabel == None:
                 ax.set_ylabel(
-                    f'CV2 - {fes.cv_name[1]}', size=label_size) # type: ignore
+                    f'CV2 - {fes.cv_name[1]}', size=label_size)  # type: ignore
             else:
                 ax.set_ylabel(ylabel, size=label_size)
             if zlabel == None:
-                ax.set_zlabel(f'Free energy ({energy_unit})', size=label_size) # type: ignore
+                # type: ignore
+                ax.set_zlabel(f'Free energy ({energy_unit})', size=label_size)
             else:
                 ax.set_zlabel(zlabel, size=label_size)  # type: ignore
         else:
             raise ValueError(
                 f"Surface plot only works for FES with exactly two CVs, and this FES has {fes.cvs}."
             )
         return fig, ax
@@ -757,15 +866,15 @@
             figsize=(image_size[0], image_size[1]),
             dpi=dpi
         )
         X = np.linspace(fes.cv_min[0], fes.cv_max[0], fes.res)
         ax.plot(X, fes.fes)
         if xlabel == None:
             ax.set_xlabel(
-                f'CV1 - {fes.cv_name[0]}') # type: ignore
+                f'CV1 - {fes.cv_name[0]}')  # type: ignore
         else:
             ax.set_xlabel(xlabel)
         if ylabel == None:
             ax.set_ylabel(f'Free Energy ({energy_unit})')
         else:
             ax.set_ylabel(ylabel)
         return fig, ax
@@ -838,34 +947,34 @@
         Usage:
         ```python
         minima.plot()
         ```
         """
         if fes_obj.minima is None:
             raise ValueError("No minima found.")
-        
+
         fig, ax = fes_obj.plot(**kwargs)
 
         free_energy_range = fes_obj.fes.max() - fes_obj.fes.min()
 
         if fes_obj.cvs == 1:
             for m in range(len(fes_obj.minima.index)):
                 ax.text(
-                    float(fes_obj.minima.iloc[m, 3]), 
-                    float(fes_obj.minima.iloc[m, 1])+free_energy_range*0.05, 
+                    float(fes_obj.minima.iloc[m, 3]),
+                    float(fes_obj.minima.iloc[m, 1])+free_energy_range*0.05,
                     fes_obj.minima.iloc[m, 0],
-                    horizontalalignment='center', 
+                    horizontalalignment='center',
                     c=mark_color,
                     verticalalignment='bottom'
                 )
 
         elif fes_obj.cvs == 2:
             for m in range(len(fes_obj.minima.index)):
                 ax.text(
-                    float(fes_obj.minima.iloc[m, 4]), 
-                    float(fes_obj.minima.iloc[m, 5]), 
+                    float(fes_obj.minima.iloc[m, 4]),
+                    float(fes_obj.minima.iloc[m, 5]),
                     fes_obj.minima.iloc[m, 0],
                     horizontalalignment='center',
-                    verticalalignment='center', 
+                    verticalalignment='center',
                     c=mark_color
                 )
-        return fig, ax
+        return fig, ax
```

### Comparing `catflow-0.4.0/catflow/metad/hills.py` & `catflow-0.5.0/catflow/analyzer/metad/hills.py`

 * *Files identical despite different names*

### Comparing `catflow-0.4.0/catflow/metad/profile.py` & `catflow-0.5.0/catflow/analyzer/metad/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import pandas as pd
 
 from itertools import product
 from typing import List, Optional, Union
 from matplotlib.colors import Colormap
 
-from catflow.graph.plotting import canvas_style
-from catflow.metad.fes import FreeEnergySurface
-from catflow.metad.hills import Hills
+from catflow.analyzer.graph.plotting import canvas_style
+from catflow.analyzer.metad.fes import FreeEnergySurface
+from catflow.analyzer.metad.hills import Hills
 
 
 class FreeEnergyProfile:
     """
     A class to calculate and visualize the free energy profile of a metadynamics simulation.
     """
```

### Comparing `catflow-0.4.0/catflow/metad/string.py` & `catflow-0.5.0/catflow/analyzer/metad/string.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
 from scipy.interpolate import Rbf, griddata, interp1d, RegularGridInterpolator
 from typing import Literal, List, Union, Tuple, Optional
 
 from catflow.utils import logger
-from catflow.metad.fes import FreeEnergySurface
+from catflow.analyzer.metad.fes import FreeEnergySurface
 
 
 class StringMethod:
     """
     Class containing methods to compute the minimum energy path between two
     points on an energy landscape $V$.
```

### Comparing `catflow-0.4.0/catflow/structure/cluster.py` & `catflow-0.5.0/catflow/analyzer/structure/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import Optional
 from scipy.spatial import distance
 from scipy.optimize import curve_fit
 from MDAnalysis import Universe
 
 
-from catflow.structure.lindemann_index import LindemannIndex
+from catflow.analyzer.structure.lindemann_index import LindemannIndex
 
 
 class Cluster(object):
     def __init__(self, path=None, **kwargs):
         self.path = path
         self.kwargs = kwargs
         if self.path is not None:
```

### Comparing `catflow-0.4.0/catflow/structure/coordination_number.py` & `catflow-0.5.0/catflow/analyzer/structure/coordination_number.py`

 * *Files identical despite different names*

### Comparing `catflow-0.4.0/catflow/structure/dynamic_selection.py` & `catflow-0.5.0/catflow/analyzer/structure/dynamic_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         ValueError: If `axis` is not "x", "y", or "z".
 
     Notes:
         This class is a subclass of `MDAnalysis.analysis.base.AnalysisBase`.
 
     Examples:
         >>> import MDAnalysis as mda
-        >>> from catflow.structure.dynamic_selection import AxisMaxDistance
+        >>> from catflow.analyzer.structure.dynamic_selection import AxisMaxDistance
         >>> u = mda.Universe("system.gro", "system.trr")
         >>> ag1 = u.select_atoms("protein")
         >>> ag2 = u.select_atoms("resname LIG")
         >>> analysis = AxisMaxDistance(ag1, ag2, axis="x", box=u.dimensions)
         >>> analysis.run()
         >>> max_distances = analysis.results.distances
     """
```

### Comparing `catflow-0.4.0/catflow/structure/lindemann_index.py` & `catflow-0.5.0/catflow/analyzer/structure/lindemann_index.py`

 * *Files identical despite different names*

### Comparing `catflow-0.4.0/catflow/tesla/ai2_kit/exploration.py` & `catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/exploration.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 from typing import List
 
 import numpy as np
 
 from catflow.utils.log_factory import logger
 from catflow.utils.lammps import lammps_variable_parser
-from catflow.tesla.base.exploration import ExplorationAnalyzer
-from catflow.tesla.ai2_kit.task import CllAnalyzer
+from catflow.analyzer.tesla.base.exploration import ExplorationAnalyzer
+from catflow.analyzer.tesla.ai2_kit.task import CllAnalyzer
 
 
 def read_model_deviation(model_devi_path: Path):
     model_devi_path = model_devi_path.resolve()
     try:
         steps = np.loadtxt(model_devi_path, usecols=0)
         max_devi_f = np.loadtxt(model_devi_path, usecols=4)
```

### Comparing `catflow-0.4.0/catflow/tesla/ai2_kit/labeling.py` & `catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/labeling.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 
-from catflow.tesla.base.labeling import LabelingAnalyzer
-from catflow.tesla.ai2_kit.task import CllAnalyzer
-from catflow.graph.plotting import canvas_style
+from catflow.analyzer.tesla.base.labeling import LabelingAnalyzer
+from catflow.analyzer.tesla.ai2_kit.task import CllAnalyzer
+from catflow.analyzer.graph.plotting import canvas_style
 
 
 class CllLabelingAnalyzer(LabelingAnalyzer, CllAnalyzer):
 
     def get_fp_tasks(self, iteration: int = 0):
         n_iter = self._iteration_dir(iteration=iteration)
         stage_path = self.dp_task.path / n_iter / 'label-vasp/tasks'
```

### Comparing `catflow-0.4.0/catflow/tesla/ai2_kit/task.py` & `catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import Union, List, Dict, Optional
 
 from ai2_kit.core.util import load_yaml_files
 from ai2_kit.core.checkpoint import set_checkpoint_file
 from ai2_kit.workflow.cll_mlp import CllWorkflowConfig
 
-from catflow.tesla.base.task import BaseTask, BaseAnalyzer
+from catflow.analyzer.tesla.base.task import BaseTask, BaseAnalyzer
 
 
 class CllTask(BaseTask):
     """CllTask is a class reading a ai2-kit directory, where the Cll-Workflow run.
     """
 
     def __init__(
@@ -24,15 +24,15 @@
 
         Args:
             path (str): The path of the tesla task.
             deepmd_version (str): DeepMD-kit version used. Default: 2.0.
         """
         super().__init__(path)
         config_data = load_yaml_files(*config_files)
-        self.config = CllWorkflowConfig.parse_obj(config_data)   
+        self.config = CllWorkflowConfig.model_validate(config_data)   
 
     @classmethod
     def from_dict(cls, dp_task_dict: dict):
         return cls(**dp_task_dict)
 
 
 class CllAnalyzer(BaseAnalyzer):
```

### Comparing `catflow-0.4.0/catflow/tesla/ai2_kit/training.py` & `catflow-0.5.0/catflow/analyzer/tesla/ai2_kit/training.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 
 import numpy as np
 from matplotlib import pyplot as plt
 
 from catflow.utils import logger
-from catflow.graph.plotting import canvas_style
-from catflow.tesla.base.training import TrainingAnalyzer
-from catflow.tesla.ai2_kit.task import CllAnalyzer, CllTask
+from catflow.analyzer.graph.plotting import canvas_style
+from catflow.analyzer.tesla.base.training import TrainingAnalyzer
+from catflow.analyzer.tesla.ai2_kit.task import CllAnalyzer, CllTask
 
 
 class CllTrainingAnalyzer(TrainingAnalyzer, CllAnalyzer):
     """Analyzer for training tasks.
     """
 
     def get_lcurve_path(self, iteration: int, model=0) -> Path:
```

### Comparing `catflow-0.4.0/catflow/tesla/base/exploration.py` & `catflow-0.5.0/catflow/analyzer/tesla/base/exploration.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from matplotlib import pyplot as plt
 
 from catflow.utils.log_factory import logger
-from catflow.graph.plotting import canvas_style, square_grid
-from catflow.tesla.base.task import BaseAnalyzer
+from catflow.analyzer.graph.plotting import canvas_style, square_grid
+from catflow.analyzer.tesla.base.task import BaseAnalyzer
 
 
 def read_model_deviation(model_devi_path: Path):
     model_devi_path = model_devi_path.resolve()
     try:
         steps = np.loadtxt(model_devi_path, usecols=0)
         max_devi_f = np.loadtxt(model_devi_path, usecols=4)
@@ -247,15 +247,15 @@
             f_trust_hi (float, optional): The higher limit of max_deviation_force. Defaults to 0.3.
             select (str, optional): Choose which param selected as plot zone. Defaults to None.
             select_value (str, optional): The dependence of `select`. 
                 Different from `group_by`, please pass only one number. Defaults to None.
             kwargs (_type_, optional): Additional keyword arguments. Include other params, such as:
                 `temps`: please use the value of `group_by`, whose default input is `"temps"`.
                 `label_unit`: the unit of `select_value`, such as 'Å'.
-                Parameters of `canvas_style`: please refer to `catflow.graph.plotting.canvas_style`.
+                Parameters of `canvas_style`: please refer to `catflow.analyzer.graph.plotting.canvas_style`.
 
         Returns:
             Figure: A plot for different desired values.
         """
 
         num_item, plot_items = self._convert_group_by(group_by, **kwargs)
```

### Comparing `catflow-0.4.0/catflow/tesla/base/labeling.py` & `catflow-0.5.0/catflow/analyzer/tesla/base/labeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import List, Literal
 
 from ase.io import read
 from matplotlib import pyplot as plt
 
 from catflow.utils.log_factory import logger
 from catflow.utils.log_factory import LogFactory
-from catflow.tesla.base.task import BaseTask, BaseAnalyzer
-from catflow.graph.plotting import canvas_style
+from catflow.analyzer.tesla.base.task import BaseTask, BaseAnalyzer
+from catflow.analyzer.graph.plotting import canvas_style
 
 
 
 class LabelingAnalyzer(BaseAnalyzer):
 
     def __init__(
         self, dp_task: BaseTask,
```

### Comparing `catflow-0.4.0/catflow/tesla/base/task.py` & `catflow-0.5.0/catflow/analyzer/tesla/base/task.py`

 * *Files identical despite different names*

### Comparing `catflow-0.4.0/catflow/tesla/base/training.py` & `catflow-0.5.0/catflow/analyzer/tesla/base/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import numpy as np
 from matplotlib import pyplot as plt
 
 from catflow.utils import logger
-from catflow.graph.plotting import canvas_style
-from catflow.tesla.base.task import BaseAnalyzer, BaseTask
+from catflow.analyzer.graph.plotting import canvas_style
+from catflow.analyzer.tesla.base.task import BaseAnalyzer, BaseTask
 
 
 class TrainingAnalyzer(BaseAnalyzer):
     """Analyzer for training tasks.
     """
 
     def __init__(
```

### Comparing `catflow-0.4.0/catflow/tesla/dpgen/exploration.py` & `catflow-0.5.0/catflow/analyzer/tesla/dpgen/exploration.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from typing import Optional, Union, List
 from matplotlib.figure import Figure
 
 import numpy as np
 from matplotlib import pyplot as plt
 
 from catflow.utils.log_factory import logger
-from catflow.graph.plotting import canvas_style, square_grid
-from catflow.tesla.base.exploration import ExplorationAnalyzer, PlottingExploartion
-from catflow.tesla.dpgen.task import DPAnalyzer
+from catflow.analyzer.graph.plotting import canvas_style, square_grid
+from catflow.analyzer.tesla.base.exploration import ExplorationAnalyzer, PlottingExploartion
+from catflow.analyzer.tesla.dpgen.task import DPAnalyzer
 
 
 class DPExplorationAnalyzer(ExplorationAnalyzer, DPAnalyzer):
     """Analyzer for DP exploration tasks."""
 
     def _iteration_tasks(self, iteration) -> List[Path]:
         n_iter = self._iteration_dir(control_step=2, iteration=iteration)
@@ -91,15 +91,15 @@
                 Should be corresponding to keys in model_devi_job. Defaults to 'temps'.
             select (str, optional): Choose which param selected as plot zone. Defaults to None.
             select_value (str, optional): The dependence of `select`. 
                 Different from `group_by`, please pass only one number. Defaults to None.
             kwargs (_type_, optional): Additional keyword arguments. Include other params, such as:
                 `temps`: please use the value of `group_by`, whose default input is `"temps"`.
                 `label_unit`: the unit of `select_value`, such as 'Å'.
-                Parameters of `canvas_style`: please refer to `catflow.graph.plotting.canvas_style`.
+                Parameters of `canvas_style`: please refer to `catflow.analyzer.graph.plotting.canvas_style`.
 
         Returns:
             Figure: A plot for different desired values.
         """
         if f_trust_hi is None:
             f_trust_hi = self._read_model_devi_trust_level(
                 "model_devi_f_trust_hi", iteration)
```

### Comparing `catflow-0.4.0/catflow/tesla/dpgen/labeling.py` & `catflow-0.5.0/catflow/analyzer/tesla/dpgen/labeling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
-from catflow.tesla.base.labeling import LabelingAnalyzer
-from catflow.tesla.dpgen.task import DPTask, DPAnalyzer
+from catflow.analyzer.tesla.base.labeling import LabelingAnalyzer
+from catflow.analyzer.tesla.dpgen.task import DPTask, DPAnalyzer
 
 
 class DPLabelingAnalyzer(LabelingAnalyzer, DPAnalyzer):
 
     def __init__(
         self, 
         dp_task: DPTask,
```

### Comparing `catflow-0.4.0/catflow/tesla/dpgen/task.py` & `catflow-0.5.0/catflow/analyzer/tesla/dpgen/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from pathlib import Path
 from typing import Optional
 
-from catflow.tesla.base.task import BaseTask, BaseAnalyzer
+from catflow.analyzer.tesla.base.task import BaseTask, BaseAnalyzer
 
 
 class DPTask(BaseTask):
     """DPTask is a class reading a DP-GEN directory, where the DP-GEN task run.
     """
 
     def __init__(
```

### Comparing `catflow-0.4.0/catflow/tesla/dpgen/training.py` & `catflow-0.5.0/catflow/analyzer/tesla/dpgen/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 from typing import Optional
 
 import numpy as np
 from matplotlib import pyplot as plt
 
 from catflow.utils import logger
-from catflow.graph.plotting import canvas_style
-from catflow.tesla.base.training import TrainingAnalyzer
-from catflow.tesla.dpgen.task import DPAnalyzer
+from catflow.analyzer.graph.plotting import canvas_style
+from catflow.analyzer.tesla.base.training import TrainingAnalyzer
+from catflow.analyzer.tesla.dpgen.task import DPAnalyzer
 
 class DPTrainingAnalyzer(TrainingAnalyzer, DPAnalyzer):
     """Analyzer for training tasks.
     """
 
     def get_lcurve_path(self, iteration: int, model=0) -> Path:
         _iteration_dir = self._iteration_dir(iteration=iteration)
```

### Comparing `catflow-0.4.0/catflow/utils/log_factory.py` & `catflow-0.5.0/catflow/utils/log_factory.py`

 * *Files identical despite different names*

### Comparing `catflow-0.4.0/pyproject.toml` & `catflow-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 [tool.poetry]
 name = "catflow"
-version = "0.4.0"
+version = "0.5.0"
 description = "Analyzing tool for deep learning based chemical research."
 authors = ["Cloudac7 <scottryuu@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.md"
-repository = "https://github.com/cloudac7/catflow"
+repository = "https://github.com/chenggroup/CatFlow"
 packages = [{include = "catflow"}]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.8"
 ase = "^3.21.1"
+click = "*"
+dpdata = "*"
+dpdispatcher = "^0.5.6"
+dpgen = "^0.11.1"
+dynaconf = "*"
 matplotlib = "^3.7.1"
 numpy = "<1.24,>=1.18"
 pandas = "^1.3.3"
 dscribe = "^1.2.2"
 mdanalysis = "^2.2"
 scipy = "^1.10.1"
 seaborn = "^0.12.2"
 pymatgen = "^2023.5.10"
 ai2-kit = ">=0.9.0"
+fire = "^0.5.0"
+ruamel-yaml = ">=0.17.21,<0.18.0"
+h5py = "^3.10.0"
 
 [tool.poetry.group.test.dependencies]
 flake8 = "*"
 pytest = "*"
 pytest-mock = "*"
 pytest-datadir = "*"
 coverage = "*"
@@ -35,12 +43,12 @@
 mike = "*"
 mkdocs-gen-files = "*"
 mkdocs-literate-nav = "^0.5.0"
 mkdocs-section-index = "*"
 mkdocs-jupyter = "^0.24.2"
 
 [tool.poetry.scripts]
-catflow = 'catflow.cmdline.base:cli'
+catflow = 'catflow.cmdline.base:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

