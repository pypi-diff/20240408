# Comparing `tmp/voila-vuetify-thermodynamics-0.6.5.tar.gz` & `tmp/voila-vuetify-thermodynamics-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-vuetify-thermodynamics-0.6.5.tar", last modified: Mon Apr  8 21:33:45 2024, max compression
+gzip compressed data, was "voila-vuetify-thermodynamics-0.6.6.tar", last modified: Mon Apr  8 21:49:33 2024, max compression
```

## Comparing `voila-vuetify-thermodynamics-0.6.5.tar` & `voila-vuetify-thermodynamics-0.6.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.787618 voila-vuetify-thermodynamics-0.6.5/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1545 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/LICENSE
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       68 2024-04-08 20:50:57.000000 voila-vuetify-thermodynamics-0.6.5/MANIFEST.in
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      297 2024-04-08 21:33:45.787524 voila-vuetify-thermodynamics-0.6.5/PKG-INFO
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1574 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/README.md
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      101 2024-04-08 21:33:45.787855 voila-vuetify-thermodynamics-0.6.5/setup.cfg
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     3518 2024-04-08 21:31:26.000000 voila-vuetify-thermodynamics-0.6.5/setup.py
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779302 voila-vuetify-thermodynamics-0.6.5/share/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779811 voila-vuetify-thermodynamics-0.6.5/share/jupyter/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779498 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779684 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.785231 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     7797 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/ansi.js
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1434 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/app.html
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       25 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/conf.json
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     3179 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/index.html.j2
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     7280 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/util.js
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.786010 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     6381 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/app.html
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       48 2024-04-08 21:29:17.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/conf.json
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779899 voila-vuetify-thermodynamics-0.6.5/share/jupyter/voila/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.779980 voila-vuetify-thermodynamics-0.6.5/share/jupyter/voila/templates/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.786249 voila-vuetify-thermodynamics-0.6.5/share/jupyter/voila/templates/vuetify-base-thermodynamics/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1772 2024-04-08 21:29:45.000000 voila-vuetify-thermodynamics-0.6.5/share/jupyter/voila/templates/vuetify-base-thermodynamics/index.html.j2
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:33:45.787262 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      297 2024-04-08 21:33:45.000000 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/PKG-INFO
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      887 2024-04-08 21:33:45.000000 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/SOURCES.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)        1 2024-04-08 21:33:45.000000 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/dependency_links.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       31 2024-04-08 21:33:45.000000 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/requires.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)        6 2024-04-08 21:33:45.000000 voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/top_level.txt
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:49:33.011199 voila-vuetify-thermodynamics-0.6.6/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1545 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.6/LICENSE
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       68 2024-04-08 20:50:57.000000 voila-vuetify-thermodynamics-0.6.6/MANIFEST.in
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      325 2024-04-08 21:49:33.011099 voila-vuetify-thermodynamics-0.6.6/PKG-INFO
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1574 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.6/README.md
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      101 2024-04-08 21:49:33.011521 voila-vuetify-thermodynamics-0.6.6/setup.cfg
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     3534 2024-04-08 21:49:28.000000 voila-vuetify-thermodynamics-0.6.6/setup.py
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:49:32.997016 voila-vuetify-thermodynamics-0.6.6/share/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:49:32.997367 voila-vuetify-thermodynamics-0.6.6/share/jupyter/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:49:32.997143 voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:49:32.997284 voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:49:33.003762 voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     7797 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/ansi.js
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1434 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/app.html
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       25 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/conf.json
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     3179 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/index.html.j2
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     7280 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/util.js
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:49:33.006849 voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     6664 2024-04-08 21:44:00.000000 voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/app.html
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       48 2024-04-08 21:29:17.000000 voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/conf.json
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:49:32.997426 voila-vuetify-thermodynamics-0.6.6/share/jupyter/voila/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:49:32.997485 voila-vuetify-thermodynamics-0.6.6/share/jupyter/voila/templates/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:49:33.007274 voila-vuetify-thermodynamics-0.6.6/share/jupyter/voila/templates/vuetify-base-thermodynamics/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1772 2024-04-08 21:29:45.000000 voila-vuetify-thermodynamics-0.6.6/share/jupyter/voila/templates/vuetify-base-thermodynamics/index.html.j2
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 21:49:33.010573 voila-vuetify-thermodynamics-0.6.6/voila_vuetify_thermodynamics.egg-info/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      325 2024-04-08 21:49:32.000000 voila-vuetify-thermodynamics-0.6.6/voila_vuetify_thermodynamics.egg-info/PKG-INFO
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      887 2024-04-08 21:49:32.000000 voila-vuetify-thermodynamics-0.6.6/voila_vuetify_thermodynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)        1 2024-04-08 21:49:32.000000 voila-vuetify-thermodynamics-0.6.6/voila_vuetify_thermodynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       45 2024-04-08 21:49:32.000000 voila-vuetify-thermodynamics-0.6.6/voila_vuetify_thermodynamics.egg-info/requires.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)        6 2024-04-08 21:49:32.000000 voila-vuetify-thermodynamics-0.6.6/voila_vuetify_thermodynamics.egg-info/top_level.txt
```

### Comparing `voila-vuetify-thermodynamics-0.6.5/LICENSE` & `voila-vuetify-thermodynamics-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.5/README.md` & `voila-vuetify-thermodynamics-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.5/setup.py` & `voila-vuetify-thermodynamics-0.6.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,20 +92,20 @@
         data_files.append((dirpath, [os.path.join(dirpath, filename) for filename in filenames]))
 
 
 print("Setup.py is being executed")
 
 setup(
     name='voila-vuetify-thermodynamics',
-    version="0.6.5",
-    description="A vuetify template for Voila",
+    version="0.6.6",
+    description="Voila template used for modeling thermodynamics",
     data_files=data_files,
-    install_requires=['voila>=0.2.0,<0.5', 'jupyter_core'],
+    install_requires=['voila>=0.2.0,<0.5', 'jupyter_core', 'voila-vuetify'],
     include_package_data=True,
-    author='Mario Buikhuizen, Maarten Breddels',
+    author='Lukas Bongartz',
     keywords=[
         'ipython',
         'jupyter',
         'widgets',
         'voila'
     ],
     cmdclass={
```

### Comparing `voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/ansi.js` & `voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/ansi.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/app.html` & `voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/index.html.j2` & `voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/util.js` & `voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/util.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.5/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/app.html` & `voila-vuetify-thermodynamics-0.6.6/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/app.html`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             <v-layout v-show="!loading">
                 <v-navigation-drawer v-model="showNavBar" app>
                     <v-toolbar flat>
                         <v-list>
                             <v-list-item>
                                 <v-list-item-title class="title">
                                     <jupyter-widget-mount-point mount-id="content-title">
-                                        Navigation
+                                        Model Parameter
                                     </jupyter-widget-mount-point>
                                 </v-list-item-title>
                             </v-list-item>
                         </v-list>
                     </v-toolbar>
 
                     <v-divider></v-divider>
@@ -96,14 +96,21 @@
                             </v-btn>
                         </template>
                         <span>Clear messages</span>
                     </v-tooltip>
                 </div>
             </v-sheet>
         </v-menu>
+        <v-footer fixed padless>
+            <v-card flat tile class="flex text-center">
+                <v-card-text class="caption">
+                    © {{ new Date().getFullYear() }} Lukas Bongartz
+                </v-card-text>
+            </v-card>
+        </v-footer>
     </v-app>
 </div>
 
 <script>
 
 var app = new Vue({
     vuetify: new Vuetify({
@@ -125,15 +132,15 @@
                 {icon: "dashboard", title: "voila", url: "https://github.com/voila-dashboards/voila"},
                 {icon: "touch_app", title: "voila-vuetify", url: "https://github.com/voila-dashboards/voila-vuetify"},
                 {icon: "web", title: "ipvuetify", url: "https://github.com/mariobuikhuizen/ipyvuetify"},
                 {icon: "web", title: "vuetify", url: "https://v15.vuetifyjs.com/en/"},
                 {icon: "widgets", title: "jupyter widgets", url: "https://github.com/jupyter-widgets/ipywidgets"},
                 {icon: "bar_chart", title: "bqplot", url: "https://github.com/bloomberg/bqplot/"},
             ],
-            title: 'Voila vuetify',
+            title: 'Bistable OECTs',
             debug: false,
             voilaDebugMessages: [],
         }
     }
 });
 
 </script>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `voila-vuetify-thermodynamics-0.6.5/share/jupyter/voila/templates/vuetify-base-thermodynamics/index.html.j2` & `voila-vuetify-thermodynamics-0.6.6/share/jupyter/voila/templates/vuetify-base-thermodynamics/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.5/voila_vuetify_thermodynamics.egg-info/SOURCES.txt` & `voila-vuetify-thermodynamics-0.6.6/voila_vuetify_thermodynamics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

