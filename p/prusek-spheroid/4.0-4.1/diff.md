# Comparing `tmp/prusek_spheroid-4.0.tar.gz` & `tmp/prusek_spheroid-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-4.0.tar", last modified: Fri Apr  5 06:03:13 2024, max compression
+gzip compressed data, was "prusek_spheroid-4.1.tar", last modified: Mon Apr  8 11:03:24 2024, max compression
```

## Comparing `prusek_spheroid-4.0.tar` & `prusek_spheroid-4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-05 06:03:13.254990 prusek_spheroid-4.0/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9094 2024-04-05 06:03:13.254774 prusek_spheroid-4.0/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-4.0/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-05 06:03:13.253121 prusek_spheroid-4.0/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    18167 2024-04-05 05:41:53.000000 prusek_spheroid-4.0/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    50417 2024-04-04 18:36:20.000000 prusek_spheroid-4.0/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-4.0/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-4.0/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-4.0/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-4.0/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     6737 2024-04-04 14:40:14.000000 prusek_spheroid-4.0/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2555 2024-04-04 18:44:25.000000 prusek_spheroid-4.0/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3641 2024-04-03 14:52:18.000000 prusek_spheroid-4.0/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-4.0/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-4.0/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-05 06:03:13.254498 prusek_spheroid-4.0/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9094 2024-04-05 06:03:13.000000 prusek_spheroid-4.0/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-05 06:03:13.000000 prusek_spheroid-4.0/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-05 06:03:13.000000 prusek_spheroid-4.0/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      120 2024-04-05 06:03:13.000000 prusek_spheroid-4.0/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-05 06:03:13.000000 prusek_spheroid-4.0/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-05 06:03:13.255068 prusek_spheroid-4.0/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      750 2024-04-05 06:03:10.000000 prusek_spheroid-4.0/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-08 11:03:24.037141 prusek_spheroid-4.1/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-08 11:03:24.036776 prusek_spheroid-4.1/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-4.1/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-08 11:03:24.035056 prusek_spheroid-4.1/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    18501 2024-04-07 11:22:36.000000 prusek_spheroid-4.1/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    50417 2024-04-04 18:36:20.000000 prusek_spheroid-4.1/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12428 2024-04-06 18:03:18.000000 prusek_spheroid-4.1/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-4.1/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-4.1/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-4.1/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-4.1/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-4.1/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-4.1/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-4.1/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-4.1/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-08 11:03:24.036453 prusek_spheroid-4.1/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-08 11:03:24.000000 prusek_spheroid-4.1/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-08 11:03:24.000000 prusek_spheroid-4.1/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-08 11:03:24.000000 prusek_spheroid-4.1/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-08 11:03:24.000000 prusek_spheroid-4.1/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-08 11:03:24.000000 prusek_spheroid-4.1/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-08 11:03:24.037202 prusek_spheroid-4.1/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-08 11:03:20.000000 prusek_spheroid-4.1/setup.py
```

### Comparing `prusek_spheroid-4.0/PKG-INFO` & `prusek_spheroid-4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 4.0
+Version: 4.1
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
@@ -14,14 +14,15 @@
 Requires-Dist: threadpoolctl
 Requires-Dist: matplotlib
 Requires-Dist: rasterio
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 Requires-Dist: torch
 Requires-Dist: imagehash
+Requires-Dist: joblib
 
 # Prusek-Spheroid
 
 Prusek-Spheroid is a Python package designed for spheroid segmentation based on provided microscope images. This package provides an easy-to-use interface and functionalities that are essential for determination of properties and characteristics of the spheroids.
 
 ## Installation
```

### Comparing `prusek_spheroid-4.0/README.md` & `prusek_spheroid-4.1/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.0/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-4.1/prusek_spheroid/ContoursClassGUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 import pandas as pd
 from prusek_spheroid import file_management as fm
 from prusek_spheroid import selection_dialog as sd
 from prusek_spheroid import metrics as metric
 from prusek_spheroid.methods import BaseImageProcessing
 from prusek_spheroid import characteristic_functions as cf
 from prusek_spheroid import image_processing as ip
