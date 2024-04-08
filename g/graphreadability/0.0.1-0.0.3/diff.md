# Comparing `tmp/graphreadability-0.0.1.tar.gz` & `tmp/graphreadability-0.0.3.tar.gz`

## Comparing `graphreadability-0.0.1.tar` & `graphreadability-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,31 @@
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/__init__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/core/__init__.py
--rw-r--r--   0        0        0    11186 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/core/metricssuite.py
--rw-r--r--   0        0        0     9412 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/core/readabilitygraph.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/io/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/io/cytoscape_api.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/io/gefx_reader.py
--rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/io/graphml_reader.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/layout/__init__.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/layout/layout_algorithms.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/metrics/__init__.py
--rw-r--r--   0        0        0    29701 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/metrics/metrics.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/tests/__init__.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/tests/test_graphreadability.py
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/tests/test_helpers.py
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/tests/test_metricssuite.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/utils/__init__.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/utils/crosses_promotion.py
--rw-r--r--   0        0        0    16679 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/utils/helpers.py
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 graphreadability-0.0.1/src/utils/apps/digitize_graphs.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 graphreadability-0.0.1/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 graphreadability-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 graphreadability-0.0.1/README.md
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 graphreadability-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 graphreadability-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 graphreadability-0.0.3/_version.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/__init__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/core/__init__.py
+-rw-r--r--   0        0        0    11097 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/core/metricssuite.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/io/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/io/cytoscape_api.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/io/gefx_reader.py
+-rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/io/graphml_reader.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/layout/__init__.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/layout/layout_algorithms.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/metrics/__init__.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/metrics/metric_helpers.py
+-rw-r--r--   0        0        0    23164 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/metrics/metrics.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/tests/__init__.py
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/tests/test_helpers.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/tests/test_metric_helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/tests/test_metrics.py
+-rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/tests/test_metricssuite.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/tests/test_data/cube.graphml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/tests/test_data/pretty_print_output.txt
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/tests/test_data/squares.graphml
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/tests/test_data/star.graphml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/utils/__init__.py
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/utils/crosses_promotion.py
+-rw-r--r--   0        0        0    16998 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/utils/helpers.py
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 graphreadability-0.0.3/graphreadability/utils/apps/digitize_graphs.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 graphreadability-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 graphreadability-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 graphreadability-0.0.3/README.md
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 graphreadability-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 graphreadability-0.0.3/PKG-INFO
```

### Comparing `graphreadability-0.0.1/src/__init__.py` & `graphreadability-0.0.3/graphreadability/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 __version__ = "0.0.1"
 __author__ = "Philip Mathieu"
 __license__ = "Apache-2.0"
 __description__ = "A Python package for calculating readability metrics for graph and network visualizations."
 
 # Import core modules
 from .core.metricssuite import MetricsSuite
-from .core.readabilitygraph import ReadabilityGraph
 
 # Import layout algorithms
-from .layout.layout_algorithms import naive_optimizer
+from .layout import layout_algorithms
 
 # Import utils
 from .utils import helpers
 from .utils import crosses_promotion
 
 # Import tests
 from . import tests
 
 __all__ = [
     "MetricsSuite",
     "ReadabilityGraph",
-    "naive_optimizer",
+    "layout_algorithms",
     "helpers",
     "crosses_promotion",
     "tests",
 ]
```

### Comparing `graphreadability-0.0.1/src/core/metricssuite.py` & `graphreadability-0.0.3/graphreadability/core/metricssuite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import math
-import time
 from typing import Optional, Union, Sequence
 import networkx as nx
 from ..metrics import metrics
 
 # Generate the list of metric functions
 METRIC_FUNCS = [
     func
     for func in dir(metrics)
-    if callable(getattr(metrics, func)) and not func.startswith("__")
+    if callable(getattr(metrics, func)) and not func.startswith("_")
 ]
 
 # Set default weights for all metrics
 DEFAULT_WEIGHTS = {func: 1 for func in METRIC_FUNCS}
 
 # Generate the dictionary of metric functions
 METRICS = {func: {"func": getattr(metrics, func)} for func in METRIC_FUNCS}
