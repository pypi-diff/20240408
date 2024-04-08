# Comparing `tmp/gpx_vis-0.3.0.tar.gz` & `tmp/gpx_vis-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx_vis-0.3.0.tar", last modified: Sun Apr  7 22:07:34 2024, max compression
+gzip compressed data, was "gpx_vis-0.3.1.tar", last modified: Sun Apr  7 22:26:25 2024, max compression
```

## Comparing `gpx_vis-0.3.0.tar` & `gpx_vis-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-07 22:07:34.597627 gpx_vis-0.3.0/
--rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.3.0/LICENSE
--rw-r--r--   0 jwt        (501) staff       (20)     2507 2024-04-07 22:07:34.597341 gpx_vis-0.3.0/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)     1969 2024-04-07 22:04:11.000000 gpx_vis-0.3.0/README.md
--rw-r--r--   0 jwt        (501) staff       (20)      578 2024-04-07 21:40:28.000000 gpx_vis-0.3.0/pyproject.toml
--rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-07 22:07:34.597695 gpx_vis-0.3.0/setup.cfg
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-07 22:07:34.595628 gpx_vis-0.3.0/src/
--rw-r--r--   0 jwt        (501) staff       (20)      174 2024-04-05 12:36:48.000000 gpx_vis-0.3.0/src/__init__.py
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-07 22:07:34.597001 gpx_vis-0.3.0/src/gpx_vis.egg-info/
--rw-r--r--   0 jwt        (501) staff       (20)     2507 2024-04-07 22:07:34.000000 gpx_vis-0.3.0/src/gpx_vis.egg-info/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      237 2024-04-07 22:07:34.000000 gpx_vis-0.3.0/src/gpx_vis.egg-info/SOURCES.txt
--rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-07 22:07:34.000000 gpx_vis-0.3.0/src/gpx_vis.egg-info/dependency_links.txt
--rw-r--r--   0 jwt        (501) staff       (20)       84 2024-04-07 22:07:34.000000 gpx_vis-0.3.0/src/gpx_vis.egg-info/requires.txt
--rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-07 22:07:34.000000 gpx_vis-0.3.0/src/gpx_vis.egg-info/top_level.txt
--rw-r--r--   0 jwt        (501) staff       (20)    18353 2024-04-07 22:07:19.000000 gpx_vis-0.3.0/src/gpx_vis.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-07 22:26:25.660035 gpx_vis-0.3.1/
+-rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.3.1/LICENSE
+-rw-r--r--   0 jwt        (501) staff       (20)     3044 2024-04-07 22:26:25.659773 gpx_vis-0.3.1/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)     2491 2024-04-07 22:24:41.000000 gpx_vis-0.3.1/README.md
+-rw-r--r--   0 jwt        (501) staff       (20)      593 2024-04-07 22:26:11.000000 gpx_vis-0.3.1/pyproject.toml
+-rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-07 22:26:25.660099 gpx_vis-0.3.1/setup.cfg
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-07 22:26:25.657557 gpx_vis-0.3.1/src/
+-rw-r--r--   0 jwt        (501) staff       (20)      113 2024-04-07 22:23:57.000000 gpx_vis-0.3.1/src/__init__.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-07 22:26:25.659372 gpx_vis-0.3.1/src/gpx_vis.egg-info/
+-rw-r--r--   0 jwt        (501) staff       (20)     3044 2024-04-07 22:26:25.000000 gpx_vis-0.3.1/src/gpx_vis.egg-info/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)      237 2024-04-07 22:26:25.000000 gpx_vis-0.3.1/src/gpx_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-07 22:26:25.000000 gpx_vis-0.3.1/src/gpx_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       83 2024-04-07 22:26:25.000000 gpx_vis-0.3.1/src/gpx_vis.egg-info/requires.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-07 22:26:25.000000 gpx_vis-0.3.1/src/gpx_vis.egg-info/top_level.txt
+-rw-r--r--   0 jwt        (501) staff       (20)    18353 2024-04-07 22:07:19.000000 gpx_vis-0.3.1/src/gpx_vis.py
```

### Comparing `gpx_vis-0.3.0/LICENSE` & `gpx_vis-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx_vis-0.3.0/PKG-INFO` & `gpx_vis-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: gpx_vis
-Version: 0.3.0
-Summary: Plots your Komoot tours
+Version: 0.3.1
+Summary: Visualising your completed Komoot tours
 Author-email: Jia Wei Teh <jiaweiteh.astro@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: folium
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: humanfriendly
-Requires-Dist: cmasher
 Requires-Dist: reverse_geocode
 Requires-Dist: matplotlib
 Requires-Dist: vincenty
+Requires-Dist: altair
 Requires-Dist: gpxpy
 
 About `gpx_vis`
 ===============
 
-`gpx_vis` allows simple and easy visualisation of your cycling/walking tours.
+`gpx_vis` enables simple and convenient visualisation of your cycling or hiking tours.
 
-Important: currently only works for .GPX from completed paths in Komoot. In development.
+Important note: Currently, it exclusively supports .GPX files generated from completed paths in Komoot. Please be aware that this tool is still in development.
 
 Install
 -------
 
 ```bash
 pip install gpx_vis
 ```
