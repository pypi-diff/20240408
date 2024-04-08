# Comparing `tmp/dongraphio-0.3.1.tar.gz` & `tmp/dongraphio-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dongraphio-0.3.1.tar", max compression
+gzip compressed data, was "dongraphio-0.3.2.tar", max compression
```

## Comparing `dongraphio-0.3.1.tar` & `dongraphio-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1418 2024-04-05 16:39:32.861939 dongraphio-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1395 2024-03-13 09:15:32.791323 dongraphio-0.3.1/README.md
--rw-r--r--   0        0        0      262 2024-04-05 16:39:32.853935 dongraphio-0.3.1/src/dongraphio/__init__.py
--rw-r--r--   0        0        0      133 2024-04-01 09:14:48.791527 dongraphio-0.3.1/src/dongraphio/base_models/__init__.py
--rw-r--r--   0        0        0    14979 2024-04-01 09:14:48.792530 dongraphio-0.3.1/src/dongraphio/base_models/grapher_logic.py
--rw-r--r--   0        0        0     5383 2024-04-01 09:14:48.793529 dongraphio-0.3.1/src/dongraphio/base_models/isochrones_logic.py
--rw-r--r--   0        0        0     2519 2024-04-05 16:37:52.018036 dongraphio-0.3.1/src/dongraphio/base_models/matrix_logic.py
--rw-r--r--   0        0        0     6150 2024-04-01 09:14:48.794528 dongraphio-0.3.1/src/dongraphio/dongraphio.py
--rw-r--r--   0        0        0     1056 2024-03-13 09:15:32.794322 dongraphio-0.3.1/src/dongraphio/enums.py
--rw-r--r--   0        0        0      559 2024-04-01 09:14:48.796532 dongraphio-0.3.1/src/dongraphio/utils/__init__.py
--rw-r--r--   0        0        0     1262 2024-03-29 09:52:53.311030 dongraphio-0.3.1/src/dongraphio/utils/geometry_utils.py
--rw-r--r--   0        0        0    19283 2024-04-01 09:14:48.797530 dongraphio-0.3.1/src/dongraphio/utils/graph_utils.py
--rw-r--r--   0        0        0     2602 2024-04-04 09:04:56.734596 dongraphio-0.3.1/src/dongraphio/utils/matrix_utils.py
--rw-r--r--   0        0        0     1713 2024-03-13 09:15:32.797336 dongraphio-0.3.1/src/dongraphio/utils/osm_worker.py
--rw-r--r--   0        0        0     1647 2024-04-01 09:14:48.799528 dongraphio-0.3.1/src/dongraphio/utils/tsp_solver.py
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 dongraphio-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1418 2024-04-08 13:00:33.697782 dongraphio-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1384 2024-04-07 11:13:31.735199 dongraphio-0.3.2/README.md
+-rw-r--r--   0        0        0      262 2024-04-08 13:00:33.752773 dongraphio-0.3.2/src/dongraphio/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-07 11:11:58.300514 dongraphio-0.3.2/src/dongraphio/base_models/__init__.py
+-rw-r--r--   0        0        0    14979 2024-04-07 11:11:58.300514 dongraphio-0.3.2/src/dongraphio/base_models/grapher_logic.py
+-rw-r--r--   0        0        0     5383 2024-04-07 11:11:58.315720 dongraphio-0.3.2/src/dongraphio/base_models/isochrones_logic.py
+-rw-r--r--   0        0        0     2719 2024-04-08 12:58:57.770722 dongraphio-0.3.2/src/dongraphio/base_models/matrix_logic.py
+-rw-r--r--   0        0        0     6150 2024-04-07 11:11:58.315720 dongraphio-0.3.2/src/dongraphio/dongraphio.py
+-rw-r--r--   0        0        0     1056 2024-03-13 09:15:32.794322 dongraphio-0.3.2/src/dongraphio/enums.py
+-rw-r--r--   0        0        0      559 2024-04-07 11:11:58.315720 dongraphio-0.3.2/src/dongraphio/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-04-07 11:11:58.315720 dongraphio-0.3.2/src/dongraphio/utils/geometry_utils.py
+-rw-r--r--   0        0        0    19283 2024-04-07 11:11:58.315720 dongraphio-0.3.2/src/dongraphio/utils/graph_utils.py
+-rw-r--r--   0        0        0     2602 2024-04-07 11:11:58.315720 dongraphio-0.3.2/src/dongraphio/utils/matrix_utils.py
+-rw-r--r--   0        0        0     1713 2024-03-13 09:15:32.797336 dongraphio-0.3.2/src/dongraphio/utils/osm_worker.py
+-rw-r--r--   0        0        0     1647 2024-04-07 11:11:58.315720 dongraphio-0.3.2/src/dongraphio/utils/tsp_solver.py
+-rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 dongraphio-0.3.2/PKG-INFO
```

### Comparing `dongraphio-0.3.1/pyproject.toml` & `dongraphio-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dongraphio"
-version = "0.3.1"
+version = "0.3.2"
 description = "Small utility library containing graph algorighms used in other projects"
 authors = ["Danila <63115678+DDonnyy@users.noreply.github.com>"]
 readme = "README.md"
 
 packages = [{ include = "dongraphio", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `dongraphio-0.3.1/README.md` & `dongraphio-0.3.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 dongrph = DonGraphio(city_crs=32638)
     
 intermodal_graph = dongrph.get_intermodal_graph_from_osm(city_osm_id=3955288)
 nx.write_graphml(intermodal_graph,"city_intermodal.graphml")
 
 builds_from = gpd.read_file("test_data/buildings.geojson")
 services_to = gpd.read_file("test_data/services.geojson")
-adjacency_matrix = dongrph.get_adjacency_matrix(buildings_from=builds_from, services_to=services_to, weight="time_min")
+adjacency_matrix = dongrph.get_adjacency_matrix(gdf_from=builds_from, gdf_to=services_to, weight="time_min")
 adjacency_matrix.to_csv("city_adjacency_matrix.csv")
 
 accessibility_isochrones, public_transport_routes, public_transport_stops = dongrph.get_accessibility_isochrones(
     graph_type=[GraphType.PUBLIC_TRANSPORT, GraphType.WALK],
     x_from=571747,
     y_from=5709639,
     weight_value=15,
```

### Comparing `dongraphio-0.3.1/src/dongraphio/base_models/grapher_logic.py` & `dongraphio-0.3.2/src/dongraphio/base_models/grapher_logic.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.1/src/dongraphio/base_models/isochrones_logic.py` & `dongraphio-0.3.2/src/dongraphio/base_models/isochrones_logic.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.1/src/dongraphio/base_models/matrix_logic.py` & `dongraphio-0.3.2/src/dongraphio/base_models/matrix_logic.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,15 +35,19 @@
             mobility_sub_graph = convert_multidigraph_to_digraph(mobility_sub_graph, self.weight)
 
         mobility_sub_graph.graph["crs"] = self.city_crs
 
         graph_gdf = nx_to_gdf(nx.MultiDiGraph(mobility_sub_graph), nodes=True)
 
         from_ = gpd.sjoin_nearest(self.gdf_from, graph_gdf)
+        from_ = from_.reset_index().drop_duplicates(subset="index", keep="first").set_index('index')
+
         to_ = gpd.sjoin_nearest(self.gdf_to, graph_gdf)
+        to_ = to_.reset_index().drop_duplicates(subset="index", keep="first").set_index("index")
+
         from_index = from_["index_right"]
         to_index = to_["index_right"]
         distance_matrix = pd.DataFrame(float(0), index=from_index, columns=to_index)
         from_index = list(set(from_index))
         to_index = list(set(to_index))
         logger.debug("Calculating distances from buildings to services ...")
```

### Comparing `dongraphio-0.3.1/src/dongraphio/dongraphio.py` & `dongraphio-0.3.2/src/dongraphio/dongraphio.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.1/src/dongraphio/enums.py` & `dongraphio-0.3.2/src/dongraphio/enums.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.1/src/dongraphio/utils/__init__.py` & `dongraphio-0.3.2/src/dongraphio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.1/src/dongraphio/utils/geometry_utils.py` & `dongraphio-0.3.2/src/dongraphio/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.1/src/dongraphio/utils/graph_utils.py` & `dongraphio-0.3.2/src/dongraphio/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.1/src/dongraphio/utils/matrix_utils.py` & `dongraphio-0.3.2/src/dongraphio/utils/matrix_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.1/src/dongraphio/utils/osm_worker.py` & `dongraphio-0.3.2/src/dongraphio/utils/osm_worker.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.1/src/dongraphio/utils/tsp_solver.py` & `dongraphio-0.3.2/src/dongraphio/utils/tsp_solver.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.1/PKG-INFO` & `dongraphio-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dongraphio
-Version: 0.3.1
+Version: 0.3.2
 Summary: Small utility library containing graph algorighms used in other projects
 Author: Danila
 Author-email: 63115678+DDonnyy@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -40,15 +40,15 @@
 dongrph = DonGraphio(city_crs=32638)
     
 intermodal_graph = dongrph.get_intermodal_graph_from_osm(city_osm_id=3955288)
 nx.write_graphml(intermodal_graph,"city_intermodal.graphml")
 
 builds_from = gpd.read_file("test_data/buildings.geojson")
 services_to = gpd.read_file("test_data/services.geojson")
-adjacency_matrix = dongrph.get_adjacency_matrix(buildings_from=builds_from, services_to=services_to, weight="time_min")
+adjacency_matrix = dongrph.get_adjacency_matrix(gdf_from=builds_from, gdf_to=services_to, weight="time_min")
 adjacency_matrix.to_csv("city_adjacency_matrix.csv")
 
 accessibility_isochrones, public_transport_routes, public_transport_stops = dongrph.get_accessibility_isochrones(
     graph_type=[GraphType.PUBLIC_TRANSPORT, GraphType.WALK],
     x_from=571747,
     y_from=5709639,
     weight_value=15,
```

