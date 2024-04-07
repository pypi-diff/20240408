# Comparing `tmp/connectome_interpreter-1.0.2.tar.gz` & `tmp/connectome_interpreter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.0.2.tar", last modified: Sun Mar 31 16:47:11 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.1.0.tar", last modified: Sun Apr  7 22:16:08 2024, max compression
```

## Comparing `connectome_interpreter-1.0.2.tar` & `connectome_interpreter-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 16:47:11.502743 connectome_interpreter-1.0.2/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      913 2024-03-31 16:47:11.501746 connectome_interpreter-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      467 2024-03-04 09:40:07.000000 connectome_interpreter-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 16:47:11.497759 connectome_interpreter-1.0.2/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.0.2/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    15178 2024-03-31 15:48:26.000000 connectome_interpreter-1.0.2/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    18051 2024-03-20 19:23:39.000000 connectome_interpreter-1.0.2/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0     7634 2024-03-20 15:39:57.000000 connectome_interpreter-1.0.2/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    17919 2024-03-31 16:43:03.000000 connectome_interpreter-1.0.2/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:47:11.500749 connectome_interpreter-1.0.2/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0      913 2024-03-31 16:47:11.000000 connectome_interpreter-1.0.2/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-03-31 16:47:11.000000 connectome_interpreter-1.0.2/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 16:47:11.000000 connectome_interpreter-1.0.2/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2024-03-31 16:47:11.000000 connectome_interpreter-1.0.2/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-03-31 16:47:11.000000 connectome_interpreter-1.0.2/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 16:47:11.502743 connectome_interpreter-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1511 2024-03-31 16:44:27.000000 connectome_interpreter-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:47:11.500749 connectome_interpreter-1.0.2/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 22:16:08.026905 connectome_interpreter-1.1.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      913 2024-04-07 22:16:08.026905 connectome_interpreter-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2024-03-04 09:40:07.000000 connectome_interpreter-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 22:16:07.991096 connectome_interpreter-1.1.0/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.1.0/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    15178 2024-04-02 10:49:52.000000 connectome_interpreter-1.1.0/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    18051 2024-03-20 19:23:39.000000 connectome_interpreter-1.1.0/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    13084 2024-04-07 22:13:37.000000 connectome_interpreter-1.1.0/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    17919 2024-03-31 16:43:03.000000 connectome_interpreter-1.1.0/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 22:16:08.023742 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0      913 2024-04-07 22:16:07.000000 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-04-07 22:16:07.000000 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 22:16:07.000000 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2024-04-07 22:16:07.000000 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-07 22:16:07.000000 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 22:16:08.026905 connectome_interpreter-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1511 2024-04-07 22:12:25.000000 connectome_interpreter-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 22:16:08.024736 connectome_interpreter-1.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.1.0/tests/__init__.py
```

### Comparing `connectome_interpreter-1.0.2/LICENSE` & `connectome_interpreter-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.0.2/PKG-INFO` & `connectome_interpreter-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome_interpreter
-Version: 1.0.2
+Version: 1.1.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
```

### Comparing `connectome_interpreter-1.0.2/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.1.0/connectome_interpreter/activation_maximisation.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.0.2/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.1.0/connectome_interpreter/compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.0.2/connectome_interpreter/utils.py` & `connectome_interpreter-1.1.0/connectome_interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.0.2/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.1.0/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome-interpreter
-Version: 1.0.2
+Version: 1.1.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
```

### Comparing `connectome_interpreter-1.0.2/setup.py` & `connectome_interpreter-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.0.2',
+    version='1.1.0',
     packages=find_packages(),
     install_requires=[
         # List your package dependencies here
         'numpy',
         'pandas',
         'scipy',
         'torch',
```

