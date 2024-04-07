# Comparing `tmp/gpx_vis-0.2.0.tar.gz` & `tmp/gpx_vis-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx_vis-0.2.0.tar", last modified: Sat Apr  6 21:28:54 2024, max compression
+gzip compressed data, was "gpx_vis-0.3.0.tar", last modified: Sun Apr  7 22:07:34 2024, max compression
```

## Comparing `gpx_vis-0.2.0.tar` & `gpx_vis-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-06 21:28:54.324493 gpx_vis-0.2.0/
--rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.2.0/LICENSE
--rw-r--r--   0 jwt        (501) staff       (20)     2312 2024-04-06 21:28:54.324103 gpx_vis-0.2.0/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)     1774 2024-04-06 21:28:30.000000 gpx_vis-0.2.0/README.md
--rw-r--r--   0 jwt        (501) staff       (20)      578 2024-04-05 21:35:37.000000 gpx_vis-0.2.0/pyproject.toml
--rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-06 21:28:54.325323 gpx_vis-0.2.0/setup.cfg
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-06 21:28:54.318631 gpx_vis-0.2.0/src/
--rw-r--r--   0 jwt        (501) staff       (20)      174 2024-04-05 12:36:48.000000 gpx_vis-0.2.0/src/__init__.py
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-06 21:28:54.323579 gpx_vis-0.2.0/src/gpx_vis.egg-info/
--rw-r--r--   0 jwt        (501) staff       (20)     2312 2024-04-06 21:28:54.000000 gpx_vis-0.2.0/src/gpx_vis.egg-info/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      237 2024-04-06 21:28:54.000000 gpx_vis-0.2.0/src/gpx_vis.egg-info/SOURCES.txt
--rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-06 21:28:54.000000 gpx_vis-0.2.0/src/gpx_vis.egg-info/dependency_links.txt
--rw-r--r--   0 jwt        (501) staff       (20)       84 2024-04-06 21:28:54.000000 gpx_vis-0.2.0/src/gpx_vis.egg-info/requires.txt
--rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-06 21:28:54.000000 gpx_vis-0.2.0/src/gpx_vis.egg-info/top_level.txt
--rw-r--r--   0 jwt        (501) staff       (20)    17387 2024-04-05 21:41:04.000000 gpx_vis-0.2.0/src/gpx_vis.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-07 22:07:34.597627 gpx_vis-0.3.0/
+-rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.3.0/LICENSE
+-rw-r--r--   0 jwt        (501) staff       (20)     2507 2024-04-07 22:07:34.597341 gpx_vis-0.3.0/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)     1969 2024-04-07 22:04:11.000000 gpx_vis-0.3.0/README.md
+-rw-r--r--   0 jwt        (501) staff       (20)      578 2024-04-07 21:40:28.000000 gpx_vis-0.3.0/pyproject.toml
+-rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-07 22:07:34.597695 gpx_vis-0.3.0/setup.cfg
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-07 22:07:34.595628 gpx_vis-0.3.0/src/
+-rw-r--r--   0 jwt        (501) staff       (20)      174 2024-04-05 12:36:48.000000 gpx_vis-0.3.0/src/__init__.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-07 22:07:34.597001 gpx_vis-0.3.0/src/gpx_vis.egg-info/
+-rw-r--r--   0 jwt        (501) staff       (20)     2507 2024-04-07 22:07:34.000000 gpx_vis-0.3.0/src/gpx_vis.egg-info/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)      237 2024-04-07 22:07:34.000000 gpx_vis-0.3.0/src/gpx_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-07 22:07:34.000000 gpx_vis-0.3.0/src/gpx_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       84 2024-04-07 22:07:34.000000 gpx_vis-0.3.0/src/gpx_vis.egg-info/requires.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-07 22:07:34.000000 gpx_vis-0.3.0/src/gpx_vis.egg-info/top_level.txt
+-rw-r--r--   0 jwt        (501) staff       (20)    18353 2024-04-07 22:07:19.000000 gpx_vis-0.3.0/src/gpx_vis.py
```

### Comparing `gpx_vis-0.2.0/LICENSE` & `gpx_vis-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx_vis-0.2.0/PKG-INFO` & `gpx_vis-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx_vis
-Version: 0.2.0
+Version: 0.3.0
 Summary: Plots your Komoot tours
 Author-email: Jia Wei Teh <jiaweiteh.astro@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -47,35 +47,34 @@
 track = Track(pathname)
 ```
 
 `pathname` serves as a reference to either a single `.gpx` file or a directory.
 If a directory path is provided, all .gpx files contained within that directory
 will be merged, but retain their original metadata (e.g., different tracks remain separated).
 This allows users to overlay multiple tracks onto a single map, 
-providing a comprehensive summary of the data being analyzed or created.
+providing a comprehensive summary of the data being analyzed.
 
 Map creation
 ------------
 
 ```python
