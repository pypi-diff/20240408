# Comparing `tmp/falconz-2.0.9.tar.gz` & `tmp/falconz-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falconz-2.0.9.tar", last modified: Mon Aug 28 16:04:18 2023, max compression
+gzip compressed data, was "falconz-2.1.0.tar", last modified: Mon Apr  8 13:18:37 2024, max compression
```

## Comparing `falconz-2.0.9.tar` & `falconz-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:04:18.102439 falconz-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (999)    35149 2023-08-28 16:04:06.000000 falconz-2.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     1726 2023-08-28 16:04:18.102439 falconz-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    13478 2023-08-28 16:04:06.000000 falconz-2.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:04:18.102439 falconz-2.0.9/falconz/
--rw-r--r--   0 runner    (1001) docker     (999)      129 2023-08-28 16:04:06.000000 falconz-2.0.9/falconz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2778 2023-08-28 16:04:06.000000 falconz-2.0.9/falconz/constants.py
--rw-r--r--   0 runner    (1001) docker     (999)     5105 2023-08-28 16:04:06.000000 falconz-2.0.9/falconz/display.py
--rw-r--r--   0 runner    (1001) docker     (999)     4265 2023-08-28 16:04:06.000000 falconz-2.0.9/falconz/download.py
--rw-r--r--   0 runner    (1001) docker     (999)     9084 2023-08-28 16:04:06.000000 falconz-2.0.9/falconz/falconz.py
--rw-r--r--   0 runner    (1001) docker     (999)     6795 2023-08-28 16:04:06.000000 falconz-2.0.9/falconz/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (999)    10152 2023-08-28 16:04:06.000000 falconz-2.0.9/falconz/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (999)    20806 2023-08-28 16:04:06.000000 falconz-2.0.9/falconz/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (999)     2795 2023-08-28 16:04:06.000000 falconz-2.0.9/falconz/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (999)     2325 2023-08-28 16:04:06.000000 falconz-2.0.9/falconz/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:04:18.102439 falconz-2.0.9/falconz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     1726 2023-08-28 16:04:18.000000 falconz-2.0.9/falconz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      444 2023-08-28 16:04:18.000000 falconz-2.0.9/falconz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:04:18.000000 falconz-2.0.9/falconz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       49 2023-08-28 16:04:18.000000 falconz-2.0.9/falconz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      283 2023-08-28 16:04:18.000000 falconz-2.0.9/falconz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        8 2023-08-28 16:04:18.000000 falconz-2.0.9/falconz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:04:18.102439 falconz-2.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     2751 2023-08-28 16:04:06.000000 falconz-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:18:37.011156 falconz-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 13:18:32.000000 falconz-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-08 13:18:37.011156 falconz-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-08 13:18:32.000000 falconz-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:18:37.011156 falconz-2.1.0/falconz/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/falconz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19478 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:18:37.011156 falconz-2.1.0/falconz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-08 13:18:36.000000 falconz-2.1.0/falconz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-08 13:18:37.000000 falconz-2.1.0/falconz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:18:36.000000 falconz-2.1.0/falconz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 13:18:36.000000 falconz-2.1.0/falconz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-08 13:18:36.000000 falconz-2.1.0/falconz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 13:18:36.000000 falconz-2.1.0/falconz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:18:37.011156 falconz-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-08 13:18:32.000000 falconz-2.1.0/setup.py
```

### Comparing `falconz-2.0.9/LICENSE` & `falconz-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `falconz-2.0.9/falconz/constants.py` & `falconz-2.1.0/falconz/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,30 +16,36 @@
 project_root = file_utilities.get_virtual_env_root()
 
 # Set the path to the binary folder
 BINARY_PATH = os.path.join(project_root, 'bin')
 
 # Set the paths to the binaries based on the operating system
 if file_utilities.get_system()[0] == 'windows':
-    GREEDY_PATH = os.path.join(BINARY_PATH, f'greedy-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    GREEDY_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                                'greedy.exe')
-    C3D_PATH = os.path.join(BINARY_PATH, f'c3d-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    C3D_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                             'c3d.exe')
+    DCM2NIIX_PATH = os.path.join(BINARY_PATH,
+                                 f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+                                 'dcm2niix.exe')
 elif file_utilities.get_system()[0] in ['linux', 'mac']:
-    GREEDY_PATH = os.path.join(BINARY_PATH, f'greedy-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    GREEDY_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                                'greedy')
-    C3D_PATH = os.path.join(BINARY_PATH, f'c3d-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    C3D_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                             'c3d')
+    DCM2NIIX_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+                                    'dcm2niix')
 else:
     raise ValueError('Unsupported OS')
 
 # Define color codes for console output
 ANSI_ORANGE = '\033[38;5;208m'
-ANSI_GREEN = '\033[38;5;40m'
+ANSI_GREEN = '\033[32m'
 ANSI_VIOLET = '\033[38;5;141m'
+ANSI_RED = '\033[38;5;196m'
 ANSI_RESET = '\033[0m'
 
 # Define the allowed modalities
 MODALITIES = ['PET', 'CT', 'MR']
 
 # Define the minimum system requirements for each registration paradigm
 MINIMUM_RAM_REQUIRED_RIGID = 4  # in GB
@@ -49,26 +55,38 @@
 MINIMUM_THREADS_REQUIRED_AFFINE = 4  # in number of threads
 MINIMUM_THREADS_REQUIRED_DEFORMABLE = 8  # in number of threads
 
 # Define the shrink levels supported
 SHRINK_LEVEL = [2, 4, 8]
 
 # Define the normalized cross correlation threshold and radius
-NCC_THRESHOLD = 0.5
+NCC_THRESHOLD = 0.6
 NCC_RADIUS = '4x4x4'
 
 # Define the file names and folder names used in the FALCONZ pipeline
 MOCO_PREFIX = 'moco_'
+NO_MOCO_PREFIX = 'no_moco_'
 ALIGNED_PREFIX = 'aligned_'
 TRANSFORMS_KEYWORD = ['*warp.nii.gz', '*rigid.mat', '*affine.mat']
 MOCO_4D_FILE_NAME = 'moco_4D.nii.gz'
 FALCON_WORKING_FOLDER = 'FALCONZ-V02' + '-' + datetime.now().strftime('%Y-%m-%d-%H-%M-%S')
 TRANSFORMS_FOLDER = 'transforms'
 MOCO_FOLDER = 'Motion-corrected-images'
+SPLIT_FOLDER = 'Split-Nifti-files'
 
 # Define the hyperparameters used in the registration process
 MULTI_RESOLUTION_SCHEME = '100x25x10'
+MULTI_RESOLUTION_SCHEME_DASH = '100x25x10x0'
 EXPECTED_DIMENSIONS = 4
 ALLOWED_REGISTRATION_PARADIGMS = ["rigid", "affine", "deformable"]
 IMAGE_INTERPOLATION = 'Linear'
 MASK_INTERPOLATION = 'Nearest Neighbor'
 COST_FUNCTION = 'NCC 2x2x2'
+PROPORTION_OF_CORES = 1 / 8  # 1/8th of the available cores will be used for motion correction
+
+# ALLOWED EXTENSIONS
+
+VALID_EXTENSIONS = ['.nii', '.nii.gz', '.hdr', '.img', '.nrrd', '.mha', '.mhd']
+
+# ALLOWED MODES
+
+ALLOWED_MODES = ['cruise', 'dash']
```

