# Comparing `tmp/napari-toothfairy-annotator-0.0.6.tar.gz` & `tmp/napari-toothfairy-annotator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-toothfairy-annotator-0.0.6.tar", last modified: Fri Apr  5 14:32:39 2024, max compression
+gzip compressed data, was "napari-toothfairy-annotator-0.0.7.tar", last modified: Mon Apr  8 08:18:00 2024, max compression
```

## Comparing `napari-toothfairy-annotator-0.0.6.tar` & `napari-toothfairy-annotator-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 14:32:39.822719 napari-toothfairy-annotator-0.0.6/
--rw-rw-rw-   0        0        0     1102 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-02 09:17:13.000000 napari-toothfairy-annotator-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4716 2024-04-05 14:32:39.822719 napari-toothfairy-annotator-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2968 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.6/README.md
--rw-rw-rw-   0        0        0     1233 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     1927 2024-04-05 14:32:39.824719 napari-toothfairy-annotator-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 14:32:39.794387 napari-toothfairy-annotator-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 14:32:39.805518 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/
--rw-rw-rw-   0        0        0     9832 2024-04-05 14:25:52.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/FDI_Annotator.py
--rw-rw-rw-   0        0        0      335 2024-04-05 14:30:15.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/__init__.py
--rw-rw-rw-   0        0        0      812 2024-03-27 10:15:18.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:32:39.819721 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/
--rw-rw-rw-   0        0        0        0 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/__init__.py
--rw-rw-rw-   0        0        0     1020 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/test_reader.py
--rw-rw-rw-   0        0        0     2284 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/test_widget.py
--rw-rw-rw-   0        0        0      143 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/test_writer.py
--rw-rw-rw-   0        0        0    13283 2024-04-03 15:21:58.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_widget.py
--rw-rw-rw-   0        0        0     1998 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_writer.py
--rw-rw-rw-   0        0        0     1514 2024-04-02 09:06:47.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-04-05 14:32:39.820722 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/
--rw-rw-rw-   0        0        0     4716 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      865 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 08:18:00.881641 napari-toothfairy-annotator-0.0.7/
+-rw-rw-rw-   0        0        0     1102 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-02 09:17:13.000000 napari-toothfairy-annotator-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4716 2024-04-08 08:18:00.881641 napari-toothfairy-annotator-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2968 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1233 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2024-04-08 08:18:00.890376 napari-toothfairy-annotator-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 08:18:00.802655 napari-toothfairy-annotator-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 08:18:00.833107 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/
+-rw-rw-rw-   0        0        0    10082 2024-04-08 07:55:49.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/FDI_Annotator.py
+-rw-rw-rw-   0        0        0      335 2024-04-08 08:17:15.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/__init__.py
+-rw-rw-rw-   0        0        0      812 2024-03-27 10:15:18.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-08 08:18:00.877581 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/
+-rw-rw-rw-   0        0        0        0 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/test_reader.py
+-rw-rw-rw-   0        0        0     2284 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/test_widget.py
+-rw-rw-rw-   0        0        0      143 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/test_writer.py
+-rw-rw-rw-   0        0        0    14237 2024-04-08 08:13:35.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_widget.py
+-rw-rw-rw-   0        0        0     1998 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_writer.py
+-rw-rw-rw-   0        0        0     1514 2024-04-02 09:06:47.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-04-08 08:18:00.879580 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/
+-rw-rw-rw-   0        0        0     4716 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      865 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-08 08:18:00.000000 napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/top_level.txt
```

### Comparing `napari-toothfairy-annotator-0.0.6/LICENSE` & `napari-toothfairy-annotator-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.6/PKG-INFO` & `napari-toothfairy-annotator-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-toothfairy-annotator
-Version: 0.0.6
+Version: 0.0.7
 Summary: The plugin employed to annotate volumes employed in the ToothFairy 2 Challenge
 Home-page: https://github.com/LucaLumetti/napari-toothfairy-annotator
 Author: Luca Lumetti
 Author-email: lumetti.luca@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LucaLumetti/napari-toothfairy-annotator/issues
 Project-URL: Documentation, https://github.com/LucaLumetti/napari-toothfairy-annotator#README.md
```

### Comparing `napari-toothfairy-annotator-0.0.6/README.md` & `napari-toothfairy-annotator-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.6/pyproject.toml` & `napari-toothfairy-annotator-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.6/setup.cfg` & `napari-toothfairy-annotator-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/FDI_Annotator.py` & `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/FDI_Annotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,17 @@
             "01": {"quadrant": 0, "ID": "01", "type": "Lower Jawbone", "name": "Lower Jawbone"},
             "02": {"quadrant": 0, "ID": "02", "type": "Upper Jawbone", "name": "Upper Jawbone"},
             "03": {"quadrant": 0, "ID": "03", "type": "Left Inferior Alveolar Canal", "name": "Left Inferior Alveolar Canal"},
             "04": {"quadrant": 0, "ID": "04", "type": "Right Inferior Alveolar Canal", "name": "Right Inferior Alveolar Canal"},
             "05": {"quadrant": 0, "ID": "05", "type": "Left Maxillary Sinus", "name": "Left Maxillary Sinus"},
             "06": {"quadrant": 0, "ID": "06", "type": "Right Maxillary Sinus", "name": "Right Maxillary Sinus"},
             "07": {"quadrant": 0, "ID": "07", "type": "Pharynx", "name": "Pharynx"},
