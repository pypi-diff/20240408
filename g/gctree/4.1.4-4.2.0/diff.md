# Comparing `tmp/gctree-4.1.4.tar.gz` & `tmp/gctree-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gctree-4.1.4.tar", last modified: Wed Mar  6 21:48:54 2024, max compression
+gzip compressed data, was "gctree-4.2.0.tar", last modified: Mon Apr  8 20:11:12 2024, max compression
```

## Comparing `gctree-4.1.4.tar` & `gctree-4.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:48:54.290171 gctree-4.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-03-06 21:48:47.000000 gctree-4.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-06 21:48:47.000000 gctree-4.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-06 21:48:54.290171 gctree-4.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-06 21:48:47.000000 gctree-4.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:48:54.286171 gctree-4.1.4/gctree/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-06 21:48:47.000000 gctree-4.1.4/gctree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-06 21:48:54.290171 gctree-4.1.4/gctree/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    82581 2024-03-06 21:48:47.000000 gctree-4.1.4/gctree/branching_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)    25815 2024-03-06 21:48:47.000000 gctree-4.1.4/gctree/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7708 2024-03-06 21:48:47.000000 gctree-4.1.4/gctree/deduplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-03-06 21:48:47.000000 gctree-4.1.4/gctree/isotype.py
--rw-r--r--   0 runner    (1001) docker     (127)    20673 2024-03-06 21:48:47.000000 gctree-4.1.4/gctree/isotyping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2371 2024-03-06 21:48:47.000000 gctree-4.1.4/gctree/mkconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    23080 2024-03-06 21:48:47.000000 gctree-4.1.4/gctree/mutation_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-03-06 21:48:47.000000 gctree-4.1.4/gctree/phylip_parse.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1159 2024-03-06 21:48:47.000000 gctree-4.1.4/gctree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:48:54.290171 gctree-4.1.4/gctree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-06 21:48:54.000000 gctree-4.1.4/gctree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-06 21:48:54.000000 gctree-4.1.4/gctree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:48:54.000000 gctree-4.1.4/gctree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-06 21:48:54.000000 gctree-4.1.4/gctree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-06 21:48:54.000000 gctree-4.1.4/gctree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-06 21:48:54.000000 gctree-4.1.4/gctree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-06 21:48:54.290171 gctree-4.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-06 21:48:47.000000 gctree-4.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:48:54.290171 gctree-4.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-06 21:48:47.000000 gctree-4.1.4/tests/test_disambiguate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-06 21:48:47.000000 gctree-4.1.4/tests/test_isotype.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-03-06 21:48:47.000000 gctree-4.1.4/tests/test_likelihoods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-06 21:48:47.000000 gctree-4.1.4/tests/test_local_branching.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-03-06 21:48:47.000000 gctree-4.1.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:11:12.132504 gctree-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-08 20:11:05.000000 gctree-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 20:11:05.000000 gctree-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-08 20:11:12.132504 gctree-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-08 20:11:05.000000 gctree-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:11:12.128504 gctree-4.2.0/gctree/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 20:11:12.132504 gctree-4.2.0/gctree/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    85481 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/branching_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26814 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7708 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/isotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20763 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/isotyping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2371 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/mkconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/mutation_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/phylip_parse.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1159 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:11:12.132504 gctree-4.2.0/gctree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 20:11:12.132504 gctree-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-08 20:11:05.000000 gctree-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:11:12.132504 gctree-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-08 20:11:05.000000 gctree-4.2.0/tests/test_disambiguate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-08 20:11:05.000000 gctree-4.2.0/tests/test_isotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-08 20:11:05.000000 gctree-4.2.0/tests/test_likelihoods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-08 20:11:05.000000 gctree-4.2.0/tests/test_local_branching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-08 20:11:05.000000 gctree-4.2.0/versioneer.py
```

### Comparing `gctree-4.1.4/LICENSE` & `gctree-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gctree-4.1.4/PKG-INFO` & `gctree-4.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gctree
-Version: 4.1.4
+Version: 4.2.0
 Summary: phylogenetic inference of genotype-collapsed trees
 Home-page: https://github.com/matsengrp/gctree
 Author: Matsen Group
 Author-email: ematsen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `gctree-4.1.4/README.md` & `gctree-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gctree-4.1.4/gctree/branching_processes.py` & `gctree-4.2.0/gctree/branching_processes.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 branching process with mutation in which the tree is collapsed to nodes that
 count the number of clonal leaves of each type."""
 
 from __future__ import annotations
 
 import gctree.utils
 from gctree.isotyping import _isotype_dagfuncs, _isotype_annotation_dagfuncs
-from gctree.mutation_model import _mutability_dagfuncs
+from gctree.mutation_model import (
+    _mutability_dagfuncs,
+    _context_poisson_likelihood_dagfuncs,
+)
 from gctree.phylip_parse import disambiguate
 
 from frozendict import frozendict
 import pandas as pd
 import seaborn as sns
 import numpy as np
 import warnings
@@ -404,15 +407,15 @@
     def mle(self, **kwargs) -> Tuple[np.float64, np.float64]:
         r"""Maximum likelihood estimate of :math:`(p, q)`.
 
         .. math::
             (p, q) = \arg\max_{p,q\in [0,1]}\ell(p, q)
 
         Args:
-            kwargs: keyword arguments passed along to the log likelihood :meth:`CollapsedTree.ll`
+            kwargs: keyword arguments passed along to the branching process likelihood :meth:`CollapsedTree.ll`
 
         Returns:
             Tuple :math:`(p, q)` with estimated branching probability and estimated mutation probability
         """
         return _mle_helper(self.ll, **kwargs)
 
     def simulate(self, p: np.float64, q: np.float64, root: bool = True):
@@ -598,15 +601,14 @@
                                     if aa1 != aa2
                                 ]
                                 if mutations:
                                     T = ete3.TextFace(
                                         "\n".join(mutations),
                                         fsize=6,
                                         tight_text=False,
-                                        ftype="Courier",
                                     )
                                     if start == 0:
                                         T.margin_top = 6
                                     else:
                                         T.margin_bottom = 6
                                     T.rotation = -90
                                     node.add_face(
@@ -1046,15 +1048,15 @@
 
         Args:
             p: branching probability
             q: mutation probability
             marginal: compute the marginal likelihood over trees, otherwise compute the joint likelihood of trees
 
         Returns:
-            Log likelihood :math:`\ell(p, q; T, A)` and its gradient :math:`\nabla\ell(p, q; T, A)`
+            Log branching process likelihood :math:`\ell(p, q; T, A)` and its gradient :math:`\nabla\ell(p, q; T, A)`
         """
         if self._cm_countlist is None:
             if self._forest is not None:
                 cmcount_dagfuncs = _cmcounter_dagfuncs()
 
                 def to_tuple(mset):
                     # When there's unobserved root unifurcation, augment with
@@ -1118,251 +1120,300 @@
     def mle(self, **kwargs) -> Tuple[np.float64, np.float64]:
         r"""Maximum likelihood estimate of :math:`(p, q)`.
 
         .. math::
             (p, q) = \arg\max_{p,q\in [0,1]}\ell(p, q)
 
         Args:
-            kwargs: keyword arguments passed along to the log likelihood :meth:`CollapsedForest.ll`
+            kwargs: keyword arguments passed along to the branching process likelihood :meth:`CollapsedForest.ll`
 
         Returns:
             Tuple :math:`(p, q)` with estimated branching probability and estimated mutation probability
         """
         self.parameters = _mle_helper(self.ll, **kwargs)
         return self.parameters
 
     @_requires_dag
-    def filter_trees(
+    def filter_trees(  # noqa: C901
         self,
         ranking_coeffs: Optional[Sequence[float]] = None,
         mutability_file: Optional[str] = None,
         substitution_file: Optional[str] = None,
         ignore_isotype: bool = False,
         chain_split: Optional[int] = None,
         verbose: bool = False,
         outbase: str = "gctree.out",
         summarize_forest: bool = False,
         tree_stats: bool = False,
+        branching_process_ranking_coeff: float = -1,
+        use_old_mut_parsimony: bool = False,
     ) -> CollapsedForest:
         """Filter trees according to specified criteria.
 
         Trim the forest to minimize a linear
         combination of branching process likelihood, isotype parsimony score,
-        mutability parsimony score, and number of alleles, with coefficients
+        context/mutability-based Poisson likelihood, and number of alleles, with coefficients
         provided in the argument ``ranking_coeffs`, in that order.
 
         Args:
             ranking_coeffs: A list or tuple of coefficients for prioritizing tree weights.