@@ -37,54 +36,58 @@
         The tolerance for symmetry detection. Default is 3.
     file_type : str, optional
         The file type of the graph file. Default is "GraphML".
     """
 
     def __init__(
         self,
-        graph: Union[nx.Graph, str] = None,
+        G: Union[nx.Graph, str] = None,
         metric_weights: Optional[dict] = DEFAULT_WEIGHTS,
         metric_combination_strategy: str = "weighted_sum",
         sym_threshold: Union[int, float] = 2,
         sym_tolerance: Union[int, float] = 3,
         file_type: str = "GraphML",
+        copy=False,
     ):
         # Dictionary mapping metric combination strategies to their functions
         self.metric_combination_strategies = {
             "weighted_sum": self.weighted_sum,
             "weighted_prod": self.weighted_prod,
         }
         # Placeholder for version of graph with crosses promoted to nodes
         self.graph_cross_promoted = None
         # Dictionary mapping metric names to their functions, values, and weights
         self.metrics = METRICS.copy()
         for k in self.metrics.keys():
-            self.metrics[k].update({"weight": 0, "value": None, "is_calculated": False})
+            self.metrics[k].update({"weight": None, "value": None})
 
         # Check all metrics given are valid and assign weights
         self.initial_weights = self.set_weights(metric_weights)
 
         # Check metric combination strategy is valid
         assert (
             metric_combination_strategy in self.metric_combination_strategies
         ), f"Unknown metric combination strategy: {metric_combination_strategy}. Available strategies: {list(self.metric_combination_strategies.keys())}"
         self.metric_combination_strategy = metric_combination_strategy
 
-        if graph is None:
+        if G is None:
             self._filename = ""
-            self._graph = self.load_graph_test()
-        elif isinstance(graph, str):
-            self._filename = graph
-            self._graph = self.load_graph(graph, file_type=file_type)
-        elif isinstance(graph, nx.Graph):
+            self.G = self.load_graph_test()
+        elif isinstance(G, str):
+            self._filename = G
+            self.G = self.load_graph(G, file_type=file_type)
+        elif isinstance(G, nx.Graph):
             self._filename = ""
-            self._graph = graph
+            if copy:
+                self.G = G.copy()
+            else:
+                self.G = G
         else:
             raise TypeError(
-                f"'graph' must be a string representing a path to a GML or GraphML file, or a NetworkX Graph object, not {type(graph)}"
+                f"'graph' must be a string representing a path to a GML or GraphML file, or a NetworkX Graph object, not {type(G)}"
             )
 
         if sym_tolerance < 0:
             raise ValueError("sym_tolerance must be positive.")
 
         self.sym_tolerance = sym_tolerance
 
@@ -106,25 +109,25 @@
         return (
             f"MetricsSuite({self._filename}) object with {len(self.metrics)} metrics."
         )
 
     def __copy__(self):
         """Return a shallow copy of the MetricsSuite object."""
         return MetricsSuite(
-            graph=self._graph,
+            G=self.G,
             metric_weights=self.initial_weights,
             metric_combination_strategy=self.metric_combination_strategy,
             sym_threshold=self.sym_threshold,
             sym_tolerance=self.sym_tolerance,
         )
 
     def __deepcopy__(self, memo):
         """Return a deep copy of the MetricsSuite object."""
         return MetricsSuite(
-            graph=self._graph.copy(),
+            G=self.G.copy(),
             metric_weights=self.initial_weights,
             metric_combination_strategy=self.metric_combination_strategy,
             sym_threshold=self.sym_threshold,
             sym_tolerance=self.sym_tolerance,
         )
 
     def load_graph_test(self, nxg=nx.sedgewick_maze_graph):
@@ -153,26 +156,25 @@
             Dictionary of metric:weight key/values.
 
         Returns
         -------
         dict
             Dictionary of metric:weight key/values for metrics with non-zero weights.
         """
-        metrics_to_remove = [
-            metric for metric, weight in metric_weights.items() if weight <= 0
-        ]
+        metric_weights = {
+            metric: weight for metric, weight in metric_weights.items() if weight > 0
+        }
 
         if any(metric_weights[metric] < 0 for metric in metric_weights):
             raise ValueError("Metric weights must be positive.")
 
