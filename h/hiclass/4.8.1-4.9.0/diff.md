# Comparing `tmp/hiclass-4.8.1.tar.gz` & `tmp/hiclass-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiclass-4.8.1.tar", last modified: Thu Apr  4 11:01:05 2024, max compression
+gzip compressed data, was "hiclass-4.9.0.tar", last modified: Mon Apr  8 18:44:23 2024, max compression
```

## Comparing `hiclass-4.8.1.tar` & `hiclass-4.9.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:01:05.905362 hiclass-4.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-04 11:00:51.000000 hiclass-4.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 11:00:51.000000 hiclass-4.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17758 2024-04-04 11:01:05.905362 hiclass-4.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-04-04 11:00:51.000000 hiclass-4.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:01:05.905362 hiclass-4.8.1/hiclass/
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/BinaryPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/ConstantClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/Explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/HierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/LocalClassifierPerLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/LocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/LocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (127)    16260 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/MultiLabelHierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/MultiLabelLocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/MultiLabelLocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 11:01:05.905362 hiclass-4.8.1/hiclass/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:01:05.905362 hiclass-4.8.1/hiclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17758 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 11:01:05.905362 hiclass-4.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-04 11:00:51.000000 hiclass-4.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:01:05.905362 hiclass-4.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    29992 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_BinaryPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_ConstantClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_Datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_Explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_HierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_LocalClassifierPerLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_LocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_LocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_LocalClassifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_MultiLabelHierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_MultiLabelLocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (127)    12129 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_MultiLabelLocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-04-04 11:00:51.000000 hiclass-4.8.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:23.975234 hiclass-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-08 18:44:08.000000 hiclass-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 18:44:08.000000 hiclass-4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-08 18:44:23.975234 hiclass-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15646 2024-04-08 18:44:08.000000 hiclass-4.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:23.975234 hiclass-4.9.0/hiclass/
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/BinaryPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/ConstantClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/Explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/HierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/LocalClassifierPerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/LocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/LocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16260 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/MultiLabelHierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/MultiLabelLocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/MultiLabelLocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-08 18:44:23.975234 hiclass-4.9.0/hiclass/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-04-08 18:44:08.000000 hiclass-4.9.0/hiclass/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:23.975234 hiclass-4.9.0/hiclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-08 18:44:23.000000 hiclass-4.9.0/hiclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-08 18:44:23.000000 hiclass-4.9.0/hiclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:44:23.000000 hiclass-4.9.0/hiclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 18:44:23.000000 hiclass-4.9.0/hiclass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 18:44:23.000000 hiclass-4.9.0/hiclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 18:44:23.000000 hiclass-4.9.0/hiclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 18:44:23.975234 hiclass-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-08 18:44:08.000000 hiclass-4.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:23.975234 hiclass-4.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29992 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_BinaryPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_ConstantClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_Datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_Explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_HierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_LocalClassifierPerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_LocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_LocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_LocalClassifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_MultiLabelHierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_MultiLabelLocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12129 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_MultiLabelLocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-08 18:44:08.000000 hiclass-4.9.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-04-08 18:44:08.000000 hiclass-4.9.0/versioneer.py
```

### Comparing `hiclass-4.8.1/LICENSE` & `hiclass-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/PKG-INFO` & `hiclass-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiclass
-Version: 4.8.1
+Version: 4.9.0
 Summary: Hierarchical Classification Library.
 Author: Fabio Malcher Miranda, Niklas Koehnecke
 Author-email: fabio.malchermiranda@hpi.de, Niklas.Koehnecke@student.hpi.uni-potsdam.de
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/scikit-learn-contrib/hiclass/issues
 Project-URL: Source Code, https://github.com/scikit-learn-contrib/hiclass
 Project-URL: Related Software, https://gitlab.com/dacs-hpi
