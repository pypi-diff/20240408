# Comparing `tmp/naps-track-1.0.6.tar.gz` & `tmp/naps-track-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/naps-track-1.0.6.tar", last modified: Wed Jun  7 16:10:40 2023, max compression
+gzip compressed data, was "dist/naps-track-1.0.7.tar", last modified: Mon Apr  8 20:52:01 2024, max compression
```

## Comparing `naps-track-1.0.6.tar` & `naps-track-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:40.000000 naps-track-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 16:10:34.000000 naps-track-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-07 16:10:40.000000 naps-track-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-07 16:10:34.000000 naps-track-1.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:40.000000 naps-track-1.0.6/naps/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/aruco.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/cost_matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6978 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/matching.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3902 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/naps_interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/naps_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/naps_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/sleap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:40.000000 naps-track-1.0.6/naps/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8011 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/utils/interactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/utils/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:40.000000 naps-track-1.0.6/naps_track.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-07 16:10:39.000000 naps-track-1.0.6/naps_track.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-07 16:10:40.000000 naps-track-1.0.6/naps_track.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:10:39.000000 naps-track-1.0.6/naps_track.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 16:10:39.000000 naps-track-1.0.6/naps_track.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 16:10:39.000000 naps-track-1.0.6/naps_track.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 16:10:39.000000 naps-track-1.0.6/naps_track.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 16:10:34.000000 naps-track-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:10:40.000000 naps-track-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-07 16:10:34.000000 naps-track-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:52:01.000000 naps-track-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 20:51:56.000000 naps-track-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-08 20:52:01.000000 naps-track-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-08 20:51:56.000000 naps-track-1.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:52:01.000000 naps-track-1.0.7/naps/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-08 20:51:56.000000 naps-track-1.0.7/naps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-08 20:51:56.000000 naps-track-1.0.7/naps/aruco.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4016 2024-04-08 20:51:56.000000 naps-track-1.0.7/naps/cost_matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6978 2024-04-08 20:51:56.000000 naps-track-1.0.7/naps/matching.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3902 2024-04-08 20:51:56.000000 naps-track-1.0.7/naps/naps_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-04-08 20:51:56.000000 naps-track-1.0.7/naps/naps_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9945 2024-04-08 20:51:56.000000 naps-track-1.0.7/naps/naps_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-08 20:51:56.000000 naps-track-1.0.7/naps/sleap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:52:01.000000 naps-track-1.0.7/naps/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:51:56.000000 naps-track-1.0.7/naps/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8188 2024-04-08 20:51:56.000000 naps-track-1.0.7/naps/utils/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-08 20:51:56.000000 naps-track-1.0.7/naps/utils/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:52:01.000000 naps-track-1.0.7/naps_track.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-08 20:52:00.000000 naps-track-1.0.7/naps_track.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-08 20:52:01.000000 naps-track-1.0.7/naps_track.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:52:00.000000 naps-track-1.0.7/naps_track.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-08 20:52:00.000000 naps-track-1.0.7/naps_track.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 20:52:00.000000 naps-track-1.0.7/naps_track.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 20:52:00.000000 naps-track-1.0.7/naps_track.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 20:51:56.000000 naps-track-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:52:01.000000 naps-track-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-08 20:51:56.000000 naps-track-1.0.7/setup.py
```

### Comparing `naps-track-1.0.6/PKG-INFO` & `naps-track-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naps-track
-Version: 1.0.6
+Version: 1.0.7
 Summary: NAPS (NAPS is ArUco Plus SLEAP)
 Home-page: https://github.com/kocherlab/naps
 License: MIT
 Project-URL: Documentation, https://naps.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/kocherlab/naps
 Project-URL: Issue tracker, https://github.com/kocherlab/naps/issues
 Description: |Stable version| |Latest version| |Documentation| |github ci| |Coverage| |conda| |Conda Upload| |PyPI Upload| |LICENSE|