-
+            "08": {"quadrant": 0, "ID": "08", "type": "Bridge", "name": "Bridge"},
+            "09": {"quadrant": 0, "ID": "09", "type": "Crown", "name": "Crown"},
+            "10": {"quadrant": 0, "ID": "10", "type": "Implant", "name": "Implant"},
             "11": {"quadrant": 1, "ID": "11", "type": "Incisor", "name": "Upper Right Central Incisor"},
             "12": {"quadrant": 1, "ID": "12", "type": "Incisor", "name": "Upper Right Lateral Incisor"},
             "13": {"quadrant": 1, "ID": "13", "type": "Canine", "name": "Upper Right Canine"},
             "14": {"quadrant": 1, "ID": "14", "type": "Premolar", "name": "Upper Right First Premolar"},
             "15": {"quadrant": 1, "ID": "15", "type": "Premolar", "name": "Upper Right Second Premolar"},
             "16": {"quadrant": 1, "ID": "16", "type": "Molar", "name": "Upper Right First Molar"},
             "17": {"quadrant": 1, "ID": "17", "type": "Molar", "name": "Upper Right Second Molar"},
```

### Comparing `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_reader.py` & `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/test_reader.py` & `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/test_widget.py` & `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_widget.py` & `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,14 +79,18 @@
             QAbstractItemView.ExtendedSelection
         )
 
         self.associate_button = QPushButton("Associate IDs")
         self.associate_button.clicked.connect(self.associate_ids)
         layout.addWidget(self.associate_button)
 
+        self.reset_assoc_button = QPushButton("Reset Association")
+        self.reset_assoc_button.clicked.connect(self.reset_assoc)
+        layout.addWidget(self.reset_assoc_button)
+
         self.reload_button = QPushButton("Reload")
         self.reload_button.clicked.connect(self.reload)
         layout.addWidget(self.reload_button)
 
         self.setLayout(layout)
         self.load_associations()
         self.update_lists()
@@ -134,14 +138,38 @@
                 self.viewer.layers['annotation'].data[mask] = 0
                 self.viewer.layers['associated'].data[mask] = int(fdi_id)
         self.viewer.layers['annotation'].refresh()
         self.viewer.layers['associated'].refresh()
         self.update_lists()
         self.save()
 
+    def reset_assoc(self,):
+        selected_items_list2 = self.list2.selectedItems()
+
+        for item2 in selected_items_list2:
+            item2 = item2.text()
+            print(f"selected: {item2}")
+            if ' > ' not in item2:
+                continue
+            id = item2.split(' > ')[0]
+            id = int(id)
+            assoc_id = self.associations[id]
+
+            print(f"removing {id} > {assoc_id}")
+
+            del self.associations[id]
+
+            mask = self.viewer.layers['associated'].data == int(assoc_id)
+            self.viewer.layers['associated'].data[mask] = 0
+            self.viewer.layers['annotation'].data[mask] = id
+        self.viewer.layers['annotation'].refresh()
+        self.viewer.layers['associated'].refresh()
+        self.update_lists()
+        self.save()
+
     def get_source(self,):
         source = self.viewer.layers['annotation'].source.path
         if source is None:
             source = self.viewer.layers['volume'].source.path
         if source is None:
             source = self.viewer.layers['annotation'].metadata['parent_folder']
         if source is None:
@@ -184,26 +212,26 @@
 
 
     def update_lists(self):
         self.list1.clear()
         self.list2.clear()
 
         for id_data in self.get_fdi_ids():
-            item = ColorWidgetItem(id_data['name'], QColor("white"))
+            item = id_data['name']
             self.list1.addItem(item)
 
         already_annotated = set(self.associations.keys())
         print(f'already_annotated: {already_annotated}')
 
         for id_data in self.get_available_ids():
             s = f'{id_data}'
             if int(id_data) in already_annotated:
                 assoc_id = self.associations[int(id_data)]
                 s += f' > {self.fdi_annotator.fdi_notation[assoc_id]["name"]}'
-            item = ColorWidgetItem(s, QColor("red"))
+            item = s
             self.list2.addItem(item)
 
     def get_available_ids(self,):
         if self._available_ids is None:
             data = self.viewer.layers['annotation'].data
             self._available_ids = np.unique(data).tolist()
             self._available_ids += self.associations.keys()
```

### Comparing `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_writer.py` & `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/napari.yaml` & `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/PKG-INFO` & `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-toothfairy-annotator
-Version: 0.0.6
+Version: 0.0.7
 Summary: The plugin employed to annotate volumes employed in the ToothFairy 2 Challenge
 Home-page: https://github.com/LucaLumetti/napari-toothfairy-annotator
 Author: Luca Lumetti
 Author-email: lumetti.luca@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LucaLumetti/napari-toothfairy-annotator/issues
 Project-URL: Documentation, https://github.com/LucaLumetti/napari-toothfairy-annotator#README.md
```

### Comparing `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/SOURCES.txt` & `napari-toothfairy-annotator-0.0.7/src/napari_toothfairy_annotator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

