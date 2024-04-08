# Comparing `tmp/fsinfo-0.0.6.tar.gz` & `tmp/fsinfo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsinfo-0.0.6.tar", last modified: Mon Apr  8 03:56:29 2024, max compression
+gzip compressed data, was "fsinfo-0.0.7.tar", last modified: Mon Apr  8 03:58:27 2024, max compression
```

## Comparing `fsinfo-0.0.6.tar` & `fsinfo-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 03:56:29.727183 fsinfo-0.0.6/
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1068 2024-04-07 21:12:40.000000 fsinfo-0.0.6/LICENSE
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1931 2024-04-08 03:56:29.726783 fsinfo-0.0.6/PKG-INFO
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1423 2024-04-08 02:02:14.000000 fsinfo-0.0.6/README.md
-drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 03:56:29.722869 fsinfo-0.0.6/fsinfo/
--rw-r--r--   0 kareltutsu   (501) staff       (20)      196 2024-04-08 03:56:20.000000 fsinfo-0.0.6/fsinfo/__init__.py
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1035 2024-04-08 03:34:18.000000 fsinfo-0.0.6/fsinfo/directoryinfo.py
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1391 2024-04-08 02:01:50.000000 fsinfo-0.0.6/fsinfo/fileinfo.py
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1301 2024-04-08 01:32:47.000000 fsinfo-0.0.6/fsinfo/filesysteminfo.py
-drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 03:56:29.726358 fsinfo-0.0.6/fsinfo.egg-info/
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1931 2024-04-08 03:56:29.000000 fsinfo-0.0.6/fsinfo.egg-info/PKG-INFO
--rw-r--r--   0 kareltutsu   (501) staff       (20)      310 2024-04-08 03:56:29.000000 fsinfo-0.0.6/fsinfo.egg-info/SOURCES.txt
--rw-r--r--   0 kareltutsu   (501) staff       (20)        1 2024-04-08 03:56:29.000000 fsinfo-0.0.6/fsinfo.egg-info/dependency_links.txt
--rw-r--r--   0 kareltutsu   (501) staff       (20)        7 2024-04-08 03:56:29.000000 fsinfo-0.0.6/fsinfo.egg-info/top_level.txt
--rw-r--r--   0 kareltutsu   (501) staff       (20)       38 2024-04-08 03:56:29.727277 fsinfo-0.0.6/setup.cfg
--rw-r--r--   0 kareltutsu   (501) staff       (20)      666 2024-04-08 03:56:23.000000 fsinfo-0.0.6/setup.py
-drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 03:56:29.725958 fsinfo-0.0.6/test/
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1732 2024-04-08 01:32:47.000000 fsinfo-0.0.6/test/test_directoryinfo.py
--rw-r--r--   0 kareltutsu   (501) staff       (20)     3268 2024-04-08 01:32:47.000000 fsinfo-0.0.6/test/test_fileinfo.py
--rw-r--r--   0 kareltutsu   (501) staff       (20)     2185 2024-04-08 01:34:02.000000 fsinfo-0.0.6/test/test_filesysteminfo.py
+drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 03:58:27.509728 fsinfo-0.0.7/
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1068 2024-04-07 21:12:40.000000 fsinfo-0.0.7/LICENSE
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1931 2024-04-08 03:58:27.509200 fsinfo-0.0.7/PKG-INFO
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1423 2024-04-08 02:02:14.000000 fsinfo-0.0.7/README.md
+drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 03:58:27.506045 fsinfo-0.0.7/fsinfo/
+-rw-r--r--   0 kareltutsu   (501) staff       (20)      196 2024-04-08 03:56:20.000000 fsinfo-0.0.7/fsinfo/__init__.py
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1037 2024-04-08 03:58:13.000000 fsinfo-0.0.7/fsinfo/directoryinfo.py
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1392 2024-04-08 03:58:16.000000 fsinfo-0.0.7/fsinfo/fileinfo.py
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1301 2024-04-08 03:58:17.000000 fsinfo-0.0.7/fsinfo/filesysteminfo.py
+drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 03:58:27.508769 fsinfo-0.0.7/fsinfo.egg-info/
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1931 2024-04-08 03:58:27.000000 fsinfo-0.0.7/fsinfo.egg-info/PKG-INFO
+-rw-r--r--   0 kareltutsu   (501) staff       (20)      310 2024-04-08 03:58:27.000000 fsinfo-0.0.7/fsinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 kareltutsu   (501) staff       (20)        1 2024-04-08 03:58:27.000000 fsinfo-0.0.7/fsinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 kareltutsu   (501) staff       (20)        7 2024-04-08 03:58:27.000000 fsinfo-0.0.7/fsinfo.egg-info/top_level.txt
+-rw-r--r--   0 kareltutsu   (501) staff       (20)       38 2024-04-08 03:58:27.509843 fsinfo-0.0.7/setup.cfg
+-rw-r--r--   0 kareltutsu   (501) staff       (20)      666 2024-04-08 03:58:25.000000 fsinfo-0.0.7/setup.py
+drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 03:58:27.508379 fsinfo-0.0.7/test/
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1732 2024-04-08 01:32:47.000000 fsinfo-0.0.7/test/test_directoryinfo.py
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     3268 2024-04-08 01:32:47.000000 fsinfo-0.0.7/test/test_fileinfo.py
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     2185 2024-04-08 01:34:02.000000 fsinfo-0.0.7/test/test_filesysteminfo.py
```

### Comparing `fsinfo-0.0.6/LICENSE` & `fsinfo-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.6/PKG-INFO` & `fsinfo-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsinfo
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for cross-platform filesystem operations, providing classes for handling files and directories.
 Home-page: https://github.com/KarelOmab/fsinfo
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fsinfo-0.0.6/README.md` & `fsinfo-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.6/fsinfo/directoryinfo.py` & `fsinfo-0.0.7/fsinfo/directoryinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from filesysteminfo import FileSystemInfo
-from fileinfo import FileInfo
+from .filesysteminfo import FileSystemInfo
+from .fileinfo import FileInfo
 import os
 import shutil
 from pathlib import Path
 
 class DirectoryInfo(FileSystemInfo):
     def __init__(self, path):
         super().__init__(path)
```

### Comparing `fsinfo-0.0.6/fsinfo/fileinfo.py` & `fsinfo-0.0.7/fsinfo/fileinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from filesysteminfo import FileSystemInfo
+from .filesysteminfo import FileSystemInfo
 from pathlib import Path
 import shutil
 
 class FileInfo(FileSystemInfo):
     def __init__(self, path):
         super().__init__(path)
```

### Comparing `fsinfo-0.0.6/fsinfo/filesysteminfo.py` & `fsinfo-0.0.7/fsinfo/filesysteminfo.py`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.6/fsinfo.egg-info/PKG-INFO` & `fsinfo-0.0.7/fsinfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsinfo
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for cross-platform filesystem operations, providing classes for handling files and directories.
 Home-page: https://github.com/KarelOmab/fsinfo
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fsinfo-0.0.6/setup.py` & `fsinfo-0.0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fsinfo',
-    version='0.0.6',
+    version='0.0.7',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='A Python library for cross-platform filesystem operations, providing classes for handling files and directories.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/fsinfo',
     packages=find_packages(),
```

### Comparing `fsinfo-0.0.6/test/test_directoryinfo.py` & `fsinfo-0.0.7/test/test_directoryinfo.py`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.6/test/test_fileinfo.py` & `fsinfo-0.0.7/test/test_fileinfo.py`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.6/test/test_filesysteminfo.py` & `fsinfo-0.0.7/test/test_filesysteminfo.py`

 * *Files identical despite different names*