@@ -27,14 +27,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
+Requires-Dist: scipy<1.13
 Provides-Extra: ray
 Requires-Dist: ray>=1.11.0; extra == "ray"
 Provides-Extra: xai
 Requires-Dist: shap==0.44.1; extra == "xai"
 Requires-Dist: xarray==2023.1.0; extra == "xai"
 Provides-Extra: dev
 Requires-Dist: flake8==4.0.1; extra == "dev"
@@ -251,15 +252,15 @@
 pipeline.fit(X_train, Y_train)
 
 # Predict
 predictions = pipeline.predict(X_test)
 ```
 
 ## Explaining Hierarchical Classifiers
-Hierarchical classifiers can provide additional insights when combined with explainability methods. HiClass allows explaining hierarchical models using SHAP values. Different hierarchical models yield different insights. More information on explaining [Local classifier per parent node](https://colab.research.google.com/drive/1rVlYuRU_uO1jw5sD6qo2HoCpCz6E6z5J?usp=sharing), [Local classifier per node](), and [Local classifier per level]() is available on [Read the Docs](https://hiclass.readthedocs.io/en/latest/algorithms/explainer.html).
+Hierarchical classifiers can provide additional insights when combined with explainability methods. HiClass allows explaining hierarchical models using SHAP values. Different hierarchical models yield different insights. More information on explaining [Local classifier per parent node](https://colab.research.google.com/drive/1rVlYuRU_uO1jw5sD6qo2HoCpCz6E6z5J?usp=sharing), [Local classifier per node](https://colab.research.google.com/drive/1wqSl1t_Qn2f62WNZQ48mdB0mNeu1XSF1?usp=sharing), and [Local classifier per level]() is available on [Read the Docs](https://hiclass.readthedocs.io/en/latest/algorithms/explainer.html).
 
 ## Step-by-step walk-through
 
 A step-by-step walk-through is available on our documentation hosted on [Read the Docs](https://hiclass.readthedocs.io/en/latest/index.html).
 
 This will guide you through the process of installing hiclass within a virtual environment, training, predicting, persisting models and much more.
```

### Comparing `hiclass-4.8.1/README.md` & `hiclass-4.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 pipeline.fit(X_train, Y_train)
 
 # Predict
 predictions = pipeline.predict(X_test)
 ```
 
 ## Explaining Hierarchical Classifiers
-Hierarchical classifiers can provide additional insights when combined with explainability methods. HiClass allows explaining hierarchical models using SHAP values. Different hierarchical models yield different insights. More information on explaining [Local classifier per parent node](https://colab.research.google.com/drive/1rVlYuRU_uO1jw5sD6qo2HoCpCz6E6z5J?usp=sharing), [Local classifier per node](), and [Local classifier per level]() is available on [Read the Docs](https://hiclass.readthedocs.io/en/latest/algorithms/explainer.html).
+Hierarchical classifiers can provide additional insights when combined with explainability methods. HiClass allows explaining hierarchical models using SHAP values. Different hierarchical models yield different insights. More information on explaining [Local classifier per parent node](https://colab.research.google.com/drive/1rVlYuRU_uO1jw5sD6qo2HoCpCz6E6z5J?usp=sharing), [Local classifier per node](https://colab.research.google.com/drive/1wqSl1t_Qn2f62WNZQ48mdB0mNeu1XSF1?usp=sharing), and [Local classifier per level]() is available on [Read the Docs](https://hiclass.readthedocs.io/en/latest/algorithms/explainer.html).
 
 ## Step-by-step walk-through
 
 A step-by-step walk-through is available on our documentation hosted on [Read the Docs](https://hiclass.readthedocs.io/en/latest/index.html).
 
 This will guide you through the process of installing hiclass within a virtual environment, training, predicting, persisting models and much more.
```

