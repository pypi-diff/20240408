# Comparing `tmp/napari-toothfairy-annotator-0.0.7.tar.gz` & `tmp/napari-toothfairy-annotator-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-toothfairy-annotator-0.0.7.tar", last modified: Mon Apr  8 08:18:00 2024, max compression
+gzip compressed data, was "napari-toothfairy-annotator-0.0.8.tar", last modified: Mon Apr  8 08:43:04 2024, max compression
```

## Comparing `napari-toothfairy-annotator-0.0.7.tar` & `napari-toothfairy-annotator-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 08:18:00.881641 napari-toothfairy-annotator-0.0.7/
--rw-rw-rw-   0        0        0     1102 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-02 09:17:13.000000 napari-toothfairy-annotator-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4716 2024-04-08 08:18:00.881641 napari-toothfairy-annotator-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2968 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.7/README.md
--rw-rw-rw-   0        0        0     1233 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0     1927 2024-04-08 08:18:00.890376 napari-toothfairy-annotator-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-08 08:18:00.802655 napari-toothfairy-annotator-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 08:18:00.833107 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/
--rw-rw-rw-   0        0        0    10082 2024-04-08 07:55:49.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/FDI_Annotator.py
--rw-rw-rw-   0        0        0      335 2024-04-08 08:17:15.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/__init__.py
--rw-rw-rw-   0        0        0      812 2024-03-27 10:15:18.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-08 08:18:00.877581 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/
--rw-rw-rw-   0        0        0        0 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/__init__.py
--rw-rw-rw-   0        0        0     1020 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/test_reader.py
--rw-rw-rw-   0        0        0     2284 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/test_widget.py
--rw-rw-rw-   0        0        0      143 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/test_writer.py
--rw-rw-rw-   0        0        0    14237 2024-04-08 08:13:35.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_widget.py
--rw-rw-rw-   0        0        0     1998 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_writer.py
--rw-rw-rw-   0        0        0     1514 2024-04-02 09:06:47.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-04-08 08:18:00.879580 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/
--rw-rw-rw-   0        0        0     4716 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      865 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 08:43:04.300583 napari-toothfairy-annotator-0.0.8/
+-rw-rw-rw-   0        0        0     1102 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-02 09:17:13.000000 napari-toothfairy-annotator-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4716 2024-04-08 08:43:04.300583 napari-toothfairy-annotator-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2968 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1233 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2024-04-08 08:43:04.307764 napari-toothfairy-annotator-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 08:43:04.261053 napari-toothfairy-annotator-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 08:43:04.274297 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/
+-rw-rw-rw-   0        0        0    10082 2024-04-08 07:55:49.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/FDI_Annotator.py
+-rw-rw-rw-   0        0        0      335 2024-04-08 08:42:45.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/__init__.py
+-rw-rw-rw-   0        0        0      812 2024-03-27 10:15:18.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-08 08:43:04.297584 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_tests/
+-rw-rw-rw-   0        0        0        0 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_tests/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_tests/test_reader.py
+-rw-rw-rw-   0        0        0     2284 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_tests/test_widget.py
+-rw-rw-rw-   0        0        0      143 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_tests/test_writer.py
+-rw-rw-rw-   0        0        0    14168 2024-04-08 08:42:40.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_widget.py
+-rw-rw-rw-   0        0        0     1998 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_writer.py
+-rw-rw-rw-   0        0        0     1514 2024-04-02 09:06:47.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-04-08 08:43:04.298583 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator.egg-info/
+-rw-rw-rw-   0        0        0     4716 2024-04-08 08:43:04.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      865 2024-04-08 08:43:04.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 08:43:04.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-08 08:43:04.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2024-04-08 08:43:04.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-08 08:43:04.000000 napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator.egg-info/top_level.txt
```

### Comparing `napari-toothfairy-annotator-0.0.7/LICENSE` & `napari-toothfairy-annotator-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.7/PKG-INFO` & `napari-toothfairy-annotator-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-toothfairy-annotator
-Version: 0.0.7
+Version: 0.0.8
 Summary: The plugin employed to annotate volumes employed in the ToothFairy 2 Challenge
 Home-page: https://github.com/LucaLumetti/napari-toothfairy-annotator
 Author: Luca Lumetti
 Author-email: lumetti.luca@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LucaLumetti/napari-toothfairy-annotator/issues
 Project-URL: Documentation, https://github.com/LucaLumetti/napari-toothfairy-annotator#README.md
```

### Comparing `napari-toothfairy-annotator-0.0.7/README.md` & `napari-toothfairy-annotator-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.7/pyproject.toml` & `napari-toothfairy-annotator-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.7/setup.cfg` & `napari-toothfairy-annotator-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/FDI_Annotator.py` & `napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/FDI_Annotator.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_reader.py` & `napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/test_reader.py` & `napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/test_widget.py` & `napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_widget.py` & `napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,20 +64,24 @@
 
         self.load_associated_volume()
 
         self.viewer.layers.move_multiple([0,2,1])
 
         layout = QVBoxLayout()
 
+        self.list1_label = QLabel('Nominal IDs:')
         self.list1 = QListWidget()
         # self.list1.setSortingEnabled(True)
+        layout.addWidget(self.list1_label)
         layout.addWidget(self.list1)
 
+        self.list2_label = QLabel('Numerical IDs:')
         self.list2 = QListWidget()
         self.list2.setSortingEnabled(True)
+        layout.addWidget(self.list2_label)
         layout.addWidget(self.list2)
         self.list2.setSelectionMode(
             QAbstractItemView.ExtendedSelection
         )
 
         self.associate_button = QPushButton("Associate IDs")
         self.associate_button.clicked.connect(self.associate_ids)
@@ -143,32 +147,31 @@
         self.save()
 
     def reset_assoc(self,):
         selected_items_list2 = self.list2.selectedItems()
 
         for item2 in selected_items_list2:
             item2 = item2.text()
-            print(f"selected: {item2}")
+
             if ' > ' not in item2:
                 continue
+
+            print(f"selected: {item2}")
+            
             id = item2.split(' > ')[0]
             id = int(id)
             assoc_id = self.associations[id]
 
             print(f"removing {id} > {assoc_id}")
 
             del self.associations[id]
 
-            mask = self.viewer.layers['associated'].data == int(assoc_id)
-            self.viewer.layers['associated'].data[mask] = 0
-            self.viewer.layers['annotation'].data[mask] = id
-        self.viewer.layers['annotation'].refresh()
-        self.viewer.layers['associated'].refresh()
         self.update_lists()
         self.save()
+        self.reload()
 
     def get_source(self,):
         source = self.viewer.layers['annotation'].source.path
         if source is None:
             source = self.viewer.layers['volume'].source.path
         if source is None:
             source = self.viewer.layers['annotation'].metadata['parent_folder']
```

### Comparing `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_writer.py` & `napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/napari.yaml` & `napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/PKG-INFO` & `napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-toothfairy-annotator
-Version: 0.0.7
+Version: 0.0.8
 Summary: The plugin employed to annotate volumes employed in the ToothFairy 2 Challenge
 Home-page: https://github.com/LucaLumetti/napari-toothfairy-annotator
 Author: Luca Lumetti
 Author-email: lumetti.luca@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LucaLumetti/napari-toothfairy-annotator/issues
 Project-URL: Documentation, https://github.com/LucaLumetti/napari-toothfairy-annotator#README.md
```

### Comparing `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/SOURCES.txt` & `napari-toothfairy-annotator-0.0.8/src/napari_toothfairy_annotator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

