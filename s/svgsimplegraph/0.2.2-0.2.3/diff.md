# Comparing `tmp/svgsimplegraph-0.2.2.tar.gz` & `tmp/svgsimplegraph-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgsimplegraph-0.2.2.tar", last modified: Fri Apr  5 23:33:34 2024, max compression
+gzip compressed data, was "svgsimplegraph-0.2.3.tar", last modified: Mon Apr  8 19:58:32 2024, max compression
```

## Comparing `svgsimplegraph-0.2.2.tar` & `svgsimplegraph-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-05 23:33:34.545918 svgsimplegraph-0.2.2/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1072 2023-05-30 04:47:02.000000 svgsimplegraph-0.2.2/LICENSE
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-05 23:33:34.545620 svgsimplegraph-0.2.2/PKG-INFO
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     6599 2024-02-12 21:11:46.000000 svgsimplegraph-0.2.2/README.md
--rw-r--r--   0 garrettpetersen   (501) staff       (20)       38 2024-04-05 23:33:34.546005 svgsimplegraph-0.2.2/setup.cfg
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      957 2024-04-05 23:32:24.000000 svgsimplegraph-0.2.2/setup.py
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-05 23:33:34.540940 svgsimplegraph-0.2.2/svgsimplegraph/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      124 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.2/svgsimplegraph/__init__.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    10527 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.2/svgsimplegraph/base.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    16487 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.2/svgsimplegraph/bubble_and_arrow.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    42467 2024-04-05 23:32:24.000000 svgsimplegraph-0.2.2/svgsimplegraph/categorical.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    15007 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.2/svgsimplegraph/ribbon.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    10208 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.2/svgsimplegraph/utils.py
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-05 23:33:34.542414 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-05 23:33:34.000000 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/PKG-INFO
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      524 2024-04-05 23:33:34.000000 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/SOURCES.txt
--rw-r--r--   0 garrettpetersen   (501) staff       (20)        1 2024-04-05 23:33:34.000000 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/dependency_links.txt
--rw-r--r--   0 garrettpetersen   (501) staff       (20)       17 2024-04-05 23:33:34.000000 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/requires.txt
--rw-r--r--   0 garrettpetersen   (501) staff       (20)       21 2024-04-05 23:33:34.000000 svgsimplegraph-0.2.2/svgsimplegraph.egg-info/top_level.txt
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-05 23:33:34.544965 svgsimplegraph-0.2.2/tests/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)        0 2023-05-30 04:47:02.000000 svgsimplegraph-0.2.2/tests/__init__.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     2778 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.2/tests/test_bubble_and_arrow.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     7535 2024-04-05 23:32:24.000000 svgsimplegraph-0.2.2/tests/test_categorical.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1700 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.2/tests/test_gist.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     3562 2024-02-11 22:35:12.000000 svgsimplegraph-0.2.2/tests/test_readme_examples.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1116 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.2/tests/test_ribbon.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-08 19:58:32.886684 svgsimplegraph-0.2.3/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1072 2023-05-30 04:47:02.000000 svgsimplegraph-0.2.3/LICENSE
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-08 19:58:32.886436 svgsimplegraph-0.2.3/PKG-INFO
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     6599 2024-02-12 21:11:46.000000 svgsimplegraph-0.2.3/README.md
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)       38 2024-04-08 19:58:32.886757 svgsimplegraph-0.2.3/setup.cfg
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      936 2024-04-08 19:58:23.000000 svgsimplegraph-0.2.3/setup.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-08 19:58:32.881829 svgsimplegraph-0.2.3/svgsimplegraph/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      124 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.3/svgsimplegraph/__init__.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    10527 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.3/svgsimplegraph/base.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    16487 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.3/svgsimplegraph/bubble_and_arrow.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    42429 2024-04-08 19:58:23.000000 svgsimplegraph-0.2.3/svgsimplegraph/categorical.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    15007 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.3/svgsimplegraph/ribbon.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    10543 2024-04-08 19:58:23.000000 svgsimplegraph-0.2.3/svgsimplegraph/utils.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-08 19:58:32.882947 svgsimplegraph-0.2.3/svgsimplegraph.egg-info/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-08 19:58:32.000000 svgsimplegraph-0.2.3/svgsimplegraph.egg-info/PKG-INFO
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      487 2024-04-08 19:58:32.000000 svgsimplegraph-0.2.3/svgsimplegraph.egg-info/SOURCES.txt
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)        1 2024-04-08 19:58:32.000000 svgsimplegraph-0.2.3/svgsimplegraph.egg-info/dependency_links.txt
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)       21 2024-04-08 19:58:32.000000 svgsimplegraph-0.2.3/svgsimplegraph.egg-info/top_level.txt
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-08 19:58:32.885826 svgsimplegraph-0.2.3/tests/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)        0 2023-05-30 04:47:02.000000 svgsimplegraph-0.2.3/tests/__init__.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     2778 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.3/tests/test_bubble_and_arrow.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     7535 2024-04-05 23:32:24.000000 svgsimplegraph-0.2.3/tests/test_categorical.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1700 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.3/tests/test_gist.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     3562 2024-02-11 22:35:12.000000 svgsimplegraph-0.2.3/tests/test_readme_examples.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1116 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.3/tests/test_ribbon.py
```

### Comparing `svgsimplegraph-0.2.2/LICENSE` & `svgsimplegraph-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.2/PKG-INFO` & `svgsimplegraph-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgsimplegraph
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple SVG graphing package
 Author: Garrett M. Petersen
 Author-email: garrett.m.petersen@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/GarrettPetersen/svgsimplegraph
 Keywords: graph,svg,base64,svg simple graph
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `svgsimplegraph-0.2.2/README.md` & `svgsimplegraph-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.2/setup.py` & `svgsimplegraph-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 # Read in the README.md for the long description on PyPI
 with open("README.md", "r") as f:
     long_description = f.read()
 
-VERSION = "0.2.2"
+VERSION = "0.2.3"
 DESCRIPTION = "Simple SVG graphing package"
 
 setup(
     name="svgsimplegraph",
     version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Garrett M. Petersen",
     author_email="garrett.m.petersen@gmail.com",
     license="MIT",
     packages=find_packages(),
-    install_requires=["matplotlib", "numpy"],
+    install_requires=[],
     keywords=["graph", "svg", "base64", "svg simple graph"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
```