### Comparing `falconz-2.0.9/falconz/display.py` & `falconz-2.1.0/falconz/display.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 This module shows predefined display messages for the falconz.
 
 Usage:
     The functions in this module can be imported and used in other modules within the falconz to show predefined display messages.
 """
 
 import logging
+import multiprocessing
 import pyfiglet
 
 from falconz import constants
 from falconz import file_utilities
 
 
 def logo():
@@ -58,16 +59,14 @@
 
 def expectations():
     """
     Display expected modalities for FALCON. This is used to check if the user has provided the correct set of modalities for each tracer set.
 
     :return: None
     """
-    print(f' Expected dimensions: {constants.EXPECTED_DIMENSIONS} | Allowed modalities: {constants.MODALITIES}')
-    logging.info(f' Expected dimensions: {constants.EXPECTED_DIMENSIONS} | Allowed modalities: {constants.MODALITIES}')
     print(
         f"{constants.ANSI_ORANGE} Warning: Only 4D images will be considered in the analysis. {constants.ANSI_RESET}")
 
     warning_message = "Only 4D images will be considered in the analysis."
     logging.warning(warning_message)
 
 
@@ -112,14 +111,14 @@
         num_jobs, avail_memory, avail_threads = file_utilities.get_number_of_possible_jobs(
             process_memory=constants.MINIMUM_RAM_REQUIRED_DEFORMABLE,
             process_threads=constants.MINIMUM_THREADS_REQUIRED_DEFORMABLE)
     else:
         raise ValueError('Unsupported registration paradigm')
 
     print(f' Available memory: {avail_memory} GB | Available threads: {avail_threads} | Number of motion correction '
-          f'done in parallel: {num_jobs}')
+          f'done in parallel: {max(1, int(multiprocessing.cpu_count() * constants.PROPORTION_OF_CORES))}')
     logging.info(f' Available memory: {avail_memory} GB | Available threads: {avail_threads} | Number of motion '
-                 f'correction done in parallel: {num_jobs}')
+                 f'correction done in parallel: {max(1, int(multiprocessing.cpu_count() * constants.PROPORTION_OF_CORES))}')
     # if input arguments doesn't have start frame, display message saying it will be calculated on the fly
     if input_args.start_frame == 99:
         print(f' {constants.ANSI_ORANGE}Warning: Start frame not provided. It will be calculated on the fly. '
               f'{constants.ANSI_RESET}')
```

### Comparing `falconz-2.0.9/falconz/download.py` & `falconz-2.1.0/falconz/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-# ----------------------------------------------------------------------------------------------------------------------
-# Author: Lalith Kumar Shiyam Sundar
-# Institution: Medical University of Vienna
-# Research Group: Quantitative Imaging and Medical Physics (QIMP) Team
-# Date: 04.07.2023
-# Version: 0.1.0
-#
-# Description:
-# This module downloads the necessary binaries and models for the falconz.
-#
-# Usage:
-# The functions in this module can be imported and used in other modules within the pumaz to download the necessary
-# binaries and models for the falconz.
-#
-# ----------------------------------------------------------------------------------------------------------------------
+"""
+.. module:: download
+   :synopsis: This module downloads the necessary binaries and models for the falconz.
+
+.. moduleauthor:: Lalith Kumar Shiyam Sundar <lalith.email@example.com>
+
+.. note::
+   Research Group: Quantitative Imaging and Medical Physics (QIMP) Team
+
+**Version**: 0.1.0
+
+**Date**: 04.07.2023
+
+Usage
+-----
+The functions in this module can be imported and used in other modules within the falconz to download the necessary
+binaries and models for the falconz.
+"""
 
 import logging
 import os
-import requests
-import time
 import zipfile
+
+import requests
 from rich.console import Console
 from rich.progress import Progress, BarColumn, TextColumn, TimeRemainingColumn, FileSizeColumn, TransferSpeedColumn
 
 from falconz import constants
 
 
 def download(item_name, item_path, item_dict):
```

### Comparing `falconz-2.0.9/falconz/falconz.py` & `falconz-2.1.0/falconz/falconz.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 .. moduleauthor:: Lalith Kumar Shiyam Sundar <lalith.shiyamsundar@meduniwien.ac.at>
 
 """
 
 # Importing necessary libraries and modules
 
 import argparse
-import colorama
-import emoji
 import logging
 import multiprocessing
 import os
 import shutil
 import sys
-import time
 from datetime import datetime
 
+import colorama
+import emoji
+from falconz.constants import FALCON_WORKING_FOLDER, PROPORTION_OF_CORES
+from falconz.image_conversion import NiftiConverter, NiftiConverterError, merge3d
+from falconz.image_processing import determine_candidate_frames, align
+from falconz.input_validation import InputValidation
+from rich.console import Console
+from rich.progress import Progress, TextColumn, TimeElapsedColumn
+
 from falconz import constants
 from falconz import display
 from falconz import download
 from falconz import file_utilities
-from falconz import image_conversion
-from falconz import input_validation
 from falconz import resources
-from falconz.constants import FALCON_WORKING_FOLDER
-from falconz.image_conversion import ImageConverter, merge3d
-from falconz.image_processing import determine_candidate_frames, align
-from falconz.input_validation import InputValidation
 
 logging.basicConfig(format='%(asctime)s %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s', level=logging.INFO,
                     filename=datetime.now().strftime('falconz-v.1.0.0.%H-%M-%d-%m-%Y.log'),
                     filemode='w')
 
 
 def main():
