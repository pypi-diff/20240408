# Comparing `tmp/metaspread-2024.0.1.tar.gz` & `tmp/metaspread-2024.0.2.tar.gz`

## Comparing `metaspread-2024.0.1.tar` & `metaspread-2024.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 metaspread-2024.0.1/requirements.txt
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/__init__.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/__main__.py
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/cancercell.py
--rw-r--r--   0        0        0    30554 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/cancermodel.py
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/configs.py
--rw-r--r--   0        0        0    15717 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/datagenerator.py
--rw-r--r--   0        0        0    19494 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/graphgenerator.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/interactive.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/quasicircle.py
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/simrunner.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/vessel.py
--rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 metaspread-2024.0.1/metaspread/videogenerator.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 metaspread-2024.0.1/.gitignore
--rw-r--r--   0        0        0    35184 2020-02-02 00:00:00.000000 metaspread-2024.0.1/LICENSE.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 metaspread-2024.0.1/README.md
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 metaspread-2024.0.1/pyproject.toml
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 metaspread-2024.0.1/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 metaspread-2024.0.2/requirements.txt
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/__init__.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/__main__.py
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/cancercell.py
+-rw-r--r--   0        0        0    30554 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/cancermodel.py
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/configs.py
+-rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/datagenerator.py
+-rw-r--r--   0        0        0    19481 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/graphgenerator.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/interactive.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/quasicircle.py
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/simrunner.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/vessel.py
+-rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 metaspread-2024.0.2/metaspread/videogenerator.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 metaspread-2024.0.2/.gitignore
+-rw-r--r--   0        0        0    35184 2020-02-02 00:00:00.000000 metaspread-2024.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 metaspread-2024.0.2/README.md
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 metaspread-2024.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 metaspread-2024.0.2/PKG-INFO
```

### Comparing `metaspread-2024.0.1/metaspread/__main__.py` & `metaspread-2024.0.2/metaspread/__main__.py`

 * *Files identical despite different names*

### Comparing `metaspread-2024.0.1/metaspread/cancercell.py` & `metaspread-2024.0.2/metaspread/cancercell.py`

 * *Files identical despite different names*

### Comparing `metaspread-2024.0.1/metaspread/cancermodel.py` & `metaspread-2024.0.2/metaspread/cancermodel.py`

 * *Files identical despite different names*

### Comparing `metaspread-2024.0.1/metaspread/configs.py` & `metaspread-2024.0.2/metaspread/configs.py`

 * *Files identical despite different names*

### Comparing `metaspread-2024.0.1/metaspread/datagenerator.py` & `metaspread-2024.0.2/metaspread/datagenerator.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,25 +41,37 @@
         df_export.to_csv(path)
 
     #create histogram of positions
     path = os.path.join(tumor_data_path, f'Cells-grid{grid_id}-step{step} - Histogram at {real_time_at_step/(3600*24):.2f} days.csv')
     if not os.path.isfile(path):
         if coords_list:
             Xm, Ym, Xe, Ye, Xv, Yv, Xvr, Yvr = coords_list[0], coords_list[1], coords_list[2], coords_list[3], coords_list[4], coords_list[5], coords_list[6], coords_list[7]
+        else:
+            coords_list = read_coords_for_plot(step, all_cells_dataframe, grid_id)
+            Xm, Ym, Xe, Ye, Xv, Yv, Xvr, Yvr = coords_list[0], coords_list[1], coords_list[2], coords_list[3], coords_list[4], coords_list[5], coords_list[6], coords_list[7]
         df_positions = pd.DataFrame({'Position': zip(Xm + Xe, Ym + Ye)})
         position_repetition_count = df_positions['Position'].value_counts()
         histogram = position_repetition_count.value_counts()
         histogram = pd.DataFrame({'Bins': histogram.index, 'Frequency': histogram.values})
         number_of_empty_positions = metaspread.configs.gridsize * metaspread.configs.gridsize - len(position_repetition_count)
         new_row = pd.DataFrame({'Bins': [0], 'Frequency': [number_of_empty_positions]})
         histogram = pd.concat([histogram, new_row])
         histogram.to_csv(path)
