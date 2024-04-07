# Comparing `tmp/landborn-0.2.4.tar.gz` & `tmp/landborn-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landborn-0.2.4.tar", last modified: Sat Apr  6 00:07:09 2024, max compression
+gzip compressed data, was "landborn-0.2.5.tar", last modified: Sun Apr  7 23:46:36 2024, max compression
```

## Comparing `landborn-0.2.4.tar` & `landborn-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-06 00:07:09.006482 landborn-0.2.4/
--rw-r--r--   0 mollynelson   (501) staff       (20)     1063 2024-02-16 00:51:51.000000 landborn-0.2.4/LICENSE
--rw-r--r--   0 mollynelson   (501) staff       (20)     1098 2024-04-06 00:07:09.006063 landborn-0.2.4/PKG-INFO
--rw-r--r--   0 mollynelson   (501) staff       (20)      871 2024-04-05 23:46:10.000000 landborn-0.2.4/README.md
-drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-06 00:07:09.001277 landborn-0.2.4/landborn/
--rw-r--r--   0 mollynelson   (501) staff       (20)      407 2024-04-06 00:06:48.000000 landborn-0.2.4/landborn/__init__.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     5633 2024-04-05 16:26:56.000000 landborn-0.2.4/landborn/barplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     7484 2024-04-05 22:56:49.000000 landborn-0.2.4/landborn/colormap.py
--rw-r--r--   0 mollynelson   (501) staff       (20)      319 2024-04-06 00:06:23.000000 landborn-0.2.4/landborn/config.py
--rw-r--r--   0 mollynelson   (501) staff       (20)    15200 2024-04-05 23:18:51.000000 landborn-0.2.4/landborn/functions.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     5224 2024-04-05 22:40:43.000000 landborn-0.2.4/landborn/gradient.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     1068 2024-02-28 16:46:45.000000 landborn-0.2.4/landborn/jointplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     4793 2024-04-05 22:47:21.000000 landborn-0.2.4/landborn/lineplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     5908 2024-04-05 22:46:40.000000 landborn-0.2.4/landborn/scatterplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     2292 2024-03-03 18:53:57.000000 landborn-0.2.4/landborn/swarmplot3.py
-drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-06 00:07:09.005420 landborn-0.2.4/landborn.egg-info/
--rw-r--r--   0 mollynelson   (501) staff       (20)     1098 2024-04-06 00:07:08.000000 landborn-0.2.4/landborn.egg-info/PKG-INFO
--rw-r--r--   0 mollynelson   (501) staff       (20)      399 2024-04-06 00:07:08.000000 landborn-0.2.4/landborn.egg-info/SOURCES.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)        1 2024-04-06 00:07:08.000000 landborn-0.2.4/landborn.egg-info/dependency_links.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)       24 2024-04-06 00:07:08.000000 landborn-0.2.4/landborn.egg-info/requires.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)        9 2024-04-06 00:07:08.000000 landborn-0.2.4/landborn.egg-info/top_level.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)       38 2024-04-06 00:07:09.006655 landborn-0.2.4/setup.cfg
--rw-r--r--   0 mollynelson   (501) staff       (20)      536 2024-04-06 00:06:43.000000 landborn-0.2.4/setup.py
+drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-07 23:46:36.473875 landborn-0.2.5/
+-rw-r--r--   0 mollynelson   (501) staff       (20)     1063 2024-02-16 00:51:51.000000 landborn-0.2.5/LICENSE
+-rw-r--r--   0 mollynelson   (501) staff       (20)     4121 2024-04-07 23:46:36.472786 landborn-0.2.5/PKG-INFO
+-rw-r--r--   0 mollynelson   (501) staff       (20)     3894 2024-04-07 23:41:57.000000 landborn-0.2.5/README.md
+drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-07 23:46:36.465640 landborn-0.2.5/landborn/
+-rw-r--r--   0 mollynelson   (501) staff       (20)      465 2024-04-07 23:46:22.000000 landborn-0.2.5/landborn/__init__.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     5633 2024-04-05 16:26:56.000000 landborn-0.2.5/landborn/barplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     7484 2024-04-05 22:56:49.000000 landborn-0.2.5/landborn/colormap.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)      315 2024-04-07 23:11:16.000000 landborn-0.2.5/landborn/config.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)    15200 2024-04-05 23:18:51.000000 landborn-0.2.5/landborn/functions.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     5504 2024-04-07 23:20:31.000000 landborn-0.2.5/landborn/heatmap.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     1068 2024-02-28 16:46:45.000000 landborn-0.2.5/landborn/jointplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     4793 2024-04-05 22:47:21.000000 landborn-0.2.5/landborn/lineplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     5908 2024-04-05 22:46:40.000000 landborn-0.2.5/landborn/scatterplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     2292 2024-03-03 18:53:57.000000 landborn-0.2.5/landborn/swarmplot3.py
+drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-07 23:46:36.471262 landborn-0.2.5/landborn.egg-info/
+-rw-r--r--   0 mollynelson   (501) staff       (20)     4121 2024-04-07 23:46:36.000000 landborn-0.2.5/landborn.egg-info/PKG-INFO
+-rw-r--r--   0 mollynelson   (501) staff       (20)      398 2024-04-07 23:46:36.000000 landborn-0.2.5/landborn.egg-info/SOURCES.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)        1 2024-04-07 23:46:36.000000 landborn-0.2.5/landborn.egg-info/dependency_links.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)       31 2024-04-07 23:46:36.000000 landborn-0.2.5/landborn.egg-info/requires.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)        9 2024-04-07 23:46:36.000000 landborn-0.2.5/landborn.egg-info/top_level.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)       38 2024-04-07 23:46:36.474158 landborn-0.2.5/setup.cfg
+-rw-r--r--   0 mollynelson   (501) staff       (20)      546 2024-04-07 23:45:53.000000 landborn-0.2.5/setup.py
```

### Comparing `landborn-0.2.4/LICENSE` & `landborn-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `landborn-0.2.4/landborn/barplot.py` & `landborn-0.2.5/landborn/barplot.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.4/landborn/colormap.py` & `landborn-0.2.5/landborn/colormap.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.4/landborn/functions.py` & `landborn-0.2.5/landborn/functions.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.4/landborn/gradient.py` & `landborn-0.2.5/landborn/heatmap.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,171 @@
 import matplotlib.pyplot as plt
+import matplotlib
 import numpy as np
 from matplotlib.collections import LineCollection
 from matplotlib.colors import Normalize
 from matplotlib.cm import ScalarMappable
-from matplotlib.colorbar import ColorbarBase
-from matplotlib.cm import viridis
 from config import Config
 import plotly.graph_objects as go
 import pandas as pd
+from matplotlib.colors import Normalize
+
+def gradient_heatmap(data, colormap='viridis', title="Gradient HeatMap", x_label="Data Point Index", save_path=None):
+    if Config.plot_backend == 'matplotlib':
+        gradient_heatmap_matplotlib(data, colormap=colormap, title=title, x_label=x_label,save_path=save_path)
+    elif Config.plot_backend == 'plotly':
+        gradient_heatmap_plotly(data, colormap=colormap, title=title, x_label=x_label,save_path=save_path)
+
 
-def custom_visualization_matplotlib(data):
+def gradient_heatmap_matplotlib(data, colormap='viridis', title="Data Visualization", x_label="testing x",save_path=None):
     fig, ax = plt.subplots()
-    # Normalize data for colormap
+    
     norm = Normalize(vmin=min(data), vmax=max(data))
-    cmap = viridis
+    cmap_name = colormap + '_r'
+    cmap = matplotlib.colormaps[cmap_name]
 
-    # Calculate optimal linewidth to make lines touch
     dpi = fig.get_dpi()
     fig_width_in_inches = fig.get_figwidth()
     total_points = len(data)
     linewidth = (fig_width_in_inches * dpi) / total_points
 
-    # Create a set of lines
     lines = []
     for i, value in enumerate(data):
-        color = cmap(norm(value))  # Map data value to colormap
-        line = [(i, 0), (i, 1)]  # Vertical line from (i, 0) to (i, 1)
+        color = cmap(norm(value))
+        line = [(i, 0), (i, 1)]
         lines.append((line, color))
 
-    # Create a LineCollection from the lines
     line_segments = LineCollection([line for line, color in lines], colors=[color for line, color in lines], linewidths=(linewidth,))
     ax.add_collection(line_segments)
 
-    # Add Colorbar
     sm = ScalarMappable(cmap=cmap, norm=norm)
     sm.set_array([])
     fig.colorbar(sm, ax=ax)
 
-    # Set limits and labels
     ax.set_xlim(0, len(data))
     ax.set_ylim(0, 1)
     ax.set_yticks([])
-    plt.show()
+    ax.set_xlabel(x_label)
+    ax.set_title(title)
+    
+    if save_path:
+        plt.savefig(save_path)
+    else:
+        plt.show()
 
 
-def custom_visualization_plotly(data, x_label="Data Point Index", y_label="", title="Data Visualization with Viridis", save_path=None):
-    # Prepare data for plotting
+def gradient_heatmap_plotly(data, colormap='Viridis', title="Data Visualization", x_label="Data Point Index", save_path=None):
     x_data = list(range(len(data)))
-    y_data = [1] * len(data)  # Constant height for all bars
-    hover_texts = [f"Value: {value:.2f}" for value in data] 
+    y_data = [1] * len(data)
+    hover_texts = [f"Value: {value:.2f}" for value in data]
+    
+    colorscale_name = colormap + "_r"
     
     fig = go.Figure(data=go.Bar(
         x=x_data,
         y=y_data,
-        # text=hover_texts,  # Assign hover text for each bar
+        text=hover_texts,
         hoverinfo="text+x",
         marker=dict(
-            color=data,  # Assign data values for color mapping
-            colorscale='Viridis',  # Use the Viridis color scale
-            colorbar=dict(title=y_label)  # Optional: customize the colorbar title
+            color=data,
+            colorscale=colorscale_name,
+            # colorbar=dict(title=y_label)
         ),
-        width=np.full(len(data), 1.05)  # Make bars touch by setting width > 1
+        width=np.full(len(data), 1.05)
     ))
 
-    # Update layout for axes, labels, and background
     fig.update_layout(
         xaxis=dict(
             title=x_label,
-            showticklabels=False,
+            showticklabels=True,
         ),
         yaxis=dict(
-            showticklabels=False,  # Typically, no need for y-axis labels in this visualization
-            title=y_label,
+            showticklabels=False,
+            title="",
         ),
         title=title,
         paper_bgcolor="white",
         plot_bgcolor="white",
         margin=dict(l=40, r=40, t=40, b=40),
     )
 
-    # fig.update_layout(width=800, height=300)
     if save_path:
         fig.write_html(save_path)
     else:
         fig.show()
 
 
-import plotly.graph_objects as go
-import pandas as pd
-import numpy as np
+def month_year_heatmap(df, title="", colormap='viridis', save_path=None):
+    if Config.plot_backend == 'matplotlib':
+        month_year_heatmap_matplotlib(df=df, title=title, colormap=colormap, save_path=save_path)
+    elif Config.plot_backend == 'plotly':
+        month_year_heatmap_plotly(df=df, title=title, colormap=colormap, save_path=save_path)
+
+def month_year_heatmap_matplotlib(df, title='Month-Year Heatmap', colormap='viridis', save_path=None):
+    norm = Normalize(vmin=df.min().min(), vmax=df.max().max())
+    cmap = matplotlib.colormaps[colormap + "_r"]
+
+    fig, ax = plt.subplots()
+    cax = ax.imshow(df.values, cmap=cmap, norm=norm, aspect='auto')
+
+    ax.set_xticks(np.arange(len(df.columns)))
+    ax.set_yticks(np.arange(len(df.index)))
+    ax.set_xticklabels(df.columns)
+    ax.set_yticklabels(df.index)
+    
+    plt.setp(ax.get_xticklabels(), rotation=45, ha="right", rotation_mode="anchor")
+    cbar = plt.colorbar(cax, ax=ax)
+    cbar.ax.set_ylabel('Magnitude', rotation=-90, va="bottom")
+    ax.set_title(title)
+
+    if save_path:
+        plt.savefig(save_path)
+    else:
+        plt.show()
+
+def month_year_heatmap_plotly(df, title='Month-Year Heatmap', colormap='Viridis', save_path=None):
 
-# Example DataFrame setup with random data
-np.random.seed(0)  # For consistent random data
-data = np.random.rand(12, 21)  # 12 months, 5 years of data
-
-years = [2010,2011,2012,2013,2014,2015,2016, 2017, 2018, 2019, 2020,2021,2022,2023,2024,2025,2026,2027,2028,2029,2030]  # Example years
-months = [
-    "January", "February", "March", "April", "May", "June",
-    "July", "August", "September", "October", "November", "December"
-]
-
-df = pd.DataFrame(data, index=months, columns=years)
-
-def create_month_year_heatmap(df, title='Month-Year Heatmap', colormap='Viridis', save_path=None):
-    """
-    Create a heatmap with month names on the y-axis and years on the x-axis.
-    
-    Parameters:
-    - df: DataFrame with years as columns, month names as the row index.
-    - title: Title of the heatmap.
-    """
-    hover_texts = [f"Value: {value:.2f}" for value in data] 
     fig = go.Figure(data=go.Heatmap(
-        z=df.values,  # Data values
-        x=df.columns,  # Year on the x-axis
-        y=df.index,  # Month names on the y-axis
-        colorscale=colormap,  # Color scale
-        colorbar=dict(title='Magnitude'),  # Colorbar configuration
+        z=df.values,
+        x=df.columns,
+        y=df.index,
+        colorscale=colormap + "_r",
+        colorbar=dict(title='Magnitude'),
     ))
 
-    # Update layout
     fig.update_layout(
         title=title,
-        xaxis=dict(title='Year', type='category'),  # Treat years as categories
-        yaxis=dict(title='Month'),  # No need for dtick here since we're using month names
+        xaxis=dict(title='Year', type='category'),
+        yaxis=dict(title='Month'),
     )
-    
     if save_path:
         fig.write_html(save_path)
     else:
         fig.show()
 
-create_month_year_heatmap(df, title='Month-Year Heatmap Test')
-
-
-
-
-
 
 
 
 
 if __name__ == "__main__":
-    li = np.concatenate([np.random.randint(0, 20, size=800), np.random.randint(20, 30, size=800), np.random.randint(30, 100, size=800)])
+    li = np.concatenate([np.random.randint(0, 20, size=400), np.random.randint(20, 30, size=400), np.random.randint(30, 100, size=400)])
     # print(li)
-    # custom_visualization_matplotlib(li)
-    data = np.random.rand(100)  # Example data
+    gradient_heatmap(li)
+    # data = np.random.rand(100)
 
-    if Config.plot_backend == 'matplotlib':
-        custom_visualization_matplotlib(data)
-    elif Config.plot_backend == 'plotly':
-        custom_visualization_plotly(li )
+    # data = pd.DataFrame({
+    #     'Category 1': np.random.rand(10),
+    #     'Category 2': np.random.rand(10),
+    #     'Category 3': np.random.rand(10),
+    # }, index=pd.date_range(start='2021-01-01', periods=10, freq='D'))
     
-    # Example usage
-    # Assuming 'data' is a pandas DataFrame with a DateTimeIndex
-    data = pd.DataFrame({
-        'Category 1': np.random.rand(10),
-        'Category 2': np.random.rand(10),
-        'Category 3': np.random.rand(10),
-    }, index=pd.date_range(start='2021-01-01', periods=10, freq='D'))
+    np.random.seed(0)
+    data = np.random.rand(12, 31)  #12 months, 5 years of data
+
+    years = [2010,2011,2012,2013,2014,2015,2016, 2017, 2018, 2019, 2020,2021,2022,2023,2024,2025,2026,2027,2028,2029,2030,2031,2032,2033,2034,2035,2036,2037,2038,2039,2040]
+    months = [
+        "January", "February", "March", "April", "May", "June",
+        "July", "August", "September", "October", "November", "December"
+    ]
+
+    df = pd.DataFrame(data, index=months, columns=years)
+    # month_year_heatmap(df, title='Month-Year Heatmap Test', colormap="magma")
```

### Comparing `landborn-0.2.4/landborn/jointplot.py` & `landborn-0.2.5/landborn/jointplot.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.4/landborn/lineplot.py` & `landborn-0.2.5/landborn/lineplot.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.4/landborn/scatterplot.py` & `landborn-0.2.5/landborn/scatterplot.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.4/landborn/swarmplot3.py` & `landborn-0.2.5/landborn/swarmplot3.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.4/setup.py` & `landborn-0.2.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import find_packages, setup
 
 setup(
     name='landborn',
     packages=find_packages(include=['landborn']),
-    version='0.2.4',
+    version='0.2.5',
     description='Landborn Visualization Library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Molly Nelson',
     author_email="mollyynelson@gmail.com",
     license='MIT',
-    install_requires=['pandas', 'numpy', 'matplotlib'],
+    install_requires=['pandas', 'numpy', 'matplotlib', 'plotly'],
     setup_requires=['pytest-runner'],
     tests_require=['pytest==8.0.0'],
     test_suite='tests'
 )
```