-        for metric in metrics_to_remove:
-            metric_weights.pop(metric)
-
-        for metric in metric_weights:
-            self.metrics[metric]["weight"] = metric_weights[metric]
+        for metric in self.metrics:
+            self.metrics[metric]["weight"] = (
+                metric_weights[metric] if metric in metric_weights else None
+            )
 
         return {
             metric: weight for metric, weight in metric_weights.items() if weight > 0
         }
 
     def apply_layout(self, pos):
         """Applies the given layout to the graph.
@@ -184,101 +186,98 @@
 
         Returns
         -------
         None
         """
         # Convert to x and y attributes
         xy = {k: {"x": v[0], "y": v[1]} for k, v in pos.items()}
-        nx.set_node_attributes(self._graph, xy)
+        nx.set_node_attributes(self.G, xy)
 
     def calculate_metric(self, metric: str = None):
         """Calculate the value of the given metric by calling the associated function."""
         if metric is None:
             raise ValueError(
                 "No metric provided. Did you mean to call calculate_metrics()?"
             )
 
-        if not self.metrics[metric]["is_calculated"]:
-            try:
-                self.metrics[metric]["value"] = self.metrics[metric]["func"](
-                    self._graph
-                )
-                self.metrics[metric]["is_calculated"] = True
-            except Exception as e:
-                print(f"Error calculating metric {metric}: {e}")
-                self.metrics[metric]["value"] = None
-                self.metrics[metric]["is_calculated"] = False
-        else:
-            pass
+        try:
+            self.metrics[metric]["value"] = self.metrics[metric]["func"](self.G)
+        except Exception as e:
+            print(f"Error calculating metric {metric}: {e}")
+            self.metrics[metric]["value"] = None
 
-    def calculate_metrics(self):
+    def calculate_metrics(self, calculate_all=False):
         """Calculates the values of all metrics with non-zero weights."""
-        start_time = time.perf_counter()
         n_metrics = 0
         for metric in self.metrics:
-            if self.metrics[metric]["weight"] != 0:
+            if self.metrics[metric]["weight"] is not None or calculate_all:
                 self.calculate_metric(metric)
                 n_metrics += 1
-        end_time = time.perf_counter()
-        print(
-            f"Calculated {n_metrics} metrics in {end_time - start_time:0.3f} seconds."
-        )
 
     def reset_metrics(self):
         """Resets all metric values and is_calculated flags to None and False, respectively."""
         for metric in self.metrics:
             self.metrics[metric]["value"] = None
             self.metrics[metric]["is_calculated"] = False
 
     def weighted_prod(self):
         """Returns the weighted product of all metrics. Should NOT be used as a cost function - may be useful for comparing graphs."""
+        used_metrics = [
+            metric
+            for metric in self.metrics.keys()
+            if self.metrics[metric]["weight"] is not None
+        ]
+        for metric in used_metrics:
+            if self.metrics[metric]["value"] is None:
+                self.calculate_metric(metric)
         return math.prod(
             self.metrics[metric]["value"] * self.metrics[metric]["weight"]
-            for metric in self.initial_weights
+            for metric in used_metrics
         )
 
     def weighted_sum(self):
         """Returns the weighted sum of all metrics. Can be used as a cost function."""
-        total_weight = sum(
-            self.metrics[metric]["weight"]
-            for metric in self.metrics
-            if self.metrics[metric]["value"] is not None
-        )
+        used_metrics = [
+            metric
+            for metric in self.metrics.keys()
+            if self.metrics[metric]["weight"] is not None
+        ]
+        total_weight = sum(self.metrics[metric]["weight"] for metric in used_metrics)
         return (
             sum(
                 self.metrics[metric]["value"] * self.metrics[metric]["weight"]
-                for metric in self.initial_weights
-                if self.metrics[metric]["value"] is not None
+                for metric in used_metrics
             )
             / total_weight
         )
 
-    def combine_metrics(self):
+    def combine_metrics(self, calculate=True):
         """Combine several metrics based on the given multiple criteria decision analysis technique."""
         # Important to loop over initial weights to avoid checking the weight of all metrics when they are not needed
-        [self.calculate_metric(metric) for metric in self.initial_weights]
+        if calculate:
+            self.calculate_metrics()
         return self.metric_combination_strategies[self.metric_combination_strategy]()
 
-    def pretty_print_metrics(self):
+    def pretty_print_metrics(self, calculate=False):
         """Prints all metrics and their values in an easily digestible view."""
