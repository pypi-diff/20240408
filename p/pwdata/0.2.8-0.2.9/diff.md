# Comparing `tmp/pwdata-0.2.8.tar.gz` & `tmp/pwdata-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwdata-0.2.8.tar", last modified: Mon Mar 25 05:51:44 2024, max compression
+gzip compressed data, was "pwdata-0.2.9.tar", last modified: Wed Mar 27 09:54:48 2024, max compression
```

## Comparing `pwdata-0.2.8.tar` & `pwdata-0.2.9.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-25 05:51:44.658800 pwdata-0.2.8/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    35148 2024-02-27 08:01:20.000000 pwdata-0.2.8/LICENSE
--rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      659 2024-03-25 05:51:44.658149 pwdata-0.2.8/PKG-INFO
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       51 2024-03-08 09:41:47.000000 pwdata-0.2.8/README.md
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-25 05:51:39.861587 pwdata-0.2.8/pwdata/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      283 2024-03-05 03:01:36.000000 pwdata-0.2.8/pwdata/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2657 2024-02-28 03:42:10.000000 pwdata-0.2.8/pwdata/atomconfig.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-25 05:51:41.273054 pwdata-0.2.8/pwdata/build/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:13.000000 pwdata-0.2.8/pwdata/build/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5902 2024-02-27 07:43:28.000000 pwdata-0.2.8/pwdata/build/cell.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2815 2024-02-28 03:47:20.000000 pwdata-0.2.8/pwdata/build/geometry.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3886 2024-03-05 02:57:00.000000 pwdata-0.2.8/pwdata/build/supercells.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    15512 2024-03-05 05:46:07.000000 pwdata-0.2.8/pwdata/build/write_struc.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-25 05:51:44.625870 pwdata-0.2.8/pwdata/calculators/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:16.000000 pwdata-0.2.8/pwdata/calculators/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14172 2024-02-27 07:43:28.000000 pwdata-0.2.8/pwdata/calculators/const.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     4873 2024-02-27 07:50:22.000000 pwdata-0.2.8/pwdata/calculators/unitconvert_lmps.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     7964 2024-02-27 07:43:28.000000 pwdata-0.2.8/pwdata/calculators/units.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14250 2024-02-28 03:43:29.000000 pwdata-0.2.8/pwdata/cp2kdata.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5439 2024-03-01 02:53:29.000000 pwdata-0.2.8/pwdata/datasets_saver.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5975 2024-03-25 05:49:22.000000 pwdata-0.2.8/pwdata/deepmd.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     8826 2024-02-28 03:44:14.000000 pwdata-0.2.8/pwdata/dump.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1648 2024-03-05 02:49:25.000000 pwdata-0.2.8/pwdata/extendedxyz.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    11091 2024-03-05 04:01:01.000000 pwdata-0.2.8/pwdata/image.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    13928 2024-02-28 03:45:13.000000 pwdata-0.2.8/pwdata/lammpsdata.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1661 2024-02-27 07:43:28.000000 pwdata-0.2.8/pwdata/lmps.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    16392 2024-03-22 04:54:49.000000 pwdata-0.2.8/pwdata/main.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5350 2024-03-18 07:39:03.000000 pwdata-0.2.8/pwdata/movement.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2587 2024-03-05 02:49:08.000000 pwdata-0.2.8/pwdata/movement_saver.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     6636 2024-02-28 03:46:06.000000 pwdata-0.2.8/pwdata/outcar.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-25 05:51:44.656389 pwdata-0.2.8/pwdata/pertub/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:19.000000 pwdata-0.2.8/pwdata/pertub/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     9133 2024-03-05 02:56:31.000000 pwdata-0.2.8/pwdata/pertub/perturbation.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2446 2024-03-05 02:56:46.000000 pwdata-0.2.8/pwdata/pertub/scale.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3066 2024-02-28 03:46:19.000000 pwdata-0.2.8/pwdata/poscar.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-25 05:51:44.657467 pwdata-0.2.8/pwdata.egg-info/
--rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      659 2024-03-25 05:51:38.000000 pwdata-0.2.8/pwdata.egg-info/PKG-INFO
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      760 2024-03-25 05:51:38.000000 pwdata-0.2.8/pwdata.egg-info/SOURCES.txt
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        1 2024-03-25 05:51:38.000000 pwdata-0.2.8/pwdata.egg-info/dependency_links.txt
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        7 2024-03-25 05:51:38.000000 pwdata-0.2.8/pwdata.egg-info/top_level.txt
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       38 2024-03-25 05:51:44.658928 pwdata-0.2.8/setup.cfg
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      824 2024-03-25 05:50:51.000000 pwdata-0.2.8/setup.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-27 09:54:48.603312 pwdata-0.2.9/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    35148 2024-02-27 08:01:20.000000 pwdata-0.2.9/LICENSE
+-rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      659 2024-03-27 09:54:48.602612 pwdata-0.2.9/PKG-INFO
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       51 2024-03-08 09:41:47.000000 pwdata-0.2.9/README.md
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-27 09:54:48.496547 pwdata-0.2.9/pwdata/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      283 2024-03-05 03:01:36.000000 pwdata-0.2.9/pwdata/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2657 2024-02-28 03:42:10.000000 pwdata-0.2.9/pwdata/atomconfig.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-27 09:54:48.524796 pwdata-0.2.9/pwdata/build/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:13.000000 pwdata-0.2.9/pwdata/build/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5902 2024-02-27 07:43:28.000000 pwdata-0.2.9/pwdata/build/cell.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2815 2024-02-28 03:47:20.000000 pwdata-0.2.9/pwdata/build/geometry.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3886 2024-03-05 02:57:00.000000 pwdata-0.2.9/pwdata/build/supercells.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    15512 2024-03-05 05:46:07.000000 pwdata-0.2.9/pwdata/build/write_struc.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-27 09:54:48.571877 pwdata-0.2.9/pwdata/calculators/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:16.000000 pwdata-0.2.9/pwdata/calculators/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14172 2024-02-27 07:43:28.000000 pwdata-0.2.9/pwdata/calculators/const.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     4873 2024-02-27 07:50:22.000000 pwdata-0.2.9/pwdata/calculators/unitconvert_lmps.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     7964 2024-02-27 07:43:28.000000 pwdata-0.2.9/pwdata/calculators/units.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14250 2024-02-28 03:43:29.000000 pwdata-0.2.9/pwdata/cp2kdata.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5439 2024-03-01 02:53:29.000000 pwdata-0.2.9/pwdata/datasets_saver.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5975 2024-03-25 05:49:22.000000 pwdata-0.2.9/pwdata/deepmd.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     8826 2024-02-28 03:44:14.000000 pwdata-0.2.9/pwdata/dump.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1648 2024-03-05 02:49:25.000000 pwdata-0.2.9/pwdata/extendedxyz.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    11091 2024-03-05 04:01:01.000000 pwdata-0.2.9/pwdata/image.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    13928 2024-02-28 03:45:13.000000 pwdata-0.2.9/pwdata/lammpsdata.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1661 2024-02-27 07:43:28.000000 pwdata-0.2.9/pwdata/lmps.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    16592 2024-03-27 09:50:17.000000 pwdata-0.2.9/pwdata/main.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5350 2024-03-18 07:39:03.000000 pwdata-0.2.9/pwdata/movement.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2587 2024-03-05 02:49:08.000000 pwdata-0.2.9/pwdata/movement_saver.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     6636 2024-02-28 03:46:06.000000 pwdata-0.2.9/pwdata/outcar.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-27 09:54:48.601092 pwdata-0.2.9/pwdata/pertub/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:19.000000 pwdata-0.2.9/pwdata/pertub/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     9133 2024-03-05 02:56:31.000000 pwdata-0.2.9/pwdata/pertub/perturbation.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2446 2024-03-05 02:56:46.000000 pwdata-0.2.9/pwdata/pertub/scale.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3066 2024-02-28 03:46:19.000000 pwdata-0.2.9/pwdata/poscar.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2764 2024-03-27 09:52:54.000000 pwdata-0.2.9/pwdata/pwmlff.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-03-27 09:54:48.601815 pwdata-0.2.9/pwdata.egg-info/
+-rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      659 2024-03-27 09:54:47.000000 pwdata-0.2.9/pwdata.egg-info/PKG-INFO
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      777 2024-03-27 09:54:47.000000 pwdata-0.2.9/pwdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        1 2024-03-27 09:54:47.000000 pwdata-0.2.9/pwdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        7 2024-03-27 09:54:47.000000 pwdata-0.2.9/pwdata.egg-info/top_level.txt
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       38 2024-03-27 09:54:48.603430 pwdata-0.2.9/setup.cfg
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      824 2024-03-27 09:54:40.000000 pwdata-0.2.9/setup.py
```

### Comparing `pwdata-0.2.8/LICENSE` & `pwdata-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/PKG-INFO` & `pwdata-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwdata
-Version: 0.2.8
+Version: 0.2.9
 Summary: pwdata is a data pre-processing tool for PWMLFF, which can be used to extract features and labels. It also provides convenient interfaces for data conversion between different software.
 Home-page: https://github.com/LonxunQuantum/pwdata
 Author: LonxunQuantum
 Author-email: lonxun@pwmat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pwdata-0.2.8/pwdata/atomconfig.py` & `pwdata-0.2.9/pwdata/atomconfig.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/build/cell.py` & `pwdata-0.2.9/pwdata/build/cell.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/build/geometry.py` & `pwdata-0.2.9/pwdata/build/geometry.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/build/supercells.py` & `pwdata-0.2.9/pwdata/build/supercells.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/build/write_struc.py` & `pwdata-0.2.9/pwdata/build/write_struc.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/calculators/const.py` & `pwdata-0.2.9/pwdata/calculators/const.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/calculators/unitconvert_lmps.py` & `pwdata-0.2.9/pwdata/calculators/unitconvert_lmps.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/calculators/units.py` & `pwdata-0.2.9/pwdata/calculators/units.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/cp2kdata.py` & `pwdata-0.2.9/pwdata/cp2kdata.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/datasets_saver.py` & `pwdata-0.2.9/pwdata/datasets_saver.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/deepmd.py` & `pwdata-0.2.9/pwdata/deepmd.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/dump.py` & `pwdata-0.2.9/pwdata/dump.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/extendedxyz.py` & `pwdata-0.2.9/pwdata/extendedxyz.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/image.py` & `pwdata-0.2.9/pwdata/image.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/lammpsdata.py` & `pwdata-0.2.9/pwdata/lammpsdata.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/lmps.py` & `pwdata-0.2.9/pwdata/lmps.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/main.py` & `pwdata-0.2.9/pwdata/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 import os, sys, glob
 from math import ceil
