# Comparing `tmp/st-input-slider-0.0.1.tar.gz` & `tmp/st-input-slider-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-input-slider-0.0.1.tar", last modified: Mon Apr  8 17:49:47 2024, max compression
+gzip compressed data, was "st-input-slider-0.0.2.tar", last modified: Mon Apr  8 19:54:40 2024, max compression
```

## Comparing `st-input-slider-0.0.1.tar` & `st-input-slider-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 17:49:47.461449 st-input-slider-0.0.1/
--rw-rw-rw-   0        0        0     1082 2024-04-05 22:58:34.000000 st-input-slider-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       52 2024-04-08 17:41:29.000000 st-input-slider-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1132 2024-04-08 17:49:47.457642 st-input-slider-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      763 2024-04-08 17:47:47.000000 st-input-slider-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 17:49:47.463720 st-input-slider-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1145 2024-04-08 17:08:32.000000 st-input-slider-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 17:49:47.331842 st-input-slider-0.0.1/st_input_slider/
--rw-rw-rw-   0        0        0     3859 2024-04-08 17:39:24.000000 st-input-slider-0.0.1/st_input_slider/__init__.py
--rw-rw-rw-   0        0        0      513 2024-04-08 17:46:24.000000 st-input-slider-0.0.1/st_input_slider/example.py
-drwxrwxrwx   0        0        0        0 2024-04-08 17:49:47.198231 st-input-slider-0.0.1/st_input_slider/frontend/
-drwxrwxrwx   0        0        0        0 2024-04-08 17:49:47.400157 st-input-slider-0.0.1/st_input_slider/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-04-08 17:41:21.000000 st-input-slider-0.0.1/st_input_slider/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-05 22:58:35.000000 st-input-slider-0.0.1/st_input_slider/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-04-08 17:41:21.000000 st-input-slider-0.0.1/st_input_slider/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 17:49:47.233276 st-input-slider-0.0.1/st_input_slider/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-04-08 17:49:47.435779 st-input-slider-0.0.1/st_input_slider/frontend/build/static/js/
--rw-rw-rw-   0        0        0   446638 2024-04-08 17:41:21.000000 st-input-slider-0.0.1/st_input_slider/frontend/build/static/js/main.7c161973.js
--rw-rw-rw-   0        0        0     1755 2024-04-08 17:41:21.000000 st-input-slider-0.0.1/st_input_slider/frontend/build/static/js/main.7c161973.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1860914 2024-04-08 17:41:21.000000 st-input-slider-0.0.1/st_input_slider/frontend/build/static/js/main.7c161973.js.map
-drwxrwxrwx   0        0        0        0 2024-04-08 17:49:47.373155 st-input-slider-0.0.1/st_input_slider.egg-info/
--rw-rw-rw-   0        0        0     1132 2024-04-08 17:49:46.000000 st-input-slider-0.0.1/st_input_slider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2024-04-08 17:49:47.000000 st-input-slider-0.0.1/st_input_slider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 17:49:46.000000 st-input-slider-0.0.1/st_input_slider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-08 17:49:46.000000 st-input-slider-0.0.1/st_input_slider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-08 17:49:46.000000 st-input-slider-0.0.1/st_input_slider.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 19:54:40.878371 st-input-slider-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2024-04-05 22:58:34.000000 st-input-slider-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       52 2024-04-08 17:41:29.000000 st-input-slider-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1128 2024-04-08 19:54:40.873383 st-input-slider-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      759 2024-04-08 19:54:11.000000 st-input-slider-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 19:54:40.879452 st-input-slider-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2024-04-08 19:53:53.000000 st-input-slider-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:54:40.714678 st-input-slider-0.0.2/st_input_slider/
+-rw-rw-rw-   0        0        0     3859 2024-04-08 17:39:24.000000 st-input-slider-0.0.2/st_input_slider/__init__.py
+-rw-rw-rw-   0        0        0      513 2024-04-08 17:46:24.000000 st-input-slider-0.0.2/st_input_slider/example.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:54:40.651358 st-input-slider-0.0.2/st_input_slider/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-08 19:54:40.801748 st-input-slider-0.0.2/st_input_slider/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-04-08 17:41:21.000000 st-input-slider-0.0.2/st_input_slider/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-05 22:58:35.000000 st-input-slider-0.0.2/st_input_slider/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2024-04-08 17:41:21.000000 st-input-slider-0.0.2/st_input_slider/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-08 19:54:40.654351 st-input-slider-0.0.2/st_input_slider/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-08 19:54:40.844272 st-input-slider-0.0.2/st_input_slider/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   446638 2024-04-08 17:41:21.000000 st-input-slider-0.0.2/st_input_slider/frontend/build/static/js/main.7c161973.js
+-rw-rw-rw-   0        0        0     1755 2024-04-08 17:41:21.000000 st-input-slider-0.0.2/st_input_slider/frontend/build/static/js/main.7c161973.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1860914 2024-04-08 17:41:21.000000 st-input-slider-0.0.2/st_input_slider/frontend/build/static/js/main.7c161973.js.map
+drwxrwxrwx   0        0        0        0 2024-04-08 19:54:40.765393 st-input-slider-0.0.2/st_input_slider.egg-info/
+-rw-rw-rw-   0        0        0     1128 2024-04-08 19:54:40.000000 st-input-slider-0.0.2/st_input_slider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2024-04-08 19:54:40.000000 st-input-slider-0.0.2/st_input_slider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 19:54:40.000000 st-input-slider-0.0.2/st_input_slider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-08 19:54:40.000000 st-input-slider-0.0.2/st_input_slider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-08 19:54:40.000000 st-input-slider-0.0.2/st_input_slider.egg-info/top_level.txt
```

### Comparing `st-input-slider-0.0.1/LICENSE` & `st-input-slider-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.0.1/PKG-INFO` & `st-input-slider-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: st-input-slider
-Version: 0.0.1
+Version: 0.0.2
 Summary: A custom Streamlit component that combines a slider with an input box for more precise value selection
 Home-page: 
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
 License-File: LICENSE
 