```

### Comparing `naps-track-1.0.6/README.rst` & `naps-track-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.6/naps/__init__.py` & `naps-track-1.0.7/naps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 # from naps import utils
 # import naps.utils
 
 # Basic Information
 __name__ = "naps-track"
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 __summary__ = "NAPS (NAPS is ArUco Plus SLEAP)"
 __url__ = "https://github.com/kocherlab/naps"
 __code__ = "https://github.com/kocherlab/naps"
 __issue__ = "https://github.com/kocherlab/naps/issues"
 __docs__ = "https://naps.readthedocs.io/en/latest/"
 __license__ = "MIT"
 __copyright__ = "2022"
```

### Comparing `naps-track-1.0.6/naps/aruco.py` & `naps-track-1.0.7/naps/aruco.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.6/naps/cost_matrix.py` & `naps-track-1.0.7/naps/cost_matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,20 @@
                                 del cost_dict[track][tag]
 
             # Create a dataframe of the matrix
             cost_dataframe = pd.DataFrame.from_dict(cost_dict).fillna(0)
             cost_dataframe = cost_dataframe.loc[~(cost_dataframe == 0).all(axis=1)]
             cost_dataframe = cost_dataframe.loc[:, ~(cost_dataframe == 0).all(axis=0)]
 
+            # Create a list of the tracks in the current frame
+            match_tracks = set(self.unmatched_dict[match_frame]) & set(cost_dataframe.columns)
+
+            # Subset the cost dataframe to only include the tracks in the current frame
+            cost_dataframe = cost_dataframe[list(match_tracks)]
+
             # Store the assignments
             for track_index, tag_index in self.assignment_method(cost_dataframe.values):
                 matched_dict[match_frame][
                     cost_dataframe.columns[track_index]
                 ] = cost_dataframe.index[tag_index]
 
         for frame in range(self.first_frame + 1, self.last_frame + 1):
```

### Comparing `naps-track-1.0.6/naps/matching.py` & `naps-track-1.0.7/naps/matching.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.6/naps/naps_interactions.py` & `naps-track-1.0.7/naps/naps_interactions.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.6/naps/naps_plot.py` & `naps-track-1.0.7/naps/naps_plot.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.6/naps/naps_track.py` & `naps-track-1.0.7/naps/naps_track.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.6/naps/sleap_utils.py` & `naps-track-1.0.7/naps/sleap_utils.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.6/naps/utils/interactor.py` & `naps-track-1.0.7/naps/utils/interactor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 import os
 
 import numpy as np
+from shapely import area
 from shapely.geometry import LineString, MultiPoint, Point
 from shapely.ops import unary_union
 
 
 class Interactor:
     def __init__(
         self,
@@ -137,14 +138,16 @@
 
                 # Return the interaction
                 return {
                     "Origin interactor": origin_interactor.name,
                     "Destination interactor": dest_interactor.name,
                     "Interaction Name": name,
                     "Interaction Frame": self.frame,
+                    "Origin Area": area(origin_interactor._models[origin]),
+                    "Destination Area": area(dest_interactor._models[dest])
                 }
 
             # Confirm a name was given for the interaction
             if not name:
                 raise Exception(
                     f"No name given for interaction with origin ({origin}) and dest ({dest})"
                 )
```

### Comparing `naps-track-1.0.6/naps/utils/tracking.py` & `naps-track-1.0.7/naps/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.6/naps_track.egg-info/PKG-INFO` & `naps-track-1.0.7/naps_track.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naps-track
-Version: 1.0.6
+Version: 1.0.7
 Summary: NAPS (NAPS is ArUco Plus SLEAP)
 Home-page: https://github.com/kocherlab/naps
 License: MIT
 Project-URL: Documentation, https://naps.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/kocherlab/naps
 Project-URL: Issue tracker, https://github.com/kocherlab/naps/issues
 Description: |Stable version| |Latest version| |Documentation| |github ci| |Coverage| |conda| |Conda Upload| |PyPI Upload| |LICENSE|
```

### Comparing `naps-track-1.0.6/setup.py` & `naps-track-1.0.7/setup.py`

 * *Files identical despite different names*