@@ -59,16 +59,16 @@
     """
     colorama.init()
 
     # Initialization: Setting up arguments, parsers, etc.
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        "-m",
-        "--main_folder",
+        "-d",
+        "--directory",
         type=str,
         help="path containing the images to motion correct",
         required=True,
     )
     parser.add_argument(
         "-rf",
         "--reference_frame_index",
@@ -94,17 +94,29 @@
     parser.add_argument(
         "-i",
         "--multi_resolution_iterations",
         type=str,
         default=constants.MULTI_RESOLUTION_SCHEME,
         help="Number of iterations for each resolution level"
     )
+    parser.add_argument(
+        "-m",
+        "--mode",
+        type=str,
+        default='cruise',
+        choices=constants.ALLOWED_MODES,
+        help="Mode of operation: cruise | dash"
+    )
     args = parser.parse_args()
     validator = InputValidation(args)
     validator.validate()
+    # change the multi-resolution scheme if the mode of operation is dash
+    if args.mode == 'dash':
+        args.multi_resolution_iterations = constants.MULTI_RESOLUTION_SCHEME_DASH
+
 
     display.logo()
     display.citation()
 
     logging.info('----------------------------------------------------------------------------------------------------')
     logging.info('                                     STARTING FALCON-Z V.2.0.0                                      ')
     logging.info('----------------------------------------------------------------------------------------------------')
@@ -129,40 +141,63 @@
 
     print('')
     binary_path = constants.BINARY_PATH
     file_utilities.create_directory(binary_path)
     system_os, system_arch = file_utilities.get_system()
     print(f'{constants.ANSI_ORANGE} Detected system: {system_os} | Detected architecture: {system_arch}'
           f'{constants.ANSI_RESET}')
-    download.download(item_name=f'greedy-{system_os}-{system_arch}', item_path=binary_path,
-                      item_dict=resources.GREEDY_BINARIES)
+    download.download(item_name=f'falcon-{system_os}-{system_arch}', item_path=binary_path,
+                      item_dict=resources.FALCON_BINARIES)
     file_utilities.set_permissions(constants.GREEDY_PATH, system_os)
-    download.download(item_name=f'c3d-{system_os}-{system_arch}', item_path=binary_path,
-                      item_dict=resources.C3D_BINARIES)
     file_utilities.set_permissions(constants.C3D_PATH, system_os)
+    file_utilities.set_permissions(constants.DCM2NIIX_PATH, system_os)
 
     # ----------------------------------
     # INPUT STANDARDIZATION
     # ----------------------------------
 
     print('')
     print(f'{constants.ANSI_VIOLET} {emoji.emojize(":magnifying_glass_tilted_left:")} STANDARDIZING INPUT DATA TO '
           f'NIFTI:{constants.ANSI_RESET}')
     print('')
     logging.info(' ')
     logging.info(' STANDARDIZING INPUT DATA TO NIFTI:')
     logging.info(' ')
-    image_dir = args.main_folder
+    image_dir = os.path.normpath(args.directory)
     parent_dir = os.path.dirname(image_dir)
     falcon_dir = os.path.join(parent_dir, FALCON_WORKING_FOLDER)
     file_utilities.create_directory(falcon_dir)
-    image_converter = ImageConverter(input_directory=image_dir, output_directory=falcon_dir)
-    split_nifti_dir = image_converter.convert()
-    print(f"{constants.ANSI_GREEN} Standardization complete.{constants.ANSI_RESET}")
-    logging.info(" Standardization complete.")
+    split_nifti_dir = os.path.join(falcon_dir, constants.SPLIT_FOLDER)
+    file_utilities.create_directory(split_nifti_dir)
+
+    console = Console()
+
+    with Progress(
+            TextColumn("[cyan]{task.fields[text]}"),
+            TimeElapsedColumn(),
+            console=console
+    ) as progress:
+
+        base_text = " Standardizing images to NIFTI format • Time elapsed:"
+        task = progress.add_task("[cyan]" + base_text,
+                                 text=base_text, total=100)
+
+        try:
+            image_converter = NiftiConverter(input_directory=image_dir, output_directory=split_nifti_dir)
+
+            # Update the task text to "Standardization complete" in green after the task is done
+            progress.update(task, text="[green] Standardization complete • Elapsed time:")
+            logging.info(" Standardization complete.")
+
+        except NiftiConverterError as e:
+            # Update the task text to "Standardization failed" in red on error
+            progress.update(task, text="[red] Standardization failed.")
+            logging.error(" Standardization failed.")
+            logging.error(e)
+            sys.exit(1)
 
     # ----------------------------------
     # MOTION CORRECTION
     # ----------------------------------
 
     org_nifti_files = file_utilities.get_files(split_nifti_dir, '*.nii')
     if len(org_nifti_files) == 0:
@@ -170,30 +205,31 @@
     reference_file = org_nifti_files[args.reference_frame_index]
     candidate_frames = org_nifti_files.copy()
     candidate_frames.remove(reference_file)
     start_frame = args.start_frame
     # choose start frame automatically if not specified
     if args.start_frame == 99:
         n_jobs = multiprocessing.cpu_count()
-        start_frame_file = determine_candidate_frames(candidate_frames, reference_file, falcon_dir,
-                                                      round(n_jobs / 2))
+        # Calculate the number of cores to use, ensuring it's at least 1
+        actual_n_jobs = max(1, round(n_jobs * PROPORTION_OF_CORES))
+        start_frame_file = determine_candidate_frames(candidate_frames, reference_file, falcon_dir, actual_n_jobs)
         # find the index of the start_frame_file in the org_nifti_files list
         start_frame = org_nifti_files.index(start_frame_file)
     # everything from and after start_frame will be motion corrected and will be called moving frames
     moving_frames = org_nifti_files[start_frame:]
-    moving_frames.remove(reference_file)
+    moving_frames = [frame for frame in moving_frames if frame != reference_file]
     # everything before that will not be motion corrected and will be called non-moco frames
     non_moco_frames = org_nifti_files[:start_frame]
     print('')
     print(f'{constants.ANSI_VIOLET} {emoji.emojize(":eagle:")} PERFORMING MOTION CORRECTION:{constants.ANSI_RESET}')
     print('')
     logging.info(' ')
     logging.info(' PERFORMING MOTION CORRECTION:')
     logging.info(' ')
-    print(f' Number of files to motion correct: {len(candidate_frames)} | Reference file: '
+    print(f' Number of files to motion correct: {len(moving_frames)} | Reference file: '
           f'{os.path.basename(reference_file)} | Start frame: {start_frame}')
     moco_dir = os.path.join(falcon_dir, constants.MOCO_FOLDER)
     file_utilities.create_directory(moco_dir)
     align(fixed_img=reference_file, moving_imgs=moving_frames, registration_type=args.registration,
           multi_resolution_iterations=args.multi_resolution_iterations, moco_dir=moco_dir)
 
     # ----------------------------------
@@ -209,20 +245,20 @@
             for transform_file in transform_files:
                 shutil.move(transform_file, transforms_dir)
         else:
             continue
 
     # COPY THE REFERENCE FRAME FROM THE SPLIT NIFTI FOLDER TO THE MOCO FOLDER WITH MOCO PREFIX
     reference_file_name = os.path.basename(reference_file)
-    moco_reference_file = os.path.join(moco_dir, constants.MOCO_PREFIX + reference_file_name)
+    moco_reference_file = os.path.join(moco_dir, constants.NO_MOCO_PREFIX + reference_file_name)
     shutil.copy(reference_file, moco_reference_file)
 
     # COPY THE NON-MOCO FRAMES FROM THE SPLIT NIFTI FOLDER TO THE MOCO FOLDER WITH MOCO PREFIX
     for non_moco_frame in non_moco_frames:
         non_moco_frame_name = os.path.basename(non_moco_frame)
-        moco_non_moco_frame = os.path.join(moco_dir, constants.MOCO_PREFIX + non_moco_frame_name)
+        moco_non_moco_frame = os.path.join(moco_dir, constants.NO_MOCO_PREFIX + non_moco_frame_name)
         shutil.copy(non_moco_frame, moco_non_moco_frame)
 
     # MERGE THE 3D MOCO FRAMES TO A 4D NIFTI FILE
-    merge3d(moco_dir, constants.MOCO_PREFIX + '*', os.path.join(moco_dir, constants.MOCO_4D_FILE_NAME))
+    merge3d(moco_dir, '*' + constants.MOCO_PREFIX + '*', os.path.join(moco_dir, constants.MOCO_4D_FILE_NAME))
     print(f'{constants.ANSI_GREEN} Motion correction complete: '
           f'Results in {moco_dir} | 4D MoCo file: {constants.MOCO_4D_FILE_NAME}{constants.ANSI_RESET}')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `falconz-2.0.9/falconz/file_utilities.py` & `falconz-2.1.0/falconz/file_utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,38 +13,83 @@
 Usage:
     The functions in this module can be imported and used in other modules within the falconz to perform file operations.
 """
 
 import glob
 import os
 import platform
-import psutil
 import shutil
 import stat
 import subprocess
 import sys
+import re
 from multiprocessing import Pool
+import logging
+
+import psutil
 
 
 def set_permissions(file_path, system_type):
     """
-    Sets permissions for a file based on the system type.
+    Set permissions for a file based on the operating system.
 
     :param file_path: The path to the file.
     :type file_path: str
-    :param system_type: The type of the system.
+    :param system_type: The type of the operating system.
     :type system_type: str
-    :raises ValueError: If the system type is not supported.
+    :return: None
+    :rtype: None
+    :raises: ValueError if the operating system is not supported.
+
+    This function sets permissions for a file based on the operating system. If the operating system is Windows, it uses
+    the `icacls` command to grant full access to everyone. If the operating system is Linux or Mac, it uses the `chmod`
+    command to add execute permission for the owner, read permission for the group, and read permission for others. If
+    the operating system is not supported, it raises a ValueError.
+
+    :raises: ValueError if the operating system is not supported.
+    :raises: subprocess.CalledProcessError if the `icacls` command fails on Windows.
+    :raises: PermissionError if the `chmod` command fails on Linux or Mac.
+    :raises: Exception if an unknown error occurs.
+
+    :Example:
+        >>> set_permissions('/path/to/file', 'linux')
+    """
+    try:
+        if system_type == "windows":
+            subprocess.check_call(["icacls", file_path, "/grant", "Everyone:(F)"])
+        elif system_type in ["linux", "mac"]:
+            os.chmod(file_path, stat.S_IRWXU | stat.S_IRGRP | stat.S_IROTH)
+        else:
+            logging.error("Unsupported OS")
+            raise ValueError("Unsupported OS")
+    except subprocess.CalledProcessError:
+        logging.error(f"Could not set permissions for {file_path} on Windows")
+        exit(1)
+    except PermissionError:
+        logging.error(f"No permission to set {file_path} as executable")
+        exit(1)
+    except Exception as e:
+        logging.error(f"An error occurred: {e}")
+        exit(1)
+
+
+def numeric_sort_key(file_path: str) -> int:
+    """
+    Extracts the numeric portion from a filename for sorting purposes.
+
+    :param file_path: The path to the file.
+    :type file_path: str
+    :return: The numeric value extracted from the filename. Returns 0 if no number is found.
+    :rtype: int
     """