@@ -56,39 +56,56 @@
 Map creation
 ------------
 
 ```python
 track.create_map(filename)
 ```
 
-This creates an html file saved to `path2file`. An interactive html map will be created.
-Hover mouse over route, or click on final waypoints (flag marker) for further info.
+This generates an HTML file saved under `filename`, which contains an interactive map.
+Users can hover over routes or click on final waypoints (flags) for additional information.
 
-If you have been very hard-working, thus having a large set of datapoints on the map: 
-there is an option to include `lite = True`. By default, this limits the datapoints on 
-each route to `50`. This number can be tweaked via the `nlite` argument. E.g.,
+In cases where the map contains a large dataset and loading time is a concern (if one
+has been very hardworking), users have the option to include `lite = True`. By default, this option limits the 
+number of data points displayed on each route to `50`. However, users can adjust this
+limit using the `nlite` argument, for instance,
 
 ```python
 track.create_map(filename, lite=True, nlite=100)
 ```
 
 City overview
 -------------
 
 ```python
 track.city_list
 ```
 
-Curious which city you went through along the way? This command creates a list
-of cities - sorted by country then name - that were detected through the tour. The 
-`frequency` parameter tells how many times a city was encountered; it should 
-somewhat correlate to time spent in that city.
+Interested in the cities you passed through on your journey? This command generates a list
+of cities - sorted by country and name - that were detected along the tour route. The 
+`frequency` parameter indicates how many times each city was encountered; 
+providing a rough estimate of the time spent in each city.
+
 
 Additional information
 ----------------------
 
-Should you wish to plot/inspect different values, these parameters are also accesssible via:  
+If you wish to plot or inspect different values, these parameters are also accessible via:
 
 `track.t`: time (UTC)<br>
 `track.x`: longitude (deg)<br>
 `track.y`: latitude (deg)<br>
 `track.z`: elevation (m)<br>
+
+Dependencies
+------------
+https://github.com/tkrajina/gpxpy
+https://pypi.org/project/reverse-geocode/
+https://github.com/python-visualization/folium
+https://pypi.org/project/humanfriendly/
+https://altair-viz.github.io/
+https://pypi.org/project/vincenty/
+https://numpy.org/
+https://pandas.pydata.org/
+https://pypi.org/project/branca/
+
+
+
```

### Comparing `gpx_vis-0.3.0/README.md` & `gpx_vis-0.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-About `gpx_vis`===============`gpx_vis` allows simple and easy visualisation of your cycling/walking tours.Important: currently only works for .GPX from completed paths in Komoot. In development.Install-------```bashpip install gpx_vis```Update to the latest version:```bashpip install gpx_vis --upgrade```Instantiate-----------```pythonfrom gpx_vis import Tracktrack = Track(pathname)````pathname` serves as a reference to either a single `.gpx` file or a directory.If a directory path is provided, all .gpx files contained within that directorywill be merged, but retain their original metadata (e.g., different tracks remain separated).This allows users to overlay multiple tracks onto a single map, providing a comprehensive summary of the data being analyzed.Map creation------------```pythontrack.create_map(filename)```This creates an html file saved to `path2file`. An interactive html map will be created.Hover mouse over route, or click on final waypoints (flag marker) for further info.If you have been very hard-working, thus having a large set of datapoints on the map: there is an option to include `lite = True`. By default, this limits the datapoints on each route to `50`. This number can be tweaked via the `nlite` argument. E.g.,```pythontrack.create_map(filename, lite=True, nlite=100)```City overview-------------```pythontrack.city_list```Curious which city you went through along the way? This command creates a listof cities - sorted by country then name - that were detected through the tour. The `frequency` parameter tells how many times a city was encountered; it should somewhat correlate to time spent in that city.Additional information----------------------Should you wish to plot/inspect different values, these parameters are also accesssible via:  `track.t`: time (UTC)<br>`track.x`: longitude (deg)<br>`track.y`: latitude (deg)<br>`track.z`: elevation (m)<br>
+About `gpx_vis`===============`gpx_vis` enables simple and convenient visualisation of your cycling or hiking tours.Important note: Currently, it exclusively supports .GPX files generated from completed paths in Komoot. Please be aware that this tool is still in development.Install-------```bashpip install gpx_vis```Update to the latest version:```bashpip install gpx_vis --upgrade```Instantiate-----------```pythonfrom gpx_vis import Tracktrack = Track(pathname)````pathname` serves as a reference to either a single `.gpx` file or a directory.If a directory path is provided, all .gpx files contained within that directorywill be merged, but retain their original metadata (e.g., different tracks remain separated).This allows users to overlay multiple tracks onto a single map, providing a comprehensive summary of the data being analyzed.Map creation------------```pythontrack.create_map(filename)```This generates an HTML file saved under `filename`, which contains an interactive map.Users can hover over routes or click on final waypoints (flags) for additional information.In cases where the map contains a large dataset and loading time is a concern (if onehas been very hardworking), users have the option to include `lite = True`. By default, this option limits the number of data points displayed on each route to `50`. However, users can adjust thislimit using the `nlite` argument, for instance,```pythontrack.create_map(filename, lite=True, nlite=100)```City overview-------------```pythontrack.city_list```Interested in the cities you passed through on your journey? This command generates a listof cities - sorted by country and name - that were detected along the tour route. The `frequency` parameter indicates how many times each city was encountered; providing a rough estimate of the time spent in each city.Additional information----------------------If you wish to plot or inspect different values, these parameters are also accessible via:`track.t`: time (UTC)<br>`track.x`: longitude (deg)<br>`track.y`: latitude (deg)<br>`track.z`: elevation (m)<br>Dependencies------------https://github.com/tkrajina/gpxpyhttps://pypi.org/project/reverse-geocode/https://github.com/python-visualization/foliumhttps://pypi.org/project/humanfriendly/https://altair-viz.github.io/https://pypi.org/project/vincenty/https://numpy.org/https://pandas.pydata.org/https://pypi.org/project/branca/
```

### Comparing `gpx_vis-0.3.0/pyproject.toml` & `gpx_vis-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpx_vis"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Jia Wei Teh", email="jiaweiteh.astro@gmail.com" },
 ]
