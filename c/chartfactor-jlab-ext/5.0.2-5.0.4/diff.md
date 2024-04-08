# Comparing `tmp/chartfactor-jlab-ext-5.0.2.tar.gz` & `tmp/chartfactor-jlab-ext-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartfactor-jlab-ext-5.0.2.tar", last modified: Tue Mar 26 23:54:35 2024, max compression
+gzip compressed data, was "chartfactor-jlab-ext-5.0.4.tar", last modified: Mon Apr  8 20:27:10 2024, max compression
```

## Comparing `chartfactor-jlab-ext-5.0.2.tar` & `chartfactor-jlab-ext-5.0.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-03-26 23:54:35.777975 chartfactor-jlab-ext-5.0.2/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1506 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.2/LICENSE
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      379 2022-09-08 23:50:12.000000 chartfactor-jlab-ext-5.0.2/MANIFEST.in
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-03-26 23:54:35.777756 chartfactor-jlab-ext-5.0.2/PKG-INFO
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1861 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.2/README.md
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-03-26 23:54:35.773753 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     6148 2023-04-06 16:48:24.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/.DS_Store
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      318 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/__init__.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      441 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/_version.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-03-26 23:54:35.773991 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2342 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/package.json
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-03-26 23:54:35.775711 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    15480 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2669 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      852 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    70526 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      336 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js.LICENSE.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     7251 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     3373 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    85623 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      219 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js.LICENSE.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     7858 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/remoteEntry.e8a0c99a92b003a00b34.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      163 2024-03-26 23:54:33.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/style.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    20796 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-03-26 23:54:35.777560 chartfactor-jlab-ext-5.0.2/chartfactor_jlab_ext.egg-info/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor_jlab_ext.egg-info/PKG-INFO
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1436 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor_jlab_ext.egg-info/SOURCES.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor_jlab_ext.egg-info/dependency_links.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-03-26 23:54:23.000000 chartfactor-jlab-ext-5.0.2/chartfactor_jlab_ext.egg-info/not-zip-safe
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       56 2024-03-26 23:54:35.000000 chartfactor-jlab-ext-5.0.2/chartfactor_jlab_ext.egg-info/top_level.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      201 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.2/install.json
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-03-26 23:54:35.776991 chartfactor-jlab-ext-5.0.2/lib/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     9591 2022-06-24 19:57:03.000000 chartfactor-jlab-ext-5.0.2/lib/cfs.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1675 2022-06-15 14:46:17.000000 chartfactor-jlab-ext-5.0.2/lib/commons.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      877 2022-06-15 14:46:17.000000 chartfactor-jlab-ext-5.0.2/lib/index.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1969 2022-06-17 17:26:57.000000 chartfactor-jlab-ext-5.0.2/lib/model.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      828 2022-05-26 22:15:14.000000 chartfactor-jlab-ext-5.0.2/lib/runner.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2642 2022-05-26 22:15:14.000000 chartfactor-jlab-ext-5.0.2/lib/storage-utils.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2198 2024-03-26 23:53:58.000000 chartfactor-jlab-ext-5.0.2/package.json
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      145 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.2/pyproject.toml
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       38 2024-03-26 23:54:35.778021 chartfactor-jlab-ext-5.0.2/setup.cfg
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2636 2022-09-08 23:50:12.000000 chartfactor-jlab-ext-5.0.2/setup.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-03-26 23:54:35.777399 chartfactor-jlab-ext-5.0.2/style/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.2/style/base.css
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       25 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.2/style/index.css
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       21 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.2/style/index.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)   259094 2022-06-07 13:33:05.000000 chartfactor-jlab-ext-5.0.2/yarn.lock
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-08 20:27:10.806266 chartfactor-jlab-ext-5.0.4/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1506 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.4/LICENSE
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      379 2022-09-08 23:50:12.000000 chartfactor-jlab-ext-5.0.4/MANIFEST.in
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-04-08 20:27:10.806061 chartfactor-jlab-ext-5.0.4/PKG-INFO
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1861 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.4/README.md
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-08 20:27:10.802416 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     6148 2023-04-06 16:48:24.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/.DS_Store
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      318 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/__init__.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      441 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/_version.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-08 20:27:10.802625 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2342 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/package.json
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-08 20:27:10.804090 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    15480 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2669 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      852 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    70526 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      336 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js.LICENSE.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     7251 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/568.96ff9f5e329201a1a978.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     3373 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    85623 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      219 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js.LICENSE.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     7858 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/remoteEntry.2e7960e8888c044d4b7e.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      163 2024-04-08 20:27:08.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/style.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    20796 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-08 20:27:10.805884 chartfactor-jlab-ext-5.0.4/chartfactor_jlab_ext.egg-info/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor_jlab_ext.egg-info/PKG-INFO
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1436 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor_jlab_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor_jlab_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-04-08 20:27:01.000000 chartfactor-jlab-ext-5.0.4/chartfactor_jlab_ext.egg-info/not-zip-safe
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       56 2024-04-08 20:27:10.000000 chartfactor-jlab-ext-5.0.4/chartfactor_jlab_ext.egg-info/top_level.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      201 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.4/install.json
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-08 20:27:10.805345 chartfactor-jlab-ext-5.0.4/lib/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     9591 2022-06-24 19:57:03.000000 chartfactor-jlab-ext-5.0.4/lib/cfs.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1675 2022-06-15 14:46:17.000000 chartfactor-jlab-ext-5.0.4/lib/commons.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      877 2022-06-15 14:46:17.000000 chartfactor-jlab-ext-5.0.4/lib/index.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1969 2022-06-17 17:26:57.000000 chartfactor-jlab-ext-5.0.4/lib/model.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      828 2022-05-26 22:15:14.000000 chartfactor-jlab-ext-5.0.4/lib/runner.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2642 2022-05-26 22:15:14.000000 chartfactor-jlab-ext-5.0.4/lib/storage-utils.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2198 2024-04-08 20:26:51.000000 chartfactor-jlab-ext-5.0.4/package.json
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      145 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.4/pyproject.toml
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       38 2024-04-08 20:27:10.806305 chartfactor-jlab-ext-5.0.4/setup.cfg
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2636 2022-09-08 23:50:12.000000 chartfactor-jlab-ext-5.0.4/setup.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-08 20:27:10.805731 chartfactor-jlab-ext-5.0.4/style/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.4/style/base.css
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       25 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.4/style/index.css
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       21 2022-02-15 22:26:32.000000 chartfactor-jlab-ext-5.0.4/style/index.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)   259094 2022-06-07 13:33:05.000000 chartfactor-jlab-ext-5.0.4/yarn.lock
```

### Comparing `chartfactor-jlab-ext-5.0.2/LICENSE` & `chartfactor-jlab-ext-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/PKG-INFO` & `chartfactor-jlab-ext-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartfactor-jlab-ext
-Version: 5.0.2
+Version: 5.0.4
 Summary: Run chartfactor-py python commands in Jupyter Lab Kernels
 Home-page: https://github.com/Aktiun/chartfactor-jlab-ext
 Author: Aktiun
 Author-email: info@aktiun.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `chartfactor-jlab-ext-5.0.2/README.md` & `chartfactor-jlab-ext-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/.DS_Store` & `chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/.DS_Store`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/package.json` & `chartfactor-jlab-ext-5.0.4/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9649122807017543%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'5.0.4'"}*