-    if system_type == "windows":
-        subprocess.check_call(["icacls", file_path, "/grant", "Everyone:(F)"])
-    elif system_type in ["linux", "mac"]:
-        os.chmod(file_path, stat.S_IRWXU | stat.S_IRGRP | stat.S_IROTH)  # equivalent to 'chmod u+x'
-    else:
-        raise ValueError("Unsupported OS")
+    # Extract the number from the filename using regex
+    match = re.search(r'(\d+)', os.path.basename(file_path))
+    if match:
+        return int(match.group(1))
+    return 0
 
 
 def get_virtual_env_root():
     """
     Gets the root directory of the virtual environment.
 
     :return: The root directory of the virtual environment.
```

### Comparing `falconz-2.0.9/falconz/image_conversion.py` & `falconz-2.1.0/falconz/image_conversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,258 +10,233 @@
 
 This module handles image conversion for the falconz.
 
 Usage:
     The functions in this module can be imported and used in other modules within the falconz to perform image conversion.
 
 """
-import SimpleITK
-import contextlib
-import dcm2niix
-import dicom2nifti
-import io
 import logging
-import nibabel as nib
 import os
+import pathlib
+import shutil
+import subprocess
+from typing import List
+
+import dask
+import nibabel as nib
 import pydicom
-import re
-import unicodedata
-from typing import Optional
+from dask import delayed
+from falconz.constants import C3D_PATH, VALID_EXTENSIONS, DCM2NIIX_PATH
 
 from falconz import file_utilities as fop
 
 
-class ImageConverter:
-    def __init__(self, input_directory: str, output_directory: str):
+class NiftiConverter:
+    """
+    A utility for converting various medical image formats in a directory into 3D NIFTI files.
+
+    Attributes:
+        input_directory (str): Path to the directory containing input images.
+        output_directory (str): Path to the directory where the converted images will be saved.
+    """
+
+    def __init__(self, input_directory: str, output_directory: str = None):
         """
-        Initializes an ImageConverter object.
+        Initializes the NiftiConverter.
 
-        :param input_directory: The path to the input directory.
-        :type input_directory: str
-        :param output_directory: The path to the output directory.
-        :type output_directory: str
+        :param str input_directory: Directory containing input images.
+        :param str output_directory: Directory for converted images. Defaults to 'converted' in input_directory.
+        :raises NiftiConverterError: If the input directory is not accessible or does not exist.
         """
+        if not os.path.exists(input_directory):
+            raise NiftiConverterError(f"Input directory '{input_directory}' does not exist or is not accessible.")
+        self.VALID_EXTENSIONS = VALID_EXTENSIONS
         self.input_directory = input_directory
-        self.output_directory = output_directory
-        self.split_nifti_directory = os.path.join(self.output_directory, 'split-nifti-files')
+        self.output_directory = output_directory if output_directory else os.path.join(input_directory, 'converted')
+        self._ensure_output_directory_exists()
+        self._process_input_directory()
+
+    def _ensure_output_directory_exists(self):
+        """Ensures the output directory exists, creating it if necessary."""
+        try:
+            if not os.path.exists(self.output_directory):
+                os.makedirs(self.output_directory)
+        except Exception as e:
+            raise NiftiConverterError(f"Error creating output directory: {e}")
+
+    def _process_input_directory(self):
+        """Processes the input directory based on the image types present."""
+        try:
+            file_list = [f for f in os.listdir(self.input_directory) if
+                         os.path.isfile(os.path.join(self.input_directory, f))]
+        except Exception as e:
+            raise NiftiConverterError(f"Error processing input directory: {e}")
+
+        if self._contains_dicom_images(file_list):
+            self._convert_dicom_series()
+        elif len(file_list) == 1:
+            self._process_single_image_file(file_list[0])
+        else:
+            self._process_multiple_image_files(file_list)
 
-        if not os.path.exists(self.split_nifti_directory):
-            os.makedirs(self.split_nifti_directory)
+    def _contains_dicom_images(self, file_list):
+        """
+        Checks if the directory contains DICOM images.
 
-    def non_nifti_to_nifti(self, input_path: str, output_directory: Optional[str] = None) -> None:
+        :param list file_list: List of filenames.
+        :return: True if DICOM images are detected, False otherwise.
+        :rtype: bool
         """
-        Converts non-NIfTI files to NIfTI format.
-
-        :param input_path: The path to the input file or directory.
-        :type input_path: str
-        :param output_directory: The path to the output directory.
-        :type output_directory: str
-        :return: None
-        """
-        if not os.path.exists(input_path):
-            print(f"Input path {input_path} does not exist.")
-            return
-
-        if os.path.isdir(input_path):
-            dicom_info = self.create_dicom_lookup(input_path)
-            nifti_dir = self.dcm2niix(input_path, output_directory)
-            self.rename_nifti_files(nifti_dir, dicom_info)
-            return
-
-        if os.path.isfile(input_path):
-            _, filename = os.path.split(input_path)
-            if filename.startswith('.') or filename.endswith(('.nii.gz', '.nii')):
-                return
-            else:
-                output_image = SimpleITK.ReadImage(input_path)
-                output_image_basename = f"{os.path.splitext(filename)[0]}.nii"
+        return any(self._is_dicom(os.path.join(self.input_directory, file)) for file in file_list)
 
-        if output_directory is None:
-            output_directory = os.path.dirname(input_path)
+    def _convert_dicom_series(self):
+        """Converts DICOM series in the directory to 3D NIFTI files."""
+        self.dcm2niix(self.input_directory, self.output_directory)
+        # remove the json file
+        json_file = [f for f in os.listdir(self.output_directory) if f.endswith('.json')]
+        if len(json_file) > 0:
+            os.remove(os.path.join(self.output_directory, json_file[0]))
 
-        output_image_path = os.path.join(output_directory, output_image_basename)
-        SimpleITK.WriteImage(output_image, output_image_path)
+        # Scan the output directory for the generated nifti files
+        converted_files = [f for f in os.listdir(self.output_directory) if (f.endswith('.nii.gz') or f.endswith('.nii'))]
 
-    def dcm2niix(self, input_path: str, output_dir: str) -> str:
+        for nifti_file in converted_files:
+            file_path = os.path.join(self.output_directory, nifti_file)
+
+            # Check if the file is 4D and needs to be split
+            if self._is_4d_image(file_path):
+                self._split_4d_image(file_path)
+                os.remove(file_path)
+
+    def _process_single_image_file(self, file_name):
         """
-        Converts DICOM files to NIfTI format using dcm2niix.
+        Processes a single image file in the directory.
 
-        :param input_path: The path to the input directory.
-        :type input_path: str
-        :param output_dir: The path to the output directory.
-        :type output_dir: str
-        :return: The path to the output directory.
-        :rtype: str
-        """
-        # Save the original stdout and stderr file descriptors.
-        original_stdout_fd = os.dup(1)
-        original_stderr_fd = os.dup(2)
-
-        # Open a null file to redirect the output.
-        with open(os.devnull, 'w') as null_file:
-            null_fd = null_file.fileno()
-
-            # Redirect stdout and stderr to the null file.
-            os.dup2(null_fd, 1)
-            os.dup2(null_fd, 2)
-
-            try:
-                dcm2niix.main(['-z', 'y', '-o', output_dir, input_path])
-            finally:
-                # Restore the original stdout and stderr file descriptors.
-                os.dup2(original_stdout_fd, 1)
-                os.dup2(original_stderr_fd, 2)
-                os.close(original_stdout_fd)
-                os.close(original_stderr_fd)
+        :param str file_name: Name of the image file.
+        """
+        full_path = os.path.join(self.input_directory, file_name)
+        if not self._has_valid_extension(file_name):
+            raise NiftiConverterError(f"Unsupported file format: {file_name}")
 