-track.create_map(path2file)
+track.create_map(filename)
 ```
 
 This creates an html file saved to `path2file`. An interactive html map will be created.
 Hover mouse over route, or click on final waypoints (flag marker) for further info.
 
-Route (Matplotlib)
-------------------
+If you have been very hard-working, thus having a large set of datapoints on the map: 
+there is an option to include `lite = True`. By default, this limits the datapoints on 
+each route to `50`. This number can be tweaked via the `nlite` argument. E.g.,
 
 ```python
-track.plt_tracks()
+track.create_map(filename, lite=True, nlite=100)
 ```
 
-Creates a latitude-longitude plot with matplotlib, colourmaped by elevation.
-
 City overview
 -------------
 
 ```python
 track.city_list
 ```
 
@@ -83,13 +82,13 @@
 of cities - sorted by country then name - that were detected through the tour. The 
 `frequency` parameter tells how many times a city was encountered; it should 
 somewhat correlate to time spent in that city.
 
 Additional information
 ----------------------
 
-Shoud you wish to plot/inspect different values, these parameters are also accesssible via:  
+Should you wish to plot/inspect different values, these parameters are also accesssible via:  
 
-`track.t`: time
-`track.x`: longitude
-`track.y`: latitude
-`track.z`: elevation
+`track.t`: time (UTC)<br>
+`track.x`: longitude (deg)<br>
+`track.y`: latitude (deg)<br>
+`track.z`: elevation (m)<br>
```

### Comparing `gpx_vis-0.2.0/README.md` & `gpx_vis-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1 +1 @@
-About `gpx_vis`===============`gpx_vis` allows simple and easy visualisation of your cycling/walking tours.Important: currently only works for .GPX from completed paths in Komoot. In development.Install-------```bashpip install gpx_vis```Update to the latest version:```bashpip install gpx_vis --upgrade```Instantiate-----------```pythonfrom gpx_vis import Tracktrack = Track(pathname)````pathname` serves as a reference to either a single `.gpx` file or a directory.If a directory path is provided, all .gpx files contained within that directorywill be merged, but retain their original metadata (e.g., different tracks remain separated).This allows users to overlay multiple tracks onto a single map, providing a comprehensive summary of the data being analyzed or created.Map creation------------```pythontrack.create_map(path2file)```This creates an html file saved to `path2file`. An interactive html map will be created.Hover mouse over route, or click on final waypoints (flag marker) for further info.Route (Matplotlib)------------------```pythontrack.plt_tracks()```Creates a latitude-longitude plot with matplotlib, colourmaped by elevation.City overview-------------```pythontrack.city_list```Curious which city you went through along the way? This command creates a listof cities - sorted by country then name - that were detected through the tour. The `frequency` parameter tells how many times a city was encountered; it should somewhat correlate to time spent in that city.Additional information----------------------Shoud you wish to plot/inspect different values, these parameters are also accesssible via:  `track.t`: time`track.x`: longitude`track.y`: latitude`track.z`: elevation
+About `gpx_vis`===============`gpx_vis` allows simple and easy visualisation of your cycling/walking tours.Important: currently only works for .GPX from completed paths in Komoot. In development.Install-------```bashpip install gpx_vis```Update to the latest version:```bashpip install gpx_vis --upgrade```Instantiate-----------```pythonfrom gpx_vis import Tracktrack = Track(pathname)````pathname` serves as a reference to either a single `.gpx` file or a directory.If a directory path is provided, all .gpx files contained within that directorywill be merged, but retain their original metadata (e.g., different tracks remain separated).This allows users to overlay multiple tracks onto a single map, providing a comprehensive summary of the data being analyzed.Map creation------------```pythontrack.create_map(filename)```This creates an html file saved to `path2file`. An interactive html map will be created.Hover mouse over route, or click on final waypoints (flag marker) for further info.If you have been very hard-working, thus having a large set of datapoints on the map: there is an option to include `lite = True`. By default, this limits the datapoints on each route to `50`. This number can be tweaked via the `nlite` argument. E.g.,```pythontrack.create_map(filename, lite=True, nlite=100)```City overview-------------```pythontrack.city_list```Curious which city you went through along the way? This command creates a listof cities - sorted by country then name - that were detected through the tour. The `frequency` parameter tells how many times a city was encountered; it should somewhat correlate to time spent in that city.Additional information----------------------Should you wish to plot/inspect different values, these parameters are also accesssible via:  `track.t`: time (UTC)<br>`track.x`: longitude (deg)<br>`track.y`: latitude (deg)<br>`track.z`: elevation (m)<br>
```

### Comparing `gpx_vis-0.2.0/pyproject.toml` & `gpx_vis-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpx_vis"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Jia Wei Teh", email="jiaweiteh.astro@gmail.com" },
 ]
 description = "Plots your Komoot tours"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gpx_vis-0.2.0/src/gpx_vis.egg-info/PKG-INFO` & `gpx_vis-0.3.0/src/gpx_vis.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx_vis