-        combined = self.combine_metrics()
+        combined = self.combine_metrics(calculate=calculate)
         print("-" * 50)
         print("{:<30s}Value\tWeight".format("Metric"))
         print("-" * 50)
         for k, v in self.metrics.items():
             if v["value"]:
                 val_str = f"{v['value']:.3f}"
                 print(f"{k:<30s}{val_str:<5s}\t{v['weight']}")
             else:
                 print(f"{k:<30s}{str(v['value']):<5s}\t{v['weight']}")
         print("-" * 50)
         print(f"Evaluation using {self.metric_combination_strategy}: {combined:.5f}")
         print("-" * 50)
 
-    def metric_table(self):
+    def metric_table(self, calculate=False):
         """Returns a dictionary of metrics and their values. Designed to work with pandas from_records() method."""
-        combined = self.combine_metrics()
+        combined = self.combine_metrics(calculate)
         metrics = {}
         for k, v in self.metrics.items():
             metrics[k] = v["value"]
-        metrics["Combined"] = combined
+        metrics["combined"] = combined
         return metrics
```

### Comparing `graphreadability-0.0.1/src/io/graphml_reader.py` & `graphreadability-0.0.3/graphreadability/io/graphml_reader.py`

 * *Files identical despite different names*

### Comparing `graphreadability-0.0.1/src/layout/layout_algorithms.py` & `graphreadability-0.0.3/graphreadability/layout/layout_algorithms.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,19 +31,24 @@
         "kamada_kawai": nx.kamada_kawai_layout,
     }
 
     scores = {}
     poss = {}
     for layout_name, layout_func in layouts.items():
         M = M_input.copy() if not inplace else M_input
-        poss[layout_name] = layout_func(M._graph)
+        poss[layout_name] = layout_func(M.G)
         M.apply_layout(poss[layout_name])
         M.calculate_metrics()
         scores[layout_name] = M.combine_metrics()
 
     # Choose the best layout
     best_layout = max(scores, key=scores.get)
     M = M_input.copy() if not inplace else M_input
     M.apply_layout(poss[best_layout])
 
     print(f"Best layout: {best_layout}. Score: {scores[best_layout]}")
     return M
+
+
+def optimize(M_input: MetricsSuite, inplace=False):
+    """Default optimizer for the graph layout."""
+    return naive_optimizer(M_input, inplace=inplace)
```

### Comparing `graphreadability-0.0.1/src/metrics/metrics.py` & `graphreadability-0.0.3/graphreadability/metrics/metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,186 +5,22 @@
 
 import random as rand
 import numpy as np
 import networkx as nx
 from scipy.spatial import ConvexHull as __ConvexHull
 from ..utils import helpers
 from ..utils import crosses_promotion