-                The order of coefficients is: isotype parsimony score, mutability parsimony score,
+                The order of coefficients is: isotype parsimony score, context poisson likelihood,
                 and number of alleles. A coefficient of ``-1`` will be applied to branching process
-                likelihood.
+                likelihood by default, unless a different value is provided to the keyword argument
+                `branching_process_ranking_coeff`. Trees are chosen to minimize this linear combination
+                of tree weights, so weights for which larger values are more optimal (such as
+                likelihoods) should have negative coefficients.
                 If ranking_coeffs is not provided, trees will be ranked lexicographically
                 by likelihood, then by other traits, in the same order.
             mutability_file: A mutability model
             substitution_file: A substitution model
             ignore_isotype: Ignore isotype parsimony when ranking. By default, isotype information added with
                 :meth:``add_isotypes`` will be used to compute isotype parsimony, which is used in ranking.
             chain_split: The index at which non-adjacent sequences are concatenated, for calculating
-                mutability parsimony.
+                context-based Poisson likelihood.
             verbose: print information about trimming
             outbase: file name stem for a file with information for each tree in the DAG.
             summarize_forest: whether to write a summary of the forest to file `[outbase].forest_summary.log`
             tree_stats: whether to write stats for each tree in the forest to file `[outbase].tree_stats.log`