-description = "Plots your Komoot tours"
+description = "Visualising your completed Komoot tours"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [    
     "folium",
     "numpy",
     "pandas",
     "humanfriendly",
-    "cmasher",
     "reverse_geocode",
     "matplotlib",
     "vincenty",
+    "altair",
     "gpxpy",
 ]
```

### Comparing `gpx_vis-0.3.0/src/gpx_vis.egg-info/PKG-INFO` & `gpx_vis-0.3.1/src/gpx_vis.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: gpx_vis
-Version: 0.3.0
-Summary: Plots your Komoot tours
+Version: 0.3.1
+Summary: Visualising your completed Komoot tours
 Author-email: Jia Wei Teh <jiaweiteh.astro@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: folium
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: humanfriendly
-Requires-Dist: cmasher
 Requires-Dist: reverse_geocode
 Requires-Dist: matplotlib
 Requires-Dist: vincenty
+Requires-Dist: altair
 Requires-Dist: gpxpy
 
 About `gpx_vis`
 ===============
 
-`gpx_vis` allows simple and easy visualisation of your cycling/walking tours.
+`gpx_vis` enables simple and convenient visualisation of your cycling or hiking tours.
 
-Important: currently only works for .GPX from completed paths in Komoot. In development.
+Important note: Currently, it exclusively supports .GPX files generated from completed paths in Komoot. Please be aware that this tool is still in development.
 
 Install
 -------
 
 ```bash
 pip install gpx_vis
 ```
@@ -56,39 +56,56 @@
 Map creation
 ------------
 
 ```python
 track.create_map(filename)
 ```
 
-This creates an html file saved to `path2file`. An interactive html map will be created.
-Hover mouse over route, or click on final waypoints (flag marker) for further info.
+This generates an HTML file saved under `filename`, which contains an interactive map.
+Users can hover over routes or click on final waypoints (flags) for additional information.
 
-If you have been very hard-working, thus having a large set of datapoints on the map: 
-there is an option to include `lite = True`. By default, this limits the datapoints on 
-each route to `50`. This number can be tweaked via the `nlite` argument. E.g.,
+In cases where the map contains a large dataset and loading time is a concern (if one
+has been very hardworking), users have the option to include `lite = True`. By default, this option limits the 
+number of data points displayed on each route to `50`. However, users can adjust this
+limit using the `nlite` argument, for instance,
 
 ```python
 track.create_map(filename, lite=True, nlite=100)
 ```
 
 City overview
 -------------
 
 ```python
 track.city_list
 ```
 
-Curious which city you went through along the way? This command creates a list
-of cities - sorted by country then name - that were detected through the tour. The 
-`frequency` parameter tells how many times a city was encountered; it should 
-somewhat correlate to time spent in that city.
+Interested in the cities you passed through on your journey? This command generates a list
+of cities - sorted by country and name - that were detected along the tour route. The 
+`frequency` parameter indicates how many times each city was encountered; 
+providing a rough estimate of the time spent in each city.
+
 
 Additional information
 ----------------------
 
-Should you wish to plot/inspect different values, these parameters are also accesssible via:  
+If you wish to plot or inspect different values, these parameters are also accessible via:
 
 `track.t`: time (UTC)<br>
 `track.x`: longitude (deg)<br>
 `track.y`: latitude (deg)<br>
 `track.z`: elevation (m)<br>
+
+Dependencies
+------------
+https://github.com/tkrajina/gpxpy
+https://pypi.org/project/reverse-geocode/
+https://github.com/python-visualization/folium
+https://pypi.org/project/humanfriendly/
+https://altair-viz.github.io/
+https://pypi.org/project/vincenty/
+https://numpy.org/
+https://pandas.pydata.org/
+https://pypi.org/project/branca/
+
+
+
```

### Comparing `gpx_vis-0.3.0/src/gpx_vis.py` & `gpx_vis-0.3.1/src/gpx_vis.py`

 * *Files identical despite different names*