+import joblib
 
 
 class Contours(BaseImageProcessing):
 
     def __init__(self, master, adresaDatasetu, adresa_output, projekt, algorithm, parameters, show_img, function,
                  contours_state, detect_corrupted, create_json, calculate_properties,
                  progress_window=None):
         super().__init__()
+        self.counter = None
         self.master = master
         self.user_decision_lock = Lock()
         self.adresaDatasetu = adresaDatasetu
         self.output_json_path = f"{adresa_output}/{projekt}/CVAT/{algorithm}/annotations/instances_default.json"
         self.output_images_path = f"{adresa_output}/{projekt}/CVAT/{algorithm}/images"
         self.output_segmented_path = f"{adresa_output}/{projekt}/segmented_images/{algorithm}"
         self.zipfile_address = f"{adresa_output}/{projekt}/CVAT/{algorithm}"
@@ -35,28 +37,37 @@
         self.contours_state = contours_state
         self.detect_corrupted = detect_corrupted
         self.create_json = create_json
         self.calculate_properties = calculate_properties
         self.f = function
         self.progress_window = progress_window
         self.min_area = self.parameters["min_area"]
+        self.model = joblib.load("gradient_boosting_classifier.joblib")
+        self.scaler = joblib.load("scaler.joblib")
 
         fm.create_directory(os.path.dirname(self.output_json_path), delete=True)
         fm.create_directory(self.output_images_path, delete=True)
         fm.create_directory(f"{self.output_segmented_path}/masks", delete=True)
         fm.create_directory(f"{self.output_segmented_path}/results", delete=True)
 
+    def evaluate(self, contour):
+        hu_moments = ip.compute_hu_moments(contour)
+        hu_moments_scaled = self.scaler.transform([hu_moments])
+        contour_class = self.model.predict(hu_moments_scaled)[0]
+        return contour_class
+
     def run(self):
         dialog = None
-        all_contour_data = []
-        filenames = os.listdir(self.adresaDatasetu)
+        self.counter = 1
+        filenames = [f for f in os.listdir(self.adresaDatasetu) if
+                     f.lower().endswith(('.png', '.jpg', '.jpeg', '.bmp', '.tiff', '.tif'))]
         total_files = len(filenames)
         print(f"loaded {total_files} dataset images")
-        self.counter = 1
 
+        all_contour_data = []
         if self.contours_state == "select":
             dialog = sd.SelectionDialog(self.master, self.counter, total_files, self.user_decision_lock)
 
         for filename in os.listdir(self.adresaDatasetu):
             if filename.lower().endswith(('.png', '.jpg', '.jpeg', '.bmp', '.tiff', '.tif')):
                 if self.contours_state == "select":
                     self.user_decision_lock.acquire()
@@ -65,99 +76,119 @@
                 img = cv.imread(img_path)
 
                 if img is None:
                     print(f"FAILED to load image: {img_path}")
                     continue  # Skip to the next image
 
                 img_gray = cv.cvtColor(img, cv.COLOR_BGR2GRAY)
+                img_gray = cv.resize(img_gray, (1000, 1000), interpolation=cv.INTER_LANCZOS4)
 
                 img_binary, inner_contours_mask = self.apply_segmentation_algorithm(self.algorithm, self.parameters,
                                                                                     img_gray,
-                                                                                    self.contours_state,
-                                                                                    self.detect_corrupted)
-
+                                                                                    self.contours_state)
 