-Version: 0.2.0
+Version: 0.3.0
 Summary: Plots your Komoot tours
 Author-email: Jia Wei Teh <jiaweiteh.astro@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -47,35 +47,34 @@
 track = Track(pathname)
 ```
 
 `pathname` serves as a reference to either a single `.gpx` file or a directory.
 If a directory path is provided, all .gpx files contained within that directory
 will be merged, but retain their original metadata (e.g., different tracks remain separated).
 This allows users to overlay multiple tracks onto a single map, 
-providing a comprehensive summary of the data being analyzed or created.
+providing a comprehensive summary of the data being analyzed.
 
 Map creation
 ------------
 
 ```python
-track.create_map(path2file)
+track.create_map(filename)
 ```
 
 This creates an html file saved to `path2file`. An interactive html map will be created.
 Hover mouse over route, or click on final waypoints (flag marker) for further info.
 
-Route (Matplotlib)
-------------------
+If you have been very hard-working, thus having a large set of datapoints on the map: 
+there is an option to include `lite = True`. By default, this limits the datapoints on 
+each route to `50`. This number can be tweaked via the `nlite` argument. E.g.,
 
 ```python
-track.plt_tracks()
+track.create_map(filename, lite=True, nlite=100)
 ```
 
-Creates a latitude-longitude plot with matplotlib, colourmaped by elevation.
-
 City overview
 -------------
 
 ```python
 track.city_list
 ```
 
@@ -83,13 +82,13 @@
 of cities - sorted by country then name - that were detected through the tour. The 
 `frequency` parameter tells how many times a city was encountered; it should 
 somewhat correlate to time spent in that city.
 
 Additional information
 ----------------------
 
-Shoud you wish to plot/inspect different values, these parameters are also accesssible via:  
+Should you wish to plot/inspect different values, these parameters are also accesssible via:  
 
-`track.t`: time
-`track.x`: longitude
-`track.y`: latitude
-`track.z`: elevation
+`track.t`: time (UTC)<br>
+`track.x`: longitude (deg)<br>
+`track.y`: latitude (deg)<br>
+`track.z`: elevation (m)<br>
```

### Comparing `gpx_vis-0.2.0/src/gpx_vis.py` & `gpx_vis-0.3.0/src/gpx_vis.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Tue Apr 2 23:14:31 2024
 
 @author: Jia Wei Teh
 