+            branching_process_ranking_coeff: Ranking coefficient to use for branching process likelihood. Value
+                is ignored unless `ranking_coeffs` argument is provided.
+            use_old_mut_parsimony: Whether to use the deprecated 'mutability parsimony' instead of
+                context-based poisson likelihood (only applicable if mutability and substitution files are
+                provided.
 
         Returns:
             The trimmed forest, containing all optimal trees according to the specified criteria, and a tuple
-            of data about the trees in that forest, with format (ll, isotype parsimony, mutability parsimony, alleles).
+            of data about the trees in that forest, with format (branching process likelihood, isotype parsimony,
+            context-based Poisson likelihood, alleles).
         """
         dag = self._forest
-        if self.parameters is None:
-            self.mle(marginal=True)
-        p, q = self.parameters
-        ll_dagfuncs = _ll_genotype_dagfuncs(p, q)
-        placeholder_dagfuncs = hdag.utils.AddFuncDict(
-            {
-                "start_func": lambda n: 0,
-                "edge_weight_func": lambda n1, n2: 0,
-                "accum_func": sum,
-            },
-            name="",
-        )
-        if ignore_isotype or not self.is_isotyped:
-            iso_funcs = placeholder_dagfuncs
+
+        if ranking_coeffs:
+            if len(ranking_coeffs) != 3:
+                raise ValueError(
+                    "If ranking_coeffs are provided to `filter_trees` method, a list of three values is expected."
+                )
+            coeffs = [branching_process_ranking_coeff] + list(ranking_coeffs)
+            if sum(abs(c) for c in coeffs) == 0:
+                raise ValueError(
+                    "At least one value provided to ranking_coeffs or the value of branching_process_ranking_coeff must be nonzero."
+                )
         else:
+            coeffs = [1] * 4
+
+        (
+            nz_coeff_bplikelihood,
+            nz_coeff_isotype_pars,
+            nz_coeff_context,
+            nz_coeff_alleles,
+        ) = [val != 0 for val in coeffs]
+        coeff_bplikelihood, coeff_isotype_pars, coeff_context, coeff_alleles = coeffs
+
+        dag_filters = []
+        if nz_coeff_bplikelihood:
+            if self.parameters is None:
+                self.mle(marginal=True)
+            p, q = self.parameters
+            ll_dagfuncs = _ll_genotype_dagfuncs(p, q)
+            dag_filters.append((ll_dagfuncs, coeff_bplikelihood))
             if verbose:
-                print("Isotype parsimony will be used as a ranking criterion")
+                print(f"Branching process parameters to be used for ranking: {(p, q)}")
+        if nz_coeff_isotype_pars and self.is_isotyped and (not ignore_isotype):
             # Check for missing isotype data in all but root node, and fake root-adjacent leaf node
             rootname = list(self._forest.dagroot.children())[0].attr["name"]
             if any(
                 not node.attr["isotype"]
                 for node in self._forest.preorder()
                 if not node.is_root() and node.attr["name"] != rootname
             ):
                 warnings.warn(
                     "Some isotype data seems to be missing. Isotype parsimony scores may be incorrect."
                 )
 
             iso_funcs = _isotype_dagfuncs()
-        if mutability_file and substitution_file:
-            if verbose:
-                print("Mutation model parsimony will be used as a ranking criterion")
+            dag_filters.append((iso_funcs, coeff_isotype_pars))
+        if nz_coeff_context and mutability_file and substitution_file:
+            if use_old_mut_parsimony:
+                mut_funcs = _mutability_dagfuncs(
+                    mutability_file=mutability_file,
+                    substitution_file=substitution_file,
+                    splits=[] if chain_split is None else [chain_split],
+                )
+            else:
+                mut_funcs = _context_poisson_likelihood_dagfuncs(
+                    mutability_file=mutability_file,
+                    substitution_file=substitution_file,
+                    splits=[] if chain_split is None else [chain_split],
+                )
+            dag_filters.append((mut_funcs, coeff_context))
+        if nz_coeff_alleles:
+            allele_funcs = _allele_dagfuncs()
+            dag_filters.append((allele_funcs, coeff_alleles))
 
-            mut_funcs = _mutability_dagfuncs(
-                mutability_file=mutability_file,
-                substitution_file=substitution_file,
-                splits=[] if chain_split is None else [chain_split],
-            )
-        else:
-            mut_funcs = placeholder_dagfuncs
-        allele_funcs = _allele_dagfuncs()
-        kwargls = (ll_dagfuncs, iso_funcs, mut_funcs, allele_funcs)
+        combined_dag_filter = functools.reduce(
+            lambda x, y: x + y, (dag_filter for dag_filter, _ in dag_filters)
+        )
         if ranking_coeffs:
             if len(ranking_coeffs) != 3:
                 raise ValueError(
                     "If ranking_coeffs are provided to `filter_trees` method, a list of three values is expected."
                 )
-            coeffs = [-1] + list(ranking_coeffs)
+            for dag_filter, coeff in dag_filters:
+                if dag_filter.optimal_func == max and coeff > 0:
+                    warnings.warn(
+                        f"Higher values for {dag_filter.weight_funcs.name} are generally better, but the "
+                        "provided ranking coefficient is positive, so trees with lower values will be preferred."
+                    )
+                if dag_filter.optimal_func == min and coeff < 0:
+                    warnings.warn(
+                        f"Lower values for {dag_filter.weight_funcs.name} are generally better, but the "
+                        "provided ranking coefficient is negative, so trees with higher values will be preferred."
+                    )
 
-            def minfunckey(weighttuple):
-                """Weighttuple will have (ll, isotypepars, mutabilitypars,
-                alleles)"""
+            filtered_coefficients = [coeff for _, coeff in dag_filters]
+
+            def linear_combinator(weighttuple):
                 return sum(
                     [
                         priority * float(weight)
-                        for priority, weight in zip(coeffs, weighttuple)
+                        for priority, weight in zip(filtered_coefficients, weighttuple)
                     ]
                 )
 
+            old_edge_func = combined_dag_filter["edge_weight_func"]
+            ranking_dag_filter = hdag.utils.HistoryDagFilter(
+                hdag.utils.AddFuncDict(
+                    {
+                        "start_func": lambda n: 0,
+                        "edge_weight_func": lambda n1, n2: linear_combinator(
+                            old_edge_func(n1, n2)
+                        ),
+                        "accum_func": sum,
+                    }
+                ),
+                min,
+                ordering_name="LinearCombination",
+            )
+            ranking_description = (
+                "Ranking trees to minimize a linear combination of "
+                + " + ".join(
+                    str(coeff) + "(" + fl.weight_funcs.name + ")"
+                    for fl, coeff in dag_filters
+                )
+            )
         else:
-
-            def minfunckey(weighttuple):
-                """Weighttuple will have (ll, isotypepars, mutabilitypars,
-                alleles)"""
-                # Sort output by likelihood, then isotype parsimony, then mutability score
-                return (-weighttuple[0],) + weighttuple[1:-1]
+            ranking_dag_filter = combined_dag_filter
+            ranking_description = "Ranking trees to " + " then ".join(
+                opt_name[:3] + "imize " + ord_name
+                for (opt_name, _), ord_name in zip(
+                    ranking_dag_filter.ordering_names,
+                    ranking_dag_filter.weight_funcs.names,
+                )
+            )
+        if verbose:
+            print(ranking_description)
 
         def print_stats(statlist, title, file=None, suppress_score=False):
             show_score = ranking_coeffs and not suppress_score
 
             def reformat(field, n=10):
                 if isinstance(field, int):
                     return format(field, "<" + str(n))
                 else:
                     return f"{field:{n}.{n}}"
 
-            def mask(weighttuple, n=10):
-                return tuple(
-                    reformat(field, n=n)
-                    for field, kwargs in zip(weighttuple, kwargls)
-                    if kwargs.name
-                )
-
-            print(f"Parameters: {(p, q)}", file=file)
             print("\n" + title + ":", file=file)
-            statstring = "\t".join(mask(tuple(kwargs.name for kwargs in kwargls), n=14))
+            statstring = "\t".join(
+                tuple(
+                    reformat(dfilter.weight_funcs.name, n=14)
+                    for dfilter, _ in dag_filters
+                )
+            )
             print(
                 f"tree     \t{statstring}" + ("\ttreescore" if show_score else ""),
                 file=file,
             )
             for j, best_weighttuple in enumerate(statlist, 1):
-                statstring = "\t".join(mask(best_weighttuple))
+                statstring = "\t".join(reformat(it) for it in best_weighttuple)
                 print(
                     f"{j:<10}\t{statstring}"
                     + (
-                        f"\t{reformat(minfunckey(best_weighttuple))}"
+                        f"\t{reformat(linear_combinator(best_weighttuple))}"
                         if show_score
                         else ""
                     ),
                     file=file,
                 )
 
-        # Filter by likelihood, isotype parsimony, mutability,
-        # and make ctrees, cforest, and render trees
-        dagweight_kwargs = ll_dagfuncs + iso_funcs + mut_funcs + allele_funcs
-        trimdag = dag.copy()
-        trimdag.trim_optimal_weight(
-            **dagweight_kwargs,
-            optimal_func=lambda l: min(l, key=minfunckey),  # noqa: E741
-        )
-        # make sure trimming worked as expected:
-        min_weightcounter = trimdag.weight_count(**dagweight_kwargs)
-        min_weightset = {minfunckey(key) for key in min_weightcounter}
-        if len(min_weightset) != 1:
-            raise RuntimeError(
-                "Filtering was not successful. After trimming, these weights are represented:",
-                min_weightset,
-            )
+        trimdag = dag[ranking_dag_filter]
 
         best_weighttuple = trimdag.optimal_weight_annotate(
-            **dagweight_kwargs,
-            optimal_func=lambda l: min(l, key=minfunckey),  # noqa: E741
+            **combined_dag_filter,
         )
+
+        if verbose:
+            print_stats([best_weighttuple], "Stats for optimal trees")
+
         if summarize_forest:
             with open(outbase + ".forest_summary.log", "w") as fh:
                 independent_best = []
-                for kwargs in kwargls:
-                    # Only summarize for stats for which information was
-                    # provided (not just placeholders):
-                    if kwargs.name:
-                        independent_best.append([])
-                        for opt in [min, max]:
-                            tempdag = dag.copy()
-                            opt_weight = tempdag.trim_optimal_weight(
-                                **kwargs, optimal_func=opt
+                for dfilter, _ in dag_filters:
+                    tempdag = dag.copy()
+                    min_val, max_val = tempdag.weight_range_annotate(**dfilter)
+                    opt_weight = tempdag.trim_optimal_weight(**dfilter)
+                    independent_best.append(opt_weight)
+                    fh.write(
+                        f"\nOverall {dfilter.weight_funcs.name} range {min_val} to {max_val}."
+                        f"\nAmong trees with {dfilter.optimal_func.__name__} {dfilter.weight_funcs.name} of: {opt_weight}\n"
+                    )
+                    for indfilter, _ in dag_filters:
+                        if indfilter.weight_funcs.name != dfilter.weight_funcs.name:
+                            minval, maxval = tempdag.weight_range_annotate(
+                                **indfilter.weight_funcs
                             )
-                            independent_best[-1].append(opt_weight)
                             fh.write(
-                                f"\nAmong trees with {opt.__name__} {kwargs.name} of: {opt_weight}\n"
+                                f"\t{indfilter.weight_funcs.name} range: {minval} to {maxval}\n"
                             )
-                            for inkwargs in kwargls:
-                                if inkwargs != kwargs and inkwargs.name:
-                                    minval = tempdag.optimal_weight_annotate(
-                                        **inkwargs, optimal_func=min
-                                    )
-                                    maxval = tempdag.optimal_weight_annotate(
-                                        **inkwargs, optimal_func=max
-                                    )
-                                    fh.write(
-                                        f"\t{inkwargs.name} range: {minval} to {maxval}\n"
-                                    )
-                independent_best[0].reverse()
                 print("\n", file=fh)
                 print_stats(
                     [
                         [
-                            stat - best[0]
+                            stat - best
                             for stat, best in zip(best_weighttuple, independent_best)
                         ]
                     ],
                     "Highest ranked tree: loss from best value",
                     file=fh,
                     suppress_score=True,
                 )
 
         if tree_stats:
-            dag_ls = list(dag.weight_count(**dagweight_kwargs).elements())
+            dag_ls = list(dag.weight_count(**combined_dag_filter).elements())
             # To clear _dp_data fields of their large cargo
             dag.optimal_weight_annotate(edge_weight_func=lambda n1, n2: 0)
+            if ranking_coeffs:
+                minfunckey = linear_combinator
+            else:
+                minfunckey = ranking_dag_filter.optimal_func
             dag_ls.sort(key=minfunckey)
 
-            df = pd.DataFrame(dag_ls, columns=dagweight_kwargs.names)
+            df = pd.DataFrame(dag_ls, columns=combined_dag_filter.weight_funcs.names)
             df.to_csv(outbase + ".tree_stats.csv")
             df["set"] = ["all_trees"] * len(df)
-            bestdf = pd.DataFrame([best_weighttuple], columns=dagweight_kwargs.names)
+            bestdf = pd.DataFrame(
+                [best_weighttuple], columns=combined_dag_filter.weight_funcs.names
+            )
             bestdf["set"] = ["best_tree"]
             toplot_df = pd.concat([df, bestdf], ignore_index=True)
             pplot = sns.pairplot(
-                toplot_df[["Log Likelihood", "Isotype Pars.", "Mut. Pars.", "set"]],
+                toplot_df.drop(["Alleles"], errors="ignore"),
                 hue="set",
                 diag_kind="hist",
             )
-            pplot.savefig(outbase + ".tree_stats.pairplot.png")
-
-        if verbose:
-            print_stats([best_weighttuple], "Stats for optimal trees")
+            pplot.savefig(outbase + ".tree_stats.pairplot.pdf")
 
         return (self._trimmed_self(trimdag), best_weighttuple)
 
     def likelihood_rankplot(self, outbase, p, q, img_type="svg"):
         """Save a rank plot of likelihoods to the file
         `[outbase].inference.likelihood_rank.[img_type]`."""
         ll_dagfuncs = _ll_genotype_dagfuncs(p, q)
@@ -1627,15 +1678,15 @@
     ll: Callable[[np.float64, np.float64], Tuple[np.float64, np.ndarray]], **kwargs
 ) -> Tuple[np.float64, np.float64]:
     # initialization
     x_0 = (0.5, 0.5)
     bounds = ((1e-6, 1 - 1e-6), (1e-6, 1 - 1e-6))
 
     def f(x):
-        """Negative log likelihood."""
+        """Negative log branching process likelihood."""
         return tuple(-y for y in ll(*x, **kwargs))
 
     grad_check = sco.check_grad(lambda x: f(x)[0], lambda x: f(x)[1], x_0)
     if grad_check > 1e-3:
         warnings.warn(
             f"gradient mismatches finite difference approximation by {grad_check}",
             RuntimeWarning,
@@ -1864,31 +1915,32 @@
             "edge_weight_func": edge_weight_func,
             "accum_func": accum_func,
         },
         name="cmcounters",
     )
 
 
-def _ll_genotype_dagfuncs(p: np.float64, q: np.float64) -> hdag.utils.AddFuncDict:
-    """Return functions for counting tree log likelihood on the history DAG.
+def _ll_genotype_dagfuncs(p: np.float64, q: np.float64) -> hdag.utils.HistoryDagFilter:
+    """Return functions for counting tree log branching process likelihood on
+    the history DAG.
 
     For numerical consistency, we resort to the use of ``decimal.Decimal``.
     This is exactly for the purpose of solving the problem that float sum is
     sensitive to order of summation, while Decimal sum is not.
 
     Still, there seems to be some inconsistency (probably in the part of the computation done with floats)
     so we wrap the Decimal in a :class:`historydag.utils.FloatState` object, where the exposed
     float is a rounded version of the hidden Decimal state, which is used for actual computations.
 
 
     Args:
         p, q: branching process parameters
 
     Returns:
-        A :meth:`historydag.utils.AddFuncDict` which may be passed as keyword arguments
+        A :meth:`historydag.utils.HistoryDagFilter` which may be passed as keyword arguments
         to :meth:`historydag.HistoryDag.weight_count`, :meth:`historydag.HistoryDag.trim_optimal_weight`,
         or :meth:`historydag.HistoryDag.optimal_weight_annotate`
         methods to trim or annotate a :meth:`historydag.HistoryDag` according to branching process likelihood.
         Weight format is ``decimal.Decimal``.
     """
 
     def edge_weight_ll_genotype(n1: hdag.HistoryDagNode, n2: hdag.HistoryDagNode):
@@ -1912,37 +1964,43 @@
             res = Decimal(CollapsedTree._ll_genotype(c, m, p, q)[0])
             return hdag.utils.FloatState(float(round(res, 8)), state=res)
 
     def accum_func(weightlist):
         res = sum(weight.state for weight in weightlist)
         return hdag.utils.FloatState(float(round(res, 8)), state=res)
 
-    return hdag.utils.AddFuncDict(
-        {
-            "start_func": lambda n: hdag.utils.FloatState(0.0, state=Decimal(0)),
-            "edge_weight_func": edge_weight_ll_genotype,
-            "accum_func": accum_func,
-        },
-        name="Log Likelihood",
+    return hdag.utils.HistoryDagFilter(
+        hdag.utils.AddFuncDict(
+            {
+                "start_func": lambda n: hdag.utils.FloatState(0.0, state=Decimal(0)),
+                "edge_weight_func": edge_weight_ll_genotype,
+                "accum_func": accum_func,
+            },
+            name="LogBPLikelihood",
+        ),
+        max,
     )
 
 
-def _allele_dagfuncs() -> hdag.utils.AddFuncDict:
+def _allele_dagfuncs() -> hdag.utils.HistoryDagFilter:
     """Return functions for filtering trees in a history DAG by allele count.
 
     The number of alleles in a tree is the number of unique sequences observed on nodes of that tree.
 
     Returns:
         A :meth:`historydag.utils.AddFuncDict` which may be passed as keyword arguments
         to :meth:`historydag.HistoryDag.weight_count`, :meth:`historydag.HistoryDag.trim_optimal_weight`,
         or :meth:`historydag.HistoryDag.optimal_weight_annotate`
         methods to trim or annotate a :meth:`historydag.HistoryDag` according to allele count.
         Weight format is ``int``.
     """
-    return hdag.utils.AddFuncDict(
-        {
-            "start_func": lambda n: 0,
-            "edge_weight_func": lambda n1, n2: n1.label != n2.label,
-            "accum_func": sum,
-        },
-        name="Alleles",
+    return hdag.utils.HistoryDagFilter(
+        hdag.utils.AddFuncDict(
+            {
+                "start_func": lambda n: 0,
+                "edge_weight_func": lambda n1, n2: n1.label != n2.label,
+                "accum_func": sum,
+            },
+            name="Alleles",
+        ),
+        min,
     )
```

### Comparing `gctree-4.1.4/gctree/cli.py` & `gctree-4.2.0/gctree/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,14 +205,16 @@
         verbose=args.verbose,
         outbase=args.outbase,
         summarize_forest=args.summarize_forest,
         tree_stats=args.tree_stats,
         mutability_file=args.mutability,
         substitution_file=args.substitution,
         chain_split=args.chain_split,
+        branching_process_ranking_coeff=args.branching_process_ranking_coeff,
+        use_old_mut_parsimony=args.use_old_mut_parsimony,
     )
 
     if args.verbose:
         if trimmed_forest.n_trees > 1:
             n_topologies = trimmed_forest.n_topologies()
             print(
                 "Degenerate ranking criteria: trimmed history DAG contains "
@@ -531,15 +533,15 @@
     parser_infer.add_argument(
         "--chain_split",
         type=int,
         default=None,
         help=(
             "when using concatenated heavy and light chains, this is the 0-based"
             " index at which the 2nd chain begins, needed for determining coding frame in both chains,"
-            " and also to correctly calculate mutability parsimony."
+            " and also to correctly calculate context-based Poisson likelihood."
         ),
     )
     parser_infer.add_argument(
         "--frame2",
         type=int,
         default=None,
         choices=(1, 2, 3),
@@ -607,24 +609,44 @@
             "they will be used to rank trees after likelihood and isotype parsimony."
             "This shall be a csv file with the first column containing fivemers, and the next four"
             "columns containing targeting probabilities for bases A, C, G, and T, respectively."
             "See a file excerpt in the documentation for :meth:`mutation_model.MutationModel`."
         ),
     )
     parser_infer.add_argument(
+        "--branching_process_ranking_coeff",
+        type=float,
+        default=-1,
+        help=(
+            "Coefficient used for branching process likelihood, when ranking trees by a linear "
+            "combination of traits. This value will be ignored if `--ranking_coeffs` argument is not "
+            "also provided."
+        ),
+    )
+    parser_infer.add_argument(
         "--ranking_coeffs",
         type=float,
         nargs=3,
         default=None,
         help=(
             "List of coefficients for ranking trees by a linear combination of traits. "
             "Coefficients are in order: isotype parsimony, mutation model parsimony, number of alleles. "
             "A coefficient of -1 will be applied to branching process likelihood. "
             "If not provided, trees will be ranked lexicographically by likelihood, "
-            "isotype parsimony, and mutability parsimony in that order."
+            "isotype parsimony, and context-based Poisson likelihood in that order."
+        ),
+    )
+    parser_infer.add_argument(
+        "--use_old_mut_parsimony",
+        action="store_true",
+        help=(
+            "Use old mutability parsimony instead of poisson context likelihood. Not recommended "
+            "unless attempting to reproduce results from older versions of gctree. "
+            "This argument will have no effect unless an S5F model is provided with the arguments "
+            "`--mutability` and `--substitution`."
         ),
     )
     parser_infer.add_argument(
         "--summarize_forest",
         action="store_true",
         help=(
             "write a file `[outbase].forest_summary.log` with a summary of traits for trees in the forest."
```

### Comparing `gctree-4.1.4/gctree/deduplicate.py` & `gctree-4.2.0/gctree/deduplicate.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.4/gctree/isotype.py` & `gctree-4.2.0/gctree/isotype.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             "  transitions are required along tree edges. Changes in node count\n"
             "  after isotype additions indicate that either observed nodes had\n"
             "  to be exploded based on observed isotypes, or isotype switching\n"
             "  order violations required internal nodes to be expanded as leaf\n"
             "  nodes.\n\n"
             "This tool doesn’t make any judgements about which tree is best.\n"
             "Tree output order is the same as in gctree inference: ranking is\n"
-            "by log likelihood before isotype additions. A determination of\n"
+            "by branching process likelihood before isotype additions. A determination of\n"
             "which is the best tree is left to the user, based on likelihoods,\n"
             "isotype parsimony score, and changes in the number of nodes after\n"
             "isotype additions.\n"
         ),
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument(
```

### Comparing `gctree-4.1.4/gctree/isotyping.py` & `gctree-4.2.0/gctree/isotyping.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,15 +401,15 @@
                 cell_id for cell_id in cell_ids if isotype_map[cell_id] == isotype
             }
             for isotype in isotypeset
         }
     return newidmap
 
 
-def _isotype_dagfuncs() -> hdag.utils.AddFuncDict:
+def _isotype_dagfuncs() -> hdag.utils.HistoryDagFilter:
     """Return functions for filtering by isotype parsimony score on the history
     DAG.
 
     The DAG on which these functions is run should have key ``isotype`` in their attr dictionaries.
     The :meth:``CollapsedForest.add_isotypes`` method can be used to achieve this.
     If isotypes aren't added, these functions will return a weight of 0 for all trees.
 
@@ -431,21 +431,24 @@
             n1isos = n1.attr["isotype"]
             n2isos = n2.attr["isotype"]
             if not n1isos or not n2isos:
                 return 0
             n1iso = list(n1isos.keys())[0]
             return int(sum(isotype_distance(n1iso, n2iso) for n2iso in n2isos.keys()))
 
-    return hdag.utils.AddFuncDict(
-        {
-            "start_func": lambda n: 0,
-            "edge_weight_func": edge_weight_func,
-            "accum_func": sum,
-        },
-        name="Isotype Pars.",
+    return hdag.utils.HistoryDagFilter(
+        hdag.utils.AddFuncDict(
+            {
+                "start_func": lambda n: 0,
+                "edge_weight_func": edge_weight_func,
+                "accum_func": sum,
+            },
+            name="Isotype Pars.",
+        ),
+        min,
     )
 
 
 def _isotype_annotation_dagfuncs(
     isotypemap: Optional[Mapping[str, str]] = None,
     isotypemap_file: Optional[str] = None,
     idmap: Optional[Mapping[str, Set[str]]] = None,
```

### Comparing `gctree-4.1.4/gctree/mkconfig.py` & `gctree-4.2.0/gctree/mkconfig.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.4/gctree/mutation_model.py` & `gctree-4.2.0/gctree/mutation_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import numpy as np
 from scipy.stats import poisson
 import random
 from Bio.Seq import Seq
 import historydag as hdag
 from multiset import FrozenMultiset
 from typing import Tuple, List, Callable, Optional
+import itertools
+import math
 
 
 class MutationModel:
     r"""A class for a mutation model, and functions to mutate sequences.
 
     Args:
         mutability_file: S5F format mutabilities
@@ -125,28 +127,33 @@
                 )
             )
         if not all(n in "ACGTN" for n in kmer):
             raise ValueError(
                 "sequence {} must contain only characters A, C, G, T, or N".format(kmer)
             )
 