-# streamlit-custom-component
+# streamlit-input-slider
 A custom Streamlit component that combines a slider with an input box for more precise value selection
 
 ## Installation instructions
 
 ```sh
 pip install st-input-slider
 ```
```

### Comparing `st-input-slider-0.0.1/README.md` & `st-input-slider-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# streamlit-custom-component
+# streamlit-input-slider
 A custom Streamlit component that combines a slider with an input box for more precise value selection
 
 ## Installation instructions
 
 ```sh
 pip install st-input-slider
 ```
```

### Comparing `st-input-slider-0.0.1/setup.py` & `st-input-slider-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="st-input-slider",
-    version="0.0.1",
+    version="0.0.2",
     author="Brayan Munoz",
     author_email="balexander.munoz@udea.edu.co",
     description="A custom Streamlit component that combines a slider with an input box for more precise value selection",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st-input-slider-0.0.1/st_input_slider/__init__.py` & `st-input-slider-0.0.2/st_input_slider/__init__.py`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.0.1/st_input_slider/example.py` & `st-input-slider-0.0.2/st_input_slider/example.py`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.0.1/st_input_slider/frontend/build/bootstrap.min.css` & `st-input-slider-0.0.2/st_input_slider/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.0.1/st_input_slider/frontend/build/static/js/main.7c161973.js` & `st-input-slider-0.0.2/st_input_slider/frontend/build/static/js/main.7c161973.js`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.0.1/st_input_slider/frontend/build/static/js/main.7c161973.js.LICENSE.txt` & `st-input-slider-0.0.2/st_input_slider/frontend/build/static/js/main.7c161973.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.0.1/st_input_slider/frontend/build/static/js/main.7c161973.js.map` & `st-input-slider-0.0.2/st_input_slider/frontend/build/static/js/main.7c161973.js.map`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.0.1/st_input_slider.egg-info/PKG-INFO` & `st-input-slider-0.0.2/st_input_slider.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: st-input-slider
-Version: 0.0.1
+Version: 0.0.2
 Summary: A custom Streamlit component that combines a slider with an input box for more precise value selection
 Home-page: 
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
 License-File: LICENSE
 
-# streamlit-custom-component
+# streamlit-input-slider
 A custom Streamlit component that combines a slider with an input box for more precise value selection
 
 ## Installation instructions
 
 ```sh
 pip install st-input-slider
 ```
```

### Comparing `st-input-slider-0.0.1/st_input_slider.egg-info/SOURCES.txt` & `st-input-slider-0.0.2/st_input_slider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