+                outer_contours, _ = cv.findContours(img_binary, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
                 if self.contours_state == "all" or self.contours_state == "select":
-                    intersection = inner_contours_mask & img_binary
-                    img_binary = img_binary - intersection
-
-                contours, hierarchy = cv.findContours(img_binary, cv.RETR_TREE, cv.CHAIN_APPROX_SIMPLE)
+                    inner_contours, _ = cv.findContours(inner_contours_mask, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
+                    inner_contours = ip.remove_small_contours(inner_contours)
 
                 height, width = np.shape(img_binary)
 
-                contours, hierarchy = ip.filter_contours_on_frame(contours, hierarchy, (height, width), self.min_area, self.detect_corrupted)
+                outer_contours = ip.filter_contours_on_frame(outer_contours, (height, width), self.min_area,
+                                                                  self.detect_corrupted)
+                outer_contours = ip.remove_small_contours(outer_contours)
+
 
                 if self.create_json:
                     if not cv.imwrite(f"{self.output_images_path}/{filename}", img):
                         print(f"FAILED to save image: {self.output_images_path}/{filename}")
 
                 img_with = img.copy()
-                if not contours:
+                if len(outer_contours) == 0:
                     if self.create_json:
                         self.coco_data = fm.convert_contours_to_coco([], [], height, width,
                                                                      filename,
                                                                      self.counter,
                                                                      self.coco_data)
                     cv.line(img_with, (0, 0), (width - 1, height - 1), (0, 0, 255), 5)
                     cv.line(img_with, (0, height - 1), (width - 1, 0), (0, 0, 255), 5)
-                    cv.line(img_without, (0, 0), (width - 1, height - 1), (0, 0, 255), 5)
-                    cv.line(img_without, (0, height - 1), (width - 1, 0), (0, 0, 255), 5)
-                else:
+                    if not cv.imwrite(
+                            f"{self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}",
+                            img_with):
+                        print(
+                            f"FAILED to save image: {self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}")
 
-                    inner_contours = []
-                    outer_contours = []
+                else:
                     img_without = img.copy()
-                    if self.contours_state == "all" or self.contours_state == "select":
-
-                        for i, contour in enumerate(contours):
-                            # Získání indexu rodiče pro aktuální konturu
-                            parent_index = hierarchy[0, i, 3]  # Correctly access the parent index
-                            if parent_index == -1:
-                                # Kontura bez rodiče - vnější kontura
-                                cv.drawContours(img_with, [contour], -1, (0, 0, 255), 2)  # Červeně pro vnější kontury
-                                outer_contours.append(contour)
-                            else:
-                                # Kontrola, zda má rodič této kontury také rodiče (kontury druhého řádu)
-                                grandparent_index = hierarchy[0][parent_index][3]
-
-                                if grandparent_index == -1:
-                                    # Kontura s jedním předkem - vnitřní kontura
-                                    cv.drawContours(img_with, [contour], -1, (255, 0, 0),
-                                                    2)  # Modře pro vnitřní kontury
-                                    inner_contours.append(contour)
+                    mask_without = np.zeros_like(img_gray)
 
-                    if len(outer_contours) == 0:
-                        outer_contours = contours
+                    for contour in outer_contours:
+                        contour = np.array(contour, dtype=np.int32)
+                        cv.fillPoly(mask_without, [contour], 255)
 
-                    mask_with = np.zeros_like(img_gray)
-                    mask_without = np.zeros_like(img_gray)
                     if self.contours_state == "all" or self.contours_state == "select":
-                        # Fill the mask for outer contours
-                        for contour in outer_contours:
-                            cv.fillPoly(mask_with, [contour], 255)
-
-                        # Create and fill a separate mask for inner contours
                         inner_mask = np.zeros_like(img_gray)
                         for contour in inner_contours:
+                            contour = np.array(contour, dtype=np.int32)
                             cv.fillPoly(inner_mask, [contour], 255)
 
                         # Find intersection between outer and inner masks
-                        intersection = mask_with & inner_mask
+                        intersection = mask_without & inner_mask
+                        inner_contours, _ = cv.findContours(intersection, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
+                        inner_contours = ip.remove_small_contours(inner_contours)
+
 
                         # Subtract intersection from the outer contours mask
-                        mask_with = mask_with - intersection
+                        mask_with = mask_without - intersection
 
-                        # For 'mask_without', only fill the outer contours on a black background
-                    for contour in outer_contours:
-                        cv.fillPoly(mask_without, [contour], 255)
+                        for contour in inner_contours:
+                            cv.drawContours(img_with, [contour], -1, (255,0,0), 2)
 
 
                     for index, contour in enumerate(outer_contours):
-                        if not self.contours_state == "all":
-                            cv.drawContours(img_without, [contour], -1, [0, 0, 255], 2)
+                        contour_budding = self.evaluate(contour)
+
+                        if not contour_budding == "no_split":
+                            color = (0,255,0)
+                        else:
+                            color = (0,0,255)
+
+                        if self.contours_state == "all":
+                            cv.drawContours(img_with, [contour], -1, color, 2)
+                        elif self.contours_state == "no":
+                            cv.drawContours(img_without, [contour], -1, color, 2)
+                        else:
+                            cv.drawContours(img_without, [contour], -1, color, 2)
+                            cv.drawContours(img_with, [contour], -1, color, 2)
+
+                        if self.contours_state == "select" and dialog:
+                            dialog.update_selection_dialog(img_without, img_with, mask_without, mask_with,
+                                                           f"{self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}",
+                                                           f"{self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}",
+                                                           self.counter)
+                        elif self.contours_state == "all":
+                            if not cv.imwrite(f"{self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}",
+                                              mask_with):
+                                print(
+                                    f"FAILED to save mask: {self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}")
+                            if not cv.imwrite(
+                                    f"{self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}",
+                                    img_with):
+                                print(
+                                    f"FAILED to save image: {self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}")
+                        else:
+                            if not cv.imwrite(f"{self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}",
+                                              mask_without):
+                                print(
+                                    f"FAILED to save mask: {self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}")
+                            if not cv.imwrite(
+                                    f"{self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}",
+                                    img_without):
+                                print(
+                                    f"FAILED to save image: {self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}")
 
                         if self.calculate_properties:
                             contour_data = {
                                 'MaskName': os.path.basename(filename),
                                 'ContourOrder': index + 1
                             }
 
@@ -168,37 +199,14 @@
 
                     if self.create_json:
                         self.coco_data = fm.convert_contours_to_coco(outer_contours, inner_contours, height, width,
                                                                      filename,
                                                                      self.counter,
                                                                      self.coco_data)
 
-                if self.contours_state == "select":
-                    dialog.update_selection_dialog(img_without, img_with, mask_without, mask_with,
-                                                   f"{self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}",
-                                                   f"{self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}", self.counter)
-                elif self.contours_state == "all":
-                    if not cv.imwrite(f"{self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}",
-                                      mask_with):
-                        print(
-                            f"FAILED to save mask: {self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}")
-                    if not cv.imwrite(f"{self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}",
-                                      img_with):
-                        print(
-                            f"FAILED to save image: {self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}")
-                else:
-                    if not cv.imwrite(f"{self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}",
-                                      mask_without):
-                        print(
-                            f"FAILED to save mask: {self.output_segmented_path}/masks/{filename.replace('.bmp', '.png')}")
-                    if not cv.imwrite(f"{self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}",
-                                      img_without):
-                        print(
-                            f"FAILED to save image: {self.output_segmented_path}/results/{filename.replace('.bmp', '.png')}")
-
                 if self.progress_window:
                     progress_text = f"{self.counter}/{total_files}"
                     self.progress_window.update_progress(progress_text)
 
                 self.counter += 1
 
         if dialog:
@@ -251,23 +259,23 @@
         img = img.numpy()
 
         # Convert image to grayscale (assuming img is in BGR format)
         img_gray = cv.cvtColor(img, cv.COLOR_BGR2GRAY)
 
         # Apply the segmentation algorithm
         img_binary, inner_contours_mask = self.apply_segmentation_algorithm(
-            self.algorithm, parameters, img_gray, self.contours_state,
-            self.detect_corrupted)
+            self.algorithm, parameters, img_gray, self.contours_state)
 
         # Further processing and IoU, TPR, PPV computation
         if self.contours_state == "all" or self.contours_state == "select":
             intersection = inner_contours_mask & img_binary
             img_binary = img_binary - intersection
 
-        contours, hierarchy = cv.findContours(img_binary, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_NONE)
+        contours, _ = cv.findContours(img_binary, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_NONE)
+
 
         mask = np.zeros_like(img_binary, dtype=np.uint8)
         if not contours:
             # If no contours are found, draw a default contour
             contour = np.array([[0, 0]], dtype=np.int32)
             cv.drawContours(mask, [contour], 0, color=255, thickness=-1)
         else:
```

### Comparing `prusek_spheroid-4.0/prusek_spheroid/GUI.py` & `prusek_spheroid-4.1/prusek_spheroid/GUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.0/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-4.1/prusek_spheroid/GradientDescentGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
             self.cont_parameters.update({"window_size": 800})
             self.cont_param_ranges.update({"window_size": [1, 2001]})
 
         if self.algorithm == "Niblack":
             self.cont_parameters.update({"k": 0.2})
             self.cont_param_ranges.update({"k": [0.0, 0.35]})
 
-        self.cont_parameters.update({"min_area": 5000, "sigma": 1.0, "std_k": 0.5})
-        self.cont_param_ranges.update({"min_area": [0, 50000], "sigma": [0.0, 5.0], "std_k": [0.0, 3.0]})
+        self.cont_parameters.update({"min_area": 0.005, "sigma": 1.0, "std_k": 0.5})
+        self.cont_param_ranges.update({"min_area": [0.0, 0.1], "sigma": [0.0, 5.0], "std_k": [0.0, 3.0]})
 
         self.disc_parameters = {"dilation_size": 2}
         self.disc_param_ranges = {"dilation_size": [0, 10]}
 
         self.lr = learning_rate
         self.num_iterations = num_iterations
         self.epsilon = 0.05
```

### Comparing `prusek_spheroid-4.0/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-4.1/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.0/prusek_spheroid/conversion.py` & `prusek_spheroid-4.1/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.0/prusek_spheroid/file_management.py` & `prusek_spheroid-4.1/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.0/prusek_spheroid/image_processing.py` & `prusek_spheroid-4.1/prusek_spheroid/image_processing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 import numpy as np
 import cv2 as cv
 from skimage import img_as_ubyte
 from skimage import feature
 
+
+def remove_small_contours(contours, min_length=4):
+    filtered_contours = []
+    for contour in contours:
+        # Přetypování na NumPy pole s typem np.int32
+        contour_np = np.array(contour, dtype=np.int32)
+
+        # Ověření, že kontura není prázdná, a kontrola délky
+        if len(contour_np) > 0:
+            if cv.arcLength(contour_np, True) >= min_length:
+                filtered_contours.append(contour_np)
+    return filtered_contours
+def compute_hu_moments(contour):
+    moments = cv.moments(contour)
+    hu_moments = cv.HuMoments(moments).flatten()
+    return hu_moments
+
 def find_intersection(img_binary, filtered_contours, contours, hierarchy, edges, inner_contours):
     result_mask = np.zeros_like(img_binary, dtype=np.uint8)
 
     for contour in filtered_contours:
         filled_contour = cv.fillPoly(np.zeros_like(img_binary), [contour], 1)
 
         intersection = filled_contour & edges
@@ -18,15 +35,15 @@
         inner_contours_mask = np.zeros_like(img_binary, dtype=np.uint8)
         for i in range(len(contours)):
             if hierarchy[0, i, 3] != -1:
                 inner_filled_contour = cv.fillPoly(np.zeros_like(img_binary), [contours[i]], 1)
 
                 inner_contours_mask = cv.bitwise_or(inner_filled_contour, inner_contours_mask)
 
-        # inner_contours_mask = f.Erosion(inner_contours_mask, 3, 1)
+        inner_contours_mask = Dilation(Erosion(inner_contours_mask, 3, 1), 3, 1)
 
         return np.clip(result_mask, 0, 1), np.clip(inner_contours_mask, 0, 1)
 
     return np.clip(result_mask, 0, 1), None
 
 
 def create_binary_mask(img_gray, threshold, dilation_size, erosion_size=None):
@@ -42,16 +59,16 @@
     mean = np.mean(img_gray)
     std = np.std(img_gray)
     low_threshold = mean - std_k * std / 2
     high_threshold = mean + std_k * std / 2
     edges = feature.canny(img_gray, sigma=sigma, low_threshold=low_threshold, high_threshold=high_threshold)
     return edges
 
-def laplacian_of_gaussian(image, std_k, sigma):
 
+def laplacian_of_gaussian(image, std_k, sigma):
     image = cv.bitwise_not(image)
 
     blurred_image = cv.GaussianBlur(image, (0, 0), sigmaX=sigma, sigmaY=sigma)
 
     laplacian = cv.Laplacian(blurred_image, cv.CV_64F)
 
     # Apply threshold to focus on significant edges
@@ -79,72 +96,39 @@
     for contour in contours:
         if cv.contourArea(contour) >= min_area:
             filtered_contours.append(contour)
 
     return filtered_contours
 
 
-def filter_contours_on_frame(contours, hierarchy, img_shape, min_area, detect_corrupted=True):
-    if hierarchy is None:
-        return [], np.empty((0, 4), int)
+def filter_contours_on_frame(contours, img_shape, min_area, detect_corrupted=True):
     height, width = img_shape
+    min_area = min_area * height * width
+    filtered_contours = []
 
     if detect_corrupted:
-        # Convert hierarchy for easier use
-        hierarchy = hierarchy[0]
-        # Identify outer contours and calculate total area of outer contours
-        outer_contours_indices = [idx for idx, h in enumerate(hierarchy) if h[3] == -1]
-        total_outer_area = sum(cv.contourArea(contours[idx]) for idx in outer_contours_indices)
-
-        # Initialize a set to keep track of contours to remove (by index)
-        remove_indices = set()
-
-        def add_children_to_remove(idx):
-            """Recursive function to add children to removal list."""
-            first_child = hierarchy[idx][2]
-            while first_child != -1:
-                remove_indices.add(first_child)
-                add_children_to_remove(first_child)  # Recurse to add any further descendants
-                first_child = hierarchy[first_child][0]  # Go to next sibling
-
-        for idx in outer_contours_indices:
-            contour = contours[idx]
-            # Check if contour touches the edges
+        total_outer_area = sum(cv.contourArea(contour) for contour in contours)
+
+        for contour in contours:
             touches_top = np.any(contour[:, :, 1] == 0)
             touches_bottom = np.any(contour[:, :, 1] == height - 1)
             touches_left = np.any(contour[:, :, 0] == 0)
             touches_right = np.any(contour[:, :, 0] == width - 1)
             num_edges_touched = sum([touches_top, touches_bottom, touches_left, touches_right])
 
             contour_area = cv.contourArea(contour)
-            if num_edges_touched > 1 or contour_area < min_area:
-                # Mark for removal and calculate area
-                remove_indices.add(idx)
-                add_children_to_remove(idx)
-
+            if num_edges_touched > 0 or contour_area < min_area:
                 # Check if the contour's area is large enough to return an empty list immediately
                 if contour_area > 0.75 * total_outer_area:
                     return [], np.empty((0, 4), int)
+            else:
+                filtered_contours.append(contour)
 
-        # Reindex remaining contours and rebuild hierarchy
-        remaining_indices = sorted(set(range(len(contours))) - remove_indices)
-        index_mapping = {old_i: new_i for new_i, old_i in enumerate(remaining_indices)}
-        filtered_contours = [contours[i] for i in remaining_indices]
-        filtered_hierarchy = []
-        for i in remaining_indices:
-            next_, previous, first_child, parent = hierarchy[i]
-            new_hierarchy = [index_mapping.get(next_, -1), index_mapping.get(previous, -1),
-                             index_mapping.get(first_child, -1), index_mapping.get(parent, -1)]
-            filtered_hierarchy.append(new_hierarchy)
-
-    else:
-        filtered_contours = list(contours)
-        filtered_hierarchy = hierarchy[0]
+    return filtered_contours
 
-    return filtered_contours, np.array([filtered_hierarchy])
 
 def check_window_size(window_size):
     return window_size + 1 if window_size % 2 == 0 else window_size
 
 
 def findContours(img_binary, inner_contours):
     if inner_contours:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prusek_spheroid-4.0/prusek_spheroid/merge_directories.py` & `prusek_spheroid-4.1/prusek_spheroid/merge_directories.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     for root, dirs, files in os.walk(root_dir):
         for file in files:
             if file.endswith('.bmp'):
                 processed_files += 1
                 file_path = os.path.join(root, file)
                 relative_path = os.path.relpath(root, root_dir)
                 new_file_name = relative_path.replace(os.path.sep, '_') + '_' + file
-                output_file_path = os.path.join(output_dir, new_file_name)
+                output_file_path = os.path.join(output_dir, new_file_name.replace(".bmp", ".png"))
 
                 try:
                     # Open and resize the image
                     with Image.open(file_path) as img:
                         img_resized = img.resize((1000, 1000), Image.LANCZOS)  # High-quality resize
                         image_hash = imagehash.average_hash(img_resized, hash_size=32)
```

### Comparing `prusek_spheroid-4.0/prusek_spheroid/methods.py` & `prusek_spheroid-4.1/prusek_spheroid/methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 import sys
 from prusek_spheroid import image_processing as ip
 from skimage.filters import threshold_sauvola, threshold_niblack
 import cv2 as cv
+import numpy as np
 
 
 class BaseImageProcessing:
-    def apply_segmentation_algorithm(self, algorithm, parameters, img, inner_contours,
-                                     detect_corrupted):
+    def apply_segmentation_algorithm(self, algorithm, parameters, img, inner_contours):
         if algorithm == "Sauvola":
-            return self.sauvola(parameters, img, inner_contours, detect_corrupted)
+            return self.sauvola(parameters, img, inner_contours)
         elif algorithm == "Niblack":
-            return self.niblack(parameters, img, inner_contours, detect_corrupted)
+            return self.niblack(parameters, img, inner_contours)
         elif algorithm == "Gaussian":
-            return self.gaussian_adaptive(parameters, img, inner_contours, detect_corrupted)
+            return self.gaussian_adaptive(parameters, img, inner_contours)
         else:
             print(f"Algorithm with name {algorithm} not found.")
             sys.exit(1)
 
     @staticmethod
-    def sauvola(parameters, img_gray, inner_contours, detect_corrupted):
+    def sauvola(parameters, img_gray, inner_contours):
         window_size = ip.check_window_size(int(parameters["window_size"]))
         std_k = parameters["std_k"]
-        min_area = parameters["min_area"]
+        min_area = parameters["min_area"] * np.shape(img_gray)[0] * np.shape(img_gray)[1]
         dilation_size = int(parameters["dilation_size"])
         sigma = parameters["sigma"]
 
         thresh_sauvola = threshold_sauvola(img_gray, window_size=window_size)
         img_binary = ip.create_binary_mask(img_gray, thresh_sauvola, dilation_size)
-        #edges = ip.calculate_canny_edges(img_gray, std_k, sigma)
-        edges = ip.laplacian_of_gaussian(img_gray, std_k, sigma)
+        edges = ip.calculate_canny_edges(img_gray, std_k, sigma)
+        # edges = ip.laplacian_of_gaussian(img_gray, std_k, sigma)
 
         contours, hierarchy = ip.findContours(img_binary, inner_contours)
         filtered_contours = ip.filter_contours(contours, min_area)
 
         return ip.find_intersection(img_binary, filtered_contours, contours, hierarchy, edges, inner_contours)
 
     @staticmethod
-    def niblack(parameters, img_gray, inner_contours, detect_corrupted):
+    def niblack(parameters, img_gray, inner_contours):
         window_size = ip.check_window_size(int(parameters["window_size"]))
         k = parameters["k"]
-        min_area = parameters["min_area"]
+        min_area = parameters["min_area"] * np.shape(img_gray)[0] * np.shape(img_gray)[1]
         std_k = parameters["std_k"]
         dilation_size = int(parameters["dilation_size"])
         sigma = parameters["sigma"]
 
         thresh_niblack = threshold_niblack(img_gray, window_size=window_size, k=k)
         img_binary = ip.create_binary_mask(img_gray, thresh_niblack, dilation_size, 1)
 
-        #edges = ip.calculate_canny_edges(img_gray, std_k, sigma)
-        edges = ip.laplacian_of_gaussian(img_gray, std_k, sigma)
+        edges = ip.calculate_canny_edges(img_gray, std_k, sigma)
+        # edges = ip.laplacian_of_gaussian(img_gray, std_k, sigma)
 
         contours, hierarchy = ip.findContours(img_binary, inner_contours)
         filtered_contours = ip.filter_contours(contours, min_area)
 
         return ip.find_intersection(img_binary, filtered_contours, contours, hierarchy, edges, inner_contours)
 
     @staticmethod
-    def gaussian_adaptive(parameters, img_gray, inner_contours, detect_corrupted):
+    def gaussian_adaptive(parameters, img_gray, inner_contours):
         window_size = ip.check_window_size(int(parameters["window_size"]))
-        min_area = parameters["min_area"]
+        min_area = parameters["min_area"] * np.shape(img_gray)[0] * np.shape(img_gray)[1]
         std_k = parameters["std_k"]
         dilation_size = int(parameters["dilation_size"])
         sigma = parameters["sigma"]
 
         img_binary = cv.adaptiveThreshold(img_gray, 255, cv.ADAPTIVE_THRESH_GAUSSIAN_C, cv.THRESH_BINARY_INV,
                                           window_size, 0)
 
         img_binary = ip.Erosion(img_binary, 1, 1)
 
         img_binary = ip.Dilation(img_binary, dilation_size, 1)
 
-        #edges = ip.calculate_canny_edges(img_gray, std_k, sigma)
-        edges = ip.laplacian_of_gaussian(img_gray, std_k, sigma)
+        edges = ip.calculate_canny_edges(img_gray, std_k, sigma)
+        # edges = ip.laplacian_of_gaussian(img_gray, std_k, sigma)
 
         contours, hierarchy = ip.findContours(img_binary, inner_contours)
 
         filtered_contours = ip.filter_contours(contours, min_area)
 
         result = ip.find_intersection(img_binary, filtered_contours, contours, hierarchy, edges, inner_contours)
```

### Comparing `prusek_spheroid-4.0/prusek_spheroid/metrics.py` & `prusek_spheroid-4.1/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.0/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-4.1/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.0/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-4.1/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 4.0
+Version: 4.1
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
@@ -14,14 +14,15 @@
 Requires-Dist: threadpoolctl
 Requires-Dist: matplotlib
 Requires-Dist: rasterio
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 Requires-Dist: torch
 Requires-Dist: imagehash
+Requires-Dist: joblib
 
 # Prusek-Spheroid
 
 Prusek-Spheroid is a Python package designed for spheroid segmentation based on provided microscope images. This package provides an easy-to-use interface and functionalities that are essential for determination of properties and characteristics of the spheroids.
 
 ## Installation
```

### Comparing `prusek_spheroid-4.0/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-4.1/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