-        return output_dir
+        if self._is_4d_image(full_path):
+            self._split_4d_image(full_path)
+        else:
+            raise NiftiConverterError("Only a single 3D volume provided. Expecting a 4D volume or multiple 3D volumes.")
+
+    def _process_multiple_image_files(self, file_list):
+        tasks = []  # List to hold delayed tasks
+        for file_name in file_list:
+            full_path = os.path.join(self.input_directory, file_name)
+            if file_name.endswith(('.nii', '.nii.gz')):
+                shutil.copy(full_path, self.output_directory)
+            elif self._has_valid_extension(file_name):
+                # Add the task to the list
+                tasks.append(self._convert_to_nifti_format(full_path))
+
+        # Compute the tasks in parallel
+        dask.compute(*tasks)
 
-    def remove_accents(self, unicode_filename):
+    def _has_valid_extension(self, file_name):
         """
-        Removes accents from a Unicode filename.
+        Checks if a file has a valid image extension.
 
-        :param unicode_filename: The Unicode filename to remove accents from.
-        :type unicode_filename: str
-        :return: The filename without accents.
-        :rtype: str
+        :param str file_name: Name of the file.
+        :return: True if valid, False otherwise.
+        :rtype: bool
+        """
+        return any(file_name.endswith(ext) for ext in self.VALID_EXTENSIONS)
+
+    def _is_4d_image(self, image_path):
+        """
+        Checks if a given image is 4D.
+
+        :param str image_path: Path to the image file.
+        :return: True if the image is 4D, False otherwise.
+        :rtype: bool
         """
         try:
-            unicode_filename = str(unicode_filename).replace(" ", "_")
-            cleaned_filename = unicodedata.normalize('NFKD', unicode_filename).encode('ASCII', 'ignore').decode('ASCII')
-            cleaned_filename = re.sub(r'[^\w\s-]', '', cleaned_filename.strip().lower())
-            cleaned_filename = re.sub(r'[-\s]+', '-', cleaned_filename)
-            return cleaned_filename
+            img = nib.funcs.squeeze_image(nib.load(image_path))
+            return img.ndim == 4
         except:
-            return unicode_filename
+            return False
 
-    def is_dicom_file(self, filename):
+    def _is_dicom(self, file_path):
         """
-        Determines if a file is a DICOM file.
+        Checks if a given file is a DICOM image.
 
-        :param filename: The name of the file to check.
-        :type filename: str
-        :return: True if the file is a DICOM file, False otherwise.
+        :param str file_path: Path to the file.
+        :return: True if the file is a DICOM image, False otherwise.
         :rtype: bool
         """
         try:
-            pydicom.dcmread(filename)
+            _ = pydicom.dcmread(file_path)
             return True
-        except pydicom.errors.InvalidDicomError:
+        except:
             return False
 
-    def create_dicom_lookup(self, dicom_dir):
+    def _split_4d_image(self, image_path):
         """
-        Creates a dictionary of DICOM file information.
+        Splits a 4D image into multiple 3D NIFTI volumes.
 
-        :param dicom_dir: The path to the directory containing DICOM files.
-        :type dicom_dir: str
-        :return: A dictionary of DICOM file information.
-        :rtype: dict
-        """
-        dicom_info = {}
-        for filename in os.listdir(dicom_dir):
-            full_path = os.path.join(dicom_dir, filename)
-            if self.is_dicom_file(full_path):
-                ds = pydicom.dcmread(full_path)
-                series_number = ds.SeriesNumber if 'SeriesNumber' in ds else None
-                series_description = ds.SeriesDescription if 'SeriesDescription' in ds else None
-                sequence_name = ds.SequenceName if 'SequenceName' in ds else None
-                protocol_name = ds.ProtocolName if 'ProtocolName' in ds else None
-                series_instance_UID = ds.SeriesInstanceUID if 'SeriesInstanceUID' in ds else None
-                if ds.Modality == 'PT':
-                    modality = 'PET'
-                else:
-                    modality = ds.Modality
-
-                if series_number is not None:
-                    base_filename = self.remove_accents(series_number)
-                    if series_description is not None:
-                        anticipated_filename = f"{base_filename}_{self.remove_accents(series_description)}.nii"
-                    elif sequence_name is not None:
-                        anticipated_filename = f"{base_filename}_{self.remove_accents(sequence_name)}.nii"
-                    elif protocol_name is not None:
-                        anticipated_filename = f"{base_filename}_{self.remove_accents(protocol_name)}.nii"
-                else:
-                    anticipated_filename = f"{self.remove_accents(series_instance_UID)}.nii"
-
-                dicom_info[anticipated_filename] = modality
-        return dicom_info
-
-    def rename_nifti_files(self, nifti_dir, dicom_info):
-        """
-        Renames NIfTI files based on DICOM file information.
-
-        :param nifti_dir: The path to the directory containing NIfTI files.
-        :type nifti_dir: str
-        :param dicom_info: A dictionary of DICOM file information.
-        :type dicom_info: dict
-        :return: None
-        """
-        for filename in os.listdir(nifti_dir):
-            if filename.endswith('.nii'):
-                modality = dicom_info.get(filename, '')
-                if modality:
-                    new_filename = f"{modality}_{filename}"
-                    os.rename(os.path.join(nifti_dir, filename), os.path.join(nifti_dir, new_filename))
-                    del dicom_info[filename]
-
-    def split4d(self, nifti_file: str, out_dir: str) -> None:
-        """
-        Splits a 4D NIfTI file into 3D NIfTI files.
-
-        :param nifti_file: The path to the 4D NIfTI file.
-        :type nifti_file: str
-        :param out_dir: The path to the output directory.
-        :type out_dir: str
-        :return: None
-        """
-        split_nifti_files = nib.funcs.four_to_three(nib.funcs.squeeze_image(nib.load(nifti_file)))
-        i = 0
-        for file in split_nifti_files:
-            # vol should be named as vol0000.nii, vol0001.nii, etc.
-
-            nib.save(file, os.path.join(out_dir, 'vol' + str(i).zfill(4) + '.nii.gz'))
-            i += 1
-
-    def convert(self):
+        :param str image_path: Path to the 4D image file.
         """
-        Converts input files to NIfTI format and splits 4D NIfTI files into 3D NIfTI files.
+        try:
+            split_nifti_files = nib.funcs.four_to_three(nib.funcs.squeeze_image(nib.load(image_path)))
+            for i, file in enumerate(split_nifti_files):
+                # file name should start with vol, with 4 digits, using leading zeros (zfill)
+                file_name = 'vol_' + str(i).zfill(4) + '.nii.gz'
+                output_path = os.path.join(self.output_directory, file_name)
+                nib.save(file, output_path)
+        except Exception as e:
+            raise NiftiConverterError(f"Error splitting 4D image: {e}")
+
+    @delayed
+    def _convert_to_nifti_format(self, image_path):
+        try:
+            output_path = os.path.join(self.output_directory, f"{pathlib.Path(image_path).stem}.nii.gz")
+            cmd_to_run = f"{C3D_PATH} {image_path} -o {output_path}"
+            cmd_to_run = cmd_to_run.replace("\n", " ").strip()
+            subprocess.run(cmd_to_run, shell=True, check=True)
+        except Exception as e:
+            raise NiftiConverterError(f"Error converting image to NIFTI: {e}")
 
-        :return: The path to the directory containing the split NIfTI files.
-        :rtype: str
+    def dcm2niix(self, input_path: str, output_dir: str) -> str:
         """