### Comparing `svgsimplegraph-0.2.2/svgsimplegraph/base.py` & `svgsimplegraph-0.2.3/svgsimplegraph/base.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.2/svgsimplegraph/bubble_and_arrow.py` & `svgsimplegraph-0.2.3/svgsimplegraph/bubble_and_arrow.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.2/svgsimplegraph/categorical.py` & `svgsimplegraph-0.2.3/svgsimplegraph/categorical.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,15 +946,15 @@
                                 10,
                                 self.font_width_estimate_multiplier,
                             )[0]
                             if self.legend_labels[next_index_with_label] is not None:
                                 break
                             next_index_with_label += 1
 
-                        if (legend_x > 0) and (
+                        if (
                             legend_x
                             + legend_rect_size
                             + self.element_spacing / 2
                             + next_label_width
                             > self.width
                         ):
                             legend_y = (
@@ -1027,15 +1027,15 @@
                                 10,
                                 self.font_width_estimate_multiplier,
                             )[0]
                             if self.legend_labels[next_index_with_label] is not None:
                                 break
                             next_index_with_label += 1
 
-                        if (legend_x > 0) and (
+                        if (
                             legend_x
                             + legend_rect_size
                             + self.element_spacing / 2
                             + next_label_width
                             > self.width
                         ):
                             legend_y = (
```

### Comparing `svgsimplegraph-0.2.2/svgsimplegraph/ribbon.py` & `svgsimplegraph-0.2.3/svgsimplegraph/ribbon.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.2/svgsimplegraph/utils.py` & `svgsimplegraph-0.2.3/svgsimplegraph/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import math
-import matplotlib
-import numpy as np
 
 
 def polar_to_cartesian(angle, radius, x=0, y=0):
     x = x + radius * math.cos(angle)
     y = y + radius * math.sin(angle)
     return x, y
 
@@ -69,41 +67,52 @@
     # Return the amount of vertical overlap
     if y1 < y2:
         return bottom1 - top2
     else:
         return bottom2 - top1
 
 
+def hex_to_rgb(color):
+    """Convert a hex color to an RGB tuple."""
+    color = color.lstrip("#")
+    lv = len(color)
+    return tuple(int(color[i : i + lv // 3], 16) / 255.0 for i in range(0, lv, lv // 3))
+
+
+def rgb_to_hex(rgb):
+    """Convert an RGB tuple to a hex color."""
+    return "#" + "".join(f"{int(c*255):02x}" for c in rgb)
+
+
 def get_color(val, colors):
     # Convert hex colors to RGB
-    rgbs = [np.array(matplotlib.colors.hex2color(color)) for color in colors]
+    rgbs = [hex_to_rgb(color) for color in colors]
 
     # Assign values to color ranges
-    ranges = np.linspace(0, 1, len(colors))
+    num_colors = len(colors)
+    ranges = [i / (num_colors - 1) for i in range(num_colors)]
 
     # If value is outside the defined range, use the edge colors.
     if val <= 0:
         return colors[0]
     elif val >= 1:
         return colors[-1]
 
     # Find the two colors between which the value lies.
     for i in range(len(ranges) - 1):
-        # Adjust the ranges to match the colors properly
         low_range = ranges[i]
         high_range = ranges[i + 1]
-        # Perform interpolation if val falls within the adjusted ranges
         if low_range <= val < high_range:
             t = (val - low_range) / (high_range - low_range)
-            color = rgbs[i] * (1 - t) + rgbs[i + 1] * t
-            break
-    else:
-        color = rgbs[0]  # default to the first color if no range found
+            # Linearly interpolate between the two colors
+            color = tuple(a * (1 - t) + b * t for a, b in zip(rgbs[i], rgbs[i + 1]))
+            return rgb_to_hex(color)
 
-    return matplotlib.colors.rgb2hex(color)
+    # Default case, should not be reached due to checks for val <= 0 and val >= 1
+    return colors[0]
 
 
 def hex_to_rgba(hex_color, alpha=1.0):
     r = int(hex_color[1:3], 16)
     g = int(hex_color[3:5], 16)
     b = int(hex_color[5:7], 16)
     return f"rgba({r}, {g}, {b}, {alpha})"
@@ -153,15 +162,19 @@
             axis_min = -math.ceil(abs(min_val) / step_size) * step_size
     else:
         axis_min = step_size * math.floor(min_val / step_size)
 
     axis_max = step_size * math.ceil(max_val / step_size)
 
     # Generate the list of ticks
-    ticks = list(np.arange(axis_min, axis_max + step_size, step_size))
+    ticks = []
+    current = axis_min
+    while current <= axis_max:
+        ticks.append(current)
+        current += step_size
 
     if include_zero:
         assert 0 in ticks, "Zero should be included in the ticks."
 
     return ticks
```

### Comparing `svgsimplegraph-0.2.2/svgsimplegraph.egg-info/PKG-INFO` & `svgsimplegraph-0.2.3/svgsimplegraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgsimplegraph
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple SVG graphing package
 Author: Garrett M. Petersen
 Author-email: garrett.m.petersen@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/GarrettPetersen/svgsimplegraph
 Keywords: graph,svg,base64,svg simple graph
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `svgsimplegraph-0.2.2/tests/test_bubble_and_arrow.py` & `svgsimplegraph-0.2.3/tests/test_bubble_and_arrow.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.2/tests/test_categorical.py` & `svgsimplegraph-0.2.3/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.2/tests/test_gist.py` & `svgsimplegraph-0.2.3/tests/test_gist.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.2/tests/test_readme_examples.py` & `svgsimplegraph-0.2.3/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.2/tests/test_ribbon.py` & `svgsimplegraph-0.2.3/tests/test_ribbon.py`

 * *Files identical despite different names*