-This script combines .gpx files in /data and overplots them onto a HTML file?
-
-Written as an extension based on gpxpy.
-
-The problem with other libraries is that they dont really have outputs i want,
-and are not very customisable. This hopefully solves the problem (a little).
+This script combines .gpx files in /data and overplots them onto a HTML file.
 """
 # main library
 import gpxpy
 
 import os
 import math
 import branca
 import folium
 import numpy as np
 import pandas as pd
+import altair as alt
 import humanfriendly
-import cmasher as cmr
 import reverse_geocode
-import matplotlib.pyplot as plt
+from folium.plugins import MarkerCluster, MiniMap
 
 from vincenty import vincenty
-from matplotlib.ticker import (AutoMinorLocator, MultipleLocator)
 
 class Track:
     """
     Instance used to process .gpx files.
     """
     
     # =============================================================================
@@ -172,14 +166,15 @@
         unique_city_list = list(set(city_list))
         # add frequency of appearance of city in tour
         for ii, unique_city in enumerate(unique_city_list):
             counts = city_list.count(unique_city)
             # update attribute
             setattr(unique_city_list[ii], 'frequency', counts)
         # return full list of cities, sorted by country then by name
+        print('Here are the cities you have been in.')
         return sorted(unique_city_list)
     
     # =============================================================================
     # Track handling
     # =============================================================================
     
     @staticmethod
@@ -220,143 +215,112 @@
                         previous_idx = idx + 1
             return track_list
 
     # =============================================================================
     # Plotting on graphs    
     # =============================================================================
 
-    def plt_tracks(self):
-        """
-        Creates a latitude-longitude plot with matplotlib, coloured by elevation.
-        """
-        # create subplot
-        fig, ax = plt.subplots(1, 1, figsize = (5, 5), dpi = 300)
-        # draw line
-        plt.scatter(self.x, self.y, c = self.z, cmap = cmr.rainforest,
-                    vmax = self._round2n(max(self.z), 3),  
-                    vmin = self._round2n(min(self.z), 3),
-                    s = 0.5,)
-        # colorbar
-        plt.colorbar(label = 'elevation (m)')
-                     
-        
-        # plot waypoints for each end and beginning of a track
-        idx_split_list = self.idx_trksplit(self)
-        for (i, j) in idx_split_list:
-            self.plt_waypoints(ax, self.x[i:j], self.y[i:j])
-            
-        # ticks
-        # 5 mini ticks between major ticks
-        xtick_n, ytick_n = 5, 5
-        xspan = max(self.x) - min(self.x)
-        yspan = max(self.y) - min(self.y)
-        # 5 ticks on each sides
-        xinterval = self._round2n(xspan/5, 2)
-        yinterval = self._round2n(yspan/5, 2)
-        ax.xaxis.set_major_locator(MultipleLocator(xinterval))
-        ax.xaxis.set_minor_locator(AutoMinorLocator(xtick_n))
-        ax.yaxis.set_major_locator(MultipleLocator(yinterval))
-        ax.yaxis.set_minor_locator(AutoMinorLocator(ytick_n))
-        ax.tick_params(axis='both', which = 'major', direction = 'in',length = 6, width = 1)
-        ax.tick_params(axis='both', which = 'minor', direction = 'in',length = 4, width = 1)
-        ax.yaxis.set_ticks_position('both')
-        ax.xaxis.set_ticks_position('both')
-
-        plt.show()
-
-    @staticmethod
-    def plt_waypoints(ax, x, y):
-        """
-        Adding mini waypoints to the plt_tracks() plot.
-        """
-        # A small trick to separate tracks without actually separating them: add waypoint at end and start of tracks
-        # start
-        ax.scatter(x[0], y[0], 
-                marker = '.', s = 100, 
-                alpha = 0.8,
-                fc = 'yellow', ec = 'k')
-        # finish
-        ax.scatter(x[-1], y[-1], 
-                marker = '^', s = 50, 
-                alpha = 0.8,
-                fc = 'blue', ec = 'k')
         
     @staticmethod
     def _round2n(x, n):
         """rounds to n significant numbers"""
         return round(x, -int(math.floor(np.log10(x))) + (n - 1))
         
     
     
     # =============================================================================
     # Plotting on maps
     # =============================================================================
     
-    def create_map(self, filename):
+    def create_map(self, filename, lite = False, **kwargs):
         """
         Map out your tour on an interactive streetmaps.
         """
         # find optimal center for map display.
         map_center = self.data[['latitude', 'longitude']].mean().values.tolist()
         # southwest (minimums) and northeast (maximums) boundary.
         map_sw = self.data[['latitude', 'longitude']].min().values.tolist()
         map_ne = self.data[['latitude', 'longitude']].max().values.tolist()
         # create Map.
         main_map = folium.Map(location = map_center)
         # specify border.
         main_map.fit_bounds([map_sw, map_ne])
         
         # create group
-        lineGroup = folium.FeatureGroup("Lines")
-        
+        lineGroup = folium.FeatureGroup(name = "Your Routes")
         # plot waypoints for each end and beginning of a track
         idx_split_list = self.idx_trksplit(self)
         # if list is empty, there is no splitting tracks
         for selected_idx in idx_split_list:
-            self._addTracksOnMap(self, lineGroup, selected_idx)
+            self._addTracksOnMap(self, lineGroup, selected_idx, lite, **kwargs)
+            
+        # clusters
+        cluster = MarkerCluster().add_to(main_map)
         # add group to map
-        lineGroup.add_to(main_map)
+        lineGroup.add_to(cluster)
         
         # add different backgrounds
         _tilesList = ['openstreetmap', 'CartoDB Voyager', 'Cartodb dark_matter', 'cartodbpositron']
         for tiles in _tilesList:
             folium.TileLayer(tiles).add_to(main_map)
         # add layer control
         folium.LayerControl(position='bottomright').add_to(main_map)
+        # add minimap 
+        MiniMap(toggle_display = True, zoom_level_offset = -4,
+                witdh = 400, height = 200,
+                position = 'topright',
+                ).add_to(main_map)
         
         # save
         if not filename.endswith(".html"):
             filename += '.html'
         main_map.save(filename)
         
         return print(f"File saved as {filename}.")
     
     @staticmethod
-    def _addTracksOnMap(self, group, selected_idx):
+    def _addTracksOnMap(self, group, selected_idx, lite, **kwargs):
         """
         This function adds individual tracks onto create_map().
         group: FeatureGroup this track belongs to.
         selected_idx: index range of this particular track.
         """
         ii, jj = selected_idx
-        track_coords = list(zip(self.y[ii:jj], self.x[ii:jj]))
+        # limit number of points shown to reduce lag, if lite is enabled.
+        if kwargs.get('nlite') is not None:
+            max_nPoints = kwargs.get('nlite')
+        else:
+            max_nPoints = 50
+        if (jj-ii) < max_nPoints or lite == False:
+            nPoints = 1 #basically means plot every single point
+        else:
+            nPoints = int((jj-ii)/max_nPoints)
+        
+            
+        track_coords = list(zip(self.y[ii:jj:nPoints], self.x[ii:jj:nPoints]))
         # popup str in html
         popupTxt = self._addPopuptxt(self, selected_idx)
         # information frame        
-        iframe = folium.IFrame(popupTxt)
+        # iframe = folium.IFrame(popupTxt)
+        elevation_graph = self._addPopupGraph(self, selected_idx)
         # create popup
-        popup = folium.Popup(iframe,
-                     min_width=300,
-                     max_width=300)
+        popup = folium.Popup(popupTxt,
+                     min_width=400,
+                     max_width=400)
+        elevation_graph.add_to(popup)
         # add tooltip
         tooltip = self._addTooltip(self, selected_idx)
         # add to group
+        # since elevation sometimes differ widly, perhaps it is better to use 
+        # log-scale as a simple fix. (as long as there aren't zero entries)
+        # Right now, I am using individual tracks for individual colorbar min/max. Can of course
+        # switch to map-wide colorbar by removing [ii:jj]
         folium.ColorLine(track_coords,
-                        colors = self.z[ii:jj],
-                        colormap = branca.colormap.linear.viridis.scale(min(self.z),max(self.z)),
+                        colors = self.z[ii:jj:nPoints],
+                        colormap = branca.colormap.linear.viridis.scale(min(self.z[ii:jj:nPoints]),max(self.z[ii:jj:nPoints])),
                         tooltip = tooltip,
                         weight = 4,
                         ).add_to(group)
         
         # add start/finish points
         folium.CircleMarker(location = track_coords[0],
                             radius = 5,
@@ -377,55 +341,100 @@
                                         'weight': 10}
         # 2. highlighted line
         highlight_line = {'geometry': {
                     'type': 'LineString',
                     # reverse coord from (y, x) into (x,y)
                     'coordinates': [coord[::-1] for coord in track_coords]
                     }}
-        # add
+        # add transparent layer to help highlighting
         folium.features.GeoJson(
                 color = 'transparent',
                 data = highlight_line['geometry'],
                 control=False,
                 tooltip = tooltip,
+                weight = 25, #transparent layer easier to highlight
                 highlight_function=highlight_function, 
                 ).add_to(group)
-        
         return  
       
     @staticmethod
     def _addPopuptxt(self, selected_idx):
         """
