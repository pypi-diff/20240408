# Comparing `tmp/neighpy-0.1.2.tar.gz` & `tmp/neighpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neighpy-0.1.2.tar", max compression
+gzip compressed data, was "neighpy-0.1.3.tar", max compression
```

## Comparing `neighpy-0.1.2.tar` & `neighpy-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2354 2024-02-20 00:24:27.038040 neighpy-0.1.2/README.md
--rw-r--r--   0        0        0      100 2024-02-20 00:24:27.054040 neighpy-0.1.2/neighpy/__init__.py
--rw-r--r--   0        0        0     2465 2024-02-20 00:24:27.054040 neighpy-0.1.2/neighpy/_mcintegrals.py
--rw-r--r--   0        0        0      125 2024-02-20 00:24:41.478363 neighpy-0.1.2/neighpy/_version.py
--rw-r--r--   0        0        0    10604 2024-02-20 00:24:27.054040 neighpy-0.1.2/neighpy/appraise.py
--rw-r--r--   0        0        0     5438 2024-02-20 00:24:27.054040 neighpy-0.1.2/neighpy/search.py
--rw-r--r--   0        0        0     1539 2024-02-20 00:24:41.478363 neighpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 neighpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35420 2024-04-08 01:27:01.766051 neighpy-0.1.3/LICENSE.rst
+-rw-r--r--   0        0        0     2445 2024-04-08 01:27:01.766051 neighpy-0.1.3/README.md
+-rw-r--r--   0        0        0      100 2024-04-08 01:27:01.810050 neighpy-0.1.3/neighpy/__init__.py
+-rw-r--r--   0        0        0     2465 2024-04-08 01:27:01.810050 neighpy-0.1.3/neighpy/_mcintegrals.py
+-rw-r--r--   0        0        0      125 2024-04-08 01:27:16.037911 neighpy-0.1.3/neighpy/_version.py
+-rw-r--r--   0        0        0    10604 2024-04-08 01:27:01.810050 neighpy-0.1.3/neighpy/appraise.py
+-rw-r--r--   0        0        0     5472 2024-04-08 01:27:01.810050 neighpy-0.1.3/neighpy/search.py
+-rw-r--r--   0        0        0     1624 2024-04-08 01:27:16.037911 neighpy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 neighpy-0.1.3/PKG-INFO
```

### Comparing `neighpy-0.1.2/README.md` & `neighpy-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![test](https://github.com/auggiemarignier/neighpy/actions/workflows/tests.yaml/badge.svg)](https://github.com/auggiemarignier/neighpy/actions/workflows/tests.yaml) [![docs](https://readthedocs.org/projects/neighpy/badge/?version=latest)](https://neighpy.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/neighpy.svg)](https://badge.fury.io/py/neighpy) [![test](https://github.com/auggiemarignier/neighpy/actions/workflows/tests.yaml/badge.svg)](https://github.com/auggiemarignier/neighpy/actions/workflows/tests.yaml) [![docs](https://readthedocs.org/projects/neighpy/badge/?version=latest)](https://neighpy.readthedocs.io/en/latest/?badge=latest)
 
 # neighpy
 
 ``neighphy`` is a Python implementation of the Neighbourhood Algorithm for the optimisation and appraisal of high-dimensional loss surfaces.
 First presented in two papers by M. Sambridge at the Australian National University in 1999, it has since been widely used, particularly in the geophysical community, for the optimisation of complex, high-dimensional functions.
 
 This implementation hopes to replace the original Fortran code with a more modern, user-friendly and flexible Python package.
@@ -55,8 +55,8 @@
 
 ## Licence
 
 This code is distributed under a [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.en.html).
 
 ## Contributing
 
-If you have any questions, please to open an issue in this repository.
+If you have any questions, please to open an issue in this repository.
```

### Comparing `neighpy-0.1.2/neighpy/_mcintegrals.py` & `neighpy-0.1.3/neighpy/_mcintegrals.py`

 * *Files identical despite different names*

### Comparing `neighpy-0.1.2/neighpy/appraise.py` & `neighpy-0.1.3/neighpy/appraise.py`

 * *Files identical despite different names*

### Comparing `neighpy-0.1.2/neighpy/search.py` & `neighpy-0.1.3/neighpy/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         self.samples = np.zeros((self.nt, self.nd))
         self.objectives = np.full(
             self.nt, np.inf
         )  # start with inf since we want to minimize
         self._current_best_ind = 0
 
-    def run(self) -> None:
+    def run(self, parallel=True) -> None:
         """
         Run the Direct Search.
 
         Populates the following attributes:
 
         - **samples** (`NDArray`) - samples generated by the direct search.
         - **objectives** (`NDArray`) - objective function values for each sample.
@@ -68,15 +68,15 @@
 
         # main optimisation loop
         for _ in tqdm(range(self.n), desc="NAI - Optimisation Loop"):
             inds = self._get_best_indices()
             self._current_best_ind = inds[0]
             cells_to_resample = self.samples[inds]
 
-            new_samples = Parallel(n_jobs=self.nr)(
+            new_samples = Parallel(n_jobs=self.nr if parallel else 1)(
                 delayed(self._random_walk_in_voronoi)(cell, k)
                 for k, cell in zip(inds, cells_to_resample)
             )
             self._update_ensemble(np.concatenate(new_samples))
 
     def _initial_random_search(self) -> NDArray:
         return np.random.uniform(
```

### Comparing `neighpy-0.1.2/pyproject.toml` & `neighpy-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neighpy"
-version = "0.1.2"
+version = "0.1.3"
 description = "Neighbourhood Algorithm in Python"
 authors = ["auggiemarignier <augustin.marignier@anu.edu.au>"]
 homepage = "https://github.com/auggiemarignier/neighpy"
 repository = "https://github.com/auggiemarignier/neighpy"
 license = "GPL-3.0-or-later"
 documentation = "https://neighpy.readthedocs.io/en/latest/index.html"
 readme = "README.md"
@@ -29,14 +29,16 @@
 [tool.poetry.group.examples]
 optional = true
 
 [tool.poetry.group.examples.dependencies]
 matplotlib = ">=3.5"
 scipy = ">=1.8"
 jupyter = "^1.0.0"
+geo-espresso = "^0.3.11"
+seislib = {git = "https://github.com/fmagrini/seislib.git"}
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "<6"
 sphinx-book-theme = ">1.0.0"
```

### Comparing `neighpy-0.1.2/PKG-INFO` & `neighpy-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neighpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Neighbourhood Algorithm in Python
 Home-page: https://github.com/auggiemarignier/neighpy
 License: GPL-3.0-or-later
 Author: auggiemarignier
 Author-email: augustin.marignier@anu.edu.au
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -17,15 +17,15 @@
 Requires-Dist: joblib (>=1.3.2,<2.0.0)
 Requires-Dist: numpy (>=1.22)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Documentation, https://neighpy.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/auggiemarignier/neighpy
 Description-Content-Type: text/markdown
 
-[![test](https://github.com/auggiemarignier/neighpy/actions/workflows/tests.yaml/badge.svg)](https://github.com/auggiemarignier/neighpy/actions/workflows/tests.yaml) [![docs](https://readthedocs.org/projects/neighpy/badge/?version=latest)](https://neighpy.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/neighpy.svg)](https://badge.fury.io/py/neighpy) [![test](https://github.com/auggiemarignier/neighpy/actions/workflows/tests.yaml/badge.svg)](https://github.com/auggiemarignier/neighpy/actions/workflows/tests.yaml) [![docs](https://readthedocs.org/projects/neighpy/badge/?version=latest)](https://neighpy.readthedocs.io/en/latest/?badge=latest)
 
 # neighpy
 
 ``neighphy`` is a Python implementation of the Neighbourhood Algorithm for the optimisation and appraisal of high-dimensional loss surfaces.
 First presented in two papers by M. Sambridge at the Australian National University in 1999, it has since been widely used, particularly in the geophysical community, for the optimisation of complex, high-dimensional functions.
 
 This implementation hopes to replace the original Fortran code with a more modern, user-friendly and flexible Python package.
@@ -79,7 +79,8 @@
 ## Licence
 
 This code is distributed under a [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.en.html).
 
 ## Contributing
 
 If you have any questions, please to open an issue in this repository.
+
```