-        mutabilities_to_average, substitutions_to_average = zip(
-            *[self.context_model[x] for x in MutationModel._disambiguate(kmer)]
-        )
-
-        average_mutability = np.mean(mutabilities_to_average)
-        average_substitution = {
-            b: sum(
-                substitution_dict[b] for substitution_dict in substitutions_to_average
+        cached = self.context_model.get(kmer, None)
+        if cached is None:
+            mutabilities_to_average, substitutions_to_average = zip(
+                *[self.context_model[x] for x in MutationModel._disambiguate(kmer)]
             )
-            / len(substitutions_to_average)
-            for b in "ACGT"
-        }
 
-        return average_mutability, average_substitution
+            average_mutability = np.mean(mutabilities_to_average)
+            average_substitution = {
+                b: sum(
+                    substitution_dict[b]
+                    for substitution_dict in substitutions_to_average
+                )
+                / len(substitutions_to_average)
+                for b in "ACGT"
+            }
+            cached = average_mutability, average_substitution
+            self.context_model[kmer] = cached
+
+        return cached
 
     def mutabilities(self, sequence: str) -> List[Tuple[np.float64, np.float64]]:
         r"""Returns the mutability of a sequence at each site, along with
         nucleotide biases.
 
         Args:
             sequence: nucleotide sequence
@@ -436,15 +443,15 @@
                     )
                 return
     yield _accum
 
 
 def _mutability_dagfuncs(
     *args, splits: List[int] = [], **kwargs
-) -> hdag.utils.AddFuncDict:
+) -> hdag.utils.HistoryDagFilter:
     """Return functions for counting mutability parsimony on the history DAG.
 
     Mutability parsimony of a tree is the sum over all edges in the tree
     of mutability distances between parent and child node sequences.
 
     The mutability distance from an ancestral sequence to a target sequence is the sum of
     :math:`-log(mutability * p)` over all sites which do match, where :math:`mutability`
@@ -474,44 +481,46 @@
 
     def distance(node1, node2):
         if node1.is_root():
             return 0
         else:
             return dist(node1.label.sequence, node2.label.sequence)
 
-    return hdag.utils.AddFuncDict(
-        {"start_func": lambda n: 0, "edge_weight_func": distance, "accum_func": sum},
-        name="Mut. Pars.",
+    return hdag.utils.HistoryDagFilter(
+        hdag.utils.AddFuncDict(
+            {
+                "start_func": lambda n: 0,
+                "edge_weight_func": distance,
+                "accum_func": sum,
+            },
+            name="Mut. Pars.",
+        ),
+        min,
     )
 
 
 def _mutability_distance_precursors(
     mutation_model: MutationModel, splits: List[int] = []
 ):
     chunk_idxs = list(zip([0] + splits, splits + [None]))
-    # Caching could be moved to the MutationModel class instead.
-    context_model = mutation_model.context_model.copy()
-    k = mutation_model.k
-    h = k // 2
-    # Build all sequences with (when k=5) one or two Ns on either end
-    templates = [
-        ("N" * left, "N" * (k - left - right), "N" * right)
-        for left in range(h + 1)
-        for right in range(h + 1)
-        if left != 0 or right != 0
-    ]
-
-    kmers_to_compute = [
-        leftns + stub + rightns
-        for leftns, ambig_stub, rightns in templates
-        for stub in _sequence_disambiguations(ambig_stub)
-    ]
-    # Cache all these mutabilities in context_model also
-    context_model.update(
-        {kmer: mutation_model.mutability(kmer) for kmer in kmers_to_compute}
+
+    h = mutation_model.k // 2
+
+    # Pads sequence with N's, including in the chain-split boundary to
+    # avoid unrelated sites from being treated as part of each others' context.
+
+    # Indices at which padding N's will be in sequences returned from add_ns.
+    # Does not include indices of last two N's.
+    padding_indices = set(
+        itertools.chain.from_iterable(
+            [
+                range(split + idx * h, split + (idx + 1) * h)
+                for idx, split in enumerate([0] + splits)
+            ]
+        )
     )
 
     def add_ns(seq: str):
         ns = "N" * h
         chunks = [seq[start:end] for start, end in chunk_idxs]
         return ns + ns.join(chunks) + ns
 
@@ -531,24 +540,34 @@
         # with rate of new base. Not sure if this is a good choice.
         if pairs:
             # for floating point behavior
             pairs = sorted(pairs.items())
             p_arr = [
                 mult
                 * (
-                    np.log(context_model[mer][0])
-                    + np.log(context_model[mer][1][newbase])
+                    np.log(mutation_model.mutability(mer)[0])
+                    + np.log(mutation_model.mutability(mer)[1][newbase])
                 )
                 for (mer, newbase), mult in pairs
             ]
             return -sum(p_arr)
         else:
             return 0.0
 
-    return (mutpairs, sum_minus_logp)
+    def mutability_sum(parent_seq):
+        padded_seq = add_ns(parent_seq)
+        for idx in padding_indices:
+            assert padded_seq[idx] == "N"
+        return sum(
+            mutation_model.mutability(padded_seq[idx - h : idx + h + 1])[0]
+            for idx, _ in enumerate(padded_seq[:-h])
+            if idx not in padding_indices
+        )
+
+    return (mutpairs, sum_minus_logp, mutability_sum)
 
 
 def _mutability_distance(mutation_model: MutationModel, splits=[]):
     """Returns a fast distance function based on passed mutation_model.
 
     First, caches computed mutabilities for k-mers with k // 2 N's on either end. This
     is pretty fast for k=5, but the distance function should be created once
@@ -558,15 +577,58 @@
     sites which do match between its two sequence arguments, where ``mutability``
     is the mutation frequency of the k-mer surrounding the mutated base (in the
     first sequence argument) and ``p`` is the transition probability to the new
     base.
 
     Note that, in particular, this function is not symmetric on its  arguments.
     """
-    mutpairs, sum_minus_logp = _mutability_distance_precursors(
+    mutpairs, sum_minus_logp, _ = _mutability_distance_precursors(
         mutation_model, splits=splits
     )
 
     def distance(seq1, seq2):
         return sum_minus_logp(mutpairs(seq1, seq2))
 
     return distance
+
+
+def _context_poisson_likelihood(mutation_model: MutationModel, splits=[]):
+    mutpairs, sum_minus_logp, mutability_sum = _mutability_distance_precursors(
+        mutation_model, splits=splits
+    )
+
+    def distance(seq1, seq2):
+        subs = mutpairs(seq1, seq2)
+        sub_count = len(subs)
+        if sub_count == 0:
+            return 0
+        else:
+            mut_sum = mutability_sum(seq1)
+            substitution_sum = -sum_minus_logp(subs)
+            return (
+                substitution_sum
+                + (sub_count * (math.log(sub_count) - math.log(mut_sum)))
+                - sub_count
+            )
+
+    return distance
+
+
+def _context_poisson_likelihood_dagfuncs(*args, splits: List[int] = [], **kwargs):
+    mutation_model = MutationModel(*args, **kwargs)
+    distance = _context_poisson_likelihood(mutation_model, splits=splits)
+
+    return hdag.utils.HistoryDagFilter(
+        hdag.utils.AddFuncDict(
+            {
+                "start_func": lambda n: 0,
+                "edge_weight_func": lambda n1, n2: (
+                    0
+                    if n1.is_ua_node()
+                    else distance(n1.label.sequence, n2.label.sequence)
+                ),
+                "accum_func": sum,
+            },
+            name="LogContextLikelihood",
+        ),
+        max,
+    )
```

### Comparing `gctree-4.1.4/gctree/phylip_parse.py` & `gctree-4.2.0/gctree/phylip_parse.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.4/gctree/utils.py` & `gctree-4.2.0/gctree/utils.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.4/gctree.egg-info/PKG-INFO` & `gctree-4.2.0/gctree.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gctree
-Version: 4.1.4
+Version: 4.2.0
 Summary: phylogenetic inference of genotype-collapsed trees
 Home-page: https://github.com/matsengrp/gctree
 Author: Matsen Group
 Author-email: ematsen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `gctree-4.1.4/gctree.egg-info/SOURCES.txt` & `gctree-4.2.0/gctree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gctree-4.1.4/setup.py` & `gctree-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.4/tests/test_disambiguate.py` & `gctree-4.2.0/tests/test_disambiguate.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.4/tests/test_isotype.py` & `gctree-4.2.0/tests/test_isotype.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,13 +47,13 @@
     # idmap_file=None,
     # isotype_names=None,
     tdag = dag.copy()
     tdag.optimal_weight_annotate(**kwargs, optimal_func=lambda l: l[0])  # noqa: E741
     for node in tdag.preorder():
         if node.attr is not None:
             node.attr["isotype"] = node._dp_data
-    kwargs = _isotype_dagfuncs()
-    c = tdag.weight_count(**kwargs)
+    dag_filter = _isotype_dagfuncs()
+    c = tdag.weight_count(**dag_filter)
     key = min(c)
     count = c[key]
-    tdag.trim_optimal_weight(**kwargs, optimal_func=min)
-    assert tdag.weight_count(**kwargs) == {key: count}
+    tdag.trim_optimal_weight(**dag_filter)
+    assert tdag.weight_count(**dag_filter) == {key: count}
```

### Comparing `gctree-4.1.4/tests/test_likelihoods.py` & `gctree-4.2.0/tests/test_likelihoods.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import gctree.branching_processes as bp
 import gctree.phylip_parse as pp
 import gctree.utils as utils
+import gctree.mutation_model as mm
+from math import log
 
 import numpy as np
 from multiset import FrozenMultiset
 from oldcode import OldCollapsedTree, OldCollapsedForest
 
 
 def make_oldctree(tree):
@@ -194,7 +196,41 @@
 def test_recursion_depth():
     """Be sure ahead-of-time caching is implemented correctly to avoid
     recursion depth issues"""
     bp.CollapsedTree._ll_genotype.cache_clear()
     bp.CollapsedTree._max_ll_cache = {}
     with np.errstate(all="raise"):
         bp.CollapsedTree._ll_genotype(2, 500, 0.4, 0.6)
+
+
+def test_context_likelihood():
+    # These files will be present if pytest is run through `make test`.
+    mutation_model = mm.MutationModel(
+        mutability_file="HS5F_Mutability.csv", substitution_file="HS5F_Substitution.csv"
+    )
+    log_likelihood = mm._context_poisson_likelihood(mutation_model, splits=[])
+
+    parent_seq = "AAGAAA"
+    child_seq = "AATCAA"
+
+    term1 = sum(
+        log(
+            mutation_model.mutability(fivemer)[0]
+            * mutation_model.mutability(fivemer)[1][target_base]
+        )
+        for fivemer, target_base in [("AAGAA", "T"), ("AGAAA", "C")]
+    )
+    sum_mutabilities = sum(
+        mutation_model.mutability(fivemer)[0]
+        for fivemer in ["NNAAG", "NAAGA", "AAGAA", "AGAAA", "GAAAN", "AAANN"]
+    )
+    true_val = term1 + 2 * log(2 / sum_mutabilities) - 2
+    assert true_val == log_likelihood(parent_seq, child_seq)
+
+    # Now test chain split:
+    parent_seq = parent_seq + parent_seq
+    child_seq = child_seq + child_seq
+    # At index 6, the second concatenated sequence starts.
+    log_likelihood = mm._context_poisson_likelihood(mutation_model, splits=[6])
+
+    true_val = 2 * term1 + 4 * log(4 / (2 * sum_mutabilities)) - 4
+    assert true_val == log_likelihood(parent_seq, child_seq)
```

### Comparing `gctree-4.1.4/tests/test_local_branching.py` & `gctree-4.2.0/tests/test_local_branching.py`

 * *Files identical despite different names*

### Comparing `gctree-4.1.4/versioneer.py` & `gctree-4.2.0/versioneer.py`

 * *Files identical despite different names*

