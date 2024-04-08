# Comparing `tmp/dcx-0.76.0.tar.gz` & `tmp/dcx-0.77.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcx-0.76.0.tar", last modified: Mon Apr  8 16:25:18 2024, max compression
+gzip compressed data, was "dcx-0.77.0.tar", last modified: Mon Apr  8 16:36:01 2024, max compression
```

## Comparing `dcx-0.76.0.tar` & `dcx-0.77.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:25:18.418844 dcx-0.76.0/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-02-16 09:45:07.000000 dcx-0.76.0/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:25:18.418657 dcx-0.76.0/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      159 2024-02-25 22:16:23.000000 dcx-0.76.0/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      716 2024-04-08 16:25:16.000000 dcx-0.76.0/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-04-08 16:25:18.418886 dcx-0.76.0/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:25:18.416234 dcx-0.76.0/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:25:18.417042 dcx-0.76.0/src/dcx/
--rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-01-14 18:51:20.000000 dcx-0.76.0/src/dcx/__init__.py
--rw-r--r--   0 robertdegen   (501) staff       (20)    64762 2024-04-08 16:14:29.000000 dcx-0.76.0/src/dcx/__main__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:25:18.418488 dcx-0.76.0/src/dcx.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:25:18.000000 dcx-0.76.0/src/dcx.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      226 2024-04-08 16:25:18.000000 dcx-0.76.0/src/dcx.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-04-08 16:25:18.000000 dcx-0.76.0/src/dcx.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       83 2024-04-08 16:25:18.000000 dcx-0.76.0/src/dcx.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-04-08 16:25:18.000000 dcx-0.76.0/src/dcx.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:36:01.462956 dcx-0.77.0/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-02-16 09:45:07.000000 dcx-0.77.0/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:36:01.462787 dcx-0.77.0/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      159 2024-02-25 22:16:23.000000 dcx-0.77.0/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      716 2024-04-08 16:35:59.000000 dcx-0.77.0/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-04-08 16:36:01.462993 dcx-0.77.0/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:36:01.460619 dcx-0.77.0/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:36:01.461293 dcx-0.77.0/src/dcx/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-01-14 18:51:20.000000 dcx-0.77.0/src/dcx/__init__.py
+-rw-r--r--   0 robertdegen   (501) staff       (20)    64947 2024-04-08 16:35:55.000000 dcx-0.77.0/src/dcx/__main__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:36:01.462629 dcx-0.77.0/src/dcx.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:36:01.000000 dcx-0.77.0/src/dcx.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      226 2024-04-08 16:36:01.000000 dcx-0.77.0/src/dcx.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-04-08 16:36:01.000000 dcx-0.77.0/src/dcx.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       83 2024-04-08 16:36:01.000000 dcx-0.77.0/src/dcx.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-04-08 16:36:01.000000 dcx-0.77.0/src/dcx.egg-info/top_level.txt
```

### Comparing `dcx-0.76.0/PKG-INFO` & `dcx-0.77.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcx
-Version: 0.76.0
+Version: 0.77.0
 Summary: Minimalistic selenium wrapper
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert/dcx
 Project-URL: Issues, https://github.com/turbo-bert/dcx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcx-0.76.0/pyproject.toml` & `dcx-0.77.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dcx"
-version = "0.76.0"
+version = "0.77.0"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "Minimalistic selenium wrapper"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dcx-0.76.0/src/dcx/__main__.py` & `dcx-0.77.0/src/dcx/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,36 +503,37 @@
                 image_params = [25, 185, screenshot_w_default_mm, calclulated_height, jpg]
             else:
                 #TODO: porttrait mode
                 pass
             pdf.page(the_page).image_manual_mm(*image_params)
 
             # OUT screenshot##################################################################################
-            png = REPORT['viewports_out'][report_i]
-            jpg = "%s.jpg" % png
-            png_ = PIL.Image.open(png)
-            jpg_ = png_.convert("RGB")
-            jpg_.save(jpg)
-            jpg_width, jpg_height = jpg_.size
-            jpg_landscape = jpg_width >= jpg_height
-            image_params = []
-            if jpg_landscape:
-                # bring to maximal width (DIN A3 Port = 250mm)
-                jpg_ratio = float(jpg_width) / float(jpg_height) # 1.XXXX
-                calclulated_height = int(float(screenshot_w_default_mm) / jpg_ratio)
-                image_params = [25, 5, screenshot_w_default_mm, calclulated_height, jpg]
-            else:
-                #TODO: porttrait mode
-                pass
-            pdf.page(the_page).image_manual_mm(*image_params)
-
-
-
-
+            
+            # screenshot maybe missing
 
+            try:
+                png = REPORT['viewports_out'][report_i]
+                jpg = "%s.jpg" % png
+                png_ = PIL.Image.open(png)
+                jpg_ = png_.convert("RGB")
+                jpg_.save(jpg)
+                jpg_width, jpg_height = jpg_.size
+                jpg_landscape = jpg_width >= jpg_height
+                image_params = []
+                if jpg_landscape:
+                    # bring to maximal width (DIN A3 Port = 250mm)
+                    jpg_ratio = float(jpg_width) / float(jpg_height) # 1.XXXX
+                    calclulated_height = int(float(screenshot_w_default_mm) / jpg_ratio)
+                    image_params = [25, 5, screenshot_w_default_mm, calclulated_height, jpg]
+                else:
+                    #TODO: porttrait mode
+                    pass
+                pdf.page(the_page).image_manual_mm(*image_params)
+            except IndexError:
+                pass
 
             the_page += 1
             i+=1
 
         pdf.page(the_page).text(1, 10, "END OF EXECUTION")
         the_page += 1
```

### Comparing `dcx-0.76.0/src/dcx.egg-info/PKG-INFO` & `dcx-0.77.0/src/dcx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcx
-Version: 0.76.0
+Version: 0.77.0
 Summary: Minimalistic selenium wrapper
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert/dcx
 Project-URL: Issues, https://github.com/turbo-bert/dcx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