-        return
+        # return
         #this will return the radius and diameter of the processed tumor
         return get_cluster_centroid_radius_and_diameter(df_positions, grid_id)
+    path = os.path.join(tumor_data_path, "Tumor radius and diameter history in grid 1.csv")
+    if not os.path.isfile(path):
+        if coords_list:
+            Xm, Ym, Xe, Ye, Xv, Yv, Xvr, Yvr = coords_list[0], coords_list[1], coords_list[2], coords_list[3], coords_list[4], coords_list[5], coords_list[6], coords_list[7]
+        else:
+            coords_list = read_coords_for_plot(step, all_cells_dataframe, grid_id)
+            Xm, Ym, Xe, Ye, Xv, Yv, Xvr, Yvr = coords_list[0], coords_list[1], coords_list[2], coords_list[3], coords_list[4], coords_list[5], coords_list[6], coords_list[7]
+        df_positions = pd.DataFrame({'Position': zip(Xm + Xe, Ym + Ye)})
+        return get_cluster_centroid_radius_and_diameter(df_positions, grid_id)
     return ([np.nan, np.nan], np.nan, np.nan)
     
 def save_growth_data(all_cells_dataframe, grid_id, cells_data_path, step_number, real_time_at_step, real_delta_time, df_csv_last_step):
     path_to_save = os.path.join(cells_data_path, f'CellsGrowth-grid{grid_id}-step{step_number} - {real_time_at_step/(3600*24):.2f} days.csv')
     if os.path.isfile(path_to_save):
         return pd.DataFrame()
     df = all_cells_dataframe.loc[(all_cells_dataframe["Grid"] == grid_id) & (all_cells_dataframe["Step"] == step_number)]
@@ -172,28 +184,28 @@
     print("Saving cells numbers data in the folder:", cells_data_path)
     print("Saving vasculature data in the folder:", vasculature_data_path)
     
     for grid_id in range(1, grids_number+1):
         print(f'\nGrid: {grid_id}')
 
         print(f'\tSaving tumor data...')
-        # df_radius_diameter_history = pd.DataFrame(columns=['Centroid x', 'Centroid y', 'Radius', 'Diameter', 'Step', 'Grid Id'])
+        df_radius_diameter_history = pd.DataFrame(columns=['Centroid x', 'Centroid y', 'Radius', 'Diameter', 'Step', 'Grid Id'])
         for id, step in enumerate(range(step_size,max_step+1,step_size)):
             real_time_at_step = real_delta_time * step
             if grid_id == 1:
-                save_cancer(all_cells_dataframe, grid_id, step, real_time_at_step, tumor_data_path)
-                # (centroid, radius, diameter) = save_cancer(all_cells_dataframe, grid_id, step, real_time_at_step, tumor_data_path)
-                # new_row = pd.DataFrame({'Centroid x': [centroid[0]], 'Centroid y': [centroid[1]],'Radius': [radius], 'Diameter': [diameter], 'Step': [step], 'Grid Id': [grid_id]})
-                # df_radius_diameter_history = pd.concat([df_radius_diameter_history, new_row])
+                # save_cancer(all_cells_dataframe, grid_id, step, real_time_at_step, tumor_data_path)
+                (centroid, radius, diameter) = save_cancer(all_cells_dataframe, grid_id, step, real_time_at_step, tumor_data_path)
+                new_row = pd.DataFrame({'Centroid x': [centroid[0]], 'Centroid y': [centroid[1]],'Radius': [radius], 'Diameter': [diameter], 'Step': [step], 'Grid Id': [grid_id]})
+                df_radius_diameter_history = pd.concat([df_radius_diameter_history, new_row])
             else:
                 save_cancer(all_cells_dataframe, grid_id, step, real_time_at_step, tumor_data_path)
