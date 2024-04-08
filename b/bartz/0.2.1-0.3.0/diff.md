# Comparing `tmp/bartz-0.2.1.tar.gz` & `tmp/bartz-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bartz-0.2.1.tar", max compression
+gzip compressed data, was "bartz-0.3.0.tar", max compression
```

## Comparing `bartz-0.2.1.tar` & `bartz-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2024-03-19 21:21:09.679092 bartz-0.2.1/LICENSE
--rw-r--r--   0        0        0      668 2024-03-31 07:38:25.385557 bartz-0.2.1/README.md
--rw-r--r--   0        0        0     3604 2024-03-31 17:16:07.269043 bartz-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    15801 2024-03-25 02:06:56.560650 bartz-0.2.1/src/bartz/BART.py
--rw-r--r--   0        0        0     1448 2024-03-31 06:56:42.369415 bartz-0.2.1/src/bartz/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 17:17:17.495575 bartz-0.2.1/src/bartz/_version.py
--rw-r--r--   0        0        0     5314 2024-03-25 19:59:40.459274 bartz-0.2.1/src/bartz/debug.py
--rw-r--r--   0        0        0     8291 2024-03-31 06:36:22.218843 bartz-0.2.1/src/bartz/grove.py
--rw-r--r--   0        0        0    10996 2024-03-31 07:46:16.755065 bartz-0.2.1/src/bartz/jaxext.py
--rw-r--r--   0        0        0     7701 2024-03-28 21:57:53.726888 bartz-0.2.1/src/bartz/mcmcloop.py
--rw-r--r--   0        0        0    39450 2024-03-31 17:01:50.025545 bartz-0.2.1/src/bartz/mcmcstep.py
--rw-r--r--   0        0        0     4634 2024-03-25 22:41:01.636106 bartz-0.2.1/src/bartz/prepcovars.py
--rw-r--r--   0        0        0     1490 1970-01-01 00:00:00.000000 bartz-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-03-19 21:21:09.679092 bartz-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3678 2024-04-08 04:46:18.271175 bartz-0.3.0/README.md
+-rw-r--r--   0        0        0     3643 2024-04-08 06:08:10.021098 bartz-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    16862 2024-04-08 05:01:06.834203 bartz-0.3.0/src/bartz/BART.py
+-rw-r--r--   0        0        0     1448 2024-03-31 06:56:42.369415 bartz-0.3.0/src/bartz/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-08 06:08:57.994671 bartz-0.3.0/src/bartz/_version.py
+-rw-r--r--   0        0        0     5314 2024-03-25 19:59:40.459274 bartz-0.3.0/src/bartz/debug.py
+-rw-r--r--   0        0        0     8500 2024-04-08 05:03:57.628481 bartz-0.3.0/src/bartz/grove.py
+-rw-r--r--   0        0        0    12033 2024-04-08 05:07:50.118723 bartz-0.3.0/src/bartz/jaxext.py
+-rw-r--r--   0        0        0     7634 2024-04-08 05:09:44.969044 bartz-0.3.0/src/bartz/mcmcloop.py
+-rw-r--r--   0        0        0    54221 2024-04-08 05:51:36.476838 bartz-0.3.0/src/bartz/mcmcstep.py
+-rw-r--r--   0        0        0     5818 2024-04-08 05:55:33.596178 bartz-0.3.0/src/bartz/prepcovars.py
+-rw-r--r--   0        0        0     4500 1970-01-01 00:00:00.000000 bartz-0.3.0/PKG-INFO
```

### Comparing `bartz-0.2.1/LICENSE` & `bartz-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bartz-0.2.1/pyproject.toml` & `bartz-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
-# 
+#
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
-# 
+#
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "bartz"
-version = "0.2.1"
+version = "0.3.0"
 description = "A JAX implementation of BART"
 authors = ["Giacomo Petrillo <info@giacomopetrillo.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Gattocrucco/bartz"
 packages = [
     { include = "bartz", from = "src" },
@@ -50,14 +50,16 @@
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.22.2"
 matplotlib = "^3.8.3"
 appnope = "^0.1.4"
 tomli = "^2.0.1"
 packaging = "^24.0"
+xgboost = "^2.0.3"
+pre-commit = "^3.7.0"
 
 [tool.poetry.group.test.dependencies]
 coverage = "^7.4.3"
 pytest = "^8.1.1"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^7.2.6"
```

### Comparing `bartz-0.2.1/src/bartz/BART.py` & `bartz-0.3.0/src/bartz/BART.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
-# 
+#
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
-# 
+#
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
@@ -45,14 +45,17 @@
     ----------
     x_train : array (p, n) or DataFrame
         The training predictors.
     y_train : array (n,) or Series
         The training responses.
     x_test : array (p, m) or DataFrame, optional
         The test predictors.
+    usequants : bool, default False
+        Whether to use predictors quantiles instead of a uniform grid to bin
+        predictors.
     sigest : float, optional
         An estimate of the residual standard deviation on `y_train`, used to
         set `lamda`. If not specified, it is estimated by linear regression.
         If `y_train` has less than two elements, it is set to 1. If n <= p, it
         is set to the variance of `y_train`. Ignored if `lamda` is specified.
     sigdf : int, default 3
         The degrees of freedom of the scaled inverse-chisquared prior on the
@@ -78,18 +81,24 @@
         not specified, it is set based on `sigest` and `sigquant`.
     offset : float, optional
         The prior mean of the latent mean function. If not specified, it is set
         to the mean of `y_train`. If `y_train` is empty, it is set to 0.
     ntree : int, default 200
         The number of trees used to represent the latent mean function.
     numcut : int, default 255
-        The maximum number of cutpoints to use for binning the predictors. Each
-        predictor is binned such that its distribution in `x_train` is
-        approximately uniform across bins. The number of bins is at most the
-        number of unique values appearing in `x_train`, or ``numcut + 1``.
+        If `usequants` is `False`: the exact number of cutpoints used to bin the
+        predictors, ranging between the minimum and maximum observed values
+        (excluded).
+
+        If `usequants` is `True`: the maximum number of cutpoints to use for
+        binning the predictors. Each predictor is binned such that its
+        distribution in `x_train` is approximately uniform across bins. The
+        number of bins is at most the number of unique values appearing in
+        `x_train`, or ``numcut + 1``.
+
         Before running the algorithm, the predictors are compressed to the
         smallest integer type that fits the bin indices, so `numcut` is best set
         to the maximum value of an unsigned integer type.
     ndpost : int, default 1000
         The number of MCMC samples to save, after burn-in.
     nskip : int, default 100
         The number of initial MCMC samples to discard as burn-in.
@@ -122,36 +131,43 @@
         The prior harmonic mean of the error variance.
     sigest : float or None
         The estimated standard deviation of the error used to set `lamda`.
     ntree : int
         The number of trees.
     maxdepth : int
         The maximum depth of the trees.
+    initkw : dict
+        Additional arguments passed to `mcmcstep.init`.
 
     Methods
     -------
     predict
 
     Notes
     -----
-    This interface imitates the function `gbart` from the R package `BART
+    This interface imitates the function ``gbart`` from the R package `BART
     <https://cran.r-project.org/package=BART>`_, but with these differences:
 
     - If `x_train` and `x_test` are matrices, they have one predictor per row
       instead of per column.
+    - If ``usequants=False``, R BART switches to quantiles anyway if there are
+      less predictor values than the required number of bins, while bartz
+      always follows the specification.
     - The error variance parameter is called `lamda` instead of `lambda`.
-    - `usequants` is always `True`.
     - `rm_const` is always `False`.
     - The default `numcut` is 255 instead of 100.
     - A lot of functionality is missing (variable selection, discrete response).
     - There are some additional attributes, and some missing.
+
+    The linear regression used to set `sigest` adds an intercept.
     """
 
     def __init__(self, x_train, y_train, *,
         x_test=None,
+        usequants=False,
         sigest=None,
         sigdf=3,
         sigquant=0.9,
         k=2,
         power=2,
         base=0.95,
         maxdepth=6,
@@ -160,32 +176,33 @@
         ntree=200,
         numcut=255,
         ndpost=1000,
         nskip=100,
         keepevery=1,
         printevery=100,
         seed=0,
+        initkw={},
         ):
 
         x_train, x_train_fmt = self._process_predictor_input(x_train)
-        
+
         y_train, y_train_fmt = self._process_response_input(y_train)
         self._check_same_length(x_train, y_train)
-        
+
         offset = self._process_offset_settings(y_train, offset)
         scale = self._process_scale_settings(y_train, k)
         lamda, sigest = self._process_noise_variance_settings(x_train, y_train, sigest, sigdf, sigquant, lamda, offset)
 
-        splits, max_split = self._determine_splits(x_train, numcut)
+        splits, max_split = self._determine_splits(x_train, usequants, numcut)
         x_train = self._bin_predictors(x_train, splits)
 
         y_train = self._transform_input(y_train, offset, scale)
         lamda_scaled = lamda / (scale * scale)
 
-        mcmc_state = self._setup_mcmc(x_train, y_train, max_split, lamda_scaled, sigdf, power, base, maxdepth, ntree)
+        mcmc_state = self._setup_mcmc(x_train, y_train, max_split, lamda_scaled, sigdf, power, base, maxdepth, ntree, initkw)
         final_state, burnin_trace, main_trace = self._run_mcmc(mcmc_state, ndpost, nskip, keepevery, printevery, seed)
 
         sigma = self._extract_sigma(main_trace, scale)
         first_sigma = self._extract_sigma(burnin_trace, scale)
 
         self.offset = offset
         self.scale = scale
@@ -275,15 +292,18 @@
             if sigest is not None:
                 sigest2 = sigest * sigest
             elif y_train.size < 2:
                 sigest2 = 1
             elif y_train.size <= x_train.shape[0]:
                 sigest2 = jnp.var(y_train - offset)
             else:
-                _, chisq, rank, _ = jnp.linalg.lstsq(x_train.T, y_train - offset)
+                x_centered = x_train.T - x_train.mean(axis=1)
+                y_centered = y_train - y_train.mean()
+                    # centering is equivalent to adding an intercept column
+                _, chisq, rank, _ = jnp.linalg.lstsq(x_centered, y_centered)
                 chisq = chisq.squeeze(0)
                 dof = len(y_train) - rank
                 sigest2 = chisq / dof
             alpha = sigdf / 2
             invchi2 = jaxext.scipy.stats.invgamma.ppf(sigquant, alpha) / 2
             invchi2rid = invchi2 * sigdf
             return sigest2 / invchi2rid, jnp.sqrt(sigest2)
@@ -301,41 +321,46 @@
     def _process_scale_settings(y_train, k):
         if y_train.size < 2:
             return 1
         else:
             return (y_train.max() - y_train.min()) / (2 * k)
 
     @staticmethod
-    def _determine_splits(x_train, numcut):
-        return prepcovars.quantilized_splits_from_matrix(x_train, numcut + 1)
+    def _determine_splits(x_train, usequants, numcut):
+        if usequants:
+            return prepcovars.quantilized_splits_from_matrix(x_train, numcut + 1)
+        else:
+            return prepcovars.uniform_splits_from_matrix(x_train, numcut + 1)
 
     @staticmethod
     def _bin_predictors(x, splits):
         return prepcovars.bin_predictors(x, splits)
 
     @staticmethod
     def _transform_input(y, offset, scale):
         return (y - offset) / scale
 
     @staticmethod
-    def _setup_mcmc(x_train, y_train, max_split, lamda, sigdf, power, base, maxdepth, ntree):
+    def _setup_mcmc(x_train, y_train, max_split, lamda, sigdf, power, base, maxdepth, ntree, initkw):
         depth = jnp.arange(maxdepth - 1)
         p_nonterminal = base / (1 + depth).astype(float) ** power
         sigma2_alpha = sigdf / 2
         sigma2_beta = lamda * sigma2_alpha
-        return mcmcstep.init(
+        kw = dict(
             X=x_train,
             y=y_train,
             max_split=max_split,
             num_trees=ntree,
             p_nonterminal=p_nonterminal,
             sigma2_alpha=sigma2_alpha,
             sigma2_beta=sigma2_beta,
             min_points_per_leaf=5,
         )
+        kw.update(initkw)
+        return mcmcstep.init(**kw)
 
     @staticmethod
     def _run_mcmc(mcmc_state, ndpost, nskip, keepevery, printevery, seed):
         if isinstance(seed, jax.Array) and jnp.issubdtype(seed.dtype, jax.dtypes.prng_key):
             key = seed
         else:
             key = jax.random.key(seed)
@@ -350,15 +375,15 @@
     def _transform_output(y, offset, scale):
         return offset + scale * y
 
     @staticmethod
     def _extract_sigma(trace, scale):
         return scale * jnp.sqrt(trace['sigma2'])
 
-    
+
     def _show_tree(self, i_sample, i_tree, print_all=False):
         from . import debug
         trace = self._main_trace
         leaf_tree = trace['leaf_trees'][i_sample, i_tree]
         var_tree = trace['var_trees'][i_sample, i_tree]
         split_tree = trace['split_trees'][i_sample, i_tree]
         debug.print_tree(leaf_tree, var_tree, split_tree, print_all)
```

### Comparing `bartz-0.2.1/src/bartz/__init__.py` & `bartz-0.3.0/src/bartz/__init__.py`

 * *Files identical despite different names*

### Comparing `bartz-0.2.1/src/bartz/debug.py` & `bartz-0.3.0/src/bartz/debug.py`

 * *Files identical despite different names*

### Comparing `bartz-0.2.1/src/bartz/grove.py` & `bartz-0.3.0/src/bartz/grove.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
-# 
+#
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
-# 
+#
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
@@ -110,15 +110,15 @@
     )
 
     def loop(carry, _):
         leaf_found, index = carry
 
         split = split_tree[index]
         var = var_tree[index]
-        
+
         leaf_found |= split == 0
         child_index = (index << 1) + (x[var] >= split)
         index = jnp.where(leaf_found, index, child_index)
 
         return (leaf_found, index), None
 
     depth = tree_depth(var_tree)
@@ -143,44 +143,49 @@
     Returns
     -------
     indices : array (m, n)
         The indices of the leaves.
     """
     return traverse_tree(X, var_trees, split_trees)
 
-def evaluate_forest(X, leaf_trees, var_trees, split_trees, dtype):
+def evaluate_forest(X, leaf_trees, var_trees, split_trees, dtype=None, sum_trees=True):
     """
     Evaluate a ensemble of trees at an array of points.
 
     Parameters
     ----------
     X : array (p, n)
         The coordinates to evaluate the trees at.
     leaf_trees : array (m, 2 ** d)
         The leaf values of the tree or forest. If the input is a forest, the
         first axis is the tree index, and the values are summed.
     var_trees : array (m, 2 ** (d - 1))
         The decision axes of the trees.
     split_trees : array (m, 2 ** (d - 1))
         The decision boundaries of the trees.
-    dtype : dtype
-        The dtype of the output.
+    dtype : dtype, optional
+        The dtype of the output. Ignored if `sum_trees` is `False`.
+    sum_trees : bool, default True
+        Whether to sum the values across trees.
 
     Returns
     -------
-    out : array (n,)
-        The sum of the values of the trees at the points in `X`.
+    out : array (n,) or (m, n)
+        The (sum of) the values of the trees at the points in `X`.
     """
     indices = traverse_forest(X, var_trees, split_trees)
     ntree, _ = leaf_trees.shape
-    tree_index = jnp.arange(ntree, dtype=jaxext.minimal_unsigned_dtype(ntree - 1))[:, None]
-    leaves = leaf_trees[tree_index, indices]
-    return jnp.sum(leaves, axis=0, dtype=dtype)
-        # this sum suggests to swap the vmaps, but I think it's better for X
-        # copying to keep it that way
+    tree_index = jnp.arange(ntree, dtype=jaxext.minimal_unsigned_dtype(ntree - 1))
+    leaves = leaf_trees[tree_index[:, None], indices]
+    if sum_trees:
+        return jnp.sum(leaves, axis=0, dtype=dtype)
+            # this sum suggests to swap the vmaps, but I think it's better for X
+            # copying to keep it that way
+    else:
+        return leaves
 
 def is_actual_leaf(split_tree, *, add_bottom_level=False):
     """
     Return a mask indicating the leaf nodes in a tree.
 
     Parameters
     ----------
@@ -234,15 +239,15 @@
     Return the depth of each node in a binary tree.
 
     Parameters
     ----------
     tree_length : int
         The length of the tree array, i.e., 2 ** d.
 
-    Returns    
+    Returns
     -------
     depth : array (tree_length,)
         The depth of each node. The root node (index 1) has depth 0. The depth
         is the position of the most significant non-zero bit in the index. The
         first element (the unused node) is marked as depth 0.
     """
     depths = []
```

### Comparing `bartz-0.2.1/src/bartz/jaxext.py` & `bartz-0.3.0/src/bartz/jaxext.py`

 * *Files 7% similar despite different names*

```diff
@@ -192,21 +192,22 @@
 
     Parameters
     ----------
     func : callable
         A jittable function with positional arguments only, with inputs and
         outputs pytrees of arrays.
     max_io_nbytes : int
-        The maximum number of input + output bytes in each batch.
-    in_axes : pytree of ints, default 0
+        The maximum number of input + output bytes in each batch (excluding
+        unbatched arguments.)
+    in_axes : pytree of int or None, default 0
         A tree matching the structure of the function input, indicating along
         which axes each array should be batched. If a single integer, it is
-        used for all arrays.
+        used for all arrays. A `None` axis indicates to not batch an argument.
     out_axes : pytree of ints, default 0
-        The same for outputs.
+        The same for outputs (but non-batching is not allowed).
     return_nbatches : bool, default False
         If True, the number of batches is returned as a second output.
 
     Returns
     -------
     batched_func : callable
         A function with the same signature as `func`, but that processes the
@@ -214,16 +215,26 @@
     """
 
     def expand_axes(axes, tree):
         if isinstance(axes, int):
             return tree_util.tree_map(lambda _: axes, tree)
         return tree_util.tree_map(lambda _, axis: axis, tree, axes)
 
+    def check_no_nones(axes, tree):
+        def check_not_none(_, axis):
+            assert axis is not None
+        tree_util.tree_map(check_not_none, tree, axes)
+
     def extract_size(axes, tree):
-        sizes = tree_util.tree_map(lambda x, axis: x.shape[axis], tree, axes)
+        def get_size(x, axis):
+            if axis is None:
+                return None
+            else:
+                return x.shape[axis]
+        sizes = tree_util.tree_map(get_size, tree, axes)
         sizes, _ = tree_util.tree_flatten(sizes)
         assert all(s == sizes[0] for s in sizes)
         return sizes[0]
 
     def sum_nbytes(tree):
         def nbytes(x):
             return math.prod(x.shape) * x.dtype.itemsize
@@ -239,31 +250,45 @@
         max_inv_divisor = dividend // min_divisor
         for inv_divisor in range(max_inv_divisor, 0, -1):
             if dividend % inv_divisor == 0:
                 return dividend // inv_divisor
         return dividend
 
     def next_divisor(dividend, min_divisor):
+        if dividend == 0:
+            return min_divisor
         if min_divisor * min_divisor <= dividend:
             return next_divisor_small(dividend, min_divisor)
         return next_divisor_large(dividend, min_divisor)
 
+    def pull_nonbatched(axes, tree):
+        def pull_nonbatched(x, axis):
+            if axis is None:
+                return None
+            else:
+                return x
+        return tree_util.tree_map(pull_nonbatched, tree, axes), tree
+
+    def push_nonbatched(axes, tree, original_tree):
+        def push_nonbatched(original_x, x, axis):
+            if axis is None:
+                return original_x
+            else:
+                return x
+        return tree_util.tree_map(push_nonbatched, original_tree, tree, axes)
+
     def move_axes_out(axes, tree):
-        def move_axis_out(axis, x):
-            if axis != 0:
-                return jnp.moveaxis(x, axis, 0)
-            return x
-        return tree_util.tree_map(move_axis_out, axes, tree)
+        def move_axis_out(x, axis):
+            return jnp.moveaxis(x, axis, 0)
+        return tree_util.tree_map(move_axis_out, tree, axes)
 
     def move_axes_in(axes, tree):
-        def move_axis_in(axis, x):
-            if axis != 0:
-                return jnp.moveaxis(x, 0, axis)
-            return x
-        return tree_util.tree_map(move_axis_in, axes, tree)
+        def move_axis_in(x, axis):
+            return jnp.moveaxis(x, 0, axis)
+        return tree_util.tree_map(move_axis_in, tree, axes)
 
     def batch(tree, nbatches):
         def batch(x):
             return x.reshape((nbatches, x.shape[0] // nbatches) + x.shape[1:])
         return tree_util.tree_map(batch, tree)
 
     def unbatch(tree):
@@ -283,34 +308,36 @@
     @jax.jit
     @functools.wraps(func)
     def batched_func(*args):
         example_result = jax.eval_shape(func, *args)
 
         in_axes = expand_axes(initial_in_axes, args)
         out_axes = expand_axes(initial_out_axes, example_result)
+        check_no_nones(out_axes, example_result)
+
+        size = extract_size((in_axes, out_axes), (args, example_result))
 
-        in_size = extract_size(in_axes, args)
-        out_size = extract_size(out_axes, example_result)
-        assert in_size == out_size
-        size = in_size
+        args, nonbatched_args = pull_nonbatched(in_axes, args)
 
-        total_nbytes = sum_nbytes(args) + sum_nbytes(example_result)
+        total_nbytes = sum_nbytes((args, example_result))
         min_nbatches = total_nbytes // max_io_nbytes + bool(total_nbytes % max_io_nbytes)
+        min_nbatches = max(1, min_nbatches)
         nbatches = next_divisor(size, min_nbatches)
-        assert 1 <= nbatches <= size
+        assert 1 <= nbatches <= max(1, size)
         assert size % nbatches == 0
         assert total_nbytes % nbatches == 0
 
         batch_nbytes = total_nbytes // nbatches
         if batch_nbytes > max_io_nbytes:
             assert size == nbatches
             warnings.warn(f'batch_nbytes = {batch_nbytes} > max_io_nbytes = {max_io_nbytes}')
 
         def loop(_, args):
             args = move_axes_in(in_axes, args)
+            args = push_nonbatched(in_axes, args, nonbatched_args)
             result = func(*args)
             result = move_axes_out(out_axes, result)
             return None, result
 
         args = move_axes_out(in_axes, args)
         args = batch(args, nbatches)
         _, result = lax.scan(loop, None, args)
```

### Comparing `bartz-0.2.1/src/bartz/mcmcloop.py` & `bartz-0.3.0/src/bartz/mcmcloop.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
-# 
+#
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
-# 
+#
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
@@ -30,16 +30,17 @@
 
 import jax
 from jax import random
 from jax import debug
 from jax import numpy as jnp
 from jax import lax
 
-from . import mcmcstep
+from . import jaxext
 from . import grove
+from . import mcmcstep
 
 @functools.partial(jax.jit, static_argnums=(1, 2, 3, 4))
 def run_mcmc(bart, n_burn, n_save, n_skip, callback, key):
     """
     Run the MCMC for the BART posterior.
 
     Parameters
@@ -87,64 +88,58 @@
     main_trace : dict
         The trace of the main phase, containing the following subset of fields
         from the `bart` dictionary, with an additional head index that runs
         over MCMC iterations: 'leaf_trees', 'var_trees', 'split_trees', plus
         the fields in `burnin_trace`.
     """
 
-    tracelist_burnin = 'sigma2', 'grow_prop_count', 'grow_acc_count', 'prune_prop_count', 'prune_acc_count'
+    tracelist_burnin = 'sigma2', 'grow_prop_count', 'grow_acc_count', 'prune_prop_count', 'prune_acc_count', 'ratios'
 
     tracelist_main = tracelist_burnin + ('leaf_trees', 'var_trees', 'split_trees')
 
     callback_kw = dict(n_burn=n_burn, n_save=n_save, n_skip=n_skip)
 
     def inner_loop(carry, _, tracelist, burnin):
         bart, i_total, i_skip, key = carry
         key, subkey = random.split(key)
         bart = mcmcstep.step(bart, subkey)
         callback(bart=bart, burnin=burnin, i_total=i_total, i_skip=i_skip, **callback_kw)
-        output = {key: bart[key] for key in tracelist}
+        output = {key: bart[key] for key in tracelist if key in bart}
         return (bart, i_total + 1, i_skip + 1, key), output
 
     def empty_trace(bart, tracelist):
-        return {
-            key: jnp.empty((0,) + bart[key].shape, bart[key].dtype)
-            for key in tracelist
-        }
+        return jax.vmap(lambda x: x, in_axes=None, out_axes=0, axis_size=0)(bart)
 
     if n_burn > 0:
         carry = bart, 0, 0, key
         burnin_loop = functools.partial(inner_loop, tracelist=tracelist_burnin, burnin=True)
         (bart, i_total, _, key), burnin_trace = lax.scan(burnin_loop, carry, None, n_burn)
     else:
         i_total = 0
         burnin_trace = empty_trace(bart, tracelist_burnin)
 
     def outer_loop(carry, _):
         bart, i_total, key = carry
         main_loop = functools.partial(inner_loop, tracelist=[], burnin=False)
         inner_carry = bart, i_total, 0, key
         (bart, i_total, _, key), _ = lax.scan(main_loop, inner_carry, None, n_skip)
-        output = {key: bart[key] for key in tracelist_main}
+        output = {key: bart[key] for key in tracelist_main if key in bart}
         return (bart, i_total, key), output
 
     if n_save > 0:
         carry = bart, i_total, key
         (bart, _, _), main_trace = lax.scan(outer_loop, carry, None, n_save)
     else:
         main_trace = empty_trace(bart, tracelist_main)
 
     return bart, burnin_trace, main_trace
 
-    # TODO I could add an argument callback_state to carry over state. This would allow e.g. accumulating counts. If I made the callback return the mcmc state, I could modify the mcmc from the callback.
-
 @functools.lru_cache
     # cache to make the callback function object unique, such that the jit
-    # of run_mcmc recognizes it => with the callback state, I can make
-    # printevery a runtime quantity
+    # of run_mcmc recognizes it
 def make_simple_print_callback(printevery):
     """
     Create a logging callback function for MCMC iterations.
 
     Parameters
     ----------
     printevery : int
@@ -189,11 +184,14 @@
         The predictors matrix, with `p` predictors and `n` observations.
 
     Returns
     -------
     y : array (n_trace, n)
         The predictions for each iteration of the MCMC.
     """
+    evaluate_trees = functools.partial(grove.evaluate_forest, sum_trees=False)
+    evaluate_trees = jaxext.autobatch(evaluate_trees, 2 ** 29, (None, 0, 0, 0))
     def loop(_, state):
-        return None, grove.evaluate_forest(X, state['leaf_trees'], state['var_trees'], state['split_trees'], jnp.float32)
+        values = evaluate_trees(X, state['leaf_trees'], state['var_trees'], state['split_trees'])
+        return None, jnp.sum(values, axis=0, dtype=jnp.float32)
     _, y = lax.scan(loop, None, trace)
     return y
```

### Comparing `bartz-0.2.1/src/bartz/mcmcstep.py` & `bartz-0.3.0/src/bartz/mcmcstep.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
-# 
+#
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
-# 
+#
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
@@ -30,14 +30,15 @@
 modified.
 
 In general, integer types are chosen to be the minimal types that contain the
 range of possible values.
 """
 
 import functools
+import math
 
 import jax
 from jax import random
 from jax import numpy as jnp
 from jax import lax
 
 from . import jaxext
@@ -50,15 +51,17 @@
     num_trees,
     p_nonterminal,
     sigma2_alpha,
     sigma2_beta,
     small_float=jnp.float32,
     large_float=jnp.float32,
     min_points_per_leaf=None,
-    suffstat_batch_size='auto',
+    resid_batch_size='auto',
+    count_batch_size='auto',
+    save_ratios=False,
     ):
     """
     Make a BART posterior sampling MCMC initial state.
 
     Parameters
     ----------
     X : int array (p, n)
@@ -78,18 +81,21 @@
         The scale parameter of the inverse gamma prior on the noise variance.
     small_float : dtype, default float32
         The dtype for large arrays used in the algorithm.
     large_float : dtype, default float32
         The dtype for scalars, small arrays, and arrays which require accuracy.
     min_points_per_leaf : int, optional
         The minimum number of data points in a leaf node. 0 if not specified.
-    suffstat_batch_size : int, None, str, default 'auto'
-        The batch size for computing sufficient statistics. `None` for no
-        batching. If 'auto', pick a value based on the device of `y`, or the
-        default device.
+    resid_batch_size, count_batch_sizes : int, None, str, default 'auto'
+        The batch sizes, along datapoints, for summing the residuals and
+        counting the number of datapoints in each leaf. `None` for no batching.
+        If 'auto', pick a value based on the device of `y`, or the default
+        device.
+    save_ratios : bool, default False
+        Whether to save the Metropolis-Hastings ratios.
 
     Returns
     -------
     bart : dict
         A dictionary with array values, representing a BART mcmc state. The
         keys are:
 
@@ -107,112 +113,144 @@
         'grow_prop_count', 'prune_prop_count' : int
             The number of grow/prune proposals made during one full MCMC cycle.
         'grow_acc_count', 'prune_acc_count' : int
             The number of grow/prune moves accepted during one full MCMC cycle.
         'p_nonterminal' : large_float array (d,)
             The probability of a nonterminal node at each depth, padded with a
             zero.
+        'p_propose_grow' : large_float array (2 ** (d - 1),)
+            The unnormalized probability of picking a leaf for a grow proposal.
         'sigma2_alpha' : large_float
             The shape parameter of the inverse gamma prior on the noise variance.
         'sigma2_beta' : large_float
             The scale parameter of the inverse gamma prior on the noise variance.
         'max_split' : int array (p,)
             The maximum split index for each variable.
         'y' : small_float array (n,)
             The response.
         'X' : int array (p, n)
             The predictors.
+        'leaf_indices' : int array (num_trees, n)
+            The index of the leaf each datapoints falls into, for each tree.
         'min_points_per_leaf' : int or None
             The minimum number of data points in a leaf node.
         'affluence_trees' : bool array (num_trees, 2 ** (d - 1)) or None
             Whether a non-bottom leaf nodes contains twice `min_points_per_leaf`
             datapoints. If `min_points_per_leaf` is not specified, this is None.
         'opt' : LeafDict
             A dictionary with config values:
 
-            'suffstat_batch_size' : int or None
-                The batch size for computing sufficient statistics.
             'small_float' : dtype
                 The dtype for large arrays used in the algorithm.
             'large_float' : dtype
                 The dtype for scalars, small arrays, and arrays which require
                 accuracy.
             'require_min_points' : bool
                 Whether the `min_points_per_leaf` parameter is specified.
+            'resid_batch_size', 'count_batch_size' : int or None
+                The data batch sizes for computing the sufficient statistics.
     """
 
     p_nonterminal = jnp.asarray(p_nonterminal, large_float)
     p_nonterminal = jnp.pad(p_nonterminal, (0, 1))
     max_depth = p_nonterminal.size
 
     @functools.partial(jax.vmap, in_axes=None, out_axes=0, axis_size=num_trees)
     def make_forest(max_depth, dtype):
         return grove.make_tree(max_depth, dtype)
 
     small_float = jnp.dtype(small_float)
     large_float = jnp.dtype(large_float)
     y = jnp.asarray(y, small_float)
-    suffstat_batch_size = _choose_suffstat_batch_size(suffstat_batch_size, y)
+    resid_batch_size, count_batch_size = _choose_suffstat_batch_size(resid_batch_size, count_batch_size, y)
+    sigma2 = jnp.array(sigma2_beta / sigma2_alpha, large_float)
+    sigma2 = jnp.where(jnp.isfinite(sigma2) & (sigma2 > 0), sigma2, 1)
 
     bart = dict(
         leaf_trees=make_forest(max_depth, small_float),
         var_trees=make_forest(max_depth - 1, jaxext.minimal_unsigned_dtype(X.shape[0] - 1)),
         split_trees=make_forest(max_depth - 1, max_split.dtype),
         resid=jnp.asarray(y, large_float),
-        sigma2=jnp.ones((), large_float),
+        sigma2=sigma2,
         grow_prop_count=jnp.zeros((), int),
         grow_acc_count=jnp.zeros((), int),
         prune_prop_count=jnp.zeros((), int),
         prune_acc_count=jnp.zeros((), int),
         p_nonterminal=p_nonterminal,
+        p_propose_grow=p_nonterminal[grove.tree_depths(2 ** (max_depth - 1))],
         sigma2_alpha=jnp.asarray(sigma2_alpha, large_float),
         sigma2_beta=jnp.asarray(sigma2_beta, large_float),
         max_split=jnp.asarray(max_split),
         y=y,
         X=jnp.asarray(X),
+        leaf_indices=jnp.ones((num_trees, y.size), jaxext.minimal_unsigned_dtype(2 ** max_depth - 1)),
         min_points_per_leaf=(
             None if min_points_per_leaf is None else
             jnp.asarray(min_points_per_leaf)
         ),
         affluence_trees=(
             None if min_points_per_leaf is None else
             make_forest(max_depth - 1, bool).at[:, 1].set(y.size >= 2 * min_points_per_leaf)
         ),
         opt=jaxext.LeafDict(
-            suffstat_batch_size=suffstat_batch_size,
             small_float=small_float,
             large_float=large_float,
             require_min_points=min_points_per_leaf is not None,
+            resid_batch_size=resid_batch_size,
+            count_batch_size=count_batch_size,
         ),
     )
 
+    if save_ratios:
+        bart['ratios'] = dict(
+            grow=dict(
+                trans_prior=jnp.full(num_trees, jnp.nan),
+                likelihood=jnp.full(num_trees, jnp.nan),
+            ),
+            prune=dict(
+                trans_prior=jnp.full(num_trees, jnp.nan),
+                likelihood=jnp.full(num_trees, jnp.nan),
+            ),
+        )
+
     return bart
 
-def _choose_suffstat_batch_size(size, y):
-    if size == 'auto':
+def _choose_suffstat_batch_size(resid_batch_size, count_batch_size, y):
+
+    @functools.cache
+    def get_platform():
         try:
             device = y.devices().pop()
         except jax.errors.ConcretizationTypeError:
             device = jax.devices()[0]
         platform = device.platform
+        if platform not in ('cpu', 'gpu'):
+            raise KeyError(f'Unknown platform: {platform}')
+        return platform
 
+    if resid_batch_size == 'auto':
+        platform = get_platform()
+        n = max(1, y.size)
         if platform == 'cpu':
-            return None
-                # maybe I should batch residuals (not counts) for numerical
-                # accuracy, even if it's slower
+            resid_batch_size = 2 ** int(round(math.log2(n / 6))) # n/6
         elif platform == 'gpu':
-            return 128 # 128 is good on A100, and V100 at high n
-                       # 512 is good on T4, and V100 at low n
-        else:
-            raise KeyError(f'Unknown platform: {platform}')
-    
-    elif size is not None:
-        return int(size)
-    
-    return size
+            resid_batch_size = 2 ** int(round((1 + math.log2(n)) / 3)) # n^1/3
+        resid_batch_size = max(1, resid_batch_size)
+
+    if count_batch_size == 'auto':
+        platform = get_platform()
+        if platform == 'cpu':
+            count_batch_size = None
+        elif platform == 'gpu':
+            n = max(1, y.size)
+            count_batch_size = 2 ** int(round(math.log2(n) / 2 - 2)) # n^1/2
+                # /4 is good on V100, /2 on L4/T4, still haven't tried A100
+            count_batch_size = max(1, count_batch_size)
+
+    return resid_batch_size, count_batch_size
 
 def step(bart, key):
     """
     Perform one full MCMC step on a BART state.
 
     Parameters
     ----------
@@ -244,22 +282,19 @@
     Returns
     -------
     bart : dict
         The new BART mcmc state.
 
     Notes
     -----
-    This function zeroes the proposal counters before using them.
+    This function zeroes the proposal counters.
     """
-    bart = bart.copy()
     key, subkey = random.split(key)
     grow_moves, prune_moves = sample_moves(bart, subkey)
-    bart['var_trees'] = grow_moves['var_tree']
-    grow_leaf_indices = grove.traverse_forest(bart['X'], grow_moves['var_tree'], grow_moves['split_tree'])
-    return accept_moves_and_sample_leaves(bart, grow_moves, prune_moves, grow_leaf_indices, key)
+    return accept_moves_and_sample_leaves(bart, grow_moves, prune_moves, key)
 
 def sample_moves(bart, key):
     """
     Propose moves for all the trees.
 
     Parameters
     ----------
@@ -270,25 +305,25 @@
 
     Returns
     -------
     grow_moves, prune_moves : dict
         The proposals for grow and prune moves. See `grow_move` and `prune_move`.
     """
     key = random.split(key, bart['var_trees'].shape[0])
-    return sample_moves_vmap_trees(bart['var_trees'], bart['split_trees'], bart['affluence_trees'], bart['max_split'], bart['p_nonterminal'], key)
+    return _sample_moves_vmap_trees(bart['var_trees'], bart['split_trees'], bart['affluence_trees'], bart['max_split'], bart['p_nonterminal'], bart['p_propose_grow'], key)
 
-@functools.partial(jaxext.vmap_nodoc, in_axes=(0, 0, 0, None, None, 0))
-def sample_moves_vmap_trees(var_tree, split_tree, affluence_tree, max_split, p_nonterminal, key):
+@functools.partial(jaxext.vmap_nodoc, in_axes=(0, 0, 0, None, None, None, 0))
+def _sample_moves_vmap_trees(*args):
+    args, key = args[:-1], args[-1]
     key, key1 = random.split(key)
-    args = var_tree, split_tree, affluence_tree, max_split, p_nonterminal
     grow = grow_move(*args, key)
     prune = prune_move(*args, key1)
     return grow, prune
 
-def grow_move(var_tree, split_tree, affluence_tree, max_split, p_nonterminal, key):
+def grow_move(var_tree, split_tree, affluence_tree, max_split, p_nonterminal, p_propose_grow, key):
     """
     Tree structure grow move proposal of BART MCMC.
 
     This moves picks a leaf node and converts it to a non-terminal node with
     two leaf children. The move is not possible if all the leaves are already at
     maximum depth.
 
@@ -300,89 +335,103 @@
         The splitting points of the tree.
     affluence_tree : bool array (2 ** (d - 1),) or None
         Whether a leaf has enough points to be grown.
     max_split : array (p,)
         The maximum split index for each variable.
     p_nonterminal : array (d,)
         The probability of a nonterminal node at each depth.
+    p_propose_grow : array (2 ** (d - 1),)
+        The unnormalized probability of choosing a leaf to grow.
     key : jax.dtypes.prng_key array
         A jax random key.
 
     Returns
     -------
     grow_move : dict
         A dictionary with fields:
 
-        'allowed' : bool
-            Whether the move is possible.
+        'num_growable' : int
+            The number of growable leaves.
         'node' : int
-            The index of the leaf to grow.
-        'var_tree' : array (2 ** (d - 1),)
-            The new decision axes of the tree.
-        'split_tree' : array (2 ** (d - 1),)
-            The new decision boundaries of the tree.
+            The index of the leaf to grow. ``2 ** d`` if there are no growable
+            leaves.
+        'left', 'right' : int
+            The indices of the children of 'node'.
+        'var', 'split' : int
+            The decision axis and boundary of the new rule.
         'partial_ratio' : float
             A factor of the Metropolis-Hastings ratio of the move. It lacks
             the likelihood ratio and the probability of proposing the prune
             move.
+        'var_tree', 'split_tree' : array (2 ** (d - 1),)
+            The updated decision axes and boundaries of the tree.
     """
 
     key, key1, key2 = random.split(key, 3)
-    
-    leaf_to_grow, num_growable, num_prunable, allowed = choose_leaf(split_tree, affluence_tree, key)
+
+    leaf_to_grow, num_growable, prob_choose, num_prunable = choose_leaf(split_tree, affluence_tree, p_propose_grow, key)
 
     var = choose_variable(var_tree, split_tree, max_split, leaf_to_grow, key1)
     var_tree = var_tree.at[leaf_to_grow].set(var.astype(var_tree.dtype))
-    
+
     split = choose_split(var_tree, split_tree, max_split, leaf_to_grow, key2)
     split_tree = split_tree.at[leaf_to_grow].set(split.astype(split_tree.dtype))
 
-    ratio = compute_partial_ratio(num_growable, num_prunable, p_nonterminal, leaf_to_grow, split_tree)
+    ratio = compute_partial_ratio(prob_choose, num_prunable, p_nonterminal, leaf_to_grow, split_tree)
 
+    left = leaf_to_grow << 1
     return dict(
-        allowed=allowed,
+        num_growable=num_growable,
         node=leaf_to_grow,
+        left=left,
+        right=left + 1,
+        var=var,
+        split=split,
         partial_ratio=ratio,
         var_tree=var_tree,
         split_tree=split_tree,
     )
 
-def choose_leaf(split_tree, affluence_tree, key):
+def choose_leaf(split_tree, affluence_tree, p_propose_grow, key):
     """
     Choose a leaf node to grow in a tree.
 
     Parameters
     ----------
     split_tree : array (2 ** (d - 1),)
         The splitting points of the tree.
     affluence_tree : bool array (2 ** (d - 1),) or None
         Whether a leaf has enough points to be grown.
+    p_propose_grow : array (2 ** (d - 1),)
+        The unnormalized probability of choosing a leaf to grow.
     key : jax.dtypes.prng_key array
         A jax random key.
 
     Returns
     -------
     leaf_to_grow : int
         The index of the leaf to grow. If ``num_growable == 0``, return
         ``2 ** d``.
     num_growable : int
         The number of leaf nodes that can be grown.
+    prob_choose : float
+        The normalized probability of choosing the selected leaf.
     num_prunable : int
         The number of leaf parents that could be pruned, after converting the
         selected leaf to a non-terminal node.
-    allowed : bool
-        Whether the grow move is allowed.
     """
-    is_growable, allowed = growable_leaves(split_tree, affluence_tree)
-    leaf_to_grow = randint_masked(key, is_growable)
-    leaf_to_grow = jnp.where(allowed, leaf_to_grow, 2 * split_tree.size)
+    is_growable = growable_leaves(split_tree, affluence_tree)
     num_growable = jnp.count_nonzero(is_growable)
+    distr = jnp.where(is_growable, p_propose_grow, 0)
+    leaf_to_grow, distr_norm = categorical(key, distr)
+    leaf_to_grow = jnp.where(num_growable, leaf_to_grow, 2 * split_tree.size)
+    prob_choose = distr[leaf_to_grow] / distr_norm
     is_parent = grove.is_leaves_parent(split_tree.at[leaf_to_grow].set(1))
     num_prunable = jnp.count_nonzero(is_parent)
-    return leaf_to_grow, num_growable, num_prunable, allowed
+    return leaf_to_grow, num_growable, prob_choose, num_prunable
 
 def growable_leaves(split_tree, affluence_tree):
     """
     Return a mask indicating the leaf nodes that can be proposed for growth.
 
     Parameters
     ----------
@@ -393,42 +442,40 @@
 
     Returns
     -------
     is_growable : bool array (2 ** (d - 1),)
         The mask indicating the leaf nodes that can be proposed to grow, i.e.,
         that are not at the bottom level and have at least two times the number
         of minimum points per leaf.
-    allowed : bool
-        Whether the grow move is allowed, i.e., there are growable leaves.
     """
     is_growable = grove.is_actual_leaf(split_tree)
     if affluence_tree is not None:
         is_growable &= affluence_tree
-    return is_growable, jnp.any(is_growable)
+    return is_growable
 
-def randint_masked(key, mask):
+def categorical(key, distr):
     """
-    Return a random integer in a range, including only some values.
+    Return a random integer from an arbitrary distribution.
 
     Parameters
     ----------
     key : jax.dtypes.prng_key array
         A jax random key.
-    mask : bool array (n,)
-        The mask indicating the allowed values.
+    distr : float array (n,)
+        An unnormalized probability distribution.
 
     Returns
     -------
     u : int
-        A random integer in the range ``[0, n)``, and which satisfies
-        ``mask[u] == True``. If all values in the mask are `False`, return `n`.
+        A random integer in the range ``[0, n)``. If all probabilities are zero,
+        return ``n``.
     """
-    ecdf = jnp.cumsum(mask)
-    u = random.randint(key, (), 0, ecdf[-1])
-    return jnp.searchsorted(ecdf, u, 'right')
+    ecdf = jnp.cumsum(distr)
+    u = random.uniform(key, (), ecdf.dtype, 0, ecdf[-1])
+    return jnp.searchsorted(ecdf, u, 'right'), ecdf[-1]
 
 def choose_variable(var_tree, split_tree, max_split, leaf_index, key):
     """
     Choose a variable to split on for a new non-terminal node.
 
     Parameters
     ----------
@@ -475,15 +522,15 @@
     -------
     var_to_ignore : int array (d - 2,)
         The indices of the variables that have an empty split range. Since the
         number of such variables is not fixed, unused values in the array are
         filled with `p`. The fill values are not guaranteed to be placed in any
         particular order. Variables may appear more than once.
     """
-    
+
     var_to_ignore = ancestor_variables(var_tree, max_split, leaf_index)
     split_range_vec = jax.vmap(split_range, in_axes=(None, None, None, None, 0))
     l, r = split_range_vec(var_tree, split_tree, max_split, leaf_index, var_to_ignore)
     num_split = r - l
     return jnp.where(num_split == 0, var_to_ignore, max_split.size)
 
 def ancestor_variables(var_tree, max_split, node_index):
@@ -607,15 +654,15 @@
     split : int
         The split point.
     """
     var = var_tree[leaf_index]
     l, r = split_range(var_tree, split_tree, max_split, leaf_index, var)
     return random.randint(key, (), l, r)
 
-def compute_partial_ratio(num_growable, num_prunable, p_nonterminal, leaf_to_grow, new_split_tree):
+def compute_partial_ratio(prob_choose, num_prunable, p_nonterminal, leaf_to_grow, new_split_tree):
     """
     Compute the product of the transition and prior ratios of a grow move.
 
     Parameters
     ----------
     num_growable : int
         The number of leaf nodes that can be grown.
@@ -636,460 +683,795 @@
         times the prior ratio P(new tree) / P(old tree), but the transition
         ratio is missing the factor P(propose prune) in the numerator.
     """
 
     # the two ratios also contain factors num_available_split *
     # num_available_var, but they cancel out
 
+    # p_prune can't be computed here because it needs the count trees, which are
+    # computed in the acceptance phase
+
     prune_allowed = leaf_to_grow != 1
         # prune allowed  <--->  the initial tree is not a root
         # leaf to grow is root  -->  the tree can only be a root
         # tree is a root  -->  the only leaf I can grow is root
 
     p_grow = jnp.where(prune_allowed, 0.5, 1)
 
-    trans_ratio = num_growable / (p_grow * num_prunable)
+    inv_trans_ratio = p_grow * prob_choose * num_prunable
 
     depth = grove.tree_depths(new_split_tree.size)[leaf_to_grow]
     p_parent = p_nonterminal[depth]
     cp_children = 1 - p_nonterminal[depth + 1]
     tree_ratio = cp_children * cp_children * p_parent / (1 - p_parent)
 
-    return trans_ratio * tree_ratio
+    return tree_ratio / inv_trans_ratio
 
-def prune_move(var_tree, split_tree, affluence_tree, max_split, p_nonterminal, key):
+def prune_move(var_tree, split_tree, affluence_tree, max_split, p_nonterminal, p_propose_grow, key):
     """
     Tree structure prune move proposal of BART MCMC.
 
     Parameters
     ----------
-    var_tree : array (2 ** (d - 1),)
+    var_tree : int array (2 ** (d - 1),)
         The variable indices of the tree.
-    split_tree : array (2 ** (d - 1),)
+    split_tree : int array (2 ** (d - 1),)
         The splitting points of the tree.
     affluence_tree : bool array (2 ** (d - 1),) or None
         Whether a leaf has enough points to be grown.
-    max_split : array (p,)
+    max_split : int array (p,)
         The maximum split index for each variable.
-    p_nonterminal : array (d,)
+    p_nonterminal : float array (d,)
         The probability of a nonterminal node at each depth.
+    p_propose_grow : float array (2 ** (d - 1),)
+        The unnormalized probability of choosing a leaf to grow.
     key : jax.dtypes.prng_key array
         A jax random key.
 
     Returns
     -------
     prune_move : dict
         A dictionary with fields:
 
         'allowed' : bool
             Whether the move is possible.
         'node' : int
-            The index of the node to prune.
+            The index of the node to prune. ``2 ** d`` if no node can be pruned.
+        'left', 'right' : int
+            The indices of the children of 'node'.
         'partial_ratio' : float
             A factor of the Metropolis-Hastings ratio of the move. It lacks
             the likelihood ratio and the probability of proposing the prune
             move. This ratio is inverted.
     """
-    node_to_prune, num_prunable, num_growable = choose_leaf_parent(split_tree, affluence_tree, key)
+    node_to_prune, num_prunable, prob_choose = choose_leaf_parent(split_tree, affluence_tree, p_propose_grow, key)
     allowed = split_tree[1].astype(bool) # allowed iff the tree is not a root
 
-    ratio = compute_partial_ratio(num_growable, num_prunable, p_nonterminal, node_to_prune, split_tree)
+    ratio = compute_partial_ratio(prob_choose, num_prunable, p_nonterminal, node_to_prune, split_tree)
 
+    left = node_to_prune << 1
     return dict(
         allowed=allowed,
         node=node_to_prune,
+        left=left,
+        right=left + 1,
         partial_ratio=ratio, # it is inverted in accept_move_and_sample_leaves
     )
 
-def choose_leaf_parent(split_tree, affluence_tree, key):
+def choose_leaf_parent(split_tree, affluence_tree, p_propose_grow, key):
     """
     Pick a non-terminal node with leaf children to prune in a tree.
 
     Parameters
     ----------
     split_tree : array (2 ** (d - 1),)
         The splitting points of the tree.
     affluence_tree : bool array (2 ** (d - 1),) or None
         Whether a leaf has enough points to be grown.
+    p_propose_grow : array (2 ** (d - 1),)
+        The unnormalized probability of choosing a leaf to grow.
     key : jax.dtypes.prng_key array
         A jax random key.
 
     Returns
     -------
     node_to_prune : int
         The index of the node to prune. If ``num_prunable == 0``, return
-        ``split_tree.size``.
+        ``2 ** d``.
     num_prunable : int
         The number of leaf parents that could be pruned.
-    num_growable : int
-        The number of leaf nodes that can be grown, after pruning the chosen
-        node.
+    prob_choose : float
+        The normalized probability of choosing the node to prune for growth.
     """
     is_prunable = grove.is_leaves_parent(split_tree)
-    node_to_prune = randint_masked(key, is_prunable)
     num_prunable = jnp.count_nonzero(is_prunable)
+    node_to_prune = randint_masked(key, is_prunable)
+    node_to_prune = jnp.where(num_prunable, node_to_prune, 2 * split_tree.size)
 
-    pruned_split_tree = split_tree.at[node_to_prune].set(0)
-    pruned_affluence_tree = (
+    split_tree = split_tree.at[node_to_prune].set(0)
+    affluence_tree = (
         None if affluence_tree is None else
         affluence_tree.at[node_to_prune].set(True)
     )
-    is_growable_leaf, _ = growable_leaves(pruned_split_tree, pruned_affluence_tree)
-    num_growable = jnp.count_nonzero(is_growable_leaf)
+    is_growable_leaf = growable_leaves(split_tree, affluence_tree)
+    prob_choose = p_propose_grow[node_to_prune]
+    prob_choose /= jnp.sum(p_propose_grow, where=is_growable_leaf)
+
+    return node_to_prune, num_prunable, prob_choose
+
+def randint_masked(key, mask):
+    """
+    Return a random integer in a range, including only some values.
+
+    Parameters
+    ----------
+    key : jax.dtypes.prng_key array
+        A jax random key.
+    mask : bool array (n,)
+        The mask indicating the allowed values.
 
-    return node_to_prune, num_prunable, num_growable
+    Returns
+    -------
+    u : int
+        A random integer in the range ``[0, n)``, and which satisfies
+        ``mask[u] == True``. If all values in the mask are `False`, return `n`.
+    """
+    ecdf = jnp.cumsum(mask)
+    u = random.randint(key, (), 0, ecdf[-1])
+    return jnp.searchsorted(ecdf, u, 'right')
 
-def accept_moves_and_sample_leaves(bart, grow_moves, prune_moves, grow_leaf_indices, key):
+def accept_moves_and_sample_leaves(bart, grow_moves, prune_moves, key):
     """
     Accept or reject the proposed moves and sample the new leaf values.
 
     Parameters
     ----------
     bart : dict
         A BART mcmc state.
     grow_moves : dict
         The proposals for grow moves, batched over the first axis. See
         `grow_move`.
     prune_moves : dict
         The proposals for prune moves, batched over the first axis. See
         `prune_move`.
-    grow_leaf_indices : int array (num_trees, n)
-        The leaf indices of the trees proposed by the grow move.
     key : jax.dtypes.prng_key array
         A jax random key.
 
     Returns
     -------
     bart : dict
         The new BART mcmc state.
     """
+    bart, grow_moves, prune_moves, count_trees, move_counts, u, z = accept_moves_parallel_stage(bart, grow_moves, prune_moves, key)
+    bart, counts = accept_moves_sequential_stage(bart, count_trees, grow_moves, prune_moves, move_counts, u, z)
+    return accept_moves_final_stage(bart, counts, grow_moves, prune_moves)
+
+def accept_moves_parallel_stage(bart, grow_moves, prune_moves, key):
+    """
+    Pre-computes quantities used to accept moves, in parallel across trees.
+
+    Parameters
+    ----------
+    bart : dict
+        A BART mcmc state.
+    grow_moves, prune_moves : dict
+        The proposals for the moves, batched over the first axis. See
+        `grow_move` and `prune_move`.
+    key : jax.dtypes.prng_key array
+        A jax random key.
+
+    Returns
+    -------
+    bart : dict
+        A partially updated BART mcmc state.
+    grow_moves, prune_moves : dict
+        The proposals for the moves, with the field 'partial_ratio' replaced
+        by 'trans_prior_ratio'.
+    count_trees : array (num_trees, 2 ** (d - 1))
+        The number of points in each potential or actual leaf node.
+    move_counts : dict
+        The counts of the number of points in the the nodes modified by the
+        moves.
+    u : float array (num_trees, 2)
+        Random uniform values used to accept the moves.
+    z : float array (num_trees, 2 ** d)
+        Random standard normal values used to sample the new leaf values.
+    """
     bart = bart.copy()
-    def loop(carry, item):
-        resid = carry.pop('resid')
-        resid, carry, trees = accept_move_and_sample_leaves(
+
+    bart['var_trees'] = grow_moves['var_tree']
+        # Since var_tree can contain garbage, I can set the var of leaf to be
+        # grown irrespectively of what move I'm gonna accept in the end.
+
+    bart['leaf_indices'] = apply_grow_to_indices(grow_moves, bart['leaf_indices'], bart['X'])
+
+    count_trees, move_counts = compute_count_trees(bart['leaf_indices'], grow_moves, prune_moves, bart['opt']['count_batch_size'])
+
+    grow_moves, prune_moves = complete_ratio(grow_moves, prune_moves, move_counts, bart['min_points_per_leaf'])
+
+    if bart['opt']['require_min_points']:
+        count_half_trees = count_trees[:, :grow_moves['split_tree'].shape[1]]
+        bart['affluence_trees'] = count_half_trees >= 2 * bart['min_points_per_leaf']
+
+    bart['leaf_trees'] = adapt_leaf_trees_to_grow_indices(bart['leaf_trees'], grow_moves)
+
+    key, subkey = random.split(key)
+    u = random.uniform(subkey, (len(bart['leaf_trees']), 2), bart['opt']['large_float'])
+    z = random.normal(key, bart['leaf_trees'].shape, bart['opt']['large_float'])
+
+    return bart, grow_moves, prune_moves, count_trees, move_counts, u, z
+
+def apply_grow_to_indices(grow_moves, leaf_indices, X):
+    """
+    Update the leaf indices to apply a grow move.
+
+    Parameters
+    ----------
+    grow_moves : dict
+        The proposals for grow moves. See `grow_move`.
+    leaf_indices : array (num_trees, n)
+        The index of the leaf each datapoint falls into.
+    X : array (p, n)
+        The predictors matrix.
+
+    Returns
+    -------
+    grow_leaf_indices : array (num_trees, n)
+        The updated leaf indices.
+    """
+    left_child = grow_moves['node'].astype(leaf_indices.dtype) << 1
+    go_right = X[grow_moves['var'], :] >= grow_moves['split'][:, None]
+    tree_size = jnp.array(2 * grow_moves['split_tree'].shape[1])
+    node_to_update = jnp.where(grow_moves['num_growable'], grow_moves['node'], tree_size)
+    return jnp.where(
+        leaf_indices == node_to_update[:, None],
+        left_child[:, None] + go_right,
+        leaf_indices,
+    )
+
+def compute_count_trees(grow_leaf_indices, grow_moves, prune_moves, batch_size):
+    """
+    Count the number of datapoints in each leaf.
+
+    Parameters
+    ----------
+    grow_leaf_indices : int array (num_trees, n)
+        The index of the leaf each datapoint falls into, if the grow move is
+        accepted.
+    grow_moves, prune_moves : dict
+        The proposals for the moves. See `grow_move` and `prune_move`.
+    batch_size : int or None
+        The data batch size to use for the summation.
+
+    Returns
+    -------
+    count_trees : int array (num_trees, 2 ** (d - 1))
+        The number of points in each potential or actual leaf node.
+    counts : dict
+        The counts of the number of points in the the nodes modified by the
+        moves, organized as two dictionaries 'grow' and 'prune', with subfields
+        'left', 'right', and 'total'.
+    """
+
+    ntree, tree_size = grow_moves['split_tree'].shape
+    tree_size *= 2
+    counts = dict(grow=dict(), prune=dict())
+    tree_indices = jnp.arange(ntree)
+
+    count_trees = count_datapoints_per_leaf(grow_leaf_indices, tree_size, batch_size)
+
+    # count datapoints in leaf to grow
+    counts['grow']['left'] = count_trees[tree_indices, grow_moves['left']]
+    counts['grow']['right'] = count_trees[tree_indices, grow_moves['right']]
+    counts['grow']['total'] = counts['grow']['left'] + counts['grow']['right']
+    count_trees = count_trees.at[tree_indices, grow_moves['node']].set(counts['grow']['total'])
+
+    # count datapoints in node to prune
+    counts['prune']['left'] = count_trees[tree_indices, prune_moves['left']]
+    counts['prune']['right'] = count_trees[tree_indices, prune_moves['right']]
+    counts['prune']['total'] = counts['prune']['left'] + counts['prune']['right']
+    count_trees = count_trees.at[tree_indices, prune_moves['node']].set(counts['prune']['total'])
+
+    return count_trees, counts
+
+def count_datapoints_per_leaf(leaf_indices, tree_size, batch_size):
+    """
+    Count the number of datapoints in each leaf.
+
+    Parameters
+    ----------
+    leaf_indices : int array (num_trees, n)
+        The index of the leaf each datapoint falls into.
+    tree_size : int
+        The size of the leaf tree array (2 ** d).
+    batch_size : int or None
+        The data batch size to use for the summation.
+
+    Returns
+    -------
+    count_trees : int array (num_trees, 2 ** (d - 1))
+        The number of points in each leaf node.
+    """
+    if batch_size is None:
+        return _count_scan(leaf_indices, tree_size)
+    else:
+        return _count_vec(leaf_indices, tree_size, batch_size)
+
+def _count_scan(leaf_indices, tree_size):
+    def loop(_, leaf_indices):
+        return None, _aggregate_scatter(1, leaf_indices, tree_size, jnp.uint32)
+    _, count_trees = lax.scan(loop, None, leaf_indices)
+    return count_trees
+
+def _aggregate_scatter(values, indices, size, dtype):
+    return (jnp
+        .zeros(size, dtype)
+        .at[indices]
+        .add(values)
+    )
+
+def _count_vec(leaf_indices, tree_size, batch_size):
+    return _aggregate_batched_alltrees(1, leaf_indices, tree_size, jnp.uint32, batch_size)
+        # uint16 is super-slow on gpu, don't use it even if n < 2^16
+
+def _aggregate_batched_alltrees(values, indices, size, dtype, batch_size):
+    ntree, n = indices.shape
+    tree_indices = jnp.arange(ntree)
+    nbatches = n // batch_size + bool(n % batch_size)
+    batch_indices = jnp.arange(n) % nbatches
+    return (jnp
+        .zeros((ntree, size, nbatches), dtype)
+        .at[tree_indices[:, None], indices, batch_indices]
+        .add(values)
+        .sum(axis=2)
+    )
+
+def complete_ratio(grow_moves, prune_moves, move_counts, min_points_per_leaf):
+    """
+    Complete non-likelihood MH ratio calculation.
+
+    This functions adds the probability of choosing the prune move.
+
+    Parameters
+    ----------
+    grow_moves, prune_moves : dict
+        The proposals for the moves. See `grow_move` and `prune_move`.
+    move_counts : dict
+        The counts of the number of points in the the nodes modified by the
+        moves.
+    min_points_per_leaf : int or None
+        The minimum number of data points in a leaf node.
+
+    Returns
+    -------
+    grow_moves, prune_moves : dict
+        The proposals for the moves, with the field 'partial_ratio' replaced
+        by 'trans_prior_ratio'.
+    """
+    grow_moves = grow_moves.copy()
+    prune_moves = prune_moves.copy()
+    compute_p_prune_vec = jax.vmap(compute_p_prune, in_axes=(0, 0, 0, None))
+    grow_p_prune, prune_p_prune = compute_p_prune_vec(grow_moves, move_counts['grow']['left'], move_counts['grow']['right'], min_points_per_leaf)
+    grow_moves['trans_prior_ratio'] = grow_moves.pop('partial_ratio') * grow_p_prune
+    prune_moves['trans_prior_ratio'] = prune_moves.pop('partial_ratio') * prune_p_prune
+    return grow_moves, prune_moves
+
+def compute_p_prune(grow_move, grow_left_count, grow_right_count, min_points_per_leaf):
+    """
+    Compute the probability of proposing a prune move.
+
+    Parameters
+    ----------
+    grow_move : dict
+        The proposal for the grow move, see `grow_move`.
+    grow_left_count, grow_right_count : int
+        The number of datapoints in the proposed children of the leaf to grow.
+    min_points_per_leaf : int or None
+        The minimum number of data points in a leaf node.
+
+    Returns
+    -------
+    grow_p_prune : float
+        The probability of proposing a prune move, after accepting the grow
+        move.
+    prune_p_prune : float
+        The probability of proposing the prune move.
+    """
+    other_growable_leaves = grow_move['num_growable'] >= 2
+    new_leaves_growable = grow_move['node'] < grow_move['split_tree'].size // 2
+    if min_points_per_leaf is not None:
+        any_above_threshold = grow_left_count >= 2 * min_points_per_leaf
+        any_above_threshold |= grow_right_count >= 2 * min_points_per_leaf
+        new_leaves_growable &= any_above_threshold
+    grow_again_allowed = other_growable_leaves | new_leaves_growable
+    grow_p_prune = jnp.where(grow_again_allowed, 0.5, 1)
+    prune_p_prune = jnp.where(grow_move['num_growable'], 0.5, 1)
+    return grow_p_prune, prune_p_prune
+
+def adapt_leaf_trees_to_grow_indices(leaf_trees, grow_moves):
+    """
+    Modify leaf values such that the indices of the grow move work on the
+    original tree.
+
+    Parameters
+    ----------
+    leaf_trees : float array (num_trees, 2 ** d)
+        The leaf values.
+    grow_moves : dict
+        The proposals for grow moves. See `grow_move`.
+
+    Returns
+    -------
+    leaf_trees : float array (num_trees, 2 ** d)
+        The modified leaf values. The value of the leaf to grow is copied to
+        what would be its children if the grow move was accepted.
+    """
+    ntree, _ = leaf_trees.shape
+    tree_indices = jnp.arange(ntree)
+    values_at_node = leaf_trees[tree_indices, grow_moves['node']]
+    return (leaf_trees
+        .at[tree_indices, grow_moves['left']]
+        .set(values_at_node)
+        .at[tree_indices, grow_moves['right']]
+        .set(values_at_node)
+    )
+
+def accept_moves_sequential_stage(bart, count_trees, grow_moves, prune_moves, move_counts, u, z):
+    """
+    The part of accepting the moves that has to be done one tree at a time.
+
+    Parameters
+    ----------
+    bart : dict
+        A partially updated BART mcmc state.
+    count_trees : array (num_trees, 2 ** (d - 1))
+        The number of points in each potential or actual leaf node.
+    grow_moves, prune_moves : dict
+        The proposals for the moves, with completed ratios. See `grow_move` and
+        `prune_move`.
+    move_counts : dict
+        The counts of the number of points in the the nodes modified by the
+        moves.
+    u : float array (num_trees, 2)
+        Random uniform values used to for proposal and accept decisions.
+    z : float array (num_trees, 2 ** d)
+        Random standard normal values used to sample the new leaf values.
+
+    Returns
+    -------
+    bart : dict
+        A partially updated BART mcmc state.
+    counts : dict
+        The indicators of proposals and acceptances for grow and prune moves.
+    """
+    bart = bart.copy()
+
+    def loop(resid, item):
+        resid, leaf_tree, split_tree, counts, ratios = accept_move_and_sample_leaves(
             bart['X'],
             len(bart['leaf_trees']),
-            bart['opt']['suffstat_batch_size'],
+            bart['opt']['resid_batch_size'],
             resid,
             bart['sigma2'],
             bart['min_points_per_leaf'],
-            carry,
+            'ratios' in bart,
             *item,
         )
-        carry['resid'] = resid
-        return carry, trees
-    carry = {
-        k: jnp.zeros_like(bart[k]) for k in
-        ['grow_prop_count', 'prune_prop_count', 'grow_acc_count', 'prune_acc_count']
-    }
-    carry['resid'] = bart['resid']
+        return resid, (leaf_tree, split_tree, counts, ratios)
+
     items = (
-        bart['leaf_trees'],
-        bart['split_trees'],
-        bart['affluence_trees'],
-        grow_moves,
-        prune_moves,
-        grow_leaf_indices,
-        random.split(key, len(bart['leaf_trees'])),
+        bart['leaf_trees'], count_trees,
+        grow_moves, prune_moves, move_counts,
+        bart['leaf_indices'],
+        u, z,
     )
-    carry, trees = lax.scan(loop, carry, items)
-    bart.update(carry)
-    bart.update(trees)
-    return bart
+    resid, (leaf_trees, split_trees, counts, ratios) = lax.scan(loop, bart['resid'], items)
+
+    bart['resid'] = resid
+    bart['leaf_trees'] = leaf_trees
+    bart['split_trees'] = split_trees
+    bart.get('ratios', {}).update(ratios)
+
+    return bart, counts
 
-def accept_move_and_sample_leaves(X, ntree, suffstat_batch_size, resid, sigma2, min_points_per_leaf, counts, leaf_tree, split_tree, affluence_tree, grow_move, prune_move, grow_leaf_indices, key):
+def accept_move_and_sample_leaves(X, ntree, resid_batch_size, resid, sigma2, min_points_per_leaf, save_ratios, leaf_tree, count_tree, grow_move, prune_move, move_counts, grow_leaf_indices, u, z):
     """
     Accept or reject a proposed move and sample the new leaf values.
 
     Parameters
     ----------
     X : int array (p, n)
         The predictors.
     ntree : int
         The number of trees in the forest.
-    suffstat_batch_size : int, None
-        The batch size for computing sufficient statistics.
+    resid_batch_size : int, None
+        The batch size for computing the sum of residuals in each leaf.
     resid : float array (n,)
         The residuals (data minus forest value).
     sigma2 : float
         The noise variance.
     min_points_per_leaf : int or None
         The minimum number of data points in a leaf node.
-    counts : dict
-        The acceptance counts from the mcmc state dict.
+    save_ratios : bool
+        Whether to save the acceptance ratios.
     leaf_tree : float array (2 ** d,)
         The leaf values of the tree.
-    split_tree : int array (2 ** (d - 1),)
-        The decision boundaries of the tree.
-    affluence_tree : bool array (2 ** (d - 1),) or None
-        Whether a leaf has enough points to be grown.
-    grow_move : dict
-        The proposal for the grow move. See `grow_move`.
-    prune_move : dict
-        The proposal for the prune move. See `prune_move`.
+    count_tree : int array (2 ** d,)
+        The number of datapoints in each leaf.
+    grow_move, prune_move : dict
+        The proposals for the moves, with completed ratios. See `grow_move` and
+        `prune_move`.
     grow_leaf_indices : int array (n,)
         The leaf indices of the tree proposed by the grow move.
-    key : jax.dtypes.prng_key array
-        A jax random key.
+    u : float array (2,)
+        Two uniform random values in [0, 1).
+    z : float array (2 ** d,)
+        Standard normal random values.
 
     Returns
     -------
     resid : float array (n,)
         The updated residuals (data minus forest value).
+    leaf_tree : float array (2 ** d,)
+        The new leaf values of the tree.
+    split_tree : int array (2 ** (d - 1),)
+        The updated decision boundaries of the tree.
     counts : dict
-        The updated acceptance counts.
-    trees : dict
-        The updated tree arrays.
+        The indicators of proposals and acceptances for grow and prune moves.
+    ratios : dict
+        The acceptance ratios for the moves. Empty if not to be saved.
     """
-    
-    # compute leaf indices in starting tree
-    grow_node = grow_move['node']
-    grow_left = grow_node << 1
-    grow_right = grow_left + 1
-    leaf_indices = jnp.where(
-        (grow_leaf_indices == grow_left) | (grow_leaf_indices == grow_right),
-        grow_node,
-        grow_leaf_indices,
-    )
 
-    # compute leaf indices in prune tree
-    prune_node = prune_move['node']
-    prune_left = prune_node << 1
-    prune_right = prune_left + 1
-    prune_leaf_indices = jnp.where(
-        (leaf_indices == prune_left) | (leaf_indices == prune_right),
-        prune_node,
-        leaf_indices,
-    )
+    # sum residuals and count units per leaf, in tree proposed by grow move
+    resid_tree = sum_resid(resid, grow_leaf_indices, leaf_tree.size, resid_batch_size)
 
     # subtract starting tree from function
-    resid += leaf_tree[leaf_indices]
+    resid_tree += count_tree * leaf_tree
 
-    # aggregate residuals and count units per leaf
-    grow_resid_tree, grow_count_tree = sufficient_stat(resid, grow_leaf_indices, leaf_tree.size, suffstat_batch_size)
-
-    # compute aggregations in starting tree
-    # I do not zero the children because garbage there does not matter
-    resid_tree = (grow_resid_tree.at[grow_node]
-        .set(grow_resid_tree[grow_left] + grow_resid_tree[grow_right]))
-    count_tree = (grow_count_tree.at[grow_node]
-        .set(grow_count_tree[grow_left] + grow_count_tree[grow_right]))
-
-    # compute aggregations in prune tree
-    prune_resid_tree = (resid_tree.at[prune_node]
-        .set(resid_tree[prune_left] + resid_tree[prune_right]))
-    prune_count_tree = (count_tree.at[prune_node]
-        .set(count_tree[prune_left] + count_tree[prune_right]))
+    # get indices of grow move
+    grow_node = grow_move['node']
+    assert grow_node.dtype == jnp.int32
+    grow_left = grow_move['left']
+    grow_right = grow_move['right']
+
+    # sum residuals in leaf to grow
+    grow_resid_left = resid_tree[grow_left]
+    grow_resid_right = resid_tree[grow_right]
+    grow_resid_total = grow_resid_left + grow_resid_right
+    resid_tree = resid_tree.at[grow_node].set(grow_resid_total)
 
-    # compute affluence trees
-    if min_points_per_leaf is not None:
-        grow_affluence_tree = grow_count_tree[:grow_count_tree.size // 2] >= 2 * min_points_per_leaf
-        prune_affluence_tree = affluence_tree.at[prune_node].set(True)
+    # get indices of prune move
+    prune_node = prune_move['node']
+    assert prune_node.dtype == jnp.int32
+    prune_left = prune_move['left']
+    prune_right = prune_move['right']
+
+    # sum residuals in node to prune
+    prune_resid_left = resid_tree[prune_left]
+    prune_resid_right = resid_tree[prune_right]
+    prune_resid_total = prune_resid_left + prune_resid_right
+    resid_tree = resid_tree.at[prune_node].set(prune_resid_total)
 
-    # compute probability of proposing prune
-    grow_p_prune = compute_p_prune_back(grow_move['split_tree'], grow_affluence_tree)
-    prune_p_prune = compute_p_prune_back(split_tree, affluence_tree)
+    # Now resid_tree and count_tree contain correct values whatever move is
+    # accepted.
 
     # compute likelihood ratios
-    grow_lk_ratio = compute_likelihood_ratio(grow_resid_tree, grow_count_tree, sigma2, grow_node, ntree, min_points_per_leaf)
-    prune_lk_ratio = compute_likelihood_ratio(resid_tree, count_tree, sigma2, prune_node, ntree, min_points_per_leaf)
+    grow_lk_ratio = compute_likelihood_ratio(grow_resid_total, grow_resid_left, grow_resid_right, move_counts['grow']['total'], move_counts['grow']['left'], move_counts['grow']['right'], sigma2, ntree)
+    prune_lk_ratio = compute_likelihood_ratio(prune_resid_total, prune_resid_left, prune_resid_right, move_counts['prune']['total'], move_counts['prune']['left'], move_counts['prune']['right'], sigma2, ntree)
 
     # compute acceptance ratios
-    grow_ratio = grow_p_prune * grow_move['partial_ratio'] * grow_lk_ratio
-    prune_ratio = prune_p_prune * prune_move['partial_ratio'] * prune_lk_ratio
+    grow_ratio = grow_move['trans_prior_ratio'] * grow_lk_ratio
+    if min_points_per_leaf is not None:
+        grow_ratio = jnp.where(move_counts['grow']['left'] >= min_points_per_leaf, grow_ratio, 0)
+        grow_ratio = jnp.where(move_counts['grow']['right'] >= min_points_per_leaf, grow_ratio, 0)
+    prune_ratio = prune_move['trans_prior_ratio'] * prune_lk_ratio
     prune_ratio = lax.reciprocal(prune_ratio)
 
-    # random coins in [0, 1) for proposal and acceptance
-    key, subkey = random.split(key)
-    u0, u1 = random.uniform(subkey, (2,))
+    # save acceptance ratios
+    ratios = {}
+    if save_ratios:
+        ratios.update(
+            grow=dict(
+                trans_prior=grow_move['trans_prior_ratio'],
+                likelihood=grow_lk_ratio,
+            ),
+            prune=dict(
+                trans_prior=lax.reciprocal(prune_move['trans_prior_ratio']),
+                likelihood=lax.reciprocal(prune_lk_ratio),
+            ),
+        )
 
     # determine what move to propose (not proposing anything is an option)
-    p_grow = jnp.where(grow_move['allowed'] & prune_move['allowed'], 0.5, grow_move['allowed'])
-    try_grow = u0 < p_grow
+    grow_allowed = grow_move['num_growable'].astype(bool)
+    p_grow = jnp.where(grow_allowed & prune_move['allowed'], 0.5, grow_allowed)
+    try_grow = u[0] < p_grow # use < instead of <= because coins are in [0, 1)
     try_prune = prune_move['allowed'] & ~try_grow
 
     # determine whether to accept the move
-    do_grow = try_grow & (u1 < grow_ratio)
-    do_prune = try_prune & (u1 < prune_ratio)
-
-    # pick trees for chosen move
-    trees = {}
-    split_tree = jnp.where(do_grow, grow_move['split_tree'], split_tree)
-    # the prune var tree is equal to the initial one, because I leave garbage values behind
-    split_tree = split_tree.at[prune_node].set(
-        jnp.where(do_prune, 0, split_tree[prune_node]))
-    if min_points_per_leaf is not None:
-        affluence_tree = jnp.where(do_grow, grow_affluence_tree, affluence_tree)
-        affluence_tree = jnp.where(do_prune, prune_affluence_tree, affluence_tree)
-    resid_tree = jnp.where(do_grow, grow_resid_tree, resid_tree)
-    count_tree = jnp.where(do_grow, grow_count_tree, count_tree)
-    resid_tree = jnp.where(do_prune, prune_resid_tree, resid_tree)
-    count_tree = jnp.where(do_prune, prune_count_tree, count_tree)
-
-    # update acceptance counts
-    counts = counts.copy()
-    counts['grow_prop_count'] += try_grow
-    counts['grow_acc_count'] += do_grow
-    counts['prune_prop_count'] += try_prune
-    counts['prune_acc_count'] += do_prune
+    do_grow = try_grow & (u[1] < grow_ratio)
+    do_prune = try_prune & (u[1] < prune_ratio)
 
-    # compute leaves posterior
-    prec_lk = count_tree / sigma2
+    # pick split tree for chosen move
+    split_tree = grow_move['split_tree']
+    split_tree = split_tree.at[jnp.where(do_grow, split_tree.size, grow_node)].set(0)
+    split_tree = split_tree.at[jnp.where(do_prune, prune_node, split_tree.size)].set(0)
+    # I can leave garbage in var_tree, resid_tree, count_tree
+
+    # compute leaves posterior and sample leaves
+    inv_sigma2 = lax.reciprocal(sigma2)
+    prec_lk = count_tree * inv_sigma2
     var_post = lax.reciprocal(prec_lk + ntree) # = 1 / (prec_lk + prec_prior)
-    mean_post = resid_tree / sigma2 * var_post # = mean_lk * prec_lk * var_post
-
-    # sample leaves
-    z = random.normal(key, mean_post.shape, mean_post.dtype)
+    mean_post = resid_tree * inv_sigma2 * var_post # = mean_lk * prec_lk * var_post
+    initial_leaf_tree = leaf_tree
     leaf_tree = mean_post + z * jnp.sqrt(var_post)
 
-    # add new tree to function
-    leaf_indices = jnp.where(do_grow, grow_leaf_indices, leaf_indices)
-    leaf_indices = jnp.where(do_prune, prune_leaf_indices, leaf_indices)
-    resid -= leaf_tree[leaf_indices]
-
-    # pack trees
-    trees = {
-        'leaf_trees': leaf_tree,
-        'split_trees': split_tree,
-        'affluence_trees': affluence_tree,
-    }
+    # copy leaves around such that the grow leaf indices select the right leaf
+    leaf_tree = (leaf_tree
+        .at[jnp.where(do_prune, prune_left, leaf_tree.size)]
+        .set(leaf_tree[prune_node])
+        .at[jnp.where(do_prune, prune_right, leaf_tree.size)]
+        .set(leaf_tree[prune_node])
+    )
+    leaf_tree = (leaf_tree
+        .at[jnp.where(do_grow, leaf_tree.size, grow_left)]
+        .set(leaf_tree[grow_node])
+        .at[jnp.where(do_grow, leaf_tree.size, grow_right)]
+        .set(leaf_tree[grow_node])
+    )
+
+    # replace old tree with new tree in function values
+    resid += (initial_leaf_tree - leaf_tree)[grow_leaf_indices]
 
-    return resid, counts, trees
+    # pack proposal and acceptance indicators
+    counts = dict(
+        grow_prop_count=try_grow,
+        grow_acc_count=do_grow,
+        prune_prop_count=try_prune,
+        prune_acc_count=do_prune,
+    )
+
+    return resid, leaf_tree, split_tree, counts, ratios
 
-def sufficient_stat(resid, leaf_indices, tree_size, batch_size):
+def sum_resid(resid, leaf_indices, tree_size, batch_size):
     """
-    Compute the sufficient statistics for the likelihood ratio of a tree move.
+    Sum the residuals in each leaf.
 
     Parameters
     ----------
     resid : float array (n,)
         The residuals (data minus forest value).
     leaf_indices : int array (n,)
         The leaf indices of the tree (in which leaf each data point falls into).
     tree_size : int
         The size of the tree array (2 ** d).
     batch_size : int, None
-        The batch size for the aggregation. Batching increases numerical
+        The data batch size for the aggregation. Batching increases numerical
         accuracy and parallelism.
 
     Returns
     -------
     resid_tree : float array (2 ** d,)
         The sum of the residuals at data points in each leaf.
-    count_tree : int array (2 ** d,)
-        The number of data points in each leaf.
     """
     if batch_size is None:
         aggr_func = _aggregate_scatter
     else:
-        aggr_func = functools.partial(_aggregate_batched, batch_size=batch_size)
-    resid_tree = aggr_func(resid, leaf_indices, tree_size, jnp.float32)
-    count_tree = aggr_func(1, leaf_indices, tree_size, jnp.uint32)
-    return resid_tree, count_tree
-
-def _aggregate_scatter(values, indices, size, dtype):
-    return (jnp
-        .zeros(size, dtype)
-        .at[indices]
-        .add(values)
-    )
+        aggr_func = functools.partial(_aggregate_batched_onetree, batch_size=batch_size)
+    return aggr_func(resid, leaf_indices, tree_size, jnp.float32)
 
-def _aggregate_batched(values, indices, size, dtype, batch_size):
-    nbatches = indices.size // batch_size + bool(indices.size % batch_size)
-    batch_indices = jnp.arange(indices.size) // batch_size
+def _aggregate_batched_onetree(values, indices, size, dtype, batch_size):
+    n, = indices.shape
+    nbatches = n // batch_size + bool(n % batch_size)
+    batch_indices = jnp.arange(n) % nbatches
     return (jnp
-        .zeros((nbatches, size), dtype)
-        .at[batch_indices, indices]
+        .zeros((size, nbatches), dtype)
+        .at[indices, batch_indices]
         .add(values)
-        .sum(axis=0)
+        .sum(axis=1)
     )
 
-def compute_p_prune_back(new_split_tree, new_affluence_tree):
-    """
-    Compute the probability of proposing a prune move after doing a grow move.
-
-    Parameters
-    ----------
-    new_split_tree : int array (2 ** (d - 1),)
-        The decision boundaries of the tree, after the grow move.
-    new_affluence_tree : bool array (2 ** (d - 1),)
-        Which leaves have enough points to be grown, after the grow move.
-
-    Returns
-    -------
-    p_prune : float
-        The probability of proposing a prune move after the grow move. This is
-        0.5 if grow is possible again, and 1 if it isn't. It can't be 0 because
-        at least the node just grown can be pruned.
-    """
-    _, grow_again_allowed = growable_leaves(new_split_tree, new_affluence_tree)
-    return jnp.where(grow_again_allowed, 0.5, 1)
-
-def compute_likelihood_ratio(resid_tree, count_tree, sigma2, node, n_tree, min_points_per_leaf):
+def compute_likelihood_ratio(total_resid, left_resid, right_resid, total_count, left_count, right_count, sigma2, n_tree):
     """
     Compute the likelihood ratio of a grow move.
 
     Parameters
     ----------
-    resid_tree : float array (2 ** d,)
-        The sum of the residuals at data points in each leaf.
-    count_tree : int array (2 ** d,)
-        The number of data points in each leaf.
+    total_resid : float
+        The sum of the residuals in the leaf to grow.
+    left_resid, right_resid : float
+        The sum of the residuals in the left/right child of the leaf to grow.
+    total_count : int
+        The number of datapoints in the leaf to grow.
+    left_count, right_count : int
+        The number of datapoints in the left/right child of the leaf to grow.
     sigma2 : float
         The noise variance.
-    node : int
-        The index of the leaf that has been grown.
     n_tree : int
         The number of trees in the forest.
-    min_points_per_leaf : int or None
-        The minimum number of data points in a leaf node.
 
     Returns
     -------
     ratio : float
         The likelihood ratio P(data | new tree) / P(data | old tree).
-
-    Notes
-    -----
-    The ratio is set to 0 if the grow move would create leaves with not enough
-    datapoints per leaf, although this is part of the prior rather than the
-    likelihood.
     """
 
-    left_child = node << 1
-    right_child = left_child + 1
-
-    left_resid = resid_tree[left_child]
-    right_resid = resid_tree[right_child]
-    total_resid = left_resid + right_resid
-
-    left_count = count_tree[left_child]
-    right_count = count_tree[right_child]
-    total_count = left_count + right_count
-
     sigma_mu2 = 1 / n_tree
     sigma2_left = sigma2 + left_count * sigma_mu2
     sigma2_right = sigma2 + right_count * sigma_mu2
     sigma2_total = sigma2 + total_count * sigma_mu2
 
     sqrt_term = sigma2 * sigma2_total / (sigma2_left * sigma2_right)
 
     exp_term = sigma_mu2 / (2 * sigma2) * (
         left_resid * left_resid / sigma2_left +
         right_resid * right_resid / sigma2_right -
         total_resid * total_resid / sigma2_total
     )
 
-    ratio = jnp.sqrt(sqrt_term) * jnp.exp(exp_term)
+    return jnp.sqrt(sqrt_term) * jnp.exp(exp_term)
 
-    if min_points_per_leaf is not None:
-        ratio = jnp.where(right_count >= min_points_per_leaf, ratio, 0)
-        ratio = jnp.where(left_count >= min_points_per_leaf, ratio, 0)
+def accept_moves_final_stage(bart, counts, grow_moves, prune_moves):
+    """
+    The final part of accepting the moves, in parallel across trees.
+
+    Parameters
+    ----------
+    bart : dict
+        A partially updated BART mcmc state.
+    counts : dict
+        The indicators of proposals and acceptances for grow and prune moves.
+    grow_moves, prune_moves : dict
+        The proposals for the moves. See `grow_move` and `prune_move`.
+
+    Returns
+    -------
+    bart : dict
+        The fully updated BART mcmc state.
+    """
+    bart = bart.copy()
+
+    for k, v in counts.items():
+        bart[k] = jnp.sum(v, axis=0)
 
-    return ratio
+    bart['leaf_indices'] = apply_moves_to_indices(bart['leaf_indices'], counts, grow_moves, prune_moves)
+
+    return bart
+
+def apply_moves_to_indices(leaf_indices, counts, grow_moves, prune_moves):
+    """
+    Update the leaf indices to match the accepted move.
+
+    Parameters
+    ----------
+    leaf_indices : int array (num_trees, n)
+        The index of the leaf each datapoint falls into, if the grow move was
+        accepted.
+    counts : dict
+        The indicators of proposals and acceptances for grow and prune moves.
+    grow_moves, prune_moves : dict
+        The proposals for the moves. See `grow_move` and `prune_move`.
+
+    Returns
+    -------
+    leaf_indices : int array (num_trees, n)
+        The updated leaf indices.
+    """
+    mask = ~jnp.array(1, leaf_indices.dtype) # ...1111111110
+    cond = (leaf_indices & mask) == grow_moves['left'][:, None]
+    leaf_indices = jnp.where(
+        cond & ~counts['grow_acc_count'][:, None],
+        grow_moves['node'][:, None].astype(leaf_indices.dtype),
+        leaf_indices,
+    )
+    cond = (leaf_indices & mask) == prune_moves['left'][:, None]
+    return jnp.where(
+        cond & counts['prune_acc_count'][:, None],
+        prune_moves['node'][:, None].astype(leaf_indices.dtype),
+        leaf_indices,
+    )
 
 def sample_sigma(bart, key):
     """
     Noise variance sampling step of BART MCMC.
 
     Parameters
     ----------
@@ -1103,14 +1485,14 @@
     bart : dict
         The new BART mcmc state.
     """
     bart = bart.copy()
 
     resid = bart['resid']
     alpha = bart['sigma2_alpha'] + resid.size / 2
-    norm2 = jnp.dot(resid, resid, preferred_element_type=bart['sigma2_beta'].dtype)
+    norm2 = jnp.dot(resid, resid, preferred_element_type=bart['opt']['large_float'])
     beta = bart['sigma2_beta'] + norm2 / 2
 
     sample = random.gamma(key, alpha)
     bart['sigma2'] = beta / sample
 
     return bart
```

### Comparing `bartz-0.2.1/src/bartz/prepcovars.py` & `bartz-0.3.0/src/bartz/prepcovars.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
-# 
+#
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
-# 
+#
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
@@ -51,18 +51,18 @@
         values at the end of each row are filled with the maximum value
         representable in the type of `X`.
     max_split : array (p,)
         The number of actually used values in each row of `splits`.
     """
     out_length = min(max_bins, X.shape[1]) - 1
     # return _quantilized_splits_from_matrix(X, out_length)
-    @functools.partial(jaxext.autobatch, max_io_nbytes=500_000_000)
-    def func(X):
+    @functools.partial(jaxext.autobatch, max_io_nbytes=2 ** 29)
+    def quantilize(X):
         return _quantilized_splits_from_matrix(X, out_length)
-    return func(X)
+    return quantilize(X)
 
 @functools.partial(jax.vmap, in_axes=(0, None))
 def _quantilized_splits_from_matrix(x, out_length):
     huge = jaxext.huge_value(x)
     u, actual_length = jaxext.unique(x, size=x.size, fill_value=huge)
     actual_length -= 1
     if jnp.issubdtype(x.dtype, jnp.integer):
@@ -78,36 +78,66 @@
     decimated_midpoints = midpoints[indices]
     truncated_midpoints = midpoints[:out_length]
     splits = jnp.where(actual_length > out_length, decimated_midpoints, truncated_midpoints)
     max_split = jnp.minimum(actual_length, out_length)
     max_split = max_split.astype(jaxext.minimal_unsigned_dtype(out_length))
     return splits, max_split
 
-@jax.jit
-def bin_predictors(X, splits):
+@functools.partial(jax.jit, static_argnums=(1,))
+def uniform_splits_from_matrix(X, num_bins):
+    """
+    Make an evenly spaced binning grid.
+
+    Parameters
+    ----------
+    X : array (p, n)
+        A matrix with `p` predictors and `n` observations.
+    num_bins : int
+        The number of bins to produce.
+
+    Returns
+    -------
+    splits : array (p, num_bins - 1)
+        A matrix containing, for each predictor, the boundaries between bins.
+        The excluded endpoints are the minimum and maximum value in each row of
+        `X`.
+    max_split : array (p,)
+        The number of cutpoints in each row of `splits`, i.e., ``num_bins - 1``.
+    """
+    low = jnp.min(X, axis=1)
+    high = jnp.max(X, axis=1)
+    splits = jnp.linspace(low, high, num_bins + 1, axis=1)[:, 1:-1]
+    assert splits.shape == (X.shape[0], num_bins - 1)
+    max_split = jnp.full(*splits.shape, jaxext.minimal_unsigned_dtype(num_bins - 1))
+    return splits, max_split
+
+@functools.partial(jax.jit, static_argnames=('method',))
+def bin_predictors(X, splits, **kw):
     """
     Bin the predictors according to the given splits.
 
     A value ``x`` is mapped to bin ``i`` iff ``splits[i - 1] < x <= splits[i]``.
 
     Parameters
     ----------
     X : array (p, n)
         A matrix with `p` predictors and `n` observations.
     splits : array (p, m)
         A matrix containing, for each predictor, the boundaries between bins.
         `m` is the maximum number of splits; each row may have shorter
         actual length, marked by padding unused locations at the end of the
         row with the maximum value allowed by the type.
+    **kw : dict
+        Additional arguments are passed to `jax.numpy.searchsorted`.
 
     Returns
     -------
     X_binned : int array (p, n)
         A matrix with `p` predictors and `n` observations, where each predictor
         has been replaced by the index of the bin it falls into.
     """
-    return _bin_predictors(X, splits)
-
-@jax.vmap
-def _bin_predictors(x, splits):
-    dtype = jaxext.minimal_unsigned_dtype(splits.size)
-    return jnp.searchsorted(splits, x).astype(dtype)
+    @functools.partial(jaxext.autobatch, max_io_nbytes=2 ** 29)
+    @jax.vmap
+    def bin_predictors(x, splits):
+        dtype = jaxext.minimal_unsigned_dtype(splits.size)
+        return jnp.searchsorted(splits, x, **kw).astype(dtype)
+    return bin_predictors(X, splits)
```

