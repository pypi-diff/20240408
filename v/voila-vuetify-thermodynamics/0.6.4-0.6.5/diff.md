# Comparing `tmp/voila-vuetify-thermodynamics-0.6.4.tar.gz` & `tmp/voila-vuetify-thermodynamics-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-vuetify-thermodynamics-0.6.4.tar", last modified: Mon Apr  8 20:52:12 2024, max compression
+gzip compressed data, was "voila-vuetify-thermodynamics-0.6.5.tar", last modified: Mon Apr  8 21:33:45 2024, max compression
```

## Comparing `voila-vuetify-thermodynamics-0.6.4.tar` & `voila-vuetify-thermodynamics-0.6.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.735186 voila-vuetify-thermodynamics-0.6.4/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1545 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/LICENSE
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       68 2024-04-08 20:50:57.000000 voila-vuetify-thermodynamics-0.6.4/MANIFEST.in
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      297 2024-04-08 20:52:12.735090 voila-vuetify-thermodynamics-0.6.4/PKG-INFO
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1574 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/README.md
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      101 2024-04-08 20:52:12.735430 voila-vuetify-thermodynamics-0.6.4/setup.cfg
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     3458 2024-04-08 20:52:04.000000 voila-vuetify-thermodynamics-0.6.4/setup.py
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.729774 voila-vuetify-thermodynamics-0.6.4/share/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.730122 voila-vuetify-thermodynamics-0.6.4/share/jupyter/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.729889 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.730032 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.733272 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     7797 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/ansi.js
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1434 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/app.html
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       25 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/conf.json
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     3179 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/index.html.j2
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     7280 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/util.js
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.733832 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-default/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     6381 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-default/app.html
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       33 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-default/conf.json
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.730182 voila-vuetify-thermodynamics-0.6.4/share/jupyter/voila/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.730244 voila-vuetify-thermodynamics-0.6.4/share/jupyter/voila/templates/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.734029 voila-vuetify-thermodynamics-0.6.4/share/jupyter/voila/templates/vuetify-base/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1757 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/voila/templates/vuetify-base/index.html.j2
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.734855 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      297 2024-04-08 20:52:12.000000 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/PKG-INFO
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      767 2024-04-08 20:52:12.000000 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/SOURCES.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)        1 2024-04-08 20:52:12.000000 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/dependency_links.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       31 2024-04-08 20:52:12.000000 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/requires.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)        6 2024-04-08 20:52:12.000000 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/top_level.txt
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.787618 voila-vuetify-thermodynamics-0.6.5/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1545 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/LICENSE
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       68 2024-04-08 20:50:57.000000 voila-vuetify-thermodynamics-0.6.5/MANIFEST.in
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      297 2024-04-08 21:33:45.787524 voila-vuetify-thermodynamics-0.6.5/PKG-INFO
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1574 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/README.md
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      101 2024-04-08 21:33:45.787855 voila-vuetify-thermodynamics-0.6.5/setup.cfg
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     3518 2024-04-08 21:31:26.000000 voila-vuetify-thermodynamics-0.6.5/setup.py
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779302 voila-vuetify-thermodynamics-0.6.5/share/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779811 voila-vuetify-thermodynamics-0.6.5/share/jupyter/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779498 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779684 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.785231 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     7797 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/ansi.js
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1434 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/app.html
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       25 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/conf.json
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     3179 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/index.html.j2
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     7280 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/util.js
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.786010 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     6381 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/app.html
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       48 2024-04-08 21:29:17.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/conf.json
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779899 voila-vuetify-thermodynamics-0.6.5/share/jupyter/voila/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779980 voila-vuetify-thermodynamics-0.6.5/share/jupyter/voila/templates/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.786249 voila-vuetify-thermodynamics-0.6.5/share/jupyter/voila/templates/vuetify-base-thermodynamics/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1772 2024-04-08 21:29:45.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/voila/templates/vuetify-base-thermodynamics/index.html.j2
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.787262 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      297 2024-04-08 21:33:45.000000 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/PKG-INFO
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      887 2024-04-08 21:33:45.000000 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)        1 2024-04-08 21:33:45.000000 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       31 2024-04-08 21:33:45.000000 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/requires.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)        6 2024-04-08 21:33:45.000000 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/top_level.txt
```

### Comparing `voila-vuetify-thermodynamics-0.6.4/LICENSE` & `voila-vuetify-thermodynamics-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.4/README.md` & `voila-vuetify-thermodynamics-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.4/setup.py` & `voila-vuetify-thermodynamics-0.6.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,18 +51,18 @@
         if not xdg:
             xdg = pjoin(home, '.local', 'share')
         return pjoin(xdg, 'jupyter')
 
 
 class DevelopCmd(develop):
     prefix_targets = [
-        ("nbconvert/templates", 'vuetify-base'),
-        ("nbconvert/templates", 'vuetify-default'),
-        ("voila/templates", 'vuetify-base'),
-        ("voila/templates", 'vuetify-default'),
+        ("nbconvert/templates", 'vuetify-base-thermodynamics'),
+        ("nbconvert/templates", 'vuetify-default-thermodynamics'),
+        ("voila/templates", 'vuetify-base-thermodynamics'),
+        ("voila/templates", 'vuetify-default-thermodynamics'),
     ]
     def run(self):
         target_dir = os.path.join(sys.prefix, 'share', 'jupyter')
         if '--user' in sys.prefix:  # TODO: is there a better way to find out?
             target_dir = user_dir()
         target_dir = os.path.join(target_dir)
 
@@ -92,15 +92,15 @@
         data_files.append((dirpath, [os.path.join(dirpath, filename) for filename in filenames]))
 
 
 print("Setup.py is being executed")
 
 setup(
     name='voila-vuetify-thermodynamics',
-    version="0.6.4",
+    version="0.6.5",
     description="A vuetify template for Voila",
     data_files=data_files,
     install_requires=['voila>=0.2.0,<0.5', 'jupyter_core'],
     include_package_data=True,
     author='Mario Buikhuizen, Maarten Breddels',
     keywords=[
         'ipython',
```

### Comparing `voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/ansi.js` & `voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/ansi.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/app.html` & `voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/index.html.j2` & `voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/util.js` & `voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/util.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-default/app.html` & `voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.4/share/jupyter/voila/templates/vuetify-base/index.html.j2` & `voila-vuetify-thermodynamics-0.6.5/share/jupyter/voila/templates/vuetify-base-thermodynamics/index.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- extends 'nbconvert/templates/vuetify-base/index.html.j2' -%}
+{%- extends 'nbconvert/templates/vuetify-base-thermodynamics/index.html.j2' -%}
 {% block notebook_execute %}
 
 {%- set kernel_id = kernel_start(nb) -%}
     <script id="jupyter-config-data" type="application/json">
         {
             "baseUrl": "{{resources.base_url}}",
             "kernelId": "{{kernel_id}}"
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-{%- extends 'nbconvert/templates/vuetify-base/index.html.j2' -%} {% block
-notebook_execute %} {%- set kernel_id = kernel_start(nb) -%}
+{%- extends 'nbconvert/templates/vuetify-base-thermodynamics/index.html.j2' -%}
+{% block notebook_execute %} {%- set kernel_id = kernel_start(nb) -%}
 {% endblock notebook_execute %} {% block cell_generator %}
 {% for cell in cell_generator(nb, kernel_id) %}
 {% if cell.cell_type == 'code' %} {% for output in cell.outputs %} {% if
 output.output_type == 'error' %}
 {% endif %} {% endfor %} {% endif %} {% endfor %} {% endblock cell_generator %}
```

