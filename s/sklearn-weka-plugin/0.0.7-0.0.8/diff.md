# Comparing `tmp/sklearn-weka-plugin-0.0.7.tar.gz` & `tmp/sklearn-weka-plugin-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn-weka-plugin-0.0.7.tar", last modified: Thu Jul  6 20:57:40 2023, max compression
+gzip compressed data, was "sklearn-weka-plugin-0.0.8.tar", last modified: Sun Apr  7 23:02:12 2024, max compression
```

## Comparing `sklearn-weka-plugin-0.0.7.tar` & `sklearn-weka-plugin-0.0.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.796982 sklearn-weka-plugin-0.0.7/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      685 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/.gitignore
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2429 2023-07-06 20:55:03.000000 sklearn-weka-plugin-0.0.7/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      367 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    35149 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/LICENSE
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3441 2023-07-06 20:57:40.796982 sklearn-weka-plugin-0.0.7/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5003 2022-01-09 22:03:06.000000 sklearn-weka-plugin-0.0.7/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1085 2022-03-31 22:30:00.000000 sklearn-weka-plugin-0.0.7/RELEASE.md
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.792982 sklearn-weka-plugin-0.0.7/doc/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6835 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/Makefile
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6494 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/make.bat
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.792982 sklearn-weka-plugin-0.0.7/doc/source/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.792982 sklearn-weka-plugin-0.0.7/doc/source/_static/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    17064 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/_static/logo.jpg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6763 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/_static/logo.pdf
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6017 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/_static/logo.png
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3236 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/_static/logo.svg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8474 2023-07-06 20:55:03.000000 sklearn-weka-plugin-0.0.7/doc/source/conf.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6513 2022-03-31 22:18:00.000000 sklearn-weka-plugin-0.0.7/doc/source/examples.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1165 2021-12-17 03:59:39.000000 sklearn-weka-plugin-0.0.7/doc/source/index.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      768 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/install.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       52 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/modules.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      621 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/sklweka.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       81 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/requirements.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-07-06 20:57:40.796982 sklearn-weka-plugin-0.0.7/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1173 2023-07-06 20:55:03.000000 sklearn-weka-plugin-0.0.7/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.792982 sklearn-weka-plugin-0.0.7/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.796982 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3441 2023-07-06 20:57:40.000000 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      810 2023-07-06 20:57:40.000000 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-07-06 20:57:40.000000 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       42 2023-07-06 20:57:40.000000 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        8 2023-07-06 20:57:40.000000 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.796982 sklearn-weka-plugin-0.0.7/src/sklweka/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/src/sklweka/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    11541 2023-07-06 20:41:56.000000 sklearn-weka-plugin-0.0.7/src/sklweka/classifiers.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8229 2023-06-19 21:09:04.000000 sklearn-weka-plugin-0.0.7/src/sklweka/clusters.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1631 2021-10-31 20:00:50.000000 sklearn-weka-plugin-0.0.7/src/sklweka/datagenerators.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    15246 2023-07-06 20:51:41.000000 sklearn-weka-plugin-0.0.7/src/sklweka/dataset.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       28 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/src/sklweka/jvm.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       33 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/src/sklweka/packages.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    13140 2023-06-19 20:45:11.000000 sklearn-weka-plugin-0.0.7/src/sklweka/preprocessing.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-04-07 23:02:11.995016 sklearn-weka-plugin-0.0.8/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      685 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/.gitignore
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2613 2024-04-07 23:01:28.000000 sklearn-weka-plugin-0.0.8/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      367 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    35149 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/LICENSE
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3625 2024-04-07 23:02:11.995016 sklearn-weka-plugin-0.0.8/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5140 2023-07-06 21:11:13.000000 sklearn-weka-plugin-0.0.8/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1085 2022-03-31 22:30:00.000000 sklearn-weka-plugin-0.0.8/RELEASE.md
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-04-07 23:02:11.995016 sklearn-weka-plugin-0.0.8/doc/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6835 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/doc/Makefile
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6494 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/doc/make.bat
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-04-07 23:02:11.995016 sklearn-weka-plugin-0.0.8/doc/source/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-04-07 23:02:11.995016 sklearn-weka-plugin-0.0.8/doc/source/_static/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    17064 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/doc/source/_static/logo.jpg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6763 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/doc/source/_static/logo.pdf
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6017 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/doc/source/_static/logo.png
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3236 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/doc/source/_static/logo.svg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8474 2024-04-07 23:01:28.000000 sklearn-weka-plugin-0.0.8/doc/source/conf.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6513 2022-03-31 22:18:00.000000 sklearn-weka-plugin-0.0.8/doc/source/examples.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1176 2023-07-06 21:06:15.000000 sklearn-weka-plugin-0.0.8/doc/source/index.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      768 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/doc/source/install.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       52 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/doc/source/modules.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      621 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/doc/source/sklweka.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       81 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/requirements.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-04-07 23:02:11.995016 sklearn-weka-plugin-0.0.8/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1178 2024-04-07 23:01:28.000000 sklearn-weka-plugin-0.0.8/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-04-07 23:02:11.991016 sklearn-weka-plugin-0.0.8/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-04-07 23:02:11.995016 sklearn-weka-plugin-0.0.8/src/sklearn_weka_plugin.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3625 2024-04-07 23:02:11.000000 sklearn-weka-plugin-0.0.8/src/sklearn_weka_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      810 2024-04-07 23:02:11.000000 sklearn-weka-plugin-0.0.8/src/sklearn_weka_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-04-07 23:02:11.000000 sklearn-weka-plugin-0.0.8/src/sklearn_weka_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       47 2024-04-07 23:02:11.000000 sklearn-weka-plugin-0.0.8/src/sklearn_weka_plugin.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        8 2024-04-07 23:02:11.000000 sklearn-weka-plugin-0.0.8/src/sklearn_weka_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-04-07 23:02:11.995016 sklearn-weka-plugin-0.0.8/src/sklweka/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/src/sklweka/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    11541 2023-07-06 20:41:56.000000 sklearn-weka-plugin-0.0.8/src/sklweka/classifiers.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8229 2023-06-19 21:09:04.000000 sklearn-weka-plugin-0.0.8/src/sklweka/clusters.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1631 2021-10-31 20:00:50.000000 sklearn-weka-plugin-0.0.8/src/sklweka/datagenerators.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    15246 2023-07-06 20:51:41.000000 sklearn-weka-plugin-0.0.8/src/sklweka/dataset.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       28 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/src/sklweka/jvm.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       33 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.8/src/sklweka/packages.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    13140 2023-06-19 20:45:11.000000 sklearn-weka-plugin-0.0.8/src/sklweka/preprocessing.py
```

### Comparing `sklearn-weka-plugin-0.0.7/.gitignore` & `sklearn-weka-plugin-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/CHANGES.rst` & `sklearn-weka-plugin-0.0.8/CHANGES.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+0.0.8 (2024-04-08)
+------------------
+
+- using `scikit-learn` instead of deprecated `sklearn` dependency for scikit-learn
+  (https://github.com/fracpete/sklearn-weka-plugin/pull/10)
+
+
 0.0.7 (2023-07-07)
 ------------------
 
 - `WekaEstimator` (module `sklweka.classifiers`) now has a custom `score` method that
   distinguishes between classification and regression to return the correct score.
 - renamed `data` to `X` and `targets` to `y`, since some sklearn schemes use named arguments
 - added dummy argument `sample_weight=None` to `fit`, `score` and `fit_predict` methods
```

### Comparing `sklearn-weka-plugin-0.0.7/LICENSE` & `sklearn-weka-plugin-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/PKG-INFO` & `sklearn-weka-plugin-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-weka-plugin
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library for making Weka algorithms available within scikit-learn. Relies on the python-weka-wrapper3 library.
 Home-page: https://github.com/fracpete/sklearn-weka-plugin
 Author: Peter "fracpete" Reutemann
 Author-email: sklweka@fracpete.org
 License: GNU General Public License version 3.0 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,21 @@
 Examples can be found at:
 
 https://github.com/fracpete/sklearn-weka-plugin-examples
 
 Changelog
 =========
 
+0.0.8 (2024-04-08)
+------------------
+
+- using `scikit-learn` instead of deprecated `sklearn` dependency for scikit-learn
+  (https://github.com/fracpete/sklearn-weka-plugin/pull/10)
+
+
 0.0.7 (2023-07-07)
 ------------------
 
 - `WekaEstimator` (module `sklweka.classifiers`) now has a custom `score` method that
   distinguishes between classification and regression to return the correct score.
 - renamed `data` to `X` and `targets` to `y`, since some sklearn schemes use named arguments
 - added dummy argument `sample_weight=None` to `fit`, `score` and `fit_predict` methods
```

### Comparing `sklearn-weka-plugin-0.0.7/README.md` & `sklearn-weka-plugin-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 Built on top of the [python-weka-wrapper3](https://github.com/fracpete/python-weka-wrapper3) 
 library, it uses the [python-javabridge](https://pypi.python.org/pypi/python-javabridge) library
 under the hood for communicating with Weka objects in the Java Virtual Machine.
 
 
 ## Functionality
 
-Currently available:
+The following is currently available:
 
 * Classifiers (classification/regression)
 * Clusters
 * Filters
 
 Things to be aware of:
 
 * You need to start the JVM in your Python code before you can use Weka (and stop it again).
 * Unlikely to work in multi-threaded/process environments (like flask).
 * Jupyter Notebooks do not play nice with python-javabridge, as you might have to restart the kernel in order to be able 
   to restart the JVM (e.g., with additional packages).
 * The conversion to Weka data structures involves guesswork, i.e., if targets are to be treated as nominal, you need 
   to convert the numeric values to strings (e.g., using `to_nominal_labels` and/or `to_nominal_attributes` functions 
   from `sklweka.dataset` or the `MakeNominal` transformer from `sklweka.preprocessing`).
+* Check the [list of known problems](https://fracpete.github.io/sklearn-weka-plugin/gotchas.html) before reporting one.
 
 
 ## Requirements
 
 The library has the following requirements:
 
 * Python 3 (does not work with Python 2)
```

### Comparing `sklearn-weka-plugin-0.0.7/RELEASE.md` & `sklearn-weka-plugin-0.0.8/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/doc/Makefile` & `sklearn-weka-plugin-0.0.8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/doc/make.bat` & `sklearn-weka-plugin-0.0.8/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/doc/source/_static/logo.jpg` & `sklearn-weka-plugin-0.0.8/doc/source/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/doc/source/_static/logo.pdf` & `sklearn-weka-plugin-0.0.8/doc/source/_static/logo.pdf`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/doc/source/_static/logo.png` & `sklearn-weka-plugin-0.0.8/doc/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/doc/source/_static/logo.svg` & `sklearn-weka-plugin-0.0.8/doc/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/doc/source/conf.py` & `sklearn-weka-plugin-0.0.8/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,17 @@
 copyright = u'2021-2023, Peter "fracpete" Reutemann'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.0.7'
+version = '0.0.8'
 # The full version, including alpha/beta/rc tags.
-release = '0.0.7'
+release = '0.0.8'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `sklearn-weka-plugin-0.0.7/doc/source/examples.rst` & `sklearn-weka-plugin-0.0.8/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/doc/source/index.rst` & `sklearn-weka-plugin-0.0.8/doc/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 ========
 
 .. toctree::
    :maxdepth: 2
 
    install
    examples
+   gotchas
 
 API
 ===
 
 .. toctree::
    :maxdepth: 4
```

### Comparing `sklearn-weka-plugin-0.0.7/doc/source/install.rst` & `sklearn-weka-plugin-0.0.8/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/doc/source/sklweka.rst` & `sklearn-weka-plugin-0.0.8/doc/source/sklweka.rst`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/setup.py` & `sklearn-weka-plugin-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     license='GNU General Public License version 3.0 (GPLv3)',
     package_dir={
         '': 'src'
     },
     packages=[
         "sklweka",
     ],
-    version="0.0.7",
+    version="0.0.8",
     author='Peter "fracpete" Reutemann',
     author_email='sklweka@fracpete.org',
     install_requires=[
         "numpy",
         "python-weka-wrapper3>=0.2.5",
-        "sklearn",
+        "scikit-learn",
     ],
 )
```

### Comparing `sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/PKG-INFO` & `sklearn-weka-plugin-0.0.8/src/sklearn_weka_plugin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-weka-plugin
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library for making Weka algorithms available within scikit-learn. Relies on the python-weka-wrapper3 library.
 Home-page: https://github.com/fracpete/sklearn-weka-plugin
 Author: Peter "fracpete" Reutemann
 Author-email: sklweka@fracpete.org
 License: GNU General Public License version 3.0 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,21 @@
 Examples can be found at:
 
 https://github.com/fracpete/sklearn-weka-plugin-examples
 
 Changelog
 =========
 
+0.0.8 (2024-04-08)
+------------------
+
+- using `scikit-learn` instead of deprecated `sklearn` dependency for scikit-learn
+  (https://github.com/fracpete/sklearn-weka-plugin/pull/10)
+
+
 0.0.7 (2023-07-07)
 ------------------
 
 - `WekaEstimator` (module `sklweka.classifiers`) now has a custom `score` method that
   distinguishes between classification and regression to return the correct score.
 - renamed `data` to `X` and `targets` to `y`, since some sklearn schemes use named arguments
 - added dummy argument `sample_weight=None` to `fit`, `score` and `fit_predict` methods
```

### Comparing `sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/SOURCES.txt` & `sklearn-weka-plugin-0.0.8/src/sklearn_weka_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/src/sklweka/classifiers.py` & `sklearn-weka-plugin-0.0.8/src/sklweka/classifiers.py`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/src/sklweka/clusters.py` & `sklearn-weka-plugin-0.0.8/src/sklweka/clusters.py`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/src/sklweka/datagenerators.py` & `sklearn-weka-plugin-0.0.8/src/sklweka/datagenerators.py`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/src/sklweka/dataset.py` & `sklearn-weka-plugin-0.0.8/src/sklweka/dataset.py`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.7/src/sklweka/preprocessing.py` & `sklearn-weka-plugin-0.0.8/src/sklweka/preprocessing.py`

 * *Files identical despite different names*

