# Comparing `tmp/praklib-0.1.420.tar.gz` & `tmp/praklib-0.1.421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.1.420.tar", last modified: Sat Apr  6 10:08:30 2024, max compression
+gzip compressed data, was "praklib-0.1.421.tar", last modified: Mon Apr  8 18:54:39 2024, max compression
```

## Comparing `praklib-0.1.420.tar` & `praklib-0.1.421.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 10:08:30.759188 praklib-0.1.420/
--rw-rw-rw-   0        0        0      263 2024-04-06 10:08:30.755885 praklib-0.1.420/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 10:08:30.719806 praklib-0.1.420/praklib/
--rw-rw-rw-   0        0        0     6179 2024-04-06 10:08:29.000000 praklib-0.1.420/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.420/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 10:08:30.753880 praklib-0.1.420/praklib.egg-info/
--rw-rw-rw-   0        0        0      263 2024-04-06 10:08:30.000000 praklib-0.1.420/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-06 10:08:30.000000 praklib-0.1.420/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 10:08:30.000000 praklib-0.1.420/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-06 10:08:30.000000 praklib-0.1.420/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 10:08:30.759188 praklib-0.1.420/setup.cfg
--rw-rw-rw-   0        0        0      382 2024-04-06 10:08:29.000000 praklib-0.1.420/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:54:38.996932 praklib-0.1.421/
+-rw-rw-rw-   0        0        0      263 2024-04-08 18:54:38.995854 praklib-0.1.421/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-08 18:54:38.975005 praklib-0.1.421/praklib/
+-rw-rw-rw-   0        0        0     6680 2024-04-08 18:54:18.000000 praklib-0.1.421/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.421/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:54:38.993851 praklib-0.1.421/praklib.egg-info/
+-rw-rw-rw-   0        0        0      263 2024-04-08 18:54:38.000000 praklib-0.1.421/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-08 18:54:38.000000 praklib-0.1.421/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 18:54:38.000000 praklib-0.1.421/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 18:54:38.000000 praklib-0.1.421/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 18:54:38.997933 praklib-0.1.421/setup.cfg
+-rw-rw-rw-   0        0        0      382 2024-04-08 18:54:37.000000 praklib-0.1.421/setup.py
```

### Comparing `praklib-0.1.420/praklib/Praktika.py` & `praklib-0.1.421/praklib/Praktika.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,15 +135,16 @@
     latex_table += "\\end{tabular}\n"
     latex_table += "\\caption{Values and their errors}\n"
     latex_table += "\\label{tab:values}\n"
     latex_table += "\\end{table}"
 
     return latex_table
 
-def graf_3d(data, xlabel = "X", ylabel = "Y", zlabel = "Z", cbarlabel = "height", cmap='viridis', projection='ortho', fcl=1):
+def graf_3d(data, xlabel = "X", ylabel = "Y", zlabel = "Z", cbarlabel = "height", cmap='viridis', projection='ortho',
+            fcl=1, velikost=0):
 
     # Create meshgrid
     x = np.arange(data.shape[1])
     y = np.arange(data.shape[0])
     X, Y = np.meshgrid(x, y)
 
     # Create 3D plot
@@ -163,8 +164,25 @@
 
     if projection=='ortho':
         ax.set_proj_type(projection)
     else:
         ax.set_proj_type(projection, focal_length=fcl)
 
     # Show plot
-    plt.show()
+    plt.show()
+
+
+def unp_to_np(unumpy_array, imag_errs=False):
+    values = unp.nominal_values(unumpy_array)
+    uncertainties = unp.std_devs(unumpy_array)
+
+    if imag_errs==False:
+        return np.column_stack((values, uncertainties))
+    if imag_errs==True:
+        result = values + 1j * uncertainties
+        return result
+
+unumpy_array = unp.uarray([1, 2, 3], [0.1, 0.2, 0.3])
+
+# Convert to two-dimensional column array
+result = unp_to_np(unumpy_array)
+print(result)
```

