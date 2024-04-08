# Comparing `tmp/fsinfo-0.0.3.tar.gz` & `tmp/fsinfo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsinfo-0.0.3.tar", last modified: Mon Apr  8 02:02:21 2024, max compression
+gzip compressed data, was "fsinfo-0.0.4.tar", last modified: Mon Apr  8 03:48:48 2024, max compression
```

## Comparing `fsinfo-0.0.3.tar` & `fsinfo-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 02:02:21.082212 fsinfo-0.0.3/
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1068 2024-04-07 21:12:40.000000 fsinfo-0.0.3/LICENSE
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1931 2024-04-08 02:02:21.081793 fsinfo-0.0.3/PKG-INFO
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1423 2024-04-08 02:02:14.000000 fsinfo-0.0.3/README.md
-drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 02:02:21.081348 fsinfo-0.0.3/fsinfo.egg-info/
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1931 2024-04-08 02:02:21.000000 fsinfo-0.0.3/fsinfo.egg-info/PKG-INFO
--rw-r--r--   0 kareltutsu   (501) staff       (20)      223 2024-04-08 02:02:21.000000 fsinfo-0.0.3/fsinfo.egg-info/SOURCES.txt
--rw-r--r--   0 kareltutsu   (501) staff       (20)        1 2024-04-08 02:02:21.000000 fsinfo-0.0.3/fsinfo.egg-info/dependency_links.txt
--rw-r--r--   0 kareltutsu   (501) staff       (20)        1 2024-04-08 02:02:21.000000 fsinfo-0.0.3/fsinfo.egg-info/top_level.txt
--rw-r--r--   0 kareltutsu   (501) staff       (20)       38 2024-04-08 02:02:21.082314 fsinfo-0.0.3/setup.cfg
--rw-r--r--   0 kareltutsu   (501) staff       (20)      666 2024-04-08 02:02:18.000000 fsinfo-0.0.3/setup.py
-drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 02:02:21.080581 fsinfo-0.0.3/test/
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1732 2024-04-08 01:32:47.000000 fsinfo-0.0.3/test/test_directoryinfo.py
--rw-r--r--   0 kareltutsu   (501) staff       (20)     3268 2024-04-08 01:32:47.000000 fsinfo-0.0.3/test/test_fileinfo.py
--rw-r--r--   0 kareltutsu   (501) staff       (20)     2185 2024-04-08 01:34:02.000000 fsinfo-0.0.3/test/test_filesysteminfo.py
+drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 03:48:48.257102 fsinfo-0.0.4/
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1068 2024-04-07 21:12:40.000000 fsinfo-0.0.4/LICENSE
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1931 2024-04-08 03:48:48.256672 fsinfo-0.0.4/PKG-INFO
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1423 2024-04-08 02:02:14.000000 fsinfo-0.0.4/README.md
+drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 03:48:48.256106 fsinfo-0.0.4/fsinfo.egg-info/
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1931 2024-04-08 03:48:48.000000 fsinfo-0.0.4/fsinfo.egg-info/PKG-INFO
+-rw-r--r--   0 kareltutsu   (501) staff       (20)      223 2024-04-08 03:48:48.000000 fsinfo-0.0.4/fsinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 kareltutsu   (501) staff       (20)        1 2024-04-08 03:48:48.000000 fsinfo-0.0.4/fsinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 kareltutsu   (501) staff       (20)        1 2024-04-08 03:48:48.000000 fsinfo-0.0.4/fsinfo.egg-info/top_level.txt
+-rw-r--r--   0 kareltutsu   (501) staff       (20)       38 2024-04-08 03:48:48.257211 fsinfo-0.0.4/setup.cfg
+-rw-r--r--   0 kareltutsu   (501) staff       (20)      666 2024-04-08 03:48:40.000000 fsinfo-0.0.4/setup.py
+drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 03:48:48.255117 fsinfo-0.0.4/test/
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1732 2024-04-08 01:32:47.000000 fsinfo-0.0.4/test/test_directoryinfo.py
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     3268 2024-04-08 01:32:47.000000 fsinfo-0.0.4/test/test_fileinfo.py
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     2185 2024-04-08 01:34:02.000000 fsinfo-0.0.4/test/test_filesysteminfo.py
```

### Comparing `fsinfo-0.0.3/LICENSE` & `fsinfo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.3/PKG-INFO` & `fsinfo-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsinfo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library for cross-platform filesystem operations, providing classes for handling files and directories.
 Home-page: https://github.com/KarelOmab/fsinfo
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fsinfo-0.0.3/README.md` & `fsinfo-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.3/fsinfo.egg-info/PKG-INFO` & `fsinfo-0.0.4/fsinfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsinfo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library for cross-platform filesystem operations, providing classes for handling files and directories.
 Home-page: https://github.com/KarelOmab/fsinfo
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fsinfo-0.0.3/setup.py` & `fsinfo-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fsinfo',
-    version='0.0.3',
+    version='0.0.4',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='A Python library for cross-platform filesystem operations, providing classes for handling files and directories.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/fsinfo',
     packages=find_packages(),
```

### Comparing `fsinfo-0.0.3/test/test_directoryinfo.py` & `fsinfo-0.0.4/test/test_directoryinfo.py`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.3/test/test_fileinfo.py` & `fsinfo-0.0.4/test/test_fileinfo.py`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.3/test/test_filesysteminfo.py` & `fsinfo-0.0.4/test/test_filesysteminfo.py`

 * *Files identical despite different names*