```diff
@@ -24,19 +24,14 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/Aktiun/chartfactor-jlab-ext",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.e8a0c99a92b003a00b34.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "chartfactor-jlab-ext/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
@@ -69,9 +64,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
-    "version": "5.0.2"
+    "version": "5.0.4"
 }
```

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js` & `chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js` & `chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt` & `chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js` & `chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js` & `chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/568.96ff9f5e329201a1a978.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunkchartfactor_jlab_ext = self.webpackChunkchartfactor_jlab_ext || []).push([
     [568], {
         774: (e, t, o) => {
             o.d(t, {
                 Z: () => l
             });
-            var s = o(138),
+            var s = o(662),
                 a = o(439);
             const n = function(e, t) {
                     "string" != typeof e && (e = e.toString()), "string" != typeof t && (t = JSON.stringify(t)), localStorage.setItem(e, t)
                 },
                 i = function(e, t) {
                     let o = localStorage.getItem(e);
                     if (null !== o) try {
@@ -188,15 +188,15 @@
                     }
                 }]
         },
         788: (e, t, o) => {
             o.d(t, {
                 Z: () => n
             });
-            var s = o(138);
+            var s = o(662);
             class a {
                 constructor(e) {
                     this._sessionContext = e, this._future = null, this._kernel_id = void 0
                 }
                 future(e, t = null) {
                     this._future = e, e && (e.onIOPub = e => {
                         switch (e.header.msg_type) {
```

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js` & `chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js` & `chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/remoteEntry.e8a0c99a92b003a00b34.js` & `chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/remoteEntry.2e7960e8888c044d4b7e.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -49,24 +49,24 @@
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         100: "7e3a5f4a20c0f69ea729",
         223: "a93208f6436a19e928eb",
         271: "6e361e59632f15ffe513",
         456: "320b2a08bbe0354d4e5c",
         486: "ea74e810f4cf66ad8b28",
-        568: "cb540ea7001c8dafbb5a",
+        568: "96ff9f5e329201a1a978",
         747: "b46981187fdb90cccf38",
         813: "05d4b12c6f2c4f7d9c5b"
     } [e] + ".js?v=" + {
         100: "7e3a5f4a20c0f69ea729",
         223: "a93208f6436a19e928eb",
         271: "6e361e59632f15ffe513",
         456: "320b2a08bbe0354d4e5c",
         486: "ea74e810f4cf66ad8b28",
-        568: "cb540ea7001c8dafbb5a",
+        568: "96ff9f5e329201a1a978",
         747: "b46981187fdb90cccf38",
         813: "05d4b12c6f2c4f7d9c5b"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -120,15 +120,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@phosphor/disposable", "1.10.1", (() => w.e(223).then((() => () => w(223))))), l("chartfactor_jlab_ext", "5.0.2", (() => w.e(568).then((() => () => w(568))))), l("jupyterlab_toastify", "4.2.1", (() => Promise.all([w.e(813), w.e(271)]).then((() => () => w(813))))), l("lodash", "4.17.21", (() => w.e(486).then((() => () => w(486)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@phosphor/disposable", "1.10.1", (() => w.e(223).then((() => () => w(223))))), l("chartfactor_jlab_ext", "5.0.4", (() => w.e(568).then((() => () => w(568))))), l("jupyterlab_toastify", "4.2.1", (() => Promise.all([w.e(813), w.e(271)]).then((() => () => w(813))))), l("lodash", "4.17.21", (() => w.e(486).then((() => () => w(486)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -225,29 +225,29 @@
     }, c = e => (e.loaded = 1, e.get()), h = (s = e => function(r, t, a, n) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, a, n)) : e(r, w.S[r], t, a, n)
     })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), p = s(((e, r, t, a, n) => {
         var o = r && w.o(r, t) && d(r, t, a);
         return o ? c(o) : n()
     })), b = {}, v = {
-        138: () => p("default", "@phosphor/disposable", [1, 1, 3, 1], (() => w.e(223).then((() => () => w(223))))),
         439: () => p("default", "lodash", [1, 4, 17, 21], (() => w.e(486).then((() => () => w(486))))),
         583: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 7]),
+        662: () => p("default", "@phosphor/disposable", [1, 1, 3, 1], (() => w.e(223).then((() => () => w(223))))),
         797: () => p("default", "jupyterlab_toastify", [1, 4, 2, 1], (() => Promise.all([w.e(813), w.e(271)]).then((() => () => w(813))))),
         854: () => h("default", "@jupyterlab/notebook", [1, 3, 6, 7]),
         953: () => h("default", "@jupyterlab/rendermime", [1, 3, 6, 7]),
         840: () => h("default", "@lumino/signaling", [1, 1, 10, 0]),
         918: () => h("default", "@lumino/algorithm", [1, 1, 9, 0]),
         271: () => h("default", "react", [1, 17, 0, 1]),
         456: () => h("default", "react-dom", [1, 17, 0, 1])
     }, m = {
         223: [840, 918],
         271: [271],
         456: [456],
-        568: [138, 439, 583, 797, 854, 953]
+        568: [439, 583, 662, 797, 854, 953]
     }, w.f.consumes = (e, r) => {
         w.o(m, e) && m[e].forEach((e => {
             if (w.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
```

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor-jlab-ext/labextension/static/third-party-licenses.json` & `chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor_jlab_ext.egg-info/PKG-INFO` & `chartfactor-jlab-ext-5.0.4/chartfactor_jlab_ext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartfactor-jlab-ext
-Version: 5.0.2
+Version: 5.0.4
 Summary: Run chartfactor-py python commands in Jupyter Lab Kernels
 Home-page: https://github.com/Aktiun/chartfactor-jlab-ext
 Author: Aktiun
 Author-email: info@aktiun.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `chartfactor-jlab-ext-5.0.2/chartfactor_jlab_ext.egg-info/SOURCES.txt` & `chartfactor-jlab-ext-5.0.4/chartfactor_jlab_ext.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 chartfactor-jlab-ext/_version.py
 chartfactor-jlab-ext/labextension/package.json
 chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js
 chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js
 chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt
 chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js
 chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js.LICENSE.txt
-chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js
+chartfactor-jlab-ext/labextension/static/568.96ff9f5e329201a1a978.js
 chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js
 chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js
 chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js.LICENSE.txt
-chartfactor-jlab-ext/labextension/static/remoteEntry.e8a0c99a92b003a00b34.js
+chartfactor-jlab-ext/labextension/static/remoteEntry.2e7960e8888c044d4b7e.js
 chartfactor-jlab-ext/labextension/static/style.js
 chartfactor-jlab-ext/labextension/static/third-party-licenses.json
 chartfactor_jlab_ext.egg-info/PKG-INFO
 chartfactor_jlab_ext.egg-info/SOURCES.txt
 chartfactor_jlab_ext.egg-info/dependency_links.txt
 chartfactor_jlab_ext.egg-info/not-zip-safe
 chartfactor_jlab_ext.egg-info/top_level.txt
```

### Comparing `chartfactor-jlab-ext-5.0.2/lib/cfs.js` & `chartfactor-jlab-ext-5.0.4/lib/cfs.js`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/lib/commons.js` & `chartfactor-jlab-ext-5.0.4/lib/commons.js`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/lib/index.js` & `chartfactor-jlab-ext-5.0.4/lib/index.js`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/lib/model.js` & `chartfactor-jlab-ext-5.0.4/lib/model.js`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/lib/runner.js` & `chartfactor-jlab-ext-5.0.4/lib/runner.js`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/lib/storage-utils.js` & `chartfactor-jlab-ext-5.0.4/lib/storage-utils.js`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/package.json` & `chartfactor-jlab-ext-5.0.4/chartfactor-jlab-ext/labextension/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9649122807017543%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.2e7960e8888c044d4b7e.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'5.0.4'"}*

```diff
@@ -24,14 +24,19 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/Aktiun/chartfactor-jlab-ext",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.2e7960e8888c044d4b7e.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "chartfactor-jlab-ext/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
@@ -64,9 +69,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
-    "version": "5.0.2"
+    "version": "5.0.4"
 }
```

### Comparing `chartfactor-jlab-ext-5.0.2/setup.py` & `chartfactor-jlab-ext-5.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `chartfactor-jlab-ext-5.0.2/yarn.lock` & `chartfactor-jlab-ext-5.0.4/yarn.lock`

 * *Files identical despite different names*

