# Comparing `tmp/landborn-0.2.5.tar.gz` & `tmp/landborn-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landborn-0.2.5.tar", last modified: Sun Apr  7 23:46:36 2024, max compression
+gzip compressed data, was "landborn-0.2.6.tar", last modified: Mon Apr  8 01:47:31 2024, max compression
```

## Comparing `landborn-0.2.5.tar` & `landborn-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-07 23:46:36.473875 landborn-0.2.5/
--rw-r--r--   0 mollynelson   (501) staff       (20)     1063 2024-02-16 00:51:51.000000 landborn-0.2.5/LICENSE
--rw-r--r--   0 mollynelson   (501) staff       (20)     4121 2024-04-07 23:46:36.472786 landborn-0.2.5/PKG-INFO
--rw-r--r--   0 mollynelson   (501) staff       (20)     3894 2024-04-07 23:41:57.000000 landborn-0.2.5/README.md
-drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-07 23:46:36.465640 landborn-0.2.5/landborn/
--rw-r--r--   0 mollynelson   (501) staff       (20)      465 2024-04-07 23:46:22.000000 landborn-0.2.5/landborn/__init__.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     5633 2024-04-05 16:26:56.000000 landborn-0.2.5/landborn/barplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     7484 2024-04-05 22:56:49.000000 landborn-0.2.5/landborn/colormap.py
--rw-r--r--   0 mollynelson   (501) staff       (20)      315 2024-04-07 23:11:16.000000 landborn-0.2.5/landborn/config.py
--rw-r--r--   0 mollynelson   (501) staff       (20)    15200 2024-04-05 23:18:51.000000 landborn-0.2.5/landborn/functions.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     5504 2024-04-07 23:20:31.000000 landborn-0.2.5/landborn/heatmap.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     1068 2024-02-28 16:46:45.000000 landborn-0.2.5/landborn/jointplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     4793 2024-04-05 22:47:21.000000 landborn-0.2.5/landborn/lineplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     5908 2024-04-05 22:46:40.000000 landborn-0.2.5/landborn/scatterplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     2292 2024-03-03 18:53:57.000000 landborn-0.2.5/landborn/swarmplot3.py
-drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-07 23:46:36.471262 landborn-0.2.5/landborn.egg-info/
--rw-r--r--   0 mollynelson   (501) staff       (20)     4121 2024-04-07 23:46:36.000000 landborn-0.2.5/landborn.egg-info/PKG-INFO
--rw-r--r--   0 mollynelson   (501) staff       (20)      398 2024-04-07 23:46:36.000000 landborn-0.2.5/landborn.egg-info/SOURCES.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)        1 2024-04-07 23:46:36.000000 landborn-0.2.5/landborn.egg-info/dependency_links.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)       31 2024-04-07 23:46:36.000000 landborn-0.2.5/landborn.egg-info/requires.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)        9 2024-04-07 23:46:36.000000 landborn-0.2.5/landborn.egg-info/top_level.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)       38 2024-04-07 23:46:36.474158 landborn-0.2.5/setup.cfg
--rw-r--r--   0 mollynelson   (501) staff       (20)      546 2024-04-07 23:45:53.000000 landborn-0.2.5/setup.py
+drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-08 01:47:31.140062 landborn-0.2.6/
+-rw-r--r--   0 mollynelson   (501) staff       (20)     1063 2024-02-16 00:51:51.000000 landborn-0.2.6/LICENSE
+-rw-r--r--   0 mollynelson   (501) staff       (20)     4121 2024-04-08 01:47:31.137532 landborn-0.2.6/PKG-INFO
+-rw-r--r--   0 mollynelson   (501) staff       (20)     3894 2024-04-07 23:41:57.000000 landborn-0.2.6/README.md
+drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-08 01:47:31.118042 landborn-0.2.6/landborn/
+-rw-r--r--   0 mollynelson   (501) staff       (20)      465 2024-04-08 01:46:27.000000 landborn-0.2.6/landborn/__init__.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     5633 2024-04-05 16:26:56.000000 landborn-0.2.6/landborn/barplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     7484 2024-04-05 22:56:49.000000 landborn-0.2.6/landborn/colormap.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)      315 2024-04-07 23:11:16.000000 landborn-0.2.6/landborn/config.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)    15200 2024-04-05 23:18:51.000000 landborn-0.2.6/landborn/functions.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     5516 2024-04-08 01:44:46.000000 landborn-0.2.6/landborn/heatmap.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     1068 2024-02-28 16:46:45.000000 landborn-0.2.6/landborn/jointplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     4793 2024-04-05 22:47:21.000000 landborn-0.2.6/landborn/lineplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     5908 2024-04-05 22:46:40.000000 landborn-0.2.6/landborn/scatterplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     2292 2024-03-03 18:53:57.000000 landborn-0.2.6/landborn/swarmplot3.py
+drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-08 01:47:31.134693 landborn-0.2.6/landborn.egg-info/
+-rw-r--r--   0 mollynelson   (501) staff       (20)     4121 2024-04-08 01:47:30.000000 landborn-0.2.6/landborn.egg-info/PKG-INFO
+-rw-r--r--   0 mollynelson   (501) staff       (20)      398 2024-04-08 01:47:30.000000 landborn-0.2.6/landborn.egg-info/SOURCES.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)        1 2024-04-08 01:47:30.000000 landborn-0.2.6/landborn.egg-info/dependency_links.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)       31 2024-04-08 01:47:30.000000 landborn-0.2.6/landborn.egg-info/requires.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)        9 2024-04-08 01:47:30.000000 landborn-0.2.6/landborn.egg-info/top_level.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)       38 2024-04-08 01:47:31.140359 landborn-0.2.6/setup.cfg
+-rw-r--r--   0 mollynelson   (501) staff       (20)      546 2024-04-08 01:46:32.000000 landborn-0.2.6/setup.py
```

### Comparing `landborn-0.2.5/LICENSE` & `landborn-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `landborn-0.2.5/PKG-INFO` & `landborn-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landborn
-Version: 0.2.5
+Version: 0.2.6
 Summary: Landborn Visualization Library
 Author: Molly Nelson
 Author-email: mollyynelson@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `landborn-0.2.5/README.md` & `landborn-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `landborn-0.2.5/landborn/barplot.py` & `landborn-0.2.6/landborn/barplot.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.5/landborn/colormap.py` & `landborn-0.2.6/landborn/colormap.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.5/landborn/functions.py` & `landborn-0.2.6/landborn/functions.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.5/landborn/heatmap.py` & `landborn-0.2.6/landborn/heatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import matplotlib.pyplot as plt
 import matplotlib
 import numpy as np
 from matplotlib.collections import LineCollection
 from matplotlib.colors import Normalize
 from matplotlib.cm import ScalarMappable
-from config import Config
+from .config import Config
 import plotly.graph_objects as go
 import pandas as pd
 from matplotlib.colors import Normalize
 
 def gradient_heatmap(data, colormap='viridis', title="Gradient HeatMap", x_label="Data Point Index", save_path=None):
     if Config.plot_backend == 'matplotlib':
         gradient_heatmap_matplotlib(data, colormap=colormap, title=title, x_label=x_label,save_path=save_path)
@@ -145,15 +145,15 @@
 
 
 
 
 if __name__ == "__main__":
     li = np.concatenate([np.random.randint(0, 20, size=400), np.random.randint(20, 30, size=400), np.random.randint(30, 100, size=400)])
     # print(li)
-    gradient_heatmap(li)
+    # gradient_heatmap(li)
     # data = np.random.rand(100)
 
     # data = pd.DataFrame({
     #     'Category 1': np.random.rand(10),
     #     'Category 2': np.random.rand(10),
     #     'Category 3': np.random.rand(10),
     # }, index=pd.date_range(start='2021-01-01', periods=10, freq='D'))
@@ -164,8 +164,8 @@
     years = [2010,2011,2012,2013,2014,2015,2016, 2017, 2018, 2019, 2020,2021,2022,2023,2024,2025,2026,2027,2028,2029,2030,2031,2032,2033,2034,2035,2036,2037,2038,2039,2040]
     months = [
         "January", "February", "March", "April", "May", "June",
         "July", "August", "September", "October", "November", "December"
     ]
 
     df = pd.DataFrame(data, index=months, columns=years)
-    # month_year_heatmap(df, title='Month-Year Heatmap Test', colormap="magma")
+    month_year_heatmap_matplotlib(df, title='Month-Year Heatmap Test', colormap="magma")
```

### Comparing `landborn-0.2.5/landborn/jointplot.py` & `landborn-0.2.6/landborn/jointplot.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.5/landborn/lineplot.py` & `landborn-0.2.6/landborn/lineplot.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.5/landborn/scatterplot.py` & `landborn-0.2.6/landborn/scatterplot.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.5/landborn/swarmplot3.py` & `landborn-0.2.6/landborn/swarmplot3.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.5/landborn.egg-info/PKG-INFO` & `landborn-0.2.6/landborn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landborn
-Version: 0.2.5
+Version: 0.2.6
 Summary: Landborn Visualization Library
 Author: Molly Nelson
 Author-email: mollyynelson@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `landborn-0.2.5/setup.py` & `landborn-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name='landborn',
     packages=find_packages(include=['landborn']),
-    version='0.2.5',
+    version='0.2.6',
     description='Landborn Visualization Library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Molly Nelson',
     author_email="mollyynelson@gmail.com",
     license='MIT',
     install_requires=['pandas', 'numpy', 'matplotlib', 'plotly'],
```