### Comparing `hiclass-4.8.1/hiclass/BinaryPolicy.py` & `hiclass-4.9.0/hiclass/BinaryPolicy.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass/ConstantClassifier.py` & `hiclass-4.9.0/hiclass/ConstantClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass/Explainer.py` & `hiclass-4.9.0/hiclass/Explainer.py`

 * *Files 15% similar despite different names*

```diff
@@ -185,14 +185,54 @@
                             predecessor
                         ]["classifier"]
                         traversals[mask, level] = classifier.predict(
                             predecessor_x
                         ).flatten()
         return traversals
 
+    def _get_traversed_nodes_lcpn(self, samples):
+        """
+        Return a list of all traversed nodes as per the provided LocalClassifierPerNode model.
+
+        Parameters
+        ----------
+        samples : array-like
+            Sample data for which to generate traversed nodes.
+
+        Returns
+        -------
+        traversals : list
+            A list of all traversed nodes as per LocalClassifierPerNode (LCPN) strategy.
+        """
+        traversals = np.empty(
+            (samples.shape[0], self.hierarchical_model.max_levels_),
+            dtype=self.hierarchical_model.dtype_,
+        )
+
+        predictions = self.hierarchical_model.predict(samples)
+
+        traversals[:, 0] = predictions[:, 0]
+        separator = np.full(
+            (samples.shape[0], 3),
+            self.hierarchical_model.separator_,
+            dtype=self.hierarchical_model.dtype_,
+        )
+
+        for level in range(1, traversals.shape[1]):
+            traversals[:, level] = np.char.add(
+                traversals[:, level - 1],
+                np.char.add(separator[:, 0], predictions[:, level]),
+            )
+
+        # For inconsistent hierarchies, levels with empty nodes should be ignored
+        mask = predictions == ""
+        traversals[mask] = ""
+
+        return traversals
+
     def _calculate_shap_values(self, X):
         """
         Return an xarray.Dataset object for a single sample provided. This dataset is aligned on the `level` attribute.
 
         Parameters
         ----------
         X : array-like
@@ -202,19 +242,24 @@
         -------
         explanation : xarray.Dataset
             A single explanation for the prediction of given sample.
         """
         traversed_nodes = []
         if isinstance(self.hierarchical_model, LocalClassifierPerParentNode):
             traversed_nodes = self._get_traversed_nodes_lcppn(X)[0]
+        elif isinstance(self.hierarchical_model, LocalClassifierPerNode):
+            traversed_nodes = self._get_traversed_nodes_lcpn(X)[0]
         datasets = []
         level = 0
         for node in traversed_nodes:
-            # Skip if classifier is not found, can happen in case of imbalanced hierarchies
-            if "classifier" not in self.hierarchical_model.hierarchy_.nodes[node]:
+            # Skip if node is empty or classifier is not found, can happen in case of imbalanced hierarchies
+            if (
+                node == ""
+                or "classifier" not in self.hierarchical_model.hierarchy_.nodes[node]
+            ):
                 continue
 
             local_classifier = self.hierarchical_model.hierarchy_.nodes[node][
                 "classifier"
             ]
 
             # Create a SHAP explainer for the local classifier
```

### Comparing `hiclass-4.8.1/hiclass/HierarchicalClassifier.py` & `hiclass-4.9.0/hiclass/HierarchicalClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass/LocalClassifierPerLevel.py` & `hiclass-4.9.0/hiclass/LocalClassifierPerLevel.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass/LocalClassifierPerNode.py` & `hiclass-4.9.0/hiclass/LocalClassifierPerNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass/LocalClassifierPerParentNode.py` & `hiclass-4.9.0/hiclass/LocalClassifierPerParentNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass/MultiLabelHierarchicalClassifier.py` & `hiclass-4.9.0/hiclass/MultiLabelHierarchicalClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass/MultiLabelLocalClassifierPerNode.py` & `hiclass-4.9.0/hiclass/MultiLabelLocalClassifierPerNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass/MultiLabelLocalClassifierPerParentNode.py` & `hiclass-4.9.0/hiclass/MultiLabelLocalClassifierPerParentNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass/__init__.py` & `hiclass-4.9.0/hiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass/datasets.py` & `hiclass-4.9.0/hiclass/datasets.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass/metrics.py` & `hiclass-4.9.0/hiclass/metrics.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/hiclass.egg-info/PKG-INFO` & `hiclass-4.9.0/hiclass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiclass
-Version: 4.8.1
+Version: 4.9.0
 Summary: Hierarchical Classification Library.
 Author: Fabio Malcher Miranda, Niklas Koehnecke
 Author-email: fabio.malchermiranda@hpi.de, Niklas.Koehnecke@student.hpi.uni-potsdam.de
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/scikit-learn-contrib/hiclass/issues
 Project-URL: Source Code, https://github.com/scikit-learn-contrib/hiclass
 Project-URL: Related Software, https://gitlab.com/dacs-hpi