+from ..metrics.metric_helpers import (
+    _count_impossible_triangle_crossings,
+    _count_4_cycles,
+    _calculate_edge_crossings,
+)
 
 
-def __count_impossible_triangle_crossings(G):
-    """Count the number of impossible triangle crossings in a graph.
-
-    An impossible triangle crossing is a crossing that cannot exist due to the geometry of the triangles involved.
-    The most crossings that can occur between two triangles is six. If the two triangles share a node, this number
-    decreases to four. If the two triangles share an edge, this number decreases to two. If the two triangles are the
-    same, this number decreases to zero.
-
-    Parameters
-    ----------
-    G : nx.Graph
-        The graph to calculate impossible triangle crossings for.
-
-    Returns
-    -------
-    total_impossible : int
-        The total number of impossible triangle crossings in the graph.
-    """
-    # Create a list of sets of three nodes that form a triangle
-    triangles = []
-    for u, v in G.edges():
-        for t in G.neighbors(u):
-            if v in G.neighbors(t) and {u, v, t} not in triangles:
-                triangles.append({u, v, t})
-
-    # Create a list of the edge sets of the triangles
-    triangle_edges = []
-    for u, v, t in triangles:
-        if {u, v} not in triangle_edges:
-            triangle_edges.append({u, v})
-        if {v, t} not in triangle_edges:
-            triangle_edges.append({v, t})
-        if {t, u} not in triangle_edges:
-            triangle_edges.append({t, u})
-
-    # Count the number of impossible triangles
-    total_impossible = 0
-    for u, v, t in triangles:
-        # Get the edges of the triangle
-        bubble = []
-        bubble.extend(G.edges(u))
-        bubble.extend(G.edges(v))
-        bubble.extend(G.edges(t))
-
-        # Create a subgraph of the triangle
-        subG = nx.Graph(bubble)
-
-        # Iterate over the edges in the input graph
-        for a, b in G.edges():
-            # Skip the edges of the subgraph
-            if (a, b) in subG.edges() or (b, a) in subG.edges():
-                continue
-
-            # Skip the edges that are part of a triangle
-            if {a, b} in triangle_edges:
-                continue
-
-            total_impossible += 1
-
-    for i, triangle in enumerate(triangles):
-        u, v, t = triangle
-        for a, b, c in triangles[i + 1 :]:
-            # Skip the same triangle
-            if {u, v, t} == {a, b, c}:
-                continue
-
-            # Triangles share an edge
-            if any(
-                ({u, v} == {a, b} or {u, v} == {b, c} or {u, v} == {c, a}),
-                ({v, t} == {a, b} or {v, t} == {b, c} or {v, t} == {c, a}),
-                ({t, u} == {a, b} or {t, u} == {b, c} or {t, u} == {c, a}),
-            ):
-
-                total_impossible += 1
-                continue
-
-            # Triangles share a node
-            if any(
-                (u == a or u == b or u == c),
-                (v == a or v == b or v == c),
-                (t == a or t == b or t == c),
-            ):
-                total_impossible += 2
-                continue
-
-            # All crossings are possible
-            total_impossible += 3
-
-    num_4_cycles = 0
-    for u, v in G.edges():
-        for t in G.neighbors(u):
-            if t == v:
-                continue
-
-            for w in G.neighbors(v):
-                if w == t or w == u:
-                    continue
-
-                if w in G.neighbors(t):
-                    square = G.subgraph([u, v, t, w])
-                    num_adj = 0
-
-                    for su, sv in square.edges():
-                        if {su, sv} in triangle_edges:
-                            num_adj += 1
-
-                    if num_adj < 2:
-                        num_4_cycles += 1
-
-    return total_impossible + (num_4_cycles // 4)
-
-
-def __calculate_edge_crossings(G, save_edge_attributes=True):
-    """Calculate all edge crossings in a graph and save them to the edge data.
-
-    Parameters
-    ----------
-    G : nx.Graph
-        The graph to calculate edge crossings for.
-    save_edge_attributes : bool
-        Whether to save the edge crossings to the edge data.
-
-    Returns
-    -------
-    crossings : set((edge1, edge2))
-        A set of all edge crossings in the graph.
-    angles : dict((edge1, edge2), angle)
-        A dictionary of angles between edges.
-    """
-    crossings = set()
-    angles = {}
-    if save_edge_attributes:
-        edge_crossings = {edge: {"count": 0, "angles": []} for edge in G.edges}
-
-    # Iterate over all pairs of edges and check for intersections
-    edges = list(G.edges)
-    for i, edge1 in enumerate(edges):
-        for edge2 in edges[i + 1 :]:
-            # Check for intersections
-            line_a = (
-                (G.nodes[edge1[0]]["x"], G.nodes[edge1[0]]["y"]),
-                (G.nodes[edge1[1]]["x"], G.nodes[edge1[1]]["y"]),
-            )
-            line_b = (
-                (G.nodes[edge2[0]]["x"], G.nodes[edge2[0]]["y"]),
-                (G.nodes[edge2[1]]["x"], G.nodes[edge2[1]]["y"]),
-            )
-            # Skip edges that share a node
-            if len(set(line_a) & set(line_b)) > 0:
-                continue
-            if helpers._intersect(line_a, line_b):
-                crossings.add((edge1, edge2))
-                # Calculate angle between edges
-                v1 = helpers.edge_vector(line_a)
-                v2 = helpers.edge_vector(line_b)
-                angle = helpers.calculate_angle_between_vectors(v1, v2)
-                angles[edge1, edge2] = angle
-                if save_edge_attributes:
-                    edge_crossings[edge1]["count"] += 1
-                    edge_crossings[edge2]["count"] += 1
-                    edge_crossings[edge1]["angles"].append(angle)
-                    edge_crossings[edge2]["angles"].append(angle)
-
-    # Save edge crossings to edge data
-    if save_edge_attributes:
-        nx.set_edge_attributes(G, edge_crossings, "edge_crossings")
-    return crossings, angles
-
-
-def edge_crossing(G, verbose=False):
+def edge_crossing(G, subtract_tri=True, subtract_4=True):
     """Calculate the metric for the number of edge_crossing, scaled against the total
     number of possible crossings.
 
     Parameters
     ----------
     G : nx.Graph
         The graph to calculate the metric for.
@@ -198,54 +34,38 @@
     """
     # Estimate for the upper bound for the number of edge crossings
     m = G.number_of_edges()
     c_all = (m * (m - 1)) / 2
 
     # Calculate the number of impossible crossings based on the node degrees
     degree = np.array([degree[1] for degree in G.degree()])
-    c_impossible = np.dot(degree, degree - 1) / 2
+    c_deg = np.dot(degree, degree - 1) / 2
 
     # Calculate the maximum number of possible crossings
-    c_mx = c_all - c_impossible
+    c_mx = c_all - c_deg
+
+    if subtract_tri:
+        c_mx -= _count_impossible_triangle_crossings(G)
 
-    if verbose:
-        # Calculate the number of impossible crossings based on triangle geometry
-        c_tri = __count_impossible_triangle_crossings(G)
-        c_mx_no_tri = c_all - c_tri
-        c_mx_no_tri_no_deg = c_all - c_impossible - c_tri
-        print(f"Total Upper bound: {c_all:.0f}")
-        print(f"Impossible by degree: {c_impossible:.0f}")
-        print(f"Impossible by triangle: {c_tri:.0f}")
-        print(f"Upper bound removing degree: {c_mx:.0f}")
-        print(f"Upper bound removing triangles: {c_mx_no_tri:.0f}")
-        print(f"Upper bound removing degree and triangles: {c_mx_no_tri_no_deg:.0f}")
+    if subtract_4:
+        c_mx -= _count_4_cycles(G)
 
     # Retrieve the edge crossings from the graph if they have been calculated, otherwise calculate
     if not nx.get_edge_attributes(G, "edge_crossings"):
-        crossings, angles = __calculate_edge_crossings(G)
+        crossings, angles = _calculate_edge_crossings(G)
     else:
         edge_crossings = nx.get_edge_attributes(G, "edge_crossings")
         crossings = set()
         for edge, crossing in edge_crossings.items():
             if crossing["count"] > 0:
                 crossings.add(edge)
 
     # Calculate the number of edge crossings
     c = len(crossings)
 
-    if verbose:
-        print(f"Num Crossings: {c}")
-        print(f"Original EC: {1 - (c / c_mx) if c_mx > 0 else 1}")
-        print(
-            f"EC without triangles: {1 - (c / c_mx_no_tri) if c_mx_no_tri > 0 else 1}"
-        )
-        print(
-            f"EC without triangles and degrees: {1 - (c / c_mx_no_tri_no_deg) if c_mx_no_tri_no_deg > 0 else 1}"
-        )
-
     return 1 - helpers.divide_or_zero(c, c_mx)
 
 
 def edge_orthogonality(G):
     """Calculate the metric for edge orthogonality.
 
     Parameters
@@ -369,15 +189,15 @@
     if G.number_of_edges() > crossing_limit:
         raise ValueError(
             f"Number of edges exceeds the crossing limit of {crossing_limit}"
         )
 
     # Check if graph edges have edge_crossings attribute
     if not nx.get_edge_attributes(G, "edge_crossings"):
-        __calculate_edge_crossings(G)
+        _calculate_edge_crossings(G)
 
     edge_crossings = nx.get_edge_attributes(G, "edge_crossings")
 
     angles_sum = 0
     for crossing in edge_crossings.values():
         ideal = 180 / (
             crossing["count"] + 1
@@ -648,15 +468,15 @@
     return (
         1 - (num_non_conforming / possible_non_conforming)
         if possible_non_conforming > 0
         else 1
     )
 
 
-def stress(G):
+def __stress(G):
     """Calculate the metric for stress.
 
     Stress is a measure of how well the graph preserves the pairwise distances between nodes.
 
     Parameters
     ----------
     G : nx.Graph
@@ -880,15 +700,15 @@
             if helpers._intersect(line_a, line_b) and (line_a, line_b) not in covered:
                 covered.append((line_b, line_a))  # Mark the edges as covered
                 c += 1  # Increment the counter for edge crossings
 
     return c
 
 
-def symmetry(
+def _symmetry(
     G=None,
     num_crossings=None,
     show_sym=False,
     crosses_limit=1e6,
     threshold=1,
     tolerance=0.1,
 ):
```

### Comparing `graphreadability-0.0.1/src/tests/test_helpers.py` & `graphreadability-0.0.3/graphreadability/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `graphreadability-0.0.1/src/utils/crosses_promotion.py` & `graphreadability-0.0.3/graphreadability/utils/crosses_promotion.py`

 * *Files identical despite different names*

### Comparing `graphreadability-0.0.1/src/utils/helpers.py` & `graphreadability-0.0.3/graphreadability/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,20 +461,32 @@
         print(n)
 
 
 def draw_graph(G, flip=True, ax=None, **kwargs):
     """Draws the graph using standard NetworkX methods with matplotlib. Due to the nature of the coordinate systems used,
     graphs will be flipped on the X axis. To see the graph the way it would be drawn in yEd, set flip to True (default=True).
     """
+    default_kwargs = {
+        "edge_color": "#BDCCB4",
+        "node_color": "#778181",
+        "linewidths": 3,
+        "node_size": 300,
+        "width": 5,
+        "edgecolors": "#333333",
+        "with_labels": False,
+    }
+    for key, value in default_kwargs.items():
+        if key not in kwargs:
+            kwargs[key] = value
 
     if flip:
         pos = {
             k: np.array((v["x"], 0 - float(v["y"])), dtype=np.float32)
             for (k, v) in [u for u in G.nodes(data=True)]
         }
     else:
         pos = {
             k: np.array((v["x"], v["y"]), dtype=np.float32)
             for (k, v) in [u for u in G.nodes(data=True)]
         }
 
-    nx.draw(G, pos=pos, ax=ax, with_labels=True, **kwargs)
+    nx.draw(G, pos=pos, ax=ax, **kwargs)
```

### Comparing `graphreadability-0.0.1/src/utils/apps/digitize_graphs.py` & `graphreadability-0.0.3/graphreadability/utils/apps/digitize_graphs.py`

 * *Files identical despite different names*

### Comparing `graphreadability-0.0.1/.gitignore` & `graphreadability-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `graphreadability-0.0.1/LICENSE.txt` & `graphreadability-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graphreadability-0.0.1/README.md` & `graphreadability-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `graphreadability-0.0.1/pyproject.toml` & `graphreadability-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "graphreadability"
 dynamic = ["version"]
 description = "A Python module for applying readability metrics graph and network visualizations."
 readme = "README.md"
@@ -32,23 +32,36 @@
     "scipy"
 ]
 
 [project.optional-dependencies]
 tests = [
     "pandas"
 ]
+docs = [
+    "mkdocs",
+    "mkdocs-material",
+    "mkdocstrings",
+    "mkdocstrings-python",
+]
 
 [project.urls]
 Homepage = "https://github.com/PhilipMathieu/graphreadability"
 
 [tool.hatch.version]
-path = "src/__init__.py"
+source = "vcs"
+tag-pattern = "^(?:[\\w-]+-)?(?P<version>[vV]?\\d+(?:.\\d+){0,2})"
+
+[tool.hatch.version.raw-options]
+local_scheme = "no-local-version"
 
 [tool.hatch.build.targets.sdist]
 include = [
-    "src",
+    "graphreadability",
 ]
 
 [tool.hatch.build.targets.wheel]
 include = [
-    "src",
+    "graphreadability",
 ]
+
+[tool.hatch.build.hooks.vcs]
+version-file = "_version.py"
```

### Comparing `graphreadability-0.0.1/PKG-INFO` & `graphreadability-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: graphreadability
-Version: 0.0.1
+Version: 0.0.3
 Summary: A Python module for applying readability metrics graph and network visualizations.
 Project-URL: Homepage, https://github.com/PhilipMathieu/graphreadability
 Author-email: Philip Mathieu <mathieu.p@northeastern.edu>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: scipy
+Provides-Extra: docs
+Requires-Dist: mkdocs; extra == 'docs'
+Requires-Dist: mkdocs-material; extra == 'docs'
+Requires-Dist: mkdocstrings; extra == 'docs'
+Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: pandas; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # `graphreadability`
 
 Python module for applying readability metrics to network and graph visualizations. This project is a work in progress that is being developed by Philip Mathieu (MS DS Student) as part of the Research Apprenticeship program at Northeastern University's Khoury College of Computer Science.
```