-        # if grid_id == 1:
-        #     path = os.path.join(tumor_data_path, f'Tumor radius and diameter history in grid {grid_id}.csv')
-        #     if not os.path.isfile(path):
-        #         df_radius_diameter_history.to_csv(path)
+        if grid_id == 1:
+            path = os.path.join(tumor_data_path, f'Tumor radius and diameter history in grid {grid_id}.csv')
+            if not os.path.isfile(path):
+                df_radius_diameter_history.to_csv(path)
 
         print(f'\tSaving cells numbers graph data...')
         df_csv_last_step = pd.DataFrame()
         for id, step in enumerate(range(step_size,max_step+1,step_size)):
             real_time_at_step = real_delta_time * step
             df_csv_last_step = save_growth_data(all_cells_dataframe, grid_id , cells_data_path, step, real_time_at_step, real_delta_time, df_csv_last_step)
```

### Comparing `metaspread-2024.0.1/metaspread/graphgenerator.py` & `metaspread-2024.0.2/metaspread/graphgenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     path_to_save = os.path.join(all_histogram_images_path, f"Cells-grid{grid_id}-step{step} - Histogram at {real_time_at_step/(3600*24):.2f} days.png")
     if os.path.isfile(path_to_save):
         return
     histogram = pd.read_csv(histogram_csv_file_path, header=0, index_col=0)
     if histogram.empty:
         return
     plt.xlabel('Number of cells per grid-point')
-    plt.ylabel('Nr. grid-points with\na given nr. of cells')
+    plt.ylabel('\nNr. grid-points with given nr. of cells')
     plt.title(f'Positions histogram at {real_time_at_step/(3600*24):.2f} days ({step} steps) - grid {grid_id}', fontsize = 13)
     plt.bar(histogram['Bins'], histogram['Frequency'])
     plt.xticks(range(metaspread.configs.carrying_capacity + 1))
     plt.xlim([-1, metaspread.configs.carrying_capacity + 1])
     plt.savefig(path_to_save)
 
 def plot_vasculature_graphs(vasculature_df, path_to_save, max_step, real_delta_time):
@@ -374,21 +374,21 @@
             os._exit(1)
         plot_vasculature_graphs(vasculature_data, vasculature_images_path, step, real_delta_time)
         plt.close()
         fig_counter += 1
         
     #plotting the radius and diameter history graph
     print(f'Plotting radius and diameter history graph...')
-    # folder_path = os.path.join(simulation_path, "Data analysis", "Tumor dynamics")
-    # file_name = [file for file in os.listdir(folder_path) if file.startswith("Tumor radius and diameter history")][0]
-    # file_path = os.path.join(folder_path, file_name)
-    # radius_history_df = pd.read_csv(file_path)#, header=0)
-    # plot_radius_diameter_history(radius_history_df, radius_diameter_images_path, step, real_delta_time)
+    folder_path = os.path.join(simulation_path, "Data analysis", "Tumor dynamics")
+    file_name = [file for file in os.listdir(folder_path) if file.startswith("Tumor radius and diameter history")][0]
+    file_path = os.path.join(folder_path, file_name)
+    radius_history_df = pd.read_csv(file_path)#, header=0)
+    plot_radius_diameter_history(radius_history_df, radius_diameter_images_path, step, real_delta_time)
     plt.close()
-    # fig_counter += 1
+    fig_counter += 1
 
     plt.show()
     plt.close()
 
     plt.show()
     plt.close()
```

### Comparing `metaspread-2024.0.1/metaspread/interactive.py` & `metaspread-2024.0.2/metaspread/interactive.py`

 * *Files identical despite different names*

### Comparing `metaspread-2024.0.1/metaspread/quasicircle.py` & `metaspread-2024.0.2/metaspread/quasicircle.py`

 * *Files identical despite different names*

### Comparing `metaspread-2024.0.1/metaspread/simrunner.py` & `metaspread-2024.0.2/metaspread/simrunner.py`

 * *Files identical despite different names*

### Comparing `metaspread-2024.0.1/metaspread/videogenerator.py` & `metaspread-2024.0.2/metaspread/videogenerator.py`

 * *Files identical despite different names*

### Comparing `metaspread-2024.0.1/LICENSE.txt` & `metaspread-2024.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `metaspread-2024.0.1/pyproject.toml` & `metaspread-2024.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metaspread"
-version = "2024.0.1"
+version = "2024.0.2"
 authors = [
   { name="Alfredo Hernández-Inostroza", email="alfredo.hernandez@ug.uchile.cl" },
 ]
 description = "A cancer and metastasis simulation package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