@@ -27,14 +27,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
+Requires-Dist: scipy<1.13
 Provides-Extra: ray
 Requires-Dist: ray>=1.11.0; extra == "ray"
 Provides-Extra: xai
 Requires-Dist: shap==0.44.1; extra == "xai"
 Requires-Dist: xarray==2023.1.0; extra == "xai"
 Provides-Extra: dev
 Requires-Dist: flake8==4.0.1; extra == "dev"
@@ -251,15 +252,15 @@
 pipeline.fit(X_train, Y_train)
 
 # Predict
 predictions = pipeline.predict(X_test)
 ```
 
 ## Explaining Hierarchical Classifiers
-Hierarchical classifiers can provide additional insights when combined with explainability methods. HiClass allows explaining hierarchical models using SHAP values. Different hierarchical models yield different insights. More information on explaining [Local classifier per parent node](https://colab.research.google.com/drive/1rVlYuRU_uO1jw5sD6qo2HoCpCz6E6z5J?usp=sharing), [Local classifier per node](), and [Local classifier per level]() is available on [Read the Docs](https://hiclass.readthedocs.io/en/latest/algorithms/explainer.html).
+Hierarchical classifiers can provide additional insights when combined with explainability methods. HiClass allows explaining hierarchical models using SHAP values. Different hierarchical models yield different insights. More information on explaining [Local classifier per parent node](https://colab.research.google.com/drive/1rVlYuRU_uO1jw5sD6qo2HoCpCz6E6z5J?usp=sharing), [Local classifier per node](https://colab.research.google.com/drive/1wqSl1t_Qn2f62WNZQ48mdB0mNeu1XSF1?usp=sharing), and [Local classifier per level]() is available on [Read the Docs](https://hiclass.readthedocs.io/en/latest/algorithms/explainer.html).
 
 ## Step-by-step walk-through
 
 A step-by-step walk-through is available on our documentation hosted on [Read the Docs](https://hiclass.readthedocs.io/en/latest/index.html).
 
 This will guide you through the process of installing hiclass within a virtual environment, training, predicting, persisting models and much more.
```

### Comparing `hiclass-4.8.1/hiclass.egg-info/SOURCES.txt` & `hiclass-4.9.0/hiclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/setup.py` & `hiclass-4.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 URL_ISSUES = "https://github.com/scikit-learn-contrib/hiclass/issues"
 EMAIL = "fabio.malchermiranda@hpi.de, Niklas.Koehnecke@student.hpi.uni-potsdam.de"
 AUTHOR = "Fabio Malcher Miranda, Niklas Koehnecke"
 REQUIRES_PYTHON = ">=3.8,<3.12"
 KEYWORDS = ["hierarchical classification"]
 DACS_SOFTWARE = "https://gitlab.com/dacs-hpi"
 # What packages are required for this module to be executed?
