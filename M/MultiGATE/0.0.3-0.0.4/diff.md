# Comparing `tmp/MultiGATE-0.0.3.tar.gz` & `tmp/MultiGATE-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MultiGATE-0.0.3.tar", last modified: Sun Apr  7 15:45:07 2024, max compression
+gzip compressed data, was "dist/MultiGATE-0.0.4.tar", last modified: Mon Apr  8 10:52:44 2024, max compression
```

## Comparing `MultiGATE-0.0.3.tar` & `MultiGATE-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-07 15:45:07.000000 MultiGATE-0.0.3/
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)    11357 2024-04-07 14:52:50.000000 MultiGATE-0.0.3/LICENSE
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-07 15:45:07.000000 MultiGATE-0.0.3/MultiGATE/
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-07 15:45:07.000000 MultiGATE-0.0.3/MultiGATE/MultiGATE.egg-info/
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-07 15:45:07.000000 MultiGATE-0.0.3/MultiGATE/MultiGATE.egg-info/PKG-INFO
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      240 2024-04-07 15:45:07.000000 MultiGATE-0.0.3/MultiGATE/MultiGATE.egg-info/SOURCES.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-07 15:45:07.000000 MultiGATE-0.0.3/MultiGATE/MultiGATE.egg-info/dependency_links.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      144 2024-04-07 15:45:07.000000 MultiGATE-0.0.3/MultiGATE/MultiGATE.egg-info/requires.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-07 15:45:07.000000 MultiGATE-0.0.3/MultiGATE/MultiGATE.egg-info/top_level.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-07 15:45:07.000000 MultiGATE-0.0.3/PKG-INFO
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       16 2024-04-07 14:52:50.000000 MultiGATE-0.0.3/README.md
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       38 2024-04-07 15:45:07.000000 MultiGATE-0.0.3/setup.cfg
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)     1036 2024-04-07 15:45:05.000000 MultiGATE-0.0.3/setup.py
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 10:52:44.000000 MultiGATE-0.0.4/
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)    11357 2024-04-07 14:52:50.000000 MultiGATE-0.0.4/LICENSE
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 10:52:44.000000 MultiGATE-0.0.4/MultiGATE/
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 10:52:44.000000 MultiGATE-0.0.4/MultiGATE/MultiGATE.egg-info/
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-08 10:52:44.000000 MultiGATE-0.0.4/MultiGATE/MultiGATE.egg-info/PKG-INFO
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      240 2024-04-08 10:52:44.000000 MultiGATE-0.0.4/MultiGATE/MultiGATE.egg-info/SOURCES.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-08 10:52:44.000000 MultiGATE-0.0.4/MultiGATE/MultiGATE.egg-info/dependency_links.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      305 2024-04-08 10:52:44.000000 MultiGATE-0.0.4/MultiGATE/MultiGATE.egg-info/requires.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-08 10:52:44.000000 MultiGATE-0.0.4/MultiGATE/MultiGATE.egg-info/top_level.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-08 10:52:44.000000 MultiGATE-0.0.4/PKG-INFO
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       16 2024-04-07 14:52:50.000000 MultiGATE-0.0.4/README.md
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       38 2024-04-08 10:52:44.000000 MultiGATE-0.0.4/setup.cfg
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)     1248 2024-04-08 10:52:03.000000 MultiGATE-0.0.4/setup.py
```

### Comparing `MultiGATE-0.0.3/LICENSE` & `MultiGATE-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MultiGATE-0.0.3/MultiGATE/MultiGATE.egg-info/PKG-INFO` & `MultiGATE-0.0.4/MultiGATE/MultiGATE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGATE
-Version: 0.0.3
+Version: 0.0.4
 Summary: MultiGATE single cell
 Home-page: https://github.com/aqlkzf/MultiGATEtest1
 Author: Jinzhao LI & Jishuai MIAO
 Author-email: jishuaimiao@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `MultiGATE-0.0.3/PKG-INFO` & `MultiGATE-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGATE
-Version: 0.0.3
+Version: 0.0.4
 Summary: MultiGATE single cell
 Home-page: https://github.com/aqlkzf/MultiGATEtest1
 Author: Jinzhao LI & Jishuai MIAO
 Author-email: jishuaimiao@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `MultiGATE-0.0.3/setup.py` & `MultiGATE-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="MultiGATE",
-    version="0.0.3",
+    version="0.0.4",
     description="MultiGATE single cell",
     package_dir={"": "MultiGATE"},
     packages=find_packages(where="MultiGATE"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aqlkzf/MultiGATEtest1",
     author="Jinzhao LI & Jishuai MIAO",
@@ -18,24 +18,34 @@
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Operating System :: OS Independent",
     ],
    install_requires=[
     'tensorflow-gpu==1.15.0',
-    'scikit-learn',
-    'pandas',
-    'scanpy',
-    'jupyterlab',
-    'tqdm',
-    'matplotlib',
-    'networkx',
-    'pybedtools',
-    'seaborn',
-    'scanpy'    
+    'scikit-learn>=1.0.2',
+    'pandas>=1.3.5',
+    'scanpy>=1.9.3',
+    'jupyterlab>=3.6.7',
+    'tqdm>=4.66.2',
+    'matplotlib>=3.5.3',
+    'networkx>=2.7',
+    'pybedtools>=0.9.0',
+    'seaborn>=0.12.2',
+    'numpy>=1.21.6',
+    'scipy>=1.7.3',
+    'scanpy>=1.9.3',
+    'numpy>=1.21.6',
+    'scipy>=1.7.3', 
+    'nvidia-ml-py3>=7.352.0', 
+    'gseapy>=1.0.4'  ,
+    
 ],
 
+
+
+
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
     python_requires="==3.7.*",
 )
```