-        Creates str-block that contains useful info about the route when clicked.
+        Creates str-block that contains useful info.
         """
         # index range
         ii, jj = selected_idx
         # track name
         track_name = self.name[ii]
         track_y = self.y[ii:jj]
         track_x = self.x[ii:jj]
         track_t = self.t[ii:jj]
         # get information
         startCity = self.City(reverse_geocode.search([[track_y[0], track_x[0]]])[0]).city
         endCity = self.City(reverse_geocode.search([[track_y[-1], track_x[-1]]])[0]).city
         dist = self._getDistance(track_y, track_x)
         timeElapsed = self._getTimeElapsed(track_t[0], track_t[-1])
         
-        # HTML fmt
+        # Option 1: As HTML fmt-ed block
         infostr = f"""
                     <h3>{track_name}</h3>
                     <h4> {startCity} - {endCity}</h4>
                     <p> 
-                    <b>Start</b>: <em>{track_t[0].strftime('%d.%m.%Y %H:%M:%S')}</em><br>
-                    <b>End</b>: <em>{track_t[-1].strftime('%d.%m.%Y %H:%M:%S')}</em><br>
+                    <b>Start</b>: <em>{track_t[0].strftime('%d.%m.%Y %H:%M:%S')} (UTC)</em><br>
+                    <b>End</b>: <em>{track_t[-1].strftime('%d.%m.%Y %H:%M:%S')} (UTC)</em><br>
                     <b>Dist</b>: {dist} km<br>
                     <b>Duration</b>: {timeElapsed}<br>
                     </p>
                   """
-        return infostr
+        # Option 2: Embedded in VegaLite graph.
+        title = f'{track_name}'
+        subtitle1 = f"""Start: {track_t[0].strftime('%d.%m.%Y %H:%M:%S')} (UTC), {startCity}"""
+        subtitle2 = f"""End: {track_t[-1].strftime('%d.%m.%Y %H:%M:%S')} (UTC), {endCity}"""
+        subtitle3 = f'Total: {dist} km, {timeElapsed}'
+                 
+        return title, subtitle1, subtitle2, subtitle3
+    
+    @staticmethod
+    def _addPopupGraph(self, selected_idx):
+        """
+        Creates elevation graph in Popup text.
+        """
+        ii, jj = selected_idx
+        # create figure with Method-based Syntax.
+        # https://altair-viz.github.io/user_guide/encodings/index.html
+        # limit number of points
+        max_nPoints = 100
+        if (jj-ii) < max_nPoints:
+            nPoints = 1
+        else:
+            nPoints = int((jj-ii)/max_nPoints)
+        
+        # titles
+        title, subtitle1, subtitle2, subtitle3 = self._addPopuptxt(self, selected_idx)
+        # plot
+        lineplot = alt.Chart(self.data[['time', 'elevation']][ii:jj:nPoints],
+                                 title = alt.Title(  title, 
+                                                     subtitle = [subtitle1, subtitle2, subtitle3])
+                                                   )\
+                            .mark_line()\
+                            .encode(
+                                 alt.X('time', axis = alt.Axis(tickMinStep=20)).title('Time (UTC'),\
+                                 alt.Y('elevation').scale(domain=(min(self.z[ii:jj:nPoints]-50), max(self.z[ii:jj:nPoints]+50))).title('Elevation (m)'),\
+                                 )\
+                            .properties(
+                                width = 300, height = 300,
+                                )
+        # turn into vega
+        elevation_graph = folium.VegaLite(
+                            lineplot,
+                            width=300,
+                            height=300,
+                            )
+        return elevation_graph
+    
     
     @staticmethod
     def _addTooltip(self, selected_idx):
         """
         Creates str-block that contains tooltip when mouse is hovered over the track.
         """
         ii, jj = selected_idx
@@ -455,8 +464,8 @@
         # calculate difference
         elapsed = end - start
         # readable
         return humanfriendly.format_timespan(elapsed)
     
     @property
     def shouldiContinueCycling(self):
-        return 'yes of course.'
+        return print('yes of course.')
```