-REQUIRED = ["networkx", "numpy", "scikit-learn"]
+REQUIRED = ["networkx", "numpy", "scikit-learn", "scipy<1.13"]
 
 # What packages are optional?
 # 'fancy feature': ['django'],}
 EXTRAS = {
     "ray": ["ray>=1.11.0"],
     "xai": ["shap==0.44.1", "xarray==2023.1.0"],
     "dev": [
```

### Comparing `hiclass-4.8.1/tests/test_BinaryPolicy.py` & `hiclass-4.9.0/tests/test_BinaryPolicy.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/tests/test_ConstantClassifier.py` & `hiclass-4.9.0/tests/test_ConstantClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/tests/test_Datasets.py` & `hiclass-4.9.0/tests/test_Datasets.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/tests/test_Explainer.py` & `hiclass-4.9.0/tests/test_Explainer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import numpy as np
 import pytest
 from sklearn.ensemble import RandomForestClassifier
-from hiclass import (
-    LocalClassifierPerParentNode,
-    Explainer,
-)
+from hiclass import LocalClassifierPerNode, LocalClassifierPerParentNode, Explainer
 
 try:
     import shap
 except ImportError:
     shap_installed = False
 else:
     shap_installed = True
@@ -73,14 +70,39 @@
         y_pred = y_preds[i]
         explanation = explanations["predicted_class"][i]
         for j in range(len(y_pred)):
             assert explanation.data[j].split(lcppn.separator_)[-1] == y_pred[j]
 
 
 @pytest.mark.skipif(not shap_installed, reason="shap not installed")
+@pytest.mark.skipif(not xarray_installed, reason="xarray not installed")
+@pytest.mark.parametrize("data", ["explainer_data", "explainer_data_no_root"])
+def test_explainer_tree_lcpn(data, request):
+    rfc = RandomForestClassifier()
+    lcpn = LocalClassifierPerNode(local_classifier=rfc, replace_classifiers=False)
+
+    x_train, x_test, y_train = request.getfixturevalue(data)
+
+    lcpn.fit(x_train, y_train)
+
+    explainer = Explainer(lcpn, data=x_train, mode="tree")
+    explanations = explainer.explain(x_test)
+
+    # Assert if explainer returns an xarray.Dataset object
+    assert isinstance(explanations, xarray.Dataset)
+    y_preds = lcpn.predict(x_test)
+
+    # Assert if predictions made are consistent with the explanation object
+    for i in range(len(x_test)):
+        y_pred = y_preds[i]
+        for j in range(len(y_pred)):
+            assert str(explanations["node"][i].data[j]) == y_pred[j]
+
+
+@pytest.mark.skipif(not shap_installed, reason="shap not installed")
 @pytest.mark.parametrize("data", ["explainer_data", "explainer_data_no_root"])
 def test_traversal_path_lcppn(data, request):
     x_train, x_test, y_train = request.getfixturevalue(data)
     rfc = RandomForestClassifier()
     lcppn = LocalClassifierPerParentNode(
         local_classifier=rfc, replace_classifiers=False
     )
@@ -95,44 +117,72 @@
             if traversals[i][j] == lcppn.root_:
                 continue
             label = traversals[i][j].split(lcppn.separator_)[-1]
             assert label == preds[i][j - 1]
 
 
 @pytest.mark.skipif(not shap_installed, reason="shap not installed")
+@pytest.mark.parametrize("data", ["explainer_data", "explainer_data_no_root"])
+def test_traversal_path_lcpn(data, request):
+    x_train, x_test, y_train = request.getfixturevalue(data)
+    rfc = RandomForestClassifier()
+    lcpn = LocalClassifierPerNode(local_classifier=rfc, replace_classifiers=False)
+
+    lcpn.fit(x_train, y_train)
+    explainer = Explainer(lcpn, data=x_train, mode="tree")
+    traversals = explainer._get_traversed_nodes_lcpn(x_test)
+    preds = lcpn.predict(x_test)
+
+    # Assert if predictions and traversals are of same length
+    assert len(preds) == len(traversals)
+
+    # Assert if traversal path in predictions is same as the computed traversal path
+    for i in range(len(x_test)):
+        for j in range(len(traversals[i])):
+            label = traversals[i][j].split(lcpn.separator_)[-1]
+            assert label == preds[i][j]
+
+
+@pytest.mark.skipif(not shap_installed, reason="shap not installed")
 @pytest.mark.skipif(not xarray_installed, reason="xarray not installed")
 @pytest.mark.parametrize("data", ["explainer_data", "explainer_data_no_root"])
-@pytest.mark.parametrize("classifier", [LocalClassifierPerParentNode])
+@pytest.mark.parametrize(
+    "classifier", [LocalClassifierPerParentNode, LocalClassifierPerNode]
+)
 def test_explain_with_xr(data, request, classifier):
     x_train, x_test, y_train = request.getfixturevalue(data)
     rfc = RandomForestClassifier()
     clf = classifier(local_classifier=rfc, replace_classifiers=False)
 
     clf.fit(x_train, y_train)
     explainer = Explainer(clf, data=x_train, mode="tree")
     explanations = explainer._explain_with_xr(x_test)
 
     # Assert if explainer returns an xarray.Dataset object
     assert isinstance(explanations, xarray.Dataset)
 
 
-@pytest.mark.parametrize("classifier", [LocalClassifierPerParentNode])
+@pytest.mark.parametrize(
+    "classifier", [LocalClassifierPerParentNode, LocalClassifierPerNode]
+)
 def test_imports(classifier):
     x_train = [[76, 12, 49], [88, 63, 31], [5, 42, 24], [17, 90, 55]]
     y_train = [["a", "b", "d"], ["a", "b", "e"], ["a", "c", "f"], ["a", "c", "g"]]
 
     rfc = RandomForestClassifier()
     clf = classifier(local_classifier=rfc, replace_classifiers=False)
     clf.fit(x_train, y_train)
 
     explainer = Explainer(clf, data=x_train, mode="tree")
     assert isinstance(explainer.data, np.ndarray)
 
 
-@pytest.mark.parametrize("classifier", [LocalClassifierPerParentNode])
+@pytest.mark.parametrize(
+    "classifier", [LocalClassifierPerParentNode, LocalClassifierPerNode]
+)
 @pytest.mark.parametrize("data", ["explainer_data"])
 @pytest.mark.parametrize("mode", ["linear", "gradient", "deep", "tree", ""])
 def test_explainers(data, request, classifier, mode):
     x_train, x_test, y_train = request.getfixturevalue(data)
     rfc = RandomForestClassifier()
     clf = classifier(local_classifier=rfc, replace_classifiers=False)
```

### Comparing `hiclass-4.8.1/tests/test_HierarchicalClassifier.py` & `hiclass-4.9.0/tests/test_HierarchicalClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/tests/test_LocalClassifierPerLevel.py` & `hiclass-4.9.0/tests/test_LocalClassifierPerLevel.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/tests/test_LocalClassifierPerNode.py` & `hiclass-4.9.0/tests/test_LocalClassifierPerNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/tests/test_LocalClassifierPerParentNode.py` & `hiclass-4.9.0/tests/test_LocalClassifierPerParentNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/tests/test_LocalClassifiers.py` & `hiclass-4.9.0/tests/test_LocalClassifiers.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/tests/test_MultiLabelHierarchicalClassifier.py` & `hiclass-4.9.0/tests/test_MultiLabelHierarchicalClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/tests/test_MultiLabelLocalClassifierPerNode.py` & `hiclass-4.9.0/tests/test_MultiLabelLocalClassifierPerNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/tests/test_MultiLabelLocalClassifierPerParentNode.py` & `hiclass-4.9.0/tests/test_MultiLabelLocalClassifierPerParentNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/tests/test_metrics.py` & `hiclass-4.9.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.1/versioneer.py` & `hiclass-4.9.0/versioneer.py`

 * *Files identical despite different names*