-        if os.path.isdir(self.input_directory):
-            self.non_nifti_to_nifti(self.input_directory, self.output_directory)
-        else:
-            print(f"Input {self.input_directory} is not a directory.")
-            return
+        Converts DICOM files to NIfTI format using dcm2niix.
+
+        Args:
+            input_path (str): The path to the input directory.
+            output_dir (str): The path to the output directory.
+
+        Returns:
+            str: The path to the output directory.
 
-        nifti_files = []
-        for root, dirs, files in os.walk(self.output_directory):
-            for file in files:
-                if file.endswith(('.nii', '.nii.gz')):
-                    nifti_files.append(os.path.join(root, file))
-
-        for file in nifti_files:
-            nifti_image = nib.load(file)
-            if len(nifti_image.shape) == 4:
-                self.split4d(file, self.split_nifti_directory)
-                nifti_files.remove(file)
+        Raises:
+            NiftiConverterError: If there's an error during DICOM to NIFTI conversion.
+        """
+        cmd_to_run: List[str] = [DCM2NIIX_PATH, '-z', 'y', '-o', output_dir, input_path]
+
+        try:
+            subprocess.run(cmd_to_run, capture_output=True, check=True)
+        except subprocess.CalledProcessError:
+            raise NiftiConverterError(f"Error during DICOM to NIFTI conversion using dcm2niix.")
+
+        return output_dir
 
-        if len(nifti_files) == 1:
-            print(" Error: Motion correction cannot be performed on a single 3D image.")
 
-        return self.split_nifti_directory
+class NiftiConverterError(Exception):
+    pass
 
 
 def merge3d(nifti_dir: str, wild_card: str, nifti_outfile: str) -> None:
     """
     Merge 3D NIFTI files into a 4D NIFTI file using nibabel
     :param nifti_dir: Directory containing the 3D NIFTI files
     :param wild_card: Wildcard to use to find the 3D NIFTI files
     :param nifti_outfile: User-defined output file name for the 4D NIFTI file
     """
     logging.info(f"Merging 3D nifti files in {nifti_dir} with wildcard {wild_card}")
     files_to_merge = fop.get_files(nifti_dir, wild_card)
-    nib.save(nib.funcs.concat_images(files_to_merge, False), nifti_outfile)
+    numeric_sorted_files_to_merge = sorted(files_to_merge, key=fop.numeric_sort_key)
+    nib.save(nib.funcs.concat_images(numeric_sorted_files_to_merge, False), nifti_outfile)
     os.chdir(nifti_dir)
     logging.info("Done")
```

### Comparing `falconz-2.0.9/falconz/image_processing.py` & `falconz-2.1.0/falconz/image_processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,35 +10,31 @@
 
 This module handles image processing for the falconz.
 
 Usage:
     The functions in this module can be imported and used in other modules within the falconz to perform image conversion.
 """
 
-import SimpleITK as sitk
 import logging
 import multiprocessing
-import nibabel
 import os
-import pandas as pd
 import pathlib
-import re
 import subprocess
-from dask import delayed, compute
-from halo import Halo
+
+import SimpleITK as sitk
+import pandas as pd
+from dask import delayed
+from dask.distributed import Client, as_completed
+from falconz.constants import GREEDY_PATH, C3D_PATH, NCC_RADIUS, NCC_THRESHOLD, COST_FUNCTION, PROPORTION_OF_CORES
+from falconz.resources import get_system_stats
 from mpire import WorkerPool
-from multiprocessing import Pool
-from nilearn.input_data import NiftiMasker
-from rich.progress import Progress, BarColumn, TextColumn
-from skimage.metrics import structural_similarity as ssim
-from tqdm import tqdm
+from rich.progress import Progress, BarColumn, TimeElapsedColumn
 
 from falconz import constants
 from falconz import file_utilities as fop
-from falconz.constants import GREEDY_PATH, C3D_PATH, NCC_RADIUS, NCC_THRESHOLD, COST_FUNCTION
 
 
 class ImageRegistration:
     """
     A class for performing image registration using the Greedy method.
 
     Attributes:
@@ -74,21 +70,20 @@
         self.moving_img = None
         self.transform_files = None
 
     def set_moving_image(self, moving_img: str, update_transforms: bool = True):
         """
         Sets the moving image for registration and updates the transform files if specified.
 
-        Parameters:
-        -----------
-        moving_img : str
-            Path to the moving/source image.
-        update_transforms : bool, default=True
-            If True, will update the paths for the transformation files based on the moving image name.
+        :param moving_img: Path to the moving/source image.
+        :type moving_img: str
+        :param update_transforms: If True, will update the paths for the transformation files based on the moving image name. Default is True.
+        :type update_transforms: bool
         """
+
         self.moving_img = moving_img
         if update_transforms:
             out_dir = pathlib.Path(self.moving_img).parent
             moving_img_filename = pathlib.Path(self.moving_img).name
             self.transform_files = {
                 'rigid': os.path.join(out_dir, f"{moving_img_filename}_rigid.mat"),
                 'affine': os.path.join(out_dir, f"{moving_img_filename}_affine.mat"),
@@ -101,17 +96,17 @@
         Perform rigid registration between the moving and fixed images.
 
         Returns:
         --------
         str
             Path to the resulting rigid transformation file.
         """
-        mask_cmd = f"-gm {re.escape(self.fixed_mask)}" if self.fixed_mask else ""
-        cmd_to_run = f"{GREEDY_PATH} -d 3 -a -i {re.escape(self.fixed_img)} {re.escape(self.moving_img)} " \
-                     f"{mask_cmd} -ia-image-centers -dof 6 -o {re.escape(self.transform_files['rigid'])} " \
+        mask_cmd = f"-gm {self.fixed_mask}" if self.fixed_mask else ""
+        cmd_to_run = f"{GREEDY_PATH} -d 3 -a -i {self.fixed_img} {self.moving_img} " \
+                     f"{mask_cmd} -ia-image-centers -dof 6 -o {self.transform_files['rigid']} " \
                      f"-n {self.multi_resolution_iterations} -m {COST_FUNCTION}"
         subprocess.run(cmd_to_run, shell=True, capture_output=True)
         logging.info(
             f"Rigid alignment: {pathlib.Path(self.moving_img).name} -> {pathlib.Path(self.fixed_img).name} | Aligned image: "
             f"moco-{pathlib.Path(self.moving_img).name} | Transform file: {pathlib.Path(self.transform_files['rigid']).name}")
         return self.transform_files['rigid']
 
@@ -120,17 +115,17 @@
         Perform affine registration between the moving and fixed images.
 
         Returns:
         --------
         str
             Path to the resulting affine transformation file.
         """
-        mask_cmd = f"-gm {re.escape(self.fixed_mask)}" if self.fixed_mask else ""
-        cmd_to_run = f"{GREEDY_PATH} -d 3 -a -i {re.escape(self.fixed_img)} {re.escape(self.moving_img)} " \
-                     f"{mask_cmd} -ia-image-centers -dof 12 -o {re.escape(self.transform_files['affine'])} " \
+        mask_cmd = f"-gm {self.fixed_mask}" if self.fixed_mask else ""
+        cmd_to_run = f"{GREEDY_PATH} -d 3 -a -i {self.fixed_img} {self.moving_img} " \
+                     f"{mask_cmd} -ia-image-centers -dof 12 -o {self.transform_files['affine']} " \
                      f"-n {self.multi_resolution_iterations} -m {COST_FUNCTION}"
         subprocess.run(cmd_to_run, shell=True, capture_output=True)
         logging.info(
             f"Affine alignment: {pathlib.Path(self.moving_img).name} -> {pathlib.Path(self.fixed_img).name} |"
             f" Aligned image: moco-{pathlib.Path(self.moving_img).name} | Transform file: {pathlib.Path(self.transform_files['affine']).name}")
         return self.transform_files['affine']
 
@@ -140,18 +135,18 @@
 
         Returns:
         --------
         tuple
             A tuple containing paths to the resulting affine, warp, and inverse warp transformation files.
         """
         self.affine()
