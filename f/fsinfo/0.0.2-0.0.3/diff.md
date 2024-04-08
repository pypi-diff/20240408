# Comparing `tmp/fsinfo-0.0.2.tar.gz` & `tmp/fsinfo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsinfo-0.0.2.tar", last modified: Mon Apr  8 02:01:24 2024, max compression
+gzip compressed data, was "fsinfo-0.0.3.tar", last modified: Mon Apr  8 02:02:21 2024, max compression
```

## Comparing `fsinfo-0.0.2.tar` & `fsinfo-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 02:01:24.124007 fsinfo-0.0.2/
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1068 2024-04-07 21:12:40.000000 fsinfo-0.0.2/LICENSE
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1930 2024-04-08 02:01:24.123442 fsinfo-0.0.2/PKG-INFO
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1422 2024-04-08 01:59:36.000000 fsinfo-0.0.2/README.md
-drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 02:01:24.122888 fsinfo-0.0.2/fsinfo.egg-info/
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1930 2024-04-08 02:01:24.000000 fsinfo-0.0.2/fsinfo.egg-info/PKG-INFO
--rw-r--r--   0 kareltutsu   (501) staff       (20)      223 2024-04-08 02:01:24.000000 fsinfo-0.0.2/fsinfo.egg-info/SOURCES.txt
--rw-r--r--   0 kareltutsu   (501) staff       (20)        1 2024-04-08 02:01:24.000000 fsinfo-0.0.2/fsinfo.egg-info/dependency_links.txt
--rw-r--r--   0 kareltutsu   (501) staff       (20)        1 2024-04-08 02:01:24.000000 fsinfo-0.0.2/fsinfo.egg-info/top_level.txt
--rw-r--r--   0 kareltutsu   (501) staff       (20)       38 2024-04-08 02:01:24.124111 fsinfo-0.0.2/setup.cfg
--rw-r--r--   0 kareltutsu   (501) staff       (20)      666 2024-04-08 01:59:42.000000 fsinfo-0.0.2/setup.py
-drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 02:01:24.122326 fsinfo-0.0.2/test/
--rw-r--r--   0 kareltutsu   (501) staff       (20)     1732 2024-04-08 01:32:47.000000 fsinfo-0.0.2/test/test_directoryinfo.py
--rw-r--r--   0 kareltutsu   (501) staff       (20)     3268 2024-04-08 01:32:47.000000 fsinfo-0.0.2/test/test_fileinfo.py
--rw-r--r--   0 kareltutsu   (501) staff       (20)     2185 2024-04-08 01:34:02.000000 fsinfo-0.0.2/test/test_filesysteminfo.py
+drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 02:02:21.082212 fsinfo-0.0.3/
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1068 2024-04-07 21:12:40.000000 fsinfo-0.0.3/LICENSE
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1931 2024-04-08 02:02:21.081793 fsinfo-0.0.3/PKG-INFO
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1423 2024-04-08 02:02:14.000000 fsinfo-0.0.3/README.md
+drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 02:02:21.081348 fsinfo-0.0.3/fsinfo.egg-info/
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1931 2024-04-08 02:02:21.000000 fsinfo-0.0.3/fsinfo.egg-info/PKG-INFO
+-rw-r--r--   0 kareltutsu   (501) staff       (20)      223 2024-04-08 02:02:21.000000 fsinfo-0.0.3/fsinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 kareltutsu   (501) staff       (20)        1 2024-04-08 02:02:21.000000 fsinfo-0.0.3/fsinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 kareltutsu   (501) staff       (20)        1 2024-04-08 02:02:21.000000 fsinfo-0.0.3/fsinfo.egg-info/top_level.txt
+-rw-r--r--   0 kareltutsu   (501) staff       (20)       38 2024-04-08 02:02:21.082314 fsinfo-0.0.3/setup.cfg
+-rw-r--r--   0 kareltutsu   (501) staff       (20)      666 2024-04-08 02:02:18.000000 fsinfo-0.0.3/setup.py
+drwxr-xr-x   0 kareltutsu   (501) staff       (20)        0 2024-04-08 02:02:21.080581 fsinfo-0.0.3/test/
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     1732 2024-04-08 01:32:47.000000 fsinfo-0.0.3/test/test_directoryinfo.py
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     3268 2024-04-08 01:32:47.000000 fsinfo-0.0.3/test/test_fileinfo.py
+-rw-r--r--   0 kareltutsu   (501) staff       (20)     2185 2024-04-08 01:34:02.000000 fsinfo-0.0.3/test/test_filesysteminfo.py
```

### Comparing `fsinfo-0.0.2/LICENSE` & `fsinfo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.2/PKG-INFO` & `fsinfo-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsinfo
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library for cross-platform filesystem operations, providing classes for handling files and directories.
 Home-page: https://github.com/KarelOmab/fsinfo
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,27 +26,28 @@
 
 ### Working with Files
 
 ```
 from YourPackageName.fileinfo import FileInfo 
 
 file = FileInfo('/path/to/your/file.txt')
-print(file.creation_time) file.copy_to('/path/to/destination/file.txt', overwrite=True)
+print(file.creation_time)
+file.copy_to('/path/to/destination/file.txt', overwrite=True)
 ```
 
 ### Working with Directories
 
 ```
 from YourPackageName.directoryinfo import DirectoryInfo 
 
 directory = DirectoryInfo('/path/to/your/directory')
 print(directory.length)  # Total size of files in the directory
 
 for  file_info  in  directory.get_files():
-	print(file_info.name)
+  print(file_info.name)
 ```
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a pull request.
 
 ## License
