# Comparing `tmp/GeoHD-0.1.7.tar.gz` & `tmp/GeoHD-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeoHD-0.1.7.tar", last modified: Sun Apr  7 19:42:47 2024, max compression
+gzip compressed data, was "GeoHD-0.1.8.tar", last modified: Mon Apr  8 19:37:50 2024, max compression
```

## Comparing `GeoHD-0.1.7.tar` & `GeoHD-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 19:42:47.962655 GeoHD-0.1.7/
-drwxrwxrwx   0        0        0        0 2024-04-07 19:42:47.954363 GeoHD-0.1.7/GeoHD/
--rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.7/GeoHD/AKDE.py
--rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.1.7/GeoHD/__init__.py
--rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.7/GeoHD/analyze.py
--rw-rw-rw-   0        0        0     4358 2024-04-05 18:26:40.000000 GeoHD-0.1.7/GeoHD/process.py
--rw-rw-rw-   0        0        0    10826 2024-04-07 19:41:22.000000 GeoHD-0.1.7/GeoHD/utils.py
--rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.1.7/GeoHD/visualize.py
--rw-rw-rw-   0        0        0     9599 2024-04-05 18:21:57.000000 GeoHD-0.1.7/GeoHD/zone.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:42:47.960678 GeoHD-0.1.7/GeoHD.egg-info/
--rw-rw-rw-   0        0        0     5266 2024-04-07 19:42:47.000000 GeoHD-0.1.7/GeoHD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-04-07 19:42:47.000000 GeoHD-0.1.7/GeoHD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 19:42:47.000000 GeoHD-0.1.7/GeoHD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-07 19:42:47.000000 GeoHD-0.1.7/GeoHD.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 19:42:47.000000 GeoHD-0.1.7/GeoHD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     5266 2024-04-07 19:42:47.961675 GeoHD-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4768 2024-04-05 18:54:02.000000 GeoHD-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 19:42:47.962655 GeoHD-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-04-07 19:42:36.000000 GeoHD-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 19:42:47.959655 GeoHD-0.1.7/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.7/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:37:50.935317 GeoHD-0.1.8/
+drwxrwxrwx   0        0        0        0 2024-04-08 19:37:50.930373 GeoHD-0.1.8/GeoHD/
+-rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.8/GeoHD/AKDE.py
+-rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.1.8/GeoHD/__init__.py
+-rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.8/GeoHD/analyze.py
+-rw-rw-rw-   0        0        0     4358 2024-04-05 18:26:40.000000 GeoHD-0.1.8/GeoHD/process.py
+-rw-rw-rw-   0        0        0    19103 2024-04-08 19:37:31.000000 GeoHD-0.1.8/GeoHD/utils.py
+-rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.1.8/GeoHD/visualize.py
+-rw-rw-rw-   0        0        0     9599 2024-04-05 18:21:57.000000 GeoHD-0.1.8/GeoHD/zone.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:37:50.935317 GeoHD-0.1.8/GeoHD.egg-info/
+-rw-rw-rw-   0        0        0     5266 2024-04-08 19:37:50.000000 GeoHD-0.1.8/GeoHD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-08 19:37:50.000000 GeoHD-0.1.8/GeoHD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 19:37:50.000000 GeoHD-0.1.8/GeoHD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-08 19:37:50.000000 GeoHD-0.1.8/GeoHD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-08 19:37:50.000000 GeoHD-0.1.8/GeoHD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     5266 2024-04-08 19:37:50.935317 GeoHD-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4768 2024-04-05 18:54:02.000000 GeoHD-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 19:37:50.935317 GeoHD-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-04-08 19:37:40.000000 GeoHD-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:37:50.935317 GeoHD-0.1.8/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.8/test/__init__.py
```

### Comparing `GeoHD-0.1.7/GeoHD/AKDE.py` & `GeoHD-0.1.8/GeoHD/AKDE.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.7/GeoHD/analyze.py` & `GeoHD-0.1.8/GeoHD/analyze.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.7/GeoHD/process.py` & `GeoHD-0.1.8/GeoHD/process.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.7/GeoHD/visualize.py` & `GeoHD-0.1.8/GeoHD/visualize.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.7/GeoHD/zone.py` & `GeoHD-0.1.8/GeoHD/zone.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.7/GeoHD.egg-info/PKG-INFO` & `GeoHD-0.1.8/GeoHD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoHD
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
 Home-page: https://github.com/yan-yuchen/GeoHD
 Author: Yuchen Yan
 Author-email: ycyan001@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `GeoHD-0.1.7/LICENSE` & `GeoHD-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.7/PKG-INFO` & `GeoHD-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoHD
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
 Home-page: https://github.com/yan-yuchen/GeoHD
 Author: Yuchen Yan
 Author-email: ycyan001@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `GeoHD-0.1.7/README.md` & `GeoHD-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.7/setup.py` & `GeoHD-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='GeoHD',
-    version='0.1.7',
+    version='0.1.8',
     description='A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data',
     author='Yuchen Yan',
     author_email='ycyan001@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yan-yuchen/GeoHD",    
     packages=find_packages(),
```