-        mask_cmd = f"-gm {re.escape(self.fixed_mask)}" if self.fixed_mask else ""
-        cmd_to_run = f"{GREEDY_PATH} -d 3 -m {COST_FUNCTION} -i {re.escape(self.fixed_img)} {re.escape(self.moving_img)} " \
-                     f"{mask_cmd} -it {re.escape(self.transform_files['affine'])} -o {re.escape(self.transform_files['warp'])} " \
-                     f"-oinv {re.escape(self.transform_files['inverse_warp'])} -sv -n {self.multi_resolution_iterations}"
+        mask_cmd = f"-gm {self.fixed_mask}" if self.fixed_mask else ""
+        cmd_to_run = f"{GREEDY_PATH} -d 3 -m {COST_FUNCTION} -i {self.fixed_img} {self.moving_img} " \
+                     f"{mask_cmd} -it {self.transform_files['affine']} -o {self.transform_files['warp']} " \
+                     f"-oinv {self.transform_files['inverse_warp']} -sv -n {self.multi_resolution_iterations}"
         subprocess.run(cmd_to_run, shell=True, capture_output=True)
         logging.info(
             f"Deformable alignment: {pathlib.Path(self.moving_img).name} -> {pathlib.Path(self.fixed_img).name} | "
             f"Aligned image: moco-{pathlib.Path(self.moving_img).name} | "
             f"Initial alignment: {pathlib.Path(self.transform_files['affine']).name}"
             f" | warp file: {pathlib.Path(self.transform_files['warp']).name}")
         return self.transform_files['affine'], self.transform_files['warp'], self.transform_files['inverse_warp']
@@ -217,20 +212,20 @@
             Paths to the transformation files used for resampling.
 
         Returns:
         --------
         str
             The command string to run.
         """
-        cmd = f"{GREEDY_PATH} -d 3 -rf {re.escape(self.fixed_img)} -ri LINEAR -rm " \
-              f"{re.escape(self.moving_img)} {re.escape(resampled_moving_img)}"
+        cmd = f"{GREEDY_PATH} -d 3 -rf {self.fixed_img} -ri LINEAR -rm " \
+              f"{self.moving_img} {resampled_moving_img}"
         if segmentation and resampled_seg:
-            cmd += f" -ri LABEL 0.2vox -rm {re.escape(segmentation)} {re.escape(resampled_seg)}"
+            cmd += f" -ri LABEL 0.2vox -rm {segmentation} {resampled_seg}"
         for transform_file in transform_files:
-            cmd += f" -r {re.escape(transform_file)}"
+            cmd += f" -r {transform_file}"
         return cmd
 
 
 @delayed
 def align_single_image(fixed_img, moving_img, registration_type, multi_resolution_iterations, moco_dir):
     """
     Aligns a single moving image to the fixed image using the specified registration type.
@@ -252,45 +247,52 @@
     aligner.set_moving_image(moving_img)
     aligner.registration(registration_type)
     aligner.resample(resampled_moving_img=os.path.join(moco_dir, constants.MOCO_PREFIX + os.path.basename(moving_img)),
                      registration_type=registration_type)
     return 1
 
 
-def align(fixed_img=str, moving_imgs=list, registration_type=str, multi_resolution_iterations=str, moco_dir=str):
-    """
-    Aligns the moving images to the fixed image using the specified registration type.
-
-    :param fixed_img: The path to the fixed image.
-    :type fixed_img: str
-    :param moving_imgs: A list of paths to the moving images.
-    :type moving_imgs: list
-    :param registration_type: The type of registration to use.
-    :type registration_type: str
-    :param multi_resolution_iterations: The number of iterations to use for multi-resolution registration.
-    :type multi_resolution_iterations: str
-    :param moco_dir: The directory to store the resampled moving images.
-    :type moco_dir: str
-    """
-    tasks = [
-        align_single_image(fixed_img, moving_img, registration_type, multi_resolution_iterations, moco_dir)
-        for moving_img in moving_imgs
-    ]
+def align(fixed_img, moving_imgs, registration_type, multi_resolution_iterations, moco_dir):
+    # Configuring Dask Client
+    num_cores = max(1, int(multiprocessing.cpu_count() * PROPORTION_OF_CORES))
+    client = Client(n_workers=num_cores, threads_per_worker=1)
 
     total_images = len(moving_imgs)
 
-    # Initialize the progress bar
-    with Progress() as progress:
-        task_description = f"[cyan] Aligning moving images to the reference frame [0/{total_images}]"
-        task = progress.add_task(task_description, total=total_images)
-
-        # Using dask to compute results and update the progress bar
-        for count, _ in enumerate(compute(*tasks), 1):
-            progress.update(task, advance=1,
-                            description=f"[cyan] Aligning moving images to the reference frame [{count}/{total_images}]")
+    # Define tasks outside of the progress context so that the progress bar appears first
+    tasks = [align_single_image(fixed_img, moving_img, registration_type, multi_resolution_iterations, moco_dir)
+             for moving_img in moving_imgs]
+
+    with Progress(
+            "[progress.description]{task.description}",
+            "[progress.percentage]{task.percentage:>3.0f}%",
+            BarColumn(),
+            "[{task.completed}/{task.total}]",
+            "• Time elapsed:",
+            TimeElapsedColumn(),
+            "• CPU Load: [cyan]{task.fields[cpu]}%",  # Adding CPU Load
+            "• Memory Load: [cyan]{task.fields[memory]}%"  # Adding Memory Load
+    ) as progress:
+        task_description = "[cyan] Aligning moving images..."
+        cpu_percent, memory_percent = get_system_stats()  # Initial CPU and Memory stats
+
+        task_id = progress.add_task(task_description, total=total_images,
+                                    cpu=cpu_percent, memory=memory_percent)  # Add them to the task fields
+
+        futures = client.compute(tasks)
+
+        # Update progress bar as tasks complete
+        for future, result in as_completed(futures, with_results=True):
+            cpu_percent, memory_percent = get_system_stats()  # Get updated stats
+            progress.update(task_id, advance=1,
+                            description="[cyan] Aligned moving images:",
+                            cpu=cpu_percent, memory=memory_percent)  # Update the task with the new stats
+
+    # Close the client to release resources after computation
+    client.close()
 
 
 def get_dimensions(nifti_file: str) -> int:
     """
     Get the dimensions of a NIFTI image file.
 
     :param nifti_file: The path to the NIFTI file.
@@ -336,53 +338,14 @@
                    intensity_statistics.GetMedian(i), intensity_statistics.GetMaximum(i),
                    intensity_statistics.GetMinimum(i)) for i in intensity_statistics.GetLabels()]
     columns = ['Mean', 'Standard Deviation', 'Median', 'Maximum', 'Minimum']
     stats_df = pd.DataFrame(data=stats_list, index=intensity_statistics.GetLabels(), columns=columns)
     return stats_df
 
 
-def get_body_mask(nifti_file: str, mask_file: str) -> str:
-    """
-    Get a mask file for a NIFTI image file.
-    
-    :param nifti_file: The path to the NIFTI file.
-    :type nifti_file: str
-    :param mask_file: The path to save the mask file.
-    :type mask_file: str
-    :return: The path to the mask file.
-    :rtype: str
-    """
-    nifti_masker = NiftiMasker(mask_strategy='epi', memory="nilearn_cache", memory_level=2, smoothing_fwhm=8)
-    nifti_masker.fit(nifti_file)
-    nibabel.save(nifti_masker.mask_img_, mask_file)
-    return mask_file
-
-
-def mask_img(nifti_file: str, mask_file: str, masked_file: str) -> str:
-    """
-    Mask a NIFTI image file with a mask file.
-    
-    :param nifti_file: The path to the NIFTI file.
-    :type nifti_file: str
-    :param mask_file: The path to the mask file.
-    :type mask_file: str
-    :param masked_file: The path to save the masked NIFTI file.
-    :type masked_file: str
-    :return: The path to the masked NIFTI file.
-    :rtype: str
-    """
-    img = sitk.ReadImage(nifti_file)
-    mask = sitk.ReadImage(mask_file, sitk.sitkFloat32)
-    masked_img = sitk.Compose(
-        [sitk.Multiply(sitk.VectorIndexSelectionCast(img, i), mask) for i in
-         range(img.GetNumberOfComponentsPerPixel())])
-    sitk.WriteImage(sitk.Cast(masked_img, sitk.sitkVectorFloat32), masked_file)
-    return masked_file
-
-
 def downscale_image(downscale_param: tuple, input_image: str) -> str:
     """
     Downscale an image based on the shrink factor and save it to the output directory.
     
     :param downscale_param: A tuple containing the output directory (str) and shrink factor (int).
     :type downscale_param: tuple
     :param input_image: The path to the input image.