```

### Comparing `fsinfo-0.0.2/README.md` & `fsinfo-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 
 ### Working with Files
 
 ```
 from YourPackageName.fileinfo import FileInfo 
 
 file = FileInfo('/path/to/your/file.txt')
-print(file.creation_time) file.copy_to('/path/to/destination/file.txt', overwrite=True)
+print(file.creation_time)
+file.copy_to('/path/to/destination/file.txt', overwrite=True)
 ```
 
 ### Working with Directories
 
 ```
 from YourPackageName.directoryinfo import DirectoryInfo 
 
 directory = DirectoryInfo('/path/to/your/directory')
 print(directory.length)  # Total size of files in the directory
 
 for  file_info  in  directory.get_files():
-	print(file_info.name)
+  print(file_info.name)
 ```
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a pull request.
 
 ## License
```

### Comparing `fsinfo-0.0.2/fsinfo.egg-info/PKG-INFO` & `fsinfo-0.0.3/fsinfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsinfo
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library for cross-platform filesystem operations, providing classes for handling files and directories.
 Home-page: https://github.com/KarelOmab/fsinfo
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,27 +26,28 @@
 
 ### Working with Files
 
 ```
 from YourPackageName.fileinfo import FileInfo 
 
 file = FileInfo('/path/to/your/file.txt')
-print(file.creation_time) file.copy_to('/path/to/destination/file.txt', overwrite=True)
+print(file.creation_time)
+file.copy_to('/path/to/destination/file.txt', overwrite=True)
 ```
 
 ### Working with Directories
 
 ```
 from YourPackageName.directoryinfo import DirectoryInfo 
 
 directory = DirectoryInfo('/path/to/your/directory')
 print(directory.length)  # Total size of files in the directory
 
 for  file_info  in  directory.get_files():
-	print(file_info.name)
+  print(file_info.name)
 ```
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a pull request.
 
 ## License
```

### Comparing `fsinfo-0.0.2/setup.py` & `fsinfo-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fsinfo',
-    version='0.0.2',
+    version='0.0.3',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='A Python library for cross-platform filesystem operations, providing classes for handling files and directories.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/fsinfo',
     packages=find_packages(),
```

### Comparing `fsinfo-0.0.2/test/test_directoryinfo.py` & `fsinfo-0.0.3/test/test_directoryinfo.py`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.2/test/test_fileinfo.py` & `fsinfo-0.0.3/test/test_fileinfo.py`

 * *Files identical despite different names*

### Comparing `fsinfo-0.0.2/test/test_filesysteminfo.py` & `fsinfo-0.0.3/test/test_filesysteminfo.py`

 * *Files identical despite different names*

