# Comparing `tmp/MultiGATE-0.0.5.tar.gz` & `tmp/MultiGATE-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MultiGATE-0.0.5.tar", last modified: Mon Apr  8 10:58:00 2024, max compression
+gzip compressed data, was "dist/MultiGATE-0.0.6.tar", last modified: Mon Apr  8 11:07:27 2024, max compression
```

## Comparing `MultiGATE-0.0.5.tar` & `MultiGATE-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 10:58:00.000000 MultiGATE-0.0.5/
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)    11357 2024-04-07 14:52:50.000000 MultiGATE-0.0.5/LICENSE
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 10:58:00.000000 MultiGATE-0.0.5/MultiGATE/
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 10:58:00.000000 MultiGATE-0.0.5/MultiGATE/MultiGATE.egg-info/
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-08 10:58:00.000000 MultiGATE-0.0.5/MultiGATE/MultiGATE.egg-info/PKG-INFO
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      240 2024-04-08 10:58:00.000000 MultiGATE-0.0.5/MultiGATE/MultiGATE.egg-info/SOURCES.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-08 10:58:00.000000 MultiGATE-0.0.5/MultiGATE/MultiGATE.egg-info/dependency_links.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      305 2024-04-08 10:58:00.000000 MultiGATE-0.0.5/MultiGATE/MultiGATE.egg-info/requires.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-08 10:58:00.000000 MultiGATE-0.0.5/MultiGATE/MultiGATE.egg-info/top_level.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-08 10:58:00.000000 MultiGATE-0.0.5/PKG-INFO
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       16 2024-04-07 14:52:50.000000 MultiGATE-0.0.5/README.md
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       38 2024-04-08 10:58:00.000000 MultiGATE-0.0.5/setup.cfg
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)     1248 2024-04-08 10:57:54.000000 MultiGATE-0.0.5/setup.py
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 11:07:27.000000 MultiGATE-0.0.6/
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)    11357 2024-04-07 14:52:50.000000 MultiGATE-0.0.6/LICENSE
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 11:07:27.000000 MultiGATE-0.0.6/MultiGATE/
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 11:07:27.000000 MultiGATE-0.0.6/MultiGATE/MultiGATE.egg-info/
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-08 11:07:27.000000 MultiGATE-0.0.6/MultiGATE/MultiGATE.egg-info/PKG-INFO
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      240 2024-04-08 11:07:27.000000 MultiGATE-0.0.6/MultiGATE/MultiGATE.egg-info/SOURCES.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-08 11:07:27.000000 MultiGATE-0.0.6/MultiGATE/MultiGATE.egg-info/dependency_links.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      305 2024-04-08 11:07:27.000000 MultiGATE-0.0.6/MultiGATE/MultiGATE.egg-info/requires.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-08 11:07:27.000000 MultiGATE-0.0.6/MultiGATE/MultiGATE.egg-info/top_level.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-08 11:07:27.000000 MultiGATE-0.0.6/PKG-INFO
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       16 2024-04-07 14:52:50.000000 MultiGATE-0.0.6/README.md
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       38 2024-04-08 11:07:27.000000 MultiGATE-0.0.6/setup.cfg
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)     1247 2024-04-08 11:07:25.000000 MultiGATE-0.0.6/setup.py
```

### Comparing `MultiGATE-0.0.5/LICENSE` & `MultiGATE-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MultiGATE-0.0.5/MultiGATE/MultiGATE.egg-info/PKG-INFO` & `MultiGATE-0.0.6/MultiGATE/MultiGATE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGATE
-Version: 0.0.5
+Version: 0.0.6
 Summary: MultiGATE single cell
 Home-page: https://github.com/aqlkzf/MultiGATEtest1
 Author: Jinzhao LI & Jishuai MIAO
 Author-email: jishuaimiao@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `MultiGATE-0.0.5/PKG-INFO` & `MultiGATE-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGATE
-Version: 0.0.5
+Version: 0.0.6
 Summary: MultiGATE single cell
 Home-page: https://github.com/aqlkzf/MultiGATEtest1
 Author: Jinzhao LI & Jishuai MIAO
 Author-email: jishuaimiao@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `MultiGATE-0.0.5/setup.py` & `MultiGATE-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="MultiGATE",
-    version="0.0.5",
+    version="0.0.6",
     description="MultiGATE single cell",
     package_dir={"": "MultiGATE"},
     packages=find_packages(where="MultiGATE"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aqlkzf/MultiGATEtest1",
     author="Jinzhao LI & Jishuai MIAO",
@@ -33,15 +33,15 @@
     'seaborn>=0.12.2',
     'numpy>=1.21.6',
     'scipy>=1.7.3',
     'scanpy>=1.9.3',
     'numpy>=1.21.6',
     'scipy>=1.7.3', 
     'nvidia-ml-py3>=7.352.0', 
-    'gseapy>=1.0.4'  ,
+    'gseapy>=1.0.4' ,
     
 ],
 
 
 
 
     extras_require={
```