@@ -392,22 +355,22 @@
     """
     output_dir, shrink_factor = downscale_param
     input_image_name = os.path.basename(input_image)
     # Blur the input image first
     input_image_blurred = os.path.join(output_dir, f"{shrink_factor}x_blurred_{input_image_name}")
     gauss_variance = (shrink_factor / 2) ** 2
     gauss_variance = int(gauss_variance)
-    cmd_to_smooth = f"{C3D_PATH} {re.escape(input_image)} -smooth-fast {gauss_variance}x{gauss_variance}x{gauss_variance}vox -o" \
-                    f" {re.escape(input_image_blurred)} "
+    cmd_to_smooth = f"{C3D_PATH} {input_image} -smooth-fast {gauss_variance}x{gauss_variance}x{gauss_variance}vox -o" \
+                    f" {input_image_blurred} "
     subprocess.run(cmd_to_smooth, shell=True, capture_output=False)
     # Resample the smoothed input image later
     input_image_downscaled = os.path.join(output_dir, f"{shrink_factor}x_downscaled_{input_image_name}")
     shrink_percentage = str(int(100 / shrink_factor))
-    cmd_to_downscale = f"{C3D_PATH} {re.escape(input_image_blurred)} -resample {shrink_percentage}x{shrink_percentage}x" \
-                       f"{shrink_percentage}% -o {re.escape(input_image_downscaled)}"
+    cmd_to_downscale = f"{C3D_PATH} {input_image_blurred} -resample {shrink_percentage}x{shrink_percentage}x" \
+                       f"{shrink_percentage}% -o {input_image_downscaled}"
     subprocess.run(cmd_to_downscale, shell=True, capture_output=False)
     return input_image_downscaled
 
 
 # Calculate the mean intensity of an image using SimpleITK
 def calc_mean_intensity(image: str) -> float:
     """
@@ -433,18 +396,18 @@
     :return: The path to the voxelwise ncc image.
     :rtype: str
     """
     # get the image names without the extension '.nii.gz'
     image1_name = os.path.basename(image1).split(".")[0]
     image2_name = os.path.basename(image2).split(".")[0]
     output_image = os.path.join(output_dir, f"ncc_{image2_name}.nii.gz")
-    c3d_cmd = f"{C3D_PATH} {re.escape(image1)} {re.escape(image2)} -ncc {NCC_RADIUS} -o {re.escape(output_image)}"
+    c3d_cmd = f"{C3D_PATH} {image1} {image2} -ncc {NCC_RADIUS} -o {output_image}"
     subprocess.run(c3d_cmd, shell=True, capture_output=False)
     # clip the negative correlations to zero
-    c3d_cmd = f"{C3D_PATH} {re.escape(output_image)} -clip 0 inf -o {re.escape(output_image)}"
+    c3d_cmd = f"{C3D_PATH} {output_image} -clip 0 inf -o {output_image}"
     subprocess.run(c3d_cmd, shell=True, capture_output=False)
     return output_image
 
 
 def determine_candidate_frames(candidate_files: list, reference_file: str, output_dir: str, njobs: int) -> int:
     """
     Determines the candidate frames of a 4D PET series on which motion correction can be performed effectively
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `falconz-2.0.9/falconz/input_validation.py` & `falconz-2.1.0/falconz/input_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 Usage:
     The functions in this module can be imported and used in other modules within the falconz to perform image conversion.
 """
 import logging
 import os
 
+from falconz.constants import ALLOWED_MODES
+
 
 class InputValidation:
     """
     A class for input validation for the falconz.
 
     :param args: The arguments to validate.
     :type args: Any
@@ -33,22 +35,23 @@
         Validates the input arguments.
         """
         self._check_directory_exists()
         self._check_reference_frame_index()
         self._check_start_frame()
         self._check_registration_type()
         self._check_multi_resolution_iterations()
+        self._check_operation_mode()
         logging.info("Input validation successful.")
 
     def _check_directory_exists(self):
         """
         Checks if the specified directory exists.
         """
-        if not os.path.exists(self.args.main_folder):
-            raise ValueError(f"The specified directory does not exist: {self.args.main_folder}")
+        if not os.path.exists(self.args.directory):
+            raise ValueError(f"The specified directory does not exist: {self.args.directory}")
 
     def _check_reference_frame_index(self):
         """
         Checks if the reference frame index is valid.
         """
         if not isinstance(self.args.reference_frame_index, int) or self.args.reference_frame_index < -1:
             raise ValueError(
@@ -73,7 +76,14 @@
         """
         Checks if the multi-resolution iterations are valid.
         """
         if not isinstance(self.args.multi_resolution_iterations, str) or not all(
                 i.isdigit() for i in self.args.multi_resolution_iterations.split('x')):
             raise ValueError(
                 f"Multi resolution iterations must be a 'x' separated numeric string: {self.args.multi_resolution_iterations}")
+
+    def _check_operation_mode(self):
+        """
+        Checks if the operation mode is valid.
+        """
+        if self.args.mode not in ALLOWED_MODES:
+            raise ValueError(f"Invalid operation mode. Allowed values are: {ALLOWED_MODES}")
```

### Comparing `falconz-2.0.9/setup.py` & `falconz-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falconz',
-    version='2.0.9',
+    version='2.1.0',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='FalconZ: A streamlined Python package for PET motion correction.',
-    python_requires='>=3.9',
+    python_requires='>=3.10',
     long_description='FalconZ is a robust and comprehensive Python package that offers a simplified approach to PET ('
                      'Positron Emission Tomography) motion correction. The software is equipped to handle both head '
                      'and total-body scans, ensuring high-accuracy results in diverse settings. Built around the '
                      'potent greedy registration toolkit, FalconZ serves as an efficient engine for registration '
                      'tasks, providing precise alignment in PET imaging. The package has been designed with '
                      'user-friendliness in mind, streamlining the implementation process of motion correction. '
                      'Whether you are a researcher, healthcare professional, or an individual working with PET scans, '
@@ -35,32 +35,32 @@
     packages=find_packages(),
     install_requires=[
         'nibabel~=3.2.2',
         'halo~=0.0.31',
         'SimpleITK~=2.2.1',
         'pydicom~=2.2.2',
         'argparse~=1.4.0',
-        'numpy~=1.22.3',
+        'numpy~=1.25.2',
         'mpire~=2.3.3',
         'openpyxl~=3.0.9',
         'matplotlib',
         'pyfiglet~=0.8.post1',
         'natsort~=8.1.0',
         'pillow>=9.2.0',
         'colorama~=0.4.6',
         'rich',
         'pandas',
         'dicom2nifti~=2.4.8',
         'requests',
         'emoji',
         'psutil',
-        'dcm2niix',
         'nilearn',
         'scikit-image',
-        'dask'
+        'dask',
+        'dask[distributed]'
     ],
     entry_points={
         'console_scripts': [
             'falconz=falconz.falconz:main',
         ],
     },
 )
```