-from collections import Counter
 from typing import (List, Union, Optional)
 # import time
 # os.chdir(os.path.dirname(os.path.abspath(__file__)))
 sys.path.append(os.path.dirname(os.path.abspath(__file__)))
 from pwdata.image import Image
 from pwdata.movement import MOVEMENT
 from pwdata.outcar import OUTCAR
 from pwdata.poscar import POSCAR
 from pwdata.atomconfig import CONFIG
 from pwdata.dump import DUMP
 from pwdata.lammpsdata import LMP
 from pwdata.cp2kdata import CP2KMD, CP2KSCF
 from pwdata.deepmd import DPNPY, DPRAW
+from pwdata.pwmlff import PWNPY
 from pwdata.movement_saver import save_to_movement
 from pwdata.extendedxyz import save_to_extxyz
 from pwdata.datasets_saver import save_to_dataset, get_pw, save_to_raw, save_to_npy
 from pwdata.build.write_struc import write_config, write_vasp, write_lammps
 
 class Save_Data(object):
     def __init__(self, data_path, datasets_path = "./PWdata", train_data_path = "train", valid_data_path = "valid", 
@@ -54,14 +54,16 @@
                 self.image_data = CP2KMD(data_path)
             elif format.lower() == 'cp2k/scf':
                 self.image_data = CP2KSCF(data_path)
             elif format.lower() == 'deepmd/npy':
                 self.image_data = DPNPY(data_path)
             elif format.lower() == 'deepmd/raw':
                 self.image_data = DPRAW(data_path)
+            elif format.lower() == 'pwmlff/npy':
+                self.image_data = PWNPY(data_path)
         self.lattice, self.position, self.energies, self.ei, self.forces, self.virials, self.atom_type, self.atom_types_image, self.image_nums = get_pw(self.image_data.get())
 
         if train_ratio is not None:  # inference 时不存数据
             self.train_ratio = train_ratio        
             self.split_and_save_data(seed, random, self.labels_path, train_data_path, valid_data_path, retain_raw)
     
     def split_and_save_data(self, seed, random, labels_path, train_path, val_path, retain_raw):
@@ -180,14 +182,16 @@
             image = CP2KMD(data_path).image_list[index]
         elif format.lower() == 'cp2k/scf':
             image = CP2KSCF(data_path).image_list[0]
         elif format.lower() == 'deepmd/npy':
             image = DPNPY(data_path).image_list[index]
         elif format.lower() == 'deepmd/raw':
             image = DPRAW(data_path).image_list[index]
+        elif format.lower() == 'pwmlff/npy':
+            image = PWNPY(data_path).image_list[index]
         else:
             raise Exception("Error! The format of the input file is not supported!")
         return image
     
     def to(self, output_path, save_format = None, **kwargs):
         """
         Write all images (>= 1) object to a new file.
```

### Comparing `pwdata-0.2.8/pwdata/movement.py` & `pwdata-0.2.9/pwdata/movement.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/movement_saver.py` & `pwdata-0.2.9/pwdata/movement_saver.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/outcar.py` & `pwdata-0.2.9/pwdata/outcar.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/pertub/perturbation.py` & `pwdata-0.2.9/pwdata/pertub/perturbation.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/pertub/scale.py` & `pwdata-0.2.9/pwdata/pertub/scale.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata/poscar.py` & `pwdata-0.2.9/pwdata/poscar.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.8/pwdata.egg-info/PKG-INFO` & `pwdata-0.2.9/pwdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwdata
-Version: 0.2.8
+Version: 0.2.9
 Summary: pwdata is a data pre-processing tool for PWMLFF, which can be used to extract features and labels. It also provides convenient interfaces for data conversion between different software.
 Home-page: https://github.com/LonxunQuantum/pwdata
 Author: LonxunQuantum
 Author-email: lonxun@pwmat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pwdata-0.2.8/pwdata.egg-info/SOURCES.txt` & `pwdata-0.2.9/pwdata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pwdata/lammpsdata.py
 pwdata/lmps.py
 pwdata/main.py
 pwdata/movement.py
 pwdata/movement_saver.py
 pwdata/outcar.py
 pwdata/poscar.py
+pwdata/pwmlff.py
 pwdata.egg-info/PKG-INFO
 pwdata.egg-info/SOURCES.txt
 pwdata.egg-info/dependency_links.txt
 pwdata.egg-info/top_level.txt
 pwdata/build/__init__.py
 pwdata/build/cell.py
 pwdata/build/geometry.py
```

### Comparing `pwdata-0.2.8/setup.py` & `pwdata-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pwdata", 
-    version="0.2.8",
+    version="0.2.9",
     author="LonxunQuantum",
     author_email="lonxun@pwmat.com",
     description="pwdata is a data pre-processing tool for PWMLFF, which can be used to extract features and labels. It also provides convenient interfaces for data conversion between different software.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LonxunQuantum/pwdata",
     packages=setuptools.find_packages(),
```

